# Comparing `tmp/checkpoint_tool-0.2.2.tar.gz` & `tmp/checkpoint_tool-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.2.2.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.3.0.tar", max compression
```

## Comparing `checkpoint_tool-0.2.2.tar` & `checkpoint_tool-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3284 2023-04-27 00:07:20.584363 checkpoint_tool-0.2.2/README.md
--rw-r--r--   0        0        0    14982 2023-04-27 00:15:06.991294 checkpoint_tool-0.2.2/checkpoint.py
--rw-r--r--   0        0        0      644 2023-04-27 00:15:28.015718 checkpoint_tool-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 checkpoint_tool-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3308 2023-04-27 00:24:50.167733 checkpoint_tool-0.3.0/README.md
+-rw-r--r--   0        0        0    15489 2023-04-27 00:45:24.936478 checkpoint_tool-0.3.0/checkpoint.py
+-rw-r--r--   0        0        0      644 2023-04-27 00:46:57.918529 checkpoint_tool-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4087 1970-01-01 00:00:00.000000 checkpoint_tool-0.3.0/PKG-INFO
```

### Comparing `checkpoint_tool-0.2.2/README.md` & `checkpoint_tool-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,30 +35,30 @@
 
     # Return function that produces a value instead of the value itself.
     return run_task
 
 # Build the task graph to compute `choose(6, 3)`
 # and greedily consume it with `concurrent.futures.ProcessPoolExecutor`
 # (i.e., as parallel as possible).
-# The cache is stored at `$CP_CACHE_DIR/checkpoint/{module_name}.{function_name}/...`
+# The cache is stored at `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{function_name}/...`
 # and reused whenever available.
 ans = choose(6, 3).run()
 ```
 
 It is possible to selectively discard cache: 
 ```python
 # After some modificaiton of `choose(3, 3)`,
 # selectively discard the cache corresponding to the modification.
 choose(3, 3).clear()
 
 # `ans` is recomputed tracing back to the computation of `choose(3, 3)`.
 ans = choose(6, 3).run()
 
 # Delete all the cache associated with `choose`,
-# equivalent to `rm -r $CP_CACHE_DIR/checkpoint/{module_name}.choose`.
+# equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.choose`.
 choose.clear()            
 ```
 
 More complex inputs can be used as long as it is JSON serializable:
 ```python
 @task
 def task1(**param1):
```

### Comparing `checkpoint_tool-0.2.2/checkpoint.py` & `checkpoint_tool-0.3.0/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Callable, Generic, NewType, Type, TypeVar, Any, cast, overload
 from typing_extensions import ParamSpec, Concatenate, Self
 import os
 from pathlib import Path
+import copy
 
 import logging
 import cloudpickle
 import zlib
 import diskcache as dc
 
 from concurrent.futures import ProcessPoolExecutor, Future, wait, FIRST_COMPLETED, Executor
@@ -123,19 +124,19 @@
     def get_result(self) -> R:
         db = self.task_factory.db
         return db.load(self.key)
 
     def run(self, *, executor: Executor | None = None) -> R:
         return self.run_with_info(executor=executor)[0]
 
-    def run_with_info(self, *, executor: Executor | None = None) -> tuple[R, dict[str, Any]]:
+    def run_with_info(self, *, executor: Executor | None = None, dump_generations: bool = False) -> tuple[R, dict[str, Any]]:
         graph = Graph.build(self)
         if executor is None:
             executor = ProcessPoolExecutor()
-        info = run_task_graph(graph=graph, executor=executor)
+        info = run_task_graph(graph=graph, executor=executor, dump_generations=dump_generations)
         return self.get_result(), info
 
     def clear(self) -> None:
         db = self.task_factory.db
         db.delete(self.key)
 
     def to_tuple(self) -> tuple[str, Json]:
@@ -198,15 +199,15 @@
     params = inspect.signature(fn).bind(*args, **kwargs)
     params.apply_defaults()
     return params.arguments
 
 
 def _serialize_arguments(fn: Callable[P, Any], *args: P.args, **kwargs: P.kwargs) -> Json:
     arguments = _normalize_arguments(fn, *args, **kwargs)
-    return cast(Json, json.dumps(arguments))
+    return cast(Json, json.dumps(arguments, separators=(',', ':'), sort_keys=True))
 
 
 AnyTask = Task[Any]
 Connector = Callable[[Callable[Concatenate[T, P], R]], Callable[P, R]]  # Takes (T, *P) -> R and return P -> R
 
 
 @overload
@@ -332,17 +333,19 @@
         g = to_expand.pop()
         if g.timestamp is None:
             out.append(g)
             to_expand.extend(g.upstream_graphs)
     return out
 
 
-def run_task_graph(graph: Graph, executor: Executor) -> dict[str, Any]:
+def run_task_graph(graph: Graph, executor: Executor, dump_generations: bool = False) -> dict[str, Any]:
     """ Consume task graph concurrently.
     """
+    info = {'stats': {}, 'generations': []}
+
     active_subgraphs = walk_subgraph_to_update(graph)
 
     # Parse graph in a flat format
     Key = tuple[str, Json]
     nodes: dict[Key, AnyTask] = {g.root.to_tuple(): g.root for g in active_subgraphs}
     task_factories: dict[str, TaskFactory[..., Any]] = {k[0]: nodes[k].task_factory for k in nodes}
 
@@ -373,14 +376,15 @@
         if path not in node_groups:
             node_groups[path] = {arg_key}
         else:
             node_groups[path].add(arg_key)
 
     stats = {k: len(args) for k, args in node_groups.items()}
     LOGGER.info(f'Following tasks will be called: {stats}')
+    info['stats'] = stats
 
     # Read concurrency budgets
     budgets: dict[str, int] = {}
     occupied: dict[str, int] = {}
     for path in node_groups:
         mc = task_factories[path].max_concurrency
         if mc is not None:
@@ -393,17 +397,20 @@
             for path, keys in node_groups.items()
             }
 
     # Execute tasks
     with executor as executor:
         in_process: set[Future[Key]] = set()
         while leaves or in_process:
+            # Log some stats
             LOGGER.info(
-                    f'desc: {len(descendants)}, prec: {len(precedents)}, leaves: {len(leaves)}, in_process: {len(in_process)}'
+                    f'nodes: {len(nodes)}, desc: {len(descendants)}, prec: {len(precedents)}, leaves: {len(leaves)}, in_process: {len(in_process)}'
                     )
+            if dump_generations:
+                info['generations'].append(copy.deepcopy(node_groups))
 
             # Submit all leaf tasks
             leftover: dict[str, list[Json]] = {}
             for path, keys in leaves.items():
                 if path in budgets:
                     free = budgets[path] - occupied[path]
                     to_submit, to_hold = keys[:free], keys[free:]
@@ -429,32 +436,35 @@
                 path = done_task[0]
                 if path in occupied:
                     occupied[path] -= 1
                     assert occupied[path] >= 0
 
                 # Remove node from graph
                 nodes.pop(done_task)
+                node_groups[path].remove(done_task[1])
+                if not node_groups[path]:
+                    del node_groups[path]
                 assert not precedents.pop(done_task)
                 next_tasks = descendants.pop(done_task)
 
-                # update precedents and leaves
+                # Update leaves
                 for next_task in next_tasks:
                     precs = precedents[next_task]
                     precs.remove(done_task)
                     if not precs:
                         path_next, key_next = next_task
                         if path_next not in leaves:
                             leaves[path_next] = [key_next]
                         else:
                             leaves[path_next].append(key_next)
 
     # Sanity check
-    assert not nodes and not descendants and not precedents, f'Graph is not empty. Should not happen.'
+    assert not nodes and not descendants and not precedents and not node_groups, f'Graph is not empty. Should not happen.'
     assert all(n == 0 for n in occupied.values()), 'Incorrect task count. Should not happen.'
-    return {'stats': stats}
+    return info
 
 
 def _run_task(task_data: bytes) -> tuple[str, Json]:
     task = cloudpickle.loads(task_data)
     assert isinstance(task, Task)
     task.set_result()
     return task.to_tuple()
```

### Comparing `checkpoint_tool-0.2.2/pyproject.toml` & `checkpoint_tool-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.2.2"
+version = "0.3.0"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint.py"}]
```

### Comparing `checkpoint_tool-0.2.2/PKG-INFO` & `checkpoint_tool-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.2.2
+Version: 0.3.0
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -55,30 +55,30 @@
 
     # Return function that produces a value instead of the value itself.
     return run_task
 
 # Build the task graph to compute `choose(6, 3)`
 # and greedily consume it with `concurrent.futures.ProcessPoolExecutor`
 # (i.e., as parallel as possible).
-# The cache is stored at `$CP_CACHE_DIR/checkpoint/{module_name}.{function_name}/...`
+# The cache is stored at `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{function_name}/...`
 # and reused whenever available.
 ans = choose(6, 3).run()
 ```
 
 It is possible to selectively discard cache: 
 ```python
 # After some modificaiton of `choose(3, 3)`,
 # selectively discard the cache corresponding to the modification.
 choose(3, 3).clear()
 
 # `ans` is recomputed tracing back to the computation of `choose(3, 3)`.
 ans = choose(6, 3).run()
 
 # Delete all the cache associated with `choose`,
-# equivalent to `rm -r $CP_CACHE_DIR/checkpoint/{module_name}.choose`.
+# equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.choose`.
 choose.clear()            
 ```
 
 More complex inputs can be used as long as it is JSON serializable:
 ```python
 @task
 def task1(**param1):
```


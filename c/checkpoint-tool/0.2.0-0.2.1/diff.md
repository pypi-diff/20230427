# Comparing `tmp/checkpoint_tool-0.2.0.tar.gz` & `tmp/checkpoint_tool-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.2.0.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.2.1.tar", max compression
```

## Comparing `checkpoint_tool-0.2.0.tar` & `checkpoint_tool-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2154 2023-04-26 14:37:43.238128 checkpoint_tool-0.2.0/README.md
--rw-r--r--   0        0        0    14649 2023-04-26 14:37:43.238625 checkpoint_tool-0.2.0/checkpoint.py
--rw-r--r--   0        0        0      637 2023-04-26 15:03:30.414021 checkpoint_tool-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 checkpoint_tool-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3105 2023-04-26 15:05:18.499592 checkpoint_tool-0.2.1/README.md
+-rw-r--r--   0        0        0    14649 2023-04-26 14:37:43.238625 checkpoint_tool-0.2.1/checkpoint.py
+-rw-r--r--   0        0        0      637 2023-04-26 15:05:42.006422 checkpoint_tool-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3877 1970-01-01 00:00:00.000000 checkpoint_tool-0.2.1/PKG-INFO
```

### Comparing `checkpoint_tool-0.2.0/checkpoint.py` & `checkpoint_tool-0.2.1/checkpoint.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.2.0/pyproject.toml` & `checkpoint_tool-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.2.0"
+version = "0.2.1"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint.py"}]
```

### Comparing `checkpoint_tool-0.2.0/PKG-INFO` & `checkpoint_tool-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: checkpoint-tool
-Version: 0.2.0
-Summary: A lightweight workflow management tool written in pure Python
-Home-page: https://github.com/koheimiya/checkpoint
-License: MIT
-Author: Kohei Miyaguchi
-Author-email: koheimiyaguchi@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dill (>=0.3.6,<0.4.0)
-Requires-Dist: diskcache (>=5.6.1,<6.0.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Project-URL: Repository, https://github.com/koheimiya/checkpoint
-Description-Content-Type: text/markdown
-
 # Checkpoint-tool
 A lightweight workflow management tool written in pure Python.
 
 Internally, it depends on `DiskCache`, `dill` and `concurrent.futures`.
 
 
 ### Installation
@@ -30,29 +10,38 @@
 ```
 
 ### Usage
 Create task with decorators:
 ```python
 from checkpoint import task, requires
 
-@task  # Mark a function as task
+# Mark a function as task
+@task
 def choose(n: int, k: int):
     if 0 < k < n:
-        @requires([choose(n - 1, k - 1), choose(n - 1, k)])  # Dependency
-        def run_task(prev_two: list[int]):
-            return sum(prev_two)
+        # Mark dependencies on other tasks;
+        # The return values of these tasks are passed as the arguments.
+        @requires(choose(n - 1, k - 1))
+        @requires(choose(n - 1, k)) 
+        def run_task(prev1: int, prev2: int) -> int:
+            # Main computation
+            return prev1 + prev2
     elif k == 0 or k == n:
+        # Dependency can change according to the task parameters (`n` and `k`).
+        # Here, we need no dependency to compute `choose(n, 1)` or `choose(n, n)`.
         def run_task() -> int:
             return 1
     else:
         raise ValueError(f'{(n, k)}')
     return run_task
 
-# Build the task graph to compute the return value of choose(6, 3) and consume it in parallel whenever possible.
-# The cache is stored at `$CP_CACHE_DIR/checkpoint/{module_name}.choice/...` and reused whenever available.
+# Build the task graph to compute the return value of choose(6, 3)
+# and greedily consume it with `concurrent.futures.ProcessPoolExecutor` (i.e., in parallel as far as possible).
+# The cache is stored at `$CP_CACHE_DIR/checkpoint/{module_name}.choice/...`
+# and reused whenever available.
 ans = choose(6, 3).run()
 ```
 
 It is possible to selectively discard cache: 
 ```python
 ### after some modificaiton of choose(3, 3) ...
 choose(3, 3).clear()      # selectively discard the cache corresponding to the modification
@@ -77,32 +66,45 @@
     def run_task(result1, result2):
         ...
     return run_task
 
 result = task3({'param1': { ... }, 'param2': { ... }}).run()
 ```
 
-Large outputs can be stored with compression:
+Task dependencies can be also specified with lists and dicts.
 ```python
-@task(compress=True)
+@task
+def task3(params):
+    @requires([task1(p) for p in params['my_param_list']])
+    @requires({k: task2(p) for k, p in params['my_param_dict'].items()})
+    def run_task(result_list, result_dict):
+        ...
+    return run_task
+
+result = task3({'my_param_list': [ ... ], 'my_param_dict': { ... }}).run()
+```
+
+Large outputs can be stored with compression via `zlib`:
+```python
+@task(compress_level=6)
 def large_output_task(*args, **kwargs):
     ...
 ```
 
-One can limit the task execution with `concurrent.futures.Executor`:
+One can control the task execution with `concurrent.futures.Executor` class:
 ```python
-from concurrent.futures import ProcessPoolExecutor
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
 @task
 def my_task():
     ...
 
-my_task().run(executor=ProcessPoolExecutor(max_workers=2))
+my_task().run(executor=ProcessPoolExecutor(max_workers=2))  # Limit the number of parallel workers
+my_task().run(executor=ThreadPoolExecutor())                # Thread-based parallelism
 ```
 
-One can also control the task-wise concurrency:
+One can also control the concurrency at a task level:
 ```python
 @task(max_concurrency=2)
 def resource_intensive_task(*args, **kwargs):
     ...
 ```
-
```


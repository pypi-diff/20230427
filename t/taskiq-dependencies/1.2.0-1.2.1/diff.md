# Comparing `tmp/taskiq_dependencies-1.2.0.tar.gz` & `tmp/taskiq_dependencies-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_dependencies-1.2.0.tar", max compression
+gzip compressed data, was "taskiq_dependencies-1.2.1.tar", max compression
```

## Comparing `taskiq_dependencies-1.2.0.tar` & `taskiq_dependencies-1.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3539 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/README.md
--rw-r--r--   0        0        0     1621 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      386 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/__init__.py
--rw-r--r--   0        0        0     9648 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/ctx.py
--rw-r--r--   0        0        0     3189 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/dependency.py
--rw-r--r--   0        0        0     7257 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/graph.py
--rw-r--r--   0        0        0        0 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/py.typed
--rw-r--r--   0        0        0      573 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/utils.py
--rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 taskiq_dependencies-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4801 2023-04-26 19:56:44.721008 taskiq_dependencies-1.2.1/README.md
+-rw-r--r--   0        0        0     1621 2023-04-26 19:56:44.721008 taskiq_dependencies-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      386 2023-04-26 19:56:44.721008 taskiq_dependencies-1.2.1/taskiq_dependencies/__init__.py
+-rw-r--r--   0        0        0    11507 2023-04-26 19:56:44.721008 taskiq_dependencies-1.2.1/taskiq_dependencies/ctx.py
+-rw-r--r--   0        0        0     3189 2023-04-26 19:56:44.721008 taskiq_dependencies-1.2.1/taskiq_dependencies/dependency.py
+-rw-r--r--   0        0        0     7669 2023-04-26 19:56:44.721008 taskiq_dependencies-1.2.1/taskiq_dependencies/graph.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:56:44.721008 taskiq_dependencies-1.2.1/taskiq_dependencies/py.typed
+-rw-r--r--   0        0        0      573 2023-04-26 19:56:44.721008 taskiq_dependencies-1.2.1/taskiq_dependencies/utils.py
+-rw-r--r--   0        0        0     5933 1970-01-01 00:00:00.000000 taskiq_dependencies-1.2.1/PKG-INFO
```

### Comparing `taskiq_dependencies-1.2.0/README.md` & `taskiq_dependencies-1.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -121,7 +121,58 @@
 
 with graph.sync_ctx() as ctx:
     print(ctx.resolve_kwargs())
 
 ```
 
 The ParamInfo has the information about name and parameters signature. It's useful if you want to create a dependency that changes based on parameter name, or signature.
+
+
+## Exception propagation
+
+By default if error happens within the context, we send this error to the dependency,
+so you can close it properly. You can disable this functionality by setting `exception_propagation` parameter to `False`.
+
+Let's imagine that you want to get a database session from pool and commit after the function is done.
+
+
+```python
+async def get_session():
+    session = sessionmaker()
+
+    yield session
+
+    await session.commit()
+
+```
+
+But what if the error happened when the dependant function was called? In this case you want to rollback, instead of commit.
+To solve this problem, you can just wrap the `yield` statement in `try except` to handle the error.
+
+```python
+async def get_session():
+    session = sessionmaker()
+
+    try:
+        yield session
+    except Exception:
+        await session.rollback()
+        return
+
+    await session.commit()
+
+```
+
+**Also, as a library developer, you can disable exception propagation**. If you do so, then no exception will ever be propagated to dependencies and no such `try except` expression will ever work.
+
+
+Example of disabled propogation.
+
+```python
+
+graph = DependencyGraph(target_func)
+
+with graph.sync_ctx(exception_propagation=False) as ctx:
+    print(ctx.resolve_kwargs())
+
+
+```
```

### Comparing `taskiq_dependencies-1.2.0/pyproject.toml` & `taskiq_dependencies-1.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-dependencies"
-version = "1.2.0"
+version = "1.2.1"
 description = "FastAPI like dependency injection implementation"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 packages = [{include = "taskiq_dependencies"}]
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
```

### Comparing `taskiq_dependencies-1.2.0/taskiq_dependencies/ctx.py` & `taskiq_dependencies-1.2.1/taskiq_dependencies/ctx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import asyncio
 import inspect
 from copy import copy
+from logging import getLogger
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional
 
 from taskiq_dependencies.utils import ParamInfo
 
 if TYPE_CHECKING:
     from taskiq_dependencies.graph import DependencyGraph  # pragma: no cover
 
 
+logger = getLogger("taskiq.dependencies.ctx")
+
+
 class BaseResolveContext:
     """Base resolver context."""
 
     def __init__(
         self,
         graph: "DependencyGraph",
         initial_cache: Optional[Dict[Any, Any]] = None,
+        exception_propagation: bool = True,
     ) -> None:
         self.graph = graph
         self.opened_dependencies: List[Any] = []
         self.sub_contexts: "List[Any]" = []
         self.initial_cache = initial_cache or {}
+        self.propagate_excs = exception_propagation
 
     def traverse_deps(  # noqa: C901, WPS210
         self,
     ) -> "Generator[DependencyGraph | Any, None, Dict[str, Any]]":
         """
         This function is used to traverse all dependencies and resolve them.
 
@@ -112,26 +118,42 @@
     It uses graph, but it doesn't modify it.
     """
 
     def __enter__(self) -> "SyncResolveContext":
         return self
 
     def __exit__(self, *args: Any) -> None:
-        self.close()
+        self.close(*args)
 
-    def close(self) -> None:
+    def close(self, *args: Any) -> None:  # noqa: C901
         """
         Close all opened dependencies.
 
         This function runs teardown of all dependencies.
+
+        :param args: exception info if any.
         """
+        exception_found = False
+        if args[1] is not None and self.propagate_excs:
+            exception_found = True
         for ctx in self.sub_contexts:
-            ctx.close()
+            ctx.close(*args)
         for dep in reversed(self.opened_dependencies):
             if inspect.isgenerator(dep):
+                if exception_found:
+                    try:
+                        dep.throw(*args)
+                    except BaseException as exc:
+                        logger.warning(
+                            "Exception found on dependency teardown %s",
+                            exc,
+                            exc_info=True,
+                        )
+                        continue
+                    continue
                 for _ in dep:  # noqa: WPS328
                     pass  # noqa: WPS420
 
     def resolver(self, executed_func: Any, initial_cache: Dict[Any, Any]) -> Any:
         """
         Sync resolver.
 
@@ -197,29 +219,56 @@
     It uses graph, but it doesn't modify it.
     """
 
     async def __aenter__(self) -> "AsyncResolveContext":
         return self
 
     async def __aexit__(self, *args: Any) -> None:
-        await self.close()
+        await self.close(*args)
 
-    async def close(self) -> None:  # noqa: C901
+    async def close(self, *args: Any) -> None:  # noqa: C901
         """
         Close all opened dependencies.
 
         This function runs teardown of all dependencies.
+
+        :param args: exception info if any.
         """
+        exception_found = False
+        if args[1] is not None and self.propagate_excs:
+            exception_found = True
         for ctx in self.sub_contexts:
-            await ctx.close()  # type: ignore
+            await ctx.close(*args)  # type: ignore
         for dep in reversed(self.opened_dependencies):
             if inspect.isgenerator(dep):
+                if exception_found:
+                    try:
+                        dep.throw(*args)
+                    except BaseException as exc:
+                        logger.warning(
+                            "Exception found on dependency teardown %s",
+                            exc,
+                            exc_info=True,
+                        )
+                        continue
+                    continue
                 for _ in dep:  # noqa: WPS328
                     pass  # noqa: WPS420
             elif inspect.isasyncgen(dep):
+                if exception_found:
+                    try:
+                        await dep.athrow(*args)
+                    except BaseException as exc:
+                        logger.warning(
+                            "Exception found on dependency teardown %s",
+                            exc,
+                            exc_info=True,
+                        )
+                        continue
+                    continue
                 async for _ in dep:  # noqa: WPS328
                     pass  # noqa: WPS420
 
     async def resolver(self, executed_func: Any, initial_cache: Dict[Any, Any]) -> Any:
         """
         Async resolver.
```

### Comparing `taskiq_dependencies-1.2.0/taskiq_dependencies/dependency.py` & `taskiq_dependencies-1.2.1/taskiq_dependencies/dependency.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.0/taskiq_dependencies/graph.py` & `taskiq_dependencies-1.2.1/taskiq_dependencies/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,43 +37,51 @@
         :return: True if depends.
         """
         return len(self.ordered_deps) <= 1
 
     def async_ctx(
         self,
         initial_cache: Optional[Dict[Any, Any]] = None,
+        exception_propagation: bool = True,
     ) -> AsyncResolveContext:
         """
         Create dependency resolver context.
 
         This context is used to actually resolve dependencies.
 
         :param initial_cache: initial cache dict.
+        :param exception_propagation: If true, all found errors within
+            context will be propagated to dependencies.
         :return: new resolver context.
         """
         return AsyncResolveContext(
             self,
             initial_cache,
+            exception_propagation,
         )
 
     def sync_ctx(
         self,
         initial_cache: Optional[Dict[Any, Any]] = None,
+        exception_propagation: bool = True,
     ) -> SyncResolveContext:
         """
         Create dependency resolver context.
 
         This context is used to actually resolve dependencies.
 
         :param initial_cache: initial cache dict.
+        :param exception_propagation: If true, all found errors within
+            context will be propagated to dependencies.
         :return: new resolver context.
         """
         return SyncResolveContext(
             self,
             initial_cache,
+            exception_propagation,
         )
 
     def _build_graph(self) -> None:  # noqa: C901, WPS210
         """
         Builds actual graph.
 
         This function collects all dependencies
```

### Comparing `taskiq_dependencies-1.2.0/taskiq_dependencies/utils.py` & `taskiq_dependencies-1.2.1/taskiq_dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.0/PKG-INFO` & `taskiq_dependencies-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-dependencies
-Version: 1.2.0
+Version: 1.2.1
 Summary: FastAPI like dependency injection implementation
 Keywords: taskiq,dependencies,injection,async,DI
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -149,7 +149,58 @@
 with graph.sync_ctx() as ctx:
     print(ctx.resolve_kwargs())
 
 ```
 
 The ParamInfo has the information about name and parameters signature. It's useful if you want to create a dependency that changes based on parameter name, or signature.
 
+
+## Exception propagation
+
+By default if error happens within the context, we send this error to the dependency,
+so you can close it properly. You can disable this functionality by setting `exception_propagation` parameter to `False`.
+
+Let's imagine that you want to get a database session from pool and commit after the function is done.
+
+
+```python
+async def get_session():
+    session = sessionmaker()
+
+    yield session
+
+    await session.commit()
+
+```
+
+But what if the error happened when the dependant function was called? In this case you want to rollback, instead of commit.
+To solve this problem, you can just wrap the `yield` statement in `try except` to handle the error.
+
+```python
+async def get_session():
+    session = sessionmaker()
+
+    try:
+        yield session
+    except Exception:
+        await session.rollback()
+        return
+
+    await session.commit()
+
+```
+
+**Also, as a library developer, you can disable exception propagation**. If you do so, then no exception will ever be propagated to dependencies and no such `try except` expression will ever work.
+
+
+Example of disabled propogation.
+
+```python
+
+graph = DependencyGraph(target_func)
+
+with graph.sync_ctx(exception_propagation=False) as ctx:
+    print(ctx.resolve_kwargs())
+
+
+```
+
```


# Comparing `tmp/alkymi-0.2.0.tar.gz` & `tmp/alkymi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alkymi-0.2.0.tar", last modified: Tue Apr 11 02:18:04 2023, max compression
+gzip compressed data, was "alkymi-0.2.1.tar", last modified: Thu Apr 27 10:26:18 2023, max compression
```

## Comparing `alkymi-0.2.0.tar` & `alkymi-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-11 02:18:04.619157 alkymi-0.2.0/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6028 2023-04-11 02:18:04.619157 alkymi-0.2.0/PKG-INFO
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     3818 2023-04-11 02:15:19.000000 alkymi-0.2.0/README.md
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-11 02:18:04.619157 alkymi-0.2.0/alkymi/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      395 2023-03-07 20:55:52.000000 alkymi-0.2.0/alkymi/__init__.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6808 2023-03-26 09:01:00.000000 alkymi-0.2.0/alkymi/checksums.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     4464 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/config.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)    21794 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/core.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     4855 2023-03-26 08:25:39.000000 alkymi-0.2.0/alkymi/decorators.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)    12242 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/foreach_recipe.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     9063 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/lab.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      124 2022-02-10 21:09:03.000000 alkymi-0.2.0/alkymi/logging.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     3781 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/progress.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        0 2022-06-02 18:56:50.000000 alkymi-0.2.0/alkymi/py.typed
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     9966 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/recipe.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6757 2022-06-02 18:56:50.000000 alkymi-0.2.0/alkymi/recipes.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)    13154 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/serialization.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     1397 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/types.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     2595 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/utils.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      120 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/version.py
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-11 02:18:04.619157 alkymi-0.2.0/alkymi.egg-info/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6028 2023-04-11 02:18:04.000000 alkymi-0.2.0/alkymi.egg-info/PKG-INFO
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      460 2023-04-11 02:18:04.000000 alkymi-0.2.0/alkymi.egg-info/SOURCES.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        1 2023-04-11 02:18:04.000000 alkymi-0.2.0/alkymi.egg-info/dependency_links.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)       49 2023-04-11 02:18:04.000000 alkymi-0.2.0/alkymi.egg-info/requires.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        7 2023-04-11 02:18:04.000000 alkymi-0.2.0/alkymi.egg-info/top_level.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)       38 2023-04-11 02:18:04.619157 alkymi-0.2.0/setup.cfg
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     2077 2023-04-11 02:15:19.000000 alkymi-0.2.0/setup.py
+drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-27 10:26:18.931690 alkymi-0.2.1/
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     1066 2022-06-02 18:56:50.000000 alkymi-0.2.1/LICENSE.md
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     6028 2023-04-27 10:26:18.931690 alkymi-0.2.1/PKG-INFO
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     3818 2023-04-25 18:56:20.000000 alkymi-0.2.1/README.md
+drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-27 10:26:18.931690 alkymi-0.2.1/alkymi/
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)      395 2023-03-07 20:55:52.000000 alkymi-0.2.1/alkymi/__init__.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     6808 2023-03-26 09:01:00.000000 alkymi-0.2.1/alkymi/checksums.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     4464 2023-04-11 02:15:19.000000 alkymi-0.2.1/alkymi/config.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)    22350 2023-04-27 10:26:15.000000 alkymi-0.2.1/alkymi/core.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     4855 2023-03-26 08:25:39.000000 alkymi-0.2.1/alkymi/decorators.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)    12242 2023-04-11 02:15:19.000000 alkymi-0.2.1/alkymi/foreach_recipe.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     9063 2023-04-25 18:56:20.000000 alkymi-0.2.1/alkymi/lab.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)      124 2022-02-10 21:09:03.000000 alkymi-0.2.1/alkymi/logging.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     3781 2023-04-11 02:15:19.000000 alkymi-0.2.1/alkymi/progress.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)        0 2022-06-02 18:56:50.000000 alkymi-0.2.1/alkymi/py.typed
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     9966 2023-04-11 02:15:19.000000 alkymi-0.2.1/alkymi/recipe.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     6757 2022-06-02 18:56:50.000000 alkymi-0.2.1/alkymi/recipes.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)    13154 2023-04-25 18:56:20.000000 alkymi-0.2.1/alkymi/serialization.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     1397 2023-04-25 18:56:20.000000 alkymi-0.2.1/alkymi/types.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     3855 2023-04-27 10:26:15.000000 alkymi-0.2.1/alkymi/utils.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)      120 2023-04-27 10:26:15.000000 alkymi-0.2.1/alkymi/version.py
+drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-27 10:26:18.931690 alkymi-0.2.1/alkymi.egg-info/
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     6028 2023-04-27 10:26:18.000000 alkymi-0.2.1/alkymi.egg-info/PKG-INFO
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)      471 2023-04-27 10:26:18.000000 alkymi-0.2.1/alkymi.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)        1 2023-04-27 10:26:18.000000 alkymi-0.2.1/alkymi.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)       49 2023-04-27 10:26:18.000000 alkymi-0.2.1/alkymi.egg-info/requires.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)        7 2023-04-27 10:26:18.000000 alkymi-0.2.1/alkymi.egg-info/top_level.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)       38 2023-04-27 10:26:18.931690 alkymi-0.2.1/setup.cfg
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     2077 2023-04-25 18:56:20.000000 alkymi-0.2.1/setup.py
```

### Comparing `alkymi-0.2.0/PKG-INFO` & `alkymi-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alkymi
-Version: 0.2.0
+Version: 0.2.1
 Summary: alkymi - Pythonic task automation
 Home-page: https://github.com/MathiasStokholm/alkymi
 Author: Mathias Bøgh Stokholm
 Author-email: mathias.stokholm@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/MathiasStokholm/alkymi/
 Project-URL: Tracker, https://github.com/MathiasStokholm/alkymi/issues
```

### Comparing `alkymi-0.2.0/README.md` & `alkymi-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi/checksums.py` & `alkymi-0.2.1/alkymi/checksums.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi/config.py` & `alkymi-0.2.1/alkymi/config.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi/core.py` & `alkymi-0.2.1/alkymi/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import concurrent.futures
 import typing
 from asyncio import Future, AbstractEventLoop, Task
 from typing import Dict, Tuple, Optional, Any, Coroutine, Union
 
 import networkx as nx
 
-from . import checksums
+from . import checksums, utils
 from .config import ProgressType, AlkymiConfig
 from .foreach_recipe import ForeachRecipe, MappedOutputs, MappedInputs
 from .logging import log
 from .progress import FancyProgress
 from .recipe import Recipe, R
 from .serialization import OutputWithValue
 from .types import Status, ProgressCallback, EvaluateProgress
@@ -344,47 +344,55 @@
         executor = concurrent.futures.ThreadPoolExecutor(max_workers=jobs if jobs > 0 else None)
 
     # Determine the progress type to use - if not provided by caller, use current setting in alkymi's global config
     if progress_type is None:
         progress_type = AlkymiConfig.get().progress_type
     progress = FancyProgress(graph, statuses, recipe) if progress_type == ProgressType.Fancy else None
 
-    # Create the asyncio event loop and set it on the calling thread
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-
-    async def _execute() -> OutputsAndChecksums[R]:
-        # Sort the graph topographically, such that any recipe in the sorted list only depends on earlier recipes
-        # This guarantees that futures only depend on already created futures
-        recipes = list(nx.topological_sort(graph))
-
-        # Create coroutines to evaluate each recipe - then from the top-down, the coroutines will request inputs that
-        # they need from other coroutines, which will be upgraded to tasks
-        # This approach is used to avoid loading outputs for recipes whose outputs are actually unused, because later
-        # recipes are already cached
-        coros_or_tasks: Dict[Recipe, Union[Coroutine, Task]] = {}
-        for _recipe in recipes:
-            # Note that 'schedule()' might mutate 'tasks' once awaited
-            coros_or_tasks[_recipe] = schedule(loop, executor, _recipe, statuses[_recipe], coros_or_tasks,
-                                               progress)
-
-        # Wait for future for target recipe to return
-        result = await coros_or_tasks[recipe]
-
-        # Close coroutines that were not converted to tasks, since they were never needed for the execution
-        for coro_or_task in coros_or_tasks.values():
-            if not isinstance(coro_or_task, asyncio.Task):
-                coro_or_task.close()
+    # Define function that can be called from current or new thread to setup and perform execution
+    def _setup_and_execute() -> OutputsAndChecksums[R]:
+        # Create the asyncio event loop and set it on the calling thread
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+
+        async def _execute() -> OutputsAndChecksums[R]:
+            # Sort the graph topographically, such that any recipe in the sorted list only depends on earlier recipes
+            # This guarantees that futures only depend on already created futures
+            recipes = list(nx.topological_sort(graph))
+
+            # Create coroutines to evaluate each recipe - then from the top-down, the coroutines will request inputs
+            # that they need from other coroutines, which will be upgraded to tasks. This approach is used to avoid
+            # loading outputs for recipes whose outputs are actually unused, because later recipes are already cached
+            coros_or_tasks: Dict[Recipe, Union[Coroutine, Task]] = {}
+            for _recipe in recipes:
+                # Note that 'schedule()' might mutate 'tasks' once awaited
+                coros_or_tasks[_recipe] = schedule(loop, executor, _recipe, statuses[_recipe], coros_or_tasks,
+                                                   progress)
+
+            # Wait for future for target recipe to return
+            result = await coros_or_tasks[recipe]
+
+            # Close coroutines that were not converted to tasks, since they were never needed for the execution
+            for coro_or_task in coros_or_tasks.values():
+                if asyncio.iscoroutine(coro_or_task):
+                    coro_or_task.close()
 
-        return result
+            return result
+
+        return loop.run_until_complete(_execute())
 
     # Return the output and checksum of the final recipe
     if progress is not None:
         progress.start()
-    output, checksum = loop.run_until_complete(_execute())
+
+    # Check if the event loop is already running - if this is the case, execution must be pushed to a new thread to
+    # avoid crashing due to the already running event loop
+    output, checksum = utils.run_on_thread(_setup_and_execute) if utils.check_current_thread_has_running_event_loop() \
+        else _setup_and_execute()
+
     if progress is not None:
         progress.stop()
     return output, checksum
 
 
 def is_clean(recipe: Recipe[R], new_input_checksums: Tuple[Optional[str], ...]) -> Status:
     """
```

### Comparing `alkymi-0.2.0/alkymi/decorators.py` & `alkymi-0.2.1/alkymi/decorators.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi/foreach_recipe.py` & `alkymi-0.2.1/alkymi/foreach_recipe.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi/lab.py` & `alkymi-0.2.1/alkymi/lab.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi/progress.py` & `alkymi-0.2.1/alkymi/progress.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi/recipe.py` & `alkymi-0.2.1/alkymi/recipe.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi/recipes.py` & `alkymi-0.2.1/alkymi/recipes.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi/serialization.py` & `alkymi-0.2.1/alkymi/serialization.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi/types.py` & `alkymi-0.2.1/alkymi/types.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.2.0/alkymi.egg-info/PKG-INFO` & `alkymi-0.2.1/alkymi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alkymi
-Version: 0.2.0
+Version: 0.2.1
 Summary: alkymi - Pythonic task automation
 Home-page: https://github.com/MathiasStokholm/alkymi
 Author: Mathias Bøgh Stokholm
 Author-email: mathias.stokholm@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/MathiasStokholm/alkymi/
 Project-URL: Tracker, https://github.com/MathiasStokholm/alkymi/issues
```

### Comparing `alkymi-0.2.0/setup.py` & `alkymi-0.2.1/setup.py`

 * *Files identical despite different names*


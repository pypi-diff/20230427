# Comparing `tmp/utbot_executor-1.6.1.tar.gz` & `tmp/utbot_executor-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utbot_executor-1.6.1.tar", max compression
+gzip compressed data, was "utbot_executor-1.6.2.tar", max compression
```

## Comparing `utbot_executor-1.6.1.tar` & `utbot_executor-1.6.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.6.1/LICENSE
--rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.6.1/README.md
--rw-r--r--   0        0        0      401 2023-04-13 11:16:20.091550 utbot_executor-1.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.6.1/utbot_executor/__init__.py
--rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.6.1/utbot_executor/__main__.py
--rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.6.1/utbot_executor/deep_serialization/__init__.py
--rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.6.1/utbot_executor/deep_serialization/deep_serialization.py
--rw-r--r--   0        0        0     1469 2023-04-13 11:03:00.871191 utbot_executor-1.6.1/utbot_executor/deep_serialization/example.py
--rw-r--r--   0        0        0     8848 2023-04-13 11:04:25.397297 utbot_executor-1.6.1/utbot_executor/deep_serialization/json_converter.py
--rw-r--r--   0        0        0    10451 2023-04-13 11:16:20.078217 utbot_executor-1.6.1/utbot_executor/deep_serialization/memory_objects.py
--rw-r--r--   0        0        0      413 2023-04-13 11:10:20.054988 utbot_executor-1.6.1/utbot_executor/deep_serialization/numpy_serialization.py
--rw-r--r--   0        0        0     5445 2023-04-13 11:04:25.397297 utbot_executor-1.6.1/utbot_executor/deep_serialization/test_json.json
--rw-r--r--   0        0        0     3871 2023-04-13 11:04:25.397297 utbot_executor-1.6.1/utbot_executor/deep_serialization/utils.py
--rw-r--r--   0        0        0     7975 2023-03-30 13:06:09.677079 utbot_executor-1.6.1/utbot_executor/executor.py
--rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.6.1/utbot_executor/listener.py
--rw-r--r--   0        0        0      873 2023-04-13 11:04:25.397297 utbot_executor-1.6.1/utbot_executor/memory_compressor.py
--rw-r--r--   0        0        0     2578 2023-03-30 11:31:56.739251 utbot_executor-1.6.1/utbot_executor/parser.py
--rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.6.1/utbot_executor/utils.py
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 utbot_executor-1.6.1/setup.py
--rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 utbot_executor-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.6.2/LICENSE
+-rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.6.2/README.md
+-rw-r--r--   0        0        0      401 2023-04-26 11:38:17.557316 utbot_executor-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.6.2/utbot_executor/__init__.py
+-rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.6.2/utbot_executor/__main__.py
+-rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.6.2/utbot_executor/deep_serialization/__init__.py
+-rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.6.2/utbot_executor/deep_serialization/deep_serialization.py
+-rw-r--r--   0        0        0     1469 2023-04-13 11:03:00.871191 utbot_executor-1.6.2/utbot_executor/deep_serialization/example.py
+-rw-r--r--   0        0        0     8848 2023-04-13 11:04:25.397297 utbot_executor-1.6.2/utbot_executor/deep_serialization/json_converter.py
+-rw-r--r--   0        0        0    10451 2023-04-13 11:16:20.078217 utbot_executor-1.6.2/utbot_executor/deep_serialization/memory_objects.py
+-rw-r--r--   0        0        0      413 2023-04-13 11:10:20.054988 utbot_executor-1.6.2/utbot_executor/deep_serialization/numpy_serialization.py
+-rw-r--r--   0        0        0     5445 2023-04-13 11:04:25.397297 utbot_executor-1.6.2/utbot_executor/deep_serialization/test_json.json
+-rw-r--r--   0        0        0     3871 2023-04-13 11:04:25.397297 utbot_executor-1.6.2/utbot_executor/deep_serialization/utils.py
+-rw-r--r--   0        0        0     8066 2023-04-26 11:37:56.776595 utbot_executor-1.6.2/utbot_executor/executor.py
+-rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.6.2/utbot_executor/listener.py
+-rw-r--r--   0        0        0      873 2023-04-13 11:04:25.397297 utbot_executor-1.6.2/utbot_executor/memory_compressor.py
+-rw-r--r--   0        0        0     2661 2023-04-26 11:14:16.320827 utbot_executor-1.6.2/utbot_executor/parser.py
+-rw-r--r--   0        0        0     1550 2023-04-26 11:37:56.759928 utbot_executor-1.6.2/utbot_executor/ut_tracer.py
+-rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.6.2/utbot_executor/utils.py
+-rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 utbot_executor-1.6.2/setup.py
+-rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 utbot_executor-1.6.2/PKG-INFO
```

### Comparing `utbot_executor-1.6.1/LICENSE` & `utbot_executor-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/README.md` & `utbot_executor-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/utbot_executor/__main__.py` & `utbot_executor-1.6.2/utbot_executor/__main__.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/utbot_executor/deep_serialization/deep_serialization.py` & `utbot_executor-1.6.2/utbot_executor/deep_serialization/deep_serialization.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/utbot_executor/deep_serialization/example.py` & `utbot_executor-1.6.2/utbot_executor/deep_serialization/example.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/utbot_executor/deep_serialization/json_converter.py` & `utbot_executor-1.6.2/utbot_executor/deep_serialization/json_converter.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/utbot_executor/deep_serialization/memory_objects.py` & `utbot_executor-1.6.2/utbot_executor/deep_serialization/memory_objects.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/utbot_executor/deep_serialization/test_json.json` & `utbot_executor-1.6.2/utbot_executor/deep_serialization/test_json.json`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/utbot_executor/deep_serialization/utils.py` & `utbot_executor-1.6.2/utbot_executor/deep_serialization/utils.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/utbot_executor/executor.py` & `utbot_executor-1.6.2/utbot_executor/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Python code executor for UnitTestBot"""
 import copy
 import inspect
 import importlib
-import json
 import logging
 import pathlib
 import sys
 import trace
 import traceback
 from typing import Any, Callable, Dict, Iterable, List, Tuple
 
 from utbot_executor.deep_serialization.deep_serialization import serialize_objects, serialize_memory_dump, \
     serialize_objects_dump
 from utbot_executor.deep_serialization.json_converter import DumpLoader, deserialize_memory_objects
 from utbot_executor.deep_serialization.memory_objects import MemoryDump, ReduceMemoryObject, PythonSerializer
 from utbot_executor.deep_serialization.utils import PythonId, getattr_by_path
 from utbot_executor.memory_compressor import compress_memory
 from utbot_executor.parser import ExecutionRequest, ExecutionResponse, ExecutionFailResponse, ExecutionSuccessResponse
+from utbot_executor.ut_tracer import UtTracer
 from utbot_executor.utils import suppress_stdout as __suppress_stdout
 
 __all__ = ['PythonExecutor']
 
 
 def _update_states(init_memory_dump: MemoryDump, state_before: MemoryDump) -> MemoryDump:
     for id_, obj in state_before.objects.items():
@@ -138,31 +138,33 @@
 
 
 def _run_calculate_function_value(
         function: Callable,
         args: List[Any],
         kwargs: Dict[str, Any],
         fullpath: str,
-        state_init: str
+        state_init: str,
+        tracer: UtTracer,
     ) -> ExecutionResponse:
     """ Calculate function evaluation result.
 
     Return serialized data: status, coverage info, object ids and memory."""
 
     _, _, _, state_before, serialized_state_before = _serialize_state(args, kwargs)
 
     __is_exception = False
 
     (__sources, __start, ) = inspect.getsourcelines(function)
     __end = __start + len(__sources)
 
-    __tracer = trace.Trace(
-        count=1,
-        trace=0,
-    )
+    # __tracer = trace.Trace(
+    #     count=1,
+    #     trace=0,
+    # )
+    __tracer = tracer
 
     try:
         with __suppress_stdout():
             __result = __tracer.runfunc(function, *args, **kwargs)
     except Exception as __exception:
         __result = __exception
         __is_exception = True
```

### Comparing `utbot_executor-1.6.1/utbot_executor/listener.py` & `utbot_executor-1.6.2/utbot_executor/listener.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/utbot_executor/memory_compressor.py` & `utbot_executor-1.6.2/utbot_executor/memory_compressor.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.6.1/utbot_executor/parser.py` & `utbot_executor-1.6.2/utbot_executor/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     function_module: str
     imports: List[str]
     syspaths: List[str]
     arguments_ids: List[str]
     kwarguments_ids: Dict[str, str]
     serialized_memory: str
     filepath: str
+    coverage_id: str
 
 
 class ExecutionResponse:
     status: str
 
 
 @dataclasses.dataclass
@@ -45,25 +46,27 @@
             'functionName',
             'functionModule',
             'imports',
             'syspaths',
             'argumentsIds',
             'kwargumentsIds',
             'serializedMemory',
-            'filepath'
+            'filepath',
+            'coverageId',
             }:
         return ExecutionRequest(
                 dct['functionName'],
                 dct['functionModule'],
                 dct['imports'],
                 dct['syspaths'],
                 dct['argumentsIds'],
                 dct['kwargumentsIds'],
                 dct['serializedMemory'],
                 dct['filepath'],
+                dct['coverageId'],
                 )
     return dct
 
 
 def parse_request(request: str) -> ExecutionRequest:
     return json.loads(request, object_hook=as_execution_result)
```

### Comparing `utbot_executor-1.6.1/setup.py` & `utbot_executor-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['utbot-executor = utbot_executor:utbot_executor']}
 
 setup_kwargs = {
     'name': 'utbot-executor',
-    'version': '1.6.1',
+    'version': '1.6.2',
     'description': '',
     'long_description': '# UtBot Executor\n\nUtil for python code execution and state serialization.\n\n## Installation\n\nYou can install module from [PyPI](https://pypi.org/project/utbot-executor/):\n\n```bash\npython -m pip install utbot-executor\n```\n\n## Usage\n\n### From console with socket listener\n\nRun with your `<hostname>` and `<port>` for socket connection\n```bash\n$ python -m utbot_executor <hostname> <port> <logfile> [<loglevel DEBUG | INFO | ERROR>]\n```\n\n### Result format:\n\n```json\n{\n        "status": "success",\n        "isException": bool,\n        "statements": list[int],\n        "missedStatements": list[int],\n        "stateBefore": memory json dump,\n        "stateAfter": memory json dump,\n        "argsIds": list[str],\n        "kwargs": list[str],\n        "resultId": str,\n}\n```\n\nor error format:\n\n```json\n{\n        "status": "fail",\n        "exception": str (traceback),\n}\n```\n\n#### States format\n\nTODO\n\n### Submodule `deep_serialization`\n\nJSON serializer and deserializer for python objects\n\n## Source\n\nGitHub [repository](https://github.com/tamarinvs19/utbot_executor)\n',
     'author': 'Vyacheslav Tamarin',
     'author_email': 'vyacheslav.tamarin@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `utbot_executor-1.6.1/PKG-INFO` & `utbot_executor-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utbot-executor
-Version: 1.6.1
+Version: 1.6.2
 Summary: 
 Author: Vyacheslav Tamarin
 Author-email: vyacheslav.tamarin@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


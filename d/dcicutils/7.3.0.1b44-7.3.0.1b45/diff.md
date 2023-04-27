# Comparing `tmp/dcicutils-7.3.0.1b44.tar.gz` & `tmp/dcicutils-7.3.0.1b45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.3.0.1b44.tar", max compression
+gzip compressed data, was "dcicutils-7.3.0.1b45.tar", max compression
```

## Comparing `dcicutils-7.3.0.1b44.tar` & `dcicutils-7.3.0.1b45.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1166 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/README.rst
--rw-r--r--   0        0        0        0 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3587 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-27 16:15:43.482113 dcicutils-7.3.0.1b44/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46730 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     7169 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    31947 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20234 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   154304 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-27 16:15:43.486113 dcicutils-7.3.0.1b44/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-27 16:15:43.490113 dcicutils-7.3.0.1b44/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-04-27 16:15:43.490113 dcicutils-7.3.0.1b44/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-04-27 16:15:43.490113 dcicutils-7.3.0.1b44/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-27 16:15:43.490113 dcicutils-7.3.0.1b44/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-04-27 16:15:43.490113 dcicutils-7.3.0.1b44/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-04-27 16:15:43.490113 dcicutils-7.3.0.1b44/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-04-27 16:15:43.490113 dcicutils-7.3.0.1b44/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3992 2023-04-27 16:15:43.490113 dcicutils-7.3.0.1b44/pyproject.toml
--rw-r--r--   0        0        0     2708 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b44/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b44/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/README.rst
+-rw-r--r--   0        0        0        0 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3587 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46730 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     7318 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    31947 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20234 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154304 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3992 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/pyproject.toml
+-rw-r--r--   0        0        0     2708 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b45/setup.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b45/PKG-INFO
```

### Comparing `dcicutils-7.3.0.1b44/README.rst` & `dcicutils-7.3.0.1b45/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/base.py` & `dcicutils-7.3.0.1b45/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/beanstalk_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/cloudformation_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/codebuild_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/command_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/common.py` & `dcicutils-7.3.0.1b45/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/creds_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/data_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/deployment_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/diff_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/docker_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/ecr_scripts.py` & `dcicutils-7.3.0.1b45/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/ecr_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/ecs_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/env_base.py` & `dcicutils-7.3.0.1b45/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/env_manager.py` & `dcicutils-7.3.0.1b45/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/env_scripts.py` & `dcicutils-7.3.0.1b45/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/env_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/env_utils_legacy.py` & `dcicutils-7.3.0.1b45/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/es_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/exceptions.py` & `dcicutils-7.3.0.1b45/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/ff_mocks.py` & `dcicutils-7.3.0.1b45/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/ff_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/function_cache_decorator.py` & `dcicutils-7.3.0.1b45/dcicutils/function_cache_decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import namedtuple, OrderedDict
 from datetime import datetime, timedelta
+from typing import Union
 import json
 import sys
 
 
 _function_cache_list = []
 
 
@@ -119,23 +120,24 @@
                     cache.popitem(last=False)
                 if not now:
                     now = datetime.now()
                 cache[cache_key] = {"value": value, "timestamp": now}
 
             return value
 
-        def cache_info(as_dict: bool = False):
+        def cache_info(as_dict: bool = False) -> Union[namedtuple, dict]:
             cache_info = namedtuple("cache_info", ["hits", "misses", "size", "maxsize", "ttl", "ttl_none",
                                                    "nocache_none", "key", "serialize_key", "updated"])
             updated = next(iter(cache.items()))[1]["timestamp"] if len(cache) > 0 else None
+            updated = updated.strftime("%Y-%m-%d %H:%M:%S") if updated else None
             info = cache_info(nhits, nmisses, len(cache), maxsize, ttl, ttl_none,
                               nocache_none, key, serialize_key, updated)
             return dict(info._asdict()) if as_dict else info
 
-        def cache_clear():
+        def cache_clear() -> None:
             nonlocal nhits, nmisses
             nhits = nmisses = 0
             cache.clear()
 
         function_wrapper.cache_info = cache_info
         function_wrapper.cache_clear = cache_clear
         _function_cache_list.append({"function_wrapper": function_wrapper, "wrapped_function": wrapped_function})
@@ -143,15 +145,15 @@
         return function_wrapper
 
     if decorator_invoked_without_args:
         return function_cache_decorator_registration(decorator_target_function)
     return function_cache_decorator_registration
 
 
-def function_cache_info():
+def function_cache_info() -> dict:
     """
     Returns a list of dictionaries representing all of the function_cache instances
     which exist; each dictonary containing detailed info about the function cache.
     For debugging/testing/troubleshooting.
     """
     info = []
     for function_cache in _function_cache_list:
```

### Comparing `dcicutils-7.3.0.1b44/dcicutils/glacier_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/jh_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/kibana/dashboards.json` & `dcicutils-7.3.0.1b45/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/kibana/readme.md` & `dcicutils-7.3.0.1b45/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/lang_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/log_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/misc_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/obfuscation_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/opensearch_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/qa_checkers.py` & `dcicutils-7.3.0.1b45/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/qa_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/redis_tools.py` & `dcicutils-7.3.0.1b45/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/redis_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/s3_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.3.0.1b45/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/secrets_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/snapshot_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/task_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/dcicutils/trace_utils.py` & `dcicutils-7.3.0.1b45/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b44/pyproject.toml` & `dcicutils-7.3.0.1b45/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.3.0.1b44"
+version = "7.3.0.1b45"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.3.0.1b44/setup.py` & `dcicutils-7.3.0.1b45/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.3.0.1b44',
+    'version': '7.3.0.1b45',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.3.0.1b44/PKG-INFO` & `dcicutils-7.3.0.1b45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.3.0.1b44
+Version: 7.3.0.1b45
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```


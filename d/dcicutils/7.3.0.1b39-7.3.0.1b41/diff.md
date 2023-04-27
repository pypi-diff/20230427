# Comparing `tmp/dcicutils-7.3.0.1b39.tar.gz` & `tmp/dcicutils-7.3.0.1b41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.3.0.1b39.tar", max compression
+gzip compressed data, was "dcicutils-7.3.0.1b41.tar", max compression
```

## Comparing `dcicutils-7.3.0.1b39.tar` & `dcicutils-7.3.0.1b41.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1166 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/README.rst
--rw-r--r--   0        0        0        0 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3587 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46730 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     4792 2023-04-27 03:05:20.817502 dcicutils-7.3.0.1b39/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    31947 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20234 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   154304 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-04-27 03:05:20.821503 dcicutils-7.3.0.1b39/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3992 2023-04-27 03:05:20.825503 dcicutils-7.3.0.1b39/pyproject.toml
--rw-r--r--   0        0        0     2708 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b39/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b39/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/README.rst
+-rw-r--r--   0        0        0        0 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3587 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46730 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-04-27 12:39:43.164312 dcicutils-7.3.0.1b41/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     5722 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    31947 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20234 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154304 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-27 12:39:43.168312 dcicutils-7.3.0.1b41/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3992 2023-04-27 12:39:43.172312 dcicutils-7.3.0.1b41/pyproject.toml
+-rw-r--r--   0        0        0     2708 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b41/setup.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b41/PKG-INFO
```

### Comparing `dcicutils-7.3.0.1b39/README.rst` & `dcicutils-7.3.0.1b41/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/base.py` & `dcicutils-7.3.0.1b41/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/beanstalk_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/cloudformation_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/codebuild_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/command_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/common.py` & `dcicutils-7.3.0.1b41/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/creds_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/data_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/deployment_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/diff_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/docker_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/ecr_scripts.py` & `dcicutils-7.3.0.1b41/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/ecr_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/ecs_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/env_base.py` & `dcicutils-7.3.0.1b41/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/env_manager.py` & `dcicutils-7.3.0.1b41/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/env_scripts.py` & `dcicutils-7.3.0.1b41/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/env_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/env_utils_legacy.py` & `dcicutils-7.3.0.1b41/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/es_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/exceptions.py` & `dcicutils-7.3.0.1b41/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/ff_mocks.py` & `dcicutils-7.3.0.1b41/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/ff_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/function_cache_decorator.py` & `dcicutils-7.3.0.1b41/dcicutils/function_cache_decorator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import OrderedDict
 from datetime import datetime, timedelta
+import json
 import sys
 
 
 def function_cache(*decorator_args, **decorator_kwargs):
     """
     Exactly analogous to the functools.lru_cache decorator, but also allows
     specifying that if the return value of the function is None then no caching
@@ -16,14 +17,21 @@
 
     In addition we support a time_to_live (ttl) decorator kwarg which can be specified,
     as a timedelta type. If the cached value for the function is more than the specified
     ttl then it is considered stale and the function will be called to get a fresh value.
     And, there is a separate time_to_live_none (ttl_none) supported which will do the
     same as ttl but will apply only if the cached value is None.
 
+    There is also a serialize_key (serialize) decorator kwarg which if specified as True,
+    will serialize the arguments (args and kwargs) to the function call and use that value,
+    converted to a string, as the key for caching the function result; this will allow
+    caching for functions which take non-hashable structured types (i.e. dict or list)
+    as arguments, which normally would not be possible, i.e. e.g. in which case this
+    error would be generated: TypeError: unhashable type: 'dict'
+
     Looked/tried and could not find an way to do this using @lru_cache;
     and also had issues trying to wrap @lru_cache with this functionality.
     First created (April 2023) to try simplify some of the caching in foursight-core APIs.
     """
     cache = OrderedDict()
     nhits = nmisses = 0
 
@@ -35,14 +43,15 @@
         decorator_invoked_without_args = False
         decorator_target_function = None
 
     maxsize = sys.maxsize
     nocache_none = False
     ttl = None
     ttl_none = None
+    serialize_key = False
 
     if decorator_args:
         maxsize_arg = decorator_args[0]
         if isinstance(maxsize_arg, int) and maxsize_arg > 0:
             maxsize = maxsize_arg
     if decorator_kwargs:
         maxsize_kwarg = decorator_kwargs.get("maxsize")
@@ -53,20 +62,25 @@
             nocache_none = nocache_none_kwarg
         ttl_kwarg = decorator_kwargs.get("time_to_live", decorator_kwargs.get("ttl"))
         if isinstance(ttl_kwarg, timedelta):
             ttl = ttl_kwarg
         ttl_none_kwarg = decorator_kwargs.get("time_to_live_none", decorator_kwargs.get("ttl_none"))
         if isinstance(ttl_none_kwarg, timedelta):
             ttl_none = ttl_none_kwarg
+        serialize_key_kwarg = decorator_kwargs.get("serialize_key", decorator_kwargs.get("serialize"))
+        if isinstance(serialize_key_kwarg, bool):
+            serialize_key = serialize_key_kwarg
 
     def function_cache_decorator_registration(wrapped_function):
 
-        def wrapper_function(*args, **kwargs):
+        def function_wrapper(*args, **kwargs):
 
             key = args + tuple(sorted(kwargs.items()))
+            if serialize_key:
+                key = json.dumps(key, default=str, separators=(",", ":"))
             cached = cache.get(key, None)
             now = None
 
             if cached is not None:
 
                 if ttl or ttl_none:
                     now = datetime.now()
@@ -105,21 +119,23 @@
             }
             if maxsize != sys.maxsize:
                 info["maxsize"] = maxsize
             if ttl:
                 info["ttl"] = ttl
             if ttl_none:
                 info["ttl_none"] = ttl_none
+            if serialize_key:
+                info["serialize"] = serialize_key
             return info
 
         def cache_clear():
             nonlocal nhits, nmisses
             nhits = nmisses = 0
             cache.clear()
 
-        wrapper_function.cache_info = cache_info
-        wrapper_function.cache_clear = cache_clear
-        return wrapper_function
+        function_wrapper.cache_info = cache_info
+        function_wrapper.cache_clear = cache_clear
+        return function_wrapper
 
     if decorator_invoked_without_args:
         return function_cache_decorator_registration(decorator_target_function)
     return function_cache_decorator_registration
```

### Comparing `dcicutils-7.3.0.1b39/dcicutils/glacier_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/jh_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/kibana/dashboards.json` & `dcicutils-7.3.0.1b41/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/kibana/readme.md` & `dcicutils-7.3.0.1b41/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/lang_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/log_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/misc_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/obfuscation_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/opensearch_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/qa_checkers.py` & `dcicutils-7.3.0.1b41/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/qa_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/redis_tools.py` & `dcicutils-7.3.0.1b41/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/redis_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/s3_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.3.0.1b41/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/secrets_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/snapshot_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/task_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/dcicutils/trace_utils.py` & `dcicutils-7.3.0.1b41/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b39/pyproject.toml` & `dcicutils-7.3.0.1b41/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.3.0.1b39"
+version = "7.3.0.1b41"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.3.0.1b39/setup.py` & `dcicutils-7.3.0.1b41/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.3.0.1b39',
+    'version': '7.3.0.1b41',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.3.0.1b39/PKG-INFO` & `dcicutils-7.3.0.1b41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.3.0.1b39
+Version: 7.3.0.1b41
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```


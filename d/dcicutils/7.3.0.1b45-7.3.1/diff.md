# Comparing `tmp/dcicutils-7.3.0.1b45.tar.gz` & `tmp/dcicutils-7.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.3.0.1b45.tar", max compression
+gzip compressed data, was "dcicutils-7.3.1.tar", max compression
```

## Comparing `dcicutils-7.3.0.1b45.tar` & `dcicutils-7.3.1.tar`

### file list

```diff
@@ -1,49 +1,47 @@
--rw-r--r--   0        0        0     1166 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/README.rst
--rw-r--r--   0        0        0        0 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3587 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-27 19:15:33.120059 dcicutils-7.3.0.1b45/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46730 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     7318 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    31947 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20234 2023-04-27 19:15:33.124059 dcicutils-7.3.0.1b45/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   154304 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3992 2023-04-27 19:15:33.128059 dcicutils-7.3.0.1b45/pyproject.toml
--rw-r--r--   0        0        0     2708 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b45/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b45/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-04-27 19:35:27.703873 dcicutils-7.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-04-27 19:35:27.703873 dcicutils-7.3.1/README.rst
+-rw-r--r--   0        0        0        0 2023-04-27 19:35:27.703873 dcicutils-7.3.1/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-27 19:35:27.703873 dcicutils-7.3.1/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3587 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46318 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    31947 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-27 19:35:27.707873 dcicutils-7.3.1/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20234 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154304 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    19745 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     8082 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-27 19:35:27.711873 dcicutils-7.3.1/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3839 2023-04-27 19:35:27.711873 dcicutils-7.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 dcicutils-7.3.1/setup.py
+-rw-r--r--   0        0        0     2954 1970-01-01 00:00:00.000000 dcicutils-7.3.1/PKG-INFO
```

### Comparing `dcicutils-7.3.0.1b45/README.rst` & `dcicutils-7.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/base.py` & `dcicutils-7.3.1/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/beanstalk_utils.py` & `dcicutils-7.3.1/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/cloudformation_utils.py` & `dcicutils-7.3.1/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/codebuild_utils.py` & `dcicutils-7.3.1/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/command_utils.py` & `dcicutils-7.3.1/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/common.py` & `dcicutils-7.3.1/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/creds_utils.py` & `dcicutils-7.3.1/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/data_utils.py` & `dcicutils-7.3.1/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/deployment_utils.py` & `dcicutils-7.3.1/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/diff_utils.py` & `dcicutils-7.3.1/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/docker_utils.py` & `dcicutils-7.3.1/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/ecr_scripts.py` & `dcicutils-7.3.1/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/ecr_utils.py` & `dcicutils-7.3.1/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/ecs_utils.py` & `dcicutils-7.3.1/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/env_base.py` & `dcicutils-7.3.1/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/env_manager.py` & `dcicutils-7.3.1/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/env_scripts.py` & `dcicutils-7.3.1/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/env_utils.py` & `dcicutils-7.3.1/dcicutils/env_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,24 +686,14 @@
     entry = (find_association(EnvUtils.PUBLIC_URL_TABLE, **{p.NAME: envname}) or
              find_association(EnvUtils.PUBLIC_URL_TABLE, **{p.ENVIRONMENT: full_env_name(envname)}) or
              find_association(EnvUtils.PUBLIC_URL_TABLE, **{p.ENVIRONMENT: short_env_name(envname)}))
     if entry:
         return entry
 
 
-def get_portal_url(envname: EnvName) -> UrlString:
-    """
-    Returns the Portal URL for the given environment name.
-    Effectively same ase get_env_real_url (below) but does not actually access
-    the URL (to get the health page is that function does); i.e. so we can get
-    the URL without exception even if there is a problem with the Portal.
-    """
-    return get_env_real_url(full_env_name(envname))
-
-
 @if_orchestrated
 def get_env_real_url(envname: EnvName) -> UrlString:
 
     entry = _find_public_url_entry(envname)
     if entry:
         return entry.get('url')
```

### Comparing `dcicutils-7.3.0.1b45/dcicutils/env_utils_legacy.py` & `dcicutils-7.3.1/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/es_utils.py` & `dcicutils-7.3.1/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/exceptions.py` & `dcicutils-7.3.1/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/ff_mocks.py` & `dcicutils-7.3.1/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/ff_utils.py` & `dcicutils-7.3.1/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/glacier_utils.py` & `dcicutils-7.3.1/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/jh_utils.py` & `dcicutils-7.3.1/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/kibana/dashboards.json` & `dcicutils-7.3.1/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/kibana/readme.md` & `dcicutils-7.3.1/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/lang_utils.py` & `dcicutils-7.3.1/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/log_utils.py` & `dcicutils-7.3.1/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/misc_utils.py` & `dcicutils-7.3.1/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/obfuscation_utils.py` & `dcicutils-7.3.1/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/opensearch_utils.py` & `dcicutils-7.3.1/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/qa_checkers.py` & `dcicutils-7.3.1/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/qa_utils.py` & `dcicutils-7.3.1/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/redis_tools.py` & `dcicutils-7.3.1/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/redis_utils.py` & `dcicutils-7.3.1/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/s3_utils.py` & `dcicutils-7.3.1/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/secrets_utils.py` & `dcicutils-7.3.1/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/snapshot_utils.py` & `dcicutils-7.3.1/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/task_utils.py` & `dcicutils-7.3.1/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/dcicutils/trace_utils.py` & `dcicutils-7.3.1/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b45/pyproject.toml` & `dcicutils-7.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.3.0.1b45"
+version = "7.3.1"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
-  { include="dcicutils", from="." },
-  { include="scripts", from="dcicutils" }
+  { include="dcicutils", from="." }
 ]
 classifiers = [
     # How mature is this project? Common values are
     #   3 - Alpha
     #   4 - Beta
     #   5 - Production/Stable
     'Development Status :: 4 - Beta',
@@ -53,15 +52,14 @@
 structlog = "^19.2.0"
 toml = ">=0.10.1,<1"
 typing-extensions = ">=3.8"  # Fourfront uses 3.8
 urllib3 = "^1.26.6"
 webtest = "^2.0.34"
 opensearch-py = "^2.0.1"
 redis = "^4.5.1"
-pyOpenSSL = "^23.1.1"
 PyJWT = "^2.6.0"
 tqdm = "^4.65.0"
 
 
 [tool.poetry.dev-dependencies]
 botocore-stubs = "1.21.22"
 boto3-stubs = "1.18.23"
@@ -74,18 +72,14 @@
 pytest = ">=4.5.0"
 pytest-cov = ">=2.7.1"
 pytest-mock = ">=1.11.0"
 pytest-redis = "^2.0.0"
 pytest-runner = ">=5.1"
 
 
-[tool.poetry.scripts]
-publish-to-pypi = "dcicutils.scripts.publish_to_pypi:main"
-
-
 [tool.pytest.ini_options]
 addopts = "--basetemp=/tmp/pytest"
 redis_exec = "/usr/local/bin/redis-server"
 filterwarnings = [
     "ignore::DeprecationWarning: distutils Version classes are deprecated. Use packaging.version instead.",
 ]
 markers = [
```

### Comparing `dcicutils-7.3.0.1b45/setup.py` & `dcicutils-7.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,52 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
-{'': '.', 'scripts': 'dcicutils/scripts'}
+{'': '.'}
 
 packages = \
-['dcicutils', 'dcicutils.scripts', 'scripts']
+['dcicutils']
 
 package_data = \
 {'': ['*'], 'dcicutils': ['kibana/*']}
 
 install_requires = \
 ['PyJWT>=2.6.0,<3.0.0',
  'PyYAML>=5.1,<5.5',
  'aws-requests-auth>=0.4.2,<1',
  'boto3>=1.17.39,<2.0.0',
  'botocore>=1.20.39,<2.0.0',
  'docker>=4.4.4,<5.0.0',
  'elasticsearch==7.13.4',
  'gitpython>=3.1.2,<4.0.0',
  'opensearch-py>=2.0.1,<3.0.0',
- 'pyOpenSSL>=23.1.1,<24.0.0',
  'pytz>=2020.4',
  'redis>=4.5.1,<5.0.0',
  'requests>=2.21.0,<3.0.0',
  'rfc3986>=1.4.0,<2.0.0',
  'structlog>=19.2.0,<20.0.0',
  'toml>=0.10.1,<1',
  'tqdm>=4.65.0,<5.0.0',
  'typing-extensions>=3.8',
  'urllib3>=1.26.6,<2.0.0',
  'webtest>=2.0.34,<3.0.0']
 
-entry_points = \
-{'console_scripts': ['publish-to-pypi = '
-                     'dcicutils.scripts.publish_to_pypi:main']}
-
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.3.0.1b45',
+    'version': '7.3.1',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'entry_points': entry_points,
     'python_requires': '>=3.7,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `dcicutils-7.3.0.1b45/PKG-INFO` & `dcicutils-7.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.3.0.1b45
+Version: 7.3.1
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,14 @@
 Requires-Dist: aws-requests-auth (>=0.4.2,<1)
 Requires-Dist: boto3 (>=1.17.39,<2.0.0)
 Requires-Dist: botocore (>=1.20.39,<2.0.0)
 Requires-Dist: docker (>=4.4.4,<5.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: opensearch-py (>=2.0.1,<3.0.0)
-Requires-Dist: pyOpenSSL (>=23.1.1,<24.0.0)
 Requires-Dist: pytz (>=2020.4)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
 Requires-Dist: requests (>=2.21.0,<3.0.0)
 Requires-Dist: rfc3986 (>=1.4.0,<2.0.0)
 Requires-Dist: structlog (>=19.2.0,<20.0.0)
 Requires-Dist: toml (>=0.10.1,<1)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
```


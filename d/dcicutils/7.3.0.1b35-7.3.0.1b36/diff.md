# Comparing `tmp/dcicutils-7.3.0.1b35.tar.gz` & `tmp/dcicutils-7.3.0.1b36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.3.0.1b35.tar", max compression
+gzip compressed data, was "dcicutils-7.3.0.1b36.tar", max compression
```

## Comparing `dcicutils-7.3.0.1b35.tar` & `dcicutils-7.3.0.1b36.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1166 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/README.rst
--rw-r--r--   0        0        0        0 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/base.py
--rwxr-xr-x   0        0        0    52659 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    13639 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/command_utils.py
--rw-r--r--   0        0        0     1649 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46730 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/exceptions.py
--rw-r--r--   0        0        0    37025 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    11502 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/log_utils.py
--rw-r--r--   0        0        0    87972 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20232 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   121536 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0    10080 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3807 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/pyproject.toml
--rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b35/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/README.rst
+-rw-r--r--   0        0        0        0 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/base.py
+-rwxr-xr-x   0        0        0    52659 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    13639 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     1649 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46730 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    37025 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-26 14:10:14.512515 dcicutils-7.3.0.1b36/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    87972 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20232 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   121536 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9718 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3807 2023-04-26 14:10:14.516515 dcicutils-7.3.0.1b36/pyproject.toml
+-rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b36/PKG-INFO
```

### Comparing `dcicutils-7.3.0.1b35/README.rst` & `dcicutils-7.3.0.1b36/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/base.py` & `dcicutils-7.3.0.1b36/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/beanstalk_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/cloudformation_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/codebuild_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/command_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/common.py` & `dcicutils-7.3.0.1b36/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/creds_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/data_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/deployment_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/diff_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/docker_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/ecr_scripts.py` & `dcicutils-7.3.0.1b36/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/ecr_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/ecs_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/env_base.py` & `dcicutils-7.3.0.1b36/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/env_manager.py` & `dcicutils-7.3.0.1b36/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/env_scripts.py` & `dcicutils-7.3.0.1b36/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/env_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/env_utils_legacy.py` & `dcicutils-7.3.0.1b36/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/es_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/exceptions.py` & `dcicutils-7.3.0.1b36/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/ff_mocks.py` & `dcicutils-7.3.0.1b36/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/ff_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/jh_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/kibana/dashboards.json` & `dcicutils-7.3.0.1b36/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/kibana/readme.md` & `dcicutils-7.3.0.1b36/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/lang_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/log_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/misc_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/obfuscation_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/opensearch_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/qa_checkers.py` & `dcicutils-7.3.0.1b36/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/qa_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/redis_tools.py` & `dcicutils-7.3.0.1b36/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/redis_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/s3_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.3.0.1b36/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/secrets_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/snapshot_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/ssl_certificate_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from cryptography.hazmat.primitives import serialization
 from datetime import datetime, timedelta
 import OpenSSL
 import socket
 import ssl
 from typing import Optional, Tuple
+from .misc_utils import future_datetime
 
 
 def get_ssl_certificate_info(hostname: str,
                              raise_exception: bool = False,
                              test_mode_certificate_expiration_warning_days: int = 0) -> Optional[dict]:
     """
     Returns a dictionary containing various data points for the SSL certificate of the given
@@ -96,22 +97,14 @@
             if extension.get_short_name() == b"subjectAltName":
                 sans_list = str(extension).replace(" ", "").split(",")
                 for san in sans_list:
                     if san.startswith("DNS:"):
                         sans.append(san[4:])
         return sorted(sans)
 
-    def is_datetime_within_ndays(d: datetime, ndays: int) -> bool:
-        """
-        Returns True iff the given datatime is within "ndays" days (in the future) of the current
-        datetime, i.e. if the current datetime plus "ndays" days is greater-than-or-equal to the
-        given datetime; otherwise returns False.
-        """
-        return (d - now) <= timedelta(days=ndays) if d >= now else False
-
     try:
         certificate = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM, pem_string)
 
         subject = certificate.get_subject()
         common_name = subject.commonName
         hostnames = get_hostnames(certificate)
         owner_country = subject.countryName
@@ -129,15 +122,15 @@
         issuer_entity = issuer.organizationName
         issuer = issuer.organizationalUnitName or issuer_entity
 
         not_before = certificate.get_notBefore().decode("UTF-8")
         not_after = certificate.get_notAfter().decode("UTF-8")
         active_at = datetime.strptime(not_before, "%Y%m%d%H%M%SZ")
         expires_at = datetime.strptime(not_after, "%Y%m%d%H%M%SZ")
-        expires_soon = is_datetime_within_ndays(expires_at, expires_soon_days)
+        expires_soon = expires_at <= future_datetime(now=now, days=expires_soon_days)
 
         expired = now >= expires_at
         inactive = now <= active_at
         invalid = inactive or expired
 
         # Note we could not currently get detect specifically if the certificate is revoked;
         # could not get the recommeneded code working consistently; no great matter.
```

### Comparing `dcicutils-7.3.0.1b35/dcicutils/task_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/dcicutils/trace_utils.py` & `dcicutils-7.3.0.1b36/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b35/pyproject.toml` & `dcicutils-7.3.0.1b36/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.3.0.1b35"
+version = "7.3.0.1b36"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.3.0.1b35/PKG-INFO` & `dcicutils-7.3.0.1b36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.3.0.1b35
+Version: 7.3.0.1b36
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```


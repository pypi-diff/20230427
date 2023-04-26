# Comparing `tmp/dcicutils-7.3.0.1b37.tar.gz` & `tmp/dcicutils-7.3.0.1b38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.3.0.1b37.tar", max compression
+gzip compressed data, was "dcicutils-7.3.0.1b38.tar", max compression
```

## Comparing `dcicutils-7.3.0.1b37.tar` & `dcicutils-7.3.0.1b38.tar`

### file list

```diff
@@ -1,47 +1,49 @@
--rw-r--r--   0        0        0     1166 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/README.rst
--rw-r--r--   0        0        0        0 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/base.py
--rwxr-xr-x   0        0        0    52659 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    13639 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/command_utils.py
--rw-r--r--   0        0        0     1649 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46730 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-04-26 22:08:08.209953 dcicutils-7.3.0.1b37/dcicutils/exceptions.py
--rw-r--r--   0        0        0    37025 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     4833 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    11502 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/log_utils.py
--rw-r--r--   0        0        0    87972 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20232 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   121536 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9718 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-04-26 22:08:08.213953 dcicutils-7.3.0.1b37/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3807 2023-04-26 22:08:08.217953 dcicutils-7.3.0.1b37/pyproject.toml
--rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b37/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-26 23:09:41.164485 dcicutils-7.3.0.1b38/README.rst
+-rw-r--r--   0        0        0        0 2023-04-26 23:09:41.164485 dcicutils-7.3.0.1b38/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-26 23:09:41.164485 dcicutils-7.3.0.1b38/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-04-26 23:09:41.164485 dcicutils-7.3.0.1b38/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3587 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46730 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     4833 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    31947 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20234 2023-04-26 23:09:41.168485 dcicutils-7.3.0.1b38/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154304 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3992 2023-04-26 23:09:41.172485 dcicutils-7.3.0.1b38/pyproject.toml
+-rw-r--r--   0        0        0     2708 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b38/setup.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b38/PKG-INFO
```

### Comparing `dcicutils-7.3.0.1b37/README.rst` & `dcicutils-7.3.0.1b38/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/base.py` & `dcicutils-7.3.0.1b38/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/beanstalk_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/beanstalk_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,35 +35,14 @@
 )
 
 
 logging.basicConfig()
 logger = logging.getLogger('logger')
 logger.setLevel(logging.INFO)
 
-# In Python 2, the safe 'input' function was called 'raw_input'.  Also in Python 2, there was a function
-# named 'input' that did eval(raw_input(...)).  Python 3 made an incompatible change, renaming 'raw_input'
-# to 'input', and it no longer has a function that does an unsafe eval.  When we supported both Python 2 & 3,
-# use a 'try' expression to sort things out and call the safe function 'use_input' to avoid confusion.
-# But PyCharm found that 'try' expression confusing, so now that we are Python 3 only, we're phasing that
-# out. For a time, we'll retain the transitional naming, though, along with an affirmative error check, so
-# we don't open any security holes.
-# TODO: We can remove this naming and check once we're we're only using Python 3.
-# -kmp 27-Mar-2020
-
-# The name whodaman was deprecated and has been removed as of dcicutils 3.0
-# Please use compute_ff_prd_env instead.
-#
-# whodaman = compute_ff_prd_env  # This naming is obsolete but retained for compatibility.
-
-# The legacy name MAGIC_CNAME was deprecated and is finally removed as of dcicutils 3.0.
-# MAGIC_CNAME = _FF_MAGIC_CNAME
-
-# The legacy name GOLDEN_DB was deprecated and is finally removed as of dcicutils 3.0.
-# GOLDEN_DB = _FF_GOLDEN_DB
-
 # identifier for locating environment variables in EB config
 ENV_VARIABLE_NAMESPACE = 'aws:elasticbeanstalk:application:environment'
 
 
 class WaitingForBoto3(Exception):
     pass
```

### Comparing `dcicutils-7.3.0.1b37/dcicutils/cloudformation_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/codebuild_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/command_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/command_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import contextlib
+import functools
 import glob
 import logging
 import os
+import re
 import requests
 import subprocess
 
 from typing import Optional
 from .exceptions import InvalidParameterError
 from .lang_utils import there_are
-from .misc_utils import PRINT, environ_bool, print_error_message
+from .misc_utils import INPUT, PRINT, environ_bool, print_error_message, decorator
 
 
 def _ask_boolean_question(question, quick=None, default=None):
     """
     Loops asking a question interactively until it gets a 'yes' or 'no' response. Returns True or False accordingly.
 
     :param question: The question to ask (without prompts for possible responses, which will be added automatically).
@@ -30,15 +32,15 @@
     affirmative = affirmatives[0]
     negative = negatives[0]
     prompt = ("%s [%s/%s]: "
               % (question,
                  affirmative.upper() if default is True else affirmative,
                  negative.upper() if default is False else negative))
     while True:
-        answer = input(prompt).strip().lower()
+        answer = INPUT(prompt).strip().lower()
         if answer in affirmatives:
             return True
         elif answer in negatives:
             return False
         elif answer == "" and default is not None:
             return default
         else:
@@ -69,14 +71,58 @@
     The response must be confirmed by pressing Enter.
     If Enter is pressed with no input text, the default is returned if there is one, or else the user is re-prompted.
     If Enter is pressed after other text than the valid responses, the user is reprompted.
     """
     return _ask_boolean_question(question, quick=True, default=default)
 
 
+DOC_PARAM_PATTERN = re.compile("^( *:param *)[^: ][^:]*:.*$")
+DOC_RETURN_PATTERN = re.compile("^ *:return:.*$")
+
+
+def add_param_to_doc(docstring, var, var_desc):
+    doclines = (docstring or "").splitlines()
+    prefix = ":param "
+    for i, line in enumerate(doclines):
+        m = DOC_PARAM_PATTERN.match(line)
+        if m:
+            prefix = m.group(1)  # the last one is best
+        m = DOC_RETURN_PATTERN.match(line)
+        if m:
+            new_desc_line = prefix + f"{var}: {var_desc}"
+            return "\n".join(doclines[:i] + [new_desc_line] + doclines[i:])
+    new_desc_line = prefix + f"{var}: {var_desc}"
+    return "\n".join(doclines + [new_desc_line])
+
+
+@decorator()
+def require_confirmation(*, prompt=None, default=True, raise_error=True):
+    """
+    Decorator that if specified will look for a kwarg called 'confirm' and if True will prompt the user
+    for confirmation.
+    """
+    def _attach_confirmation(func):
+
+        func_name = func.__name__
+
+        @functools.wraps(func)
+        def _func_with_confirmation(*args, confirm=default, **kwargs):
+            if not confirm or y_or_n(prompt or f"Are you sure you want to proceed with {func_name}?"):
+                return func(*args, **kwargs)
+            elif raise_error:
+                raise ScriptFailure("Aborted by user.")
+
+        _func_with_confirmation.__doc__ = add_param_to_doc(func.__doc__ or f"Missing doc for {func_name}.",
+                                                           "confirm", "whether to ask for confirmation")
+
+        return _func_with_confirmation
+
+    return _attach_confirmation
+
+
 class ShellScript:
     """
     This is really an internal class. You're intended to work via the shell_script context manager.
     But there might be uses for this class, too, so we'll give it a pretty name.
     """
 
     # This is the shell the script will use to execute
```

### Comparing `dcicutils-7.3.0.1b37/dcicutils/creds_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/data_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/deployment_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/diff_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/docker_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/ecr_scripts.py` & `dcicutils-7.3.0.1b38/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/ecr_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/ecs_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/env_base.py` & `dcicutils-7.3.0.1b38/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/env_manager.py` & `dcicutils-7.3.0.1b38/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/env_scripts.py` & `dcicutils-7.3.0.1b38/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/env_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/env_utils_legacy.py` & `dcicutils-7.3.0.1b38/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/es_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/exceptions.py` & `dcicutils-7.3.0.1b38/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/ff_mocks.py` & `dcicutils-7.3.0.1b38/dcicutils/ff_mocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from dcicutils.qa_utils import (
     MockBoto3, MockBotoElasticBeanstalkClient, MockBotoS3Client, ControlledTime, MockResponse,
     make_mock_beanstalk, make_mock_beanstalk_cname, make_mock_beanstalk_environment_variables,
 )
 from dcicutils.s3_utils import EnvManager
 from typing import Optional, TextIO
 from unittest import mock
-from . import beanstalk_utils, ff_utils, s3_utils, env_utils, env_base, env_manager
+from . import beanstalk_utils, ff_utils, s3_utils, env_utils, env_base, env_manager, glacier_utils
 from .common import LEGACY_GLOBAL_ENV_BUCKET
 
 
 _MOCK_APPLICATION_NAME = "4dn-web"
 _MOCK_SERVICE_USERNAME = 'service-accout-name'
 _MOCK_SERVICE_PASSWORD = 'service-accout-pw'
 _MOCK_APPLICATION_OPTIONS_PARTIAL = (
@@ -144,54 +144,51 @@
             EnvManager.LEGACY_ES_URL_KEY: make_mock_es_url(environment),
             EnvManager.LEGACY_ENV_NAME_KEY: environment,
             "ecosystem": ecosystem_file
         }
         write_config(environment, record)
     write_config(ecosystem_file, {"is_legacy": True})
     # Now we arrange that s3_utils, ff_utils, etc. modules share the illusion that our mock IS the boto3 library
-    with mock.patch.object(s3_utils, "boto3", mock_boto3):
-        with mock.patch.object(ff_utils, "boto3", mock_boto3):
-            with mock.patch.object(beanstalk_utils, "boto3", mock_boto3):
-                with mock.patch.object(env_utils, "boto3", mock_boto3):
-                    with mock.patch.object(env_base, "boto3", mock_boto3):
-                        with mock.patch.object(env_manager, "boto3", mock_boto3):
-                            with mock.patch.object(s3_utils.EnvManager, "fetch_health_page_json") as mock_fetcher:
-                                # This is all that's needed for s3Utils to initialize an EnvManager.
-                                # We might have to add more later.
-                                def mocked_fetch_health_page_json(url, use_urllib=True):
-                                    ignored(use_urllib)  # we don't test this
-                                    m = re.match(r'.*(fourfront-[a-z0-9-]+)(?:[.]|$)', url)
-                                    if m:
-                                        env_name = m.group(1)  # we found it with a fourfront-prefix, so use as is
-                                        return make_mock_health_page(env_name)
-                                    m = re.match(r'(?:https?://)?([a-z0-9-]+)'
-                                                 r'(?:[.](4dnucleome[.]org|hms.harvard.edu)([/].*)|$)', url)
-                                    if m:
-                                        env_name = full_env_name(m.group(1))  # no fourfront- prefix, so add one
-                                        return make_mock_health_page(env_name)
-                                    raise NotImplementedError(f"Mock can't handle URL: {url}")
-
-                                mock_fetcher.side_effect = mocked_fetch_health_page_json
-                                # The mocked encrypt key is expected by various tools in the s3_utils module
-                                # to be supplied as an environment variable (i.e., in os.environ), so this
-                                # sets up that environment variable.
-                                if require_sse:
-                                    with override_environ(S3_ENCRYPT_KEY=s3_class.SSE_ENCRYPT_KEY):
+    with mock.patch.object(glacier_utils, "boto3", mock_boto3):
+        with mock.patch.object(s3_utils, "boto3", mock_boto3):
+            with mock.patch.object(ff_utils, "boto3", mock_boto3):
+                with mock.patch.object(beanstalk_utils, "boto3", mock_boto3):
+                    with mock.patch.object(env_utils, "boto3", mock_boto3):
+                        with mock.patch.object(env_base, "boto3", mock_boto3):
+                            with mock.patch.object(env_manager, "boto3", mock_boto3):
+                                with mock.patch.object(s3_utils.EnvManager, "fetch_health_page_json") as mock_fetcher:
+                                    # This is all that's needed for s3Utils to initialize an EnvManager.
+                                    # We might have to add more later.
+                                    def mocked_fetch_health_page_json(url, use_urllib=True):
+                                        ignored(use_urllib)  # we don't test this
+                                        m = re.match(r'.*(fourfront-[a-z0-9-]+)(?:[.]|$)', url)
+                                        if m:
+                                            env_name = m.group(1)  # we found it with a fourfront-prefix, so use as is
+                                            return make_mock_health_page(env_name)
+                                        m = re.match(r'(?:https?://)?([a-z0-9-]+)'
+                                                     r'(?:[.](4dnucleome[.]org|hms.harvard.edu)([/].*)|$)', url)
+                                        if m:
+                                            env_name = full_env_name(m.group(1))  # no fourfront- prefix, so add one
+                                            return make_mock_health_page(env_name)
+                                        raise NotImplementedError(f"Mock can't handle URL: {url}")
+
+                                    mock_fetcher.side_effect = mocked_fetch_health_page_json
+                                    # The mocked encrypt key is expected by various tools in the s3_utils module
+                                    # to be supplied as an environment variable (i.e., in os.environ), so this
+                                    # sets up that environment variable.
+                                    overrides = {}
+                                    if require_sse:
+                                        overrides['S3_ENCRYPT_KEY'] = s3_class.SSE_ENCRYPT_KEY
+                                    with override_environ(**overrides):
                                         with EnvUtils.local_env_utils_for_testing(
                                                 global_env_bucket=os.environ.get('GLOBAL_ENV_BUCKET'),
-                                                env_name=(
-                                                        environments[0]
-                                                        if environments else
-                                                        os.environ.get('ENV_NAME'))):
+                                                env_name=(environments[0]
+                                                          if environments
+                                                          else os.environ.get('ENV_NAME'))):
                                             yield mock_boto3
-                                else:
-                                    with EnvUtils.local_env_utils_for_testing(
-                                            global_env_bucket=os.environ.get('GLOBAL_ENV_BUCKET'),
-                                            env_name=os.environ.get('ENV_NAME')):
-                                        yield mock_boto3
 
 
 DEFAULT_SSE_ENVIRONMENTS_TO_MOCK = ['fourfront-foo', 'fourfront-bar']
 
 
 @contextlib.contextmanager
 def mocked_s3utils_with_sse(beanstalks=None, environments=None, require_sse=True, files=None):
```

### Comparing `dcicutils-7.3.0.1b37/dcicutils/ff_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/function_cache_decorator.py` & `dcicutils-7.3.0.1b38/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/jh_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/kibana/dashboards.json` & `dcicutils-7.3.0.1b38/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/kibana/readme.md` & `dcicutils-7.3.0.1b38/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/lang_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/log_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/misc_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/misc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,41 +26,62 @@
 
 
 # Is this the right place for this? I feel like this should be done in an application, not a library.
 # -kmp 27-Apr-2020
 logging.basicConfig()
 
 
+class NamedObject(object):
+
+    def __init__(self, name):
+        self.name = name
+
+    def __str__(self):
+        return f"<{self.name}>"
+
+    def __repr__(self):
+        return f"<{self.name}@{id(self):x}>"
+
+
 # Using PRINT(...) for debugging, rather than its more familiar lowercase form) for intended programmatic output,
 # makes it easier to find stray print statements that were left behind in debugging. -kmp 30-Mar-2020
 
-class _PRINT:
+class _MOCKABLE_IO:
 
-    def __init__(self):
-        self._printer = print  # necessary indirection for sake of qa_utils.printed_output
+    def __init__(self, wrapped_action):
+        self.wrapped_action = wrapped_action  # necessary indirection for sake of qa_utils.printed_output
 
     def __call__(self, *args, timestamped=False, **kwargs):
         """
         Prints its args space-separated, as 'print' would, possibly with an hh:mm:ss timestamp prepended.
 
         :param args: an object to be printed
         :param with_time: a boolean specifying whether to prepend a timestamp
         """
         if timestamped:
             hh_mm_ss = str(datetime.datetime.now().strftime("%H:%M:%S"))
-            self._printer(hh_mm_ss, *args, **kwargs)
+            return self.wrapped_action(' '.join(map(str, (hh_mm_ss, *args))), **kwargs)
         else:
-            self._printer(*args, **kwargs)
+            return self.wrapped_action(' '.join(map(str, args)), **kwargs)
+
 
+def _mockable_input(*args):
+    return input(*args)
 
-prompt_for_input = input  # In Python 3, this does 'safe' input reading.
 
-PRINT = _PRINT()
+builtin_print = print
+
+PRINT = _MOCKABLE_IO(wrapped_action=print)
 PRINT.__name__ = 'PRINT'
 
+INPUT = _MOCKABLE_IO(wrapped_action=_mockable_input)
+INPUT.__name__ = 'INPUT'
+
+prompt_for_input = INPUT  # In Python 3, input does 'safe' input reading. INPUT is our mockable alternative
+
 
 @contextlib.contextmanager
 def lines_printed_to(file):
     """
     This context manager opens a file and returns a function that can be called repeatedly during the body context
     to do do line-by-line output to that file. It uses PRINT to do that output, so the unit test tools for PRINT
     can be used to test this.
@@ -596,15 +617,18 @@
     if frac == 0.0:
         seconds = int(intpart)
     if as_type is not None:
         seconds = as_type(seconds)
     return seconds
 
 
-# Pulled this in from "glacier" branch for use in foursight-core (2023-04-26).
+MIN_DATETIME = datetime.datetime(datetime.MINYEAR, 1, 1, 0, 0, 0)
+MIN_DATETIME_UTC = datetime.datetime(datetime.MINYEAR, 1, 1, 0, 0, 0, tzinfo=pytz.UTC)
+
+
 def future_datetime(*, now=None, seconds=0, minutes=0, hours=0, days=0, weeks=0, milliseconds=0):
     delta = datetime.timedelta(seconds=seconds, minutes=minutes, hours=hours,
                                days=days, weeks=weeks, milliseconds=milliseconds)
     return (now or datetime.datetime.now()) + delta
 
 
 REF_TZ = pytz.timezone(os.environ.get("REF_TZ") or "US/Eastern")
@@ -1701,14 +1725,60 @@
         self.getter = getter
 
     def __get__(self, instance, instance_class):
         ignored(instance)
         return self.getter(instance_class)
 
 
+class managed_property(object):
+    """
+    Sample use:
+
+        class Temperature:
+
+            def __init__(self, fahrenheit=32):
+                self.fahrenheit = fahrenheit
+
+            @managed_property
+            def centigrade(self, degrees):
+                if degrees == managed_property.MISSING:
+                    return (self.fahrenheit - 32) * 5 / 9.0
+                else:
+                    self.fahrenheit = degrees * 9 / 5.0 + 32
+
+        t1 = Temperature()
+        assert t1.fahrenheit == 32
+        assert t1.centigrade == 0.0
+
+        t2 = Temperature(fahrenheit=68)
+        assert t2.fahrenheit == 68.0
+        assert t2.centigrade == 20.0
+        t2.centigrade = 5
+        assert t2.centigrade == 5.0
+        assert t2.fahrenheit == 41.0
+
+        t2.fahrenheit = -40
+        assert t2.centigrade == -40.0
+
+    """
+
+    MISSING = NamedObject("missing")
+
+    def __init__(self, handler):
+
+        self.handler = handler
+
+    def __get__(self, instance, instance_class):
+        ignored(instance_class)
+        return self.handler(instance, self.MISSING)
+
+    def __set__(self, instance, value):
+        self.handler(instance, value)
+
+
 class classproperty_cached(object):
     """
     This decorator is like 'classproperty', but the function is run only on first use, not every time, and then cached.
 
     Such a property returns the same value each time, just like any class property,
     but initialization is delayed until first use and determined by a call to the decorated function.
 
@@ -1900,26 +1970,14 @@
     """
 
     @classproperty_cached_each_subclass
     def singleton(cls):  # noQA - PyCharm wrongly thinks the argname should be 'self'
         return cls()     # noQA - PyCharm flags a bogus warning for this
 
 
-class NamedObject(object):
-
-    def __init__(self, name):
-        self.name = name
-
-    def __str__(self):
-        return f"<{self.name}>"
-
-    def __repr__(self):
-        return f"<{self.name}@{id(self):x}>"
-
-
 def key_value_dict(key, value):
     """
     Given a key k and a value v, returns the dictionary {"Key": k, "Value": v}, which is a format AWS is fond of.
     """
     return {'Key': key, 'Value': value}
 
 
@@ -2186,20 +2244,59 @@
     * This will also take tuples as input, though the result will be a list.
     :param lst: list to de-duplicate
     :return: de-duplicated list
     """
     return list(set(lst))
 
 
-def chunked(seq, chunk_size=1):
+def chunked(seq, *, chunk_size=1):
     if not isinstance(chunk_size, int) or chunk_size < 1:
         raise ValueError(f"The chunk_size, {chunk_size}, must be a positive integer.")
     chunk = []
     i = 0
     for item in seq:
         chunk.append(item)
         i = (i + 1) % chunk_size
         if i == 0:
             yield chunk
             chunk = []
     if chunk:
         yield chunk
+
+
+def map_chunked(fn, seq, *, chunk_size=1, reduce=None):
+    result = (fn(chunk) for chunk in chunked(seq, chunk_size=chunk_size))
+    return reduce(result) if reduce is not None else result
+
+
+_36_DIGITS = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ"
+
+
+def format_in_radix(n: int, *, radix: int):
+
+    if not isinstance(n, int) or n < 0:
+        raise ValueError(f"Expected n to be a non-negative integer {n}")
+    if radix < 2 or radix > 36:
+        raise ValueError(f"Expected radix to be an integer between 2 and 36, inclusive: {radix}")
+    buffer = []
+    while n > 0:
+        quo = n // radix
+        rem = n % radix
+        buffer += _36_DIGITS[rem]
+        n = quo
+    buffer.reverse()
+    return "".join(buffer) or "0"
+
+
+def parse_in_radix(text: str, *, radix: int):
+    if not (text and isinstance(text, str)):
+        raise ValueError(f"Expected a string to parse: {text}")
+    if radix < 2 or radix > 36:
+        raise ValueError(f"Expected radix to be an integer between 2 and 36, inclusive: {radix}")
+    res = 0
+    try:
+        for c in text:
+            res = res * radix + _36_DIGITS.index(c.upper())
+        return res
+    except Exception:
+        pass
+    raise ValueError(f"Unable to parse: {text!r}")
```

### Comparing `dcicutils-7.3.0.1b37/dcicutils/obfuscation_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/opensearch_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/qa_checkers.py` & `dcicutils-7.3.0.1b38/dcicutils/qa_checkers.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 
 class DebuggingArtifactChecker(StaticSourcesChecker):
 
     DEBUGGING_PATTERNS = [
         {
             'key': 'print',
             'summary': "call to print",
-            'pattern': r"^[^#]*print[(]"
+            'pattern': r"^[^#]*\bprint[(]"
         },
         {
             'key': 'pdb',
             'summary': "active use of pdb.set_trace",
             'pattern': r"^[^#]*pdb[.]set_trace[(][)]"
         },
     ]
```

### Comparing `dcicutils-7.3.0.1b37/dcicutils/qa_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/qa_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,30 +12,36 @@
 import io
 import logging
 import os
 import pytest
 import pytz
 import re
 import sys
+import threading
 import time
 import uuid
 
 from botocore.credentials import Credentials as Boto3Credentials
 from botocore.exceptions import ClientError
 from collections import defaultdict
 from json import dumps as json_dumps, loads as json_loads
-from typing import Any, Optional, List, DefaultDict
+from typing import Any, Optional, List, DefaultDict, Union, Type, Dict
+from typing_extensions import Literal
 from unittest import mock
+from . import misc_utils as misc_utils_module, command_utils as command_utils_module
+from .common import S3StorageClass
 from .env_utils import short_env_name
 from .exceptions import ExpectedErrorNotSeen, WrongErrorSeen, UnexpectedErrorAfterFix, WrongErrorSeenAfterFix
+from .glacier_utils import GlacierUtils
 from .lang_utils import there_are
 from .misc_utils import (
-    PRINT, ignored, Retry, remove_prefix, REF_TZ,
+    PRINT, INPUT, ignored, Retry, remove_prefix, REF_TZ, builtin_print,
     environ_bool, exported, override_environ, override_dict, local_attrs, full_class_name,
-    find_associations, get_error_message, remove_suffix,
+    find_associations, get_error_message, remove_suffix, format_in_radix, future_datetime,
+    _mockable_input,  # noQA - need this to keep mocking consistent
 )
 from .qa_checkers import QA_EXCEPTION_PATTERN, find_uses, confirm_no_uses, VersionChecker, ChangeLogChecker
 
 
 # Using these names via qa_utils is deprecated. Their proper, supported home is now in qa_checkers.
 # Please rewrite imports to get them from qa_checkers, not qa_utils. -kmp 21-Sep-2022
 exported(QA_EXCEPTION_PATTERN, find_uses, confirm_no_uses, VersionChecker, ChangeLogChecker)
@@ -395,17 +401,22 @@
         self.stream = io.BytesIO() if binary else io.StringIO()
 
     def __enter__(self):
         return self.stream
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         content = self.stream.getvalue()
+        file_system = self.file_system
+        if file_system.exists(self.file):
+            if FILE_SYSTEM_VERBOSE:  # noQA - Debugging option. Doesn't need testing.
+                PRINT(f"Preparing to overwrite {self.file}.")
+            file_system.prepare_for_overwrite(self.file)
         if FILE_SYSTEM_VERBOSE:  # noQA - Debugging option. Doesn't need testing.
-            PRINT("Writing %r to %s." % (content, self.file))
-        self.file_system.files[self.file] = content if isinstance(content, bytes) else content.encode(self.encoding)
+            PRINT(f"Writing {content!r} to {self.file}.")
+        file_system.files[self.file] = content if isinstance(content, bytes) else content.encode(self.encoding)
 
 
 class MockFileSystem:
     """Extremely low-tech mock file system."""
 
     def __init__(self, files=None, default_encoding='utf-8', auto_mirror_files_for_read=False, do_not_auto_mirror=()):
         self.default_encoding = default_encoding
@@ -430,17 +441,21 @@
                 if (self.OS_PATH_EXISTS(file)
                         # file might be in files if someone has been manipulating the file structure directly
                         and file not in self.files):
                     with open(file, 'rb') as fp:
                         self.files[file] = fp.read()
                 self._do_not_mirror(file)
 
+    def prepare_for_overwrite(self, file):
+        # By default this does nothing, but it could do something
+        pass
+
     def exists(self, file):
         self._maybe_auto_mirror_file(file)
-        return bool(self.files.get(file))
+        return self.files.get(file) is not None  # don't want an empty file to pass for missing
 
     def remove(self, file):
         self._maybe_auto_mirror_file(file)
         if self.files.pop(file, None) is None:
             raise FileNotFoundError("No such file or directory: %s" % file)
 
     def open(self, file, mode='r', encoding=None):
@@ -475,14 +490,59 @@
     def mock_exists_open_remove(self):
         with mock.patch("os.path.exists", self.exists):
             with mock.patch("io.open", self.open):
                 with mock.patch("os.remove", self.remove):
                     yield self
 
 
+class MockAWSFileSystem(MockFileSystem):
+
+    def __init__(self, boto3=None, s3=None, versioning_buckets: Union[Literal[True], list, set, tuple] = True,
+                 **kwargs):
+        self.boto3 = boto3 or MockBoto3()
+        self.s3: MockBotoS3Client = s3 or self.boto3.client('s3')
+        if versioning_buckets is not True:
+            versioning_buckets = set(versioning_buckets or {})
+        self.versioning_buckets: Union[Literal[True], set] = versioning_buckets
+        super().__init__(**kwargs)
+
+    def add_bucket_versioning(self, versioning_buckets: Union[Literal[True], list, set, tuple]):
+        """
+        Expands bucket versioning as follows:
+          * If the set is already True (all buckets are versioned), nothing can expand that, so do nothing.
+          * If the set is given as simply True (all buckets should be versioned), that bcomes the new state.
+          * Otherwise, if given a list, set, or tuple of bucket names, and there's already a set, then merge those.
+        """
+        if versioning_buckets is True or self.versioning_buckets is True:
+            self.versioning_buckets = True
+            return
+        else:
+            self.versioning_buckets |= (versioning_buckets or {})
+            return
+
+    def bucket_uses_versioning(self, bucket):
+        """
+        Returns True if the given bucket is needs versioning support.
+        This can happen either of two ways:
+          * If self.versioning_buckets is True, the result is True.
+          * Otherwise, self.versioning_buckets is expected to be a set, and we check if bucket is in that set.
+        """
+        return self.versioning_buckets is True or bucket in self.versioning_buckets
+
+    def prepare_for_overwrite(self, filename):
+        """
+        This method overrides a no-op in the parent class and is a hook to allow noticing we'll want to
+        archive an old file version when we're about to write new data.
+        """
+        bucket, key = filename.split('/', 1)
+        ignored(key)
+        if self.bucket_uses_versioning(bucket):
+            self.s3.archive_current_version(filename=filename)
+
+
 class MockUUIDModule:
     """
     This mock is intended to replace the uuid module itself, not the UUID class (which it ordinarily tries to use).
     In effect, this only changes how UUID strings are generated, not how UUID objects returned are represented.
     However, mocking this is a little complicated because you have to replace individual methods. e.g.,
 
         import uuid
@@ -595,40 +655,47 @@
         return defaultdict(lambda: [])
 
     @classmethod
     def _file_last_dict(cls) -> DefaultDict[Optional[str], Optional[str]]:
         return defaultdict(lambda: None)
 
     def mock_print_handler(self, *args, **kwargs):
+        return self.mock_action_handler(print, *args, **kwargs)
+
+    def mock_input_handler(self, *args, **kwargs):
+        return self.mock_action_handler(_mockable_input, *args, **kwargs)
+
+    def mock_action_handler(self, wrapped_action, *args, **kwargs):
         """
         For the simple case of stdout, .last has the last line and .lines contains all lines.
         For all cases, even stdout, .file_lines[fp] and .lines[fp] contain it.
         Notes:
             * If None is the fp value, sys.stdout is used instead. so that None and the current
               value of sys.stdout are synonyms.
             * This mock ignores 'end=' and will treat all calls to PRINT as if they were separate lines.
         """
         text = " ".join(map(str, args))
         texts = remove_suffix('\n', text).split('\n')
         last_text = texts[-1]
-        print(text, **kwargs)  # noQA - This call to print is low-level implementation
+        result = wrapped_action(text, **kwargs)  # noQA - This call to print is low-level implementation
         # This only captures non-file output output.
         file = kwargs.get('file')
         if file is None:
             file = sys.stdout
         if file is sys.stdout:
             # Easy access to stdout
             self.lines.extend(texts)
             self.last = last_text
             # Every output to stdout is implicitly like output to no file (None)
             self.file_lines[None].extend(texts)
             self.file_last[None] = last_text
         # All accesses of any file/fp, including stdout, get associated with that destination
         self.file_lines[file].extend(texts)
         self.file_last[file] = last_text
+        return result  # print did not havea a result, but input does, so be careful to return it.
 
     def reset(self):
         self.lines = []
         self.last = None
         self.file_lines = self._file_lines_dict()
         self.file_last = self._file_last_dict()
 
@@ -660,16 +727,18 @@
                 assert printed.lines == ['The successor of 3 is 4.']
                 show_successor(4)
                 assert printed.last == 'The successor of 4 is 5.'
                 assert printed.lines == ['The successor of 3 is 4.', 'The successor of 4 is 5.']
     """
 
     printed = _PrintCapturer()
-    with local_attrs(PRINT, _printer=printed.mock_print_handler):
-        yield printed
+    # Use the same PrintCapturer object to capture output from both print and input.
+    with local_attrs(PRINT, wrapped_action=printed.mock_print_handler):
+        with local_attrs(INPUT, wrapped_action=printed.mock_input_handler):
+            yield printed
 
 
 class MockKeysNotImplemented(NotImplementedError):
 
     def __init__(self, operation, keys):
         self.operation = operation
         self.keys = keys
@@ -1918,61 +1987,247 @@
 
     def __init__(self, logical_id=None, physical_resource_id=None):
         self.logical_id = logical_id or f"MockedLogicalId{id(self)}"
         self.physical_resource_id = physical_resource_id or f"MockedPhysicalResourceId{id(self)}"
         self.stack_name = None  # This will get filled out if used as a resource on a mock stack
 
 
-class MockObjectAttributeBlock:
+class MockTemporaryRestoration:
+
+    def __init__(self, delay_seconds: Union[int, float], duration_days: Union[int, float],
+                 storage_class: S3StorageClass):
+        self._available_after = future_datetime(seconds=delay_seconds)
+        self._available_until = future_datetime(now=self.available_after, days=duration_days)
+        self._storage_class = storage_class
+
+    @property
+    def available_after(self):
+        return self._available_after
+
+    @property
+    def available_until(self):
+        return self._available_until
+
+    @property
+    def storage_class(self):
+        return self._storage_class
+
+    def is_expired(self, now=None):
+        now = now or datetime.datetime.now()
+        return now >= self.available_until
+
+    def is_active(self, now=None):
+        now = now or datetime.datetime.now()
+        return now >= self.available_after and not self.is_expired(now=now)
+
+    def hurry_restoration(self):
+        self._available_after = datetime.datetime.now()
+
+    def hurry_restoration_expiry(self):
+        self._available_until = datetime.datetime.now()
+
+
+class MockObjectBasicAttributeBlock:
+
+    def __init__(self, filename, s3):
+        self.last_modified = datetime.datetime.now()
+        self.s3: MockBotoS3Client = s3
+        self.filename: str = filename
+        self.version_id: str = self._generate_version_id()
+
+    def __str__(self):
+        return f"<{self.filename}#{self.version_id}>"
+
+    VERSION_ID_INITIAL_WIDTH = len(format_in_radix(time.time_ns(), radix=36))
+    #  In a single instantiation of python, now 50+ years into the epoch, this mock could overflow one
+    #  digit of this, but not realistically more. So reserving space for one digit of overflow after
+    #  whatever time it is on load.
+    VERSION_ID_MAX_WIDTH = VERSION_ID_INITIAL_WIDTH + 1
+
+    MONTONIC_VERSIONS = False
+
+    @classmethod
+    def _generate_version_id(cls):
+        if cls.MONTONIC_VERSIONS:
+            return format_in_radix(time.time_ns(), radix=36)
+        else:
+            return str(uuid.uuid4()).replace('-', '.').lower()
+
+    @property
+    def storage_class(self) -> S3StorageClass:
+        raise NotImplementedError(f"The method 'storage_class' is expected to be implemented"
+                                  f" in subclasses of MockObjectBasicAttributeBlock: {self}")
+
+    def initialize_storage_class(self, value: S3StorageClass):
+        raise NotImplementedError(f"The method 'initialize_storage_class' is expected to be implemented"
+                                  f" in subclasses of MockObjectBasicAttributeBlock: {self}")
+
+    @property
+    def tagset(self) -> List[Dict[Literal['Key', 'Value'], str]]:
+        """
+        Returns a list of Key/Value dictionaries: [{'Key': ..., 'Value':  ...}, ...]
+        """
+        raise NotImplementedError(f"The method 'tagset' is expected to be implemented"
+                                  f" in subclasses of MockObjectBasicAttributeBlock: {self}")
+
+    def set_tagset(self, value: List[Dict[Literal['Key', 'Value'], str]]):
+        """
+        Sets the tagset to a given list of Key/Value dictionaries: [{'Key': ..., 'Value':  ...}, ...]
+        """
+        raise NotImplementedError(f"The method 'set_tagset' is expected to be implemented"
+                                  f" in subclasses of MockObjectBasicAttributeBlock: {self}")
+
+
+class MockObjectDeleteMarker(MockObjectBasicAttributeBlock):
+
+    @property
+    def storage_class(self) -> S3StorageClass:
+        raise Exception(f"Attempt to find storage class for mock-deleted S3 filename {self.filename}")
+
+    def initialize_storage_class(self, value: S3StorageClass):
+        raise Exception(f"Attempt to initialize storage class for mock-deleted S3 filename {self.filename}")
+
+    @property
+    def tagset(self) -> List[Dict[Literal['Key', 'Value'], str]]:
+        raise Exception(f"Attempt to set tagset for mock-deleted S3 filename {self.filename}")
+
+    def set_tagset(self, value: List[Dict[Literal['Key', 'Value'], str]]):
+        raise Exception(f"Attempt to set tagset for mock-deleted S3 filename {self.filename}")
+
 
-    def __init__(self, filename, boto3):
-        self.filename = filename
-        self.storage_class = boto3.storage_class
-        self.tagset = []
-        # keys go here
+class MockObjectAttributeBlock(MockObjectBasicAttributeBlock):
+
+    def __init__(self, filename, s3):
+        super().__init__(filename=filename, s3=s3)
+        self._storage_class: S3StorageClass = s3.storage_class
+        self._tagset = []
+        # Content must be added later. The file system at time this object is created may still have a stale value.
+        self._content = None
+        self._restoration: Optional[MockTemporaryRestoration] = None
+
+    @property
+    def content(self):
+        return self._content
+
+    def set_content(self, content):
+        if self._content is None:
+            self._content = content
+        else:
+            raise RuntimeError("Attempt to set content for an attribute block that already had content.")
+
+    @property
+    def tagset(self) -> List[Dict[Literal['Key', 'Value'], str]]:
+        return copy.deepcopy(self._tagset)  # don't rely on caller to leave what we give them unmodified
+
+    def set_tagset(self, value: List[Dict[Literal['Key', 'Value'], str]]):
+        self._tagset = copy.deepcopy(value)  # don't rely on caller not to later modify the value given
+
+    @property
+    def storage_class(self):
+        restoration = self.restoration
+        return restoration.storage_class if restoration else self._storage_class
+
+    def initialize_storage_class(self, value):
+        if self.restoration:
+            # It's ambiguous what is intended, but also this interface is really intended only for initialization
+            # and should not be used in the middle of a mock operation. The storage class is not dynamically mutable.
+            # You need to use the mock operations to make new versions with the right storage class after that.
+            raise Exception("Tried to set storage class in an attribute block"
+                            " while a temporary restoration is ongoing.")
+        self._storage_class = value
+
+    _RESTORATION_LOCK = threading.Lock()
+
+    def hurry_restoration(self):
+        with self._RESTORATION_LOCK:
+            restoration = self.restoration
+            if restoration:
+                restoration.hurry_restoration()
+
+    def hurry_restoration_expiry(self):
+        with self._RESTORATION_LOCK:
+            restoration = self.restoration
+            if restoration:
+                restoration.hurry_restoration_expiry()
+
+    def storage_class_for_copy_source(self):
+        with self._RESTORATION_LOCK:
+            restoration = self.restoration
+            if restoration:
+                if not restoration.is_active():
+                    raise Exception("Restoration request still in progress.")
+                return restoration.storage_class
+            else:
+                return self._storage_class
+
+    @property
+    def restoration(self):
+        restoration = self._restoration
+        if restoration and restoration.is_expired():
+            self._restoration = restoration = None
+        return restoration
+
+    def restore_temporarily(self, delay_seconds: Union[int, float], duration_days: Union[int, float],
+                            storage_class: S3StorageClass):
+        with self._RESTORATION_LOCK:
+            if self.restoration:
+                raise Exception("You are already have an active restoration and cannot re-restore it.")
+            self._restoration = MockTemporaryRestoration(delay_seconds=delay_seconds,
+                                                         duration_days=duration_days,
+                                                         storage_class=storage_class)
 
 
 @MockBoto3.register_client(kind='s3')
-class MockBotoS3Client:
+class MockBotoS3Client(MockBoto3Client):
     """
     This is a mock of certain S3 functionality.
     """
 
     MOCK_STATIC_FILES = {}
     MOCK_REQUIRED_ARGUMENTS = {}
 
-    DEFAULT_STORAGE_CLASS = "STANDARD"
+    DEFAULT_STORAGE_CLASS: S3StorageClass = "STANDARD"
 
-    def __init__(self, *, region_name=None, mock_other_required_arguments=None, mock_s3_files=None,
-                 storage_class=None, boto3=None):
-        self.boto3 = boto3 or MockBoto3()
+    def __init__(self, *,
+                 region_name: str = None,
+                 mock_other_required_arguments: Optional[List[str]] = None,
+                 mock_s3_files: Dict[str, Union[str, bytes]] = None,
+                 storage_class: Optional[S3StorageClass] = None,
+                 boto3: Optional[MockBoto3] = None,
+                 versioning_buckets: Union[Literal[True], list, set, tuple] = True):
+        self.boto3 = boto3 = boto3 or MockBoto3()
         if region_name not in (None, 'us-east-1'):
             raise ValueError(f"Unexpected region: {region_name}")
 
         files_cache_marker = '_s3_file_data'
-        shared_reality = self.boto3.shared_reality
+        shared_reality = boto3.shared_reality
         s3_files = shared_reality.get(files_cache_marker)
         if s3_files is None:
             files = self.MOCK_STATIC_FILES.copy()
             for name, content in (mock_s3_files or {}).items():
                 files[name] = content
-            shared_reality[files_cache_marker] = s3_files = MockFileSystem(files=files)
+            shared_reality[files_cache_marker] = s3_files = MockAWSFileSystem(files=files, boto3=boto3, s3=self)
         self.s3_files = s3_files
+        s3_files.add_bucket_versioning(versioning_buckets)
 
         other_required_arguments = self.MOCK_REQUIRED_ARGUMENTS.copy()
         for name, content in mock_other_required_arguments or {}:
             other_required_arguments[name] = content
         self.other_required_arguments = other_required_arguments
-        self.storage_class = storage_class or self.DEFAULT_STORAGE_CLASS
+        self.storage_class: S3StorageClass = storage_class or self.DEFAULT_STORAGE_CLASS
 
     def check_for_kwargs_required_by_mock(self, operation, Bucket, Key, **kwargs):
         ignored(Bucket, Key)
         if kwargs != self.other_required_arguments:
             raise MockKeysNotImplemented(operation, self.other_required_arguments.keys())
 
+    def create_object_for_testing(self, object_content: str, *, Bucket: str, Key: str):
+        assert isinstance(object_content, str)
+        self.upload_fileobj(Fileobj=io.BytesIO(object_content.encode('utf-8')), Bucket=Bucket, Key=Key)
+
     def upload_fileobj(self, Fileobj, Bucket, Key, **kwargs):  # noqa - Uppercase argument names are chosen by AWS
         self.check_for_kwargs_required_by_mock("upload_fileobj", Bucket=Bucket, Key=Key, **kwargs)
         data = Fileobj.read()
         PRINT("Uploading %s (%s bytes) to bucket %s key %s"
               % (Fileobj, len(data), Bucket, Key))
         with self.s3_files.open(os.path.join(Bucket, Key), 'wb') as fp:
             fp.write(data)
@@ -2024,34 +2279,50 @@
         self.s3_files.files[Bucket + "/" + Key] = Body
         return {
             'ETag': self._content_etag(Body)
         }
 
     @staticmethod
     def _content_etag(content):
-        return hashlib.md5(content).hexdigest()
+        # For reasons known only to AWS, the ETag, though described as an MD5 hash, begins and ends with
+        # doublequotes, so an example from
+        # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/client/list_object_versions.html
+        # shows:  'ETag': '"6805f2cfc46c0f04559748bb039d69ae"',
+        return f'"{hashlib.md5(content).hexdigest()}"'
 
     def Bucket(self, name):  # noQA - AWS function naming style
         return MockBotoS3Bucket(s3=self, name=name)
 
     def head_object(self, Bucket, Key, **kwargs):  # noQA - AWS argument naming style
         self.check_for_kwargs_required_by_mock("head_object", Bucket=Bucket, Key=Key, **kwargs)
 
         pseudo_filename = os.path.join(Bucket, Key)
 
         if self.s3_files.exists(pseudo_filename):
             content = self.s3_files.files[pseudo_filename]
-            return {
+            attribute_block = self._object_attribute_block(filename=pseudo_filename)
+            assert isinstance(attribute_block, MockObjectAttributeBlock)  # if file exists, should be normal block
+            result = {
                 'Bucket': Bucket,
                 'Key': Key,
                 'ETag': self._content_etag(content),
                 'ContentLength': len(content),
-                'StorageClass': self._object_storage_class(filename=pseudo_filename),
+                'StorageClass': attribute_block.storage_class,  # self._object_storage_class(filename=pseudo_filename)
                 # Numerous others, but this is enough to make the dictionary non-empty and to satisfy some of our tools
             }
+            restoration = attribute_block.restoration
+            if restoration:
+                assert isinstance(restoration, MockTemporaryRestoration)
+                if restoration.is_active():
+                    result['Restore'] = f'ongoing-request="false", expiry-date="{restoration.available_until}"'
+                else:
+                    result['Restore'] = f'ongoing-request="true"'
+            # if datetime.datetime.now() < attribute_block.available_after:
+            #     result['Restore'] = 'ongoing-request="true"'
+            return result
         else:
             # I would need to research what specific error is needed here and hwen,
             # since it might be a 404 (not found) or a 403 (permissions), depending on various details.
             # For now, just fail in any way since maybe our code doesn't care.
             raise Exception(f"Mock File Not Found: {pseudo_filename}."
                             f" Existing files: {list(self.s3_files.files.keys())}")
 
@@ -2063,18 +2334,14 @@
                 return {"ResponseMetadata": {"HTTPStatusCode": 200}}
         raise ClientError(operation_name='HeadBucket',
                           error_response={  # noQA - PyCharm wrongly complains about this dictionary
                               "Error": {"Code": "404", "Message": "Not Found"},
                               "ResponseMetadata": {"HTTPStatusCode": 404},
                           })
 
-    def list_objects_v2(self, Bucket):  # noQA - AWS argument naming style
-        # This is different but similar to list_objects. However we don't really care about that.
-        return self.list_objects(Bucket=Bucket)
-
     def get_object_tagging(self, Bucket, Key):
         pseudo_file = f"{Bucket}/{Key}"
         return {
             'ResponseMetadata': {
                 # Not presently mocked: RequestId, HostId
                 'HTTPStatusCode': 200,
                 'HTTPHeaders': {
@@ -2112,102 +2379,209 @@
     def _object_attribute_map(self):
         """
         Returns the storage class map for this mock.
 
         Note that this is a property of the boto3 instance (through its .shared_reality) not of the s3 mock itself
         so that if another client is created by that same boto3 mock, it will see the same storage classes.
         """
-        storage_class_map = self.boto3.shared_reality.get('storage_class_map')
-        if not storage_class_map:
-            self.boto3.shared_reality['storage_class_map'] = storage_class_map = {}
-        return storage_class_map
+        object_attribute_map = self.boto3.shared_reality.get('object_attribute_map')
+        if not object_attribute_map:
+            self.boto3.shared_reality['object_attribute_map'] = object_attribute_map = {}
+        return object_attribute_map
+
+    def _object_attribute_blocks(self, filename):
+        attribute_map = self._object_attribute_map()
+        attribute_blocks = attribute_map.get(filename) or []
+        if not attribute_blocks:
+            attribute_map[filename] = attribute_blocks
+        return attribute_blocks
+
+    def _object_all_versions(self, filename):
+        attribute_blocks = self._object_attribute_blocks(filename)
+        if not attribute_blocks and self.s3_files.files.get(filename) is not None:
+            # print(f"AUTOCREATING {filename}")
+            # This will demand-create the first one because our mock initialization protocols are sloppy
+            new_attribute_block = MockObjectAttributeBlock(filename=filename, s3=self)
+            attribute_blocks.append(new_attribute_block)
+        # else:
+        #     print(f"NOT AUTOCREATING {filename} for {self} because {self.s3_files.files}")
+        return attribute_blocks
 
-    def _object_attribute_block(self, filename):
+    def _object_attribute_block(self, filename) -> MockObjectBasicAttributeBlock:
         """
         Returns the attribute_block for an S3 object.
         This contains information like storage class and tagsets.
 
         Because this is an internal routine, 'filename' is 'bucket/key' to match the mock file system we use internally.
 
         Note that this is a property of the boto3 instance (through its .shared_reality) not of the s3 mock itself
         so that if another client is created by that same boto3 mock, it will see the same storage classes.
         """
-        attribute_map = self._object_attribute_map()
-        attribute_block = attribute_map.get(filename)
-        if not attribute_block:
-            attribute_map[filename] = attribute_block = MockObjectAttributeBlock(filename=filename, boto3=self)
-        return attribute_block
+        all_versions: List[MockObjectBasicAttributeBlock] = self._object_all_versions(filename)
+        if not all_versions:
+            # This situation and usually we should not be calling this function at this point,
+            # but try to help developer debug what's going on...
+            if filename in self.s3_files.files:
+                context = f"mock special non-file (bucket?) s3 item: {filename}"
+            else:
+                context = f"mock non-existent S3 file: {filename}"
+            raise ValueError(f"Attempt to obtain object attribute block for {context}.")
+        return all_versions[-1]
+
+    _ARCHIVE_LOCK = threading.Lock()
+
+    def hurry_restoration_for_testing(self, s3_filename, attribute_block=None):
+        """
+        This can be used in testing to hurry up the wait for a temporary restore to become available.
+        """
+        attribute_block = attribute_block or self._object_attribute_block(s3_filename)
+        assert isinstance(attribute_block, MockObjectAttributeBlock)
+        attribute_block.hurry_restoration()
+
+    def hurry_restoration_expiry_for_testing(self, s3_filename, attribute_block=None):
+        """
+        This can be used in testing to hurry up the wait for a temporary restore to expire.
+        """
+        attribute_block = attribute_block or self._object_attribute_block(s3_filename)
+        assert isinstance(attribute_block, MockObjectAttributeBlock)
+        attribute_block.hurry_restoration_expiry()
+
+    def archive_current_version(self, filename,
+                                replacement_class: Type[MockObjectBasicAttributeBlock] = MockObjectAttributeBlock,
+                                init: Optional[callable] = None) -> Optional[MockObjectBasicAttributeBlock]:
+        with self._ARCHIVE_LOCK:
+            # The file system dictionary is the source of content authority until we archive things,
+            # and then the current version has to be archived.
+            content = self.s3_files.files.get(filename)  # might be missing. you can delete a file that doesn't exist
+            preexisting_version = None
+            if content:
+                preexisting_version = self._object_attribute_block(filename)
+                assert isinstance(preexisting_version, MockObjectAttributeBlock)  # should be no content if deleted
+                preexisting_version.set_content(content)
+            new_block = self._prepare_new_attribute_block(filename, attribute_class=replacement_class)
+            self._check_versions_registered(filename, preexisting_version, new_block)
+            if init is not None:
+                init()  # caller can supply an init function to be run while still inside lock
+            return new_block
+
+    def _check_versions_registered(self, filename, *versions: Optional[MockObjectBasicAttributeBlock]):
+        """
+        Performs a useful consistency check to identify problems early, but has no functional effect on other code
+        other than to raise an error if there is a problem.
+
+        :param filename: the S3 filename (in the form bucket/key)
+        :param versions: the versions to check. each should be an attribute block, a delete marker, or None
+        """
+        all_versions = self._object_all_versions(filename)
+        # Check that each of the given versions is present in all_versions
+        for version in versions:
+            if version:
+                assert version in all_versions
+        # We know that all versions are stored in time order. Make sure their simulated last-modified dates
+        # are in time order to match.
+        prior_date = None
+        for version in all_versions:
+            if version:
+                if prior_date:
+                    assert version.last_modified > prior_date
+                prior_date = version.last_modified
+
+    def _prepare_new_attribute_block(self, filename,
+                                     attribute_class: Type[MockObjectBasicAttributeBlock] = MockObjectAttributeBlock
+                                     ) -> MockObjectBasicAttributeBlock:  # given the type, instantiates that type
+        new_block = attribute_class(filename=filename, s3=self)
+        all_versions = self._object_all_versions(filename)
+        all_versions.append(new_block)
+        # NOTE WELL: This would seem information-destroying, but this method should only be called when you're
+        #            about to write new data anyway, after having archived previous data, which means it should
+        #            really only be called by archive_current_version after it has done any necessary saving away
+        #            of a prior version (depending on whether versioning is enabled).
+        self.s3_files.files[filename] = None
+        return new_block
 
     def _object_tagset(self, filename):
         """
         Returns the tagset for the 'filename' in this S3 mock.
         Because this is an internal routine, 'filename' is 'bucket/key' to match the mock file system we use internally.
 
         Note that this is a property of the boto3 instance (through its .shared_reality) not of the s3 mock itself
         so that if another client is created by that same boto3 mock, it will see the same storage classes.
         """
         attribute_block = self._object_attribute_block(filename)
-        return copy.deepcopy(attribute_block.tagset)  # Don't let recipient of value change our stored value
+        return attribute_block.tagset
 
     def _set_object_tagset(self, filename, tagset):
         """
         Sets the tagset for the 'filename' in this S3 mock to the given value.
         Because this is an internal routine, 'filename' is 'bucket/key' to match the mock file system we use internally.
 
         Presently the value is not error-checked. That might change.
         By special exception, passing value=None will revert the storage class to the default for the given mock,
         for which the default default is 'STANDARD'.
 
         Note that this is a property of the boto3 instance (through its .shared_reality) not of the s3 mock itself
         so that if another client is created by that same boto3 mock, it will see the same storage classes.
         """
-        assert isinstance(tagset, list) and all(isinstance(pair, dict) for pair in tagset), (
-            f"An internal tagset must be a list of Key/Value dictionaries: {tagset}"
-        )
         attribute_block = self._object_attribute_block(filename)
-        attribute_block.tagset = copy.deepcopy(tagset)  # Don't share state with our argument
+        attribute_block.set_tagset(tagset)
 
-    def _object_storage_class(self, filename):
+    def _object_version_id(self, filename):
+        """
+        Returns the VersionId for the 'filename' in this S3 mock.
+        Because this is an internal routine, 'filename' is 'bucket/key' to match the mock file system we use internally.
+
+        Note that this is a property of the boto3 instance (through its .shared_reality) not of the s3 mock itself
+        so that if another client is created by that same boto3 mock, it will see the same storage classes.
+        """
+        attribute_block = self._object_attribute_block(filename)
+        return attribute_block.version_id
+
+    def _object_last_modified(self, filename) -> datetime.datetime:
+
+        attribute_block = self._object_attribute_block(filename)
+        return attribute_block.last_modified
+
+    def _object_storage_class(self, filename) -> S3StorageClass:
         """
         Returns the storage class for the 'filename' in this S3 mock.
         Because this is an internal routine, 'filename' is 'bucket/key' to match the mock file system we use internally.
 
         Note that this is a property of the boto3 instance (through its .shared_reality) not of the s3 mock itself
         so that if another client is created by that same boto3 mock, it will see the same storage classes.
         """
         attribute_block = self._object_attribute_block(filename)
         return attribute_block.storage_class
 
-    def _set_object_storage_class(self, filename, value):
+    def _set_object_storage_class_for_testing(self, s3_filename, value: S3StorageClass):
         """
         Sets the storage class for the 'filename' in this S3 mock to the given value.
         Because this is an internal routine, 'filename' is 'bucket/key' to match the mock file system we use internally.
 
         Presently the value is not error-checked. That might change.
         By special exception, passing value=None will revert the storage class to the default for the given mock,
         for which the default default is 'STANDARD'.
 
         Note that this is a property of the boto3 instance (through its .shared_reality) not of the s3 mock itself
         so that if another client is created by that same boto3 mock, it will see the same storage classes.
         """
-        attribute_block = self._object_attribute_block(filename)
-        attribute_block.storage_class = value
+        attribute_block = self._object_attribute_block(s3_filename)
+        attribute_block.initialize_storage_class(value)
 
     def list_objects(self, Bucket, Prefix=None):  # noQA - AWS argument naming style
         # Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects
         bucket_prefix = Bucket + "/"
         bucket_prefix_length = len(bucket_prefix)
         search_prefix = bucket_prefix + (Prefix or '')
         found = []
         for filename, content in self.s3_files.files.items():
             if filename.startswith(search_prefix):
                 found.append({
                     'Key': filename[bucket_prefix_length:],
                     'ETag': self._content_etag(content),
-                    # "LastModified": ...,
+                    'LastModified': self._object_last_modified(filename=filename),
                     # "Owner": {"DisplayName": ..., "ID"...},
                     "Size": len(content),
                     "StorageClass": self._object_storage_class(filename=filename),
                 })
         return {
             # "CommonPrefixes": {"Prefix": ...},
             "Contents": found,
@@ -2219,14 +2593,243 @@
             # "MaxKeys": ...,
             # "NextContinuationToken": ...,
             "Name": Bucket,
             "Prefix": Prefix,
             # "StartAfter": ...,
         }
 
+    def list_objects_v2(self, Bucket):  # noQA - AWS argument naming style
+        # This is different but similar to list_objects. However we don't really care about that.
+        return self.list_objects(Bucket=Bucket)
+
+    def copy_object(self, CopySource, Bucket, Key, CopySourceVersionId=None,
+                    StorageClass: Optional[S3StorageClass] = None):
+        return self._copy_object(CopySource=CopySource, Bucket=Bucket, Key=Key,
+                                 CopySourceVersionId=CopySourceVersionId, StorageClass=StorageClass)
+
+    def _copy_object(self, CopySource, Bucket, Key, CopySourceVersionId, StorageClass: Optional[S3StorageClass] = None,
+                     allow_glacial=False):
+        target_storage_class: S3StorageClass = StorageClass or self.storage_class
+        source_bucket = CopySource['Bucket']
+        source_key = CopySource['Key']
+        source_version_id = CopySource.get('VersionId')  # Optional
+        source_s3_filename = f"{source_bucket}/{source_key}"
+        target_bucket = Bucket
+        target_key = Key
+        target_version_id = CopySourceVersionId
+        target_s3_filename = f"{target_bucket}/{target_key}"
+        copy_in_place = False  # might be overridden below
+        if CopySourceVersionId:
+            if CopySourceVersionId != source_version_id or source_bucket != Bucket or source_key != Key:
+                raise AssertionError(f"This mock expected that if CopySourceVersionId is given,"
+                                     f" a matching Bucket, Key, and VersionId appears in CopySource."
+                                     f" CopySource={CopySource!r} Bucket={Bucket!r} Key={Key!r}"
+                                     f" CopySourceVersionId={CopySourceVersionId!r}")
+            copy_in_place = True
+        source_data = self.s3_files.files.get(source_s3_filename)
+        if source_version_id:
+            source_version = self._get_versioned_object(source_s3_filename, source_version_id)
+            source_data = source_data if source_version.content is None else source_version.content
+        else:
+            source_version = self._object_attribute_block(source_s3_filename)
+        source_storage_class = source_version.storage_class_for_copy_source()
+        if source_data is None:
+            # Probably this will only happen for VersionId=None, but show the VersionId anyway,
+            # but if there's a data inconsistency, we could get here for other reasons,
+            # so show the version id just in case to help debugging. -kmp 21-Apr-2023
+            raise Exception(f"S3 location Bucket={Bucket} Key={Key} VersionId{source_version_id} does not exist.")
+        assert isinstance(source_version, MockObjectAttributeBlock)  # we know this because it has data
+        if not allow_glacial:
+            if GlacierUtils.is_glacier_storage_class(source_storage_class):
+                raise Exception(f"The Copy source {CopySource!r} is in storage class {source_storage_class!r}"
+                                f" and must be restored first.")
+        if not copy_in_place:  # We don't archive previous version or update content for copy-in-place.
+            self.archive_current_version(target_s3_filename)
+            # In this case, we've made a new version and it will be current.
+            # In that case, the files dictionary needs the content copied.
+            self.s3_files.files[target_s3_filename] = source_data
+        target_attribute_block = self._get_versioned_object(target_s3_filename, target_version_id)
+        new_storage_class = target_storage_class
+        if (copy_in_place
+                and GlacierUtils.transition_involves_glacier_restoration(source_storage_class, target_storage_class)):
+            new_storage_class = None  # For a restoration, the don't update the glacier data. It's restored elsewhere.
+            target_attribute_block.restore_temporarily(delay_seconds=self.RESTORATION_DELAY_SECONDS,
+                                                       duration_days=1, storage_class=target_storage_class)
+            PRINT(f"Set up restoration {target_attribute_block.restoration}")
+        else:
+            PRINT(f"The copy was not a temporary restoration.")
+        if new_storage_class:
+            target_attribute_block.initialize_storage_class(new_storage_class)
+        return {'Success': True}
+
+    RESTORATION_DELAY_SECONDS = 2
+
+    def delete_object(self, Bucket, Key, VersionId, **unimplemented_keyargs):
+        # Doc:
+        #  * https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/client/delete_object.html
+        #  * https://docs.aws.amazon.com/AmazonS3/latest/userguide/DeletingObjectVersions.html
+        assert not unimplemented_keyargs, (f"The mock for delete_object needs to be extended."
+                                           f" {there_are(unimplemented_keyargs, kind='unimplemented key')}")
+        assert VersionId and isinstance(VersionId, str), "A VersionId must be supplied to delete_object."
+        s3_filename = f"{Bucket}/{Key}"
+        result = {
+            'ResponseMetadata': self.compute_mock_response_metadata(),
+            'VersionId': VersionId
+        }
+        if not VersionId:
+            # Just like AWS, we don't actually verify that this file even exists in this case.
+            # We allow you to delete a file that does not exist. We just add a delete marker
+            # on the top of the existing versions.
+            props = self._delete_current_version(s3_filename=s3_filename)
+        else:
+            # Just like in AWS, when a version id is given, that version is in-place deleted
+            # with no new delete marker creates.
+            props = self._delete_versioned_object(s3_filename=s3_filename, version_id=VersionId)
+        for key, value in props.items():
+            result[key] = value
+        return result
+
+    def _delete_current_version(self, s3_filename) -> Dict[str, Any]:
+        """
+        Deletes the current version of a versioned file, by piling a delete marker atop it.
+        """
+        delete_marker = self.archive_current_version(s3_filename, replacement_class=MockObjectDeleteMarker)
+        if delete_marker:
+            assert isinstance(delete_marker, MockObjectDeleteMarker)
+            all_versions = self._object_all_versions(s3_filename)
+            all_versions.append(delete_marker)
+            return {'DeleteMarker': True}
+        else:
+            return {}
+
+    def _get_versioned_object(self, s3_filename, version_id=None) -> MockObjectAttributeBlock:
+        found = self._find_versioned_object(s3_filename, version_id)
+        if not found:
+            raise Exception(f"Mock S3 file {s3_filename!r} with version_id {version_id!r} not found.")
+        if isinstance(found, MockObjectDeleteMarker):
+            raise Exception(f"Mock S3 file {s3_filename!r} with version id {version_id!r} is a delete marker.")
+        assert isinstance(found, MockObjectAttributeBlock)
+        return found
+
+    def _find_versioned_object(self, s3_filename, version_id=None) -> Optional[MockObjectBasicAttributeBlock]:
+        all_versions = self._object_all_versions(s3_filename)
+        if version_id is None:
+            if all_versions:
+                return all_versions[-1]
+        else:
+            for version in all_versions:
+                if version.version_id == version_id:
+                    return version
+        return None
+
+    def _delete_versioned_object(self, s3_filename, version_id) -> Dict[str, Any]:
+        """
+        Deletes the current version of a versioned file, by removing it in-place.
+        This path never makes a new delete marker.
+        """
+        result = {}
+        found_version = self._find_versioned_object(s3_filename, version_id)
+        if not found_version:
+            raise ClientError(operation_name="DeleteObject",
+                              error_response={  # noQA - PyCharm wrongly complains about this dictionary
+                                  "Error": {
+                                      "Code": "InvalidArgument",
+                                      "Message": "Invalid version id specified",
+                                      "ArgumentName": "versionId",
+                                      "ArgumentValue": version_id
+                                  }})
+        # Delete the old version
+        all_versions = self._object_all_versions(s3_filename)
+        all_versions.remove(found_version)
+        if isinstance(found_version, MockObjectDeleteMarker):
+            # 'DeleteMarker': True appears in a result if a delete marker is added or removed.
+            # In this case, no new delete marker was added, but one was removed.
+            result['DeleteMarker'] = True
+        # Reset state for the version that shows through
+        if all_versions:
+            # If there are still versions remaining, update the content dictionary in self.s3_files.files
+            new_content = None
+            new_current_version: MockObjectBasicAttributeBlock = all_versions[-1]
+            if isinstance(new_current_version, MockObjectAttributeBlock):
+                new_content = new_current_version.content
+            self.s3_files.files[s3_filename] = new_content
+        else:
+            # If there are no versions remaining, we've completely deleted the thing. Just remove all record.
+            del self.s3_files.files[s3_filename]
+        return result
+
+    def restore_object(self, Bucket, Key, RestoreRequest, VersionId: Optional[str] = None,
+                       StorageClass: Optional[S3StorageClass] = None):
+        duration_days: int = RestoreRequest.get('Days')
+        storage_class: S3StorageClass = StorageClass or self.storage_class
+        s3_filename = f"{Bucket}/{Key}"
+        if not self.s3_files.exists(s3_filename):
+            raise Exception(f"S3 file at Bucket={Bucket!r} Key={Key!r} does not exist,"
+                            f" so cannot be restored from glacier.")
+        attribute_block = self._object_attribute_block(s3_filename)
+        assert isinstance(attribute_block, MockObjectAttributeBlock)  # since the file exists, this should be good
+        attribute_block.restore_temporarily(delay_seconds=self.RESTORATION_DELAY_SECONDS,
+                                            duration_days=duration_days,
+                                            storage_class=storage_class)
+        return {'Success': True}
+
+    def list_object_versions(self, Bucket, Prefix='', **unimplemented_keyargs):  # noQA - AWS argument naming style
+        assert not unimplemented_keyargs, (f"The mock for list_object_versions needs to be extended."
+                                           f" {there_are(unimplemented_keyargs, kind='unimplemented key')}")
+        version_descriptions = []
+        delete_marker_descriptions = []
+        bucket_prefix = Bucket + "/"
+        bucket_prefix_length = len(bucket_prefix)
+        search_prefix = bucket_prefix + (Prefix or '')
+        aws_file_system = self.s3_files
+        for filename, content in aws_file_system.files.items():
+            key = filename[bucket_prefix_length:]
+            if filename.startswith(search_prefix):
+                all_versions = self._object_all_versions(filename)
+                most_recent_version = all_versions[-1]
+                for version in all_versions:
+                    if isinstance(version, MockObjectAttributeBlock):
+                        version_descriptions.append({
+                            # 'Owner': {
+                            #     "DisplayName": "4dn-dcic-technical",
+                            #     "ID": "9e7e144b18724b65641286dfa355edb64c424035706bd1674e9096ee77422a45"
+                            # },
+                            'Key': key,
+                            'VersionId': version.version_id,
+                            'IsLatest': version == most_recent_version,
+                            'ETag': self._content_etag(content),
+                            'Size': len(content if version.content is None else version.content),
+                            'StorageClass': version.storage_class,
+                            'LastModified': version.last_modified,  # type datetime.datetime
+                        })
+                    else:
+                        delete_marker_descriptions.append({
+                            # 'Owner': {
+                            #     "DisplayName": "4dn-dcic-technical",
+                            #     "ID": "9e7e144b18724b65641286dfa355edb64c424035706bd1674e9096ee77422a45"
+                            # },
+                            'Key': key,
+                            'VersionId': version.version_id,
+                            'IsLatest': version == most_recent_version,
+                            'LastModified': version.last_modified,  # type datetime.datetime
+                        })
+                # for other_versions in self.s3_files.other_files[filename]:
+        return {
+            'ResponseMetadata': self.compute_mock_response_metadata(),
+            'IsTruncated': False,
+            'Versions': version_descriptions,
+            'DeleteMarkers': delete_marker_descriptions,
+            'Name': Bucket,
+            'Prefix': Prefix,
+            # 'KeyMarker': "",
+            # 'VersionIdMarker': "",
+            # 'MaxKeys': 1000,
+            # 'EncodingType': "url",
+        }
+
 
 class MockBotoS3Bucket:
 
     def __init__(self, name, s3=None):
         assert s3, "missing s3"
         self.s3 = s3
         self.name = name
@@ -2779,7 +3382,47 @@
         return False
 
     def duration_seconds(self):
         if self.start is None:
             return None
         end = datetime.datetime.now() if self.end is None else self.end
         return (end - self.start).total_seconds()
+
+
+@contextlib.contextmanager
+def print_expected(*expected):
+
+    def mocked_print(*what):
+        printed = " ".join(what)
+        assert printed in expected
+
+    with mock.patch.object(command_utils_module, "PRINT") as mock_print:
+        mock_print.side_effect = mocked_print
+        yield
+
+
+class OutOfInputs(Exception):
+    pass
+
+
+@contextlib.contextmanager
+def input_series(*items):
+    with mock.patch.object(misc_utils_module, 'input') as mock_input:
+
+        def mocked_input(*args, **kwargs):
+            ignored(kwargs)
+            (arg,) = args
+            if not inputs:
+                raise OutOfInputs()
+            result = inputs.pop()
+            builtin_print(arg)
+            builtin_print(result)
+            return result
+
+        mock_input.side_effect = mocked_input
+
+        inputs = []
+
+        for item in reversed(items):
+            inputs.append(item)
+        yield
+        assert not inputs, "Did not use all inputs."
```

### Comparing `dcicutils-7.3.0.1b37/dcicutils/redis_tools.py` & `dcicutils-7.3.0.1b38/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/redis_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/s3_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.3.0.1b38/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/secrets_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/snapshot_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/ssl_certificate_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from cryptography.hazmat.primitives import serialization
-from datetime import datetime, timedelta
+from datetime import datetime
 import OpenSSL
 import socket
 import ssl
 from typing import Optional, Tuple
 from .misc_utils import future_datetime
```

### Comparing `dcicutils-7.3.0.1b37/dcicutils/task_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/dcicutils/trace_utils.py` & `dcicutils-7.3.0.1b38/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b37/pyproject.toml` & `dcicutils-7.3.0.1b38/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.3.0.1b37"
+version = "7.3.0.1b38"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
@@ -55,21 +55,24 @@
 typing-extensions = ">=3.8"  # Fourfront uses 3.8
 urllib3 = "^1.26.6"
 webtest = "^2.0.34"
 opensearch-py = "^2.0.1"
 redis = "^4.5.1"
 pyOpenSSL = "^23.1.1"
 PyJWT = "^2.6.0"
+tqdm = "^4.65.0"
 
 
 [tool.poetry.dev-dependencies]
 botocore-stubs = "1.21.22"
 boto3-stubs = "1.18.23"
 coverage = ">=5.3.1"
-coveralls = ">=3.3.1"
+# Loaded manually in GA workflow for coverage because a dependency on 2to3
+# in its docopts dependency makes a problem for laoding it here in poetry. -kmp 7-Apr-2023
+# coveralls = ">=3.3.1"
 flake8 = ">=3.9.2"
 flaky = ">=3.7.0"
 pytest = ">=4.5.0"
 pytest-cov = ">=2.7.1"
 pytest-mock = ">=1.11.0"
 pytest-redis = "^2.0.0"
 pytest-runner = ">=5.1"
```

### Comparing `dcicutils-7.3.0.1b37/PKG-INFO` & `dcicutils-7.3.0.1b38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.3.0.1b37
+Version: 7.3.0.1b38
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
@@ -32,14 +32,15 @@
 Requires-Dist: pyOpenSSL (>=23.1.1,<24.0.0)
 Requires-Dist: pytz (>=2020.4)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
 Requires-Dist: requests (>=2.21.0,<3.0.0)
 Requires-Dist: rfc3986 (>=1.4.0,<2.0.0)
 Requires-Dist: structlog (>=19.2.0,<20.0.0)
 Requires-Dist: toml (>=0.10.1,<1)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typing-extensions (>=3.8)
 Requires-Dist: urllib3 (>=1.26.6,<2.0.0)
 Requires-Dist: webtest (>=2.0.34,<3.0.0)
 Project-URL: Repository, https://github.com/4dn-dcic/utils
 Description-Content-Type: text/x-rst
 
 =====
```


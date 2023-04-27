# Comparing `tmp/phasellm-0.0.3.tar.gz` & `tmp/phasellm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasellm-0.0.3.tar", last modified: Tue Apr 25 05:59:21 2023, max compression
+gzip compressed data, was "phasellm-0.0.4.tar", last modified: Thu Apr 27 21:33:26 2023, max compression
```

## Comparing `phasellm-0.0.3.tar` & `phasellm-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:59:21.888495 phasellm-0.0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-04-25 05:58:31.000000 phasellm-0.0.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-25 05:59:21.888495 phasellm-0.0.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4845 2023-04-25 05:58:31.000000 phasellm-0.0.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:59:21.888495 phasellm-0.0.3/phasellm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:58:31.000000 phasellm-0.0.3/phasellm/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:59:21.888495 phasellm-0.0.3/phasellm/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-04-25 05:58:31.000000 phasellm-0.0.3/phasellm/eval/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3500 2023-04-25 05:58:31.000000 phasellm-0.0.3/phasellm/eval/eval.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:59:21.888495 phasellm-0.0.3/phasellm/llms/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-25 05:58:31.000000 phasellm-0.0.3/phasellm/llms/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13829 2023-04-25 05:58:31.000000 phasellm-0.0.3/phasellm/llms/llms.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 05:59:21.888495 phasellm-0.0.3/phasellm.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-25 05:59:21.000000 phasellm-0.0.3/phasellm.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-04-25 05:59:21.000000 phasellm-0.0.3/phasellm.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 05:59:21.000000 phasellm-0.0.3/phasellm.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-04-25 05:59:21.000000 phasellm-0.0.3/phasellm.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-25 05:59:21.000000 phasellm-0.0.3/phasellm.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-25 05:59:21.888495 phasellm-0.0.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-25 05:59:11.000000 phasellm-0.0.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:33:26.816733 phasellm-0.0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-04-27 21:29:32.000000 phasellm-0.0.4/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-27 21:33:26.816733 phasellm-0.0.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4845 2023-04-27 21:29:32.000000 phasellm-0.0.4/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:33:26.812734 phasellm-0.0.4/phasellm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:29:32.000000 phasellm-0.0.4/phasellm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1338 2023-04-27 21:29:41.000000 phasellm-0.0.4/phasellm/agents.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3499 2023-04-27 21:29:41.000000 phasellm-0.0.4/phasellm/eval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2013 2023-04-27 21:29:41.000000 phasellm-0.0.4/phasellm/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13653 2023-04-27 21:29:41.000000 phasellm-0.0.4/phasellm/llms.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:33:26.812734 phasellm-0.0.4/phasellm.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-27 21:33:26.000000 phasellm-0.0.4/phasellm.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-04-27 21:33:26.000000 phasellm-0.0.4/phasellm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-27 21:33:26.000000 phasellm-0.0.4/phasellm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      126 2023-04-27 21:33:26.000000 phasellm-0.0.4/phasellm.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-27 21:33:26.000000 phasellm-0.0.4/phasellm.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-27 21:33:26.816733 phasellm-0.0.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1167 2023-04-27 21:29:41.000000 phasellm-0.0.4/setup.py
```

### Comparing `phasellm-0.0.3/LICENSE` & `phasellm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.3/PKG-INFO` & `phasellm-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.3/README.md` & `phasellm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.3/phasellm/eval/eval.py` & `phasellm-0.0.4/phasellm/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Support for LLM evaluation.
 """
 
 #TODO I don't like the way I'm structuring this stuff right now. I should actually run some experiments first.
 
-from ..llms import OpenAIGPTWrapper
+from .llms import OpenAIGPTWrapper
 
 import random
 
 class BinaryPreference():
     """
     Tracks a prompt, prompt variables, responses, and the calculated preference.
     """
```

### Comparing `phasellm-0.0.3/phasellm/llms/llms.py` & `phasellm-0.0.4/phasellm/llms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """
 Abstract classes and wrappers for LLMs, chatbots, and prompts.
 """
 
-# TODO Make all prompts to text completion be strings, so people can fill prompts in. Or support both if need be...
-# TODO Add tests, etc... Make sure everything still works.
-
 import requests
 import json
 import re
 
 # Imports for external APIs
 import openai
 import cohere
```

### Comparing `phasellm-0.0.3/phasellm.egg-info/PKG-INFO` & `phasellm-0.0.4/phasellm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.3/setup.py` & `phasellm-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 DESCRIPTION = "Wrappers for common large langugae models (LLMs) with support for evaluation."
 
 LONG_DESCRIPTION = "PhaseLLM provides wrappers for common large language models and use cases. This makes it easy to swap models in and out as needed. We also provide support for evaluation of models so you can choose which models are better to use."
 
 setup(
     name="phasellm",
@@ -19,14 +19,15 @@
         "Flask>=2.0.0",
         "requests>=2.24.0",
         "openai>=0.26.0",
         "cohere>=4.0.0",
         "transformers>=4.25.0",
         "accelerate>=0.16.0",
         "torch>=1.0.0",
+        "python-dotenv",
     ],
     python_requires=">=3.7",
     keywords="llm, nlp, evaluation, ai",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```


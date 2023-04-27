# Comparing `tmp/one-api-tool-0.2.2.tar.gz` & `tmp/one-api-tool-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.2.2.tar", last modified: Thu Apr 27 11:29:21 2023, max compression
+gzip compressed data, was "one-api-tool-0.2.3.tar", last modified: Thu Apr 27 11:36:51 2023, max compression
```

## Comparing `one-api-tool-0.2.2.tar` & `one-api-tool-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.553032 one-api-tool-0.2.2/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.2/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 11:29:21.552875 one-api-tool-0.2.2/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.2.2/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.549750 one-api-tool-0.2.2/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      560 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)      173 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-27 11:29:21.000000 one-api-tool-0.2.2/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.550373 one-api-tool-0.2.2/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.2/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.551392 one-api-tool-0.2.2/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.2/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2492 2023-04-27 09:10:04.000000 one-api-tool-0.2.2/oneapi/commands/one_api_eval_file.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2206 2023-04-27 10:07:56.000000 one-api-tool-0.2.2/oneapi/commands/one_api_eval_one.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-04-27 08:57:27.000000 one-api-tool-0.2.2/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6668 2023-04-27 11:29:05.000000 one-api-tool-0.2.2/oneapi/one_ai_eval.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9512 2023-04-26 11:27:45.000000 one-api-tool-0.2.2/oneapi/one_api.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.551893 one-api-tool-0.2.2/oneapi/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       42 2023-04-27 09:08:42.000000 one-api-tool-0.2.2/oneapi/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     5614 2023-04-27 09:51:38.000000 one-api-tool-0.2.2/oneapi/prompt_template/prompter.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:29:21.552501 one-api-tool-0.2.2/oneapi/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       25 2023-04-27 02:46:39.000000 one-api-tool-0.2.2/oneapi/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2657 2023-04-27 02:20:51.000000 one-api-tool-0.2.2/oneapi/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-27 11:29:21.553078 one-api-tool-0.2.2/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1245 2023-04-27 11:26:59.000000 one-api-tool-0.2.2/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.165367 one-api-tool-0.2.3/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.3/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 11:36:51.165185 one-api-tool-0.2.3/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.2.3/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.160107 one-api-tool-0.2.3/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      609 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)      173 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-27 11:36:51.000000 one-api-tool-0.2.3/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.160853 one-api-tool-0.2.3/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.3/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.162036 one-api-tool-0.2.3/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.3/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2492 2023-04-27 09:10:04.000000 one-api-tool-0.2.3/oneapi/commands/one_api_eval_file.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2206 2023-04-27 10:07:56.000000 one-api-tool-0.2.3/oneapi/commands/one_api_eval_one.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-04-27 08:57:27.000000 one-api-tool-0.2.3/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6668 2023-04-27 11:29:05.000000 one-api-tool-0.2.3/oneapi/one_ai_eval.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     9512 2023-04-26 11:27:45.000000 one-api-tool-0.2.3/oneapi/one_api.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.163661 one-api-tool-0.2.3/oneapi/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       42 2023-04-27 09:08:42.000000 one-api-tool-0.2.3/oneapi/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)      858 2023-04-27 11:27:56.000000 one-api-tool-0.2.3/oneapi/prompt_template/eval_prompt_template.json
+-rw-r--r--   0 zhangchong   (501) staff       (20)     5614 2023-04-27 09:51:38.000000 one-api-tool-0.2.3/oneapi/prompt_template/prompter.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 11:36:51.164819 one-api-tool-0.2.3/oneapi/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       25 2023-04-27 02:46:39.000000 one-api-tool-0.2.3/oneapi/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2657 2023-04-27 02:20:51.000000 one-api-tool-0.2.3/oneapi/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-27 11:36:51.165413 one-api-tool-0.2.3/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1334 2023-04-27 11:36:50.000000 one-api-tool-0.2.3/setup.py
```

### Comparing `one-api-tool-0.2.2/LICENSE` & `one-api-tool-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.2/PKG-INFO` & `one-api-tool-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.2
+Version: 0.2.3
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.2.2/README.md` & `one-api-tool-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.2/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.2.3/one_api_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.2
+Version: 0.2.3
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.2.2/one_api_tool.egg-info/SOURCES.txt` & `one-api-tool-0.2.3/one_api_tool.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 oneapi/one_ai_eval.py
 oneapi/one_api.py
 oneapi/commands/__init__.py
 oneapi/commands/one_api_eval_file.py
 oneapi/commands/one_api_eval_one.py
 oneapi/commands/one_api_requst.py
 oneapi/prompt_template/__init__.py
+oneapi/prompt_template/eval_prompt_template.json
 oneapi/prompt_template/prompter.py
 oneapi/utils/__init__.py
 oneapi/utils/data_utils.py
```

### Comparing `one-api-tool-0.2.2/oneapi/commands/one_api_eval_file.py` & `one-api-tool-0.2.3/oneapi/commands/one_api_eval_file.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.2/oneapi/commands/one_api_eval_one.py` & `one-api-tool-0.2.3/oneapi/commands/one_api_eval_one.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.2/oneapi/commands/one_api_requst.py` & `one-api-tool-0.2.3/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.2/oneapi/one_ai_eval.py` & `one-api-tool-0.2.3/oneapi/one_ai_eval.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.2/oneapi/one_api.py` & `one-api-tool-0.2.3/oneapi/one_api.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.2/oneapi/prompt_template/prompter.py` & `one-api-tool-0.2.3/oneapi/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.2/oneapi/utils/data_utils.py` & `one-api-tool-0.2.3/oneapi/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.2/setup.py` & `one-api-tool-0.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(),
+    package_data={
+      "oneapi":["prompt_template/eval_prompt_template.json"]  
+    },
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
         "httpx",
```


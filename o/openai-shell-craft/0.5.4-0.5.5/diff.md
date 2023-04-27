# Comparing `tmp/openai_shell_craft-0.5.4.tar.gz` & `tmp/openai_shell_craft-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_shell_craft-0.5.4.tar", last modified: Mon Apr 17 16:24:56 2023, max compression
+gzip compressed data, was "openai_shell_craft-0.5.5.tar", last modified: Thu Apr 27 15:10:24 2023, max compression
```

## Comparing `openai_shell_craft-0.5.4.tar` & `openai_shell_craft-0.5.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.962135 openai_shell_craft-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-17 16:24:56.962135 openai_shell_craft-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.958135 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:24:56.962135 openai_shell_craft-0.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.958135 openai_shell_craft-0.5.4/shell_craft/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.958135 openai_shell_craft-0.5.4/shell_craft/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.958135 openai_shell_craft-0.5.4/shell_craft/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/factories/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.962135 openai_shell_craft-0.5.4/shell_craft/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/prompts/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/prompts/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/prompts/templates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.962135 openai_shell_craft-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/tests/test_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:10:24.378052 openai_shell_craft-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-27 15:10:24.378052 openai_shell_craft-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:10:24.370051 openai_shell_craft-0.5.5/openai_shell_craft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-27 15:10:24.000000 openai_shell_craft-0.5.5/openai_shell_craft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-27 15:10:24.000000 openai_shell_craft-0.5.5/openai_shell_craft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:10:24.000000 openai_shell_craft-0.5.5/openai_shell_craft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-27 15:10:24.000000 openai_shell_craft-0.5.5/openai_shell_craft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 15:10:24.000000 openai_shell_craft-0.5.5/openai_shell_craft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 15:10:24.000000 openai_shell_craft-0.5.5/openai_shell_craft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:10:24.378052 openai_shell_craft-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:10:24.370051 openai_shell_craft-0.5.5/shell_craft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:10:24.374052 openai_shell_craft-0.5.5/shell_craft/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/cli/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/cli/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/cli/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/cli/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/cli/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:10:24.374052 openai_shell_craft-0.5.5/shell_craft/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/factories/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:10:24.378052 openai_shell_craft-0.5.5/shell_craft/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/prompts/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/prompts/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/prompts/templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/shell_craft/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:10:24.378052 openai_shell_craft-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-27 15:10:07.000000 openai_shell_craft-0.5.5/tests/test_factories.py
```

### Comparing `openai_shell_craft-0.5.4/LICENSE` & `openai_shell_craft-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/PKG-INFO` & `openai_shell_craft-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_shell_craft
-Version: 0.5.4
+Version: 0.5.5
 Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
 Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
 Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
 Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_shell_craft-0.5.4/README.md` & `openai_shell_craft-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/openai_shell_craft.egg-info/PKG-INFO` & `openai_shell_craft-0.5.5/openai_shell_craft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-shell-craft
-Version: 0.5.4
+Version: 0.5.5
 Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
 Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
 Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
 Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_shell_craft-0.5.4/openai_shell_craft.egg-info/SOURCES.txt` & `openai_shell_craft-0.5.5/openai_shell_craft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/pyproject.toml` & `openai_shell_craft-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai_shell_craft"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
   { name="Johnathan Irvin", email="irvinjohnathan@gmail.com" },
 ]
 description = "Generating shell commands and code using natural language models (OpenAI ChatGPT)."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `openai_shell_craft-0.5.4/shell_craft/__init__.py` & `openai_shell_craft-0.5.5/shell_craft/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/__main__.py` & `openai_shell_craft-0.5.5/shell_craft/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/cli/__init__.py` & `openai_shell_craft-0.5.5/shell_craft/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/cli/help.py` & `openai_shell_craft-0.5.5/shell_craft/cli/help.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/cli/key.py` & `openai_shell_craft-0.5.5/shell_craft/cli/key.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/cli/language.py` & `openai_shell_craft-0.5.5/shell_craft/cli/language.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/cli/main.py` & `openai_shell_craft-0.5.5/shell_craft/cli/main.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/cli/models.py` & `openai_shell_craft-0.5.5/shell_craft/cli/models.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/cli/parser.py` & `openai_shell_craft-0.5.5/shell_craft/cli/parser.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/cli/prompt.py` & `openai_shell_craft-0.5.5/shell_craft/cli/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/cli/request.py` & `openai_shell_craft-0.5.5/shell_craft/cli/request.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/factories/__init__.py` & `openai_shell_craft-0.5.5/shell_craft/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/factories/prompt.py` & `openai_shell_craft-0.5.5/shell_craft/factories/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/prompts/__init__.py` & `openai_shell_craft-0.5.5/shell_craft/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/prompts/languages.py` & `openai_shell_craft-0.5.5/shell_craft/prompts/languages.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/prompts/prompt.py` & `openai_shell_craft-0.5.5/shell_craft/prompts/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,11 +51,11 @@
         }
 
         Returns:
             list[MODEL_MESSAGE]: The messages to send to the model.
         """        
         return [
             {
-                "role": "system",
+                "role": "user",
                 "content": self.content
             }
         ] + self.examples
```

### Comparing `openai_shell_craft-0.5.4/shell_craft/prompts/templates.py` & `openai_shell_craft-0.5.5/shell_craft/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/shell_craft/service.py` & `openai_shell_craft-0.5.5/shell_craft/service.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.5.4/tests/test_factories.py` & `openai_shell_craft-0.5.5/tests/test_factories.py`

 * *Files identical despite different names*


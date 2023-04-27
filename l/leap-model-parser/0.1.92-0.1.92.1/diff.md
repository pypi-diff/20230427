# Comparing `tmp/leap_model_parser-0.1.92.tar.gz` & `tmp/leap_model_parser-0.1.92.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_parser-0.1.92.tar", max compression
+gzip compressed data, was "leap_model_parser-0.1.92.1.tar", max compression
```

## Comparing `leap_model_parser-0.1.92.tar` & `leap_model_parser-0.1.92.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92/LICENSE
--rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92/README.md
--rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92/leap_model_parser/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92/leap_model_parser/contract/__init__.py
--rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92/leap_model_parser/contract/importmodelresponse.py
--rw-r--r--   0        0        0    43172 2023-04-24 08:36:26.808246 leap_model_parser-0.1.92/leap_model_parser/contract/nodedata.py
--rw-r--r--   0        0        0   414214 2023-04-24 08:36:26.808246 leap_model_parser-0.1.92/leap_model_parser/contract/ui_components.json
--rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92/leap_model_parser/keras_json_model_import.py
--rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92/leap_model_parser/model_parser.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92/leap_model_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92/leap_model_parser/utils/layerpedia/__init__.py
--rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92/leap_model_parser/utils/layerpedia/layerpedia.py
--rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92/leap_model_parser/utils/tlinspection/__init__.py
--rw-r--r--   0        0        0     2786 2023-04-24 08:36:26.808246 leap_model_parser-0.1.92/leap_model_parser/utils/tlinspection/leapinspection.py
--rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/__init__.py
--rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/generatenodedata.py
--rw-r--r--   0        0        0     5799 2023-04-24 08:36:26.808246 leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
--rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/ui_components_config.yaml
--rw-r--r--   0        0        0     1052 2023-04-24 08:38:14.580216 leap_model_parser-0.1.92/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 leap_model_parser-0.1.92/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92.1/LICENSE
+-rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92.1/README.md
+-rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92.1/leap_model_parser/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92.1/leap_model_parser/contract/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92.1/leap_model_parser/contract/importmodelresponse.py
+-rw-r--r--   0        0        0    43172 2023-04-27 14:39:00.374765 leap_model_parser-0.1.92.1/leap_model_parser/contract/nodedata.py
+-rw-r--r--   0        0        0   414214 2023-04-27 14:39:00.374765 leap_model_parser-0.1.92.1/leap_model_parser/contract/ui_components.json
+-rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92.1/leap_model_parser/keras_json_model_import.py
+-rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92.1/leap_model_parser/model_parser.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92.1/leap_model_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92.1/leap_model_parser/utils/layerpedia/__init__.py
+-rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92.1/leap_model_parser/utils/layerpedia/layerpedia.py
+-rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92.1/leap_model_parser/utils/tlinspection/__init__.py
+-rw-r--r--   0        0        0     2786 2023-04-27 14:39:00.374765 leap_model_parser-0.1.92.1/leap_model_parser/utils/tlinspection/leapinspection.py
+-rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92.1/leap_model_parser/utils/uicomponents/__init__.py
+-rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92.1/leap_model_parser/utils/uicomponents/generatenodedata.py
+-rw-r--r--   0        0        0     5799 2023-04-27 14:39:00.374765 leap_model_parser-0.1.92.1/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
+-rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92.1/leap_model_parser/utils/uicomponents/ui_components_config.yaml
+-rw-r--r--   0        0        0     1056 2023-04-27 14:40:35.287285 leap_model_parser-0.1.92.1/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 leap_model_parser-0.1.92.1/PKG-INFO
```

### Comparing `leap_model_parser-0.1.92/LICENSE` & `leap_model_parser-0.1.92.1/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/leap_model_parser/contract/importmodelresponse.py` & `leap_model_parser-0.1.92.1/leap_model_parser/contract/importmodelresponse.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/leap_model_parser/contract/nodedata.py` & `leap_model_parser-0.1.92.1/leap_model_parser/contract/nodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/leap_model_parser/contract/ui_components.json` & `leap_model_parser-0.1.92.1/leap_model_parser/contract/ui_components.json`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/leap_model_parser/keras_json_model_import.py` & `leap_model_parser-0.1.92.1/leap_model_parser/keras_json_model_import.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/leap_model_parser/model_parser.py` & `leap_model_parser-0.1.92.1/leap_model_parser/model_parser.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/leap_model_parser/utils/layerpedia/layerpedia.py` & `leap_model_parser-0.1.92.1/leap_model_parser/utils/layerpedia/layerpedia.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/leap_model_parser/utils/tlinspection/leapinspection.py` & `leap_model_parser-0.1.92.1/leap_model_parser/utils/tlinspection/leapinspection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/generatenodedata.py` & `leap_model_parser-0.1.92.1/leap_model_parser/utils/uicomponents/generatenodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/tensorflowinscpection.py` & `leap_model_parser-0.1.92.1/leap_model_parser/utils/uicomponents/tensorflowinscpection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/ui_components_config.yaml` & `leap_model_parser-0.1.92.1/leap_model_parser/utils/uicomponents/ui_components_config.yaml`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.92/pyproject.toml` & `leap_model_parser-0.1.92.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leap-model-parser"
-version = "0.1.92"
+version = "0.1.92.1"
 description = ""
 authors = ["idan <idan.yogev@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-parser"
 homepage = "https://github.com/tensorleap/leap-model-parser"
 include = [
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
 tensorflow-macos = {version = "2.11.0", markers = "platform_machine  == 'arm64'"}
 numpy = "^1.22.3"
 onnx = "1.10.1"
-onnx2kerastl = "0.0.83"
+onnx2kerastl = "0.0.83.1"
 keras-data-format-converter = "0.1.14"
 leap-model-rebuilder = "0.1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 mypy = "^0.941"
 grappa = "^1.0.1"
```

### Comparing `leap_model_parser-0.1.92/PKG-INFO` & `leap_model_parser-0.1.92.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-model-parser
-Version: 0.1.92
+Version: 0.1.92.1
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-parser
 License: MIT
 Author: idan
 Author-email: idan.yogev@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keras-data-format-converter (==0.1.14)
 Requires-Dist: leap-model-rebuilder (==0.1.5)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: onnx (==1.10.1)
-Requires-Dist: onnx2kerastl (==0.0.83)
+Requires-Dist: onnx2kerastl (==0.0.83.1)
 Requires-Dist: tensorflow (==2.11.0) ; platform_machine == "x86_64"
 Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64"
 Project-URL: Repository, https://github.com/tensorleap/leap-model-parser
 Description-Content-Type: text/markdown
 
 # Tensorleap model parser
 Used to parse model to the import format
```


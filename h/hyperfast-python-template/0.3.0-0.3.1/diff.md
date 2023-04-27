# Comparing `tmp/hyperfast_python_template-0.3.0.tar.gz` & `tmp/hyperfast_python_template-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.3.0.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.3.1.tar", max compression
```

## Comparing `hyperfast_python_template-0.3.0.tar` & `hyperfast_python_template-0.3.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1071 2023-04-27 07:14:25.134899 hyperfast_python_template-0.3.0/LICENSE
--rw-r--r--   0        0        0     5698 2023-04-27 07:14:18.682906 hyperfast_python_template-0.3.0/README.md
--rw-r--r--   0        0        0     3112 2023-04-27 07:14:40.554888 hyperfast_python_template-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6282 1970-01-01 00:00:00.000000 hyperfast_python_template-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-27 07:17:54.819143 hyperfast_python_template-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5698 2023-04-27 07:17:48.690796 hyperfast_python_template-0.3.1/README.md
+-rw-r--r--   0        0        0     3112 2023-04-27 07:18:14.036223 hyperfast_python_template-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6282 1970-01-01 00:00:00.000000 hyperfast_python_template-0.3.1/PKG-INFO
```

### Comparing `hyperfast_python_template-0.3.0/LICENSE` & `hyperfast_python_template-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.3.0/README.md` & `hyperfast_python_template-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.3.0/pyproject.toml` & `hyperfast_python_template-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.3.0"
+version = "0.3.1"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
```

### Comparing `hyperfast_python_template-0.3.0/PKG-INFO` & `hyperfast_python_template-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python template that helps you jump start your project
 Home-page: https://hyperfast-python.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```


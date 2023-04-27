# Comparing `tmp/pyXhUtils-1.3.4.tar.gz` & `tmp/pyXhUtils-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyXhUtils-1.3.4.tar", last modified: Thu Apr 27 03:35:27 2023, max compression
+gzip compressed data, was "pyXhUtils-1.3.5.tar", last modified: Thu Apr 27 03:49:24 2023, max compression
```

## Comparing `pyXhUtils-1.3.4.tar` & `pyXhUtils-1.3.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.789559 pyXhUtils-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/src/pyXhUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-27 03:35:27.000000 pyXhUtils-1.3.4/src/pyXhUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-27 03:35:27.000000 pyXhUtils-1.3.4/src/pyXhUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:35:27.000000 pyXhUtils-1.3.4/src/pyXhUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 03:35:27.000000 pyXhUtils-1.3.4/src/pyXhUtils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/src/xh_file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_file_utils/FileUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_file_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/src/xh_functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_functional/FunctionalUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/src/xh_ini_modifier/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_ini_modifier/InitModifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_ini_modifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/src/xh_utils_apache_log/
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_apache_log/ApacheLog.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_apache_log/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/src/xh_utils_file_changes/
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_file_changes/FileChanges.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_file_changes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/src/xh_utils_ip/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_ip/IpHostFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_ip/IpTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/src/xh_utils_progress/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_progress/ProgressPinger.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_progress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/src/xh_utils_script_file_writer/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_script_file_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_script_file_writer/script_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:35:27.793559 pyXhUtils-1.3.4/src/xh_utils_string/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_string/StringUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-27 03:35:14.000000 pyXhUtils-1.3.4/src/xh_utils_string/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.657330 pyXhUtils-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-27 03:49:24.653330 pyXhUtils-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 03:49:24.657330 pyXhUtils-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.641330 pyXhUtils-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.645330 pyXhUtils-1.3.5/src/pyXhUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-27 03:49:24.000000 pyXhUtils-1.3.5/src/pyXhUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-27 03:49:24.000000 pyXhUtils-1.3.5/src/pyXhUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:49:24.000000 pyXhUtils-1.3.5/src/pyXhUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 03:49:24.000000 pyXhUtils-1.3.5/src/pyXhUtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.645330 pyXhUtils-1.3.5/src/xh_file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_file_utils/FileUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_file_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.645330 pyXhUtils-1.3.5/src/xh_functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_functional/FunctionalUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.649330 pyXhUtils-1.3.5/src/xh_ini_modifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_ini_modifier/InitModifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_ini_modifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.649330 pyXhUtils-1.3.5/src/xh_utils_apache_log/
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_apache_log/ApacheLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_apache_log/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.649330 pyXhUtils-1.3.5/src/xh_utils_file_changes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_file_changes/FileChanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_file_changes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.653330 pyXhUtils-1.3.5/src/xh_utils_ip/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_ip/IpHostFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_ip/IpTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.653330 pyXhUtils-1.3.5/src/xh_utils_progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_progress/ProgressPinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_progress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.653330 pyXhUtils-1.3.5/src/xh_utils_script_file_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_script_file_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_script_file_writer/script_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:49:24.653330 pyXhUtils-1.3.5/src/xh_utils_string/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_string/StringUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-27 03:49:07.000000 pyXhUtils-1.3.5/src/xh_utils_string/__init__.py
```

### Comparing `pyXhUtils-1.3.4/LICENSE.txt` & `pyXhUtils-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.4/PKG-INFO` & `pyXhUtils-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyXhUtils
-Version: 1.3.4
+Version: 1.3.5
 Summary: A collection of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev-py/xhUtils
 Project-URL: Bug Tracker, https://github.com/xh-dev-py/xhUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyXhUtils-1.3.4/README.md` & `pyXhUtils-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.4/pyproject.toml` & `pyXhUtils-1.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyXhUtils"
-version = "1.3.4"
+version = "1.3.5"
 description = "A collection of self dev py library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = []
 [[project.authors]]
 name = "xethhung"
```

### Comparing `pyXhUtils-1.3.4/src/pyXhUtils.egg-info/PKG-INFO` & `pyXhUtils-1.3.5/src/pyXhUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyXhUtils
-Version: 1.3.4
+Version: 1.3.5
 Summary: A collection of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev-py/xhUtils
 Project-URL: Bug Tracker, https://github.com/xh-dev-py/xhUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyXhUtils-1.3.4/src/pyXhUtils.egg-info/SOURCES.txt` & `pyXhUtils-1.3.5/src/pyXhUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.4/src/xh_file_utils/FileUtils.py` & `pyXhUtils-1.3.5/src/xh_file_utils/FileUtils.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.4/src/xh_functional/FunctionalUtils.py` & `pyXhUtils-1.3.5/src/xh_functional/FunctionalUtils.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.4/src/xh_ini_modifier/InitModifier.py` & `pyXhUtils-1.3.5/src/xh_ini_modifier/InitModifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                                         )
 
     @staticmethod
     def load_as_list(file: str) -> List[OpenSSLConfigMeta]:
         return list(OpenSSLConfigLoader.load(file))
 
     @staticmethod
-    def load_as_stream(file: str) -> Stream[OpenSSLConfigMeta]:
+    def load_as_stream(file: str) -> Stream[OpenSSLConfigMeta, OpenSSLConfigMeta]:
         return Stream(OpenSSLConfigLoader.load_as_list(file))
 
 
 class IniFile:
     @staticmethod
     def batch_rename_section(parser: configparser.ConfigParser, replace_with: Callable[[str], str]):
         sections = parser.sections()
```

### Comparing `pyXhUtils-1.3.4/src/xh_utils_apache_log/ApacheLog.py` & `pyXhUtils-1.3.5/src/xh_utils_apache_log/ApacheLog.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.4/src/xh_utils_file_changes/FileChanges.py` & `pyXhUtils-1.3.5/src/xh_utils_file_changes/FileChanges.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.4/src/xh_utils_ip/IpTools.py` & `pyXhUtils-1.3.5/src/xh_utils_ip/IpTools.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.4/src/xh_utils_progress/ProgressPinger.py` & `pyXhUtils-1.3.5/src/xh_utils_progress/ProgressPinger.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.4/src/xh_utils_script_file_writer/script_writer.py` & `pyXhUtils-1.3.5/src/xh_utils_script_file_writer/script_writer.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.4/src/xh_utils_string/StringUtils.py` & `pyXhUtils-1.3.5/src/xh_utils_string/StringUtils.py`

 * *Files identical despite different names*


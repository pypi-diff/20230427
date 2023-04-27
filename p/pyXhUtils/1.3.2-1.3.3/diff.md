# Comparing `tmp/pyXhUtils-1.3.2.tar.gz` & `tmp/pyXhUtils-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyXhUtils-1.3.2.tar", last modified: Wed Apr 26 17:16:16 2023, max compression
+gzip compressed data, was "pyXhUtils-1.3.3.tar", last modified: Wed Apr 26 17:35:13 2023, max compression
```

## Comparing `pyXhUtils-1.3.2.tar` & `pyXhUtils-1.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.117009 pyXhUtils-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-26 17:16:16.117009 pyXhUtils-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:16:16.117009 pyXhUtils-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.109009 pyXhUtils-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.113009 pyXhUtils-1.3.2/src/pyXhUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-26 17:16:16.000000 pyXhUtils-1.3.2/src/pyXhUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-26 17:16:16.000000 pyXhUtils-1.3.2/src/pyXhUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:16:16.000000 pyXhUtils-1.3.2/src/pyXhUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 17:16:16.000000 pyXhUtils-1.3.2/src/pyXhUtils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.113009 pyXhUtils-1.3.2/src/xh_file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_file_utils/FileUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_file_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.113009 pyXhUtils-1.3.2/src/xh_functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_functional/FunctionalUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.113009 pyXhUtils-1.3.2/src/xh_ini_modifier/
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_ini_modifier/InitModifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_ini_modifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.113009 pyXhUtils-1.3.2/src/xh_utils_apache_log/
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_apache_log/ApacheLog.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_apache_log/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.113009 pyXhUtils-1.3.2/src/xh_utils_file_changes/
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_file_changes/FileChanges.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_file_changes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.113009 pyXhUtils-1.3.2/src/xh_utils_ip/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_ip/IpHostFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_ip/IpTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.117009 pyXhUtils-1.3.2/src/xh_utils_progress/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_progress/ProgressPinger.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_progress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.117009 pyXhUtils-1.3.2/src/xh_utils_script_file_writer/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_script_file_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_script_file_writer/script_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:16:16.117009 pyXhUtils-1.3.2/src/xh_utils_string/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_string/StringUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 17:16:04.000000 pyXhUtils-1.3.2/src/xh_utils_string/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.646333 pyXhUtils-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-26 17:35:13.646333 pyXhUtils-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:35:13.646333 pyXhUtils-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.638333 pyXhUtils-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.642333 pyXhUtils-1.3.3/src/pyXhUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-26 17:35:13.000000 pyXhUtils-1.3.3/src/pyXhUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-26 17:35:13.000000 pyXhUtils-1.3.3/src/pyXhUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:35:13.000000 pyXhUtils-1.3.3/src/pyXhUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 17:35:13.000000 pyXhUtils-1.3.3/src/pyXhUtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.642333 pyXhUtils-1.3.3/src/xh_file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_file_utils/FileUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_file_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.642333 pyXhUtils-1.3.3/src/xh_functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_functional/FunctionalUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.642333 pyXhUtils-1.3.3/src/xh_ini_modifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_ini_modifier/InitModifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_ini_modifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.642333 pyXhUtils-1.3.3/src/xh_utils_apache_log/
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_apache_log/ApacheLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_apache_log/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.642333 pyXhUtils-1.3.3/src/xh_utils_file_changes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_file_changes/FileChanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_file_changes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.642333 pyXhUtils-1.3.3/src/xh_utils_ip/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_ip/IpHostFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_ip/IpTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.646333 pyXhUtils-1.3.3/src/xh_utils_progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_progress/ProgressPinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_progress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.646333 pyXhUtils-1.3.3/src/xh_utils_script_file_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_script_file_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_script_file_writer/script_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:35:13.646333 pyXhUtils-1.3.3/src/xh_utils_string/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_string/StringUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 17:34:42.000000 pyXhUtils-1.3.3/src/xh_utils_string/__init__.py
```

### Comparing `pyXhUtils-1.3.2/LICENSE.txt` & `pyXhUtils-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.2/PKG-INFO` & `pyXhUtils-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyXhUtils
-Version: 1.3.2
+Version: 1.3.3
 Summary: A collection of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev-py/xhUtils
 Project-URL: Bug Tracker, https://github.com/xh-dev-py/xhUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyXhUtils-1.3.2/README.md` & `pyXhUtils-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.2/pyproject.toml` & `pyXhUtils-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyXhUtils"
-version = "1.3.2"
+version = "1.3.3"
 description = "A collection of self dev py library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = []
 [[project.authors]]
 name = "xethhung"
```

### Comparing `pyXhUtils-1.3.2/src/pyXhUtils.egg-info/PKG-INFO` & `pyXhUtils-1.3.3/src/pyXhUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyXhUtils
-Version: 1.3.2
+Version: 1.3.3
 Summary: A collection of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev-py/xhUtils
 Project-URL: Bug Tracker, https://github.com/xh-dev-py/xhUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyXhUtils-1.3.2/src/pyXhUtils.egg-info/SOURCES.txt` & `pyXhUtils-1.3.3/src/pyXhUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.2/src/xh_file_utils/FileUtils.py` & `pyXhUtils-1.3.3/src/xh_file_utils/FileUtils.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,7 +20,8 @@
     def check_file(path, label="File", check_exists=True, check_is_file=False, check_is_directory=False):
         if check_exists and not os.path.exists(path):
             raise Exception(f"File[{path}] not exists")
         if check_is_file and not os.path.isfile(path):
             raise Exception(f"{label}[{path}] is not file")
         if check_is_directory and not os.path.isdir(path):
             raise Exception(f"{label}[{path}] is not directory")
+        return True
```

### Comparing `pyXhUtils-1.3.2/src/xh_functional/FunctionalUtils.py` & `pyXhUtils-1.3.3/src/xh_functional/FunctionalUtils.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.2/src/xh_ini_modifier/InitModifier.py` & `pyXhUtils-1.3.3/src/xh_ini_modifier/InitModifier.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.2/src/xh_utils_apache_log/ApacheLog.py` & `pyXhUtils-1.3.3/src/xh_utils_apache_log/ApacheLog.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.2/src/xh_utils_file_changes/FileChanges.py` & `pyXhUtils-1.3.3/src/xh_utils_file_changes/FileChanges.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.2/src/xh_utils_ip/IpTools.py` & `pyXhUtils-1.3.3/src/xh_utils_ip/IpTools.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.2/src/xh_utils_progress/ProgressPinger.py` & `pyXhUtils-1.3.3/src/xh_utils_progress/ProgressPinger.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.2/src/xh_utils_script_file_writer/script_writer.py` & `pyXhUtils-1.3.3/src/xh_utils_script_file_writer/script_writer.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.2/src/xh_utils_string/StringUtils.py` & `pyXhUtils-1.3.3/src/xh_utils_string/StringUtils.py`

 * *Files identical despite different names*


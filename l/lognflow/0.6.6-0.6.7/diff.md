# Comparing `tmp/lognflow-0.6.6.tar.gz` & `tmp/lognflow-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.6.6.tar", last modified: Thu Apr 27 10:35:39 2023, max compression
+gzip compressed data, was "lognflow-0.6.7.tar", last modified: Thu Apr 27 10:51:46 2023, max compression
```

## Comparing `lognflow-0.6.6.tar` & `lognflow-0.6.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:35:39.400457 lognflow-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-27 10:35:28.000000 lognflow-0.6.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-27 10:35:28.000000 lognflow-0.6.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-27 10:35:28.000000 lognflow-0.6.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 10:35:28.000000 lognflow-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-27 10:35:28.000000 lognflow-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-27 10:35:39.400457 lognflow-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-27 10:35:28.000000 lognflow-0.6.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:35:39.400457 lognflow-0.6.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 10:35:28.000000 lognflow-0.6.6/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:35:39.400457 lognflow-0.6.6/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 10:35:28.000000 lognflow-0.6.6/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69493 2023-04-27 10:35:28.000000 lognflow-0.6.6/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-27 10:35:28.000000 lognflow-0.6.6/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-27 10:35:28.000000 lognflow-0.6.6/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:35:39.400457 lognflow-0.6.6/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 10:35:39.000000 lognflow-0.6.6/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 10:35:39.404457 lognflow-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-27 10:35:28.000000 lognflow-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:35:39.400457 lognflow-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 10:35:28.000000 lognflow-0.6.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-27 10:35:28.000000 lognflow-0.6.6/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-27 10:35:28.000000 lognflow-0.6.6/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-27 10:35:28.000000 lognflow-0.6.6/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:51:46.291388 lognflow-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-27 10:51:32.000000 lognflow-0.6.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-27 10:51:32.000000 lognflow-0.6.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-27 10:51:32.000000 lognflow-0.6.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 10:51:32.000000 lognflow-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-27 10:51:32.000000 lognflow-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-27 10:51:46.291388 lognflow-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-27 10:51:32.000000 lognflow-0.6.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:51:46.287388 lognflow-0.6.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:51:46.287388 lognflow-0.6.7/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 10:51:32.000000 lognflow-0.6.7/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69530 2023-04-27 10:51:32.000000 lognflow-0.6.7/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-27 10:51:32.000000 lognflow-0.6.7/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-27 10:51:32.000000 lognflow-0.6.7/lognflow/printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:51:46.287388 lognflow-0.6.7/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 10:51:46.291388 lognflow-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-27 10:51:32.000000 lognflow-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:51:46.287388 lognflow-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 10:51:32.000000 lognflow-0.6.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-27 10:51:32.000000 lognflow-0.6.7/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-27 10:51:32.000000 lognflow-0.6.7/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-27 10:51:32.000000 lognflow-0.6.7/tests/test_printprogress.py
```

### Comparing `lognflow-0.6.6/CONTRIBUTING.rst` & `lognflow-0.6.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/HISTORY.rst` & `lognflow-0.6.7/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -61,11 +61,15 @@
 
 0.6.5 (2023-04-26)
 ------------------
 * Fixed a bug in the docs to allow sphinx compile it.
 * log_var will log only the valid time stamps.
 * added end keyword argument to log_text
 
-0.6.6 (2023-05-01)
+0.6.6 (2023-04-27)
 ------------------
 * Better documentation
-* added tifffile imread to logviewer and imwrite to lognflow
+* added tifffile imread to logviewer and imwrite to lognflow
+
+0.6.7 (2023-04-27)
+------------------
+* A bug in tifffile support was fixed
```

### Comparing `lognflow-0.6.6/LICENSE` & `lognflow-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/PKG-INFO` & `lognflow-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.6.6
+Version: 0.6.7
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -171,11 +171,15 @@
 
 0.6.5 (2023-04-26)
 ------------------
 * Fixed a bug in the docs to allow sphinx compile it.
 * log_var will log only the valid time stamps.
 * added end keyword argument to log_text
 
-0.6.6 (2023-05-01)
+0.6.6 (2023-04-27)
 ------------------
 * Better documentation
 * added tifffile imread to logviewer and imwrite to lognflow
+
+0.6.7 (2023-04-27)
+------------------
+* A bug in tifffile support was fixed
```

### Comparing `lognflow-0.6.6/README.rst` & `lognflow-0.6.7/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/docs/Makefile` & `lognflow-0.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/docs/conf.py` & `lognflow-0.6.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/docs/installation.rst` & `lognflow-0.6.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/docs/make.bat` & `lognflow-0.6.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/lognflow/lognflow.py` & `lognflow-0.6.7/lognflow/lognflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,28 +570,30 @@
         param_dir, param_name = self._prepare_param_dir(parameter_name)
         fpath = self._get_fpath(param_dir, param_name, save_as, time_tag)
             
         if(save_as == 'npy'):
             np.save(fpath, parameter_value)
         elif(save_as == 'npz'):
             np.savez(fpath, **parameter_value)
-        elif((save_as == '.tif') | (save_as == '.tiff')):
+        elif((save_as == 'tif') | (save_as == 'tiff')):
             from tifffile import imwrite
             imwrite(fpath, parameter_value)
         elif(save_as == 'txt'):
             with open(fpath,'a') as fdata: 
                 fdata.write(str(parameter_value))
         elif(save_as == 'mat'):
             from scipy.io import savemat
             if(mat_field is None):
                 mat_field = param_name
             savemat(fpath, {f'{mat_field}':parameter_value})
         elif(save_as == 'torch'):
             from torch import save as torch_save
             torch_save(parameter_value.state_dict(), fpath)
+        else:
+            fpath = None
         return fpath
     
     def log_plt(self, 
                 parameter_name: str, 
                 image_format='jpeg', dpi=1200,
                 time_tag: bool = None,
                 close_plt = True):
```

### Comparing `lognflow-0.6.6/lognflow/logviewer.py` & `lognflow-0.6.7/lognflow/logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/lognflow/printprogress.py` & `lognflow-0.6.7/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/lognflow.egg-info/PKG-INFO` & `lognflow-0.6.7/lognflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.6.6
+Version: 0.6.7
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -171,11 +171,15 @@
 
 0.6.5 (2023-04-26)
 ------------------
 * Fixed a bug in the docs to allow sphinx compile it.
 * log_var will log only the valid time stamps.
 * added end keyword argument to log_text
 
-0.6.6 (2023-05-01)
+0.6.6 (2023-04-27)
 ------------------
 * Better documentation
 * added tifffile imread to logviewer and imwrite to lognflow
+
+0.6.7 (2023-04-27)
+------------------
+* A bug in tifffile support was fixed
```

### Comparing `lognflow-0.6.6/lognflow.egg-info/SOURCES.txt` & `lognflow-0.6.7/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/setup.py` & `lognflow-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.6.6'
+__version__ = '0.6.7'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.6.6/tests/test_lognflow.py` & `lognflow-0.6.7/tests/test_lognflow.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/tests/test_logviewer.py` & `lognflow-0.6.7/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.6/tests/test_printprogress.py` & `lognflow-0.6.7/tests/test_printprogress.py`

 * *Files identical despite different names*


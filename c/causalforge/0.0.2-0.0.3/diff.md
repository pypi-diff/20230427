# Comparing `tmp/causalforge-0.0.2.tar.gz` & `tmp/causalforge-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalforge-0.0.2.tar", last modified: Wed Apr 26 22:51:24 2023, max compression
+gzip compressed data, was "causalforge-0.0.3.tar", last modified: Wed Apr 26 23:08:40 2023, max compression
```

## Comparing `causalforge-0.0.2.tar` & `causalforge-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 22:51:24.056101 causalforge-0.0.2/
--rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.2/LICENSE
--rw-r--r--   0 AG62216    (501) staff       (20)     2421 2023-04-26 22:51:24.056230 causalforge-0.0.2/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)     1986 2023-04-26 22:41:54.000000 causalforge-0.0.2/README.md
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 22:51:24.051906 causalforge-0.0.2/causalforge/
--rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-04-26 22:48:26.000000 causalforge-0.0.2/causalforge/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 22:51:24.055638 causalforge-0.0.2/causalforge/tests/
--rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.2/causalforge/tests/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 22:51:24.054997 causalforge-0.0.2/causalforge.egg-info/
--rw-r--r--   0 AG62216    (501) staff       (20)     2421 2023-04-26 22:51:23.000000 causalforge-0.0.2/causalforge.egg-info/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-04-26 22:51:24.000000 causalforge-0.0.2/causalforge.egg-info/SOURCES.txt
--rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-04-26 22:51:23.000000 causalforge-0.0.2/causalforge.egg-info/dependency_links.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      134 2023-04-26 22:51:23.000000 causalforge-0.0.2/causalforge.egg-info/requires.txt
--rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-04-26 22:51:23.000000 causalforge-0.0.2/causalforge.egg-info/top_level.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-04-26 22:51:24.056851 causalforge-0.0.2/setup.cfg
--rw-r--r--   0 AG62216    (501) staff       (20)     1606 2023-04-26 20:06:00.000000 causalforge-0.0.2/setup.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:08:40.504611 causalforge-0.0.3/
+-rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.3/LICENSE
+-rw-r--r--   0 AG62216    (501) staff       (20)     2473 2023-04-26 23:08:40.504743 causalforge-0.0.3/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)     2038 2023-04-26 23:08:00.000000 causalforge-0.0.3/README.md
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:08:40.499684 causalforge-0.0.3/causalforge/
+-rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-04-26 23:08:00.000000 causalforge-0.0.3/causalforge/__init__.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:08:40.504194 causalforge-0.0.3/causalforge/tests/
+-rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.3/causalforge/tests/__init__.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:08:40.503547 causalforge-0.0.3/causalforge.egg-info/
+-rw-r--r--   0 AG62216    (501) staff       (20)     2473 2023-04-26 23:08:40.000000 causalforge-0.0.3/causalforge.egg-info/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-04-26 23:08:40.000000 causalforge-0.0.3/causalforge.egg-info/SOURCES.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-04-26 23:08:40.000000 causalforge-0.0.3/causalforge.egg-info/dependency_links.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      134 2023-04-26 23:08:40.000000 causalforge-0.0.3/causalforge.egg-info/requires.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-04-26 23:08:40.000000 causalforge-0.0.3/causalforge.egg-info/top_level.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-04-26 23:08:40.505371 causalforge-0.0.3/setup.cfg
+-rw-r--r--   0 AG62216    (501) staff       (20)     1606 2023-04-26 20:06:00.000000 causalforge-0.0.3/setup.py
```

### Comparing `causalforge-0.0.2/LICENSE` & `causalforge-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.2/PKG-INFO` & `causalforge-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Package for Causal Inference
 Home-page: https://gitlab.com/gtesei/causalFlow
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img alt="autoimpute-logo" class="causalFlow-logo"  height="250" width="300"  src="logo.png">
+<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://github.com/anthem-ai/causalflow/blob/main/logo.png">
 
 # CausalFlow
 
 [![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
 [![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
```

### Comparing `causalforge-0.0.2/README.md` & `causalforge-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img alt="autoimpute-logo" class="causalFlow-logo"  height="250" width="300"  src="logo.png">
+<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://github.com/anthem-ai/causalflow/blob/main/logo.png">
 
 # CausalFlow
 
 [![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
 [![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
```

### Comparing `causalforge-0.0.2/causalforge.egg-info/PKG-INFO` & `causalforge-0.0.3/causalforge.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Package for Causal Inference
 Home-page: https://gitlab.com/gtesei/causalFlow
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img alt="autoimpute-logo" class="causalFlow-logo"  height="250" width="300"  src="logo.png">
+<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://github.com/anthem-ai/causalflow/blob/main/logo.png">
 
 # CausalFlow
 
 [![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
 [![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
```

### Comparing `causalforge-0.0.2/setup.py` & `causalforge-0.0.3/setup.py`

 * *Files identical despite different names*


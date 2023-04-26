# Comparing `tmp/causalforge-0.0.4.tar.gz` & `tmp/causalforge-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalforge-0.0.4.tar", last modified: Wed Apr 26 23:17:11 2023, max compression
+gzip compressed data, was "causalforge-0.0.5.tar", last modified: Wed Apr 26 23:22:24 2023, max compression
```

## Comparing `causalforge-0.0.4.tar` & `causalforge-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:17:11.920596 causalforge-0.0.4/
--rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.4/LICENSE
--rw-r--r--   0 AG62216    (501) staff       (20)     2489 2023-04-26 23:17:11.920750 causalforge-0.0.4/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)     2038 2023-04-26 23:08:00.000000 causalforge-0.0.4/README.md
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:17:11.915798 causalforge-0.0.4/causalforge/
--rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-04-26 23:16:11.000000 causalforge-0.0.4/causalforge/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:17:11.920162 causalforge-0.0.4/causalforge/tests/
--rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.4/causalforge/tests/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:17:11.919373 causalforge-0.0.4/causalforge.egg-info/
--rw-r--r--   0 AG62216    (501) staff       (20)     2489 2023-04-26 23:17:11.000000 causalforge-0.0.4/causalforge.egg-info/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-04-26 23:17:11.000000 causalforge-0.0.4/causalforge.egg-info/SOURCES.txt
--rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-04-26 23:17:11.000000 causalforge-0.0.4/causalforge.egg-info/dependency_links.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      134 2023-04-26 23:17:11.000000 causalforge-0.0.4/causalforge.egg-info/requires.txt
--rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-04-26 23:17:11.000000 causalforge-0.0.4/causalforge.egg-info/top_level.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-04-26 23:17:11.921433 causalforge-0.0.4/setup.cfg
--rw-r--r--   0 AG62216    (501) staff       (20)     1659 2023-04-26 23:15:59.000000 causalforge-0.0.4/setup.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:22:24.868419 causalforge-0.0.5/
+-rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.5/LICENSE
+-rw-r--r--   0 AG62216    (501) staff       (20)     2499 2023-04-26 23:22:24.868624 causalforge-0.0.5/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)     2048 2023-04-26 23:21:19.000000 causalforge-0.0.5/README.md
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:22:24.863670 causalforge-0.0.5/causalforge/
+-rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-04-26 23:21:33.000000 causalforge-0.0.5/causalforge/__init__.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:22:24.867959 causalforge-0.0.5/causalforge/tests/
+-rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.5/causalforge/tests/__init__.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:22:24.867195 causalforge-0.0.5/causalforge.egg-info/
+-rw-r--r--   0 AG62216    (501) staff       (20)     2499 2023-04-26 23:22:24.000000 causalforge-0.0.5/causalforge.egg-info/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-04-26 23:22:24.000000 causalforge-0.0.5/causalforge.egg-info/SOURCES.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-04-26 23:22:24.000000 causalforge-0.0.5/causalforge.egg-info/dependency_links.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      134 2023-04-26 23:22:24.000000 causalforge-0.0.5/causalforge.egg-info/requires.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-04-26 23:22:24.000000 causalforge-0.0.5/causalforge.egg-info/top_level.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-04-26 23:22:24.869594 causalforge-0.0.5/setup.cfg
+-rw-r--r--   0 AG62216    (501) staff       (20)     1659 2023-04-26 23:15:59.000000 causalforge-0.0.5/setup.py
```

### Comparing `causalforge-0.0.4/LICENSE` & `causalforge-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.4/PKG-INFO` & `causalforge-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Package for Causal Inference
 Home-page: https://github.com/anthem-ai/causalflow
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://github.com/anthem-ai/causalflow/blob/main/logo.png">
+<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalflow/main/logo.png">
 
 # CausalFlow
 
 [![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
 [![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
```

### Comparing `causalforge-0.0.4/README.md` & `causalforge-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://github.com/anthem-ai/causalflow/blob/main/logo.png">
+<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalflow/main/logo.png">
 
 # CausalFlow
 
 [![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
 [![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
```

### Comparing `causalforge-0.0.4/causalforge.egg-info/PKG-INFO` & `causalforge-0.0.5/causalforge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Package for Causal Inference
 Home-page: https://github.com/anthem-ai/causalflow
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://github.com/anthem-ai/causalflow/blob/main/logo.png">
+<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalflow/main/logo.png">
 
 # CausalFlow
 
 [![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
 [![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
```

### Comparing `causalforge-0.0.4/setup.py` & `causalforge-0.0.5/setup.py`

 * *Files identical despite different names*


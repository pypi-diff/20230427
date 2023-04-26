# Comparing `tmp/causalforge-0.0.1.tar.gz` & `tmp/causalforge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalforge-0.0.1.tar", last modified: Wed Apr 26 01:08:56 2023, max compression
+gzip compressed data, was "causalforge-0.0.2.tar", last modified: Wed Apr 26 22:51:24 2023, max compression
```

## Comparing `causalforge-0.0.1.tar` & `causalforge-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 01:08:56.727446 causalforge-0.0.1/
--rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.1/LICENSE
--rw-r--r--   0 AG62216    (501) staff       (20)     2791 2023-04-26 01:08:56.727580 causalforge-0.0.1/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)     2356 2023-04-25 21:02:01.000000 causalforge-0.0.1/README.md
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 01:08:56.722641 causalforge-0.0.1/causalforge/
--rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-04-22 02:11:58.000000 causalforge-0.0.1/causalforge/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 01:08:56.726969 causalforge-0.0.1/causalforge/tests/
--rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.1/causalforge/tests/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 01:08:56.726162 causalforge-0.0.1/causalforge.egg-info/
--rw-r--r--   0 AG62216    (501) staff       (20)     2791 2023-04-26 01:08:56.000000 causalforge-0.0.1/causalforge.egg-info/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-04-26 01:08:56.000000 causalforge-0.0.1/causalforge.egg-info/SOURCES.txt
--rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-04-26 01:08:56.000000 causalforge-0.0.1/causalforge.egg-info/dependency_links.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      125 2023-04-26 01:08:56.000000 causalforge-0.0.1/causalforge.egg-info/requires.txt
--rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-04-26 01:08:56.000000 causalforge-0.0.1/causalforge.egg-info/top_level.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-04-26 01:08:56.728188 causalforge-0.0.1/setup.cfg
--rw-r--r--   0 AG62216    (501) staff       (20)     1606 2023-04-26 01:08:51.000000 causalforge-0.0.1/setup.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 22:51:24.056101 causalforge-0.0.2/
+-rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.2/LICENSE
+-rw-r--r--   0 AG62216    (501) staff       (20)     2421 2023-04-26 22:51:24.056230 causalforge-0.0.2/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)     1986 2023-04-26 22:41:54.000000 causalforge-0.0.2/README.md
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 22:51:24.051906 causalforge-0.0.2/causalforge/
+-rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-04-26 22:48:26.000000 causalforge-0.0.2/causalforge/__init__.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 22:51:24.055638 causalforge-0.0.2/causalforge/tests/
+-rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.2/causalforge/tests/__init__.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 22:51:24.054997 causalforge-0.0.2/causalforge.egg-info/
+-rw-r--r--   0 AG62216    (501) staff       (20)     2421 2023-04-26 22:51:23.000000 causalforge-0.0.2/causalforge.egg-info/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-04-26 22:51:24.000000 causalforge-0.0.2/causalforge.egg-info/SOURCES.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-04-26 22:51:23.000000 causalforge-0.0.2/causalforge.egg-info/dependency_links.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      134 2023-04-26 22:51:23.000000 causalforge-0.0.2/causalforge.egg-info/requires.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-04-26 22:51:23.000000 causalforge-0.0.2/causalforge.egg-info/top_level.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-04-26 22:51:24.056851 causalforge-0.0.2/setup.cfg
+-rw-r--r--   0 AG62216    (501) staff       (20)     1606 2023-04-26 20:06:00.000000 causalforge-0.0.2/setup.py
```

### Comparing `causalforge-0.0.1/LICENSE` & `causalforge-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.1/PKG-INFO` & `causalforge-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Package for Causal Inference
 Home-page: https://gitlab.com/gtesei/causalFlow
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,18 +12,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img alt="autoimpute-logo" class="causalFlow-logo"  height="250" width="300"  src="logo.png">
 
 # CausalFlow
 
-[![Build Status](https://api.travis-ci.org/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV.svg?branch=master)](https://travis-ci.org/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV)
-[![PyPI version](https://badge.fury.io/py/python-dev-docker-project.svg)](https://badge.fury.io/py/python-dev-docker-project)
-[![Coverage Status](https://coveralls.io/repos/github/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV/badge.svg?branch=master)](https://coveralls.io/github/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV?branch=master)
-[![Documentation Status](https://readthedocs.org/projects/patterns-for-continuous-integration-docker-travis-ci-2-dev/badge/?version=latest)](https://patterns-for-continuous-integration-docker-travis-ci-2-dev.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
+[![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+
 
 CausalFlow is a Python package that provides a suite of modeling & causal inference methods using machine learning algorithms based on Elevence Health recent research. It provides convenient APIs that allow to estimate Propensity Score, Average Treatment Effect (ATE), Conditional Average Treatment Effect (CATE) or Individual Treatment Effect (ITE) 
 from experimental or observational data.
 
 <details>
   <summary> <H3>Installing Python Package</H3>  </summary>
```

### Comparing `causalforge-0.0.1/README.md` & `causalforge-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <img alt="autoimpute-logo" class="causalFlow-logo"  height="250" width="300"  src="logo.png">
 
 # CausalFlow
 
-[![Build Status](https://api.travis-ci.org/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV.svg?branch=master)](https://travis-ci.org/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV)
-[![PyPI version](https://badge.fury.io/py/python-dev-docker-project.svg)](https://badge.fury.io/py/python-dev-docker-project)
-[![Coverage Status](https://coveralls.io/repos/github/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV/badge.svg?branch=master)](https://coveralls.io/github/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV?branch=master)
-[![Documentation Status](https://readthedocs.org/projects/patterns-for-continuous-integration-docker-travis-ci-2-dev/badge/?version=latest)](https://patterns-for-continuous-integration-docker-travis-ci-2-dev.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
+[![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+
 
 CausalFlow is a Python package that provides a suite of modeling & causal inference methods using machine learning algorithms based on Elevence Health recent research. It provides convenient APIs that allow to estimate Propensity Score, Average Treatment Effect (ATE), Conditional Average Treatment Effect (CATE) or Individual Treatment Effect (ITE) 
 from experimental or observational data.
 
 <details>
   <summary> <H3>Installing Python Package</H3>  </summary>
```

### Comparing `causalforge-0.0.1/causalforge.egg-info/PKG-INFO` & `causalforge-0.0.2/causalforge.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Package for Causal Inference
 Home-page: https://gitlab.com/gtesei/causalFlow
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,18 +12,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img alt="autoimpute-logo" class="causalFlow-logo"  height="250" width="300"  src="logo.png">
 
 # CausalFlow
 
-[![Build Status](https://api.travis-ci.org/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV.svg?branch=master)](https://travis-ci.org/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV)
-[![PyPI version](https://badge.fury.io/py/python-dev-docker-project.svg)](https://badge.fury.io/py/python-dev-docker-project)
-[![Coverage Status](https://coveralls.io/repos/github/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV/badge.svg?branch=master)](https://coveralls.io/github/gtesei/Patterns_for_Continuous_Integration_Docker_Travis_CI_2_DEV?branch=master)
-[![Documentation Status](https://readthedocs.org/projects/patterns-for-continuous-integration-docker-travis-ci-2-dev/badge/?version=latest)](https://patterns-for-continuous-integration-docker-travis-ci-2-dev.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
+[![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+
 
 CausalFlow is a Python package that provides a suite of modeling & causal inference methods using machine learning algorithms based on Elevence Health recent research. It provides convenient APIs that allow to estimate Propensity Score, Average Treatment Effect (ATE), Conditional Average Treatment Effect (CATE) or Individual Treatment Effect (ITE) 
 from experimental or observational data.
 
 <details>
   <summary> <H3>Installing Python Package</H3>  </summary>
```

### Comparing `causalforge-0.0.1/setup.py` & `causalforge-0.0.2/setup.py`

 * *Files identical despite different names*


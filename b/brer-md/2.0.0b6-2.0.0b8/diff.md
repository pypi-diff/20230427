# Comparing `tmp/brer-md-2.0.0b6.tar.gz` & `tmp/brer-md-2.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/eric/develop/PycharmProjects/run_brer/dist/.tmp-udo5rf0m/brer-md-2.0.0b6.tar", last modified: Thu Mar  2 14:27:11 2023, max compression
+gzip compressed data, was "/Users/eric/develop/PycharmProjects/run_brer/dist/.tmp-7uok5ooc/brer-md-2.0.0b8.tar", last modified: Thu Apr 27 15:28:24 2023, max compression
```

## Comparing `brer-md-2.0.0b6.tar` & `brer-md-2.0.0b8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-02 14:27:11.547567 brer-md-2.0.0b6/
--rw-r--r--   0 eric       (501) staff       (20)    26526 2020-06-17 12:45:59.000000 brer-md-2.0.0b6/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      178 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)    10459 2023-03-02 14:27:11.546988 brer-md-2.0.0b6/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     9844 2023-03-02 14:25:20.000000 brer-md-2.0.0b6/README.rst
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-02 14:27:11.497252 brer-md-2.0.0b6/_custom_build/
--rw-r--r--   0 eric       (501) staff       (20)    25208 2022-12-24 14:58:23.000000 brer-md-2.0.0b6/_custom_build/backend.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-02 14:27:11.500896 brer-md-2.0.0b6/brer_md.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)    10459 2023-03-02 14:27:11.000000 brer-md-2.0.0b6/brer_md.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1164 2023-03-02 14:27:11.000000 brer-md-2.0.0b6/brer_md.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-03-02 14:27:11.000000 brer-md-2.0.0b6/brer_md.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2022-12-22 15:25:32.000000 brer-md-2.0.0b6/brer_md.egg-info/not-zip-safe
--rw-r--r--   0 eric       (501) staff       (20)       86 2023-03-02 14:27:11.000000 brer-md-2.0.0b6/brer_md.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)        5 2023-03-02 14:27:11.000000 brer-md-2.0.0b6/brer_md.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)     2161 2022-11-02 13:51:10.000000 brer-md-2.0.0b6/pyproject.toml
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-03-02 14:27:11.547765 brer-md-2.0.0b6/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      714 2022-12-24 14:57:26.000000 brer-md-2.0.0b6/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-02 14:27:11.493981 brer-md-2.0.0b6/src/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-02 14:27:11.506482 brer-md-2.0.0b6/src/brer/
--rw-r--r--   0 eric       (501) staff       (20)      487 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/brer/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     2088 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/brer/_compat.py
--rw-r--r--   0 eric       (501) staff       (20)       24 2023-03-02 14:27:11.000000 brer-md-2.0.0b6/src/brer/_version.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-02 14:27:11.507753 brer-md-2.0.0b6/src/brer/data/
--rw-r--r--   0 eric       (501) staff       (20)     7360 2022-11-29 14:58:02.000000 brer-md-2.0.0b6/src/brer/data/pair_data.json
--rw-r--r--   0 eric       (501) staff       (20)  7552688 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/brer/data/topol.tpr
--rw-r--r--   0 eric       (501) staff       (20)     4394 2022-11-02 12:54:55.000000 brer-md-2.0.0b6/src/brer/directory_helper.py
--rw-r--r--   0 eric       (501) staff       (20)     6440 2022-11-30 14:57:08.000000 brer-md-2.0.0b6/src/brer/pair_data.py
--rw-r--r--   0 eric       (501) staff       (20)     6490 2022-11-02 12:54:55.000000 brer-md-2.0.0b6/src/brer/plugin_configs.py
--rw-r--r--   0 eric       (501) staff       (20)        0 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/brer/py.typed
--rw-r--r--   0 eric       (501) staff       (20)    29188 2022-12-24 14:58:23.000000 brer-md-2.0.0b6/src/brer/run_config.py
--rw-r--r--   0 eric       (501) staff       (20)    12336 2022-12-22 09:40:59.000000 brer-md-2.0.0b6/src/brer/run_data.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-02 14:27:11.524205 brer-md-2.0.0b6/src/plugin/
--rw-r--r--   0 eric       (501) staff       (20)     3171 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/CMakeLists.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-02 14:27:11.534898 brer-md-2.0.0b6/src/plugin/cpp/
--rw-r--r--   0 eric       (501) staff       (20)     2847 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/cpp/CMakeLists.txt
--rw-r--r--   0 eric       (501) staff       (20)     5959 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/cpp/brerpotential.cpp
--rw-r--r--   0 eric       (501) staff       (20)     5932 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/cpp/brerpotential.h
--rw-r--r--   0 eric       (501) staff       (20)     2778 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/cpp/linearpotential.cpp
--rw-r--r--   0 eric       (501) staff       (20)     2778 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/cpp/linearpotential.h
--rw-r--r--   0 eric       (501) staff       (20)     4150 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/cpp/linearstoppotential.cpp
--rw-r--r--   0 eric       (501) staff       (20)     4220 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/cpp/linearstoppotential.h
--rw-r--r--   0 eric       (501) staff       (20)     1786 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/cpp/sessionresources.cpp
--rw-r--r--   0 eric       (501) staff       (20)    13977 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/cpp/sessionresources.h
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-02 14:27:11.537718 brer-md-2.0.0b6/src/plugin/pythonmodule/
--rw-r--r--   0 eric       (501) staff       (20)     1049 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/pythonmodule/CMakeLists.txt
--rw-r--r--   0 eric       (501) staff       (20)    24487 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/pythonmodule/export_plugin.cpp
--rw-r--r--   0 eric       (501) staff       (20)      198 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/src/plugin/pythonmodule/export_plugin.h
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-02 14:27:11.545508 brer-md-2.0.0b6/tests/
--rw-r--r--   0 eric       (501) staff       (20)       26 2022-09-23 11:55:27.000000 brer-md-2.0.0b6/tests/pytest.ini
--rw-r--r--   0 eric       (501) staff       (20)      698 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/tests/test_dirhelper.py
--rw-r--r--   0 eric       (501) staff       (20)     1407 2022-11-30 14:32:15.000000 brer-md-2.0.0b6/tests/test_pair_data.py
--rw-r--r--   0 eric       (501) staff       (20)     1977 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/tests/test_plugin_binding.py
--rw-r--r--   0 eric       (501) staff       (20)     1770 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/tests/test_plugin_configs.py
--rw-r--r--   0 eric       (501) staff       (20)     6439 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/tests/test_run_config.py
--rw-r--r--   0 eric       (501) staff       (20)     2897 2022-11-30 15:01:51.000000 brer-md-2.0.0b6/tests/test_run_data.py
--rw-r--r--   0 eric       (501) staff       (20)    49825 2022-10-31 13:13:27.000000 brer-md-2.0.0b6/tests/testdata.json
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:24.032871 brer-md-2.0.0b8/
+-rw-r--r--   0 eric       (501) staff       (20)    26526 2020-06-17 12:45:59.000000 brer-md-2.0.0b8/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      178 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)    10504 2023-04-27 15:28:24.032062 brer-md-2.0.0b8/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     9889 2023-04-25 00:36:25.000000 brer-md-2.0.0b8/README.rst
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.936930 brer-md-2.0.0b8/_custom_build/
+-rw-r--r--   0 eric       (501) staff       (20)    25208 2022-12-24 14:58:23.000000 brer-md-2.0.0b8/_custom_build/backend.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.942583 brer-md-2.0.0b8/brer_md.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)    10504 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/brer_md.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1164 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/brer_md.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/brer_md.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2022-12-22 15:25:32.000000 brer-md-2.0.0b8/brer_md.egg-info/not-zip-safe
+-rw-r--r--   0 eric       (501) staff       (20)       86 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/brer_md.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)        5 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/brer_md.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)     2161 2023-04-26 22:54:28.000000 brer-md-2.0.0b8/pyproject.toml
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-04-27 15:28:24.033124 brer-md-2.0.0b8/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      714 2022-12-24 14:57:26.000000 brer-md-2.0.0b8/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.931124 brer-md-2.0.0b8/src/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.954122 brer-md-2.0.0b8/src/brer/
+-rw-r--r--   0 eric       (501) staff       (20)      487 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/brer/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     2088 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/brer/_compat.py
+-rw-r--r--   0 eric       (501) staff       (20)       24 2023-04-27 15:28:23.000000 brer-md-2.0.0b8/src/brer/_version.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.956401 brer-md-2.0.0b8/src/brer/data/
+-rw-r--r--   0 eric       (501) staff       (20)     7360 2022-11-29 14:58:02.000000 brer-md-2.0.0b8/src/brer/data/pair_data.json
+-rw-r--r--   0 eric       (501) staff       (20)  7552688 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/brer/data/topol.tpr
+-rw-r--r--   0 eric       (501) staff       (20)     4394 2022-11-02 12:54:55.000000 brer-md-2.0.0b8/src/brer/directory_helper.py
+-rw-r--r--   0 eric       (501) staff       (20)     6440 2022-11-30 14:57:08.000000 brer-md-2.0.0b8/src/brer/pair_data.py
+-rw-r--r--   0 eric       (501) staff       (20)     6490 2022-11-02 12:54:55.000000 brer-md-2.0.0b8/src/brer/plugin_configs.py
+-rw-r--r--   0 eric       (501) staff       (20)        0 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/brer/py.typed
+-rw-r--r--   0 eric       (501) staff       (20)    30367 2023-04-26 23:00:44.000000 brer-md-2.0.0b8/src/brer/run_config.py
+-rw-r--r--   0 eric       (501) staff       (20)    12336 2022-12-22 09:40:59.000000 brer-md-2.0.0b8/src/brer/run_data.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:23.988483 brer-md-2.0.0b8/src/plugin/
+-rw-r--r--   0 eric       (501) staff       (20)     3171 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/CMakeLists.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:24.005318 brer-md-2.0.0b8/src/plugin/cpp/
+-rw-r--r--   0 eric       (501) staff       (20)     2847 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/CMakeLists.txt
+-rw-r--r--   0 eric       (501) staff       (20)     5959 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/brerpotential.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     5932 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/brerpotential.h
+-rw-r--r--   0 eric       (501) staff       (20)     2778 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/linearpotential.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     2778 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/linearpotential.h
+-rw-r--r--   0 eric       (501) staff       (20)     4150 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/linearstoppotential.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     4220 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/linearstoppotential.h
+-rw-r--r--   0 eric       (501) staff       (20)     1786 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/sessionresources.cpp
+-rw-r--r--   0 eric       (501) staff       (20)    13977 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/cpp/sessionresources.h
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:24.009788 brer-md-2.0.0b8/src/plugin/pythonmodule/
+-rw-r--r--   0 eric       (501) staff       (20)     1049 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/pythonmodule/CMakeLists.txt
+-rw-r--r--   0 eric       (501) staff       (20)    24487 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/pythonmodule/export_plugin.cpp
+-rw-r--r--   0 eric       (501) staff       (20)      198 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/src/plugin/pythonmodule/export_plugin.h
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-27 15:28:24.024578 brer-md-2.0.0b8/tests/
+-rw-r--r--   0 eric       (501) staff       (20)       26 2022-09-23 11:55:27.000000 brer-md-2.0.0b8/tests/pytest.ini
+-rw-r--r--   0 eric       (501) staff       (20)      698 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/tests/test_dirhelper.py
+-rw-r--r--   0 eric       (501) staff       (20)     1407 2022-11-30 14:32:15.000000 brer-md-2.0.0b8/tests/test_pair_data.py
+-rw-r--r--   0 eric       (501) staff       (20)     1977 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/tests/test_plugin_binding.py
+-rw-r--r--   0 eric       (501) staff       (20)     1770 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/tests/test_plugin_configs.py
+-rw-r--r--   0 eric       (501) staff       (20)     7561 2023-04-27 15:26:23.000000 brer-md-2.0.0b8/tests/test_run_config.py
+-rw-r--r--   0 eric       (501) staff       (20)     2910 2023-04-25 00:58:43.000000 brer-md-2.0.0b8/tests/test_run_data.py
+-rw-r--r--   0 eric       (501) staff       (20)    49825 2022-10-31 13:13:27.000000 brer-md-2.0.0b8/tests/testdata.json
```

### Comparing `brer-md-2.0.0b6/LICENSE` & `brer-md-2.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/PKG-INFO` & `brer-md-2.0.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brer-md
-Version: 2.0.0b6
+Version: 2.0.0b8
 Summary: A set of scripts for running BRER simulations using gmxapi.
 Author: Jennifer M. Hays, Kasson Lab BRER Team
 Author-email: Kasson Lab BRER Team <kassonlab@gmail.com>
 License: LGPL 2.1
 Project-URL: Source, https://github.com/kassonlab/brer-md/
 Project-URL: Documentation, https://kassonlab.github.io/brer-md/
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
@@ -19,15 +19,15 @@
 
 |Build and test| |Documentation| |codecov|
 
 Source: https://github.com/kassonlab/brer-md
 
 Documentation: https://kassonlab.github.io/brer-md/
 
-The ``brer`` Python package provides a set of scripts for running
+The ``brer-md`` Python package provides a set of scripts for running
 Bias-Resampling Ensemble Refinement (BRER) simulations using
 `gmxapi <https://gmxapi.org/>`__. Details of the BRER
 method may be found in:
 
 Hays, J. M., Cafiso, D. S., & Kasson, P. M. Hybrid Refinement of
 Heterogeneous Conformational Ensembles using Spectroscopic Data. *The
 Journal of Physical Chemistry Letters*. DOI:
@@ -41,15 +41,15 @@
 
 If you’re going to use a pip or a conda environment, you’ll need:
 
 -  Python 3.8 or newer.
 -  A GROMACS installation supporting client software builds.
 -  `gmxapi <https://manual.gromacs.org/current/gmxapi>`__ for GROMACS.
 
-``brer`` includes a simple C++ extension module that can be attached to a GROMACS
+``brer-md`` includes a simple C++ extension module that can be attached to a GROMACS
 molecular dynamics (MD) simulator through the gmxapi Python interface.
 GROMACS installations (and GROMACS dependencies) can be built rather specifically
 for their computing environments. The ``brer`` package is distributed as source
 code that must be built for a specific GROMACS installation.
 
 .. note::
     For several recent versions of GROMACS, the “legacy API” needs
@@ -84,14 +84,16 @@
 Generally, ``pip`` will automatically install any package dependencies.
 
 If a GROMACS installation is discoverable (you have "sourced" a GMXRC file or
 defined a GROMACS_DIR environment variable), then the ``gmxapi`` Python package
 will be installed automatically with the ``brer`` package.
 Simply::
 
+    pip install --pre brer-md
+    # or
     pip install git+https://github.com/kassonlab/brer-md.git
 
 If you prefer to install ``gmxapi`` separately (such as to specify an older
 package version), you can provide ``--no-deps`` and ``--no-build-isolation``
 to ``pip install``, and the existing ``gmxapi`` installation will be used.
 
 You can pre-install (other) required packages using the
```

### Comparing `brer-md-2.0.0b6/README.rst` & `brer-md-2.0.0b8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 |Build and test| |Documentation| |codecov|
 
 Source: https://github.com/kassonlab/brer-md
 
 Documentation: https://kassonlab.github.io/brer-md/
 
-The ``brer`` Python package provides a set of scripts for running
+The ``brer-md`` Python package provides a set of scripts for running
 Bias-Resampling Ensemble Refinement (BRER) simulations using
 `gmxapi <https://gmxapi.org/>`__. Details of the BRER
 method may be found in:
 
 Hays, J. M., Cafiso, D. S., & Kasson, P. M. Hybrid Refinement of
 Heterogeneous Conformational Ensembles using Spectroscopic Data. *The
 Journal of Physical Chemistry Letters*. DOI:
@@ -25,15 +25,15 @@
 
 If you’re going to use a pip or a conda environment, you’ll need:
 
 -  Python 3.8 or newer.
 -  A GROMACS installation supporting client software builds.
 -  `gmxapi <https://manual.gromacs.org/current/gmxapi>`__ for GROMACS.
 
-``brer`` includes a simple C++ extension module that can be attached to a GROMACS
+``brer-md`` includes a simple C++ extension module that can be attached to a GROMACS
 molecular dynamics (MD) simulator through the gmxapi Python interface.
 GROMACS installations (and GROMACS dependencies) can be built rather specifically
 for their computing environments. The ``brer`` package is distributed as source
 code that must be built for a specific GROMACS installation.
 
 .. note::
     For several recent versions of GROMACS, the “legacy API” needs
@@ -68,14 +68,16 @@
 Generally, ``pip`` will automatically install any package dependencies.
 
 If a GROMACS installation is discoverable (you have "sourced" a GMXRC file or
 defined a GROMACS_DIR environment variable), then the ``gmxapi`` Python package
 will be installed automatically with the ``brer`` package.
 Simply::
 
+    pip install --pre brer-md
+    # or
     pip install git+https://github.com/kassonlab/brer-md.git
 
 If you prefer to install ``gmxapi`` separately (such as to specify an older
 package version), you can provide ``--no-deps`` and ``--no-build-isolation``
 to ``pip install``, and the existing ``gmxapi`` installation will be used.
 
 You can pre-install (other) required packages using the
```

### Comparing `brer-md-2.0.0b6/_custom_build/backend.py` & `brer-md-2.0.0b8/_custom_build/backend.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/brer_md.egg-info/PKG-INFO` & `brer-md-2.0.0b8/brer_md.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brer-md
-Version: 2.0.0b6
+Version: 2.0.0b8
 Summary: A set of scripts for running BRER simulations using gmxapi.
 Author: Jennifer M. Hays, Kasson Lab BRER Team
 Author-email: Kasson Lab BRER Team <kassonlab@gmail.com>
 License: LGPL 2.1
 Project-URL: Source, https://github.com/kassonlab/brer-md/
 Project-URL: Documentation, https://kassonlab.github.io/brer-md/
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
@@ -19,15 +19,15 @@
 
 |Build and test| |Documentation| |codecov|
 
 Source: https://github.com/kassonlab/brer-md
 
 Documentation: https://kassonlab.github.io/brer-md/
 
-The ``brer`` Python package provides a set of scripts for running
+The ``brer-md`` Python package provides a set of scripts for running
 Bias-Resampling Ensemble Refinement (BRER) simulations using
 `gmxapi <https://gmxapi.org/>`__. Details of the BRER
 method may be found in:
 
 Hays, J. M., Cafiso, D. S., & Kasson, P. M. Hybrid Refinement of
 Heterogeneous Conformational Ensembles using Spectroscopic Data. *The
 Journal of Physical Chemistry Letters*. DOI:
@@ -41,15 +41,15 @@
 
 If you’re going to use a pip or a conda environment, you’ll need:
 
 -  Python 3.8 or newer.
 -  A GROMACS installation supporting client software builds.
 -  `gmxapi <https://manual.gromacs.org/current/gmxapi>`__ for GROMACS.
 
-``brer`` includes a simple C++ extension module that can be attached to a GROMACS
+``brer-md`` includes a simple C++ extension module that can be attached to a GROMACS
 molecular dynamics (MD) simulator through the gmxapi Python interface.
 GROMACS installations (and GROMACS dependencies) can be built rather specifically
 for their computing environments. The ``brer`` package is distributed as source
 code that must be built for a specific GROMACS installation.
 
 .. note::
     For several recent versions of GROMACS, the “legacy API” needs
@@ -84,14 +84,16 @@
 Generally, ``pip`` will automatically install any package dependencies.
 
 If a GROMACS installation is discoverable (you have "sourced" a GMXRC file or
 defined a GROMACS_DIR environment variable), then the ``gmxapi`` Python package
 will be installed automatically with the ``brer`` package.
 Simply::
 
+    pip install --pre brer-md
+    # or
     pip install git+https://github.com/kassonlab/brer-md.git
 
 If you prefer to install ``gmxapi`` separately (such as to specify an older
 package version), you can provide ``--no-deps`` and ``--no-build-isolation``
 to ``pip install``, and the existing ``gmxapi`` installation will be used.
 
 You can pre-install (other) required packages using the
```

### Comparing `brer-md-2.0.0b6/brer_md.egg-info/SOURCES.txt` & `brer-md-2.0.0b8/brer_md.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/pyproject.toml` & `brer-md-2.0.0b8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # gmxapi versions. We may have to override the `requires` metadata in terms of
 # the dependency version used by the binary as it is built.
 requires = [
     "cmake>=3.15",
     "gmxapi",
     "pybind11>=2.6",
     "setuptools>=61",
-    "versioningit~=2.0",
+    "versioningit>=2.0",
     "wheel"
 ]
 build-backend = "backend"
 backend-path = ["_custom_build"]
 
 [project]
 name = "brer-md"
```

### Comparing `brer-md-2.0.0b6/setup.py` & `brer-md-2.0.0b8/setup.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/brer/_compat.py` & `brer-md-2.0.0b8/src/brer/_compat.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/brer/data/pair_data.json` & `brer-md-2.0.0b8/src/brer/data/pair_data.json`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/brer/data/topol.tpr` & `brer-md-2.0.0b8/src/brer/data/topol.tpr`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/brer/directory_helper.py` & `brer-md-2.0.0b8/src/brer/directory_helper.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/brer/pair_data.py` & `brer-md-2.0.0b8/src/brer/pair_data.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/brer/plugin_configs.py` & `brer-md-2.0.0b8/src/brer/plugin_configs.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/brer/run_config.py` & `brer-md-2.0.0b8/src/brer/run_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """RunConfig class handles the actual workflow logic."""
-__all__ = ('RunConfig',)
+__all__ = ("RunConfig",)
 
 import collections.abc
 import dataclasses
+import functools
+import importlib
 import logging
 import os
 import pathlib
 import shutil
+import sys
 import typing
 import warnings
 from typing import Sequence
 from typing import Union
 
 from .pair_data import PairDataCollection
 from .pair_data import sample_all
@@ -21,32 +24,64 @@
 from .plugin_configs import ProductionPluginConfig
 from .plugin_configs import TrainingPluginConfig
 from .run_data import RunData
 
 _Path = Union[str, pathlib.Path]
 
 
-def _gmxapi_missing(*args, **kwargs):
-    raise RuntimeError('brer requires gmxapi. See https://github.com/kassonlab/brer_md#requirements')
+def _gmxapi_missing(*args, msg: str = "", **kwargs):
+    """Placeholder function for missing gmxapi functionality.
 
-
-try:
-    # noinspection PyPep8Naming,PyUnresolvedReferences
-    from gmxapi.simulation.context import Context as _context
-    # noinspection PyUnresolvedReferences
-    from gmxapi.simulation.workflow import WorkElement, from_tpr
-except (ImportError, ModuleNotFoundError):
-    try:
-        # noinspection PyPep8Naming
-        from gmx.context import Context as _context
-        from gmx.workflow import from_tpr, WorkElement
-    except (ImportError, ModuleNotFoundError):
-        _context = _gmxapi_missing
-        from_tpr = _gmxapi_missing
-        WorkElement = _gmxapi_missing
+    Allows import errors to be deferred until run time to aid in docs builds
+    and troubleshooting. Try to provide a useful RuntimeError that includes
+    the details of the import error(s).
+    """
+    _message = (
+        "brer requires gmxapi. See https://github.com/kassonlab/brer_md#requirements"
+    )
+    if msg:
+        _message = "\n".join((_message, msg))
+    raise RuntimeError(_message)
+
+
+def get_api_callable(attr: str, modules: typing.Iterable[str]):
+    """Get a gmxapi callable or placeholder.
+
+    Try to import *attr* from successive *modules*. Return the first callable
+    found, else return a placeholder that emits a RuntimeError when called.
+    """
+    message = ""
+    version = ""
+    func = None
+    for module in modules:
+        try:
+            mod = importlib.import_module(module)
+            func = getattr(mod, attr)
+            base = module.split(".")[0]
+            version = sys.modules[base].__version__
+        except ImportError as e:
+            message = "\n".join((message, f"Could not import {module}: {str(e)}"))
+        else:
+            break
+    if callable(func):
+        qualname = ".".join((func.__module__, func.__name__))
+    else:
+        func = functools.partial(_gmxapi_missing, msg=message)
+        qualname = ".".join((_gmxapi_missing.__module__, "_gmxapi_missing"))
+
+    report = "Using" \
+             + " ".join((qualname, version)) \
+             + " for {attr}."
+    logging.info(report)
+    return func
+
+
+_context = get_api_callable("Context", ("gmxapi.simulation.context", "gmx.context"))
+from_tpr = get_api_callable("from_tpr", ("gmxapi.simulation.workflow", "gmx.workflow"))
+WorkElement = get_api_callable("WorkElement", ("gmxapi.simulation.workflow", "gmx.workflow"))
 
 
 def check_consistency(*, data: PairDataCollection, state: RunData):
     """Check for mismatched data sources.
 
     Returns
     -------
```

### Comparing `brer-md-2.0.0b6/src/brer/run_data.py` & `brer-md-2.0.0b8/src/brer/run_data.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/CMakeLists.txt` & `brer-md-2.0.0b8/src/plugin/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/cpp/CMakeLists.txt` & `brer-md-2.0.0b8/src/plugin/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/cpp/brerpotential.cpp` & `brer-md-2.0.0b8/src/plugin/cpp/brerpotential.cpp`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/cpp/brerpotential.h` & `brer-md-2.0.0b8/src/plugin/cpp/brerpotential.h`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/cpp/linearpotential.cpp` & `brer-md-2.0.0b8/src/plugin/cpp/linearpotential.cpp`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/cpp/linearpotential.h` & `brer-md-2.0.0b8/src/plugin/cpp/linearpotential.h`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/cpp/linearstoppotential.cpp` & `brer-md-2.0.0b8/src/plugin/cpp/linearstoppotential.cpp`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/cpp/linearstoppotential.h` & `brer-md-2.0.0b8/src/plugin/cpp/linearstoppotential.h`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/cpp/sessionresources.cpp` & `brer-md-2.0.0b8/src/plugin/cpp/sessionresources.cpp`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/cpp/sessionresources.h` & `brer-md-2.0.0b8/src/plugin/cpp/sessionresources.h`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/pythonmodule/CMakeLists.txt` & `brer-md-2.0.0b8/src/plugin/pythonmodule/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/src/plugin/pythonmodule/export_plugin.cpp` & `brer-md-2.0.0b8/src/plugin/pythonmodule/export_plugin.cpp`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/tests/test_dirhelper.py` & `brer-md-2.0.0b8/tests/test_dirhelper.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/tests/test_pair_data.py` & `brer-md-2.0.0b8/tests/test_pair_data.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/tests/test_plugin_binding.py` & `brer-md-2.0.0b8/tests/test_plugin_binding.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/tests/test_plugin_configs.py` & `brer-md-2.0.0b8/tests/test_plugin_configs.py`

 * *Files identical despite different names*

### Comparing `brer-md-2.0.0b6/tests/test_run_config.py` & `brer-md-2.0.0b8/tests/test_run_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 logger = logging.getLogger()
 
 try:
     from mpi4py import MPI
 except ImportError:
     MPI = None
 
+try:
+    from gmxapi.utility import config
+except ImportError:
+    config = dict
+
 # To use PyCharm debug server, you would need something like the following:
 # if rank == 0:
 #     import pydevd_pycharm
 #
 #     pydevd_pycharm.settrace('localhost',
 #                             port=33333,
 #                             stdoutToServer=True,
@@ -32,14 +37,29 @@
 # Try to get a reasonable number of threads to use.
 try:
     num_cpus: int = len(os.sched_getaffinity(0))
 except Exception:
     num_cpus = 4
 
 
+def test_import_utility(simulation_input):
+    from brer.run_config import _context, from_tpr, WorkElement, get_api_callable
+    _context()
+    element = from_tpr(simulation_input)
+    assert isinstance(element, WorkElement)
+    func = get_api_callable("nonsense", ("missing1",))
+    with pytest.raises(RuntimeError, match="Could not import missing1"):
+        func()
+    func = get_api_callable("nonsense", ("missing1", "missing2"))
+    with pytest.raises(RuntimeError, match="Could not import missing2"):
+        func()
+    with pytest.raises(RuntimeError, match="Could not import missing1"):
+        func()
+
+
 @contextlib.contextmanager
 def working_directory_fence():
     """Ensure restoration of working directory when leaving context manager."""
     wd = os.getcwd()
     try:
         yield wd
     finally:
@@ -74,16 +94,22 @@
         # See https://github.com/kassonlab/run_brer/issues/8
         with pytest.raises(RuntimeError):
             rc.run(max_hours=0.0001)
         assert rc.run_data.get('phase') == 'training'
 
         # Allow the training phase to converge.
         rc.run_data.set(tolerance=10000)
+
         # Include a test for kwarg handling.
-        rc.run(threads=num_cpus)
+        kwargs = dict()
+        # From gmxapi/CMakeLists.txt, this is "library", "tmpi", or None
+        mpi_type = config().get("gmx_mpi_type")
+        if mpi_type == "tmpi":
+            kwargs["threads"] = num_cpus
+        rc.run(**kwargs)
 
         # Convergence phase.
         assert rc.run_data.get('phase') == 'convergence'
         # Check that bad alpha is caught.
         _original_alpha = [None] * len(rc.run_data.pair_params)
         for i, name in enumerate(rc.run_data.pair_params):
             _original_alpha[i] = rc.run_data.get('alpha', name=name)
@@ -157,28 +183,35 @@
                         num_samples=2,
                         sample_period=0.1,
                         production_time=0.2)
 
         # Training phase.
         assert rc.run_data.get('phase') == 'training'
         # Include a test for kwarg handling.
-        rc.run(threads=2)
+        kwargs = dict()
+        mpi_type = config().get("gmx_mpi_type")
+        if mpi_type == "tmpi":
+            kwargs["threads"] = 2
+        rc.run(**kwargs)
 
         # Convergence phase.
         assert rc.run_data.get('phase') == 'convergence'
-        rc.run(threads=4)
+        if mpi_type == "tmpi":
+            kwargs['threads'] = 4
+        rc.run(**kwargs)
 
         # Production phase.
         assert rc.run_data.get('phase') == 'production'
         with pytest.raises(TypeError):
             # Test handling of kwarg collisions.
             rc.run(end_time=1.0)
         # Note that rc.__production failed, but rc.run() will have changed directory.
         # This is an unspecified side effect, but we can use it for some additional
         # inspection.
         assert len(os.listdir()) == 0
         # Test another kwarg.
-        rc.run(threads=4, max_hours=0.001)
+        kwargs['max_hours'] = 0.001
+        rc.run(**kwargs)
 
         if comm.Get_size() > 1:
             # TODO(https://github.com/kassonlab/run_brer/issues/7): Confirm that we actually ran different ensemble members.
             ...
```

### Comparing `brer-md-2.0.0b6/tests/test_run_data.py` & `brer-md-2.0.0b8/tests/test_run_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,9 +84,9 @@
     with tempfile.NamedTemporaryFile(suffix='.json', mode='w') as tmp:
         test_data = raw_pair_data.copy()
         for name in test_data:
             test_data[name]['name'] = f'{name}_different'
         json.dump(test_data, tmp)
         tmp.flush()
         # Tolerates redundant *name* field. Warns if inconsistent.
-        with pytest.warns(match='instead of'):
+        with pytest.warns(UserWarning, match='instead of'):
             PairDataCollection.create_from(tmp.name)
```

### Comparing `brer-md-2.0.0b6/tests/testdata.json` & `brer-md-2.0.0b8/tests/testdata.json`

 * *Files identical despite different names*


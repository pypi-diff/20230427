# Comparing `tmp/hagrid-0.3.3.tar.gz` & `tmp/hagrid-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagrid-0.3.3.tar", last modified: Wed Apr 26 05:54:05 2023, max compression
+gzip compressed data, was "hagrid-0.3.4.tar", last modified: Thu Apr 27 05:11:48 2023, max compression
```

## Comparing `hagrid-0.3.3.tar` & `hagrid-0.3.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:54:05.928377 hagrid-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-26 05:54:05.928377 hagrid-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-26 05:51:49.000000 hagrid-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:54:05.924377 hagrid-0.3.3/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/art.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)   134776 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/git_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/land.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-26 05:52:04.000000 hagrid-0.3.3/hagrid/manifest_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/nb_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/orchestra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/parse_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/quickstart_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/rand_sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 05:52:04.000000 hagrid-0.3.3/hagrid/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/win_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/wizard_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:54:05.928377 hagrid-0.3.3/hagrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 05:54:05.928377 hagrid-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-26 05:52:04.000000 hagrid-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:54:05.928377 hagrid-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:51:49.000000 hagrid-0.3.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:54:05.928377 hagrid-0.3.3/tests/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:51:49.000000 hagrid-0.3.3/tests/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-26 05:51:49.000000 hagrid-0.3.3/tests/hagrid/cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:11:48.729418 hagrid-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-27 05:11:48.729418 hagrid-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-27 05:09:31.000000 hagrid-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:11:48.729418 hagrid-0.3.4/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/art.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134776 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/git_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/land.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-27 05:09:45.000000 hagrid-0.3.4/hagrid/manifest_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/nb_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/orchestra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/parse_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/quickstart_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/rand_sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-27 05:09:45.000000 hagrid-0.3.4/hagrid/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/win_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-27 05:09:31.000000 hagrid-0.3.4/hagrid/wizard_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:11:48.729418 hagrid-0.3.4/hagrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-27 05:11:48.000000 hagrid-0.3.4/hagrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-27 05:11:48.000000 hagrid-0.3.4/hagrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 05:11:48.000000 hagrid-0.3.4/hagrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 05:11:48.000000 hagrid-0.3.4/hagrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 05:11:48.000000 hagrid-0.3.4/hagrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 05:11:48.000000 hagrid-0.3.4/hagrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 05:11:48.729418 hagrid-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-27 05:09:45.000000 hagrid-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:11:48.729418 hagrid-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:09:31.000000 hagrid-0.3.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:11:48.729418 hagrid-0.3.4/tests/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:09:31.000000 hagrid-0.3.4/tests/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-27 05:09:31.000000 hagrid-0.3.4/tests/hagrid/cli_test.py
```

### Comparing `hagrid-0.3.3/README.md` & `hagrid-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/__init__.py` & `hagrid-0.3.4/hagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/art.py` & `hagrid-0.3.4/hagrid/art.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/auth.py` & `hagrid-0.3.4/hagrid/auth.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/azure.py` & `hagrid-0.3.4/hagrid/azure.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/cache.py` & `hagrid-0.3.4/hagrid/cache.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/cli.py` & `hagrid-0.3.4/hagrid/cli.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/deps.py` & `hagrid-0.3.4/hagrid/deps.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/grammar.py` & `hagrid-0.3.4/hagrid/grammar.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/land.py` & `hagrid-0.3.4/hagrid/land.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/launch.py` & `hagrid-0.3.4/hagrid/launch.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/lib.py` & `hagrid-0.3.4/hagrid/lib.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/manifest_template.yml` & `hagrid-0.3.4/hagrid/manifest_template.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 manifestVersion: 0.1
-hagrid_version: 0.3.3
-syft_version: 0.8.0-beta.9
-dockerTag: 0.8.0-beta.9
+hagrid_version: 0.3.4
+syft_version: 0.8.0-beta.10
+dockerTag: 0.8.0-beta.10
 baseUrl: https://raw.githubusercontent.com/OpenMined/PySyft/
-hash: b1396848e85f6e0332983ac9007db3461f81b826
+hash: 142304a17c54aa7b0c340b7a9c3ef57b99d96547
 target_dir: ~/.hagrid/PySyft/
 files:
   grid:
     path: packages/grid/
     common:
     - rabbitmq/rabbitmq.conf
     - redis/redis.conf
```

### Comparing `hagrid-0.3.3/hagrid/mode.py` & `hagrid-0.3.4/hagrid/mode.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/names.py` & `hagrid-0.3.4/hagrid/names.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/orchestra.py` & `hagrid-0.3.4/hagrid/orchestra.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/parse_template.py` & `hagrid-0.3.4/hagrid/parse_template.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/quickstart_ui.py` & `hagrid-0.3.4/hagrid/quickstart_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/rand_sec.py` & `hagrid-0.3.4/hagrid/rand_sec.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/style.py` & `hagrid-0.3.4/hagrid/style.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/util.py` & `hagrid-0.3.4/hagrid/util.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/win_bootstrap.py` & `hagrid-0.3.4/hagrid/win_bootstrap.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid/wizard_ui.py` & `hagrid-0.3.4/hagrid/wizard_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/hagrid.egg-info/SOURCES.txt` & `hagrid-0.3.4/hagrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.3/setup.py` & `hagrid-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 import platform
 
 # third party
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 
 DATA_FILES = {"img": ["hagrid/img/*.png"], "hagrid": ["*.yml"]}
 
 packages = [
     "ascii_magic",
     "click>=7.1",
     "cryptography>=37.0.2",
```

### Comparing `hagrid-0.3.3/tests/hagrid/cli_test.py` & `hagrid-0.3.4/tests/hagrid/cli_test.py`

 * *Files identical despite different names*


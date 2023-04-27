# Comparing `tmp/fabrictestbed-1.4.5rc2.tar.gz` & `tmp/fabrictestbed-1.4.5rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.4.5rc2.tar", last modified: Thu Apr 27 14:19:10 2023, max compression
+gzip compressed data, was "fabrictestbed-1.4.5rc3.tar", last modified: Thu Apr 27 14:51:56 2023, max compression
```

## Comparing `fabrictestbed-1.4.5rc2.tar` & `fabrictestbed-1.4.5rc3.tar`

### file list

```diff
@@ -1,32 +1,17 @@
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:19:10.948703 fabrictestbed-1.4.5rc2/
--rw-r--r--   0 kthare10   (503) staff       (20)     1071 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/LICENSE
--rw-r--r--   0 kthare10   (503) staff       (20)       24 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/MANIFEST.in
--rw-r--r--   0 kthare10   (503) staff       (20)     6101 2023-04-27 14:19:10.948200 fabrictestbed-1.4.5rc2/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     5603 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/README.md
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:19:10.938190 fabrictestbed-1.4.5rc2/fabrictestbed/
--rw-r--r--   0 kthare10   (503) staff       (20)       25 2023-04-27 14:18:12.000000 fabrictestbed-1.4.5rc2/fabrictestbed/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:19:10.943107 fabrictestbed-1.4.5rc2/fabrictestbed/cli/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/fabrictestbed/cli/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)    18087 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/fabrictestbed/cli/cli.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1452 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/fabrictestbed/cli/exceptions.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:19:10.943579 fabrictestbed-1.4.5rc2/fabrictestbed/slice_editor/
--rw-r--r--   0 kthare10   (503) staff       (20)     1914 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/fabrictestbed/slice_editor/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:19:10.945611 fabrictestbed-1.4.5rc2/fabrictestbed/slice_manager/
--rw-r--r--   0 kthare10   (503) staff       (20)      201 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)    17886 2023-04-27 14:18:44.000000 fabrictestbed-1.4.5rc2/fabrictestbed/slice_manager/slice_manager.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:19:10.946681 fabrictestbed-1.4.5rc2/fabrictestbed/util/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/fabrictestbed/util/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1452 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/fabrictestbed/util/constants.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:19:10.941596 fabrictestbed-1.4.5rc2/fabrictestbed.egg-info/
--rw-r--r--   0 kthare10   (503) staff       (20)     6101 2023-04-27 14:19:10.000000 fabrictestbed-1.4.5rc2/fabrictestbed.egg-info/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)      613 2023-04-27 14:19:10.000000 fabrictestbed-1.4.5rc2/fabrictestbed.egg-info/SOURCES.txt
--rw-r--r--   0 kthare10   (503) staff       (20)        1 2023-04-27 14:19:10.000000 fabrictestbed-1.4.5rc2/fabrictestbed.egg-info/dependency_links.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       57 2023-04-27 14:19:10.000000 fabrictestbed-1.4.5rc2/fabrictestbed.egg-info/entry_points.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       96 2023-04-27 14:19:10.000000 fabrictestbed-1.4.5rc2/fabrictestbed.egg-info/requires.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       19 2023-04-27 14:19:10.000000 fabrictestbed-1.4.5rc2/fabrictestbed.egg-info/top_level.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       81 2023-04-27 14:18:03.000000 fabrictestbed-1.4.5rc2/requirements.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       38 2023-04-27 14:19:10.948857 fabrictestbed-1.4.5rc2/setup.cfg
--rw-r--r--   0 kthare10   (503) staff       (20)     1071 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/setup.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:19:10.947639 fabrictestbed-1.4.5rc2/test/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/test/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2210 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc2/test/test_cli.py
+-rw-r--r--   0        0        0     1806 2023-04-27 14:50:00.258551 fabrictestbed-1.4.5rc3/.gitignore
+-rw-r--r--   0        0        0     1071 2023-04-26 16:15:21.494794 fabrictestbed-1.4.5rc3/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-26 16:15:21.494897 fabrictestbed-1.4.5rc3/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2023-04-26 16:15:21.495044 fabrictestbed-1.4.5rc3/README.md
+-rw-r--r--   0        0        0       25 2023-04-27 14:50:24.559428 fabrictestbed-1.4.5rc3/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:15:21.495306 fabrictestbed-1.4.5rc3/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    18087 2023-04-26 16:15:21.495535 fabrictestbed-1.4.5rc3/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2023-04-26 16:15:21.495890 fabrictestbed-1.4.5rc3/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-04-26 16:15:21.496100 fabrictestbed-1.4.5rc3/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2023-04-26 16:15:21.496284 fabrictestbed-1.4.5rc3/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    17886 2023-04-27 14:18:44.441875 fabrictestbed-1.4.5rc3/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:15:21.496579 fabrictestbed-1.4.5rc3/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1452 2023-04-26 16:15:21.496691 fabrictestbed-1.4.5rc3/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0      906 2023-04-27 14:51:49.373381 fabrictestbed-1.4.5rc3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 16:15:21.497061 fabrictestbed-1.4.5rc3/test/__init__.py
+-rw-r--r--   0        0        0     2210 2023-04-26 16:15:21.497240 fabrictestbed-1.4.5rc3/test/test_cli.py
+-rw-r--r--   0        0        0     6281 1970-01-01 00:00:00.000000 fabrictestbed-1.4.5rc3/PKG-INFO
```

### Comparing `fabrictestbed-1.4.5rc2/LICENSE` & `fabrictestbed-1.4.5rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc2/PKG-INFO` & `fabrictestbed-1.4.5rc3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.4.5rc2
+Version: 1.4.5rc3
 Summary: FABRIC Python Client Library with CLI
-Home-page: https://github.com/fabric-testbed/fabric-cli
-Author: Erica Fu, Komal Thareja
-Author-email: ericafu@renci.org, kthare10@unc.edu
+Keywords: Swagger,FABRIC Python Client Library with CLI
+Author-email: Komal Thareja <kthare10@renci.org>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: fabric-credmgr-client==1.3.2
+Requires-Dist: fabric-orchestrator-client==1.4.5rc2
+Requires-Dist: paramiko
+Project-URL: Home, https://fabric-testbed.net/
+Project-URL: Sources, https://github.com/fabric-testbed/fabric-cli
 
 [![PyPI](https://img.shields.io/pypi/v/fabrictestbed?style=plastic)](https://pypi.org/project/fabrictestbed/)
 
 
 # FABRIC TESTBED USER LIBRARY AND CLI
 
 Fabric User CLI for experiments
@@ -161,7 +164,8 @@
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   query  Query user slice sliver(s)
 ```
+
```

### Comparing `fabrictestbed-1.4.5rc2/README.md` & `fabrictestbed-1.4.5rc3/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc2/fabrictestbed/cli/cli.py` & `fabrictestbed-1.4.5rc3/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc2/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.4.5rc3/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc2/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.4.5rc3/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc2/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.4.5rc3/fabrictestbed/slice_manager/slice_manager.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc2/fabrictestbed/util/constants.py` & `fabrictestbed-1.4.5rc3/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc2/test/test_cli.py` & `fabrictestbed-1.4.5rc3/test/test_cli.py`

 * *Files identical despite different names*


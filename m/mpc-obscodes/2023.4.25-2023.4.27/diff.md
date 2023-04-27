# Comparing `tmp/mpc_obscodes-2023.4.25.tar.gz` & `tmp/mpc_obscodes-2023.4.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2023.4.25.tar", last modified: Tue Apr 25 00:08:15 2023, max compression
+gzip compressed data, was "mpc_obscodes-2023.4.27.tar", last modified: Thu Apr 27 17:26:20 2023, max compression
```

## Comparing `mpc_obscodes-2023.4.25.tar` & `mpc_obscodes-2023.4.27.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:08:15.258460 mpc_obscodes-2023.4.25/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-25 00:07:57.000000 mpc_obscodes-2023.4.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-25 00:08:15.258460 mpc_obscodes-2023.4.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-25 00:07:57.000000 mpc_obscodes-2023.4.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:08:15.258460 mpc_obscodes-2023.4.25/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-25 00:07:57.000000 mpc_obscodes-2023.4.25/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-25 00:07:57.000000 mpc_obscodes-2023.4.25/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)   245092 2023-04-25 00:08:03.000000 mpc_obscodes-2023.4.25/mpc_obscodes/obscodes_extended.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:08:15.258460 mpc_obscodes-2023.4.25/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:07:57.000000 mpc_obscodes-2023.4.25/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-25 00:07:57.000000 mpc_obscodes-2023.4.25/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 00:07:57.000000 mpc_obscodes-2023.4.25/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:08:15.258460 mpc_obscodes-2023.4.25/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-25 00:08:15.000000 mpc_obscodes-2023.4.25/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-25 00:08:15.000000 mpc_obscodes-2023.4.25/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:08:15.000000 mpc_obscodes-2023.4.25/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 00:08:15.000000 mpc_obscodes-2023.4.25/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 00:08:15.000000 mpc_obscodes-2023.4.25/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-25 00:08:03.000000 mpc_obscodes-2023.4.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 00:08:15.258460 mpc_obscodes-2023.4.25/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:26:20.321140 mpc_obscodes-2023.4.27/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 17:26:20.321140 mpc_obscodes-2023.4.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:26:20.317140 mpc_obscodes-2023.4.27/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245177 2023-04-27 17:26:05.000000 mpc_obscodes-2023.4.27/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 17:26:05.000000 mpc_obscodes-2023.4.27/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:26:20.321140 mpc_obscodes-2023.4.27/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:26:20.317140 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 17:26:20.000000 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-27 17:26:20.000000 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:26:20.000000 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 17:26:20.000000 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 17:26:20.000000 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-27 17:26:05.000000 mpc_obscodes-2023.4.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:26:20.321140 mpc_obscodes-2023.4.27/setup.cfg
```

### Comparing `mpc_obscodes-2023.4.25/PKG-INFO` & `mpc_obscodes-2023.4.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2023.4.25
+Version: 2023.4.27
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # Minor Planet Center Observatory Codes
```

### Comparing `mpc_obscodes-2023.4.25/README.md` & `mpc_obscodes-2023.4.27/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.25/mpc_obscodes/fetch.py` & `mpc_obscodes-2023.4.27/mpc_obscodes/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil
 
 import requests
 
 URL = "https://minorplanetcenter.net/Extended_Files/obscodes_extended.json.gz"
 FILE_COMPRESSED = os.path.join(os.path.dirname(__file__), "obscodes_extended.json.gz")
 FILE_DECOMPRESSED =  os.path.join(os.path.dirname(__file__), "obscodes_extended.json")
-MD5_FILE =  os.path.join(os.path.dirname(__file__), "obscodes_extended.json.md5")
+MD5_FILE =  os.path.join(os.path.dirname(__file__), "obscodes_extended.md5")
 
 
 def fetch_file(url: str, output_file: str):
     """
     Fetches the file from the given URL and saves it to the output file.
 
     Parameters
```

### Comparing `mpc_obscodes-2023.4.25/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2023.4.27/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995883079456567%*

 * *Differences: {"'M52'": "OrderedDict([('Longitude', 8.5785), ('cos', 0.758941), ('sin', 0.649052), ('Name', "*

 * *          "'Sassari')])"}*

```diff
@@ -12067,14 +12067,20 @@
     },
     "M51": {
         "Longitude": 9.22697,
         "Name": "Robert Mayer Sternwarte, Heilbronn",
         "cos": 0.6555,
         "sin": 0.752709
     },
+    "M52": {
+        "Longitude": 8.5785,
+        "Name": "Sassari",
+        "cos": 0.758941,
+        "sin": 0.649052
+    },
     "M90": {
         "Longitude": 65.4286,
         "Name": "Chervishevo",
         "cos": 0.54672,
         "sin": 0.83452
     },
     "N27": {
```

### Comparing `mpc_obscodes-2023.4.25/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2023.4.27/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.25/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc-obscodes
-Version: 2023.4.25
+Version: 2023.4.27
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # Minor Planet Center Observatory Codes
```

### Comparing `mpc_obscodes-2023.4.25/pyproject.toml` & `mpc_obscodes-2023.4.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2023.04.25"
+version = "2023.04.27"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```


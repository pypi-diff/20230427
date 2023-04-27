# Comparing `tmp/camerahub_tagger-0.2.3.tar.gz` & `tmp/camerahub_tagger-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camerahub_tagger-0.2.3.tar", max compression
+gzip compressed data, was "camerahub_tagger-0.2.4.tar", max compression
```

## Comparing `camerahub_tagger-0.2.3.tar` & `camerahub_tagger-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2839 2023-04-26 15:31:32.520531 camerahub_tagger-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-04-26 15:31:32.520531 camerahub_tagger-0.2.3/camerahub_tagger/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-26 15:31:32.520531 camerahub_tagger-0.2.3/camerahub_tagger/api.py
--rw-r--r--   0        0        0     2011 2023-04-26 15:31:32.520531 camerahub_tagger-0.2.3/camerahub_tagger/config.py
--rw-r--r--   0        0        0     5518 2023-04-26 15:31:32.520531 camerahub_tagger-0.2.3/camerahub_tagger/funcs.py
--rwxr-xr-x   0        0        0     5468 2023-04-26 15:31:32.520531 camerahub_tagger-0.2.3/camerahub_tagger/main.py
--rw-r--r--   0        0        0      649 2023-04-26 15:32:01.656718 camerahub_tagger-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3565 1970-01-01 00:00:00.000000 camerahub_tagger-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2839 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/camerahub_tagger/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/camerahub_tagger/api.py
+-rw-r--r--   0        0        0     2011 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/camerahub_tagger/config.py
+-rw-r--r--   0        0        0     5519 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/camerahub_tagger/funcs.py
+-rwxr-xr-x   0        0        0     5468 2023-04-26 20:08:17.718695 camerahub_tagger-0.2.4/camerahub_tagger/main.py
+-rw-r--r--   0        0        0      649 2023-04-26 20:08:39.487991 camerahub_tagger-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3565 1970-01-01 00:00:00.000000 camerahub_tagger-0.2.4/PKG-INFO
```

### Comparing `camerahub_tagger-0.2.3/README.md` & `camerahub_tagger-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.2.3/camerahub_tagger/api.py` & `camerahub_tagger-0.2.4/camerahub_tagger/api.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.2.3/camerahub_tagger/config.py` & `camerahub_tagger-0.2.4/camerahub_tagger/config.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.2.3/camerahub_tagger/funcs.py` & `camerahub_tagger-0.2.4/camerahub_tagger/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 def guess_frame(filepath):
     """
     Guess a negative's film id and frame id based on its filename
     Assumes a format of [film]-[frame]-title.jpg
     for example 123-22-holiday.jpg
     """
     filename = basename(filepath)
-    match = re.search(r'^(\d+)-(\d+).*\.jpe?g$', filename.lower())
+    match = re.search(r'^(\d+)-(\w+)-.*\.jpe?g$', filename.lower())
     if match and match.group(1) and match.group(2):
         returnval = (match.group(1), match.group(2))
     else:
         returnval = None
     return returnval
```

### Comparing `camerahub_tagger-0.2.3/camerahub_tagger/main.py` & `camerahub_tagger-0.2.4/camerahub_tagger/main.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.2.3/pyproject.toml` & `camerahub_tagger-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camerahub-tagger"
-version = "0.2.3"
+version = "0.2.4"
 description = "EXIF tagger for CameraHub"
 authors = ["Jonathan Gazeley <me@jonathangazeley.com>"]
 repository = "https://github.com/camerahub/tagger"
 homepage = "https://camerahub.info/"
 readme = ["README.md"]
 keywords = ["EXIF", "photography", "CameraHub", "metadata"]
```

### Comparing `camerahub_tagger-0.2.3/PKG-INFO` & `camerahub_tagger-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camerahub-tagger
-Version: 0.2.3
+Version: 0.2.4
 Summary: EXIF tagger for CameraHub
 Home-page: https://camerahub.info/
 Keywords: EXIF,photography,CameraHub,metadata
 Author: Jonathan Gazeley
 Author-email: me@jonathangazeley.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```


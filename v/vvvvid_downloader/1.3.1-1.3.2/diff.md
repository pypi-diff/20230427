# Comparing `tmp/vvvvid_downloader-1.3.1.tar.gz` & `tmp/vvvvid_downloader-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvvvid_downloader-1.3.1.tar", last modified: Tue Jan  4 11:19:08 2022, max compression
+gzip compressed data, was "vvvvid_downloader-1.3.2.tar", last modified: Thu Apr 27 15:39:53 2023, max compression
```

## Comparing `vvvvid_downloader-1.3.1.tar` & `vvvvid_downloader-1.3.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      156 2021-04-26 13:58:18.349162 vvvvid_downloader-1.3.1/.editorconfig
--rw-r--r--   0        0        0       73 2021-05-02 14:10:39.782990 vvvvid_downloader-1.3.1/.gitattributes
--rw-r--r--   0        0        0     2206 2021-04-26 13:58:18.349162 vvvvid_downloader-1.3.1/.gitignore
--rw-r--r--   0        0        0     1198 2022-01-04 11:16:28.839171 vvvvid_downloader-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      251 2022-01-04 11:14:09.192572 vvvvid_downloader-1.3.1/Pipfile
--rw-r--r--   0        0        0    16734 2022-01-04 11:14:21.369014 vvvvid_downloader-1.3.1/Pipfile.lock
--rw-r--r--   0        0        0      978 2022-01-03 15:12:36.271525 vvvvid_downloader-1.3.1/README.md
--rw-r--r--   0        0        0     1211 2021-11-29 22:26:09.466364 vvvvid_downloader-1.3.1/UNLICENSE
--rw-r--r--   0        0        0      664 2022-01-04 11:07:14.039562 vvvvid_downloader-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       77 2022-01-04 10:52:32.540532 vvvvid_downloader-1.3.1/vvvvid_downloader/__init__.py
--rw-r--r--   0        0        0     8058 2022-01-04 11:04:24.764188 vvvvid_downloader-1.3.1/vvvvid_downloader/__main__.py
--rw-r--r--   0        0        0     1372 2021-05-02 22:19:44.553871 vvvvid_downloader-1.3.1/vvvvid_downloader/vvvvid.py
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 vvvvid_downloader-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      147 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.2/.editorconfig
+-rw-r--r--   0        0        0       73 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.2/.gitattributes
+-rw-r--r--   0        0        0     2064 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1198 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0      243 2023-04-27 14:44:52.806456 vvvvid_downloader-1.3.2/Pipfile
+-rw-r--r--   0        0        0    26600 2023-04-27 14:45:26.766698 vvvvid_downloader-1.3.2/Pipfile.lock
+-rw-r--r--   0        0        0      978 2023-04-27 14:44:09.270044 vvvvid_downloader-1.3.2/README.md
+-rw-r--r--   0        0        0     1211 2023-04-27 14:44:09.270044 vvvvid_downloader-1.3.2/UNLICENSE
+-rw-r--r--   0        0        0      663 2023-04-27 15:37:54.210365 vvvvid_downloader-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-04-27 15:36:29.529395 vvvvid_downloader-1.3.2/vvvvid_downloader/__init__.py
+-rw-r--r--   0        0        0     4180 2023-04-27 14:53:50.208970 vvvvid_downloader-1.3.2/vvvvid_downloader/__main__.py
+-rw-r--r--   0        0        0     1852 2023-04-27 14:44:09.271044 vvvvid_downloader-1.3.2/vvvvid_downloader/api.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:44:09.271044 vvvvid_downloader-1.3.2/vvvvid_downloader/py.typed
+-rw-r--r--   0        0        0     9663 2023-04-27 15:09:03.413557 vvvvid_downloader-1.3.2/vvvvid_downloader/responses.py
+-rw-r--r--   0        0        0     1308 2023-04-27 14:44:09.271044 vvvvid_downloader-1.3.2/vvvvid_downloader/vvvvid.py
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 vvvvid_downloader-1.3.2/PKG-INFO
```

### Comparing `vvvvid_downloader-1.3.1/CHANGELOG.md` & `vvvvid_downloader-1.3.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.1/README.md` & `vvvvid_downloader-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.1/UNLICENSE` & `vvvvid_downloader-1.3.2/UNLICENSE`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.1/pyproject.toml` & `vvvvid_downloader-1.3.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9"
 ]
 description-file = "README.md"
 requires = [
-    "inquirer ==2.9.1",
-    "httpx ==0.21.1",
-    "rich ==10.16.2",
-    "click ==8.0.3",
+    "inquirer ==3.1.3",
+    "httpx ==0.24.0",
+    "rich ==13.3.5",
+    "click ==8.1.3",
     "h2 >=3,<5"
 ]
 requires-python = ">=3.9"
 
 [tool.isort]
 profile = "black"
```

### Comparing `vvvvid_downloader-1.3.1/PKG-INFO` & `vvvvid_downloader-1.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vvvvid_downloader
-Version: 1.3.1
+Version: 1.3.2
 Summary: Uno script in Python per scaricare da VVVVID. 
 Home-page: https://github.com/nearata/vvvvid-downloader
 Author: Nearata
 Author-email: nearata@protonmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: inquirer ==2.9.1
-Requires-Dist: httpx ==0.21.1
-Requires-Dist: rich ==10.16.2
-Requires-Dist: click ==8.0.3
+Requires-Dist: inquirer ==3.1.3
+Requires-Dist: httpx ==0.24.0
+Requires-Dist: rich ==13.3.5
+Requires-Dist: click ==8.1.3
 Requires-Dist: h2 >=3,<5
 
 # VVVVID Downloader
 
 > Uno script in Python per scaricare da VVVVID.
 
 ## Requisiti
```


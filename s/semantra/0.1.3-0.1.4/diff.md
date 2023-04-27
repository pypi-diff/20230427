# Comparing `tmp/semantra-0.1.3.tar.gz` & `tmp/semantra-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.1.3.tar", last modified: Wed Apr 26 04:21:20 2023, max compression
+gzip compressed data, was "semantra-0.1.4.tar", last modified: Thu Apr 27 04:40:14 2023, max compression
```

## Comparing `semantra-0.1.3.tar` & `semantra-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.028869 semantra-0.1.3/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.1.3/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)    10618 2023-04-26 04:21:20.028656 semantra-0.1.3/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)    10075 2023-04-26 04:20:51.000000 semantra-0.1.3/README.md
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.016445 semantra-0.1.3/client/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.018545 semantra-0.1.3/client/public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.020494 semantra-0.1.3/client/public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-23 21:34:21.000000 semantra-0.1.3/client/public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449083 2023-04-23 21:34:21.000000 semantra-0.1.3/client/public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495725 2023-04-23 21:34:21.000000 semantra-0.1.3/client/public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.3/client/public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.3/client/public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.1.3/client/public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)     1020 2023-04-26 04:20:51.000000 semantra-0.1.3/pyproject.toml
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-26 04:21:20.028907 semantra-0.1.3/setup.cfg
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.016707 semantra-0.1.3/src/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.024271 semantra-0.1.3/src/semantra/
--rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.1.3/src/semantra/__init__.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.026286 semantra-0.1.3/src/semantra/__pycache__/
--rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.1.3/src/semantra/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    10961 2023-04-23 04:37:57.000000 semantra-0.1.3/src/semantra/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     3086 2023-04-23 04:37:58.000000 semantra-0.1.3/src/semantra/__pycache__/pdf.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    19561 2023-04-23 12:15:19.000000 semantra-0.1.3/src/semantra/__pycache__/semantra.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-04-23 04:37:58.000000 semantra-0.1.3/src/semantra/__pycache__/util.cpython-39.pyc
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.026717 semantra-0.1.3/src/semantra/client_public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.027418 semantra-0.1.3/src/semantra/client_public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-23 21:34:21.000000 semantra-0.1.3/src/semantra/client_public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449083 2023-04-23 21:34:21.000000 semantra-0.1.3/src/semantra/client_public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495725 2023-04-23 21:34:21.000000 semantra-0.1.3/src/semantra/client_public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.3/src/semantra/client_public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.3/src/semantra/client_public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.1.3/src/semantra/client_public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)    11501 2023-04-26 04:12:41.000000 semantra-0.1.3/src/semantra/models.py
--rw-r--r--   0 freedmand   (501) staff       (20)     3325 2023-04-26 04:20:51.000000 semantra-0.1.3/src/semantra/pdf.py
--rw-r--r--   0 freedmand   (501) staff       (20)    28701 2023-04-26 04:12:41.000000 semantra-0.1.3/src/semantra/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-26 04:12:41.000000 semantra-0.1.3/src/semantra/util.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.025097 semantra-0.1.3/src/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)    10618 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      176 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/top_level.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:40:14.062604 semantra-0.1.4/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.1.4/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)    10618 2023-04-27 04:40:14.062250 semantra-0.1.4/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)    10075 2023-04-26 12:51:15.000000 semantra-0.1.4/README.md
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:40:14.052308 semantra-0.1.4/client/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:40:14.054674 semantra-0.1.4/client/public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:40:14.055859 semantra-0.1.4/client/public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-27 04:27:23.000000 semantra-0.1.4/client/public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449083 2023-04-27 04:38:40.000000 semantra-0.1.4/client/public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495725 2023-04-27 04:38:40.000000 semantra-0.1.4/client/public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.4/client/public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.4/client/public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-27 04:38:40.000000 semantra-0.1.4/client/public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)     1020 2023-04-27 04:39:47.000000 semantra-0.1.4/pyproject.toml
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-27 04:40:14.062643 semantra-0.1.4/setup.cfg
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:40:14.052590 semantra-0.1.4/src/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:40:14.057745 semantra-0.1.4/src/semantra/
+-rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.1.4/src/semantra/__init__.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:40:14.059832 semantra-0.1.4/src/semantra/__pycache__/
+-rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.1.4/src/semantra/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    10961 2023-04-23 04:37:57.000000 semantra-0.1.4/src/semantra/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     3086 2023-04-23 04:37:58.000000 semantra-0.1.4/src/semantra/__pycache__/pdf.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    19561 2023-04-23 12:15:19.000000 semantra-0.1.4/src/semantra/__pycache__/semantra.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-04-23 04:37:58.000000 semantra-0.1.4/src/semantra/__pycache__/util.cpython-39.pyc
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:40:14.060332 semantra-0.1.4/src/semantra/client_public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:40:14.061021 semantra-0.1.4/src/semantra/client_public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-27 04:27:23.000000 semantra-0.1.4/src/semantra/client_public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449083 2023-04-27 04:38:40.000000 semantra-0.1.4/src/semantra/client_public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495725 2023-04-27 04:38:40.000000 semantra-0.1.4/src/semantra/client_public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.4/src/semantra/client_public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.4/src/semantra/client_public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-27 04:38:40.000000 semantra-0.1.4/src/semantra/client_public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)    11501 2023-04-27 04:38:40.000000 semantra-0.1.4/src/semantra/models.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     3325 2023-04-27 04:38:40.000000 semantra-0.1.4/src/semantra/pdf.py
+-rw-r--r--   0 freedmand   (501) staff       (20)    28701 2023-04-27 04:38:40.000000 semantra-0.1.4/src/semantra/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-27 04:38:40.000000 semantra-0.1.4/src/semantra/util.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:40:14.058615 semantra-0.1.4/src/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)    10618 2023-04-27 04:40:14.000000 semantra-0.1.4/src/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-04-27 04:40:14.000000 semantra-0.1.4/src/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-27 04:40:14.000000 semantra-0.1.4/src/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-27 04:40:14.000000 semantra-0.1.4/src/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      176 2023-04-27 04:40:14.000000 semantra-0.1.4/src/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-27 04:40:14.000000 semantra-0.1.4/src/semantra.egg-info/top_level.txt
```

### Comparing `semantra-0.1.3/LICENSE` & `semantra-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/PKG-INFO` & `semantra-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.1.3
+Version: 0.1.4
 Summary: A semantic search CLI tool
 Author-email: Dylan Freedman <freedmand@gmail.com>
 Project-URL: Homepage, https://github.com/freedmand/semantra
 Project-URL: Repository, https://github.com/freedmand/semantra
 Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `semantra-0.1.3/README.md` & `semantra-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/client/public/build/bundle.css` & `semantra-0.1.4/client/public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/client/public/build/bundle.js` & `semantra-0.1.4/client/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/client/public/build/bundle.js.map` & `semantra-0.1.4/client/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/client/public/favicon.png` & `semantra-0.1.4/client/public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/client/public/global.css` & `semantra-0.1.4/client/public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/pyproject.toml` & `semantra-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semantra"
-version = "0.1.3"
+version = "0.1.4"
 description = "A semantic search CLI tool"
 authors = [{name = "Dylan Freedman", email = "freedmand@gmail.com"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `semantra-0.1.3/src/semantra/__pycache__/models.cpython-39.pyc` & `semantra-0.1.4/src/semantra/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/__pycache__/pdf.cpython-39.pyc` & `semantra-0.1.4/src/semantra/__pycache__/pdf.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/__pycache__/semantra.cpython-39.pyc` & `semantra-0.1.4/src/semantra/__pycache__/semantra.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/__pycache__/util.cpython-39.pyc` & `semantra-0.1.4/src/semantra/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/client_public/build/bundle.css` & `semantra-0.1.4/src/semantra/client_public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/client_public/build/bundle.js` & `semantra-0.1.4/src/semantra/client_public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/client_public/build/bundle.js.map` & `semantra-0.1.4/src/semantra/client_public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/client_public/favicon.png` & `semantra-0.1.4/src/semantra/client_public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/client_public/global.css` & `semantra-0.1.4/src/semantra/client_public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/models.py` & `semantra-0.1.4/src/semantra/models.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/pdf.py` & `semantra-0.1.4/src/semantra/pdf.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/semantra.py` & `semantra-0.1.4/src/semantra/semantra.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra/util.py` & `semantra-0.1.4/src/semantra/util.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.3/src/semantra.egg-info/PKG-INFO` & `semantra-0.1.4/src/semantra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.1.3
+Version: 0.1.4
 Summary: A semantic search CLI tool
 Author-email: Dylan Freedman <freedmand@gmail.com>
 Project-URL: Homepage, https://github.com/freedmand/semantra
 Project-URL: Repository, https://github.com/freedmand/semantra
 Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `semantra-0.1.3/src/semantra.egg-info/SOURCES.txt` & `semantra-0.1.4/src/semantra.egg-info/SOURCES.txt`

 * *Files identical despite different names*


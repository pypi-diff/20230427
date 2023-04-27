# Comparing `tmp/materialyoucolor-1.0.1.tar.gz` & `tmp/materialyoucolor-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "materialyoucolor-1.0.1.tar", last modified: Sat Apr 22 13:18:27 2023, max compression
+gzip compressed data, was "materialyoucolor-1.1.tar", last modified: Thu Apr 27 16:45:47 2023, max compression
```

## Comparing `materialyoucolor-1.0.1.tar` & `materialyoucolor-1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:18:27.491904 materialyoucolor-1.0.1/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     1068 2023-04-22 12:23:08.000000 materialyoucolor-1.0.1/LICENSE
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     2551 2023-04-22 13:18:27.491904 materialyoucolor-1.0.1/PKG-INFO
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     2304 2023-04-22 12:54:42.000000 materialyoucolor-1.0.1/README.md
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:18:27.471904 materialyoucolor-1.0.1/materialyoucolor/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)       18 2023-04-22 13:12:56.000000 materialyoucolor-1.0.1/materialyoucolor/__init__.py
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:18:27.478571 materialyoucolor-1.0.1/materialyoucolor/blend/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:16:21.000000 materialyoucolor-1.0.1/materialyoucolor/blend/__init__.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     1940 2023-04-22 12:17:00.000000 materialyoucolor-1.0.1/materialyoucolor/blend/blend.py
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:18:27.481904 materialyoucolor-1.0.1/materialyoucolor/hct/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:16:27.000000 materialyoucolor-1.0.1/materialyoucolor/hct/__init__.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     7315 2023-04-22 12:16:44.000000 materialyoucolor-1.0.1/materialyoucolor/hct/cam16.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     3961 2023-04-22 12:19:17.000000 materialyoucolor-1.0.1/materialyoucolor/hct/hct.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     2476 2023-04-22 12:15:44.000000 materialyoucolor-1.0.1/materialyoucolor/hct/viewing_conditions.py
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:18:27.485237 materialyoucolor-1.0.1/materialyoucolor/palettes/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:16:58.000000 materialyoucolor-1.0.1/materialyoucolor/palettes/__init__.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)      645 2023-04-22 12:19:31.000000 materialyoucolor-1.0.1/materialyoucolor/palettes/core_palette.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)      971 2023-04-22 12:20:14.000000 materialyoucolor-1.0.1/materialyoucolor/palettes/tonal_palette.py
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:18:27.485237 materialyoucolor-1.0.1/materialyoucolor/scheme/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:17:04.000000 materialyoucolor-1.0.1/materialyoucolor/scheme/__init__.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     8061 2023-04-22 12:20:03.000000 materialyoucolor-1.0.1/materialyoucolor/scheme/scheme.py
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:18:27.485237 materialyoucolor-1.0.1/materialyoucolor/score/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:16:34.000000 materialyoucolor-1.0.1/materialyoucolor/score/__init__.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     3347 2023-04-22 12:19:59.000000 materialyoucolor-1.0.1/materialyoucolor/score/score.py
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:18:27.491904 materialyoucolor-1.0.1/materialyoucolor/utils/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:16:30.000000 materialyoucolor-1.0.1/materialyoucolor/utils/__init__.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)    15411 2023-04-22 12:18:32.000000 materialyoucolor-1.0.1/materialyoucolor/utils/color_utils.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     1099 2023-04-17 10:11:07.000000 materialyoucolor-1.0.1/materialyoucolor/utils/math_utils.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     1423 2023-04-22 12:23:00.000000 materialyoucolor-1.0.1/materialyoucolor/utils/string_utils.py
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     3115 2023-04-22 12:19:48.000000 materialyoucolor-1.0.1/materialyoucolor/utils/theme_utils.py
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 13:18:27.475237 materialyoucolor-1.0.1/materialyoucolor.egg-info/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     2551 2023-04-22 13:18:27.000000 materialyoucolor-1.0.1/materialyoucolor.egg-info/PKG-INFO
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)      902 2023-04-22 13:18:27.000000 materialyoucolor-1.0.1/materialyoucolor.egg-info/SOURCES.txt
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        1 2023-04-22 13:18:27.000000 materialyoucolor-1.0.1/materialyoucolor.egg-info/dependency_links.txt
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        7 2023-04-22 13:18:27.000000 materialyoucolor-1.0.1/materialyoucolor.egg-info/requires.txt
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)       17 2023-04-22 13:18:27.000000 materialyoucolor-1.0.1/materialyoucolor.egg-info/top_level.txt
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)       38 2023-04-22 13:18:27.491904 materialyoucolor-1.0.1/setup.cfg
--rwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)      625 2023-04-22 13:18:14.000000 materialyoucolor-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.593905 materialyoucolor-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-27 16:45:26.000000 materialyoucolor-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-27 16:45:47.593905 materialyoucolor-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-27 16:45:26.000000 materialyoucolor-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.585905 materialyoucolor-1.1/materialyoucolor/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/blend/blend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/hct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/cam16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/hct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/viewing_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/palettes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/palettes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/palettes/core_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/palettes/tonal_palette.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/scheme/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/score/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/score/score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.593905 materialyoucolor-1.1/materialyoucolor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/theme_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:45:47.593905 materialyoucolor-1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      750 2023-04-27 16:45:26.000000 materialyoucolor-1.1/setup.py
```

### Comparing `materialyoucolor-1.0.1/LICENSE` & `materialyoucolor-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/PKG-INFO` & `materialyoucolor-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: materialyoucolor
-Version: 1.0.1
+Version: 1.1
 Summary: Material You color generation algorithms in pure python!
 Author: Ansh Dadwal
 Author-email: anshdadwal298@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # materialyoucolor-pyhton
```

### Comparing `materialyoucolor-1.0.1/README.md` & `materialyoucolor-1.1/README.md`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/blend/blend.py` & `materialyoucolor-1.1/materialyoucolor/blend/blend.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/hct/cam16.py` & `materialyoucolor-1.1/materialyoucolor/hct/cam16.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/hct/hct.py` & `materialyoucolor-1.1/materialyoucolor/hct/hct.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/hct/viewing_conditions.py` & `materialyoucolor-1.1/materialyoucolor/hct/viewing_conditions.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/palettes/core_palette.py` & `materialyoucolor-1.1/materialyoucolor/palettes/core_palette.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/palettes/tonal_palette.py` & `materialyoucolor-1.1/materialyoucolor/palettes/tonal_palette.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/scheme/scheme.py` & `materialyoucolor-1.1/materialyoucolor/scheme/scheme.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/score/score.py` & `materialyoucolor-1.1/materialyoucolor/score/score.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/utils/color_utils.py` & `materialyoucolor-1.1/materialyoucolor/utils/color_utils.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/utils/math_utils.py` & `materialyoucolor-1.1/materialyoucolor/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/utils/string_utils.py` & `materialyoucolor-1.1/materialyoucolor/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor/utils/theme_utils.py` & `materialyoucolor-1.1/materialyoucolor/utils/theme_utils.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0.1/materialyoucolor.egg-info/PKG-INFO` & `materialyoucolor-1.1/materialyoucolor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: materialyoucolor
-Version: 1.0.1
+Version: 1.1
 Summary: Material You color generation algorithms in pure python!
 Author: Ansh Dadwal
 Author-email: anshdadwal298@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # materialyoucolor-pyhton
```

### Comparing `materialyoucolor-1.0.1/materialyoucolor.egg-info/SOURCES.txt` & `materialyoucolor-1.1/materialyoucolor.egg-info/SOURCES.txt`

 * *Files identical despite different names*


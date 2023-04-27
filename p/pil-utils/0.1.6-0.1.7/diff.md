# Comparing `tmp/pil_utils-0.1.6.tar.gz` & `tmp/pil_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pil_utils-0.1.6.tar", max compression
+gzip compressed data, was "pil_utils-0.1.7.tar", max compression
```

## Comparing `pil_utils-0.1.6.tar` & `pil_utils-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-04-04 05:31:48.632330 pil_utils-0.1.6/LICENSE
--rw-r--r--   0        0        0     4487 2023-04-04 05:31:48.632330 pil_utils-0.1.6/README.md
--rw-r--r--   0        0        0       83 2023-04-04 05:31:48.632330 pil_utils-0.1.6/pil_utils/__init__.py
--rw-r--r--   0        0        0    21621 2023-04-04 05:31:48.632330 pil_utils-0.1.6/pil_utils/build_image.py
--rw-r--r--   0        0        0     4638 2023-04-04 05:31:48.632330 pil_utils-0.1.6/pil_utils/fonts.py
--rw-r--r--   0        0        0     3557 2023-04-04 05:31:48.632330 pil_utils-0.1.6/pil_utils/gradient.py
--rw-r--r--   0        0        0    18354 2023-04-04 05:31:48.632330 pil_utils-0.1.6/pil_utils/text2image.py
--rw-r--r--   0        0        0      948 2023-04-04 05:31:48.632330 pil_utils-0.1.6/pil_utils/types.py
--rw-r--r--   0        0        0      611 2023-04-04 05:31:48.636330 pil_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5389 1970-01-01 00:00:00.000000 pil_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-27 05:42:16.041846 pil_utils-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4487 2023-04-27 05:42:16.041846 pil_utils-0.1.7/README.md
+-rw-r--r--   0        0        0       83 2023-04-27 05:42:16.041846 pil_utils-0.1.7/pil_utils/__init__.py
+-rw-r--r--   0        0        0    21677 2023-04-27 05:42:16.041846 pil_utils-0.1.7/pil_utils/build_image.py
+-rw-r--r--   0        0        0     4638 2023-04-27 05:42:16.041846 pil_utils-0.1.7/pil_utils/fonts.py
+-rw-r--r--   0        0        0     3557 2023-04-27 05:42:16.041846 pil_utils-0.1.7/pil_utils/gradient.py
+-rw-r--r--   0        0        0    18354 2023-04-27 05:42:16.041846 pil_utils-0.1.7/pil_utils/text2image.py
+-rw-r--r--   0        0        0      948 2023-04-27 05:42:16.041846 pil_utils-0.1.7/pil_utils/types.py
+-rw-r--r--   0        0        0      611 2023-04-27 05:42:16.045846 pil_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5389 1970-01-01 00:00:00.000000 pil_utils-0.1.7/PKG-INFO
```

### Comparing `pil_utils-0.1.6/LICENSE` & `pil_utils-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pil_utils-0.1.6/README.md` & `pil_utils-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pil_utils-0.1.6/pil_utils/build_image.py` & `pil_utils-0.1.7/pil_utils/build_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,21 +453,23 @@
           * ``stroke_fill``: 描边颜色
           * ``font_fallback``: 是否使用后备字体，默认为 `True`
           * ``fontname``: 指定首选字体
           * ``fallback_fonts``: 指定备选字体
         """
 
         if len(xy) == 2:
-            text2img = Text2Image.from_bbcode_text(
+            text2img = Text2Image.from_text(
                 text,
                 fontsize,
+                style,
+                weight,
                 fill,
                 spacing,
                 lines_align,
-                stroke_ratio,
+                int(fontsize * stroke_ratio),
                 stroke_fill,
                 font_fallback,
                 fontname,
                 fallback_fonts,
             )
             text2img.draw_on_image(self.image, xy)
             return self
```

### Comparing `pil_utils-0.1.6/pil_utils/fonts.py` & `pil_utils-0.1.7/pil_utils/fonts.py`

 * *Files identical despite different names*

### Comparing `pil_utils-0.1.6/pil_utils/gradient.py` & `pil_utils-0.1.7/pil_utils/gradient.py`

 * *Files identical despite different names*

### Comparing `pil_utils-0.1.6/pil_utils/text2image.py` & `pil_utils-0.1.7/pil_utils/text2image.py`

 * *Files identical despite different names*

### Comparing `pil_utils-0.1.6/pil_utils/types.py` & `pil_utils-0.1.7/pil_utils/types.py`

 * *Files identical despite different names*

### Comparing `pil_utils-0.1.6/pyproject.toml` & `pil_utils-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pil-utils"
-version = "0.1.6"
+version = "0.1.7"
 description = "A simple PIL wrapper and text-to-image tool"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MeetWq/pil-utils"
 repository = "https://github.com/MeetWq/pil-utils"
```

### Comparing `pil_utils-0.1.6/PKG-INFO` & `pil_utils-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pil-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple PIL wrapper and text-to-image tool
 Home-page: https://github.com/MeetWq/pil-utils
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


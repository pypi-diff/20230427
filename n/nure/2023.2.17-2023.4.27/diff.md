# Comparing `tmp/nure-2023.2.17.tar.gz` & `tmp/nure-2023.4.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nure-2023.2.17.tar", last modified: Fri Feb 17 09:52:59 2023, max compression
+gzip compressed data, was "nure-2023.4.27.tar", last modified: Thu Apr 27 06:52:27 2023, max compression
```

## Comparing `nure-2023.2.17.tar` & `nure-2023.4.27.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-02-17 09:52:57.543160 nure-2023.2.17/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    35149 2021-05-21 04:50:18.000000 nure-2023.2.17/LICENSE
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-02-17 09:52:57.543160 nure-2023.2.17/PKG-INFO
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       30 2021-05-21 04:25:06.000000 nure-2023.2.17/README.md
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-02-17 09:52:57.065624 nure-2023.2.17/nure/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:41:00.000000 nure-2023.2.17/nure/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2523 2021-11-20 09:30:50.000000 nure-2023.2.17/nure/archive.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2379 2021-11-30 04:05:06.000000 nure-2023.2.17/nure/array.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-02-17 09:52:57.102693 nure-2023.2.17/nure/code/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       62 2021-07-13 10:11:18.000000 nure-2023.2.17/nure/code/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1353 2021-07-13 16:16:01.000000 nure-2023.2.17/nure/code/label_coder.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     4912 2022-07-29 07:41:08.000000 nure-2023.2.17/nure/dataframe.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1263 2021-07-21 05:24:39.000000 nure-2023.2.17/nure/datetime.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      106 2021-05-21 06:28:06.000000 nure-2023.2.17/nure/debug.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1325 2022-11-14 10:39:27.000000 nure-2023.2.17/nure/dict.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      487 2021-11-30 04:03:48.000000 nure-2023.2.17/nure/func.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-02-17 09:52:57.197537 nure-2023.2.17/nure/image/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2022-04-14 09:32:11.000000 nure-2023.2.17/nure/image/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    10331 2022-04-14 09:44:09.000000 nure-2023.2.17/nure/image/annotate.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6438 2022-04-14 09:32:48.000000 nure-2023.2.17/nure/image/func.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     5594 2022-04-14 09:43:18.000000 nure-2023.2.17/nure/image/pil.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1457 2022-03-22 08:57:21.000000 nure-2023.2.17/nure/meta.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      445 2021-05-21 04:25:40.000000 nure-2023.2.17/nure/path.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-02-17 09:52:57.355656 nure-2023.2.17/nure/sync/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:53:57.000000 nure-2023.2.17/nure/sync/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      457 2021-05-21 09:16:57.000000 nure-2023.2.17/nure/sync/bigquery.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1628 2021-11-30 04:09:01.000000 nure-2023.2.17/nure/sync/cache.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3249 2021-07-23 06:18:01.000000 nure-2023.2.17/nure/sync/googlesheet.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      706 2021-05-21 09:17:03.000000 nure-2023.2.17/nure/sync/postgre.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3054 2023-02-17 09:37:27.000000 nure-2023.2.17/nure/sync/s3.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1806 2022-09-18 04:11:30.000000 nure-2023.2.17/nure/sync/sql.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1450 2021-09-17 11:26:33.000000 nure-2023.2.17/nure/sync/suffix.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2872 2021-11-05 14:16:28.000000 nure-2023.2.17/nure/volatitle.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-02-17 09:52:57.418160 nure-2023.2.17/nure.egg-info/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-02-17 09:52:56.000000 nure-2023.2.17/nure.egg-info/PKG-INFO
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      842 2023-02-17 09:52:56.000000 nure-2023.2.17/nure.egg-info/SOURCES.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        1 2023-02-17 09:52:56.000000 nure-2023.2.17/nure.egg-info/dependency_links.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      145 2023-02-17 09:52:56.000000 nure-2023.2.17/nure.egg-info/requires.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        5 2023-02-17 09:52:56.000000 nure-2023.2.17/nure.egg-info/top_level.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      103 2021-05-21 04:28:28.000000 nure-2023.2.17/pyproject.toml
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      849 2023-02-17 09:52:57.543160 nure-2023.2.17/setup.cfg
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-02-17 09:52:57.527534 nure-2023.2.17/tests/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1011 2021-11-20 09:51:16.000000 nure-2023.2.17/tests/test_archive.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1225 2021-09-17 11:28:32.000000 nure-2023.2.17/tests/test_bigquery.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2890 2021-07-13 16:25:33.000000 nure-2023.2.17/tests/test_coder.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      792 2021-07-23 06:18:01.000000 nure-2023.2.17/tests/test_googlesheet.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3698 2021-11-30 04:05:08.000000 nure-2023.2.17/tests/test_parallel.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      708 2021-09-17 11:49:25.000000 nure-2023.2.17/tests/test_postgre.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      655 2021-10-08 07:11:48.000000 nure-2023.2.17/tests/test_s3.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:26.389725 nure-2023.4.27/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    35149 2021-05-21 04:50:18.000000 nure-2023.4.27/LICENSE
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-04-27 06:52:26.390870 nure-2023.4.27/PKG-INFO
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       30 2021-05-21 04:25:06.000000 nure-2023.4.27/README.md
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:25.875040 nure-2023.4.27/nure/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:41:00.000000 nure-2023.4.27/nure/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2523 2021-11-20 09:30:50.000000 nure-2023.4.27/nure/archive.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2379 2021-11-30 04:05:06.000000 nure-2023.4.27/nure/array.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:25.915948 nure-2023.4.27/nure/code/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       62 2021-07-13 10:11:18.000000 nure-2023.4.27/nure/code/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1353 2021-07-13 16:16:01.000000 nure-2023.4.27/nure/code/label_coder.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     4912 2022-07-29 07:41:08.000000 nure-2023.4.27/nure/dataframe.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1263 2021-07-21 05:24:39.000000 nure-2023.4.27/nure/datetime.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      106 2021-05-21 06:28:06.000000 nure-2023.4.27/nure/debug.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1325 2022-11-14 10:39:27.000000 nure-2023.4.27/nure/dict.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      487 2021-11-30 04:03:48.000000 nure-2023.4.27/nure/func.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:26.005656 nure-2023.4.27/nure/image/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2022-04-14 09:32:11.000000 nure-2023.4.27/nure/image/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    10331 2022-04-14 09:44:09.000000 nure-2023.4.27/nure/image/annotate.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6438 2022-04-14 09:32:48.000000 nure-2023.4.27/nure/image/func.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     5944 2023-04-27 06:39:33.000000 nure-2023.4.27/nure/image/pil.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1457 2022-03-22 08:57:21.000000 nure-2023.4.27/nure/meta.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      445 2021-05-21 04:25:40.000000 nure-2023.4.27/nure/path.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:26.176942 nure-2023.4.27/nure/sync/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:53:57.000000 nure-2023.4.27/nure/sync/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      457 2021-05-21 09:16:57.000000 nure-2023.4.27/nure/sync/bigquery.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1628 2021-11-30 04:09:01.000000 nure-2023.4.27/nure/sync/cache.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3249 2021-07-23 06:18:01.000000 nure-2023.4.27/nure/sync/googlesheet.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      706 2021-05-21 09:17:03.000000 nure-2023.4.27/nure/sync/postgre.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3055 2023-04-27 06:21:53.000000 nure-2023.4.27/nure/sync/s3.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1806 2022-09-18 04:11:30.000000 nure-2023.4.27/nure/sync/sql.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1450 2021-09-17 11:26:33.000000 nure-2023.4.27/nure/sync/suffix.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2872 2021-11-05 14:16:28.000000 nure-2023.4.27/nure/volatitle.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:26.254263 nure-2023.4.27/nure.egg-info/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-04-27 06:52:25.000000 nure-2023.4.27/nure.egg-info/PKG-INFO
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      842 2023-04-27 06:52:25.000000 nure-2023.4.27/nure.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        1 2023-04-27 06:52:25.000000 nure-2023.4.27/nure.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      145 2023-04-27 06:52:25.000000 nure-2023.4.27/nure.egg-info/requires.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        5 2023-04-27 06:52:25.000000 nure-2023.4.27/nure.egg-info/top_level.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      103 2021-05-21 04:28:28.000000 nure-2023.4.27/pyproject.toml
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      849 2023-04-27 06:52:26.396545 nure-2023.4.27/setup.cfg
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-04-27 06:52:26.372464 nure-2023.4.27/tests/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1011 2021-11-20 09:51:16.000000 nure-2023.4.27/tests/test_archive.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1225 2021-09-17 11:28:32.000000 nure-2023.4.27/tests/test_bigquery.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2890 2021-07-13 16:25:33.000000 nure-2023.4.27/tests/test_coder.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      792 2021-07-23 06:18:01.000000 nure-2023.4.27/tests/test_googlesheet.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3698 2021-11-30 04:05:08.000000 nure-2023.4.27/tests/test_parallel.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      708 2021-09-17 11:49:25.000000 nure-2023.4.27/tests/test_postgre.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      655 2021-10-08 07:11:48.000000 nure-2023.4.27/tests/test_s3.py
```

### Comparing `nure-2023.2.17/LICENSE` & `nure-2023.4.27/LICENSE`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/PKG-INFO` & `nure-2023.4.27/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nure
-Version: 2023.2.17
+Version: 2023.4.27
 Summary: Data Science Utilities
 Home-page: https://github.com/tranduytrung/nure
 Author: Trung Tran
 Author-email: tranduytrung@outlook.com
 Project-URL: Bug Tracker, https://github.com/tranduytrung/nure/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nure-2023.2.17/nure/archive.py` & `nure-2023.4.27/nure/archive.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/array.py` & `nure-2023.4.27/nure/array.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/code/label_coder.py` & `nure-2023.4.27/nure/code/label_coder.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/dataframe.py` & `nure-2023.4.27/nure/dataframe.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/datetime.py` & `nure-2023.4.27/nure/datetime.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/dict.py` & `nure-2023.4.27/nure/dict.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/image/annotate.py` & `nure-2023.4.27/nure/image/annotate.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/image/func.py` & `nure-2023.4.27/nure/image/func.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/image/pil.py` & `nure-2023.4.27/nure/image/pil.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-import numpy as np
+from typing import Dict, Any, Tuple, List
 
+import numpy as np
 import PIL.Image
 import PIL.ImageColor
 import PIL.ImageDraw
 import PIL.ImageFont
+from PIL.Image import Image
+from PIL.ImageFont import ImageFont
 
 from . import func
 
 
-def wrap_text(text, font: PIL.ImageFont.ImageFont, width):
+def wrap_text(text, font: ImageFont, width):
     w, _ = font.getsize(text)
     max_char = int((width / w) * len(text))
     n_lines = len(text) // max_char + (len(text) % max_char != 0)
     wrapped_text = '\n'.join([text[i * max_char:(i + 1) * max_char] for i in range(n_lines)])
     return wrapped_text
 
 
-def draw_text(image, text, pos=(0, 0), font=None, text_color='white', background_color='black', wrap=False):
+def draw_text(image: Image, text: str, pos=(0, 0), font=None, text_color='white', background_color='black', wrap=False):
     # get font
     if font is None:
         font = PIL.ImageFont.load_default()
     # context
     draw = PIL.ImageDraw.Draw(image)
 
     # draw background
@@ -37,35 +40,37 @@
             width = image.size[0] - pos[0]
         text = wrap_text(text, font, width)
 
     # draw text
     draw.text(pos, text, fill=text_color, font=font)
 
 
-def draw_receptive_field(image, size=224, outline=(255, 0, 0)):
+def draw_receptive_field(image: Image, size=224, outline=(255, 0, 0)):
     # context
     draw = PIL.ImageDraw.Draw(image)
     # retangle
     image_size = image.size
     left_top = (np.array(image_size) - size) // 2
     right_bottom = left_top + size
     draw.rectangle([*left_top, *right_bottom], outline=outline, width=3)
 
 
-def draw_rect(image, box=[0, 0, 224, 224], outline=(255, 0, 0), width=2):
+def draw_rect(image: Image, box=[0, 0, 224, 224], outline=(255, 0, 0), width=2):
     # context
     draw = PIL.ImageDraw.Draw(image)
     # retangle
     draw.rectangle(box, outline=outline, width=width)
 
 
 __default_colors__ = [PIL.ImageColor.getrgb(c) for c in ['#B22222', '#FF69B4', '#FF6347', '#FFD700', '#ADFF2F', '#40E0D0']]
 
 
-def draw_bboxes(image, bboxes, classes, scores=None, id2name=None, colors=__default_colors__, copy=True):
+def draw_bboxes(image: Image, bboxes: np.ndarray, classes: np.ndarray,
+                scores: np.ndarray = None, id2name: Dict[Any, str] = None,
+                colors=__default_colors__, font: ImageFont = None, copy=True):
     """ draw bounding boxes with their class names on images
     Input:
         image: PIL.Image
         bboxes: [n_boxes, (x1, y1, x2, y2)]
         classes, scores: [n_boxes]
         id2name: dict
     """
@@ -73,15 +78,17 @@
         image = image.copy()
 
     if id2name is not None:
         labels = [id2name.get(cid, 'unknown') for cid in classes]
     else:
         labels = [str(cid) for cid in classes]
 
-    font = PIL.ImageFont.truetype('./fonts/Roboto-Regular.ttf', size=14)
+    # get font
+    if font is None:
+        font = PIL.ImageFont.load_default()
 
     for idx in range(bboxes.shape[0]):
         color = colors[idx % len(colors)]
         x1, y1, x2, y2 = bboxes[idx]
 
         draw_rect(image, [x1, y1, x2, y2], outline=color)
         text = str(labels[idx])
@@ -90,15 +97,15 @@
 
         _, h = font.getsize(text)
         draw_text(image, text, [x1, y1 - h], font=font, text_color='black', background_color=color)
 
     return image
 
 
-def make_grid(images, grid=None, max_size=224, bg_color=(255, 255, 255)):
+def make_grid(images: List[Image], grid: Tuple[int, int] = None, max_size=224, bg_color=(255, 255, 255)):
     """ make a image grid
     Parameters:
         images: array of PIL.Image
             list of image
         grid: 2-tuple of int or int
             (n_col, n_row) or n_col
         max_size: int
@@ -132,30 +139,35 @@
             background.paste(PIL.Image.fromarray(nResized), (left, top))
 
             pasted_images += 1
 
     return background
 
 
-def draw_palette(colors, size=64):
+def draw_palette(colors: List[Tuple[int, int, int]], size=64):
     palette = np.empty((size, len(colors) * size, 3), dtype=np.uint8)
     for i in range(len(colors)):
         palette[:, i * size:(i + 1) * size, :] = colors[i]
     return PIL.Image.fromarray(palette)
 
 
 EDGE_TOP = 0
 EDGE_LEFT = 1
 EDGE_RIGHT = 2
 EDGE_BOTTOM = 3
 
 
-def draw_text_at_edge(image, text, pos=EDGE_BOTTOM,
-                      font_size=14, text_width=100, background_color=0, text_color='white'):
-    font = PIL.ImageFont.truetype('./fonts/Roboto-Regular.ttf', size=font_size)
+def draw_text_at_edge(image: Image, text: str, pos=EDGE_BOTTOM,
+                      font: ImageFont = None, text_width=100,
+                      background_color=0, text_color='white'):
+
+    # get font
+    if font is None:
+        font = PIL.ImageFont.load_default()
+
     if pos in [EDGE_TOP, EDGE_BOTTOM]:
         text_width = image.size[0]
 
     wrapped_text = wrap_text(text, font, text_width)
     _, text_height = font.getsize_multiline(wrapped_text)
     if pos in [EDGE_TOP, EDGE_BOTTOM]:
         image_width = image.size[0]
```

### Comparing `nure-2023.2.17/nure/meta.py` & `nure-2023.4.27/nure/meta.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/sync/cache.py` & `nure-2023.4.27/nure/sync/cache.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/sync/googlesheet.py` & `nure-2023.4.27/nure/sync/googlesheet.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/sync/postgre.py` & `nure-2023.4.27/nure/sync/postgre.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/sync/s3.py` & `nure-2023.4.27/nure/sync/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class S3Uri:
     def __init__(self, bucket: str, key: str) -> None:
         self.bucket = bucket
         self.key = key
 
-    PARSE_RE = re.compile(R"^s3://(?P<bucket>[0-9a-z.-]+)\/(?P<key>([0-9A-Za-z!\-_.*'\()]+/?)+)(?<!/)$")
+    PARSE_RE = re.compile(R"^s3://(?P<bucket>[0-9a-z.-]+)\/(?P<key>([0-9A-Za-z!\-_.*%'\()]+/?)+)(?<!/)$")
 
     @staticmethod
     def parse(uri: str):
         # Bucket name
         # https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-s3-bucket-naming-requirements.html
         # Object name
         # https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-keys.html
```

### Comparing `nure-2023.2.17/nure/sync/sql.py` & `nure-2023.4.27/nure/sync/sql.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/sync/suffix.py` & `nure-2023.4.27/nure/sync/suffix.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure/volatitle.py` & `nure-2023.4.27/nure/volatitle.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/nure.egg-info/PKG-INFO` & `nure-2023.4.27/nure.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nure
-Version: 2023.2.17
+Version: 2023.4.27
 Summary: Data Science Utilities
 Home-page: https://github.com/tranduytrung/nure
 Author: Trung Tran
 Author-email: tranduytrung@outlook.com
 Project-URL: Bug Tracker, https://github.com/tranduytrung/nure/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nure-2023.2.17/nure.egg-info/SOURCES.txt` & `nure-2023.4.27/nure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/setup.cfg` & `nure-2023.4.27/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nure
-version = 2023.02.17
+version = 2023.04.27
 author = Trung Tran
 author_email = tranduytrung@outlook.com
 description = Data Science Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tranduytrung/nure
 project_urls =
```

### Comparing `nure-2023.2.17/tests/test_archive.py` & `nure-2023.4.27/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/tests/test_bigquery.py` & `nure-2023.4.27/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/tests/test_coder.py` & `nure-2023.4.27/tests/test_coder.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/tests/test_googlesheet.py` & `nure-2023.4.27/tests/test_googlesheet.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/tests/test_parallel.py` & `nure-2023.4.27/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/tests/test_postgre.py` & `nure-2023.4.27/tests/test_postgre.py`

 * *Files identical despite different names*

### Comparing `nure-2023.2.17/tests/test_s3.py` & `nure-2023.4.27/tests/test_s3.py`

 * *Files identical despite different names*


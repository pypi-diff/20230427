# Comparing `tmp/text_box_wrapper-0.1.3.tar.gz` & `tmp/text_box_wrapper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_box_wrapper-0.1.3.tar", last modified: Sun Apr 23 19:06:55 2023, max compression
+gzip compressed data, was "text_box_wrapper-0.1.4.tar", last modified: Thu Apr 27 15:59:52 2023, max compression
```

## Comparing `text_box_wrapper-0.1.3.tar` & `text_box_wrapper-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 panc       (501) staff       (20)        0 2023-04-23 19:06:55.800414 text_box_wrapper-0.1.3/
--rw-r--r--   0 panc       (501) staff       (20)     1061 2023-04-23 17:02:32.000000 text_box_wrapper-0.1.3/LICENSE
--rw-r--r--   0 panc       (501) staff       (20)     2615 2023-04-23 19:06:55.761950 text_box_wrapper-0.1.3/PKG-INFO
--rw-r--r--   0 panc       (501) staff       (20)     1954 2023-04-23 18:11:56.000000 text_box_wrapper-0.1.3/README.md
--rw-r--r--   0 panc       (501) staff       (20)       38 2023-04-23 19:06:55.800616 text_box_wrapper-0.1.3/setup.cfg
--rw-r--r--   0 panc       (501) staff       (20)      964 2023-04-23 19:06:45.000000 text_box_wrapper-0.1.3/setup.py
-drwxr-xr-x   0 panc       (501) staff       (20)        0 2023-04-23 19:06:55.752334 text_box_wrapper-0.1.3/text_box_wrapper/
--rw-r--r--   0 panc       (501) staff       (20)        0 2023-04-23 19:05:02.000000 text_box_wrapper-0.1.3/text_box_wrapper/__init__.py
--rw-r--r--   0 panc       (501) staff       (20)     3206 2023-04-22 21:29:11.000000 text_box_wrapper-0.1.3/text_box_wrapper/wrapper.py
-drwxr-xr-x   0 panc       (501) staff       (20)        0 2023-04-23 19:06:55.757889 text_box_wrapper-0.1.3/text_box_wrapper.egg-info/
--rw-r--r--   0 panc       (501) staff       (20)     2615 2023-04-23 19:06:55.000000 text_box_wrapper-0.1.3/text_box_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 panc       (501) staff       (20)      243 2023-04-23 19:06:55.000000 text_box_wrapper-0.1.3/text_box_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 panc       (501) staff       (20)        1 2023-04-23 19:06:55.000000 text_box_wrapper-0.1.3/text_box_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 panc       (501) staff       (20)       17 2023-04-23 19:06:55.000000 text_box_wrapper-0.1.3/text_box_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 panc       (501) staff       (20)        0 2023-04-27 15:59:52.460248 text_box_wrapper-0.1.4/
+-rw-r--r--   0 panc       (501) staff       (20)     1061 2023-04-23 17:02:32.000000 text_box_wrapper-0.1.4/LICENSE
+-rw-r--r--   0 panc       (501) staff       (20)     2614 2023-04-27 15:59:52.454488 text_box_wrapper-0.1.4/PKG-INFO
+-rw-r--r--   0 panc       (501) staff       (20)     1953 2023-04-27 15:57:45.000000 text_box_wrapper-0.1.4/README.md
+-rw-r--r--   0 panc       (501) staff       (20)       38 2023-04-27 15:59:52.461710 text_box_wrapper-0.1.4/setup.cfg
+-rw-r--r--   0 panc       (501) staff       (20)      982 2023-04-27 15:54:50.000000 text_box_wrapper-0.1.4/setup.py
+drwxr-xr-x   0 panc       (501) staff       (20)        0 2023-04-27 15:59:52.447763 text_box_wrapper-0.1.4/text_box_wrapper/
+-rw-r--r--   0 panc       (501) staff       (20)        0 2023-04-23 19:05:02.000000 text_box_wrapper-0.1.4/text_box_wrapper/__init__.py
+-rw-r--r--   0 panc       (501) staff       (20)     3084 2023-04-27 15:56:12.000000 text_box_wrapper-0.1.4/text_box_wrapper/wrapper.py
+drwxr-xr-x   0 panc       (501) staff       (20)        0 2023-04-27 15:59:52.453736 text_box_wrapper-0.1.4/text_box_wrapper.egg-info/
+-rw-r--r--   0 panc       (501) staff       (20)     2614 2023-04-27 15:59:52.000000 text_box_wrapper-0.1.4/text_box_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 panc       (501) staff       (20)      282 2023-04-27 15:59:52.000000 text_box_wrapper-0.1.4/text_box_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 panc       (501) staff       (20)        1 2023-04-27 15:59:52.000000 text_box_wrapper-0.1.4/text_box_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 panc       (501) staff       (20)        8 2023-04-27 15:59:52.000000 text_box_wrapper-0.1.4/text_box_wrapper.egg-info/requires.txt
+-rw-r--r--   0 panc       (501) staff       (20)       17 2023-04-27 15:59:52.000000 text_box_wrapper-0.1.4/text_box_wrapper.egg-info/top_level.txt
```

### Comparing `text_box_wrapper-0.1.3/LICENSE` & `text_box_wrapper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `text_box_wrapper-0.1.3/PKG-INFO` & `text_box_wrapper-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_box_wrapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple package to wrap text with ASCII art
 Home-page: https://github.com/Hootrix/text-box-wrapper
 Author: Ho
 Author-email: hhtjim@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -53,15 +53,15 @@
 ###########################################
 ```
 
 # Customizing the wrapper
 You can customize the padding, border string, 
 and alignment:
 ```
-from utils.common import wrap,wrap_with_ascii_art
+from text_box_wrapper import wrap_with_ascii_art
 
 text = "你好，成都"
 border_string = "#"
 wrapped_text = wrap_with_ascii_art(text, min_padding=5, vertical_padding=2, border_string=border_string, alignment="center")
 print(wrapped_text)
```

### Comparing `text_box_wrapper-0.1.3/README.md` & `text_box_wrapper-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ###########################################
 ```
 
 # Customizing the wrapper
 You can customize the padding, border string, 
 and alignment:
 ```
-from utils.common import wrap,wrap_with_ascii_art
+from text_box_wrapper import wrap_with_ascii_art
 
 text = "你好，成都"
 border_string = "#"
 wrapped_text = wrap_with_ascii_art(text, min_padding=5, vertical_padding=2, border_string=border_string, alignment="center")
 print(wrapped_text)
```

### Comparing `text_box_wrapper-0.1.3/setup.py` & `text_box_wrapper-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="text_box_wrapper",
-    version="0.1.3",
+    version="0.1.4",
     description="A simple package to wrap text with ASCII art",
     author="Ho",
     author_email="hhtjim@gmail.com",
     packages=find_packages(),
     install_requires=[
+        "wcwidth"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

### Comparing `text_box_wrapper-0.1.3/text_box_wrapper/wrapper.py` & `text_box_wrapper-0.1.4/text_box_wrapper/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import re
-import unicodedata
+from wcwidth import wcwidth
 from typing import Callable
 
 def wrap(min_padding=10, vertical_padding=None, border_string="#" * 5, alignment="center"):
     def decorator(func: Callable) -> Callable:
         def wrapper(*args, **kwargs):
             text = func(*args, **kwargs)
             return wrap_with_ascii_art(text, min_padding, vertical_padding, border_string, alignment)
         return wrapper
     return decorator
 
 def wrap_with_ascii_art(text, min_padding=10, vertical_padding=None, border_string="#" * 5, alignment="center") -> str:
-    def get_char_width(char):
-        width = unicodedata.east_asian_width(char)
-        return 2 if width in 'FWA' else 1
-
     def get_text_width(text):
-        return sum(get_char_width(char) for char in text)
+        return sum(wcwidth(char) for char in text)
     
     padding_char = " "
     ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')  # 用于匹配ANSI转义序列的正则表达式
     text_without_colors = ansi_escape.sub('', text)  # 移除彩色字符
     text_lines = text.split("\n")
     text_lines_without_colors = text_without_colors.split("\n")
```

### Comparing `text_box_wrapper-0.1.3/text_box_wrapper.egg-info/PKG-INFO` & `text_box_wrapper-0.1.4/text_box_wrapper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-box-wrapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple package to wrap text with ASCII art
 Home-page: https://github.com/Hootrix/text-box-wrapper
 Author: Ho
 Author-email: hhtjim@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -53,15 +53,15 @@
 ###########################################
 ```
 
 # Customizing the wrapper
 You can customize the padding, border string, 
 and alignment:
 ```
-from utils.common import wrap,wrap_with_ascii_art
+from text_box_wrapper import wrap_with_ascii_art
 
 text = "你好，成都"
 border_string = "#"
 wrapped_text = wrap_with_ascii_art(text, min_padding=5, vertical_padding=2, border_string=border_string, alignment="center")
 print(wrapped_text)
```


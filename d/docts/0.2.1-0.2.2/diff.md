# Comparing `tmp/docts-0.2.1.tar.gz` & `tmp/docts-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docts-0.2.1.tar", last modified: Thu Apr 27 08:24:43 2023, max compression
+gzip compressed data, was "docts-0.2.2.tar", last modified: Thu Apr 27 09:39:55 2023, max compression
```

## Comparing `docts-0.2.1.tar` & `docts-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:43.626972 docts-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 08:24:33.000000 docts-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 08:24:33.000000 docts-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-27 08:24:43.626972 docts-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-27 08:24:33.000000 docts-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 08:24:33.000000 docts-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 08:24:33.000000 docts-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:24:43.626972 docts-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:43.622972 docts-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:43.626972 docts-0.2.1/src/docts/
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-27 08:24:42.000000 docts-0.2.1/src/docts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 08:24:33.000000 docts-0.2.1/src/docts/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:43.626972 docts-0.2.1/src/docts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:55.387328 docts-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 09:39:47.000000 docts-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 09:39:47.000000 docts-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-27 09:39:55.387328 docts-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-27 09:39:47.000000 docts-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 09:39:47.000000 docts-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 09:39:47.000000 docts-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:39:55.387328 docts-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:55.387328 docts-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:55.387328 docts-0.2.2/src/docts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-04-27 09:39:54.000000 docts-0.2.2/src/docts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 09:39:47.000000 docts-0.2.2/src/docts/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:55.387328 docts-0.2.2/src/docts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/top_level.txt
```

### Comparing `docts-0.2.1/LICENSE` & `docts-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docts-0.2.1/PKG-INFO` & `docts-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docts
-Version: 0.2.1
+Version: 0.2.2
 Summary: python package docts
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/docts
 Project-URL: Homepage, https://github.com/foyoux/docts
 Project-URL: Bug Tracker, https://github.com/foyoux/docts/issues
 Keywords: docts
 Classifier: Programming Language :: Python
```

### Comparing `docts-0.2.1/README.md` & `docts-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `docts-0.2.1/pyproject.toml` & `docts-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docts-0.2.1/src/docts/__init__.py` & `docts-0.2.2/src/docts/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 __title__ = 'docts'
 __author__ = 'foyoux'
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 __description__ = 'document translate, read & translate & write'
 __url__ = 'https://github.com/foyoux/docts'
 __author_email__ = 'yimi.0822@qq.com'
 __license__ = 'GPL-3.0'
 __copyright__ = f'Copyright 2021-2023 {__author__}'
 __ide__ = 'PyCharm - https://www.jetbrains.com/pycharm/'
 
 import argparse
 import html
 import re
+from itertools import islice
 from typing import Callable, Pattern, AnyStr, List
 
 from pygtrans import Translate, Null
 
 # filter start
 
 UPPER_CHAR = re.compile(r'[A-Z]')
@@ -83,21 +84,24 @@
     words = [html.unescape(i) for i in set(origen_words) if i != '']
 
     print(f'过滤重复或空文本 parse_xlf: {len(origen_words) - len(words)}')
 
     return words
 
 
-def write_xlf(xlf_path: str, origins: List[str], client: Translate, trans: List[str] = None):
+def write_xlf(xlf_path: str, origins: List[str], client: Translate, trans: List[str] = None, limit=5000):
     # 翻译
     if trans is None:
-        trans = client.translate(origins)
-        if isinstance(trans, Null):
-            print(trans.msg)
-            raise
+        trans = []
+        for lst in [list(islice(origins, i, i + limit)) for i in range(0, len(origins), limit)]:
+            tl = client.translate(lst)
+            if isinstance(tl, Null):
+                print(tl.msg)
+                raise trans
+            trans.extend(tl)
         trans = [i.translatedText for i in trans]
 
     # 写入文件
     with open(xlf_path, 'w', encoding='utf-8', newline='') as f:
         f.write(
             '<?xml version="1.0" encoding="utf-8"?>\n'
             '<xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" '
@@ -122,19 +126,20 @@
             '  </file>\n'
             '</xliff>'
         )
 
 
 class Docts:
 
-    def __init__(self, xlf_path: str, client: Translate):
+    def __init__(self, xlf_path: str, client: Translate, limit: int = 5000):
         self.xlf_path = xlf_path
         self.words = parse_xlf(xlf_path)
         self.ignores = []
         self.client = client
+        self.limit = limit
 
     def add_filter(self, _filter: Callable[[str], bool]):
         """
         添加过滤器, 排除某些无需导出的内容
         :param _filter:
         :return:
         """
@@ -215,21 +220,21 @@
     def reset(self):
         self.words.extend(self.ignores)
         return self
 
     def save_words(self):
         """..."""
         xlf_path = self.xlf_path[:-4] + '_words.xlf'
-        write_xlf(xlf_path, self.words, self.client)
+        write_xlf(xlf_path, self.words, self.client, limit=self.limit)
         return xlf_path
 
     def save_ignores(self):
         """..."""
         xlf_path = self.xlf_path[:-4] + '_ignores.xlf'
-        write_xlf(xlf_path, self.ignores, self.client, self.ignores)
+        write_xlf(xlf_path, self.ignores, self.client, self.ignores, limit=self.limit)
         return xlf_path
 
 
 def main():
     epilog = f'%(prog)s({__version__}) by foyoux(https://github.com/foyoux/docts)'
     parser = argparse.ArgumentParser(prog='docts', description='', epilog=epilog)
     parser.add_argument('-v', '--version', action='version', version=epilog)
```

### Comparing `docts-0.2.1/src/docts.egg-info/PKG-INFO` & `docts-0.2.2/src/docts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docts
-Version: 0.2.1
+Version: 0.2.2
 Summary: python package docts
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/docts
 Project-URL: Homepage, https://github.com/foyoux/docts
 Project-URL: Bug Tracker, https://github.com/foyoux/docts/issues
 Keywords: docts
 Classifier: Programming Language :: Python
```


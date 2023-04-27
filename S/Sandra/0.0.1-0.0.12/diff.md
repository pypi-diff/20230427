# Comparing `tmp/Sandra-0.0.1.tar.gz` & `tmp/Sandra-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sandra-0.0.1.tar", last modified: Wed Apr 26 03:09:34 2023, max compression
+gzip compressed data, was "Sandra-0.0.12.tar", last modified: Thu Apr 27 18:54:42 2023, max compression
```

## Comparing `Sandra-0.0.1.tar` & `Sandra-0.0.12.tar`

### file list

```diff
@@ -1,22 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 03:09:34.139813 Sandra-0.0.1/
--rw-rw-rw-   0        0        0     1076 2023-04-26 02:58:51.000000 Sandra-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4281 2023-04-26 03:09:34.139813 Sandra-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3764 2023-04-26 02:54:24.000000 Sandra-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-04-26 01:25:34.000000 Sandra-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      692 2023-04-26 03:09:34.141813 Sandra-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 03:09:34.083445 Sandra-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 03:09:34.108764 Sandra-0.0.1/src/Sandra/
--rw-rw-rw-   0        0        0       85 2023-04-26 02:56:04.000000 Sandra-0.0.1/src/Sandra/__init__.py
--rw-rw-rw-   0        0        0      534 2023-04-26 02:46:00.000000 Sandra-0.0.1/src/Sandra/data.py
--rw-rw-rw-   0        0        0     2805 2023-04-26 02:55:03.000000 Sandra-0.0.1/src/Sandra/performance.py
--rw-rw-rw-   0        0        0     4965 2023-04-26 01:35:19.000000 Sandra-0.0.1/src/Sandra/sandra.py
--rw-rw-rw-   0        0        0     1332 2023-04-26 02:08:05.000000 Sandra-0.0.1/src/Sandra/troy.py
-drwxrwxrwx   0        0        0        0 2023-04-26 03:09:34.135788 Sandra-0.0.1/src/Sandra.egg-info/
--rw-rw-rw-   0        0        0     4281 2023-04-26 03:09:34.000000 Sandra-0.0.1/src/Sandra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-04-26 03:09:34.000000 Sandra-0.0.1/src/Sandra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 03:09:34.000000 Sandra-0.0.1/src/Sandra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-26 03:09:34.000000 Sandra-0.0.1/src/Sandra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-26 03:09:34.000000 Sandra-0.0.1/src/Sandra.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 03:09:34.138812 Sandra-0.0.1/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 02:09:29.000000 Sandra-0.0.1/src/tests/__init__.py
--rw-rw-rw-   0        0        0     4331 2023-04-26 02:55:44.000000 Sandra-0.0.1/src/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:54:42.325344 Sandra-0.0.12/
+-rw-rw-rw-   0        0        0     1080 2023-04-27 16:41:21.000000 Sandra-0.0.12/LICENSE
+-rw-rw-rw-   0        0        0     5128 2023-04-27 18:54:42.324328 Sandra-0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     4441 2023-04-27 18:29:34.000000 Sandra-0.0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 18:54:42.303330 Sandra-0.0.12/Sandra/
+-rw-rw-rw-   0        0        0      132 2023-04-27 18:12:46.000000 Sandra-0.0.12/Sandra/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-04-27 18:01:39.000000 Sandra-0.0.12/Sandra/helpers.py
+-rw-rw-rw-   0        0        0     2912 2023-04-27 16:34:16.000000 Sandra-0.0.12/Sandra/performance.py
+-rw-rw-rw-   0        0        0     4965 2023-04-26 01:35:19.000000 Sandra-0.0.12/Sandra/sandra.py
+-rw-rw-rw-   0        0        0     1332 2023-04-26 02:08:05.000000 Sandra-0.0.12/Sandra/troy.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:54:42.323341 Sandra-0.0.12/Sandra.egg-info/
+-rw-rw-rw-   0        0        0     5128 2023-04-27 18:54:42.000000 Sandra-0.0.12/Sandra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-04-27 18:54:42.000000 Sandra-0.0.12/Sandra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 18:54:42.000000 Sandra-0.0.12/Sandra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-27 18:54:42.000000 Sandra-0.0.12/Sandra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 18:54:42.000000 Sandra-0.0.12/Sandra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 18:54:42.325344 Sandra-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-04-27 18:54:21.000000 Sandra-0.0.12/setup.py
```

### Comparing `Sandra-0.0.1/LICENSE` & `Sandra-0.0.12/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
-Copyright (c) 2018 YOUR NAME
+Copyright (c) 2018 George Assaad
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 The above copyright notice and this permission notice shall be included in all
```

### Comparing `Sandra-0.0.1/src/Sandra/performance.py` & `Sandra-0.0.12/Sandra/performance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from Crypto.Cipher import AES 
 from . import sandra
+from . import troy
 
 import timeit
 import pandas as pd
 
-def performance_test():
-    with open('./txt/taylor_swift_1KB.txt', 'rb') as f:
-        taylor_swift_1KB = f.read()
-
-    with open('./txt/taylor_swift_5KB.txt', 'rb') as f:
-        taylor_swift_5KB = f.read()
-
-    with open('./txt/taylor_swift_10KB.txt', 'rb') as f:
-        taylor_swift_10KB = f.read()
-
-    with open('./txt/taylor_swift_100KB.txt', 'rb') as f:
-        taylor_swift_100KB = f.read()
-
-    files = {
-        'taylor_swift_1KB.txt'  : taylor_swift_1KB,
-        'taylor_swift_5KB.txt'  : taylor_swift_5KB,
-        'taylor_swift_10KB.txt' : taylor_swift_10KB,
-        'taylor_swift_100KB.txt': taylor_swift_100KB
-    }
+def performance_test(names, files_data):
+    # with open('./txt/taylor_swift_1KB.txt', 'rb') as f:
+    #     taylor_swift_1KB = f.read()
+
+    # with open('./txt/taylor_swift_5KB.txt', 'rb') as f:
+    #     taylor_swift_5KB = f.read()
+
+    # with open('./txt/taylor_swift_10KB.txt', 'rb') as f:
+    #     taylor_swift_10KB = f.read()
+
+    # with open('./txt/taylor_swift_100KB.txt', 'rb') as f:
+    #     taylor_swift_100KB = f.read()
+
+    # files = {
+    #     'taylor_swift_1KB.txt'  : taylor_swift_1KB,
+    #     'taylor_swift_5KB.txt'  : taylor_swift_5KB,
+    #     'taylor_swift_10KB.txt' : taylor_swift_10KB,
+    #     'taylor_swift_100KB.txt': taylor_swift_100KB
+    # }
+    files = dict(zip(names, files_data))
 
     iv   = bytes.fromhex('fffffe00000000000000000000000000')
     key  = bytes.fromhex('00000000000000000000000000000000')
 
     stats = dict()
 
     def run_n_times(mode_name, encryptor, decryptor, OPENPGP=0, n=100):
```

### Comparing `Sandra-0.0.1/src/Sandra/sandra.py` & `Sandra-0.0.12/Sandra/sandra.py`

 * *Files identical despite different names*

### Comparing `Sandra-0.0.1/src/Sandra/troy.py` & `Sandra-0.0.12/Sandra/troy.py`

 * *Files identical despite different names*


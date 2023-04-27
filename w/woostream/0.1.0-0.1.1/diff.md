# Comparing `tmp/woostream-0.1.0.tar.gz` & `tmp/woostream-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woostream-0.1.0.tar", max compression
+gzip compressed data, was "woostream-0.1.1.tar", max compression
```

## Comparing `woostream-0.1.0.tar` & `woostream-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-04-27 11:05:40.612337 woostream-0.1.0/README.md
--rw-r--r--   0        0        0      422 2023-04-27 12:12:07.502824 woostream-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5220 2023-04-27 12:47:15.718870 woostream-0.1.0/woostream/__main__.py
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 woostream-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-27 11:05:40.612337 woostream-0.1.1/README.md
+-rw-r--r--   0        0        0      422 2023-04-27 12:52:44.117116 woostream-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5272 2023-04-27 12:50:53.788982 woostream-0.1.1/woostream/__main__.py
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 woostream-0.1.1/PKG-INFO
```

### Comparing `woostream-0.1.0/woostream/__main__.py` & `woostream-0.1.1/woostream/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,16 @@
         required='--telegram-token' in sys.argv
     )
 
     parser.add_argument(
         '--debug-level',
         type=str,
         required=True,
-        choices=list(logging._nameToLevel.keys())
+        choices=list(logging._nameToLevel.keys()),
+        default=logging._levelToName[logging.INFO]
     )
 
     args = parser.parse_args()
 
     logging.basicConfig(
         level=logging._nameToLevel[args.debug_level]
     )
```

### Comparing `woostream-0.1.0/PKG-INFO` & `woostream-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woostream
-Version: 0.1.0
+Version: 0.1.1
 Summary: Listen to fills & position updates on Woo X
 License: MIT
 Author: waterquarks
 Author-email: waterquarks@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/xia_engine-0.8.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine-0.8.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 1258185 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1417 b- defN 23-Apr-26 17:48 xia_engine/__init__.py
--rw-r--r--  2.0 unx   460800 b- defN 23-Apr-26 17:53 xia_engine/acl.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   594432 b- defN 23-Apr-26 17:52 xia_engine/base.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   794112 b- defN 23-Apr-26 17:58 xia_engine/document.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   749056 b- defN 23-Apr-26 17:56 xia_engine/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   262144 b- defN 23-Apr-26 17:59 xia_engine/exception.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   462848 b- defN 23-Apr-26 17:54 xia_engine/fields.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-26 17:59 xia_engine-0.8.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      745 b- defN 23-Apr-26 17:59 xia_engine-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-26 17:59 xia_engine-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-26 17:59 xia_engine-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1052 b- defN 23-Apr-26 17:59 xia_engine-0.8.0.dist-info/RECORD
-12 files, 3326868 bytes uncompressed, 1256419 bytes compressed:  62.3%
+Zip file size: 1258857 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1417 b- defN 23-Apr-26 19:50 xia_engine/__init__.py
+-rw-r--r--  2.0 unx   460800 b- defN 23-Apr-26 19:56 xia_engine/acl.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   594432 b- defN 23-Apr-26 19:54 xia_engine/base.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   794112 b- defN 23-Apr-26 20:00 xia_engine/document.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   749056 b- defN 23-Apr-26 19:59 xia_engine/engine.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   262144 b- defN 23-Apr-26 20:01 xia_engine/exception.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   462848 b- defN 23-Apr-26 19:57 xia_engine/fields.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-26 20:01 xia_engine-0.8.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      745 b- defN 23-Apr-26 20:01 xia_engine-0.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-26 20:01 xia_engine-0.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-26 20:01 xia_engine-0.8.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1052 b- defN 23-Apr-26 20:01 xia_engine-0.8.1.dist-info/RECORD
+12 files, 3326868 bytes uncompressed, 1257091 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xia_engine/exception.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_engine/fields.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine-0.8.0.dist-info/LICENSE.txt
+Filename: xia_engine-0.8.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine-0.8.0.dist-info/METADATA
+Filename: xia_engine-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine-0.8.0.dist-info/WHEEL
+Filename: xia_engine-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine-0.8.0.dist-info/top_level.txt
+Filename: xia_engine-0.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine-0.8.0.dist-info/RECORD
+Filename: xia_engine-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine/__init__.py

```diff
@@ -20,8 +20,8 @@
     "MetaEngine", "MetaRamEngine", "MetaCache",
     "Acl", "AclItem",
     "XiaError", 'AuthorizationError', 'AuthenticationError', "OutOfScopeError",
     'NotFoundError', 'ConflictError', 'BadRequestError', "UnprocessableError",
     "ServerError"
 ]
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
```

## Comparing `xia_engine-0.8.0.dist-info/METADATA` & `xia_engine-0.8.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine
-Version: 0.8.0
+Version: 0.8.1
 Summary: X-I-A Engine
-Home-page: https://develop.x-i-a.com/docs/xia-engine/0.8.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine/0.8.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine-0.8.0.dist-info/RECORD` & `xia_engine-0.8.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_engine/__init__.py,sha256=mDgqCV2WxNJ2Z1hPjs5X95Xi7K_8n57HysxF28sajVM,1417
-xia_engine/acl.cp39-win_amd64.pyd,sha256=PrA4GB6WR1iVO5YU6AQarOVwLZlyz3XV0JoPLSa21XY,460800
-xia_engine/base.cp39-win_amd64.pyd,sha256=I1VvbXsnZVwVZ7UjCb_Dw4UxvUR6KQi6prgf2vOQA44,594432
-xia_engine/document.cp39-win_amd64.pyd,sha256=LydbeGpMhZDXWf4Jsxfr82rtKvbj12zw1nuvwWglFjI,794112
-xia_engine/engine.cp39-win_amd64.pyd,sha256=RRQE8mzy3LYjVTDRysPH8FZrjRoQcotl-5zFHzFFa-A,749056
-xia_engine/exception.cp39-win_amd64.pyd,sha256=YSa3vbf3bCUJUQyUf1t0mnaIvr3GslbOlEXYrU-_-dQ,262144
-xia_engine/fields.cp39-win_amd64.pyd,sha256=bHxEqY8dvRXEcrJE4beCHU6M1nEuu2cjgsgCBop8kJw,462848
-xia_engine-0.8.0.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_engine-0.8.0.dist-info/METADATA,sha256=81wxzFH14xXYLczKddYiwGTCRG_t2mSJLuMRUlHPm9s,745
-xia_engine-0.8.0.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine-0.8.0.dist-info/top_level.txt,sha256=Q896WUzHNHm14oiEaw7BbLcGbvHkKPKEQOBa8Z06dbk,11
-xia_engine-0.8.0.dist-info/RECORD,,
+xia_engine/__init__.py,sha256=LFIdKlzmT21QfHp2v4hl3Y7nBgMr6Pslyq29x3ZvIQk,1417
+xia_engine/acl.cp39-win_amd64.pyd,sha256=ibnq52PMnViNpm3ZgzV4MtOJy0ZCLnpWgmAzWJOAbWs,460800
+xia_engine/base.cp39-win_amd64.pyd,sha256=Ah18jmBThn5NFiajvXNtibmjbVeR_Qy1eiD7nf5qYgg,594432
+xia_engine/document.cp39-win_amd64.pyd,sha256=hiS5StaIF36eRY2vFz58ALHG_3QdTl-QXltJlVbKqpI,794112
+xia_engine/engine.cp39-win_amd64.pyd,sha256=WTUNCvmguEKUEL3ll4EIuGZ88KHxRNjGFwCXEzytdzw,749056
+xia_engine/exception.cp39-win_amd64.pyd,sha256=2PlpI8u0JBrHS4IYoyoTP4mdKpzG3fsNlguAeB9Uwm4,262144
+xia_engine/fields.cp39-win_amd64.pyd,sha256=EFQADOAlmJqC4YMf2iC_oODNEAq5J9fXV8pyyXptvmM,462848
+xia_engine-0.8.1.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine-0.8.1.dist-info/METADATA,sha256=g5UhTetK5qFSDy7nsIejOLo9liJWSCFK30Nz92adQxU,745
+xia_engine-0.8.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine-0.8.1.dist-info/top_level.txt,sha256=Q896WUzHNHm14oiEaw7BbLcGbvHkKPKEQOBa8Z06dbk,11
+xia_engine-0.8.1.dist-info/RECORD,,
```


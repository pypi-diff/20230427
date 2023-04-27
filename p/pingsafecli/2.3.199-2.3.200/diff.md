# Comparing `tmp/pingsafecli-2.3.199-py3-none-any.whl.zip` & `tmp/pingsafecli-2.3.200-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8543986 bytes, number of entries: 8
+Zip file size: 8543991 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 16:55 pingsafecli/__init__.py
 -rwxr-xr-x  2.0 unx 17012674 b- defN 23-Apr-26 15:50 pingsafecli/go-rego-evaluator
--rw-r--r--  2.0 unx     1556 b- defN 23-Apr-26 18:59 pingsafecli/main.py
--rwxr-xr-x  2.0 unx      541 b- defN 23-Apr-26 19:07 pingsafecli-2.3.199.data/scripts/pingsafecli
--rw-r--r--  2.0 unx      663 b- defN 23-Apr-26 19:07 pingsafecli-2.3.199.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 19:07 pingsafecli-2.3.199.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-26 19:07 pingsafecli-2.3.199.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      664 b- defN 23-Apr-26 19:07 pingsafecli-2.3.199.dist-info/RECORD
-8 files, 17016202 bytes uncompressed, 8542822 bytes compressed:  49.8%
+-rw-r--r--  2.0 unx     1559 b- defN 23-Apr-27 12:14 pingsafecli/main.py
+-rwxr-xr-x  2.0 unx      541 b- defN 23-Apr-27 12:17 pingsafecli-2.3.200.data/scripts/pingsafecli
+-rw-r--r--  2.0 unx      663 b- defN 23-Apr-27 12:17 pingsafecli-2.3.200.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 12:17 pingsafecli-2.3.200.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-27 12:17 pingsafecli-2.3.200.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      664 b- defN 23-Apr-27 12:17 pingsafecli-2.3.200.dist-info/RECORD
+8 files, 17016205 bytes uncompressed, 8542827 bytes compressed:  49.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pingsafecli/go-rego-evaluator
 Comment: 
 
 Filename: pingsafecli/main.py
 Comment: 
 
-Filename: pingsafecli-2.3.199.data/scripts/pingsafecli
+Filename: pingsafecli-2.3.200.data/scripts/pingsafecli
 Comment: 
 
-Filename: pingsafecli-2.3.199.dist-info/METADATA
+Filename: pingsafecli-2.3.200.dist-info/METADATA
 Comment: 
 
-Filename: pingsafecli-2.3.199.dist-info/WHEEL
+Filename: pingsafecli-2.3.200.dist-info/WHEEL
 Comment: 
 
-Filename: pingsafecli-2.3.199.dist-info/top_level.txt
+Filename: pingsafecli-2.3.200.dist-info/top_level.txt
 Comment: 
 
-Filename: pingsafecli-2.3.199.dist-info/RECORD
+Filename: pingsafecli-2.3.200.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingsafecli/main.py

```diff
@@ -37,12 +37,12 @@
                     os.remove(file_path)
 
 
 
 
 if __name__ == '__main__':
     ckv = PingSafeCli()
-    print ("world")
+    print ("world123")
     sys.exit(ckv.run("a", "b"))
```

## Comparing `pingsafecli-2.3.199.data/scripts/pingsafecli` & `pingsafecli-2.3.200.data/scripts/pingsafecli`

 * *Files identical despite different names*

## Comparing `pingsafecli-2.3.199.dist-info/METADATA` & `pingsafecli-2.3.200.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pingsafecli
-Version: 2.3.199
+Version: 2.3.200
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/checkov
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Classifier: Environment :: Console
 Requires-Python: >=3.7
```

## Comparing `pingsafecli-2.3.199.dist-info/RECORD` & `pingsafecli-2.3.200.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 pingsafecli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pingsafecli/go-rego-evaluator,sha256=wBM-aEJKmEwAGNRaKc9QRcdKjfkfP3N6weLp-FhFY30,17012674
-pingsafecli/main.py,sha256=sMFy4p_1KO-bYmBpZ4FDIUCemqjpsfCzeSnWT7no1ME,1556
-pingsafecli-2.3.199.data/scripts/pingsafecli,sha256=2G7hEyFP78TaQLTFeyhE_yUUcWkq8AYLMWkUIp67XdM,541
-pingsafecli-2.3.199.dist-info/METADATA,sha256=N0jtbd_2eSoD_IzNZuU_eTkEEc7wV7hNtqD1F-afP2E,663
-pingsafecli-2.3.199.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pingsafecli-2.3.199.dist-info/top_level.txt,sha256=jQGXsOZMG5Xz4cC5yzJshe1hA7wgKbautrUBk5s05Ok,12
-pingsafecli-2.3.199.dist-info/RECORD,,
+pingsafecli/main.py,sha256=jQcGzi9E7Ybb-QHqJbLNupHyRJPghPeHK2oMUaniEaU,1559
+pingsafecli-2.3.200.data/scripts/pingsafecli,sha256=2G7hEyFP78TaQLTFeyhE_yUUcWkq8AYLMWkUIp67XdM,541
+pingsafecli-2.3.200.dist-info/METADATA,sha256=4F5gJHXuqznqTYg9hf2fLhZJV6r-rWLu5PFJhU8V5_s,663
+pingsafecli-2.3.200.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pingsafecli-2.3.200.dist-info/top_level.txt,sha256=jQGXsOZMG5Xz4cC5yzJshe1hA7wgKbautrUBk5s05Ok,12
+pingsafecli-2.3.200.dist-info/RECORD,,
```


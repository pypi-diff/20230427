# Comparing `tmp/langpack-0.0.6-py2.py3-none-any.whl.zip` & `tmp/langpack-0.0.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 15164 bytes, number of entries: 12
+Zip file size: 15221 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 18:39 langpack/__init__.py
 -rw-rw-r--  2.0 unx      857 b- defN 23-Apr-21 03:47 langpack/app_template.py
 -rw-rw-r--  2.0 unx      611 b- defN 23-Apr-21 04:02 langpack/client_template.py
 -rw-rw-r--  2.0 unx     2787 b- defN 23-Apr-20 22:07 langpack/index.html
 -rw-rw-r--  2.0 unx     7528 b- defN 23-Apr-21 05:17 langpack/tester.py
 -rw-rw-r--  2.0 unx    26705 b- defN 23-Apr-26 20:45 langpack/tools.py
--rw-rw-r--  2.0 unx    10248 b- defN 23-Apr-26 22:27 langpack/utils.py
--rw-rw-r--  2.0 unx      905 b- defN 23-Apr-26 22:28 langpack-0.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-26 22:28 langpack-0.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx      200 b- defN 23-Apr-26 22:28 langpack-0.0.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-26 22:28 langpack-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      936 b- defN 23-Apr-26 22:28 langpack-0.0.6.dist-info/RECORD
-12 files, 50896 bytes uncompressed, 13600 bytes compressed:  73.3%
+-rw-rw-r--  2.0 unx    10435 b- defN 23-Apr-26 22:31 langpack/utils.py
+-rw-rw-r--  2.0 unx      905 b- defN 23-Apr-26 22:32 langpack-0.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-26 22:32 langpack-0.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      200 b- defN 23-Apr-26 22:32 langpack-0.0.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-26 22:32 langpack-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      936 b- defN 23-Apr-26 22:32 langpack-0.0.7.dist-info/RECORD
+12 files, 51083 bytes uncompressed, 13657 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: langpack/tools.py
 Comment: 
 
 Filename: langpack/utils.py
 Comment: 
 
-Filename: langpack-0.0.6.dist-info/METADATA
+Filename: langpack-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: langpack-0.0.6.dist-info/WHEEL
+Filename: langpack-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: langpack-0.0.6.dist-info/entry_points.txt
+Filename: langpack-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: langpack-0.0.6.dist-info/top_level.txt
+Filename: langpack-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: langpack-0.0.6.dist-info/RECORD
+Filename: langpack-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langpack/utils.py

```diff
@@ -290,14 +290,21 @@
         ssh_command,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         shell=True,
         text=True,
     )
 
+    while True:
+        output = process.stdout.readline()
+        if output == "" and process.poll() is not None:
+            break
+        if output:
+            print(output.strip())
+
 
 def zip_and_upload_to_s3(source_folder, destination_bucket, destination_key, region):
     # Create a new zip file
     zip_filename = source_folder + ".zip"
     with zipfile.ZipFile(zip_filename, "w", zipfile.ZIP_DEFLATED) as zip_file:
         # Add all files in the source folder to the zip file
         for root, dirs, files in os.walk(source_folder):
```

## Comparing `langpack-0.0.6.dist-info/METADATA` & `langpack-0.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langpack
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library to pakcage and deploy langugage model apps
 Home-page: UNKNOWN
 Author: Chuan Li
 Author-email: c@lambdalabs.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Dist: apify-client (==1.0.0)
```

## Comparing `langpack-0.0.6.dist-info/RECORD` & `langpack-0.0.7.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 langpack/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 langpack/app_template.py,sha256=Athx3xBnaw3twNdjtR_qbM37CRXj8-iL2e8CL0vjoaY,857
 langpack/client_template.py,sha256=76uiHaqX-YNpbl4yd62a-V1dXV5S0tcxbTXYOsGTQfI,611
 langpack/index.html,sha256=BQdpj0HZwhSfctr69ZeddzalBGHAp3WCb-LM6rkIzJM,2787
 langpack/tester.py,sha256=PoDgNQe_fis7y6ZsQOITTF6M1svBZ-Sp2cE5EqTRadU,7528
 langpack/tools.py,sha256=nni5vUGARmswRjcARWcfxAB3Kp3WnHSIsBw5S46QwI8,26705
-langpack/utils.py,sha256=15Y9qsKloub7QJ93ABznMaxDU8LzTj_sPNnkZLa_AVM,10248
-langpack-0.0.6.dist-info/METADATA,sha256=APm_qXY9ViXO3omfzp4OPszjod_6JRvkl49rLbYTriI,905
-langpack-0.0.6.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
-langpack-0.0.6.dist-info/entry_points.txt,sha256=75SUv2OYYKWRl1QtqkCrb1Kt0LbnrXOHG7Iy5e4E71M,200
-langpack-0.0.6.dist-info/top_level.txt,sha256=j92Fj-GurEfjdOLmRWAy5wdVGVoOFqkhz6grAYs19Yw,9
-langpack-0.0.6.dist-info/RECORD,,
+langpack/utils.py,sha256=_uyeINrf-iu3V_UQl3AUID9SpAxTZqCsfCF3iVbrt1s,10435
+langpack-0.0.7.dist-info/METADATA,sha256=INYdrmmciffYtC-xJLtCUuoPDZzGbphL4A9EHYbOVKo,905
+langpack-0.0.7.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
+langpack-0.0.7.dist-info/entry_points.txt,sha256=75SUv2OYYKWRl1QtqkCrb1Kt0LbnrXOHG7Iy5e4E71M,200
+langpack-0.0.7.dist-info/top_level.txt,sha256=j92Fj-GurEfjdOLmRWAy5wdVGVoOFqkhz6grAYs19Yw,9
+langpack-0.0.7.dist-info/RECORD,,
```


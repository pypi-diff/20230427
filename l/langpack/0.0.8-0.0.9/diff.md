# Comparing `tmp/langpack-0.0.8-py2.py3-none-any.whl.zip` & `tmp/langpack-0.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 15199 bytes, number of entries: 12
+Zip file size: 15208 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 18:39 langpack/__init__.py
 -rw-rw-r--  2.0 unx      857 b- defN 23-Apr-21 03:47 langpack/app_template.py
 -rw-rw-r--  2.0 unx      611 b- defN 23-Apr-21 04:02 langpack/client_template.py
 -rw-rw-r--  2.0 unx     2787 b- defN 23-Apr-20 22:07 langpack/index.html
 -rw-rw-r--  2.0 unx     7528 b- defN 23-Apr-21 05:17 langpack/tester.py
--rw-rw-r--  2.0 unx    26705 b- defN 23-Apr-26 20:45 langpack/tools.py
--rw-rw-r--  2.0 unx    10364 b- defN 23-Apr-26 23:30 langpack/utils.py
--rw-rw-r--  2.0 unx      905 b- defN 23-Apr-26 23:30 langpack-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-26 23:30 langpack-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx      200 b- defN 23-Apr-26 23:30 langpack-0.0.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-26 23:30 langpack-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      936 b- defN 23-Apr-26 23:30 langpack-0.0.8.dist-info/RECORD
-12 files, 51012 bytes uncompressed, 13635 bytes compressed:  73.3%
+-rw-rw-r--  2.0 unx    26730 b- defN 23-Apr-26 23:42 langpack/tools.py
+-rw-rw-r--  2.0 unx    10343 b- defN 23-Apr-26 23:42 langpack/utils.py
+-rw-rw-r--  2.0 unx      905 b- defN 23-Apr-26 23:43 langpack-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-26 23:43 langpack-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      200 b- defN 23-Apr-26 23:43 langpack-0.0.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-26 23:43 langpack-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      936 b- defN 23-Apr-26 23:43 langpack-0.0.9.dist-info/RECORD
+12 files, 51016 bytes uncompressed, 13644 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: langpack/tools.py
 Comment: 
 
 Filename: langpack/utils.py
 Comment: 
 
-Filename: langpack-0.0.8.dist-info/METADATA
+Filename: langpack-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: langpack-0.0.8.dist-info/WHEEL
+Filename: langpack-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: langpack-0.0.8.dist-info/entry_points.txt
+Filename: langpack-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: langpack-0.0.8.dist-info/top_level.txt
+Filename: langpack-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: langpack-0.0.8.dist-info/RECORD
+Filename: langpack-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langpack/tools.py

```diff
@@ -749,15 +749,15 @@
             run_docker_command(remote_ip, username, lambda_cloud_key, docker_command)
             app_path = "/home/ubuntu/app"
         else:
             # otherwise assuming the app is already downloaded on the
             app_path = args.app_path
 
         # Launch the app using docker
-        docker_command = f"sudo docker run --network host -v {app_path}:/app {env_str} -w /app chuanli11/langpack-ubuntu:22.04 python3 app.py"
+        docker_command = f"nohup sudo docker run --network host -v {app_path}:/app {env_str} -w /app chuanli11/langpack-ubuntu:22.04 python3 app.py > /dev/null 2>&1 &"
         print("-----------------------------------------------")
         print(docker_command)
         run_docker_command(remote_ip, username, lambda_cloud_key, docker_command)
 
         print(f"App launched at http://{remote_ip}:5000/predict")
 
     else:
```

## langpack/utils.py

```diff
@@ -291,15 +291,14 @@
             ssh_command,
             stdin=devnull,
             stdout=devnull,
             stderr=devnull,
             shell=True,
             start_new_session=True,
         )
-    process.detach()
 
 
 def zip_and_upload_to_s3(source_folder, destination_bucket, destination_key, region):
     # Create a new zip file
     zip_filename = source_folder + ".zip"
     with zipfile.ZipFile(zip_filename, "w", zipfile.ZIP_DEFLATED) as zip_file:
         # Add all files in the source folder to the zip file
```

## Comparing `langpack-0.0.8.dist-info/METADATA` & `langpack-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langpack
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library to pakcage and deploy langugage model apps
 Home-page: UNKNOWN
 Author: Chuan Li
 Author-email: c@lambdalabs.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Dist: apify-client (==1.0.0)
```


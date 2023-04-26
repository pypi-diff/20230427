# Comparing `tmp/langpack-0.0.5-py2.py3-none-any.whl.zip` & `tmp/langpack-0.0.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 15185 bytes, number of entries: 12
+Zip file size: 15164 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 18:39 langpack/__init__.py
 -rw-rw-r--  2.0 unx      857 b- defN 23-Apr-21 03:47 langpack/app_template.py
 -rw-rw-r--  2.0 unx      611 b- defN 23-Apr-21 04:02 langpack/client_template.py
 -rw-rw-r--  2.0 unx     2787 b- defN 23-Apr-20 22:07 langpack/index.html
 -rw-rw-r--  2.0 unx     7528 b- defN 23-Apr-21 05:17 langpack/tester.py
--rw-rw-r--  2.0 unx    26543 b- defN 23-Apr-26 20:32 langpack/tools.py
--rw-rw-r--  2.0 unx    10404 b- defN 23-Apr-26 18:27 langpack/utils.py
--rw-rw-r--  2.0 unx      905 b- defN 23-Apr-26 20:33 langpack-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-26 20:33 langpack-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx      200 b- defN 23-Apr-26 20:33 langpack-0.0.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-26 20:33 langpack-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      936 b- defN 23-Apr-26 20:33 langpack-0.0.5.dist-info/RECORD
-12 files, 50890 bytes uncompressed, 13621 bytes compressed:  73.2%
+-rw-rw-r--  2.0 unx    26705 b- defN 23-Apr-26 20:45 langpack/tools.py
+-rw-rw-r--  2.0 unx    10248 b- defN 23-Apr-26 22:27 langpack/utils.py
+-rw-rw-r--  2.0 unx      905 b- defN 23-Apr-26 22:28 langpack-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-26 22:28 langpack-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      200 b- defN 23-Apr-26 22:28 langpack-0.0.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-26 22:28 langpack-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      936 b- defN 23-Apr-26 22:28 langpack-0.0.6.dist-info/RECORD
+12 files, 50896 bytes uncompressed, 13600 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: langpack/tools.py
 Comment: 
 
 Filename: langpack/utils.py
 Comment: 
 
-Filename: langpack-0.0.5.dist-info/METADATA
+Filename: langpack-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: langpack-0.0.5.dist-info/WHEEL
+Filename: langpack-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: langpack-0.0.5.dist-info/entry_points.txt
+Filename: langpack-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: langpack-0.0.5.dist-info/top_level.txt
+Filename: langpack-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: langpack-0.0.5.dist-info/RECORD
+Filename: langpack-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langpack/tools.py

```diff
@@ -750,16 +750,20 @@
             app_path = "/home/ubuntu/app"
         else:
             # otherwise assuming the app is already downloaded on the
             app_path = args.app_path
 
         # Launch the app using docker
         docker_command = f"sudo docker run --network host -v {app_path}:/app {env_str} -w /app chuanli11/langpack-ubuntu:22.04 python3 app.py"
+        print("-----------------------------------------------")
+        print(docker_command)
         run_docker_command(remote_ip, username, lambda_cloud_key, docker_command)
 
+        print(f"App launched at http://{remote_ip}:5000/predict")
+
     else:
         raise f"Instance type {args.instance} is not supported"
 
 
 def download_app_from_s3():
     parser = argparse.ArgumentParser()
     parser.add_argument("s3_url", default="", help="S3 bucket URL for fetching the app")
```

## langpack/utils.py

```diff
@@ -282,25 +282,21 @@
         print(result.stderr.strip())
         raise f"{command} failed."
 
 
 def run_docker_command(hostname, username, lambda_cloud_key, command):
     ssh_command = f"ssh -i {lambda_cloud_key} {username}@{hostname} {command}"
 
-    with open(os.devnull, "w") as devnull:
-        result = subprocess.Popen(
-            ssh_command,
-            stdin=devnull,
-            stdout=devnull,
-            stderr=devnull,
-            shell=True,
-            start_new_session=True,
-        )
-
-    print(f"App launched at http://{hostname}:5000/predict")
+    process = subprocess.Popen(
+        ssh_command,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        shell=True,
+        text=True,
+    )
 
 
 def zip_and_upload_to_s3(source_folder, destination_bucket, destination_key, region):
     # Create a new zip file
     zip_filename = source_folder + ".zip"
     with zipfile.ZipFile(zip_filename, "w", zipfile.ZIP_DEFLATED) as zip_file:
         # Add all files in the source folder to the zip file
```

## Comparing `langpack-0.0.5.dist-info/METADATA` & `langpack-0.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langpack
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library to pakcage and deploy langugage model apps
 Home-page: UNKNOWN
 Author: Chuan Li
 Author-email: c@lambdalabs.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Dist: apify-client (==1.0.0)
```


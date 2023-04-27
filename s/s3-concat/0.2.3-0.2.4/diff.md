# Comparing `tmp/s3-concat-0.2.3.tar.gz` & `tmp/s3-concat-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3-concat-0.2.3.tar", last modified: Fri May 21 13:44:13 2021, max compression
+gzip compressed data, was "s3-concat-0.2.4.tar", last modified: Thu Apr 27 19:28:42 2023, max compression
```

## Comparing `s3-concat-0.2.3.tar` & `s3-concat-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-21 13:44:13.742378 s3-concat-0.2.3/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2020-10-03 01:16:20.000000 s3-concat-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3127 2021-05-21 13:44:13.742378 s3-concat-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2222 2020-10-03 01:16:20.000000 s3-concat-0.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-21 13:44:13.738378 s3-concat-0.2.3/s3_concat/
--rw-rw-rw-   0 root         (0) root         (0)     2403 2021-05-21 13:43:09.000000 s3-concat-0.2.3/s3_concat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1588 2020-10-03 01:16:20.000000 s3-concat-0.2.3/s3_concat/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     7467 2021-02-03 13:21:17.000000 s3-concat-0.2.3/s3_concat/multipart_upload_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2873 2021-05-21 13:43:09.000000 s3-concat-0.2.3/s3_concat/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-21 13:44:13.738378 s3-concat-0.2.3/s3_concat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3127 2021-05-21 13:44:13.000000 s3-concat-0.2.3/s3_concat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2021-05-21 13:44:13.000000 s3-concat-0.2.3/s3_concat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-21 13:44:13.000000 s3-concat-0.2.3/s3_concat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2021-05-21 13:44:13.000000 s3-concat-0.2.3/s3_concat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2021-05-21 13:44:13.000000 s3-concat-0.2.3/s3_concat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2021-05-21 13:44:13.000000 s3-concat-0.2.3/s3_concat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-05-21 13:44:13.742378 s3-concat-0.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      814 2021-05-21 13:41:06.000000 s3-concat-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:28:42.168610 s3-concat-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2020-10-03 01:16:20.000000 s3-concat-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-04-27 19:28:42.168610 s3-concat-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-04-27 19:26:56.000000 s3-concat-0.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:28:42.164610 s3-concat-0.2.4/s3_concat/
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-04-27 19:13:00.000000 s3-concat-0.2.4/s3_concat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2023-04-27 19:13:00.000000 s3-concat-0.2.4/s3_concat/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     7467 2023-04-27 18:46:29.000000 s3-concat-0.2.4/s3_concat/multipart_upload_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-04-27 19:13:00.000000 s3-concat-0.2.4/s3_concat/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:28:42.168610 s3-concat-0.2.4/s3_concat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-04-27 19:28:42.000000 s3-concat-0.2.4/s3_concat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-27 19:28:42.000000 s3-concat-0.2.4/s3_concat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:28:42.000000 s3-concat-0.2.4/s3_concat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-27 19:28:42.000000 s3-concat-0.2.4/s3_concat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-27 19:28:42.000000 s3-concat-0.2.4/s3_concat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-27 19:28:42.000000 s3-concat-0.2.4/s3_concat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 19:28:42.168610 s3-concat-0.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-04-27 18:46:29.000000 s3-concat-0.2.4/setup.py
```

### Comparing `s3-concat-0.2.3/LICENSE` & `s3-concat-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `s3-concat-0.2.3/PKG-INFO` & `s3-concat-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 Metadata-Version: 2.1
 Name: s3-concat
-Version: 0.2.3
+Version: 0.2.4
 Summary: Concat files in s3
 Home-page: https://github.com/xtream1101/s3-concat
 Author: Eddy Hintze
-Author-email: eddy@hintze.co
 License: MIT
-Description: # Python S3 Concat
-        
-        [![PyPI](https://img.shields.io/pypi/v/s3-concat.svg)](https://pypi.python.org/pypi/s3-concat)
-        [![PyPI](https://img.shields.io/pypi/l/s3-concat.svg)](https://pypi.python.org/pypi/s3-concat)  
-        
-        
-        S3 Concat is used to concatenate many small files in an s3 bucket into fewer larger files.
-        
-        
-        ## Install
-        `pip install s3-concat`
-        
-        
-        ## Usage
-        
-        ### Command Line
-        `$ s3-concat -h`
-        
-        ### Import
-        ```python
-        from s3_concat import S3Concat
-        
-        bucket = 'YOUR_BUCKET_NAME'
-        path_to_concat = 'PATH_TO_FILES_TO_CONCAT'
-        concatenated_file = 'FILE_TO_SAVE_TO.json'
-        # Setting this to a size will always add a part number at the end of the file name
-        min_file_size = '50MB'  # ex: FILE_TO_SAVE_TO-1.json, FILE_TO_SAVE_TO-2.json, ...
-        # Setting this to None will concat all files into a single file
-        # min_file_size = None  ex: FILE_TO_SAVE_TO.json
-        
-        # Init the job
-        job = S3Concat(bucket, concatenated_file, min_file_size,
-                       content_type='application/json',
-                      #  session=boto3.session.Session(),  # For custom aws session
-                      # s3_client_kwargs={}  # Use to pass arguments allowed by the s3 client: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html
-                       )
-        # Add files, can call multiple times to add files from other directories
-        job.add_files(path_to_concat)
-        # Add a single file at a time
-        job.add_file('some/file_key.json')
-        # Only use small_parts_threads if you need to. See Advanced Usage section below.
-        job.concat(small_parts_threads=4)
-        ```
-        
-        ## Advanced Usage
-        
-        Depending on your use case, you may want to use `small_parts_threads`.  
-        
-          - `small_parts_threads` is only used when the files you are trying to concat are less then 5MB. Due to the limitations of the s3 multipart_upload api (see *Limitations* below) any files less then 5MB need to be download locally, concated together, then re uploaded. By setting this thread count it will download the parts in parallel for faster creation of the concatination process.  
-        
-        The values set for these arguments depends on your use case and the system you are running this on.
-        
-        
-        ## Limitations
-        This uses the multipart upload of s3 and its limits are https://docs.aws.amazon.com/AmazonS3/latest/dev/qfacts.html
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python S3 Concat
+
+[![PyPI](https://img.shields.io/pypi/v/s3-concat.svg)](https://pypi.python.org/pypi/s3-concat)
+[![PyPI](https://img.shields.io/pypi/l/s3-concat.svg)](https://pypi.python.org/pypi/s3-concat)  
+
+
+S3 Concat is used to concatenate many small files in an s3 bucket into fewer larger files.
+
+
+## Install
+`pip install s3-concat`
+
+
+## Usage
+
+### Command Line
+`$ s3-concat -h`
+
+### Import
+```python
+from s3_concat import S3Concat
+
+bucket = 'YOUR_BUCKET_NAME'
+path_to_concat = 'PATH_TO_FILES_TO_CONCAT'
+concatenated_file = 'FILE_TO_SAVE_TO.json'
+# Setting this to a size will always add a part number at the end of the file name
+min_file_size = '50MB'  # ex: FILE_TO_SAVE_TO-1.json, FILE_TO_SAVE_TO-2.json, ...
+# Setting this to None will concat all files into a single file
+# min_file_size = None  ex: FILE_TO_SAVE_TO.json
+
+# Init the job
+job = S3Concat(bucket, concatenated_file, min_file_size,
+               content_type='application/json',
+              #  session=boto3.session.Session(),  # For custom aws session
+              # s3_client_kwargs={}  # Use to pass arguments allowed by the s3 client: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html
+               )
+# Add files, can call multiple times to add files from other directories
+job.add_files(path_to_concat)
+# Add a single file at a time
+job.add_file('some/file_key.json')
+# Only use small_parts_threads if you need to. See Advanced Usage section below.
+job.concat(small_parts_threads=4, main_threads=2)
+```
+
+## Advanced Usage
+
+Depending on your use case, you may want to use more threads then just 1.  
+
+  - `main_threads` is the number of threads to use when uploading files to s3. This will help when there are a lot of files that are already over the `min_file_size` that is set
+
+  - `small_parts_threads` is only used when the files you are trying to concat are less then 5MB. These are spawned from _inside_ of the `main_threads`. Due to the limitations of the s3 multipart_upload api (see *Limitations* below) any files less then 5MB need to be downloaded locally, concated together, then re uploaded. By setting this thread count it will download the parts in parallel for faster creation of the concatenation process.  
+
+The values set for these arguments depends on your use case and the system you are running this on.
+
+
+## Limitations
+This uses the multipart upload of s3 and its limits are https://docs.aws.amazon.com/AmazonS3/latest/dev/qfacts.html
+
+
```

### Comparing `s3-concat-0.2.3/README.md` & `s3-concat-0.2.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,21 +35,23 @@
               # s3_client_kwargs={}  # Use to pass arguments allowed by the s3 client: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html
                )
 # Add files, can call multiple times to add files from other directories
 job.add_files(path_to_concat)
 # Add a single file at a time
 job.add_file('some/file_key.json')
 # Only use small_parts_threads if you need to. See Advanced Usage section below.
-job.concat(small_parts_threads=4)
+job.concat(small_parts_threads=4, main_threads=2)
 ```
 
 ## Advanced Usage
 
-Depending on your use case, you may want to use `small_parts_threads`.  
+Depending on your use case, you may want to use more threads then just 1.  
 
-  - `small_parts_threads` is only used when the files you are trying to concat are less then 5MB. Due to the limitations of the s3 multipart_upload api (see *Limitations* below) any files less then 5MB need to be download locally, concated together, then re uploaded. By setting this thread count it will download the parts in parallel for faster creation of the concatination process.  
+  - `main_threads` is the number of threads to use when uploading files to s3. This will help when there are a lot of files that are already over the `min_file_size` that is set
+
+  - `small_parts_threads` is only used when the files you are trying to concat are less then 5MB. These are spawned from _inside_ of the `main_threads`. Due to the limitations of the s3 multipart_upload api (see *Limitations* below) any files less then 5MB need to be downloaded locally, concated together, then re uploaded. By setting this thread count it will download the parts in parallel for faster creation of the concatenation process.  
 
 The values set for these arguments depends on your use case and the system you are running this on.
 
 
 ## Limitations
 This uses the multipart upload of s3 and its limits are https://docs.aws.amazon.com/AmazonS3/latest/dev/qfacts.html
```

### Comparing `s3-concat-0.2.3/s3_concat/__init__.py` & `s3-concat-0.2.4/s3_concat/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import boto3
 import logging
 
-from .utils import _create_s3_client, _convert_to_bytes, _chunk_by_size
+from .utils import (
+    _create_s3_client,
+    _convert_to_bytes,
+    _chunk_by_size,
+    _threads
+)
 from .multipart_upload_job import MultipartUploadJob
 
 logger = logging.getLogger(__name__)
 
 
 class S3Concat:
 
@@ -17,33 +22,33 @@
         self.bucket = bucket
         self.key = key
         self.min_file_size = _convert_to_bytes(min_file_size)
         self.content_type = content_type
         self.all_files = []
         self.s3 = s3_client or _create_s3_client(session, s3_client_kwargs=s3_client_kwargs)  # noqa: E501
 
-    def concat(self, small_parts_threads=1):
+    def concat(self, small_parts_threads=1, main_threads=1):
 
         grouped_parts_list = _chunk_by_size(self.all_files, self.min_file_size)
         logger.info("Created {} concatenation groups"
                     .format(len(grouped_parts_list)))
 
-        part_keys = []
-        for part_data in grouped_parts_list:
+        def process_uploads(part_data):
             upload_resp = MultipartUploadJob(
                 self.bucket,
                 self.key,
                 part_data,
                 self.s3,
                 small_parts_threads=small_parts_threads,
                 add_part_number=self.min_file_size is not None,
                 content_type=self.content_type,
             )
-            part_keys.append(upload_resp.result_filepath)
+            return upload_resp.result_filepath
 
+        part_keys = _threads(main_threads, grouped_parts_list, process_uploads)
         return part_keys
 
     def add_files(self, prefix):
 
         def resp_to_filelist(resp):
             return [(x['Key'], x['Size']) for x in resp['Contents']]
```

### Comparing `s3-concat-0.2.3/s3_concat/cli.py` & `s3-concat-0.2.4/s3_concat/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,25 @@
                         )
     parser.add_argument("--filesize",
                         help=("Use to create multiple files if needed."
                               " Min filesize of the concatenated files"
                               " in [B,KB,MB,GB,TB]. e.x. 5.2GB"),
                         default=None,
                         )
+    parser.add_argument("--main-threads",
+                        type=int,
+                        help=("[Advanced Usage] Number of threads to"
+                              " use for the s3 uploading. (Default: 1)"),
+                        default=1)
     parser.add_argument("--small-parts-threads",
                         type=int,
                         help=("[Advanced Usage] Number of threads to"
                               " download small parts with. (Default: 1)"),
                         default=1)
     args = parser.parse_args()
 
     job = S3Concat(args.bucket, args.output, args.filesize)
     job.add_files(args.folder)
-    job.concat(small_parts_threads=args.small_parts_threads)
+    job.concat(
+        small_parts_threads=args.small_parts_threads,
+        main_threads=args.main_threads
+    )
```

### Comparing `s3-concat-0.2.3/s3_concat/multipart_upload_job.py` & `s3-concat-0.2.4/s3_concat/multipart_upload_job.py`

 * *Files identical despite different names*

### Comparing `s3-concat-0.2.3/s3_concat/utils.py` & `s3-concat-0.2.4/s3_concat/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,23 +57,33 @@
         list -- Each list of files is the min file size
     """
     grouped_list = []
     current_list = []
     current_size = 0
     current_index = 1
     for p in file_list:
+        if min_file_size is not None:
+            # If the current file is already larger then the min file size,
+            # just add it to the list on its own
+            if p[1] > min_file_size:
+                grouped_list.append((current_index, [p]))
+                current_index += 1
+                continue
+
+            # If multiple files have hit the min size, add them to the list
+            if current_size > min_file_size:
+                grouped_list.append((current_index, current_list))
+                current_list = []
+                current_size = 0
+                current_index += 1
+
         current_size += p[1]
         current_list.append(p)
-        if min_file_size is not None and current_size > min_file_size:
-            grouped_list.append((current_index, current_list))
-            current_list = []
-            current_size = 0
-            current_index += 1
 
-    # Get anything left over
+    # Get anything left over that did not add up to the min size
     if current_size != 0:
         grouped_list.append((current_index, current_list))
 
     return grouped_list
 
 
 def _convert_to_bytes(value):
```

### Comparing `s3-concat-0.2.3/s3_concat.egg-info/PKG-INFO` & `s3-concat-0.2.4/s3_concat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 Metadata-Version: 2.1
 Name: s3-concat
-Version: 0.2.3
+Version: 0.2.4
 Summary: Concat files in s3
 Home-page: https://github.com/xtream1101/s3-concat
 Author: Eddy Hintze
-Author-email: eddy@hintze.co
 License: MIT
-Description: # Python S3 Concat
-        
-        [![PyPI](https://img.shields.io/pypi/v/s3-concat.svg)](https://pypi.python.org/pypi/s3-concat)
-        [![PyPI](https://img.shields.io/pypi/l/s3-concat.svg)](https://pypi.python.org/pypi/s3-concat)  
-        
-        
-        S3 Concat is used to concatenate many small files in an s3 bucket into fewer larger files.
-        
-        
-        ## Install
-        `pip install s3-concat`
-        
-        
-        ## Usage
-        
-        ### Command Line
-        `$ s3-concat -h`
-        
-        ### Import
-        ```python
-        from s3_concat import S3Concat
-        
-        bucket = 'YOUR_BUCKET_NAME'
-        path_to_concat = 'PATH_TO_FILES_TO_CONCAT'
-        concatenated_file = 'FILE_TO_SAVE_TO.json'
-        # Setting this to a size will always add a part number at the end of the file name
-        min_file_size = '50MB'  # ex: FILE_TO_SAVE_TO-1.json, FILE_TO_SAVE_TO-2.json, ...
-        # Setting this to None will concat all files into a single file
-        # min_file_size = None  ex: FILE_TO_SAVE_TO.json
-        
-        # Init the job
-        job = S3Concat(bucket, concatenated_file, min_file_size,
-                       content_type='application/json',
-                      #  session=boto3.session.Session(),  # For custom aws session
-                      # s3_client_kwargs={}  # Use to pass arguments allowed by the s3 client: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html
-                       )
-        # Add files, can call multiple times to add files from other directories
-        job.add_files(path_to_concat)
-        # Add a single file at a time
-        job.add_file('some/file_key.json')
-        # Only use small_parts_threads if you need to. See Advanced Usage section below.
-        job.concat(small_parts_threads=4)
-        ```
-        
-        ## Advanced Usage
-        
-        Depending on your use case, you may want to use `small_parts_threads`.  
-        
-          - `small_parts_threads` is only used when the files you are trying to concat are less then 5MB. Due to the limitations of the s3 multipart_upload api (see *Limitations* below) any files less then 5MB need to be download locally, concated together, then re uploaded. By setting this thread count it will download the parts in parallel for faster creation of the concatination process.  
-        
-        The values set for these arguments depends on your use case and the system you are running this on.
-        
-        
-        ## Limitations
-        This uses the multipart upload of s3 and its limits are https://docs.aws.amazon.com/AmazonS3/latest/dev/qfacts.html
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python S3 Concat
+
+[![PyPI](https://img.shields.io/pypi/v/s3-concat.svg)](https://pypi.python.org/pypi/s3-concat)
+[![PyPI](https://img.shields.io/pypi/l/s3-concat.svg)](https://pypi.python.org/pypi/s3-concat)  
+
+
+S3 Concat is used to concatenate many small files in an s3 bucket into fewer larger files.
+
+
+## Install
+`pip install s3-concat`
+
+
+## Usage
+
+### Command Line
+`$ s3-concat -h`
+
+### Import
+```python
+from s3_concat import S3Concat
+
+bucket = 'YOUR_BUCKET_NAME'
+path_to_concat = 'PATH_TO_FILES_TO_CONCAT'
+concatenated_file = 'FILE_TO_SAVE_TO.json'
+# Setting this to a size will always add a part number at the end of the file name
+min_file_size = '50MB'  # ex: FILE_TO_SAVE_TO-1.json, FILE_TO_SAVE_TO-2.json, ...
+# Setting this to None will concat all files into a single file
+# min_file_size = None  ex: FILE_TO_SAVE_TO.json
+
+# Init the job
+job = S3Concat(bucket, concatenated_file, min_file_size,
+               content_type='application/json',
+              #  session=boto3.session.Session(),  # For custom aws session
+              # s3_client_kwargs={}  # Use to pass arguments allowed by the s3 client: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html
+               )
+# Add files, can call multiple times to add files from other directories
+job.add_files(path_to_concat)
+# Add a single file at a time
+job.add_file('some/file_key.json')
+# Only use small_parts_threads if you need to. See Advanced Usage section below.
+job.concat(small_parts_threads=4, main_threads=2)
+```
+
+## Advanced Usage
+
+Depending on your use case, you may want to use more threads then just 1.  
+
+  - `main_threads` is the number of threads to use when uploading files to s3. This will help when there are a lot of files that are already over the `min_file_size` that is set
+
+  - `small_parts_threads` is only used when the files you are trying to concat are less then 5MB. These are spawned from _inside_ of the `main_threads`. Due to the limitations of the s3 multipart_upload api (see *Limitations* below) any files less then 5MB need to be downloaded locally, concated together, then re uploaded. By setting this thread count it will download the parts in parallel for faster creation of the concatenation process.  
+
+The values set for these arguments depends on your use case and the system you are running this on.
+
+
+## Limitations
+This uses the multipart upload of s3 and its limits are https://docs.aws.amazon.com/AmazonS3/latest/dev/qfacts.html
+
+
```

### Comparing `s3-concat-0.2.3/setup.py` & `s3-concat-0.2.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='s3-concat',
     packages=['s3_concat'],
-    version='0.2.3',
+    version='0.2.4',
     description='Concat files in s3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Eddy Hintze',
-    author_email="eddy@hintze.co",
     url="https://github.com/xtream1101/s3-concat",
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
```


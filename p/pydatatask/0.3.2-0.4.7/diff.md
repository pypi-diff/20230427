# Comparing `tmp/pydatatask-0.3.2.tar.gz` & `tmp/pydatatask-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydatatask-0.3.2.tar", last modified: Fri Mar 31 07:39:46 2023, max compression
+gzip compressed data, was "pydatatask-0.4.7.tar", last modified: Thu Apr 27 18:13:32 2023, max compression
```

## Comparing `pydatatask-0.3.2.tar` & `pydatatask-0.4.7.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:39:46.276839 pydatatask-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-31 07:39:36.000000 pydatatask-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-31 07:39:36.000000 pydatatask-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-31 07:39:46.276839 pydatatask-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-31 07:39:36.000000 pydatatask-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:39:46.272838 pydatatask-0.3.2/pydatatask/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-31 07:39:38.000000 pydatatask-0.3.2/pydatatask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pydatatask/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pydatatask/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pydatatask/pod_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pydatatask/proc_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pydatatask/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38219 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pydatatask/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pydatatask/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pydatatask/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    45295 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pydatatask/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pydatatask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:39:46.272838 pydatatask-0.3.2/pydatatask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-31 07:39:46.000000 pydatatask-0.3.2/pydatatask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-31 07:39:46.000000 pydatatask-0.3.2/pydatatask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 07:39:46.000000 pydatatask-0.3.2/pydatatask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 07:39:46.000000 pydatatask-0.3.2/pydatatask.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-31 07:39:46.000000 pydatatask-0.3.2/pydatatask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-31 07:39:46.000000 pydatatask-0.3.2/pydatatask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-03-31 07:39:36.000000 pydatatask-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 07:39:46.276839 pydatatask-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:39:46.276839 pydatatask-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-31 07:39:36.000000 pydatatask-0.3.2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-03-31 07:39:36.000000 pydatatask-0.3.2/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-31 07:39:36.000000 pydatatask-0.3.2/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-31 07:39:36.000000 pydatatask-0.3.2/tests/test_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-03-31 07:39:36.000000 pydatatask-0.3.2/tests/test_kube.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-03-31 07:39:36.000000 pydatatask-0.3.2/tests/test_minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-03-31 07:39:36.000000 pydatatask-0.3.2/tests/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-03-31 07:39:36.000000 pydatatask-0.3.2/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-31 07:39:36.000000 pydatatask-0.3.2/tests/test_related.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-31 07:39:36.000000 pydatatask-0.3.2/tests/test_repo_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:13:32.630795 pydatatask-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-27 18:13:19.000000 pydatatask-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 18:13:19.000000 pydatatask-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-27 18:13:32.630795 pydatatask-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-27 18:13:19.000000 pydatatask-0.4.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:13:32.630795 pydatatask-0.4.7/pydatatask/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-27 18:13:24.000000 pydatatask-0.4.7/pydatatask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/pod_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/proc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39077 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45791 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pydatatask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:13:32.630795 pydatatask-0.4.7/pydatatask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-27 18:13:32.000000 pydatatask-0.4.7/pydatatask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-27 18:13:32.000000 pydatatask-0.4.7/pydatatask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:13:32.000000 pydatatask-0.4.7/pydatatask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:13:32.000000 pydatatask-0.4.7/pydatatask.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 18:13:32.000000 pydatatask-0.4.7/pydatatask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 18:13:32.000000 pydatatask-0.4.7/pydatatask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-27 18:13:19.000000 pydatatask-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:13:32.630795 pydatatask-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:13:19.000000 pydatatask-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:13:32.630795 pydatatask-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-27 18:13:19.000000 pydatatask-0.4.7/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-27 18:13:19.000000 pydatatask-0.4.7/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-27 18:13:19.000000 pydatatask-0.4.7/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-27 18:13:19.000000 pydatatask-0.4.7/tests/test_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-04-27 18:13:19.000000 pydatatask-0.4.7/tests/test_kube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-27 18:13:19.000000 pydatatask-0.4.7/tests/test_minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-27 18:13:19.000000 pydatatask-0.4.7/tests/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-27 18:13:19.000000 pydatatask-0.4.7/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-27 18:13:19.000000 pydatatask-0.4.7/tests/test_related.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-27 18:13:19.000000 pydatatask-0.4.7/tests/test_repo_base.py
```

### Comparing `pydatatask-0.3.2/LICENSE` & `pydatatask-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatatask-0.3.2/PKG-INFO` & `pydatatask-0.4.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatatask
-Version: 0.3.2
+Version: 0.4.7
 Summary: Library for constructing data-centric processing pipelines with few invariants
 Author-email: Audrey Dutcher <audrey@rhelmot.io>
 License: Copyright 2022 Audrey Dutcher
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -12,13 +12,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: repository, https://github.com/rhelmot/pydatatask
 Project-URL: documentation, https://pydatatask.readthedocs.io/
 Keywords: pipeline,data,task,repository,processing,async,kubernetes,s3,mongodb,docker,ssh
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: fuse
 Provides-Extra: dev
 Provides-Extra: type
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 License-File: LICENSE
```

### Comparing `pydatatask-0.3.2/README.rst` & `pydatatask-0.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `pydatatask-0.3.2/pydatatask/main.py` & `pydatatask-0.4.7/pydatatask/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,28 +22,34 @@
         launch              Manually start a task
         shell               Launch an interactive shell to interrogate the pipeline
 
     options:
       -h, --help            show this help message and exit
 """
 
-from typing import Callable, Dict, Iterable, List, Optional, Set, Union
+from typing import Awaitable, Callable, Dict, Iterable, List, Optional, Set, Union
 import argparse
 import asyncio
 import logging
 import re
 import sys
 
 import IPython
 import yaml
 
 from .pipeline import Pipeline
 from .repository import BlobRepository, MetadataRepository, Repository
 from .task import Link, Task
 
+fuse: Optional[Callable[[Pipeline, str, bool], Awaitable[None]]]
+try:
+    from .fuse import main as fuse
+except ModuleNotFoundError:
+    fuse = None
+
 log = logging.getLogger(__name__)
 token_re = re.compile(r"\w+\.\w+")
 
 __all__ = (
     "main",
     "update",
     "cat_data",
@@ -149,14 +155,20 @@
         help="Store metadata related to task completion",
     )
     parser_launch.set_defaults(func=launch)
 
     parser_shell = subparsers.add_parser("shell", help="Launch an interactive shell to interrogate the pipeline")
     parser_shell.set_defaults(func=shell)
 
+    if fuse is not None:
+        parser_fuse = subparsers.add_parser("fuse", help="Mount a fuse filesystem to explore the pipeline's repos")
+        parser_fuse.set_defaults(func=fuse)
+        parser_fuse.add_argument("path", help="The mountpoint")
+        parser_fuse.add_argument("--verbose", "-v", dest="debug", action="store_true", help="Show FUSE debug logging")
+
     if instrument is not None:
         instrument(subparsers)
 
     args = parser.parse_args()
     ns = vars(args)
     func = ns.pop("func")
     result_or_coro = func(pipeline, **ns)
```

### Comparing `pydatatask-0.3.2/pydatatask/pod_manager.py` & `pydatatask-0.4.7/pydatatask/pod_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
             self._api_ws = None
 
     async def launch(self, job, task, manifest):
         """
         Create a pod with the given manifest, named and labeled for this podman's app and the given job and task.
         """
         assert manifest["kind"] == "Pod"
+        task = task.replace("_", "-")
 
         manifest["metadata"] = manifest.get("metadata", {})
         manifest["metadata"].update(
             {
                 "name": "%s-%s-%s" % (self.app, job, task),
                 "labels": {
                     "app": self.app,
@@ -120,15 +121,15 @@
         """
         Return a list of pods labeled for this podman's app and (optional) the given job and task.
         """
         selectors = ["app=" + self.app]
         if job is not None:
             selectors.append("job=" + job)
         if task is not None:
-            selectors.append("task=" + task)
+            selectors.append("task=" + task.replace("_", "-"))
         selector = ",".join(selectors)
         return (await self.v1.list_namespaced_pod(self.namespace, label_selector=selector)).items
 
     async def delete(self, pod: V1Pod):
         """
         Destroy the given pod.
         """
```

### Comparing `pydatatask-0.3.2/pydatatask/proc_manager.py` & `pydatatask-0.4.7/pydatatask/proc_manager.py`

 * *Files identical despite different names*

### Comparing `pydatatask-0.3.2/pydatatask/repository.py` & `pydatatask-0.4.7/pydatatask/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,14 +337,16 @@
 class FileRepository(FileRepositoryBase, BlobRepository):
     """
     A file repository whose members are files, treated as streamable blobs.
     """
 
     @job_getter
     async def open(self, job, mode="r"):
+        if not self.is_valid_job_id(job):
+            raise KeyError(job)
         return aiofiles.open(self.fullpath(job), mode)
 
     async def delete(self, job):
         try:
             await aiofiles.os.unlink(self.fullpath(job))
         except FileNotFoundError:
             pass
@@ -464,19 +466,25 @@
 class S3BucketInfo:
     """
     The data structure returned from :meth:`S3BucketRepository.info`.
 
     :ivar uri: The s3 URI of the current job's resource, e.g. ``s3://bucket/prefix/job.ext``. ``str(info)`` will also
                return this.
     :ivar endpoint: The URL of the API server providing the S3 interface.
+    :ivar bucket: The name of the bucket objects are stored in.
+    :ivar prefix: How to prefix an object name such that it will fit into this repository.
+    :ivar suffix: How to suffix an object name such that it will fit into this repository.
     """
 
-    def __init__(self, endpoint: str, uri: str):
+    def __init__(self, endpoint: str, uri: str, bucket: str, prefix: str, suffix: str):
         self.endpoint = endpoint
         self.uri = uri
+        self.prefix = prefix
+        self.suffix = suffix
+        self.bucket = bucket
 
     def __str__(self):
         return self.uri
 
 
 class S3BucketRepository(BlobRepository):
     """
@@ -484,79 +492,81 @@
     """
 
     def __init__(
         self,
         client: Callable[[], S3Client],
         bucket: str,
         prefix: str = "",
-        extension: str = "",
+        suffix: str = "",
         mimetype: str = "application/octet-stream",
         incluster_endpoint: Optional[str] = None,
     ):
         """
         :param client: A callable returning an aiobotocore S3 client connected and authenticated to the server you wish
                        to store things on.
         :param bucket: The name of the bucket from which to load and store.
         :param prefix: A prefix to put on the job name before translating it into a bucket path. If this is meant to be
                        a directory name it should end with a slash character.
-        :param extension: A suffix to put on the job name before translating it into a bucket path. If this is meant to
+        :param suffix: A suffix to put on the job name before translating it into a bucket path. If this is meant to
                           be a file extension it should start with a dot.
         :param mimetype: The MIME type to set the content when adding data.
         :param incluster_endpoint: Optional: An endpoint URL to provide as the result of info() queries instead of
                                    extracting the URL from ``client``.
         """
         self._client = client
         self.bucket = bucket
         self.prefix = prefix
-        self.extension = extension
+        self.suffix = suffix
         self.mimetype = mimetype
         self.incluster_endpoint = incluster_endpoint
 
     @property
     def client(self):
         """
         The aiobotocore S3 client. This will raise an error if the client comes from a session which is not opened.
         """
         return self._client()
 
     def __repr__(self):
-        return f"<{type(self).__name__} {self.bucket}/{self.prefix}*{self.extension}>"
+        return f"<{type(self).__name__} {self.bucket}/{self.prefix}*{self.suffix}>"
 
     async def contains(self, item):
         try:
             await self.client.head_object(Bucket=self.bucket, Key=self.object_name(item))
         except botocore.exceptions.ClientError:
             return False
         else:
             return True
 
     async def unfiltered_iter(self):
         paginator = self.client.get_paginator("list_objects")
         async for page in paginator.paginate(Bucket=self.bucket, Prefix=self.prefix):
             for obj in page.get("Contents", []):
-                if obj["Key"].endswith(self.extension):
-                    yield obj["Key"][len(self.prefix) : -len(self.extension) if self.extension else None]
+                if obj["Key"].endswith(self.suffix):
+                    yield obj["Key"][len(self.prefix) : -len(self.suffix) if self.suffix else None]
 
     async def validate(self):
         try:
             await self.client.head_bucket(Bucket=self.bucket)
         except botocore.exceptions.ClientError as e:
             if "404" in str(e):
                 await self.client.create_bucket(Bucket=self.bucket)
             else:
                 raise
 
     def object_name(self, job):
         """
         Return the object name for the given job.
         """
-        return f"{self.prefix}{job}{self.extension}"
+        return f"{self.prefix}{job}{self.suffix}"
 
     @job_getter
     async def open(self, job, mode="r"):
+        if not self.is_valid_job_id(job):
+            raise KeyError(job)
         if mode == "wb":
             return S3BucketBinaryWriter(self, job)
         elif mode == "w":
             return AWriteText(S3BucketBinaryWriter(self, job))
         elif mode == "rb":
             return S3BucketReader((await self.client.get_object(Bucket=self.bucket, Key=self.object_name(job)))["Body"])
         elif mode == "r":
@@ -570,14 +580,17 @@
     async def info(self, job):
         """
         Return an `S3BucketInfo` corresponding to the given job.
         """
         return S3BucketInfo(
             self.incluster_endpoint or self.client._endpoint.host,
             f"s3://{self.bucket}/{self.object_name(job)}",
+            self.bucket,
+            self.prefix,
+            self.suffix,
         )
 
     async def delete(self, job):
         await self.client.delete_object(Bucket=self.bucket, Key=self.object_name(job))
 
 
 class MongoMetadataRepository(MetadataRepository):
@@ -631,14 +644,16 @@
         return result
 
     async def info_all(self) -> Dict[str, Any]:
         return {entry["_id"]: entry async for entry in self.collection.find({})}
 
     @job_getter
     async def dump(self, job, data):
+        if not self.is_valid_job_id(job):
+            raise KeyError(job)
         await self.collection.replace_one({"_id": job}, data, upsert=True)
 
 
 class DockerRepository(Repository):
     """
     A docker repository is, well, an actual docker repository hosted in some registry somewhere. Keys translate to tags
     on this repository.
@@ -708,16 +723,16 @@
         if self.registry.ssl:
             username, password = base64.b64decode(result).decode().split(":")
             dxf_obj.authenticate(username, password, response)
         else:
             dxf_obj._headers = {"Authorization": "Basic " + result}
 
     async def delete(self, job):
-        if not await self.contains(job):
-            return
+        # if not await self.contains(job):
+        #    return
 
         self._delete_inner(job)  # blocking! epic fail
 
     def _delete_inner(self, job):
         random_data = os.urandom(16)
         random_digest = "sha256:" + hashlib.sha256(random_data).hexdigest()
 
@@ -899,14 +914,16 @@
     async def info(self, job):
         async with await self.open(job, "rb") as fp:
             s = await fp.read()
         return yaml.safe_load(s)
 
     @job_getter
     async def dump(self, job, data):
+        if not self.is_valid_job_id(job):
+            raise KeyError(job)
         s = yaml.safe_dump(data, None)
         async with await self.open(job, "w") as fp:
             await fp.write(s)
 
 
 class YamlMetadataFileRepository(YamlMetadataRepository, FileRepository):
     """
@@ -918,16 +935,16 @@
 
 
 class YamlMetadataS3Repository(YamlMetadataRepository, S3BucketRepository):
     """
     A metadata repository based on a s3 bucket repository.
     """
 
-    def __init__(self, client, bucket, prefix, extension=".yaml", mimetype="text/yaml"):
-        super().__init__(client, bucket, prefix, extension=extension, mimetype=mimetype)
+    def __init__(self, client, bucket, prefix, suffix=".yaml", mimetype="text/yaml"):
+        super().__init__(client, bucket, prefix, suffix=suffix, mimetype=mimetype)
 
     @job_getter
     async def info(self, job):
         try:
             return await super().info(job)
         except botocore.exceptions.ClientError as e:
             if "NoSuchKey" in str(e):
@@ -1066,14 +1083,16 @@
 
     @job_getter
     async def info(self, job):
         return self.data.get(job)
 
     @job_getter
     async def dump(self, job, data):
+        if not self.is_valid_job_id(job):
+            raise KeyError(job)
         self.data[job] = data
 
     async def contains(self, item):
         return item in self.data
 
     async def delete(self, job):
         del self.data[job]
@@ -1135,14 +1154,16 @@
         """
         There is no templating info for an `InProcessBlobRepository`.
         """
         return None
 
     @job_getter
     async def open(self, job, mode="r"):
+        if not self.is_valid_job_id(job):
+            raise KeyError(job)
         stream = InProcessBlobStream(self, job)
         if mode == "r":
             return AReadText(stream)
         elif mode == "w":
             return AWriteText(stream)
         else:
             return stream
```

### Comparing `pydatatask-0.3.2/pydatatask/resource_manager.py` & `pydatatask-0.4.7/pydatatask/resource_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,65 +19,75 @@
 from kubernetes.utils import parse_quantity
 
 __all__ = ("ResourceType", "Resources", "ResourceManager", "parse_quantity")
 
 
 class ResourceType(Enum):
     """
-    An enum class indicating a type of resource. Presently can be CPU or MEM.
+    An enum class indicating a type of resource. Presently can be CPU, MEM, or RATE.
     """
 
     CPU = auto()
     MEM = auto()
+    RATE = auto()
 
 
 @dataclass
 class Resources:
     """
     A dataclass containing a quantity of resources.
 
     Resources can be summed:
 
     .. code:: python
 
-        r = pydatatask.Resources.parse(1, 1)
-        r += pydatatask.Resources.parse(2, 3)
-        r -= pydatatask.Resources.parse(1, 1)
-        assert r == pydatatask.Resources.parse(2, 3)
+        r = pydatatask.Resources.parse(1, 1, 100)
+        r += pydatatask.Resources.parse(2, 3, 0)
+        r -= pydatatask.Resources.parse(1, 1, 0)
+        assert r == pydatatask.Resources.parse(2, 3, 100)
     """
 
     cpu: Decimal = field(default=Decimal(0))
     mem: Decimal = field(default=Decimal(0))
+    launches: int = 1
 
     @staticmethod
-    def parse(cpu: Union[str, float, int, Decimal], mem: Union[str, float, int, Decimal]) -> "Resources":
-        """
-        Construct a :class:`Resources` instance by parsing the given quantities of CPU and memory.
-        """
-        return Resources(cpu=parse_quantity(cpu), mem=parse_quantity(mem))
+    def parse(
+        cpu: Union[str, float, int, Decimal],
+        mem: Union[str, float, int, Decimal],
+        launches: Union[str, float, int, Decimal, None] = None,
+    ) -> "Resources":
+        """
+        Construct a :class:`Resources` instance by parsing the given quantities of CPU, memory, and launches.
+        """
+        if launches is None:
+            launches = 999999999
+        return Resources(cpu=parse_quantity(cpu), mem=parse_quantity(mem), launches=int(launches))
 
     def __add__(self, other: "Resources"):
-        return Resources(cpu=self.cpu + other.cpu, mem=self.mem + other.mem)
+        return Resources(cpu=self.cpu + other.cpu, mem=self.mem + other.mem, launches=self.launches + other.launches)
 
     def __mul__(self, other: int):
-        return Resources(cpu=self.cpu * other, mem=self.mem * other)
+        return Resources(cpu=self.cpu * other, mem=self.mem * other, launches=self.launches * other)
 
     def __sub__(self, other: "Resources"):
         return self + other * -1
 
     def excess(self, limit: "Resources") -> Optional[ResourceType]:
         """
         Determine if these resources are over a given limit.
 
         :return: The ResourceType of the first resource that is over-limit, or None if self is under-limit.
         """
         if self.cpu > limit.cpu:
             return ResourceType.CPU
         elif self.mem > limit.mem:
             return ResourceType.MEM
+        elif self.launches > limit.launches:
+            return ResourceType.RATE
         else:
             return None
 
 
 class ResourceManager:
     """
     The ResourceManager tracks quotas of resources. Direct use of this class beyond construction will only be necessary
@@ -105,14 +115,22 @@
 
     async def _getter(self):
         result = Resources()
         for getter in self._registered_getters:
             result += await getter()
         return result
 
+    async def flush(self):
+        """
+        Forget the cached amount of resources currently being used. Next call to reserve or relinquish will calculate
+        usage anew.
+        """
+        async with self._lock:
+            self._cached = None
+
     async def reserve(self, request: Resources) -> Optional[ResourceType]:
         """
         Atomically reserve the given amount of resources and return None, or do nothing and return the limiting resource
         type if any resource would be over-quota.
         """
         async with self._lock:
             if self._cached is None:
```

### Comparing `pydatatask-0.3.2/pydatatask/session.py` & `pydatatask-0.4.7/pydatatask/session.py`

 * *Files identical despite different names*

### Comparing `pydatatask-0.3.2/pydatatask/task.py` & `pydatatask-0.4.7/pydatatask/task.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 For a shortcut for linking the output of one task as the input of another task, see `Task.plug`.
 
 .. autodata:: STDOUT
 """
 from typing import (
     TYPE_CHECKING,
     Any,
+    Awaitable,
     Callable,
-    Coroutine,
     Dict,
     Iterable,
     Optional,
     Protocol,
     Tuple,
     Union,
 )
@@ -27,14 +27,15 @@
 from asyncio import Future
 from concurrent.futures import FIRST_EXCEPTION, Executor, wait
 from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 from enum import Enum, auto
 from pathlib import Path
 import asyncio
+import copy
 import inspect
 import logging
 import os
 import sys
 import traceback
 
 from kubernetes_asyncio.client import ApiException, V1Pod
@@ -333,32 +334,14 @@
         Part one of the pipeline maintenance loop. Override this to perform any maintenance operations on the set of
         live tasks. Typically, this entails reaping finished processes.
 
         Returns True if literally anything interesting happened, or if there are any live tasks.
         """
         raise NotImplementedError
 
-    async def launch_all(self):
-        """
-        Part two of the pipeline maintenance loop. Do not override this; the default implementation is typically pretty
-        good - it enumerates `ready` and calls `launch` for each ready job.
-
-        Returns True if there were any jobs to launch.
-        """
-        launchers = [self._launch(job) async for job in self.ready]
-        await asyncio.gather(*launchers)
-        return bool(launchers)
-
-    async def _launch(self, job):
-        try:
-            l.debug("Launching %s:%s", self.name, job)
-            await self.launch(job)
-        except:
-            l.exception("Failed to launch %s:%s", self, job)
-
     @abstractmethod
     async def launch(self, job):
         """
         Launch a job. Override this to begin execution of the provided job. Error handling will be done for you.
         """
         raise NotImplementedError
 
@@ -407,28 +390,31 @@
         self,
         name: str,
         podman: Callable[[], PodManager],
         resources: ResourceManager,
         template: Union[str, Path],
         logs: Optional[BlobRepository],
         done: Optional[MetadataRepository],
+        window: timedelta = timedelta(minutes=1),
         timeout: Optional[timedelta] = None,
         env: Optional[Dict[str, Any]] = None,
         ready: Optional[Repository] = None,
     ):
         """
         :param name: The name of the task.
         :param podman: A callable returning a PodManager to use to connect to the cluster.
         :param resources: A ResourceManager instance. Tasks launched will contribute to its quota and be denied if they
                           would break the quota.
         :param template: YAML markup for a pod manifest template, either as a string or a path to a file.
         :param logs: Optional: A BlobRepository to dump pod logs to on completion. Linked as "logs" with
                                ``inhibits_start, required_for_output, is_status``.
         :param done: A MetadataRepository in which to dump some information about the pod's lifetime and termination on
                      completion. Linked as "done" with ``inhibits_start, required_for_output, is_status``.
+        :param window:  Optional: How far back into the past to look in order to determine whether we have recently
+                        launched too many pods too quickly.
         :param timeout: Optional: When a pod is found to have been running continuously for this amount of time, it will
                         be timed out and stopped. The method `handle_timeout` will be called in-process.
         :param env:     Optional: Additional keys to add to the template environment.
         :param ready:   Optional: A repository from which to read task-ready status.
 
         It is highly recommended to provide one or more of ``done`` or ``logs`` so that at least one link is present
         with ``inhibits_start``.
@@ -439,14 +425,15 @@
         self.resources = resources
         self._podman = podman
         self.logs = logs
         self.timeout = timeout
         self.done = done
         self.env = env if env is not None else {}
         self.warned = False
+        self.window = window
 
         self.resources.register(self._get_load)
 
         self.link(
             "live",
             LiveKubeRepository(self),
             is_status=True,
@@ -475,24 +462,23 @@
         """
         The pod manager instance for this task. Will raise an error if the manager is provided by an unopened session.
         """
         return self._podman()
 
     async def _get_load(self):
         usage = Resources()
+        cutoff = datetime.now(tz=timezone.utc) - self.window
 
         try:
-            for pod in (
-                await self.podman.v1.list_namespaced_pod(
-                    self.podman.namespace, label_selector=f"app={self.podman.app},task={self.name}"
-                )
-            ).items:
+            for pod in await self.podman.query(task=self.name):
+                if pod.metadata.creation_timestamp > cutoff:
+                    usage += Resources(launches=1)
                 for container in pod.spec.containers:
                     usage += Resources.parse(
-                        container.resources.requests["cpu"], container.resources.requests["memory"]
+                        container.resources.requests["cpu"], container.resources.requests["memory"], 0
                     )
         except ApiException as e:
             if e.reason != "Forbidden":
                 raise
 
         return usage
 
@@ -509,18 +495,20 @@
             if asyncio.iscoroutine(item):
                 item.close()
 
         assert manifest["kind"] == "Pod"
         spec = manifest["spec"]
         spec["restartPolicy"] = "Never"
 
-        request = Resources()
+        request = Resources(launches=1)
         for container in spec["containers"]:
             request += Resources.parse(
-                container["resources"]["requests"]["cpu"], container["resources"]["requests"]["memory"]
+                container["resources"]["requests"]["cpu"],
+                container["resources"]["requests"]["memory"],
+                0,
             )
 
         limit = await self.resources.reserve(request)
         if limit is None:
             try:
                 await self.podman.launch(job, self.name, manifest)
             except:
@@ -533,66 +521,69 @@
     async def _cleanup(self, pod: V1Pod, reason: str):
         job = pod.metadata.labels["job"]
 
         if self.logs is not None:
             async with await self.logs.open(job, "w") as fp:
                 try:
                     await fp.write(await self.podman.logs(pod))
-                except TimeoutError:
+                except (TimeoutError, ApiException):
                     await fp.write("<failed to fetch logs>\n")
         if self.done is not None:
             data = {
                 "reason": reason,
                 "start_time": pod.metadata.creation_timestamp,
-                "end_time": datetime.now(timezone.utc),
+                "end_time": datetime.now(tz=timezone.utc),
                 "image": pod.status.container_statuses[0].image,
                 "node": pod.spec.node_name,
             }
             await self.done.dump(job, data)
 
         await self.delete(pod)
 
     async def delete(self, pod: V1Pod):
         """
         Kill a pod and relinquish its resources without marking the task as complete.
         """
-        request = Resources()
+        request = Resources(launches=1)
         for container in pod.spec.containers:
-            request += Resources.parse(container.resources.requests["cpu"], container.resources.requests["memory"])
+            request += Resources.parse(container.resources.requests["cpu"], container.resources.requests["memory"], 0)
         await self.podman.delete(pod)
         await self.resources.relinquish(request)
 
     async def update(self):
         self.warned = False
         result = False
 
         pods = await self.podman.query(task=self.name)
-        for pod in pods:
-            result = True
-            try:
-                uptime: timedelta = datetime.now(timezone.utc) - pod.metadata.creation_timestamp
-                total_min = uptime.total_seconds() // 60
-                uptime_hours, uptime_min = divmod(total_min, 60)
-                l.debug(
-                    "Pod %s is alive for %dh%dm",
-                    pod.metadata.name,
-                    uptime_hours,
-                    uptime_min,
-                )
-                if pod.status.phase in ("Succeeded", "Failed"):
-                    l.debug("...finished: %s", pod.status.phase)
-                    await self._cleanup(pod, pod.status.phase)
-                elif self.timeout is not None and uptime > self.timeout:
-                    l.debug("...timed out")
-                    await self.handle_timeout(pod)
-                    await self._cleanup(pod, "Timeout")
-            except Exception:
-                l.exception("Failed to update kube task %s:%s", self.name, pod.metadata.name)
+        result = bool(pods)
+        jobs = [self._update_one(pod) for pod in pods]
+        await asyncio.gather(*jobs)
         return result
 
+    async def _update_one(self, pod: V1Pod):
+        try:
+            uptime: timedelta = datetime.now(tz=timezone.utc) - pod.metadata.creation_timestamp
+            total_min = uptime.total_seconds() // 60
+            uptime_hours, uptime_min = divmod(total_min, 60)
+            l.debug(
+                "Pod %s is alive for %dh%dm",
+                pod.metadata.name,
+                uptime_hours,
+                uptime_min,
+            )
+            if pod.status.phase in ("Succeeded", "Failed"):
+                l.debug("...finished: %s", pod.status.phase)
+                await self._cleanup(pod, pod.status.phase)
+            elif self.timeout is not None and uptime > self.timeout:
+                l.debug("...timed out")
+                await self.handle_timeout(pod)
+                await self._cleanup(pod, "Timeout")
+        except Exception:
+            l.exception("Failed to update kube task %s:%s", self.name, pod.metadata.name)
+
     async def handle_timeout(self, pod: V1Pod):
         """
         You may override this method in a subclass, and it will be called whenever a pod times out. You can use this
         method to e.g. scrape in-progress data out of the pod via an exec.
         """
 
 
@@ -613,14 +604,15 @@
         self,
         name: str,
         manager: Callable[[], "AbstractProcessManager"],
         resource_manager: "ResourceManager",
         job_resources: "Resources",
         pids: MetadataRepository,
         template: str,
+        window: timedelta = timedelta(minutes=1),
         environ: Optional[Dict[str, str]] = None,
         done: Optional[MetadataRepository] = None,
         stdin: Optional[BlobRepository] = None,
         stdout: Optional[BlobRepository] = None,
         stderr: Optional[Union[BlobRepository, _StderrIsStdout]] = None,
         ready: Optional[Repository] = None,
     ):
@@ -632,14 +624,16 @@
         :param job_resources: The amount of resources an individual job should contribute to the quota. Note that this
                               is currently **not enforced** target-side, so jobs may actually take up more resources
                               than assigned.
         :param pids: A metadata repository used to store the current live-status of processes. Will automatically be
                      linked as "pids" with ``is_status, inhibits_start, inhibits_output``.
         :param template: YAML markup for the template of a script to run, either as a string or a path to a file.
         :param environ: Additional environment variables to set on the target machine before running the task.
+        :param window: How recently a process must have been launched in order to contribute to the process
+                       rate-limiting.
         :param done: Optional: A metadata repository in which to dump some information about the process's lifetime and
                      termination on completion. Linked as "done" with
                      ``inhibits_start, required_for_output, is_status``.
         :param stdin: Optional: A blob repository from which to source the process' standard input. The content will be
                       preloaded and transferred to the target environment, so the target does not need to be
                       authenticated to this repository. Linked as "stdin" with ``is_input``.
         :param stdout: Optional: A blob repository into which to dump the process' standard output. The content will be
@@ -660,18 +654,20 @@
         self.pids = pids
         self.template = template
         self.environ = environ
         self.done = done
         self.stdin = stdin
         self.stdout = stdout
         self._stderr = stderr
-        self.job_resources = job_resources
+        self.job_resources = copy.copy(job_resources)
+        self.job_resources.launches = 1
         self.resource_manager = resource_manager
         self._manager = manager
         self.warned = False
+        self.window = window
 
         self.resource_manager.register(self._get_load)
 
         self.link("pids", pids, is_status=True, inhibits_start=True, inhibits_output=True)
         if stdin is not None:
             self.link("stdin", stdin, is_input=True)
         if stdout is not None:
@@ -685,18 +681,24 @@
     def manager(self) -> "AbstractProcessManager":
         """
         The process manager for this task. Will raise an error if the manager comes from a session which is closed.
         """
         return self._manager()
 
     async def _get_load(self) -> "Resources":
+        cutoff = datetime.now(tz=timezone.utc) - self.window
         count = 0
-        async for _ in self.pids:
+        recent = 0
+        job_map = await self.pids.info_all()
+        for v in job_map.values():
             count += 1
-        return self.job_resources * count
+            if v["start_time"] > cutoff:
+                recent += 1
+
+        return self.job_resources * count - Resources(launches=count - recent)
 
     @property
     def stderr(self) -> Optional[BlobRepository]:
         """
         The repository into which stderr will be dumped, or None if it will go to the null device.
         """
         if isinstance(self._stderr, BlobRepository):
@@ -722,18 +724,20 @@
         expected_live = set(pid_map)
         try:
             live_pids = await self.manager.get_live_pids(expected_live)
         except Exception:
             l.error("Could not load live PIDs for %s", self, exc_info=True)
         else:
             died = expected_live - live_pids
+            coros = []
             for pid in died:
                 job = pid_map[pid]
                 start_time = job_map[job]["start_time"]
-                await self._reap(job, start_time)
+                coros.append(self._reap(job, start_time))
+            await asyncio.gather(*coros)
         return bool(expected_live)
 
     async def launch(self, job):
         limit = await self.resource_manager.reserve(self.job_resources)
         if limit is not None:
             if not self.warned:
                 l.warning("Cannot launch %s: %s limit", self, limit)
@@ -816,15 +820,15 @@
 
 
 class FunctionTaskProtocol(Protocol):
     """
     The protocol which is expected by the tasks which take a python function to execute.
     """
 
-    def __call__(self, job: str, **kwargs) -> Coroutine:
+    def __call__(self, job: str, **kwargs) -> Awaitable[None]:
         ...
 
 
 class InProcessSyncTask(Task):
     """
     A task which runs in-process. Typical usage of this task might look like the following:
 
@@ -877,15 +881,15 @@
             else:
                 raise NameError("%s takes parameter %s but no such argument is available" % (self.func, name))
 
     async def update(self):
         pass
 
     async def launch(self, job):
-        start_time = datetime.now()
+        start_time = datetime.now(tz=timezone.utc)
         l.debug("Launching in-process %s:%s...", self.name, job)
         args = dict(self._env)
         if "job" in args:
             args["job"] = job
         args = await build_env(args, job, RepoHandlingMode.SMART)
         try:
             await self.func(**args)
@@ -896,15 +900,15 @@
                 "exception": repr(e),
                 "traceback": traceback.format_tb(e.__traceback__),
             }
         else:
             l.debug("...success")
             result = {"result": "success"}
         result["start_time"] = start_time
-        result["end_time"] = datetime.now()
+        result["end_time"] = datetime.now(tz=timezone.utc)
         if self.metadata:
             await self.done.dump(job, result)
 
 
 class ExecutorTask(Task):
     """
     A task which runs python functions in a :external:class:`concurrent.futures.Executor`. This has not been tested on
@@ -953,30 +957,32 @@
     def __call__(self, f: Callable) -> "ExecutorTask":
         self.func = f
         return self
 
     async def update(self):
         result = bool(self.jobs)
         done, _ = wait(self.jobs, 0, FIRST_EXCEPTION)
+        coros = []
         for finished_job in done:
             job, start_time = self.jobs.pop(finished_job)
             # noinspection PyAsyncCall
             self.rev_jobs.pop(job)
-            await self._cleanup(finished_job, job, start_time)
+            coros.append(self._cleanup(finished_job, job, start_time))
+        await asyncio.gather(*coros)
         return result
 
     async def _cleanup(self, job_future, job, start_time):
         e = job_future.exception()
         if e is not None:
             l.info("Executor task %s:%s failed", self.name, job, exc_info=e)
             data = {
                 "result": "exception",
                 "exception": repr(e),
                 "traceback": traceback.format_tb(e.__traceback__),
-                "end_time": datetime.now(),
+                "end_time": datetime.now(tz=timezone.utc),
             }
         else:
             l.debug("...executor task %s:%s success", self.name, job)
             data = {"result": "success", "end_time": job_future.result()}
         data["start_time"] = start_time
         await self.done.dump(job, data)
 
@@ -995,15 +1001,15 @@
 
     async def launch(self, job):
         l.debug("Launching %s:%s with %s...", self.name, job, self.executor)
         args = dict(self._env)
         if "job" in args:
             args["job"] = job
         args = await build_env(args, job, RepoHandlingMode.SMART)
-        start_time = datetime.now()
+        start_time = datetime.now(tz=timezone.utc)
         running_job = self.executor.submit(self._timestamped_func, self.func, args)
         if self.synchronous:
             while not running_job.done():
                 await asyncio.sleep(0.1)
             await self._cleanup(running_job, job, start_time)
         else:
             self.jobs[running_job] = (job, start_time)
@@ -1018,15 +1024,15 @@
             future.cancel()
             self.jobs.pop(future)
 
     @staticmethod
     def _timestamped_func(func, args):
         loop = asyncio.new_event_loop()
         loop.run_until_complete(func(**args))
-        return datetime.now()
+        return datetime.now(tz=timezone.utc)
 
 
 class KubeFunctionTask(KubeTask):
     """
     A task which runs a python function on a kubernetes cluster. Requires a pod template which will execute a python
     script calling `pydatatask.main.main`. This works by running ``python3 main.py launch [task] [job] --sync``.
 
@@ -1137,15 +1143,15 @@
     async def launch(self, job):
         if self.synchronous:
             await self._launch_sync(job)
         else:
             await super().launch(job)
 
     async def _launch_sync(self, job):
-        start_time = datetime.now()
+        start_time = datetime.now(tz=timezone.utc)
         l.debug("Launching --sync %s:%s...", self.name, job)
         args = dict(self._func_env)
         if "job" in args:
             args["job"] = job
         args = await build_env(args, job, RepoHandlingMode.SMART)
         try:
             await self.func(**args)
@@ -1156,10 +1162,10 @@
                 "exception": repr(e),
                 "traceback": traceback.format_tb(e.__traceback__),
             }
         else:
             l.debug("...success")
             result = {"result": "success"}
         result["start_time"] = start_time
-        result["end_time"] = datetime.now()
+        result["end_time"] = datetime.now(tz=timezone.utc)
         if self.metadata:
             await self.func_done.dump(job, result)
```

### Comparing `pydatatask-0.3.2/pydatatask/utils.py` & `pydatatask-0.4.7/pydatatask/utils.py`

 * *Files identical despite different names*

### Comparing `pydatatask-0.3.2/pydatatask.egg-info/PKG-INFO` & `pydatatask-0.4.7/pydatatask.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatatask
-Version: 0.3.2
+Version: 0.4.7
 Summary: Library for constructing data-centric processing pipelines with few invariants
 Author-email: Audrey Dutcher <audrey@rhelmot.io>
 License: Copyright 2022 Audrey Dutcher
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -12,13 +12,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: repository, https://github.com/rhelmot/pydatatask
 Project-URL: documentation, https://pydatatask.readthedocs.io/
 Keywords: pipeline,data,task,repository,processing,async,kubernetes,s3,mongodb,docker,ssh
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: fuse
 Provides-Extra: dev
 Provides-Extra: type
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 License-File: LICENSE
```

### Comparing `pydatatask-0.3.2/pydatatask.egg-info/SOURCES.txt` & `pydatatask-0.4.7/pydatatask.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
+setup.py
 pydatatask/__init__.py
+pydatatask/fuse.py
 pydatatask/main.py
 pydatatask/pipeline.py
 pydatatask/pod_manager.py
 pydatatask/proc_manager.py
 pydatatask/py.typed
 pydatatask/repository.py
 pydatatask/resource_manager.py
```

### Comparing `pydatatask-0.3.2/pyproject.toml` & `pydatatask-0.4.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -27,27 +27,34 @@
     "aiofiles",
     "aioshutil",
     "psutil",
     "asyncssh",
 ]
 
 [project.optional-dependencies]
+all = [
+    "pydatafs"
+]
+fuse = [
+    "pydatafs"
+]
 dev = [
     "tox>=4.0.0",
     "black",
     "isort",
     "pre-commit",
 ]
 type = [
     "mypy",
     "kubernetes-typed",
     "types-pyyaml",
     "networkx-stubs",
     "types-aiofiles",
     "types-psutil",
+    "pyfuse3-stubs",
 ]
 test = [
     "pytest",
     "pytest-cov",
     "coverage[toml]"
 ]
 lint = [
@@ -83,22 +90,17 @@
 ignore_missing_imports = true
 
 # https://jira.mongodb.org/projects/MOTOR/issues/MOTOR-331
 [[tool.mypy.overrides]]
 module = "motor.*"
 ignore_missing_imports = true
 
-# https://github.com/davedoesdev/dxf/pull/43
-[[tool.mypy.overrides]]
-module = "dxf.*"
-ignore_missing_imports = true
-
-# https://github.com/ipython/ipython/pull/13858
+# lol
 [[tool.mypy.overrides]]
-module = "IPython.*"
+module = "pydatafs.*"
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--cov=pydatatask --cov-report=xml -ra --log-level INFO"
 
 [tool.black]
```

### Comparing `pydatatask-0.3.2/tests/test_basic.py` & `pydatatask-0.4.7/tests/test_basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 data = await fp.read(await repo0.info(job))
             async with await repo1.open(job, "w") as fp:
                 await fp.write(data.hex()[: len(data)])
 
         task.link("repo0", repo0, is_input=True)
         task.link("repo1", repo1, is_output=True)
 
-        pipeline = pydatatask.Pipeline([task], session)
+        pipeline = pydatatask.Pipeline([task], session, [])
         async with pipeline:
             await pydatatask.run(pipeline, forever=False, launch_once=False, timeout=None)
 
         assert len(repo0.data) == len(repo1.data)
         for job, i in repo0.data.items():
             assert len(repo1.data[job]) == i
```

### Comparing `pydatatask-0.3.2/tests/test_docker.py` & `pydatatask-0.4.7/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `pydatatask-0.3.2/tests/test_executor.py` & `pydatatask-0.4.7/tests/test_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
         phase0.link("repo_zero", repo0, is_input=True)
         phase0.link("repo_one", repo1, is_output=True)
 
         phase1.plug(phase0)
         phase1.link("repo_two", repo2, is_output=True)
 
-        pipeline = pydatatask.Pipeline([phase0, phase1], session)
+        pipeline = pydatatask.Pipeline([phase0, phase1], session, [])
 
         async with pipeline:
             await pydatatask.run(pipeline, forever=False, launch_once=False, timeout=120)
             await pydatatask.launch(pipeline, "phase0", "bar", sync=True, meta=True, force=True)
 
         assert repo2.data["foo"] == "weh!?"
         assert "exception" in phase0_done.data["bar"]
```

### Comparing `pydatatask-0.3.2/tests/test_filesystem.py` & `pydatatask-0.4.7/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `pydatatask-0.3.2/tests/test_kube.py` & `pydatatask-0.4.7/tests/test_kube.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             self.kube_context = self.minikube_profile
 
     async def test_kube(self):
         session = pydatatask.Session()
 
         await kubernetes_asyncio.config.load_kube_config(context=self.kube_context)
 
-        cluster_quota = pydatatask.ResourceManager(pydatatask.Resources.parse("1", "1Gi"))
+        cluster_quota = pydatatask.ResourceManager(pydatatask.Resources.parse("1", "1Gi", 99999))
 
         @session.resource
         async def podman():
             podman = pydatatask.PodManager(
                 f"test-{self.test_id}",
                 self.kube_namespace,
             )
@@ -106,15 +106,15 @@
                     memory: 100Mi
             """,
             logs=repoLogs,
             done=repoDone,
         )
         task.link("repo0", repo0, is_input=True)
 
-        pipeline = pydatatask.Pipeline([task], session)
+        pipeline = pydatatask.Pipeline([task], session, [cluster_quota])
 
         async with pipeline:
             await pydatatask.update(pipeline)
             live = task.links["live"].repo
             launched = [x async for x in live]
             assert launched
             assert await live.contains(launched[0])
```

### Comparing `pydatatask-0.3.2/tests/test_minio.py` & `pydatatask-0.4.7/tests/test_minio.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             "s3",
             endpoint_url="http://" + self.minio_endpoint,
             aws_access_key_id=self.minio_username,
             aws_secret_access_key=self.minio_password,
         ).__aenter__()
 
     async def test_minio(self):
-        repo = pydatatask.S3BucketRepository(lambda: self.client, self.bucket, prefix="weh/", extension=".weh")
+        repo = pydatatask.S3BucketRepository(lambda: self.client, self.bucket, prefix="weh/", suffix=".weh")
         repo_yaml = pydatatask.YamlMetadataS3Repository(lambda: self.client, self.bucket, prefix="weh/")
         assert repr(repo)
         await repo.validate()
         await repo_yaml.validate()
 
         async with await repo.open("foo", "w") as fp:
             await fp.write("hello world")
```

### Comparing `pydatatask-0.3.2/tests/test_mongodb.py` & `pydatatask-0.4.7/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `pydatatask-0.3.2/tests/test_process.py` & `pydatatask-0.4.7/tests/test_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     async def test_local_process(self):
         session = pydatatask.Session()
 
         @session.resource
         async def localhost():
             yield pydatatask.LocalLinuxManager(self.app, local_path=self.dir)
 
-        quota = pydatatask.ResourceManager(pydatatask.Resources.parse(1, 1))
+        quota = pydatatask.ResourceManager(pydatatask.Resources.parse(1, 1, 99999))
 
         repo_input = pydatatask.FileRepository(self.dir / "input")
         await repo_input.validate()
         for i in range(self.n):
             async with await repo_input.open(str(i), "w") as fp:
                 await fp.write(str(i))
         repo_stdout = pydatatask.InProcessBlobRepository()
@@ -51,23 +51,23 @@
         task = pydatatask.ProcessTask(
             "task",
             localhost,
             quota,
             pydatatask.Resources.parse("100m", "100m"),
             repo_pids,
             template,
-            {},
-            repo_done,
-            None,
-            repo_stdout,
-            pydatatask.STDOUT,
+            environ={},
+            done=repo_done,
+            stdin=None,
+            stdout=repo_stdout,
+            stderr=pydatatask.STDOUT,
         )
         task.link("input", repo_input, is_input=True)
 
-        pipeline = pydatatask.Pipeline([task], session)
+        pipeline = pydatatask.Pipeline([task], session, [quota])
 
         async with pipeline:
             await pydatatask.run(pipeline, False, False, 120)
 
         assert len(repo_pids.data) == 0
         assert len(repo_stdout.data) == self.n
         assert len(repo_done.data) == self.n
@@ -106,42 +106,45 @@
             f"{self.port}:2222",
             "-e",
             "USER_NAME=weh",
             "-e",
             "USER_PASSWORD=weh",
             "-e",
             "PASSWORD_ACCESS=true",
-            "linuxserver/openssh-server:latest",
+            "linuxserver/openssh-server:version-9.1_p1-r2",
             stdin=asyncio.subprocess.DEVNULL,
             stdout=asyncio.subprocess.DEVNULL,
             stderr=asyncio.subprocess.DEVNULL,
         )
         await p.communicate()
         if await p.wait() != 0:
-            raise unittest.SkipTest(
-                "No minio endpoint configured and docker failed to launch linuxserver/openssh-server:latest"
-            )
+            raise unittest.SkipTest("docker failed to launch linuxserver/openssh-server:version-9.1_p1-r2")
         self.docker_name = name
         await asyncio.sleep(2)
 
     async def test_ssh_process(self):
         session = pydatatask.Session()
 
         @session.resource
         async def ssh():
             async with asyncssh.connect(
-                "localhost", port=self.port, username="weh", password="weh", known_hosts=None
+                "localhost",
+                port=self.port,
+                username="weh",
+                password="weh",
+                known_hosts=None,
+                client_keys=None,
             ) as s:
                 yield s
 
         @session.resource
         async def procman():
             yield pydatatask.SSHLinuxManager(self.test_id, ssh)
 
-        quota = pydatatask.ResourceManager(pydatatask.Resources.parse(1, 1))
+        quota = pydatatask.ResourceManager(pydatatask.Resources.parse(1, 1, 99999))
 
         repo_stdin = pydatatask.InProcessBlobRepository({str(i): str(i).encode() for i in range(self.n)})
         repo_stdout = pydatatask.InProcessBlobRepository()
         repo_stderr = pydatatask.InProcessBlobRepository()
         repo_done = pydatatask.InProcessMetadataRepository()
         repo_pids = pydatatask.InProcessMetadataRepository()
 
@@ -155,34 +158,34 @@
         task = pydatatask.ProcessTask(
             "task",
             procman,
             quota,
             pydatatask.Resources.parse("100m", "100m"),
             repo_pids,
             template,
-            {},
-            repo_done,
-            repo_stdin,
-            repo_stdout,
-            repo_stderr,
+            environ={},
+            done=repo_done,
+            stdin=repo_stdin,
+            stdout=repo_stdout,
+            stderr=repo_stderr,
         )
 
-        pipeline = pydatatask.Pipeline([task], session)
+        pipeline = pydatatask.Pipeline([task], session, [quota])
 
         async with pipeline:
             await pydatatask.run(pipeline, False, False, 120)
 
         assert len(repo_stdin.data) == self.n
         assert len(repo_stdout.data) == self.n
         assert len(repo_stderr.data) == self.n
         assert len(repo_done.data) == self.n
         assert len(repo_pids.data) == 0
 
         for i in range(self.n):
-            assert repo_stderr.data[str(i)] == f"hello world!\ngoodbye world!\n".encode()
+            assert repo_stderr.data[str(i)] == "hello world!\ngoodbye world!\n".encode()
             assert (
                 repo_stdout.data[str(i)]
                 == f"The message of day {i} is {base64.b64encode(repo_stdin.data[str(i)]).decode()}. That's pretty great!\n".encode()
             )
             assert repo_done.data[str(i)]["return_code"] == 0
 
     async def asyncTearDown(self):
```

### Comparing `pydatatask-0.3.2/tests/test_related.py` & `pydatatask-0.4.7/tests/test_related.py`

 * *Files identical despite different names*

### Comparing `pydatatask-0.3.2/tests/test_repo_base.py` & `pydatatask-0.4.7/tests/test_repo_base.py`

 * *Files identical despite different names*


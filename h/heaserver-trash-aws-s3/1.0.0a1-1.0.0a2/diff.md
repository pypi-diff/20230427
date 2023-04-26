# Comparing `tmp/heaserver-trash-aws-s3-1.0.0a1.tar.gz` & `tmp/heaserver-trash-aws-s3-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a1.tar", last modified: Thu Apr 13 17:42:49 2023, max compression
+gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a2.tar", last modified: Wed Apr 26 23:42:17 2023, max compression
```

## Comparing `heaserver-trash-aws-s3-1.0.0a1.tar` & `heaserver-trash-aws-s3-1.0.0a2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:42:49.132017 heaserver-trash-aws-s3-1.0.0a1/
--rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a1/LICENSE
--rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0     4352 2023-04-13 17:42:49.131017 heaserver-trash-aws-s3-1.0.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 17:42:49.132017 heaserver-trash-aws-s3-1.0.0a1/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-04-13 17:41:59.000000 heaserver-trash-aws-s3-1.0.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:42:49.092516 heaserver-trash-aws-s3-1.0.0a1/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 17:42:49.091514 heaserver-trash-aws-s3-1.0.0a1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2023-04-13 17:42:49.104514 heaserver-trash-aws-s3-1.0.0a1/src/heaserver/trashawss3/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a1/src/heaserver/trashawss3/__init__.py
--rw-rw-rw-   0        0        0    45517 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a1/src/heaserver/trashawss3/service.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:42:49.105514 heaserver-trash-aws-s3-1.0.0a1/src/heaserver/trashawss3/wstl/
--rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a1/src/heaserver/trashawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2023-04-13 17:42:49.127019 heaserver-trash-aws-s3-1.0.0a1/src/heaserver_trash_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     4352 2023-04-13 17:42:49.000000 heaserver-trash-aws-s3-1.0.0a1/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-13 17:42:49.000000 heaserver-trash-aws-s3-1.0.0a1/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:42:49.000000 heaserver-trash-aws-s3-1.0.0a1/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-04-13 17:42:49.000000 heaserver-trash-aws-s3-1.0.0a1/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-04-13 17:42:49.000000 heaserver-trash-aws-s3-1.0.0a1/src/heaserver_trash_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 17:42:49.000000 heaserver-trash-aws-s3-1.0.0a1/src/heaserver_trash_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 17:42:49.092516 heaserver-trash-aws-s3-1.0.0a1/tests/
-drwxrwxrwx   0        0        0        0 2023-04-13 17:42:49.093515 heaserver-trash-aws-s3-1.0.0a1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-04-13 17:42:49.130017 heaserver-trash-aws-s3-1.0.0a1/tests/heaserver/trashawss3test/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a1/tests/heaserver/trashawss3test/__init__.py
--rw-rw-rw-   0        0        0    68988 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a1/tests/heaserver/trashawss3test/test_all.py
--rw-rw-rw-   0        0        0     6276 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a1/tests/heaserver/trashawss3test/testcase.py
+drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.870536 heaserver-trash-aws-s3-1.0.0a2/
+-rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a2/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4352 2023-04-26 23:42:17.869459 heaserver-trash-aws-s3-1.0.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 23:42:17.870536 heaserver-trash-aws-s3-1.0.0a2/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-04-26 23:41:45.000000 heaserver-trash-aws-s3-1.0.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.817972 heaserver-trash-aws-s3-1.0.0a2/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.817972 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/
+drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.841809 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/__init__.py
+-rw-rw-rw-   0        0        0    47506 2023-04-26 23:41:02.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/service.py
+drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.843808 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/wstl/
+-rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.865894 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     4352 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 23:42:17.000000 heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.833809 heaserver-trash-aws-s3-1.0.0a2/tests/
+drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.834808 heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-04-26 23:42:17.868557 heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/__init__.py
+-rw-rw-rw-   0        0        0    69298 2023-04-26 23:41:02.000000 heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/test_all.py
+-rw-rw-rw-   0        0        0     6276 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/testcase.py
```

### Comparing `heaserver-trash-aws-s3-1.0.0a1/LICENSE` & `heaserver-trash-aws-s3-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a1/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a1/README.md` & `heaserver-trash-aws-s3-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a1/setup.py` & `heaserver-trash-aws-s3-1.0.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-trash-aws-s3',
-    version='1.0.0a1',
+    version='1.0.0a2',
     description="deleted file management",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
```

### Comparing `heaserver-trash-aws-s3-1.0.0a1/src/heaserver/trashawss3/service.py` & `heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     :param request: the HTTP request.
     :return: Always returns status code 200.
     """
     return response.status_ok()
 
 
-@routes.route('OPTIONS', '/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}')
+@routes.route('OPTIONS', '/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}')
 async def get_item_options(request: web.Request) -> web.Response:
     """
     Gets the allowed HTTP methods for a trash item.
 
     :param request: a HTTP request (required).
     :return: the HTTP response.
     ---
@@ -103,15 +103,15 @@
             return response.status_not_found()
     except web.HTTPError as e:
         headers: dict[Union[str, istr], str] = {
             hdrs.CONTENT_TYPE: 'text/plain; charset=utf-8'}
         return response.status_generic(status=e.status, body=e.text, headers=headers)
 
 
-@routes.route('OPTIONS', '/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/opener')
+@routes.route('OPTIONS', '/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/opener')
 async def get_item_opener_options(request: web.Request) -> web.Response:
     """
     Gets the allowed HTTP methods for a trash item opener.
 
     :param request: a HTTP request (required).
     :return: the HTTP response.
     ---
@@ -164,29 +164,29 @@
             return response.status_not_found()
     except web.HTTPError as e:
         headers: dict[Union[str, istr], str] = {
             hdrs.CONTENT_TYPE: 'text/plain; charset=utf-8'}
         return response.status_generic(status=e.status, body=e.text, headers=headers)
 
 
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}')
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}')
 @action(name='heaserver-awss3trash-item-get-open-choices',
         rel='hea-opener-choices hea-context-menu',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/opener',
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/opener',
         itemif='actual_object_type_name == "heaobject.folder.AWSS3Folder"')
 @action(name='heaserver-awss3trash-item-get-properties',
         rel='hea-properties hea-context-menu')
 @action('heaserver-awss3trash-item-restore',
         rel='hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/restorer')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/restorer')
 @action('heaserver-awss3trash-item-permanently-delete',
         rel='hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/deleter')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/deleter')
 @action('heaserver-awss3trash-item-get-self', rel='self',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}')
 @action('heaserver-awss3trash-item-get-volume',
         rel='hea-volume',
         path='/volumes/{volume_id}')
 @action('heaserver-awss3trash-item-get-awsaccount',
         rel='hea-account',
         path='/volumes/{volume_id}/awsaccounts/me')
 async def get_deleted_item(request: web.Request) -> web.Response:
@@ -226,30 +226,30 @@
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
     return await response.get(request, await _get_deleted_item(request))
 
 
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/trashfolders/{trash_folder_id}/items/')
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/trashfolders/{trash_folder_id}/items')
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trashfolders/{trash_folder_id}/items/')
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trashfolders/{trash_folder_id}/items')
 @action(name='heaserver-awss3trash-item-get-open-choices',
         rel='hea-opener-choices hea-context-menu',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/opener',
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/opener',
         itemif='actual_object_type_name == "heaobject.folder.AWSS3Folder"')
 @action(name='heaserver-awss3trash-item-get-properties',
         rel='hea-properties hea-context-menu')
 @action('heaserver-awss3trash-item-restore',
         rel='hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/restorer')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/restorer')
 @action('heaserver-awss3trash-item-permanently-delete',
         rel='hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/deleter')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/deleter')
 @action('heaserver-awss3trash-item-get-self', rel='self',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}')
 async def get_items_in_trash_folder(request: web.Request) -> web.Response:
     """
     Gets a list of all deleted items in a volume, bucket, and trash folder. It
     only retrieves items with the folder as a parent, not including any
     subfolders.
 
     :param request: the HTTP request.
@@ -295,30 +295,30 @@
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
     return await response.get_all(request, [i async for i in _get_deleted_items(request)])
 
 
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/trash/')
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/trash')
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/awss3trash/')
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/awss3trash')
 @action(name='heaserver-awss3trash-item-get-open-choices',
         rel='hea-opener-choices hea-context-menu',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/opener',
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/opener',
         itemif='actual_object_type_name == "heaobject.folder.AWSS3Folder"')
 @action(name='heaserver-awss3trash-item-get-properties',
         rel='hea-properties hea-context-menu')
 @action('heaserver-awss3trash-item-restore',
         rel='hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/restorer')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/restorer')
 @action('heaserver-awss3trash-item-permanently-delete',
         rel='hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/deleter')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/deleter')
 @action('heaserver-awss3trash-item-get-self', rel='self',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}')
 async def get_deleted_items_in_folder(request: web.Request) -> web.Response:
     """
     Gets a list of all deleted items in a volume, bucket, and folder. It only
     retrieves items with the folder as a parent, not including any subfolders.
 
     :param request: the HTTP request.
     :return: the list of items with delete markers or the requested bucket, or
@@ -363,32 +363,32 @@
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
     return await response.get_all(request, [i async for i in _get_deleted_items(request)])
 
 
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/trash/')
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/trash')
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/')
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trash')
 @action(name='heaserver-awss3trash-item-get-open-choices',
         rel='hea-opener-choices hea-context-menu',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/opener',
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/opener',
         itemif='isheaobject(heaobject.folder.AWSS3Folder)')
 @action('heaserver-awss3trash-item-get-properties',
         rel='hea-properties hea-context-menu')
 @action('heaserver-awss3trash-item-restore',
         rel='hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/restorer')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/restorer')
 @action('heaserver-awss3trash-item-permanently-delete',
         rel='hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/deleter')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/deleter')
 @action('heaserver-awss3trash-item-get-self', rel='self',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}')
 @action('heaserver-awss3trash-do-empty-trash', rel='hea-trash-emptier',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trashemptier')
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trashemptier')
 async def get_all_deleted_items(request: web.Request) -> web.Response:
     """
     Gets a list of all deleted items in a volume and bucket.
 
     :param request: the HTTP request.
     :return: the list of items with delete markers or the requested bucket, Not
     Found.
@@ -422,15 +422,59 @@
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
     return await response.get_all(request, [i async for i in _get_deleted_items(request)])
 
 
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/trashemptier')
+
+@routes.get('/volumes/{volume_id}/awss3trash/')
+@routes.get('/volumes/{volume_id}/awss3trash')
+async def get_all_deleted_items_all_buckets(request: web.Request) -> web.Response:
+    """
+    Gets a list of all deleted items in a volume.
+
+    :param request: the HTTP request.
+    :return: the list of items with delete markers.
+    ---
+    summary: Gets a list of all deleted items.
+    tags:
+        - heaserver-trash-aws-s3
+    parameters:
+        - name: volume_id
+          in: path
+          required: true
+          description: The id of the volume to check for deleted files.
+          schema:
+            type: string
+          examples:
+            example:
+              summary: A volume id
+              value: 666f6f2d6261722d71757578
+    responses:
+      '200':
+        $ref: '#/components/responses/200'
+      '404':
+        $ref: '#/components/responses/404'
+    """
+    try:
+        volume_id = request.match_info['volume_id']
+    except KeyError as e:
+        return response.status_bad_request(str(e))
+    s3: S3Client = await request.app[HEA_DB].get_client(request, 's3', volume_id)
+    loop = asyncio.get_running_loop()
+    resp_ = await loop.run_in_executor(None, s3.list_buckets)
+    resp_list = []
+    for bucket in resp_.get('Buckets', []):
+        async for item in _get_deleted_items_private(s3, request.match_info['volume_id'], bucket['Name'], None, request.headers.get(SUB)):
+            resp_list.append(item)
+    return await response.get_all(request, resp_list)
+
+
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trashemptier')
 async def do_empty_trash(request: web.Request) -> web.Response:
     """
     Empties a version-enabled bucket's trash.
 
     :param request: the HTTP request.
     :return: No Content or Not Found.
     ---
@@ -463,15 +507,15 @@
         $ref: '#/components/responses/204'
       '404':
         $ref: '#/components/responses/404'
     """
     return await _do_empty_trash(request)
 
 
-@routes.delete('/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}')
+@routes.delete('/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}')
 async def permanently_delete_object_with_delete(request: web.Request) -> web.Response:
     """
     Delete all versions of a version enabled file
 
     :param request: the HTTP request.
     :return: No Content or Not Found.
     ---
@@ -505,15 +549,15 @@
         $ref: '#/components/responses/204'
       '404':
         $ref: '#/components/responses/404'
     """
     return await _permanently_delete_object(request)
 
 
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/deleter')
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/deleter')
 async def permanently_delete_object(request: web.Request) -> web.Response:
     """
     Delete all versions of a version enabled file
 
     :param request: the HTTP request.
     :return: No Content or Not Found.
     ---
@@ -547,15 +591,15 @@
         $ref: '#/components/responses/204'
       '404':
         $ref: '#/components/responses/404'
     """
     return await _permanently_delete_object(request)
 
 
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/restorer')
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/restorer')
 async def restore_object(request: web.Request) -> web.Response:
     """
     Removes the delete marker for a specified file
 
     :param request: the HTTP request.
     :return: No Content or Not Found.
     ---
@@ -590,18 +634,18 @@
       '404':
         $ref: '#/components/responses/404'
     """
     return await _undelete_object(request)
 
 
 
-@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/trash/{id}/opener')
+@routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/opener')
 @action('heaserver-awss3trash-item-open-default',
         rel='hea-opener hea-default application/x.item',
-        path='/volumes/{volume_id}/buckets/{bucket_id}/trashfolders/{id}/items/',
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trashfolders/{id}/items/',
         itemif='isheaobject(heaobject.folder.AWSS3Folder)')
 async def get_trash_item_opener(request: web.Request) -> web.Response:
     """
     Opens the requested trash forder.
 
     :param request: the HTTP request. Required.
     :return: the opened folder, or Not Found if the requested item does not exist.
@@ -771,14 +815,20 @@
     except (KeyDecodeException, ValueError) as e:
         raise response.status_not_found()
 
     try:
         s3 = await request.app[HEA_DB].get_client(request, 's3', volume_id)
     except ValueError:
         raise response.status_not_found()
+
+    async for item in _get_deleted_items_private(s3, volume_id, bucket_id, prefix, request.headers.get(SUB)):
+        yield item
+
+
+async def _get_deleted_items_private(s3, volume_id, bucket_id, prefix=None, sub_user=None) -> AsyncIterator[DesktopObjectDict]:
     loop_ = asyncio.get_running_loop()
 
     async for response_ in _get_version_objects(s3, bucket_id, prefix, loop_):
         keyfunc = lambda x: x['Key']
         keys = set()  # Potentially delete?
         for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain(response_.get('DeleteMarkers', []), response_.get('Versions', []))), key=keyfunc), key=keyfunc):
             if prefix is not None and not key.startswith(prefix):
@@ -786,24 +836,24 @@
             delete_markers_to_versions = {}
             delete_markers = []
             prev_delete_marker = None
             for is_delete_marker, versions_ in itertools.groupby(versions, key=lambda x: 'Size' not in x):
                 if is_delete_marker:
                     prev_delete_marker = next(versions_)
                     delete_markers.append(prev_delete_marker)
-                    delete_markers_to_versions[prev_delete_marker['VersionId']] = None
+                    # delete_markers_to_versions[prev_delete_marker['VersionId']] = None
                 elif prev_delete_marker and (prev_delete_marker['VersionId'] in delete_markers_to_versions):
                     delete_markers_to_versions[prev_delete_marker['VersionId']] = list(versions_)
             for delete_marker in delete_markers:
                 key = delete_marker['Key']
                 # if prefix is not None and parent(key) != prefix:
                 #     continue
                 last_modified = delete_marker['LastModified']
 
-                version = next((v for v in delete_markers_to_versions[delete_marker['VersionId']] \
+                version = next((v for v in delete_markers_to_versions.get(delete_marker['VersionId'], []) \
                                 if 'Size' in v and v['LastModified'] < delete_marker['LastModified']), None)
                 storage_class = version['StorageClass'] if version is not None and not is_folder(key) else None
                 # This is for handling folders
                 if prefix is not None:
                     try:
                         key_index = key.index('/', len(prefix))
                         if key_index > -1:
@@ -819,15 +869,15 @@
 
                 item = AWSS3FolderFileTrashItem()
                 item.bucket_id = bucket_id
                 item.key = key
                 item.version = delete_marker['VersionId']
                 item.modified = last_modified
                 item.created = last_modified
-                item.owner = request.headers.get(SUB, NONE_USER)
+                item.owner = sub_user if sub_user is not None else NONE_USER
                 item.volume_id = volume_id
                 item.source = AWS_S3
                 item.storage_class = storage_class
                 item.size = size
                 item.actual_object_type_name = AWSS3Folder.get_type_name() \
                     if is_folder(key) else AWSS3FileObject.get_type_name()
                 if is_folder(key):
```

### Comparing `heaserver-trash-aws-s3-1.0.0a1/src/heaserver/trashawss3/wstl/all.json` & `heaserver-trash-aws-s3-1.0.0a2/src/heaserver/trashawss3/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a1/src/heaserver_trash_aws_s3.egg-info/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a1/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt` & `heaserver-trash-aws-s3-1.0.0a2/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a1/tests/heaserver/trashawss3test/test_all.py` & `heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/test_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,37 +46,37 @@
                 Bucket='arp-scale-2-cloud-bucket-with-tags11', Prefix=key2)
             self.__version2 = next(v['VersionId'] for v in sorted(
                 versions['DeleteMarkers'], key=lambda x: x['LastModified'], reverse=True) if v['Key'] == key2)
 
             self.maxDiff = None
             self.__app = runner.get_application(db=self.__db,
                                                 wstl_builder_factory=wstl.builder_factory(package=service.__package__,
-                                                                                          href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/'))
+                                                                                          href='http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/'))
             return super().run(result)
 
     async def test_get_deleted_item_not_found(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C1') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C1') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_get_deleted_item_bucket_not_found(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_get_deleted_item_volume_not_found(self):
-        async with self.client.get(f'/volumes/1/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
+        async with self.client.get(f'/volumes/1/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_get_deleted_item_status(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             self.assertEqual(200, resp.status)
 
     async def test_get_deleted_item(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             actual = [{'collection': {'version': '1.0',
-                                      'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}',
+                                      'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}',
                                       'items': [
                                         {'data': [
                                             {'name': 'actual_object_id', 'value': 'VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_id', 'display': True},
                                             {'name': 'actual_object_type_name', 'value': 'heaobject.data.AWSS3FileObject', 'prompt': 'actual_object_type_name', 'display': True},
                                             {'name': 'actual_object_uri', 'value': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_uri', 'display': True},
                                             {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                             {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True}, {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
@@ -97,17 +97,17 @@
                                             {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                             {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                             {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
-                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
-                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
-                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'},
+                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
+                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
+                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'},
                                             {'prompt': 'View volume', 'rel': 'hea-volume', 'href': 'http://localhost:8080/volumes/666f6f2d6261722d71757578'},
                                             {'prompt': 'View account', 'rel': 'hea-account', 'href': 'http://localhost:8080/volumes/666f6f2d6261722d71757578/awsaccounts/me'}]}],
                                       'template': {'prompt': 'Properties', 'rel': 'hea-properties hea-context-menu',
                                                    'data': [
                                                         {'name': 'id', 'value': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', 'prompt': 'Id', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'display_name', 'value': 'TextFileUTF8.txt', 'prompt': 'Name', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'Original location', 'required': False, 'readOnly': True, 'pattern': None},
@@ -123,15 +123,15 @@
                                                         {'name': 'modified', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                                         {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
                                                         {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(_ordered(actual), _ordered(await resp.json()))
 
     async def test_get_deleted_item_nvpjson(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
             actual = [{'actual_object_id': 'VGV4dEZpbGVVVEY4LnR4dA==',
                        'actual_object_type_name':
                        'heaobject.data.AWSS3FileObject',
                        'actual_object_uri': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/VGV4dEZpbGVVVEY4LnR4dA==',
                        'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
                        'created': '2022-05-17T00:00:00+00:00',
                        'derived_by': None,
@@ -154,19 +154,19 @@
                        'storage_class': 'STANDARD',
                        'type': 'heaobject.trash.AWSS3FolderFileTrashItem',
                        'version': self.__version1,
                        'volume_id': '666f6f2d6261722d71757578'}]
             self.assertEqual(actual, await resp.json())
 
     async def test_get_deleted_items_status(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash') as resp:
             self.assertEqual(200, resp.status)
 
     async def test_get_deleted_items_nvpjson(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
             actual = [{'actual_object_id': 'VGV4dEZpbGVVVEY4LnR4dA==',
                        'actual_object_type_name':
                        'heaobject.data.AWSS3FileObject',
                        'actual_object_uri': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/VGV4dEZpbGVVVEY4LnR4dA==',
                        'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
                        'created': '2022-05-17T00:00:00+00:00',
                        'derived_by': None,
@@ -214,17 +214,17 @@
                        'storage_class': 'STANDARD',
                        'type': 'heaobject.trash.AWSS3FolderFileTrashItem',
                        'version': self.__version2,
                        'volume_id': '666f6f2d6261722d71757578'}]
             self.assertEqual(actual, await resp.json())
 
     async def test_get_deleted_items(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash') as resp:
             actual = [{'collection': {'version': '1.0',
-                                      'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash',
+                                      'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash',
                                       'items': [
                                           {'data': [
                                               {'name': 'actual_object_id', 'value': 'VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_id', 'display': True},
                                               {'name': 'actual_object_type_name', 'value': 'heaobject.data.AWSS3FileObject', 'prompt': 'actual_object_type_name', 'display': True},
                                               {'name': 'actual_object_uri', 'value': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_uri', 'display': True},
                                               {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                               {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
@@ -246,17 +246,17 @@
                                               {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                               {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                               {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                               {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                               {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                               {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                            'links': [
-                                              {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
-                                              {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
-                                              {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
+                                              {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
+                                              {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
+                                              {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
                                             {'data': [
                                               {'name': 'actual_object_id', 'value': 'YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU=', 'prompt': 'actual_object_id', 'display': True},
                                               {'name': 'actual_object_type_name', 'value': 'heaobject.data.AWSS3FileObject', 'prompt': 'actual_object_type_name',  'display': True},
                                               {'name': 'actual_object_uri', 'value': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU=', 'prompt': 'actual_object_uri', 'display': True},
                                               {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                               {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
                                               {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
@@ -275,17 +275,17 @@
                                               {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/afolder/anotherfolder/BinaryFile', 'prompt': 's3_uri', 'display': True},
                                               {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True}, {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                               {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True}, {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                               {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                               {'name': 'version', 'value': self.__version2, 'prompt': 'version', 'display': True},
                                               {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                             'links': [
-                                              {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}/restorer'},
-                                              {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}/deleter'},
-                                              {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}'}]}],
+                                              {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}/restorer'},
+                                              {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}/deleter'},
+                                              {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}'}]}],
                                       'template': {
                                         'prompt': 'Properties',
                                         'rel': 'hea-properties hea-context-menu',
                                         'data': [
                                             {'name': 'id', 'value': None, 'prompt': 'Id', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'display_name', 'value': None, 'prompt': 'Name', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'original_location', 'value': None, 'prompt': 'Original location', 'required': False, 'readOnly': True, 'pattern': None},
@@ -301,33 +301,33 @@
                                             {'name': 'modified', 'value': None, 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'source', 'value': None, 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(_ordered(actual), _ordered(await resp.json()))
 
     async def test_get_deleted_items_invalid_folder_id(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/toor/trash') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/toor/awss3trash') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_get_deleted_items_bucket_not_found(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags/awss3folders/root/trash') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags/awss3folders/root/awss3trash') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_get_deleted_items_volume_not_found(self):
-        async with self.client.get('/volumes/1/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/trash') as resp:
+        async with self.client.get('/volumes/1/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/awss3trash') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_get_deleted_items_folder_status(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/trash') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/awss3trash') as resp:
             self.assertEqual(200, resp.status)
 
     async def test_get_deleted_items_folder(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/trash') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/awss3trash') as resp:
             actual = [{'collection': {'version': '1.0',
-                                      'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/trash',
+                                      'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/awss3trash',
                                       'items': [
                                         {'data': [
                                             {'name': 'actual_object_id', 'value': 'VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_id', 'display': True},
                                             {'name': 'actual_object_type_name', 'value': 'heaobject.data.AWSS3FileObject', 'prompt': 'actual_object_type_name', 'display': True},
                                             {'name': 'actual_object_uri', 'value': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_uri', 'display': True},
                                             {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                             {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
@@ -347,17 +347,17 @@
                                             {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True}, {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                             {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                             {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
-                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
-                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
-                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
+                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
+                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
+                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
                                         {'data': [
                                             {'name': 'actual_object_id', 'value': 'YWZvbGRlci8=', 'prompt': 'actual_object_id', 'display': True},
                                             {'name': 'actual_object_type_name', 'value': 'heaobject.folder.AWSS3Folder', 'prompt': 'actual_object_type_name', 'display': True},
                                             {'name': 'actual_object_uri', 'value': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/YWZvbGRlci8=', 'prompt': 'actual_object_uri', 'display': True},
                                             {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                             {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
                                             {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
@@ -378,18 +378,18 @@
                                             {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                             {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                             {'name': 'version', 'value': self.__version2, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
-                                            {'prompt': 'Open', 'rel': 'hea-opener-choices hea-context-menu', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci8%3D%2C{self.__version2}/opener'},
-                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci8%3D%2C{self.__version2}/restorer'},
-                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci8%3D%2C{self.__version2}/deleter'},
-                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci8%3D%2C{self.__version2}'}]}],
+                                            {'prompt': 'Open', 'rel': 'hea-opener-choices hea-context-menu', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/opener'},
+                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/restorer'},
+                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/deleter'},
+                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}'}]}],
                                         'template': {'prompt': 'Properties', 'rel': 'hea-properties hea-context-menu',
                                           'data': [
                                             {'name': 'id', 'value': None, 'prompt': 'Id', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'display_name', 'value': None, 'prompt': 'Name', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'original_location', 'value': None, 'prompt': 'Original location', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'type', 'value': None, 'prompt': 'Type', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'description', 'value': None, 'prompt': 'Description', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'textarea'},
@@ -403,29 +403,29 @@
                                             {'name': 'modified', 'value': None, 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'source', 'value': None, 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(actual, await resp.json())
 
     async def test_get_deleted_items_invalid_trash_folder(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trashfolders/toor/items') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashfolders/toor/items') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_get_deleted_items_bucket_not_found_trash_folder(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags/trashfolders/root/items') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags/awss3trashfolders/root/items') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_get_deleted_items_volume_not_found_trash_folder(self):
-        async with self.client.get('/volumes/1/buckets/arp-scale-2-cloud-bucket-with-tags11/trashfolders/root/items') as resp:
+        async with self.client.get('/volumes/1/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashfolders/root/items') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_get_deleted_items_trash_folder(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trashfolders/root/items') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashfolders/root/items') as resp:
             actual = [{'collection': {'version': '1.0',
-                                      'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trashfolders/root/items',
+                                      'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashfolders/root/items',
                                       'items': [
                                         {'data': [
                                             {'name': 'actual_object_id', 'value': 'VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_id', 'display': True},
                                             {'name': 'actual_object_type_name', 'value': 'heaobject.data.AWSS3FileObject', 'prompt': 'actual_object_type_name', 'display': True},
                                             {'name': 'actual_object_uri', 'value': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_uri', 'display': True},
                                             {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                             {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
@@ -445,17 +445,17 @@
                                             {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True}, {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                             {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                             {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
-                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
-                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
-                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
+                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
+                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
+                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
                                         {'data': [
                                             {'name': 'actual_object_id', 'value': 'YWZvbGRlci8=', 'prompt': 'actual_object_id', 'display': True},
                                             {'name': 'actual_object_type_name', 'value': 'heaobject.folder.AWSS3Folder', 'prompt': 'actual_object_type_name', 'display': True},
                                             {'name': 'actual_object_uri', 'value': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/YWZvbGRlci8=', 'prompt': 'actual_object_uri', 'display': True},
                                             {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                             {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
                                             {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
@@ -476,18 +476,18 @@
                                             {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                             {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                             {'name': 'version', 'value': self.__version2, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
-                                            {'prompt': 'Open', 'rel': 'hea-opener-choices hea-context-menu', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci8%3D%2C{self.__version2}/opener'},
-                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci8%3D%2C{self.__version2}/restorer'},
-                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci8%3D%2C{self.__version2}/deleter'},
-                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/YWZvbGRlci8%3D%2C{self.__version2}'}]}],
+                                            {'prompt': 'Open', 'rel': 'hea-opener-choices hea-context-menu', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/opener'},
+                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/restorer'},
+                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/deleter'},
+                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}'}]}],
                                         'template': {'prompt': 'Properties', 'rel': 'hea-properties hea-context-menu',
                                           'data': [
                                             {'name': 'id', 'value': None, 'prompt': 'Id', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'display_name', 'value': None, 'prompt': 'Name', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'original_location', 'value': None, 'prompt': 'Original location', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'type', 'value': None, 'prompt': 'Type', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'description', 'value': None, 'prompt': 'Description', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'textarea'},
@@ -501,81 +501,81 @@
                                             {'name': 'modified', 'value': None, 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'source', 'value': None, 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(actual, await resp.json())
 
     async def test_do_empty_trash_status(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trashemptier') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashemptier') as resp:
             self.assertEqual(204, resp.status)
 
     async def test_do_empty_trash(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trashemptier') as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashemptier') as resp:
             if resp.status != 204:
                 self.fail(f'Trash emptier responded with wrong status code {resp.status}')
 
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
             self.assertEqual([], await resp.json())
 
     async def test_permanently_delete_item_status(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/deleter') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/deleter') as resp:
             self.assertEqual(204, resp.status)
 
     async def test_permanently_delete_item(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/deleter') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/deleter') as resp:
             if resp.status != 204:
                 self.fail(f'Permanent delete failed for item VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1} with status code {resp.status}')
 
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_permanently_delete_item_status_delete(self):
-        async with self.client.delete(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
+        async with self.client.delete(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             self.assertEqual(204, resp.status)
 
     async def test_permanently_delete_item_delete(self):
-        async with self.client.delete(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
+        async with self.client.delete(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             if resp.status != 204:
                 self.fail(f'Permanent delete failed for item VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1} with status code {resp.status}')
 
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_restore_status(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/restorer') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/restorer') as resp:
             self.assertEqual(204, resp.status)
 
     async def test_restore_check_trash_item(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/restorer') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/restorer') as resp:
             if resp.status != 204:
                 self.fail(f'Restore of item VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1} failed with status code {resp.status}')
 
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_restore_check_trash_item_count(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/restorer', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/restorer', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
             if resp.status != 204:
                 self.fail(f'Restore of item VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1} failed with status code {resp.status}')
 
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/') as resp:
             self.assertEqual(1, len(await resp.json()))
 
     async def test_restore_check_bucket(self):
-        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/restorer') as resp:
+        async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}/restorer') as resp:
             if resp.status != 204:
                 self.fail(f'Restore of item VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1} failed with status code {resp.status}')
 
         s3 = boto3.client('s3')
         from heaserver.service.db import awsservicelib
         async for obj in awsservicelib.list_objects(s3, bucket_id='arp-scale-2-cloud-bucket-with-tags11'):
             if obj['Key'] == 'TextFileUTF8.txt':
                 break
         else:
             self.fail('Object TextFileUTF8.txt not restored')
 
     async def test_trash_item_count(self):
-        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/trash/', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
+        async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
             self.assertEqual(2, len(await resp.json()))
 
     async def get_application(self) -> Application:
         return self.__app
```

### Comparing `heaserver-trash-aws-s3-1.0.0a1/tests/heaserver/trashawss3test/testcase.py` & `heaserver-trash-aws-s3-1.0.0a2/tests/heaserver/trashawss3test/testcase.py`

 * *Files identical despite different names*


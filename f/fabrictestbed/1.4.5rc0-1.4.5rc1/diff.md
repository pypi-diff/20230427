# Comparing `tmp/fabrictestbed-1.4.5rc0.tar.gz` & `tmp/fabrictestbed-1.4.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.4.5rc0.tar", last modified: Thu Apr 27 13:34:00 2023, max compression
+gzip compressed data, was "fabrictestbed-1.4.5rc1.tar", last modified: Thu Apr 27 13:42:19 2023, max compression
```

## Comparing `fabrictestbed-1.4.5rc0.tar` & `fabrictestbed-1.4.5rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:34:00.658338 fabrictestbed-1.4.5rc0/
--rw-r--r--   0 kthare10   (503) staff       (20)     1071 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/LICENSE
--rw-r--r--   0 kthare10   (503) staff       (20)       24 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/MANIFEST.in
--rw-r--r--   0 kthare10   (503) staff       (20)     6101 2023-04-27 13:34:00.657927 fabrictestbed-1.4.5rc0/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     5603 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/README.md
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:34:00.650450 fabrictestbed-1.4.5rc0/fabrictestbed/
--rw-r--r--   0 kthare10   (503) staff       (20)       25 2023-04-27 13:33:26.000000 fabrictestbed-1.4.5rc0/fabrictestbed/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:34:00.654379 fabrictestbed-1.4.5rc0/fabrictestbed/cli/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/fabrictestbed/cli/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)    18087 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/fabrictestbed/cli/cli.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1452 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/fabrictestbed/cli/exceptions.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:34:00.654814 fabrictestbed-1.4.5rc0/fabrictestbed/slice_editor/
--rw-r--r--   0 kthare10   (503) staff       (20)     1914 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/fabrictestbed/slice_editor/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:34:00.655750 fabrictestbed-1.4.5rc0/fabrictestbed/slice_manager/
--rw-r--r--   0 kthare10   (503) staff       (20)      201 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)    18177 2023-04-27 13:30:34.000000 fabrictestbed-1.4.5rc0/fabrictestbed/slice_manager/slice_manager.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:34:00.656577 fabrictestbed-1.4.5rc0/fabrictestbed/util/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/fabrictestbed/util/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1452 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/fabrictestbed/util/constants.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:34:00.652975 fabrictestbed-1.4.5rc0/fabrictestbed.egg-info/
--rw-r--r--   0 kthare10   (503) staff       (20)     6101 2023-04-27 13:34:00.000000 fabrictestbed-1.4.5rc0/fabrictestbed.egg-info/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)      613 2023-04-27 13:34:00.000000 fabrictestbed-1.4.5rc0/fabrictestbed.egg-info/SOURCES.txt
--rw-r--r--   0 kthare10   (503) staff       (20)        1 2023-04-27 13:34:00.000000 fabrictestbed-1.4.5rc0/fabrictestbed.egg-info/dependency_links.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       57 2023-04-27 13:34:00.000000 fabrictestbed-1.4.5rc0/fabrictestbed.egg-info/entry_points.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       96 2023-04-27 13:34:00.000000 fabrictestbed-1.4.5rc0/fabrictestbed.egg-info/requires.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       19 2023-04-27 13:34:00.000000 fabrictestbed-1.4.5rc0/fabrictestbed.egg-info/top_level.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       81 2023-04-27 13:33:43.000000 fabrictestbed-1.4.5rc0/requirements.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       38 2023-04-27 13:34:00.658471 fabrictestbed-1.4.5rc0/setup.cfg
--rw-r--r--   0 kthare10   (503) staff       (20)     1071 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/setup.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:34:00.657348 fabrictestbed-1.4.5rc0/test/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/test/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2210 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc0/test/test_cli.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:42:19.241974 fabrictestbed-1.4.5rc1/
+-rw-r--r--   0 kthare10   (503) staff       (20)     1071 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/LICENSE
+-rw-r--r--   0 kthare10   (503) staff       (20)       24 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/MANIFEST.in
+-rw-r--r--   0 kthare10   (503) staff       (20)     6101 2023-04-27 13:42:19.241563 fabrictestbed-1.4.5rc1/PKG-INFO
+-rw-r--r--   0 kthare10   (503) staff       (20)     5603 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/README.md
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:42:19.233358 fabrictestbed-1.4.5rc1/fabrictestbed/
+-rw-r--r--   0 kthare10   (503) staff       (20)       25 2023-04-27 13:42:13.000000 fabrictestbed-1.4.5rc1/fabrictestbed/__init__.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:42:19.237466 fabrictestbed-1.4.5rc1/fabrictestbed/cli/
+-rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/fabrictestbed/cli/__init__.py
+-rw-r--r--   0 kthare10   (503) staff       (20)    18087 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/fabrictestbed/cli/cli.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1452 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/fabrictestbed/cli/exceptions.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:42:19.237892 fabrictestbed-1.4.5rc1/fabrictestbed/slice_editor/
+-rw-r--r--   0 kthare10   (503) staff       (20)     1914 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/fabrictestbed/slice_editor/__init__.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:42:19.239181 fabrictestbed-1.4.5rc1/fabrictestbed/slice_manager/
+-rw-r--r--   0 kthare10   (503) staff       (20)      201 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0 kthare10   (503) staff       (20)    18250 2023-04-27 13:41:41.000000 fabrictestbed-1.4.5rc1/fabrictestbed/slice_manager/slice_manager.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:42:19.240149 fabrictestbed-1.4.5rc1/fabrictestbed/util/
+-rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/fabrictestbed/util/__init__.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1452 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/fabrictestbed/util/constants.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:42:19.235756 fabrictestbed-1.4.5rc1/fabrictestbed.egg-info/
+-rw-r--r--   0 kthare10   (503) staff       (20)     6101 2023-04-27 13:42:19.000000 fabrictestbed-1.4.5rc1/fabrictestbed.egg-info/PKG-INFO
+-rw-r--r--   0 kthare10   (503) staff       (20)      613 2023-04-27 13:42:19.000000 fabrictestbed-1.4.5rc1/fabrictestbed.egg-info/SOURCES.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)        1 2023-04-27 13:42:19.000000 fabrictestbed-1.4.5rc1/fabrictestbed.egg-info/dependency_links.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)       57 2023-04-27 13:42:19.000000 fabrictestbed-1.4.5rc1/fabrictestbed.egg-info/entry_points.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)       96 2023-04-27 13:42:19.000000 fabrictestbed-1.4.5rc1/fabrictestbed.egg-info/requires.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)       19 2023-04-27 13:42:19.000000 fabrictestbed-1.4.5rc1/fabrictestbed.egg-info/top_level.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)       81 2023-04-27 13:33:43.000000 fabrictestbed-1.4.5rc1/requirements.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)       38 2023-04-27 13:42:19.242104 fabrictestbed-1.4.5rc1/setup.cfg
+-rw-r--r--   0 kthare10   (503) staff       (20)     1071 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/setup.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:42:19.241025 fabrictestbed-1.4.5rc1/test/
+-rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/test/__init__.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     2210 2023-04-26 16:15:21.000000 fabrictestbed-1.4.5rc1/test/test_cli.py
```

### Comparing `fabrictestbed-1.4.5rc0/LICENSE` & `fabrictestbed-1.4.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc0/PKG-INFO` & `fabrictestbed-1.4.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.4.5rc0
+Version: 1.4.5rc1
 Summary: FABRIC Python Client Library with CLI
 Home-page: https://github.com/fabric-testbed/fabric-cli
 Author: Erica Fu, Komal Thareja
 Author-email: ericafu@renci.org, kthare10@unc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fabrictestbed-1.4.5rc0/README.md` & `fabrictestbed-1.4.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc0/fabrictestbed/cli/cli.py` & `fabrictestbed-1.4.5rc1/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc0/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.4.5rc1/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc0/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.4.5rc1/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc0/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.4.5rc1/fabrictestbed/slice_manager/slice_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,27 +252,28 @@
         if slice_id is None or not isinstance(slice_id, str):
             return Status.INVALID_ARGUMENTS, SliceManagerException("Invalid arguments - slice_id")
 
         if self.__should_renew():
             self.__load_tokens()
         return self.oc_proxy.modify_accept(token=self.get_id_token(), slice_id=slice_id)
 
-    def delete(self, *, slice_object: Slice, email: str = None) -> Tuple[Status, Union[Exception, None]]:
+    def delete(self, *, slice_object: Slice = None, email: str = None) -> Tuple[Status, Union[Exception, None]]:
         """
         Delete slice(s)
         @param slice_object slice to be deleted
         @param email user's email
         @return Tuple containing Status and Exception/Json containing deletion status
         """
         if email is None and (slice_object is None or not isinstance(slice_object, Slice)):
             return Status.INVALID_ARGUMENTS, SliceManagerException(f"Invalid arguments - "
                                                                    f"slice_object: {slice_object}/email: {email}")
         if self.__should_renew():
             self.__load_tokens()
-        return self.oc_proxy.delete(token=self.get_id_token(), slice_id=slice_object.slice_id, email=email)
+        slice_id = slice_object.slice_id if slice_object is not None else None
+        return self.oc_proxy.delete(token=self.get_id_token(), slice_id=slice_id, email=email)
 
     def slices(self, includes: List[SliceState] = None, excludes: List[SliceState] = None, name: str = None,
                limit: int = 20, offset: int = 0, slice_id: str = None) -> Tuple[Status, Union[Exception, List[Slice]]]:
         """
         Get slices
         @param includes list of the slice state used to include the slices in the output
         @param excludes list of the slice state used to exclude the slices from the output
```

### Comparing `fabrictestbed-1.4.5rc0/fabrictestbed/util/constants.py` & `fabrictestbed-1.4.5rc1/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc0/fabrictestbed.egg-info/PKG-INFO` & `fabrictestbed-1.4.5rc1/fabrictestbed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.4.5rc0
+Version: 1.4.5rc1
 Summary: FABRIC Python Client Library with CLI
 Home-page: https://github.com/fabric-testbed/fabric-cli
 Author: Erica Fu, Komal Thareja
 Author-email: ericafu@renci.org, kthare10@unc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fabrictestbed-1.4.5rc0/fabrictestbed.egg-info/SOURCES.txt` & `fabrictestbed-1.4.5rc1/fabrictestbed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc0/setup.py` & `fabrictestbed-1.4.5rc1/setup.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc0/test/test_cli.py` & `fabrictestbed-1.4.5rc1/test/test_cli.py`

 * *Files identical despite different names*


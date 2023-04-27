# Comparing `tmp/adlfs-2023.1.0.tar.gz` & `tmp/adlfs-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adlfs-2023.1.0.tar", last modified: Tue Jan 17 11:14:49 2023, max compression
+gzip compressed data, was "adlfs-2023.4.0.tar", last modified: Thu Apr 27 14:58:13 2023, max compression
```

## Comparing `adlfs-2023.1.0.tar` & `adlfs-2023.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 11:14:49.212203 adlfs-2023.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-01-17 11:14:38.000000 adlfs-2023.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-01-17 11:14:38.000000 adlfs-2023.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6531 2023-01-17 11:14:49.212203 adlfs-2023.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5871 2023-01-17 11:14:38.000000 adlfs-2023.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 11:14:49.212203 adlfs-2023.1.0/adlfs/
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-01-17 11:14:38.000000 adlfs-2023.1.0/adlfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-01-17 11:14:49.212203 adlfs-2023.1.0/adlfs/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     7629 2023-01-17 11:14:38.000000 adlfs-2023.1.0/adlfs/gen1.py
--rw-r--r--   0 runner    (1001) docker     (122)    74957 2023-01-17 11:14:38.000000 adlfs-2023.1.0/adlfs/spec.py
--rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-01-17 11:14:38.000000 adlfs-2023.1.0/adlfs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 11:14:49.212203 adlfs-2023.1.0/adlfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6531 2023-01-17 11:14:49.000000 adlfs-2023.1.0/adlfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-01-17 11:14:49.000000 adlfs-2023.1.0/adlfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 11:14:49.000000 adlfs-2023.1.0/adlfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-01-17 11:14:49.000000 adlfs-2023.1.0/adlfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 11:14:48.000000 adlfs-2023.1.0/adlfs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-01-17 11:14:49.000000 adlfs-2023.1.0/adlfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 11:14:49.000000 adlfs-2023.1.0/adlfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-01-17 11:14:38.000000 adlfs-2023.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-01-17 11:14:49.212203 adlfs-2023.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1481 2023-01-17 11:14:38.000000 adlfs-2023.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    68739 2023-01-17 11:14:38.000000 adlfs-2023.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:58:13.066924 adlfs-2023.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-04-27 14:57:56.000000 adlfs-2023.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-27 14:57:56.000000 adlfs-2023.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6531 2023-04-27 14:58:13.066924 adlfs-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5871 2023-04-27 14:57:56.000000 adlfs-2023.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:58:13.066924 adlfs-2023.4.0/adlfs/
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-04-27 14:57:56.000000 adlfs-2023.4.0/adlfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-04-27 14:58:13.066924 adlfs-2023.4.0/adlfs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7629 2023-04-27 14:57:56.000000 adlfs-2023.4.0/adlfs/gen1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74343 2023-04-27 14:57:56.000000 adlfs-2023.4.0/adlfs/spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-04-27 14:57:56.000000 adlfs-2023.4.0/adlfs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 14:58:13.066924 adlfs-2023.4.0/adlfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6531 2023-04-27 14:58:13.000000 adlfs-2023.4.0/adlfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-27 14:58:13.000000 adlfs-2023.4.0/adlfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 14:58:13.000000 adlfs-2023.4.0/adlfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-27 14:58:13.000000 adlfs-2023.4.0/adlfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 14:58:12.000000 adlfs-2023.4.0/adlfs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-27 14:58:13.000000 adlfs-2023.4.0/adlfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-27 14:58:13.000000 adlfs-2023.4.0/adlfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-27 14:57:56.000000 adlfs-2023.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-27 14:58:13.066924 adlfs-2023.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1481 2023-04-27 14:57:56.000000 adlfs-2023.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    68739 2023-04-27 14:57:56.000000 adlfs-2023.4.0/versioneer.py
```

### Comparing `adlfs-2023.1.0/LICENSE.txt` & `adlfs-2023.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adlfs-2023.1.0/PKG-INFO` & `adlfs-2023.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adlfs
-Version: 2023.1.0
+Version: 2023.4.0
 Summary: Access Azure Datalake Gen1 with fsspec and dask
 Home-page: https://github.com/dask/adlfs/
 Maintainer: Greg Hayes
 Maintainer-email: hayesgb@gmail.com
 License: BSD
 Keywords: file-system,dask,azure
 Classifier: Intended Audience :: Developers
```

### Comparing `adlfs-2023.1.0/README.md` & `adlfs-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `adlfs-2023.1.0/adlfs/gen1.py` & `adlfs-2023.4.0/adlfs/gen1.py`

 * *Files identical despite different names*

### Comparing `adlfs-2023.1.0/adlfs/spec.py` & `adlfs-2023.4.0/adlfs/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 
 from __future__ import absolute_import, division, print_function
 
 import asyncio
+import errno
 import io
 import logging
 import os
 import re
 import warnings
 import weakref
 from collections import defaultdict
@@ -493,29 +494,14 @@
         key, _, version_id = keypart.partition("?versionid=")
         return (
             container,
             key,
             version_id if self.version_aware and version_id else None,
         )
 
-    def info(self, path, refresh=False, **kwargs):
-        try:
-            fetch_from_azure = (path and self._ls_from_cache(path) is None) or refresh
-        except Exception:
-            fetch_from_azure = True
-        if fetch_from_azure:
-            return sync(
-                self.loop,
-                self._info,
-                path,
-                refresh,
-                version_id=kwargs.get("version_id"),
-            )
-        return super().info(path)
-
     def modified(self, path: str) -> datetime:
         return self.info(path)["last_modified"]
 
     def created(self, path: str) -> datetime:
         return self.info(path)["creation_time"]
 
     async def _info(self, path, refresh=False, **kwargs):
@@ -527,52 +513,68 @@
         Some file systems might not be able to measure the file's size, in
         which case, the returned dict will include ``'size': None``.
         Returns
         -------
         dict with keys: name (full path in the FS), size (in bytes), type (file,
         directory, or something else) and other FS-specific keys.
         """
-        if refresh:
-            invalidate_cache = True
-        else:
-            invalidate_cache = False
         container, path, path_version_id = self.split_path(path)
         fullpath = "/".join([container, path]) if path else container
         version_id = _coalesce_version_id(path_version_id, kwargs.get("version_id"))
         kwargs["version_id"] = version_id
 
-        out = await self._ls(
-            fullpath, detail=True, invalidate_cache=invalidate_cache, **kwargs
-        )
-        fullpath = fullpath.rstrip("/")
-        out1 = [
-            o
-            for o in out
-            if o["name"].rstrip("/") == fullpath
-            and (version_id is None or o["version_id"] == version_id)
-        ]
-        if len(out1) == 1:
-            if "size" not in out1[0]:
-                out1[0]["size"] = None
-            return out1[0]
-        elif len(out1) > 1 or out:
-            return {"name": fullpath, "size": None, "type": "directory"}
-        else:
-            # Check the directory listing as the path may have been deleted
-            out = await self._ls(
-                self._parent(path),
-                detail=True,
-                invalidate_cache=invalidate_cache,
-                **kwargs,
-            )
-            out = [o for o in out if o["name"].rstrip("/") == path]
-            if out:
-                return out[0]
-            else:
-                raise FileNotFoundError
+        if fullpath == "":
+            return {"name": "", "size": None, "type": "directory"}
+        elif path == "":
+            if not refresh and _ROOT_PATH in self.dircache:
+                out = [o for o in self.dircache[_ROOT_PATH] if o["name"] == container]
+                if out:
+                    return out[0]
+            try:
+                async with self.service_client.get_container_client(
+                    container=container
+                ) as cc:
+                    properties = await cc.get_container_properties()
+            except ResourceNotFoundError as exc:
+                raise FileNotFoundError from exc
+            info = (await self._details([properties]))[0]
+            # Make result consistent with _ls_containers()
+            if not info.get("metadata"):
+                info["metadata"] = None
+            return info
+
+        if not refresh:
+            out = self._ls_from_cache(fullpath)
+            if out is not None:
+                if self.version_aware and version_id is not None:
+                    out = [
+                        o
+                        for o in out
+                        if o["name"] == fullpath and match_blob_version(o, version_id)
+                    ]
+                    if out:
+                        return out[0]
+                else:
+                    out = [o for o in out if o["name"] == fullpath]
+                    if out:
+                        return out[0]
+                    return {"name": fullpath, "size": None, "type": "directory"}
+
+        try:
+            async with self.service_client.get_blob_client(container, path) as bc:
+                props = await bc.get_blob_properties(version_id=version_id)
+            return (await self._details([props]))[0]
+        except ResourceNotFoundError:
+            pass
+
+        if not version_id:
+            if await self._dir_exists(container, path):
+                return {"name": fullpath, "size": None, "type": "directory"}
+
+        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), fullpath)
 
     def glob(self, path, **kwargs):
         return sync(self.loop, self._glob, path)
 
     async def _glob(self, path, **kwargs):
         """
         Find files by glob-matching.
@@ -675,95 +677,86 @@
         if (version_id or versions) and not self.version_aware:
             raise ValueError(
                 "version_id/versions cannot be specified if the filesystem "
                 "is not version aware"
             )
 
         if (
-            target_path not in self.dircache
-            or return_glob
-            or versions
-            or not any(
+            target_path in self.dircache
+            and not return_glob
+            and not versions
+            and all(
                 match_blob_version(b, version_id) for b in self.dircache[target_path]
             )
         ):
-            if container not in ["", delimiter]:
-                # This is the case where the container name is passed
-                async with self.service_client.get_container_client(
-                    container=container
-                ) as cc:
-                    path = path.strip("/")
-                    include = ["metadata"]
-                    if version_id is not None or versions:
-                        assert self.version_aware
-                        include.append("versions")
-                    blobs = cc.walk_blobs(include=include, name_starts_with=path)
-
-                # Check the depth that needs to be screened
-                depth = target_path.count("/")
-                outblobs = []
-                try:
-                    async for next_blob in blobs:
-                        if depth in [0, 1] and path == "":
-                            outblobs.append(next_blob)
-                        elif isinstance(next_blob, BlobProperties):
-                            if next_blob["name"].count("/") == depth:
-                                outblobs.append(next_blob)
-                            elif not next_blob["name"].endswith("/") and (
-                                next_blob["name"].count("/") == (depth - 1)
-                            ):
-                                outblobs.append(next_blob)
-                        else:
-                            async for blob_ in next_blob:
-                                if isinstance(blob_, BlobProperties) or isinstance(
-                                    blob_, BlobPrefix
+            return self.dircache[target_path]
+
+        assert container not in ["", delimiter]
+        async with self.service_client.get_container_client(container=container) as cc:
+            path = path.strip("/")
+            include = ["metadata"]
+            if version_id is not None or versions:
+                assert self.version_aware
+                include.append("versions")
+            blobs = cc.walk_blobs(include=include, name_starts_with=path)
+
+        # Check the depth that needs to be screened
+        depth = target_path.count("/")
+        outblobs = []
+        try:
+            async for next_blob in blobs:
+                if depth in [0, 1] and path == "":
+                    outblobs.append(next_blob)
+                elif isinstance(next_blob, BlobProperties):
+                    if next_blob["name"].count("/") == depth:
+                        outblobs.append(next_blob)
+                    elif not next_blob["name"].endswith("/") and (
+                        next_blob["name"].count("/") == (depth - 1)
+                    ):
+                        outblobs.append(next_blob)
+                else:
+                    async for blob_ in next_blob:
+                        if isinstance(blob_, BlobProperties) or isinstance(
+                            blob_, BlobPrefix
+                        ):
+                            if blob_["name"].endswith("/"):
+                                if blob_["name"].rstrip("/").count("/") == depth:
+                                    outblobs.append(blob_)
+                                elif blob_["name"].count("/") == depth and (
+                                    hasattr(blob_, "size") and blob_["size"] == 0
                                 ):
-                                    if blob_["name"].endswith("/"):
-                                        if (
-                                            blob_["name"].rstrip("/").count("/")
-                                            == depth
-                                        ):
-                                            outblobs.append(blob_)
-                                        elif blob_["name"].count("/") == depth and (
-                                            hasattr(blob_, "size")
-                                            and blob_["size"] == 0
-                                        ):
-                                            outblobs.append(blob_)
-                                        else:
-                                            pass
-                                    elif blob_["name"].count("/") == (depth):
-                                        outblobs.append(blob_)
-                                    else:
-                                        pass
-                except ResourceNotFoundError:
-                    raise FileNotFoundError
-                finalblobs = await self._details(
-                    outblobs,
-                    target_path=target_path,
-                    return_glob=return_glob,
-                    version_id=version_id,
-                    versions=versions,
-                )
-                if return_glob:
-                    return finalblobs
-                finalblobs = await self._details(
-                    outblobs,
-                    target_path=target_path,
-                    version_id=version_id,
-                    versions=versions,
+                                    outblobs.append(blob_)
+                                else:
+                                    pass
+                            elif blob_["name"].count("/") == (depth):
+                                outblobs.append(blob_)
+                            else:
+                                pass
+        except ResourceNotFoundError:
+            raise FileNotFoundError(
+                errno.ENOENT, os.strerror(errno.ENOENT), target_path
+            )
+        finalblobs = await self._details(
+            outblobs,
+            target_path=target_path,
+            return_glob=return_glob,
+            version_id=version_id,
+            versions=versions,
+        )
+        if return_glob:
+            return finalblobs
+        if not finalblobs:
+            if not await self._exists(target_path):
+                raise FileNotFoundError(
+                    errno.ENOENT, os.strerror(errno.ENOENT), target_path
                 )
-                if not finalblobs:
-                    if not await self._exists(target_path):
-                        raise FileNotFoundError
-                    return []
-                if not self.version_aware or finalblobs[0].get("is_current_version"):
-                    self.dircache[target_path] = finalblobs
-                return finalblobs
-
-        return self.dircache[target_path]
+            return []
+        if not self.version_aware or finalblobs[0].get("is_current_version"):
+            self.dircache[target_path] = finalblobs
+        return finalblobs
 
     async def _ls(
         self,
         path: str,
         detail: bool = False,
         invalidate_cache: bool = False,
         delimiter: str = "/",
@@ -876,49 +869,37 @@
                     for key in VERSIONED_BLOB_PROPERTIES
                     if content.has_key(key)  # NOQA
                 )
             if content.has_key("container"):  # NOQA
                 fname = f"{content.container}{delimiter}{content.name}"
                 fname = fname.rstrip(delimiter)
                 if content.has_key("size"):  # NOQA
-                    data.update({"name": fname})
-                    data.update({"size": content.size})
-                    data.update({"type": "file"})
+                    data["name"] = fname
+                    data["size"] = content.size
+                    data["type"] = "file"
                 else:
-                    data.update({"name": fname})
-                    data.update({"size": None})
-                    data.update({"type": "directory"})
+                    data["name"] = fname
+                    data["size"] = None
+                    data["type"] = "directory"
             else:
                 fname = f"{content.name}"
-                data.update({"name": fname})
-                data.update({"size": None})
-                data.update({"type": "directory"})
-            if "metadata" in data.keys():
-                if data["metadata"] is not None:
-                    if (
-                        "is_directory" in data["metadata"].keys()
-                        and data["metadata"]["is_directory"] == "true"
-                    ):
-                        data.update({"type": "directory"})
-                        data.update({"size": None})
-                    elif (
-                        "is_directory" in data["metadata"].keys()
-                        and data["metadata"]["is_directory"] == "false"
-                    ):
-                        data.update({"type": "file"})
-                    elif (
-                        "hdi_isfolder" in data["metadata"].keys()
-                        and data["metadata"]["hdi_isfolder"] == "true"
-                    ):
-                        data.update({"type": "directory"})
-                        data.update({"size": None})
-                    else:
-                        pass
+                data["name"] = fname
+                data["size"] = None
+                data["type"] = "directory"
+            if data.get("metadata"):
+                if data["metadata"].get("is_directory") == "true":
+                    data["type"] = "directory"
+                    data["size"] = None
+                elif data["metadata"].get("is_directory") == "false":
+                    data["type"] = "file"
+                elif data["metadata"].get("hdi_isfolder") == "true":
+                    data["type"] = "directory"
+                    data["size"] = None
             if return_glob:
-                data.update({"name": data["name"].rstrip("/")})
+                data["name"] = data["name"].rstrip("/")
             output.append(data)
         if target_path:
             if (
                 len(output) == 1
                 and output[0]["type"] == "file"
                 and not self.version_aware
             ):
@@ -1409,34 +1390,42 @@
             try:
                 if await bc.exists(version_id=version_id):
                     return True
             except HttpResponseError:
                 if version_id is not None:
                     return False
                 raise
+        return await self._dir_exists(container_name, path)
 
+    async def _dir_exists(self, container, path):
         dir_path = path.rstrip("/") + "/"
-        async with self.service_client.get_container_client(
-            container=container_name
-        ) as container_client:
-            async for blob in container_client.list_blobs(
-                results_per_page=1, name_starts_with=dir_path
-            ):
-                return True
-            else:
-                return False
+        try:
+            async with self.service_client.get_container_client(
+                container=container
+            ) as container_client:
+                async for blob in container_client.list_blobs(
+                    results_per_page=1, name_starts_with=dir_path
+                ):
+                    return True
+                else:
+                    return False
+        except ResourceNotFoundError:
+            return False
 
     async def _pipe_file(self, path, value, overwrite=True, **kwargs):
         """Set the bytes of given file"""
         container_name, path, _ = self.split_path(path)
         async with self.service_client.get_blob_client(
             container=container_name, blob=path
         ) as bc:
             result = await bc.upload_blob(
-                data=value, overwrite=overwrite, metadata={"is_directory": "false"}
+                data=value,
+                overwrite=overwrite,
+                metadata={"is_directory": "false"},
+                **kwargs,
             )
         self.invalidate_cache(self._parent(path))
         return result
 
     pipe_file = sync_wrapper(_pipe_file)
 
     async def _cat_file(self, path, start=None, end=None, **kwargs):
@@ -1581,15 +1570,15 @@
                         # This is to verify that we don't miss files
                         fullpath = fullpath.rstrip("/")
                         if not await self._exists(fullpath):
                             continue
                     out.add(fullpath)
 
         if not out:
-            raise FileNotFoundError
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), path)
         return list(sorted(out))
 
     async def _put_file(
         self, lpath, rpath, delimiter="/", overwrite=False, callback=None, **kwargws
     ):
         """
         Copy single file to remote
@@ -1599,15 +1588,15 @@
         :param delimitier: Filepath delimiter
         :param overwrite: Boolean (False).  If True, overwrite the existing file present
         """
 
         container_name, path, _ = self.split_path(rpath, delimiter=delimiter)
 
         if os.path.isdir(lpath):
-            self.makedirs(rpath, exist_ok=True)
+            await self._mkdir(rpath)
         else:
             try:
                 with open(lpath, "rb") as f1:
                     async with self.service_client.get_blob_client(
                         container_name, path
                     ) as bc:
                         await bc.upload_blob(
```

### Comparing `adlfs-2023.1.0/adlfs/utils.py` & `adlfs-2023.4.0/adlfs/utils.py`

 * *Files identical despite different names*

### Comparing `adlfs-2023.1.0/adlfs.egg-info/PKG-INFO` & `adlfs-2023.4.0/adlfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adlfs
-Version: 2023.1.0
+Version: 2023.4.0
 Summary: Access Azure Datalake Gen1 with fsspec and dask
 Home-page: https://github.com/dask/adlfs/
 Maintainer: Greg Hayes
 Maintainer-email: hayesgb@gmail.com
 License: BSD
 Keywords: file-system,dask,azure
 Classifier: Intended Audience :: Developers
```

### Comparing `adlfs-2023.1.0/setup.py` & `adlfs-2023.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `adlfs-2023.1.0/versioneer.py` & `adlfs-2023.4.0/versioneer.py`

 * *Files identical despite different names*


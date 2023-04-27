# Comparing `tmp/podman-4.4.1.tar.gz` & `tmp/podman-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podman-4.4.1.tar", last modified: Tue Feb 21 20:42:19 2023, max compression
+gzip compressed data, was "podman-4.5.0.tar", last modified: Thu Apr 27 14:43:27 2023, max compression
```

## Comparing `podman-4.4.1.tar` & `podman-4.5.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-02-21 20:42:19.541442 podman-4.4.1/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    11357 2022-10-19 21:26:36.000000 podman-4.4.1/LICENSE
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2886 2023-02-21 20:42:19.541442 podman-4.4.1/PKG-INFO
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1745 2022-10-19 21:26:36.000000 podman-4.4.1/README.md
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-02-21 20:42:19.533442 podman-4.4.1/podman/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      277 2022-10-19 21:26:36.000000 podman-4.4.1/podman/__init__.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-02-21 20:42:19.537442 podman-4.4.1/podman/api/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1684 2022-10-19 21:26:36.000000 podman-4.4.1/podman/api/__init__.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1980 2022-10-19 21:26:36.000000 podman-4.4.1/podman/api/adapter_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      256 2022-10-19 21:26:36.000000 podman-4.4.1/podman/api/cached_property.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14670 2022-10-19 21:26:36.000000 podman-4.4.1/podman/api/client.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2918 2022-10-19 21:26:36.000000 podman-4.4.1/podman/api/http_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2935 2022-10-19 21:26:36.000000 podman-4.4.1/podman/api/parse_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     9974 2022-10-19 21:26:36.000000 podman-4.4.1/podman/api/ssh.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3845 2022-10-19 21:26:36.000000 podman-4.4.1/podman/api/tar_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)   109047 2023-02-09 13:04:40.000000 podman-4.4.1/podman/api/typing_extensions.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5976 2022-10-19 21:26:36.000000 podman-4.4.1/podman/api/uds.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8429 2022-10-19 21:26:36.000000 podman-4.4.1/podman/client.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-02-21 20:42:19.541442 podman-4.4.1/podman/domain/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)        0 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/__init__.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3474 2023-02-20 19:54:55.000000 podman-4.4.1/podman/domain/config.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    19416 2023-02-07 13:10:19.000000 podman-4.4.1/podman/domain/containers.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    30948 2023-02-20 19:54:49.000000 podman-4.4.1/podman/domain/containers_create.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5405 2023-02-07 13:10:19.000000 podman-4.4.1/podman/domain/containers_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3305 2023-02-07 13:10:19.000000 podman-4.4.1/podman/domain/containers_run.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/events.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3699 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/images.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8616 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/images_build.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14363 2023-02-09 13:04:40.000000 podman-4.4.1/podman/domain/images_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1697 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/ipam.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3968 2023-02-09 13:04:40.000000 podman-4.4.1/podman/domain/manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     7485 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/manifests.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4882 2023-02-09 13:04:40.000000 podman-4.4.1/podman/domain/networks.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     6920 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/networks_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3451 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/pods.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5465 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/pods_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2936 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/registry_data.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4026 2023-02-09 13:04:40.000000 podman-4.4.1/podman/domain/secrets.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2931 2022-10-19 21:26:36.000000 podman-4.4.1/podman/domain/system.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4969 2023-02-09 13:04:40.000000 podman-4.4.1/podman/domain/volumes.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-02-21 20:42:19.541442 podman-4.4.1/podman/errors/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2710 2022-10-19 21:26:36.000000 podman-4.4.1/podman/errors/__init__.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4045 2022-10-19 21:26:36.000000 podman-4.4.1/podman/errors/exceptions.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      894 2022-10-19 21:26:36.000000 podman-4.4.1/podman/tlsconfig.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)       82 2023-02-21 16:57:31.000000 podman-4.4.1/podman/version.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-02-21 20:42:19.534442 podman-4.4.1/podman.egg-info/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2886 2023-02-21 20:42:19.000000 podman-4.4.1/podman.egg-info/PKG-INFO
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1155 2023-02-21 20:42:19.000000 podman-4.4.1/podman.egg-info/SOURCES.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)        1 2023-02-21 20:42:19.000000 podman-4.4.1/podman.egg-info/dependency_links.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)       56 2023-02-21 20:42:19.000000 podman-4.4.1/podman.egg-info/requires.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)        7 2023-02-21 20:42:19.000000 podman-4.4.1/podman.egg-info/top_level.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      759 2023-02-20 19:54:55.000000 podman-4.4.1/pyproject.toml
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1310 2023-02-21 20:42:19.541442 podman-4.4.1/setup.cfg
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      611 2022-10-19 21:26:36.000000 podman-4.4.1/setup.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.561593 podman-4.5.0/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    11357 2022-10-19 21:26:36.000000 podman-4.5.0/LICENSE
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2884 2023-04-27 14:43:27.561593 podman-4.5.0/PKG-INFO
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1745 2022-10-19 21:26:36.000000 podman-4.5.0/README.md
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.557593 podman-4.5.0/podman/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      277 2022-10-19 21:26:36.000000 podman-4.5.0/podman/__init__.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.558593 podman-4.5.0/podman/api/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2023-04-27 13:32:41.000000 podman-4.5.0/podman/api/__init__.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1980 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/adapter_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      256 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/cached_property.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14670 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/client.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2918 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/http_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3270 2023-04-27 13:32:41.000000 podman-4.5.0/podman/api/parse_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     9974 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/ssh.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3845 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/tar_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)   109033 2023-04-27 13:32:41.000000 podman-4.5.0/podman/api/typing_extensions.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5976 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/uds.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8640 2023-04-27 13:32:41.000000 podman-4.5.0/podman/client.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.560593 podman-4.5.0/podman/domain/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)        0 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/__init__.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3720 2023-04-27 13:32:41.000000 podman-4.5.0/podman/domain/config.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    18880 2023-04-27 13:32:41.000000 podman-4.5.0/podman/domain/containers.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    31505 2023-04-27 13:32:41.000000 podman-4.5.0/podman/domain/containers_create.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5405 2023-02-07 13:10:19.000000 podman-4.5.0/podman/domain/containers_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3305 2023-02-07 13:10:19.000000 podman-4.5.0/podman/domain/containers_run.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/events.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3699 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/images.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8616 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/images_build.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14363 2023-02-09 13:04:40.000000 podman-4.5.0/podman/domain/images_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1697 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/ipam.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3968 2023-02-09 13:04:40.000000 podman-4.5.0/podman/domain/manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     7485 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/manifests.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4882 2023-02-09 13:04:40.000000 podman-4.5.0/podman/domain/networks.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     6920 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/networks_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3451 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/pods.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5465 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/pods_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2936 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/registry_data.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4026 2023-02-09 13:04:40.000000 podman-4.5.0/podman/domain/secrets.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2931 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/system.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4969 2023-02-09 13:04:40.000000 podman-4.5.0/podman/domain/volumes.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.560593 podman-4.5.0/podman/errors/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2710 2022-10-19 21:26:36.000000 podman-4.5.0/podman/errors/__init__.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4045 2022-10-19 21:26:36.000000 podman-4.5.0/podman/errors/exceptions.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      894 2022-10-19 21:26:36.000000 podman-4.5.0/podman/tlsconfig.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)       82 2023-04-27 13:33:53.000000 podman-4.5.0/podman/version.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.557593 podman-4.5.0/podman.egg-info/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2884 2023-04-27 14:43:27.000000 podman-4.5.0/podman.egg-info/PKG-INFO
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1155 2023-04-27 14:43:27.000000 podman-4.5.0/podman.egg-info/SOURCES.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)        1 2023-04-27 14:43:27.000000 podman-4.5.0/podman.egg-info/dependency_links.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)       84 2023-04-27 14:43:27.000000 podman-4.5.0/podman.egg-info/requires.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)        7 2023-04-27 14:43:27.000000 podman-4.5.0/podman.egg-info/top_level.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      662 2023-04-27 13:32:41.000000 podman-4.5.0/pyproject.toml
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1313 2023-04-27 14:43:27.561593 podman-4.5.0/setup.cfg
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      611 2022-10-19 21:26:36.000000 podman-4.5.0/setup.py
```

### Comparing `podman-4.4.1/LICENSE` & `podman-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/PKG-INFO` & `podman-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podman
-Version: 4.4.1
+Version: 4.5.0
 Summary: Bindings for Podman RESTful API
 Home-page: https://github.com/containers/podman-py
 Author: Brent Baude, Jhon Honce
 Author-email: jhonce@redhat.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/containers/podman-py/issues
 Project-URL: Libpod API, https://docs.podman.io/en/latest/_static/api.html
@@ -72,9 +72,7 @@
 
     print(json.dumps(client.df(), indent=4))
 ```
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/containers/podman-py/blob/main/CONTRIBUTING.md)
-
-
```

### Comparing `podman-4.4.1/README.md` & `podman-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/api/__init__.py` & `podman-4.5.0/podman/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from podman.api.parse_utils import (
     decode_header,
     frames,
     parse_repository,
     prepare_cidr,
     prepare_timestamp,
     stream_frames,
+    stream_helper,
 )
 from podman.api.tar_utils import create_tar, prepare_containerfile, prepare_containerignore
 from .. import version
 
 DEFAULT_CHUNK_SIZE = 2 * 1024 * 1024
 
 
@@ -54,8 +55,9 @@
     'prepare_body',
     'prepare_cidr',
     'prepare_containerfile',
     'prepare_containerignore',
     'prepare_filters',
     'prepare_timestamp',
     'stream_frames',
+    'stream_helper',
 ]
```

### Comparing `podman-4.4.1/podman/api/adapter_utils.py` & `podman-4.5.0/podman/api/adapter_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/api/client.py` & `podman-4.5.0/podman/api/client.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/api/http_utils.py` & `podman-4.5.0/podman/api/http_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/api/parse_utils.py` & `podman-4.5.0/podman/api/parse_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,7 +93,18 @@
         if not frame_length:
             continue
 
         data = response.raw.read(frame_length)
         if not data:
             return
         yield data
+
+
+def stream_helper(
+    response: Response, decode_to_json: bool = False
+) -> Union[Iterator[bytes], Iterator[Dict[str, Any]]]:
+    """Helper to stream results and optionally decode to json"""
+    for value in response.iter_lines():
+        if decode_to_json:
+            yield json.loads(value)
+        else:
+            yield value
```

### Comparing `podman-4.4.1/podman/api/ssh.py` & `podman-4.5.0/podman/api/ssh.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/api/tar_utils.py` & `podman-4.5.0/podman/api/tar_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/api/typing_extensions.py` & `podman-4.5.0/podman/api/typing_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -948,16 +948,15 @@
         metaclass=_ExtensionsGenericMeta,
         extra=contextlib.AbstractAsyncContextManager,
     ):
         __slots__ = ()
 
     __all__.append('AsyncContextManager')
 elif sys.version_info[:2] >= (3, 5):
-    exec(
-        """
+    exec("""
 class AsyncContextManager(typing.Generic[T_co]):
     __slots__ = ()
 
     async def __aenter__(self):
         return self
 
     @abc.abstractmethod
@@ -967,16 +966,15 @@
     @classmethod
     def __subclasshook__(cls, C):
         if cls is AsyncContextManager:
             return _check_methods_in_mro(C, "__aenter__", "__aexit__")
         return NotImplemented
 
 __all__.append('AsyncContextManager')
-"""
-    )
+""")
 
 if hasattr(typing, 'DefaultDict'):
     DefaultDict = typing.DefaultDict
 elif _geqv_defined:
 
     class DefaultDict(
         collections.defaultdict,
```

### Comparing `podman-4.4.1/podman/api/uds.py` & `podman-4.5.0/podman/api/uds.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/client.py` & `podman-4.5.0/podman/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,22 +109,27 @@
             assert_hostname: Ignored.
             environment: Dict containing input environment. Default: os.environ
             credstore_env: Dict containing environment for credential store
             use_ssh_client: Use system ssh client rather than ssh module. Always, True.
 
         Returns:
             Client used to communicate with a Podman service.
+
+        Raises:
+            ValueError when required environment variable is not set
         """
         environment = environment or os.environ
         credstore_env = credstore_env or {}
 
         if version == "auto":
             version = None
 
         host = environment.get("CONTAINER_HOST") or environment.get("DOCKER_HOST") or None
+        if host is None:
+            raise ValueError("CONTAINER_HOST or DOCKER_HOST must be set to URL of podman service.")
 
         return PodmanClient(
             base_url=host,
             version=version,
             timeout=timeout,
             tls=False,
             credstore_env=credstore_env,
```

### Comparing `podman-4.4.1/podman/domain/config.py` & `podman-4.5.0/podman/domain/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """Read containers.conf file."""
+import sys
 import urllib
 from pathlib import Path
 from typing import Dict, Optional
 
 import xdg.BaseDirectory
 
-try:
-    import toml
-except ImportError:
-    import pytoml as toml
-
 from podman.api import cached_property
 
+if sys.version_info >= (3, 11):
+    from tomllib import loads as toml_loads
+else:
+    try:
+        from tomli import loads as toml_loads
+    except ImportError:
+        try:
+            from toml import loads as toml_loads
+        except ImportError:
+            from pytoml import loads as toml_loads
+
 
 class ServiceConnection:
     """ServiceConnection defines a connection to the Podman service."""
 
     def __init__(self, name: str, attrs: Dict[str, str]):
         """Create a Podman ServiceConnection."""
         self.name = name
@@ -60,15 +67,15 @@
         else:
             self.path = Path(path)
 
         self.attrs = {}
         if self.path.exists():
             with self.path.open(encoding='utf-8') as file:
                 buffer = file.read()
-            self.attrs = toml.loads(buffer)
+            self.attrs = toml_loads(buffer)
 
     def __hash__(self) -> int:
         return hash(tuple(self.path.name))
 
     def __eq__(self, other) -> bool:
         if isinstance(other, PodmanConfig):
             return self.id == other.id and self.attrs == other.attrs
```

### Comparing `podman-4.4.1/podman/domain/containers.py` & `podman-4.5.0/podman/domain/containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Model and Manager for Container resources."""
-import io
 import json
 import logging
 import shlex
 from contextlib import suppress
-from typing import Any, Dict, Iterable, Iterator, List, Mapping, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, Iterable, Iterator, List, Mapping, Optional, Tuple, Union
 
 import requests
-from requests import Response
 
 from podman import api
 from podman.domain.images import Image
 from podman.domain.images_manager import ImagesManager
 from podman.domain.manager import PodmanResource
 from podman.errors import APIError
 
@@ -386,15 +384,17 @@
             detach_keys: Override the key sequence for detaching a container (Podman only)
         """
         response = self.client.post(
             f"/containers/{self.id}/start", params={"detachKeys": kwargs.get("detach_keys")}
         )
         response.raise_for_status()
 
-    def stats(self, **kwargs) -> Union[Sequence[Dict[str, bytes]], bytes]:
+    def stats(
+        self, **kwargs
+    ) -> Union[bytes, Dict[str, Any], Iterator[bytes], Iterator[Dict[str, Any]]]:
         """Return statistics for container.
 
         Keyword Args:
             decode (bool): If True and stream is True, stream will be decoded into dict's.
                 Default: False.
             stream (bool): Stream statistics until cancelled. Default: True.
 
@@ -406,35 +406,21 @@
         decode = kwargs.get("decode", False)
 
         params = {
             "containers": self.id,
             "stream": stream,
         }
 
-        response = self.client.get("/containers/stats", params=params)
+        response = self.client.get("/containers/stats", params=params, stream=stream)
         response.raise_for_status()
 
         if stream:
-            return self._stats_helper(decode, response.iter_lines())
+            return api.stream_helper(response, decode_to_json=decode)
 
-        with io.StringIO() as buffer:
-            for entry in response.text:
-                buffer.write(json.dumps(entry) + "\n")
-            return buffer.getvalue()
-
-    @staticmethod
-    def _stats_helper(
-        decode: bool, body: List[Dict[str, Any]]
-    ) -> Iterator[Union[str, Dict[str, Any]]]:
-        """Helper needed to allow stats() to return either a generator or a str."""
-        for entry in body:
-            if decode:
-                yield json.loads(entry)
-            else:
-                yield entry
+        return json.loads(response.content) if decode else response.content
 
     def stop(self, **kwargs) -> None:
         """Stop container.
 
         Keyword Args:
             all (bool): When True, stop all containers. Default: False (Podman only)
             ignore (bool): When True, ignore error if container already stopped (Podman only)
@@ -466,31 +452,28 @@
             ps_args (str): When given, arguments will be passed to ps
             stream (bool): When True, repeatedly return results. Default: False
 
         Raises:
             NotFound: when the container no longer exists
             APIError: when the service reports an error
         """
+        stream = kwargs.get("stream", False)
+
         params = {
+            "stream": stream,
             "ps_args": kwargs.get("ps_args"),
-            "stream": kwargs.get("stream", False),
         }
-        response = self.client.get(f"/containers/{self.id}/top", params=params)
+        response = self.client.get(f"/containers/{self.id}/top", params=params, stream=stream)
         response.raise_for_status()
 
-        if params["stream"]:
-            self._top_helper(response)
+        if stream:
+            return api.stream_helper(response, decode_to_json=True)
 
         return response.json()
 
-    @staticmethod
-    def _top_helper(response: Response) -> Iterator[Dict[str, Any]]:
-        for line in response.iter_lines():
-            yield line
-
     def unpause(self) -> None:
         """Unpause processes in container."""
         response = self.client.post(f"/containers/{self.id}/unpause")
         response.raise_for_status()
 
     def update(self, **kwargs):
         """Update resource configuration of the containers.
```

### Comparing `podman-4.4.1/podman/domain/containers_create.py` & `podman-4.5.0/podman/domain/containers_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from contextlib import suppress
 from typing import Any, Dict, List, MutableMapping, Union
 
 from podman import api
 from podman.domain.containers import Container
 from podman.domain.images import Image
 from podman.domain.pods import Pod
+from podman.domain.secrets import Secret
 from podman.errors import ImageNotFound
 
 logger = logging.getLogger("podman.containers")
 
 
 class CreateMixin:  # pylint: disable=too-few-public-methods
     """Class providing create method for ContainersManager."""
@@ -195,14 +196,15 @@
 
                 - Name: One of on-failure, or always.
                 - MaximumRetryCount: Number of times to restart the container on failure.
 
                 For example: {"Name": "on-failure", "MaximumRetryCount": 5}
 
             runtime (str): Runtime to use with this container.
+            secrets (Union[List[Secret]|List[str]]): Secrets to add to this container.
             security_opt (List[str]): A List[str]ing values to customize labels for MLS systems,
                 such as SELinux.
             shm_size (Union[str, int]): Size of /dev/shm (e.g. 1G).
             stdin_open (bool): Keep STDIN open even if not attached.
             stdout (bool): Return logs from STDOUT when detach=False. Default: True.
             stderr (bool): Return logs from STDERR when detach=False. Default: False.
             stop_signal (str): The stop signal to use to stop the container (e.g. SIGINT).
@@ -219,17 +221,19 @@
             tty (bool): Allocate a pseudo-TTY.
             ulimits (List[Ulimit]): Ulimits to set inside the container.
             use_config_proxy (bool): If True, and if the docker client configuration
                 file (~/.config/containers/config.json by default) contains a proxy configuration,
                 the corresponding environment variables will be set in the container being built.
             user (Union[str, int]): Username or UID to run commands as inside the container.
             userns_mode (str): Sets the user namespace mode for the container when user namespace
-                remapping option is enabled. Supported values are: host
+                remapping option is enabled. Supported values documented here
+                https://docs.podman.io/en/latest/markdown/options/userns.container.html#userns-mode
             uts_mode (str): Sets the UTS namespace mode for the container.
-                Supported values are: host
+                Supported values are documented here
+                https://docs.podman.io/en/latest/markdown/options/uts.container.html
             version (str): The version of the API to use. Set to auto to automatically detect
                 the server's version. Default: 3.0.0
             volume_driver (str): The name of a volume driver/plugin.
             volumes (Dict[str, Dict[str, Union[str, list]]]): A dictionary to configure
                 volumes mounted inside the container.
                 The key is either the host path or a volume name, and the value is
                 a dictionary with the keys:
@@ -423,15 +427,15 @@
             "remove": args.pop("remove", args.pop("auto_remove", None)),
             "resource_limits": {},
             "rootfs": pop("rootfs"),
             "rootfs_propagation": pop("rootfs_propagation"),
             "sdnotifyMode": pop("sdnotifyMode"),  # TODO document, podman only
             "seccomp_policy": pop("seccomp_policy"),  # TODO document, podman only
             "seccomp_profile_path": pop("seccomp_profile_path"),  # TODO document, podman only
-            "secrets": pop("secrets"),  # TODO document, podman only
+            "secrets": [],  # TODO document, podman only
             "selinux_opts": pop("security_opt"),
             "shm_size": to_bytes(pop("shm_size")),
             "static_mac": pop("mac_address"),
             "stdin": pop("stdin_open"),
             "stop_signal": pop("stop_signal"),
             "stop_timeout": pop("stop_timeout"),  # TODO document, podman only
             "sysctl": pop("sysctls"),
@@ -598,14 +602,20 @@
                 if not isinstance(mode, str):
                     raise ValueError("'mode' value should be a str")
                 options.append(mode)
 
             volume = {"Name": key, "Dest": value["bind"], "Options": options}
             params["volumes"].append(volume)
 
+        for item in args.pop("secrets", []):
+            if isinstance(item, Secret):
+                params["secrets"].append({"ID": item.id})
+            elif isinstance(item, str):
+                params["secrets"].append({"ID": item})
+
         if "cgroupns" in args:
             params["cgroupns"] = {"nsmode": args.pop("cgroupns")}
 
         if "ipc_mode" in args:
             params["ipcns"] = {"nsmode": args.pop("ipc_mode")}
 
         if "network_mode" in args:
```

### Comparing `podman-4.4.1/podman/domain/containers_manager.py` & `podman-4.5.0/podman/domain/containers_manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/containers_run.py` & `podman-4.5.0/podman/domain/containers_run.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/events.py` & `podman-4.5.0/podman/domain/events.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/images.py` & `podman-4.5.0/podman/domain/images.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/images_build.py` & `podman-4.5.0/podman/domain/images_build.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/images_manager.py` & `podman-4.5.0/podman/domain/images_manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/ipam.py` & `podman-4.5.0/podman/domain/ipam.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/manager.py` & `podman-4.5.0/podman/domain/manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/manifests.py` & `podman-4.5.0/podman/domain/manifests.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/networks.py` & `podman-4.5.0/podman/domain/networks.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/networks_manager.py` & `podman-4.5.0/podman/domain/networks_manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/pods.py` & `podman-4.5.0/podman/domain/pods.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/pods_manager.py` & `podman-4.5.0/podman/domain/pods_manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/registry_data.py` & `podman-4.5.0/podman/domain/registry_data.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/secrets.py` & `podman-4.5.0/podman/domain/secrets.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/system.py` & `podman-4.5.0/podman/domain/system.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/domain/volumes.py` & `podman-4.5.0/podman/domain/volumes.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/errors/__init__.py` & `podman-4.5.0/podman/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/errors/exceptions.py` & `podman-4.5.0/podman/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman/tlsconfig.py` & `podman-4.5.0/podman/tlsconfig.py`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/podman.egg-info/PKG-INFO` & `podman-4.5.0/podman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podman
-Version: 4.4.1
+Version: 4.5.0
 Summary: Bindings for Podman RESTful API
 Home-page: https://github.com/containers/podman-py
 Author: Brent Baude, Jhon Honce
 Author-email: jhonce@redhat.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/containers/podman-py/issues
 Project-URL: Libpod API, https://docs.podman.io/en/latest/_static/api.html
@@ -72,9 +72,7 @@
 
     print(json.dumps(client.df(), indent=4))
 ```
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/containers/podman-py/blob/main/CONTRIBUTING.md)
-
-
```

### Comparing `podman-4.4.1/podman.egg-info/SOURCES.txt` & `podman-4.5.0/podman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `podman-4.4.1/pyproject.toml` & `podman-4.5.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -5,33 +5,28 @@
 target-version = ["py36"]
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.tox
   | \.venv
+  | \.history
   | build
   | dist
   | docs
   | hack
 )/
 '''
 [tool.isort]
 profile = "black"
 line_length = 100
 [build-system]
 # Any changes should be copied into requirements.txt, setup.cfg, and/or test-requirements.txt
 requires = [
-    "pyxdg>=0.26",
-    "requests>=2.24",
     "setuptools>=46.4",
-    "sphinx",
-    "toml>=0.10.2",
-    "urllib3>=1.26.5",
-    "wheel",
 ]
 build-backend = "setuptools.build_meta"
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "DEBUG"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
```

### Comparing `podman-4.4.1/setup.cfg` & `podman-4.5.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = podman
-version = attr: podman.__version__
+version = 4.5.0
 author = Brent Baude, Jhon Honce
 author_email = jhonce@redhat.com
 description = Bindings for Podman RESTful API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/containers/podman-py
 license = Apache-2.0
@@ -31,15 +31,15 @@
 [options]
 include_package_data = True
 python_requires = >=3.6
 test_suite = 
 install_requires = 
 	pyxdg >=0.26
 	requests >=2.24
-	toml >=0.10.2
+	tomli>=1.2.3; python_version<'3.11'
 	urllib3 >=1.26.5
 
 [bdist_wheel]
 universal = false
 
 [sdist]
 formats = gztar
```

### Comparing `podman-4.4.1/setup.py` & `podman-4.5.0/setup.py`

 * *Files identical despite different names*


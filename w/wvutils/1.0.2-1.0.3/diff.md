# Comparing `tmp/wvutils-1.0.2.tar.gz` & `tmp/wvutils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wvutils-1.0.2.tar", last modified: Tue Mar  7 01:21:24 2023, max compression
+gzip compressed data, was "wvutils-1.0.3.tar", last modified: Thu Apr 27 02:41:52 2023, max compression
```

## Comparing `wvutils-1.0.2.tar` & `wvutils-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-03-07 01:21:24.993493 wvutils-1.0.2/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    35149 2023-02-23 04:14:09.000000 wvutils-1.0.2/LICENSE
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    63861 2023-03-07 01:21:24.993493 wvutils-1.0.2/PKG-INFO
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    22155 2023-03-07 01:15:56.000000 wvutils-1.0.2/README.md
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     4186 2023-03-05 01:04:09.000000 wvutils-1.0.2/pyproject.toml
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       38 2023-03-07 01:21:24.993493 wvutils-1.0.2/setup.cfg
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      567 2023-03-05 00:32:19.000000 wvutils-1.0.2/setup.py
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-03-07 01:21:24.993493 wvutils-1.0.2/src/
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-03-07 01:21:24.993493 wvutils-1.0.2/src/wvutils/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       22 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/__init__.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     2306 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/args.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    10300 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/aws.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      483 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/compat.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      271 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/constants.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      816 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/errors.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     3821 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/general.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     2833 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/path.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     5022 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/proxies.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    10555 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/restruct.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     1472 2023-03-07 01:15:56.000000 wvutils-1.0.2/src/wvutils/typing.py
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-03-07 01:21:24.993493 wvutils-1.0.2/src/wvutils.egg-info/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    63861 2023-03-07 01:21:24.000000 wvutils-1.0.2/src/wvutils.egg-info/PKG-INFO
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      557 2023-03-07 01:21:24.000000 wvutils-1.0.2/src/wvutils.egg-info/SOURCES.txt
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)        1 2023-03-07 01:21:24.000000 wvutils-1.0.2/src/wvutils.egg-info/dependency_links.txt
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       90 2023-03-07 01:21:24.000000 wvutils-1.0.2/src/wvutils.egg-info/requires.txt
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)        8 2023-03-07 01:21:24.000000 wvutils-1.0.2/src/wvutils.egg-info/top_level.txt
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-03-07 01:21:24.993493 wvutils-1.0.2/tests/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     3056 2023-03-07 01:15:56.000000 wvutils-1.0.2/tests/test_args.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    15095 2023-03-07 01:15:56.000000 wvutils-1.0.2/tests/test_aws.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     3357 2023-03-07 01:15:56.000000 wvutils-1.0.2/tests/test_path.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     3936 2023-03-07 01:15:56.000000 wvutils-1.0.2/tests/test_proxies.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     9703 2023-03-07 01:15:56.000000 wvutils-1.0.2/tests/test_utils.py
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 02:41:52.939221 wvutils-1.0.3/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    35149 2023-02-23 04:14:09.000000 wvutils-1.0.3/LICENSE
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    74404 2023-04-27 02:41:52.939221 wvutils-1.0.3/PKG-INFO
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    32698 2023-04-27 02:39:19.000000 wvutils-1.0.3/README.md
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     4172 2023-04-27 02:31:56.000000 wvutils-1.0.3/pyproject.toml
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       38 2023-04-27 02:41:52.939221 wvutils-1.0.3/setup.cfg
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      567 2023-03-05 00:32:19.000000 wvutils-1.0.3/setup.py
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 02:41:52.935221 wvutils-1.0.3/src/
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 02:41:52.935221 wvutils-1.0.3/src/wvutils/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       22 2023-04-27 02:39:36.000000 wvutils-1.0.3/src/wvutils/__init__.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     2581 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/args.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    10461 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/aws.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      499 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/compat.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      478 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/constants.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     1343 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/dt.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      896 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/errors.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    10296 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/general.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     9421 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/parquet.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     3217 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/path.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     5626 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/proxies.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    11554 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/restruct.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     2004 2023-04-27 02:31:56.000000 wvutils-1.0.3/src/wvutils/type_aliases.py
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 02:41:52.935221 wvutils-1.0.3/src/wvutils.egg-info/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    74404 2023-04-27 02:41:52.000000 wvutils-1.0.3/src/wvutils.egg-info/PKG-INFO
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      692 2023-04-27 02:41:52.000000 wvutils-1.0.3/src/wvutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)        1 2023-04-27 02:41:52.000000 wvutils-1.0.3/src/wvutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      199 2023-04-27 02:41:52.000000 wvutils-1.0.3/src/wvutils.egg-info/requires.txt
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)        8 2023-04-27 02:41:52.000000 wvutils-1.0.3/src/wvutils.egg-info/top_level.txt
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-04-27 02:41:52.935221 wvutils-1.0.3/tests/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     1731 2023-04-27 02:31:56.000000 wvutils-1.0.3/tests/test_args.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    17647 2023-04-27 02:31:56.000000 wvutils-1.0.3/tests/test_aws.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      168 2023-04-27 02:31:56.000000 wvutils-1.0.3/tests/test_constants.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     8366 2023-04-27 02:31:56.000000 wvutils-1.0.3/tests/test_dt.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    10433 2023-04-27 02:31:56.000000 wvutils-1.0.3/tests/test_general.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    10321 2023-04-27 02:31:56.000000 wvutils-1.0.3/tests/test_parquet.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     3492 2023-04-27 02:31:56.000000 wvutils-1.0.3/tests/test_path.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     3876 2023-04-27 02:31:56.000000 wvutils-1.0.3/tests/test_proxies.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    17453 2023-04-27 02:31:56.000000 wvutils-1.0.3/tests/test_restruct.py
```

### Comparing `wvutils-1.0.2/LICENSE` & `wvutils-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wvutils-1.0.2/PKG-INFO` & `wvutils-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wvutils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Collection of common utilities.
 Author-email: The Phosmic Development Team <dev@phosmic.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -789,22 +789,22 @@
 - _Session_ - Boto3 session.
 
 <a id="wvutils.aws.clear_boto3_sessions"></a>
 
 #### `clear_boto3_sessions`
 
 ```python
-def clear_boto3_sessions()
+def clear_boto3_sessions() -> int
 ```
 
 Clear all globally shared Boto3 sessions (thread-safe).
 
 **Returns**:
 
-- _bool_ - Whether any sessions were cleared.
+- _int_ - Number of sessions cleared.
 
 <a id="wvutils.aws.boto3_client_ctx"></a>
 
 #### `boto3_client_ctx`
 
 ```python
 @contextmanager
@@ -853,26 +853,26 @@
 #### `download_from_s3`
 
 ```python
 def download_from_s3(file_path: FilePath,
                      bucket_name: str,
                      bucket_path: str,
                      region_name: AWSRegion,
-                     overwrite: bool = True) -> None
+                     overwrite: bool = False) -> None
 ```
 
 Download a file from S3.
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Output path to use while downloading the file.
 - `bucket_name` _str_ - Name of the S3 bucket containing the file.
 - `bucket_path` _str_ - Path of the S3 bucket containing the file.
 - `region_name` _AWSRegion_ - Region name for S3.
-- `overwrite` _bool_ - Overwrite file on disk if already exists. Defaults to True.
+- `overwrite` _bool_ - Overwrite file on disk if already exists. Defaults to False.
 
 **Raises**:
 
 - `FileExistsError` - If the file already exists and overwrite is False.
 
 <a id="wvutils.aws.upload_file_to_s3"></a>
 
@@ -996,14 +996,112 @@
 Stop the execution of a query in Athena.
 
 **Arguments**:
 
 - `qeid` _str_ - Query execution ID of the query to stop.
 - `region_name` _AWSRegion_ - Region name for Athena.
 
+<a id="wvutils.errors"></a>
+
+# `wvutils.errors`
+
+Custom errors.
+
+This module contains custom exceptions that are used throughout the package.
+
+<a id="wvutils.errors.WVUtilsError"></a>
+
+## `WVUtilsError` Objects
+
+```python
+class WVUtilsError(Exception)
+```
+
+Base class for all wvutils exceptions.
+
+<a id="wvutils.errors.JSONError"></a>
+
+## `JSONError` Objects
+
+```python
+class JSONError(Exception)
+```
+
+Base class for all JSON exceptions.
+
+<a id="wvutils.errors.JSONEncodeError"></a>
+
+## `JSONEncodeError` Objects
+
+```python
+class JSONEncodeError(JSONError, TypeError)
+```
+
+Raised when JSON serializing fails.
+
+<a id="wvutils.errors.JSONDecodeError"></a>
+
+## `JSONDecodeError` Objects
+
+```python
+class JSONDecodeError(JSONError, ValueError)
+```
+
+Raised when JSON deserializing fails.
+
+<a id="wvutils.errors.PickleError"></a>
+
+## `PickleError` Objects
+
+```python
+class PickleError(Exception)
+```
+
+Base class for all pickle exceptions.
+
+<a id="wvutils.errors.PickleEncodeError"></a>
+
+## `PickleEncodeError` Objects
+
+```python
+class PickleEncodeError(PickleError, TypeError)
+```
+
+Raised when pickle serializing fails.
+
+<a id="wvutils.errors.PickleDecodeError"></a>
+
+## `PickleDecodeError` Objects
+
+```python
+class PickleDecodeError(PickleError, ValueError)
+```
+
+Raised when unpickling fails.
+
+<a id="wvutils.errors.HashError"></a>
+
+## `HashError` Objects
+
+```python
+class HashError(Exception)
+```
+
+Base class for all hashing exceptions.
+
+<a id="wvutils.errors.HashEncodeError"></a>
+
+## `HashEncodeError` Objects
+
+```python
+class HashEncodeError(HashError, TypeError)
+```
+
+Raised when hashing fails.
+
 <a id="wvutils.path"></a>
 
 # `wvutils.path`
 
 Utilities for working with paths.
 
 This module provides utilities for working with paths.
@@ -1014,14 +1112,16 @@
 
 ```python
 def is_pathlike(potential_path: Any) -> bool
 ```
 
 Check if an object is path-like.
 
+An object is path-like if it is a string or has a `__fspath__` method.
+
 **Arguments**:
 
 - `potential_path` _Any_ - Object to check.
 
 **Returns**:
 
 - _bool_ - True if the object is path-like, otherwise False.
@@ -1032,22 +1132,29 @@
 
 ```python
 def stringify_path(file_path: FilePath) -> str
 ```
 
 Stringify a path-like object.
 
+The path-like object is first converted to a string, then the user directory is expanded.
+> An object is path-like if it is a string or has a `__fspath__` method.
+
 **Arguments**:
 
 - `file_path` _FilePath_ - Path-like object to stringify.
 
 **Returns**:
 
 - _str_ - Path-like object as a string.
 
+**Raises**:
+
+- `TypeError` - If the object is not path-like.
+
 <a id="wvutils.path.ensure_abspath"></a>
 
 #### `ensure_abspath`
 
 ```python
 def ensure_abspath(file_path: str) -> str
 ```
@@ -1068,22 +1175,29 @@
 
 ```python
 def resolve_path(file_path: FilePath) -> str
 ```
 
 Stringify and resolve a path-like object.
 
+The path-like object is first converted to a string, then the user directory is expanded, and finally the path is resolved to an absolute path.
+> An object is path-like if it is a string or has a `__fspath__` method.
+
 **Arguments**:
 
 - `file_path` _FilePath_ - Path-like object to resolve.
 
 **Returns**:
 
 - _str_ - Absolute path of the path-like object as a string.
 
+**Raises**:
+
+- `TypeError` - If the object is not path-like.
+
 <a id="wvutils.path.xdg_cache_path"></a>
 
 #### `xdg_cache_path`
 
 ```python
 def xdg_cache_path() -> str
 ```
@@ -1123,17 +1237,20 @@
 
 ```python
 def add_proxies(proxies: list[str], include_duplicates: bool = False) -> None
 ```
 
 Add additional proxy addresses.
 
+All proxy addresses added will be added to the end of the list.
+
 **Arguments**:
 
 - `proxies` _list[str]_ - List of proxy addresses.
+- `include_duplicates` _bool, optional_ - Whether to include duplicates. Defaults to False.
 
 <a id="wvutils.proxies.ProxyManager.set_proxies"></a>
 
 #### `ProxyManager.set_proxies`
 
 ```python
 def set_proxies(proxies: list[str]) -> None
@@ -1201,14 +1318,18 @@
 
 - `address` _str_ - HTTPS proxy address.
 
 **Returns**:
 
 - _str_ - HTTP proxy address.
 
+**Raises**:
+
+- `ValueError` - If the address does not start with 'http://' or 'https://'.
+
 <a id="wvutils.proxies.prepare_http_proxy_for_requests"></a>
 
 #### `prepare_http_proxy_for_requests`
 
 ```python
 def prepare_http_proxy_for_requests(address: str) -> dict[str, str]
 ```
@@ -1221,35 +1342,35 @@
 
 **Returns**:
 
 - _dict[str, str]_ - Dictionary of HTTP and HTTPS proxy addresses.
 
 **Raises**:
 
-- `ValueError` - If the address does not start with 'http(s)://'.
+- `ValueError` - If the address does not start with 'http://' or 'https://'.
 
 <a id="wvutils.args"></a>
 
 # `wvutils.args`
 
 Utilities for parsing arguments from the command line.
 
 This module provides utilities for parsing arguments from the command line.
 
 <a id="wvutils.args.nonempty_string"></a>
 
 #### `nonempty_string`
 
 ```python
-def nonempty_string(name: str) -> Callable
+def nonempty_string(name: str) -> Callable[[str], str]
 ```
 
 Ensure a string is non-empty.
 
-Example Usage:
+**Example**:
 
 ```python
 subparser.add_argument(
     "hashtag",
     type=nonempty_string("hashtag"),
     help="A hashtag (without #)",
 )
@@ -1257,68 +1378,90 @@
 
 **Arguments**:
 
 - `name` _str_ - Name of the function, used for debugging.
 
 **Returns**:
 
-- _Callable_ - The decorated function.
+- _Callable[[str], str]_ - The decorated function.
 
 <a id="wvutils.args.safechars_string"></a>
 
 #### `safechars_string`
 
 ```python
 def safechars_string(
-    name: str,
-    allowed_chars: str | set[str] | tuple[str] | list[str] | None = None
-) -> Callable
+        name: str,
+        allowed_chars: Collection[str] | None = None) -> Callable[[str], str]
 ```
 
 Ensure a string contains only safe characters.
 
-Example Usage:
+**Example**:
 
 ```python
 subparser.add_argument(
     "--session-key",
     type=safechars_string,
     help="Key to share a single token across processes",
 )
 ```
 
 **Arguments**:
 
 - `name` _str_ - Name of the function, used for debugging.
-- `allowed_chars` _str | set[str] | tuple[str] | list[str] | None, optional_ - Custom characters used to validate the function name. Defaults to None.
+- `allowed_chars` _Collection[str] | None, optional_ - Custom characters used to validate the function name. Defaults to None.
 
 **Returns**:
 
-- _Callable_ - The decorated function.
+- _Callable[[str], str]_ - The decorated function.
+
+**Raises**:
+
+- `ValueError` - If empty collection of allowed characters is provided.
 
 <a id="wvutils.general"></a>
 
 # `wvutils.general`
 
 General utilities for working with Python.
 
 This module provides general utilities for working with Python.
 
+<a id="wvutils.general.is_iolike"></a>
+
+#### `is_iolike`
+
+```python
+def is_iolike(potential_io: Any) -> bool
+```
+
+Check if an object is IO-like.
+
+**Arguments**:
+
+- `potential_io` _Any_ - Object to check.
+
+**Returns**:
+
+- _bool_ - True if the object is IO-like, otherwise False.
+
 <a id="wvutils.general.count_lines_in_file"></a>
 
 #### `count_lines_in_file`
 
 ```python
 def count_lines_in_file(file_path: FilePath) -> int
 ```
 
-Count the Number of Lines in a File
+Count the number of lines in a file.
+
+**Notes**:
 
-All files have at least 1 line:
-number of lines = # of newlines + 1
+  All files have at least 1 line (# of lines = # of newlines + 1).
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to count lines in.
 
 **Returns**:
 
@@ -1328,15 +1471,15 @@
 
 #### `sys_set_recursion_limit`
 
 ```python
 def sys_set_recursion_limit() -> None
 ```
 
-Raise Recursion Limit to Allow for More Recurse
+Raise recursion limit to allow for more recurse.
 
 <a id="wvutils.general.gc_set_threshold"></a>
 
 #### `gc_set_threshold`
 
 ```python
 def gc_set_threshold() -> None
@@ -1353,34 +1496,38 @@
 #### `chunker`
 
 ```python
 def chunker(seq: Sequence[Any],
             n: int) -> Generator[Sequence[Any], None, None]
 ```
 
-Iterate a Sequence in Chunks
+Iterate a sequence in size `n` chunks.
 
 **Arguments**:
 
 - `seq` _Sequence[Any]_ - Sequence of values.
 - `n` _int_ - Number of values per chunk.
 
 **Yields**:
 
 - _Sequence[Any]_ - Chunk of values with length <= n.
 
+**Raises**:
+
+- `ValueError` - If `n` is 0 or negative.
+
 <a id="wvutils.general.is_iterable"></a>
 
 #### `is_iterable`
 
 ```python
 def is_iterable(obj: Any) -> bool
 ```
 
-Check if an Object is Iterable
+Check if an object is iterable.
 
 **Arguments**:
 
 - `obj` _Any_ - Object to check.
 
 **Returns**:
 
@@ -1393,15 +1540,35 @@
 ```python
 def rename_key(obj: dict,
                src_key: str,
                dest_key: str,
                in_place: bool = False) -> dict | None
 ```
 
-Rename a Dictionary Key
+Rename a dictionary key.
+
+**Todo**:
+
+  * Add support for nested keys.
+  * Add support for renaming multiple keys at once.
+  * Add support for non-string (built-in) key types.
+
+  All of the following are True:
+
+  ```python
+  isinstance(True, bool)
+  isinstance(True, int)
+  1 == True
+  1 in {1: "a"}
+  True in {1: "a"}
+  1 in {True: "a"}
+  True in {True: "a"}
+  1 in {1: "a", True: "b"}
+  True in {1: "a", True: "b"}
+  ```
 
 **Arguments**:
 
 - `obj` _dict_ - Reference to the dictionary to modify.
 - `src` _str_ - Name of the key to rename.
 - `dest` _str_ - Name of the key to change to.
 - `in_place` _bool, optional_ - Perform in-place using the provided reference. Defaults to False.
@@ -1411,27 +1578,338 @@
 - _dict | None_ - Copy of the dictionary if in_place is False, otherwise None.
 
 <a id="wvutils.general.unnest_key"></a>
 
 #### `unnest_key`
 
 ```python
-def unnest_key(obj: dict, *keys: str) -> Any
+def unnest_key(obj: dict, *keys: str) -> Any | None
 ```
 
-Fetch a Value from a Deeply Nested Dictionary
+Fetch a value from a deeply nested dictionary.
 
 **Arguments**:
 
 - `obj` _dict_ - Dictionary to recursively iterate.
 - `*keys` _str_ - Ordered keys to fetch.
 
 **Returns**:
 
-- _Any_ - The result of the provided keys.
+- _Any | None_ - The result of the provided keys, or None if any key is not found.
+
+<a id="wvutils.general.sort_dict_by_key"></a>
+
+#### `sort_dict_by_key`
+
+```python
+def sort_dict_by_key(obj: dict,
+                     reverse: bool = False,
+                     deep_copy: bool = False) -> dict | None
+```
+
+Sort a dictionary by key.
+
+**Arguments**:
+
+- `obj` _dict_ - Dictionary to sort.
+- `reverse` _bool, optional_ - Sort in reverse order. Defaults to False.
+- `deep_copy` _bool, optional_ - Return a deep copy of the dictionary. Defaults to False.
+
+**Returns**:
+
+- _dict | None_ - Dictionary sorted by key. If `in_place` is True, None is returned.
+
+**Raises**:
+
+- `ValueError` - If the dictionary keys are not of the same type.
+
+<a id="wvutils.general.dedupe_list"></a>
+
+#### `dedupe_list`
+
+```python
+def dedupe_list(values: list[Any], raise_on_dupe: bool = False) -> list[Any]
+```
+
+Remove duplicate values from a list.
+
+**Example**:
+
+```python
+dedupe_list([1, 2, 3, 1, 2, 3])
+# [1, 2, 3]
+```
+
+**Arguments**:
+
+- `values` _list[Any]_ - List of values to dedupe.
+- `raise_on_dupe` _bool, optional_ - Raise an error if a duplicate is found. Defaults to False.
+
+**Returns**:
+
+- _list[Any]_ - List of unique values.
+
+**Raises**:
+
+- `ValueError` - If a duplicate is found and `raise_on_dupe` is True.
+
+<a id="wvutils.general.dupe_in_list"></a>
+
+#### `dupe_in_list`
+
+```python
+def dupe_in_list(values: list[Any]) -> bool
+```
+
+Check if a list has duplicate values.
+
+**Arguments**:
+
+- `values` _list[Any]_ - List of values to check.
+
+**Returns**:
+
+- _bool_ - Whether the list has duplicate values.
+
+<a id="wvutils.general.invert_dict_of_str"></a>
+
+#### `invert_dict_of_str`
+
+```python
+def invert_dict_of_str(obj: dict[Any, str],
+                       deep_copy: bool = False,
+                       raise_on_dupe: bool = False) -> dict
+```
+
+Invert a dictionary of strings.
+
+**Notes**:
+
+  The value of the last key with a given value will be used.
+
+**Example**:
+
+```python
+invert_dict_of_str({"a": "b", "c": "d"})
+# {"b": "a", "d": "c"}
+```
+
+**Arguments**:
+
+- `obj` _dict[Any, str]_ - Dictionary to invert.
+- `deep_copy` _bool, optional_ - Return a deep copy of the dictionary. Defaults to False.
+- `raise_on_dupe` _bool, optional_ - Raise an error if a duplicate is found. Defaults to False.
+
+**Returns**:
+
+- _dict_ - Inverted dictionary.
+
+**Raises**:
+
+- `ValueError` - If a duplicate is found and `raise_on_dupe` is True.
+
+<a id="wvutils.dt"></a>
+
+# `wvutils.dt`
+
+Datetime utilities.
+
+This module contains functions and classes that are used to work with datetimes.
+
+<a id="wvutils.dt.dtformats"></a>
+
+## `dtformats` Objects
+
+```python
+class dtformats()
+```
+
+Datetime formats.
+
+**Attributes**:
+
+- `twitter` _str_ - Twitter datetime format.
+- `reddit` _str_ - Reddit datetime format.
+- `general` _str_ - General datetime format.
+- `db` _str_ - Database datetime format.
+- `date` _str_ - Date format.
+- `time_12h` _str_ - 12-hour time format with timezone.
+- `time_24h` _str_ - 24-hour time format with timezone.
+
+<a id="wvutils.dt.num_days_in_month"></a>
+
+#### `num_days_in_month`
+
+```python
+def num_days_in_month(year: int, month: int) -> int
+```
+
+Determine the number of days in a month.
+
+**Arguments**:
+
+- `year` _int_ - Year to check.
+- `month` _int_ - Month to check.
+
+**Returns**:
+
+- _int_ - Number of days in the month.
+
+<a id="wvutils.parquet"></a>
+
+# `wvutils.parquet`
+
+Parquet utilities.
+
+This module provides utilities for working with Parquet files.
+
+<a id="wvutils.parquet.get_parquet_session"></a>
+
+#### `get_parquet_session`
+
+```python
+def get_parquet_session(use_s3: bool,
+                        region_name: AWSRegion | None = None) -> fs.FileSystem
+```
+
+Get the globally shared Parquet filesystem session.
+
+**Todo**:
+
+  * Add support for other session parameters.
+
+**Arguments**:
+
+- `use_s3` _bool_ - Use S3 if True, otherwise uses local filesystem.
+- `region_name` _AWSRegion | None, optional_ - AWS region name. Defaults to None.
+
+  
+
+**Returns**:
+
+- _pyarrow.fs.FileSystem_ - The filesystem session.
+
+<a id="wvutils.parquet.clear_parquet_sessions"></a>
+
+#### `clear_parquet_sessions`
+
+```python
+def clear_parquet_sessions() -> int
+```
+
+Clear all globally shared Parquet filesystem sessions.
+
+**Returns**:
+
+- _int_ - Number of sessions cleared.
+
+<a id="wvutils.parquet.create_pa_schema"></a>
+
+#### `create_pa_schema`
+
+```python
+def create_pa_schema(schema_template: dict[str, str]) -> pa.schema
+```
+
+Create a parquet schema from a template.
+
+**Example**:
+
+```python
+{
+    "key_a": "string",
+    "key_b": "integer",
+    "key_c": "float",
+    "key_d": "bool",
+    "key_e": "timestamp[s]",
+    "key_f": "timestamp[ms]",
+    "key_g": "timestamp[ns]",
+}
+```
+
+  becomes
+
+```python
+pa.schema([
+    ("key_a", pa.string()),
+    ("key_b", pa.int64()),
+    ("key_c", pa.float64()),
+    ("key_d", pa.bool_()),
+    ("key_e", pa.timestamp("s",  tz=utc)),
+    ("key_f", pa.timestamp("ms", tz=utc)),
+    ("key_g", pa.timestamp("ns", tz=utc)),
+])
+```
+
+**Arguments**:
+
+- `schema_template` _Sequence[Sequence[str]]_ - Data names and parquet types for creating the schema.
+
+**Returns**:
+
+- _pa.schema_ - Final parquet schema.
+
+**Raises**:
+
+- `ValueError` - If an unknown type name is encountered.
+
+<a id="wvutils.parquet.force_dataframe_dtypes"></a>
+
+#### `force_dataframe_dtypes`
+
+```python
+def force_dataframe_dtypes(dataframe: pd.DataFrame,
+                           template: dict[str, str]) -> pd.DataFrame
+```
+
+Force the data types of a dataframe using a template.
+
+**Arguments**:
+
+- `dataframe` _pd.DataFrame_ - Dataframe to force types.
+- `template` _dict[str, str]_ - Template to use for forcing types.
+
+**Returns**:
+
+- _pd.DataFrame_ - Dataframe with forced types.
+
+**Raises**:
+
+- `ValueError` - If an unknown type name is encountered.
+
+<a id="wvutils.parquet.export_dataset"></a>
+
+#### `export_dataset`
+
+```python
+def export_dataset(data: list[dict] | deque[dict] | pd.DataFrame,
+                   output_location: str | FilePath,
+                   primary_template: dict[str, str],
+                   partitions_template: dict[str, str],
+                   *,
+                   basename_template: str | None = None,
+                   use_s3: bool = False,
+                   region_name: AWSRegion | None = None,
+                   use_threads: bool = False,
+                   overwrite: bool = False) -> None
+```
+
+Write to dataset to local filesystem or AWS S3.
+
+**Arguments**:
+
+- `data` _list[dict] | deque[dict] | pd.DataFrame]_ - List, deque, or dataframe of objects to be written.
+- `output_location` _str | FilePath_ - Location to write the dataset to.
+- `primary_template` _dict[str, str]_ - Parquet schema template to use for the table (excluding partitions).
+  partitions_template(dict[str, str]): Parquet schema template to use for the partitions.
+- `basename_template` _str, optional_ - Filename template to use when writing to S3 or locally. Defaults to None.
+- `use_s3` _bool, optional_ - Use S3 as the destination when exporting parquet files. Defaults to False.
+- `region_name` _AWSRegion, optional_ - AWS region to use when exporting to S3. Defaults to None.
+- `use_threads` _bool, optional_ - Use multiple threads when exporting. Defaults to False.
+- `overwrite` _bool, optional_ - Overwrite existing files. Defaults to False.
 
 <a id="wvutils.restruct"></a>
 
 # `wvutils.restruct`
 
 Utilities for restructuring data.
 
@@ -1463,225 +1941,230 @@
 Read more: https://github.com/cloudpipe/cloudpickle/blob/master/README.md#overriding-pickles-serialization-mechanism-for-importable-constructs
 
 <a id="wvutils.restruct.json_dumps"></a>
 
 #### `json_dumps`
 
 ```python
-def json_dumps(obj: JSONEncodable) -> str
+def json_dumps(obj: JSONSerializable) -> str
 ```
 
 Encode an object as JSON.
 
 **Arguments**:
 
-- `obj` _JSONEncodable_ - Object to encode.
+- `obj` _JSONSerializable_ - Object to encode.
 
 **Returns**:
 
 - _str_ - Object encoded as JSON.
 
 **Raises**:
 
 - `JSONEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.jsonl_dumps"></a>
 
 #### `jsonl_dumps`
 
 ```python
-def jsonl_dumps(objs: Iterable[JSONEncodable]) -> str
+def jsonl_dumps(objs: Iterable[JSONSerializable]) -> str
 ```
 
 Encode objects as JSONL.
 
 **Arguments**:
 
-- `objs` _Iterable[JSONEncodable]_ - Objects to encode.
+- `objs` _Iterable[JSONSerializable]_ - Objects to encode.
 
 **Returns**:
 
 - _str_ - Objects encoded as JSONL.
 
 **Raises**:
 
-- `JSONEncodeError` - If the object could not be encoded.
+- `JSONEncodeError` - If the objects could not be encoded.
 
 <a id="wvutils.restruct.json_dump"></a>
 
 #### `json_dump`
 
 ```python
-def json_dump(file_path: str, obj: JSONEncodable) -> None
+def json_dump(obj: JSONSerializable, file_path: str) -> None
 ```
 
 Encode an object as JSON and write it to a file.
 
 **Arguments**:
 
 - `file_path` _str_ - Path of the file to open.
-- `obj` _JSONEncodable_ - Object to encode.
 
 **Raises**:
 
 - `JSONEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.jsonl_dump"></a>
 
 #### `jsonl_dump`
 
 ```python
-def jsonl_dump(file_path: str, objs: Iterable[JSONEncodable]) -> None
+def jsonl_dump(objs: Iterable[JSONSerializable], file_path: str) -> None
 ```
 
 Encode objects as JSONL and write them to a file.
 
 **Arguments**:
 
+- `objs` _Iterable[JSONSerializable]_ - Objects to encode.
 - `file_path` _str_ - Path of the file to open.
-- `objs` _Iterable[JSONEncodable]_ - Objects to encode.
 
 **Raises**:
 
-- `JSONEncodeError` - If the object could not be encoded.
+- `JSONEncodeError` - If the objects could not be encoded.
 
 <a id="wvutils.restruct.json_loads"></a>
 
 #### `json_loads`
 
 ```python
-def json_loads(encoded_obj: str) -> JSONEncodable
+def json_loads(encoded_obj: str) -> JSONSerializable
 ```
 
 Decode a JSON-encoded object.
 
 **Arguments**:
 
 - `encoded_obj` _str_ - Object to decode.
 
 **Returns**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the object could not be decoded.
 
 <a id="wvutils.restruct.json_load"></a>
 
 #### `json_load`
 
 ```python
-def json_load(file_path: FilePath) -> JSONEncodable
+def json_load(file_path: FilePath) -> JSONSerializable
 ```
 
 Decode a file containing a JSON-encoded object.
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to open.
 
 **Returns**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the file could not be decoded.
 
 <a id="wvutils.restruct.jsonl_loader"></a>
 
 #### `jsonl_loader`
 
 ```python
 def jsonl_loader(
-        file_path: FilePath,
-        *,
-        allow_empty_lines: bool = True
-) -> Generator[JSONEncodable, None, None]
+    file_path: FilePath,
+    *,
+    allow_empty_lines: bool = False
+) -> Generator[JSONSerializable, None, None]
 ```
 
 Decode a file containing JSON-encoded objects, one per line.
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to open.
-- `allow_empty_lines` _bool, optional_ - Whether to allow empty lines. Defaults to True.
+- `allow_empty_lines` _bool, optional_ - Whether to allow (skip) empty lines. Defaults to False.
 
 **Yields**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the line could not be decoded, or if an empty line was found and `allow_empty_lines` is False.
 
 <a id="wvutils.restruct.squeegee_loader"></a>
 
 #### `squeegee_loader`
 
 ```python
 def squeegee_loader(
-        file_path: FilePath) -> Generator[JSONEncodable, None, None]
+        file_path: FilePath) -> Generator[JSONSerializable, None, None]
 ```
 
 Automatically decode a file containing JSON-encoded objects.
 
 Supports multiple formats (JSON, JSONL, JSONL of JSONL, etc).
 
+**Todo**:
+
+  * Add support for pretty-printed JSON that has been appended to a file.
+
+  
+
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to open.
 
 **Yields**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the line could not be decoded.
 
 <a id="wvutils.restruct.gen_hash"></a>
 
 #### `gen_hash`
 
 ```python
-def gen_hash(obj: MD5Hashable) -> str | None
+def gen_hash(obj: MD5Hashable) -> str
 ```
 
 Create an MD5 hash from a hashable object.
 
-Note: Tuples and sets are not hashable, so they are converted to lists.
+Note: Tuples and deques are not hashable, so they are converted to lists.
 
 **Arguments**:
 
 - `obj` _MD5Hashable_ - Object to hash.
 
 **Returns**:
 
-- _str | None_ - MD5 hash of the object, or None if object was an empty iterable.
+- _str_ - MD5 hash of the object.
 
 **Raises**:
 
 - `HashEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.pickle_dump"></a>
 
 #### `pickle_dump`
 
 ```python
-def pickle_dump(file_path: FilePath, obj: PickleSerializable) -> None
+def pickle_dump(obj: PickleSerializable, file_path: FilePath) -> None
 ```
 
 Serialize an object as a pickle and write it to a file.
 
 **Arguments**:
 
+- `obj` _JSONSerializable_ - Object to serialize.
 - `file_path` _FilePath_ - Path of the file to write.
-- `obj` _JSONEncodable_ - Object to serialize.
 
 **Raises**:
 
 - `PickleEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.pickle_dumps"></a>
```

### Comparing `wvutils-1.0.2/README.md` & `wvutils-1.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -87,22 +87,22 @@
 - _Session_ - Boto3 session.
 
 <a id="wvutils.aws.clear_boto3_sessions"></a>
 
 #### `clear_boto3_sessions`
 
 ```python
-def clear_boto3_sessions()
+def clear_boto3_sessions() -> int
 ```
 
 Clear all globally shared Boto3 sessions (thread-safe).
 
 **Returns**:
 
-- _bool_ - Whether any sessions were cleared.
+- _int_ - Number of sessions cleared.
 
 <a id="wvutils.aws.boto3_client_ctx"></a>
 
 #### `boto3_client_ctx`
 
 ```python
 @contextmanager
@@ -151,26 +151,26 @@
 #### `download_from_s3`
 
 ```python
 def download_from_s3(file_path: FilePath,
                      bucket_name: str,
                      bucket_path: str,
                      region_name: AWSRegion,
-                     overwrite: bool = True) -> None
+                     overwrite: bool = False) -> None
 ```
 
 Download a file from S3.
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Output path to use while downloading the file.
 - `bucket_name` _str_ - Name of the S3 bucket containing the file.
 - `bucket_path` _str_ - Path of the S3 bucket containing the file.
 - `region_name` _AWSRegion_ - Region name for S3.
-- `overwrite` _bool_ - Overwrite file on disk if already exists. Defaults to True.
+- `overwrite` _bool_ - Overwrite file on disk if already exists. Defaults to False.
 
 **Raises**:
 
 - `FileExistsError` - If the file already exists and overwrite is False.
 
 <a id="wvutils.aws.upload_file_to_s3"></a>
 
@@ -294,14 +294,112 @@
 Stop the execution of a query in Athena.
 
 **Arguments**:
 
 - `qeid` _str_ - Query execution ID of the query to stop.
 - `region_name` _AWSRegion_ - Region name for Athena.
 
+<a id="wvutils.errors"></a>
+
+# `wvutils.errors`
+
+Custom errors.
+
+This module contains custom exceptions that are used throughout the package.
+
+<a id="wvutils.errors.WVUtilsError"></a>
+
+## `WVUtilsError` Objects
+
+```python
+class WVUtilsError(Exception)
+```
+
+Base class for all wvutils exceptions.
+
+<a id="wvutils.errors.JSONError"></a>
+
+## `JSONError` Objects
+
+```python
+class JSONError(Exception)
+```
+
+Base class for all JSON exceptions.
+
+<a id="wvutils.errors.JSONEncodeError"></a>
+
+## `JSONEncodeError` Objects
+
+```python
+class JSONEncodeError(JSONError, TypeError)
+```
+
+Raised when JSON serializing fails.
+
+<a id="wvutils.errors.JSONDecodeError"></a>
+
+## `JSONDecodeError` Objects
+
+```python
+class JSONDecodeError(JSONError, ValueError)
+```
+
+Raised when JSON deserializing fails.
+
+<a id="wvutils.errors.PickleError"></a>
+
+## `PickleError` Objects
+
+```python
+class PickleError(Exception)
+```
+
+Base class for all pickle exceptions.
+
+<a id="wvutils.errors.PickleEncodeError"></a>
+
+## `PickleEncodeError` Objects
+
+```python
+class PickleEncodeError(PickleError, TypeError)
+```
+
+Raised when pickle serializing fails.
+
+<a id="wvutils.errors.PickleDecodeError"></a>
+
+## `PickleDecodeError` Objects
+
+```python
+class PickleDecodeError(PickleError, ValueError)
+```
+
+Raised when unpickling fails.
+
+<a id="wvutils.errors.HashError"></a>
+
+## `HashError` Objects
+
+```python
+class HashError(Exception)
+```
+
+Base class for all hashing exceptions.
+
+<a id="wvutils.errors.HashEncodeError"></a>
+
+## `HashEncodeError` Objects
+
+```python
+class HashEncodeError(HashError, TypeError)
+```
+
+Raised when hashing fails.
+
 <a id="wvutils.path"></a>
 
 # `wvutils.path`
 
 Utilities for working with paths.
 
 This module provides utilities for working with paths.
@@ -312,14 +410,16 @@
 
 ```python
 def is_pathlike(potential_path: Any) -> bool
 ```
 
 Check if an object is path-like.
 
+An object is path-like if it is a string or has a `__fspath__` method.
+
 **Arguments**:
 
 - `potential_path` _Any_ - Object to check.
 
 **Returns**:
 
 - _bool_ - True if the object is path-like, otherwise False.
@@ -330,22 +430,29 @@
 
 ```python
 def stringify_path(file_path: FilePath) -> str
 ```
 
 Stringify a path-like object.
 
+The path-like object is first converted to a string, then the user directory is expanded.
+> An object is path-like if it is a string or has a `__fspath__` method.
+
 **Arguments**:
 
 - `file_path` _FilePath_ - Path-like object to stringify.
 
 **Returns**:
 
 - _str_ - Path-like object as a string.
 
+**Raises**:
+
+- `TypeError` - If the object is not path-like.
+
 <a id="wvutils.path.ensure_abspath"></a>
 
 #### `ensure_abspath`
 
 ```python
 def ensure_abspath(file_path: str) -> str
 ```
@@ -366,22 +473,29 @@
 
 ```python
 def resolve_path(file_path: FilePath) -> str
 ```
 
 Stringify and resolve a path-like object.
 
+The path-like object is first converted to a string, then the user directory is expanded, and finally the path is resolved to an absolute path.
+> An object is path-like if it is a string or has a `__fspath__` method.
+
 **Arguments**:
 
 - `file_path` _FilePath_ - Path-like object to resolve.
 
 **Returns**:
 
 - _str_ - Absolute path of the path-like object as a string.
 
+**Raises**:
+
+- `TypeError` - If the object is not path-like.
+
 <a id="wvutils.path.xdg_cache_path"></a>
 
 #### `xdg_cache_path`
 
 ```python
 def xdg_cache_path() -> str
 ```
@@ -421,17 +535,20 @@
 
 ```python
 def add_proxies(proxies: list[str], include_duplicates: bool = False) -> None
 ```
 
 Add additional proxy addresses.
 
+All proxy addresses added will be added to the end of the list.
+
 **Arguments**:
 
 - `proxies` _list[str]_ - List of proxy addresses.
+- `include_duplicates` _bool, optional_ - Whether to include duplicates. Defaults to False.
 
 <a id="wvutils.proxies.ProxyManager.set_proxies"></a>
 
 #### `ProxyManager.set_proxies`
 
 ```python
 def set_proxies(proxies: list[str]) -> None
@@ -499,14 +616,18 @@
 
 - `address` _str_ - HTTPS proxy address.
 
 **Returns**:
 
 - _str_ - HTTP proxy address.
 
+**Raises**:
+
+- `ValueError` - If the address does not start with 'http://' or 'https://'.
+
 <a id="wvutils.proxies.prepare_http_proxy_for_requests"></a>
 
 #### `prepare_http_proxy_for_requests`
 
 ```python
 def prepare_http_proxy_for_requests(address: str) -> dict[str, str]
 ```
@@ -519,35 +640,35 @@
 
 **Returns**:
 
 - _dict[str, str]_ - Dictionary of HTTP and HTTPS proxy addresses.
 
 **Raises**:
 
-- `ValueError` - If the address does not start with 'http(s)://'.
+- `ValueError` - If the address does not start with 'http://' or 'https://'.
 
 <a id="wvutils.args"></a>
 
 # `wvutils.args`
 
 Utilities for parsing arguments from the command line.
 
 This module provides utilities for parsing arguments from the command line.
 
 <a id="wvutils.args.nonempty_string"></a>
 
 #### `nonempty_string`
 
 ```python
-def nonempty_string(name: str) -> Callable
+def nonempty_string(name: str) -> Callable[[str], str]
 ```
 
 Ensure a string is non-empty.
 
-Example Usage:
+**Example**:
 
 ```python
 subparser.add_argument(
     "hashtag",
     type=nonempty_string("hashtag"),
     help="A hashtag (without #)",
 )
@@ -555,68 +676,90 @@
 
 **Arguments**:
 
 - `name` _str_ - Name of the function, used for debugging.
 
 **Returns**:
 
-- _Callable_ - The decorated function.
+- _Callable[[str], str]_ - The decorated function.
 
 <a id="wvutils.args.safechars_string"></a>
 
 #### `safechars_string`
 
 ```python
 def safechars_string(
-    name: str,
-    allowed_chars: str | set[str] | tuple[str] | list[str] | None = None
-) -> Callable
+        name: str,
+        allowed_chars: Collection[str] | None = None) -> Callable[[str], str]
 ```
 
 Ensure a string contains only safe characters.
 
-Example Usage:
+**Example**:
 
 ```python
 subparser.add_argument(
     "--session-key",
     type=safechars_string,
     help="Key to share a single token across processes",
 )
 ```
 
 **Arguments**:
 
 - `name` _str_ - Name of the function, used for debugging.
-- `allowed_chars` _str | set[str] | tuple[str] | list[str] | None, optional_ - Custom characters used to validate the function name. Defaults to None.
+- `allowed_chars` _Collection[str] | None, optional_ - Custom characters used to validate the function name. Defaults to None.
 
 **Returns**:
 
-- _Callable_ - The decorated function.
+- _Callable[[str], str]_ - The decorated function.
+
+**Raises**:
+
+- `ValueError` - If empty collection of allowed characters is provided.
 
 <a id="wvutils.general"></a>
 
 # `wvutils.general`
 
 General utilities for working with Python.
 
 This module provides general utilities for working with Python.
 
+<a id="wvutils.general.is_iolike"></a>
+
+#### `is_iolike`
+
+```python
+def is_iolike(potential_io: Any) -> bool
+```
+
+Check if an object is IO-like.
+
+**Arguments**:
+
+- `potential_io` _Any_ - Object to check.
+
+**Returns**:
+
+- _bool_ - True if the object is IO-like, otherwise False.
+
 <a id="wvutils.general.count_lines_in_file"></a>
 
 #### `count_lines_in_file`
 
 ```python
 def count_lines_in_file(file_path: FilePath) -> int
 ```
 
-Count the Number of Lines in a File
+Count the number of lines in a file.
+
+**Notes**:
 
-All files have at least 1 line:
-number of lines = # of newlines + 1
+  All files have at least 1 line (# of lines = # of newlines + 1).
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to count lines in.
 
 **Returns**:
 
@@ -626,15 +769,15 @@
 
 #### `sys_set_recursion_limit`
 
 ```python
 def sys_set_recursion_limit() -> None
 ```
 
-Raise Recursion Limit to Allow for More Recurse
+Raise recursion limit to allow for more recurse.
 
 <a id="wvutils.general.gc_set_threshold"></a>
 
 #### `gc_set_threshold`
 
 ```python
 def gc_set_threshold() -> None
@@ -651,34 +794,38 @@
 #### `chunker`
 
 ```python
 def chunker(seq: Sequence[Any],
             n: int) -> Generator[Sequence[Any], None, None]
 ```
 
-Iterate a Sequence in Chunks
+Iterate a sequence in size `n` chunks.
 
 **Arguments**:
 
 - `seq` _Sequence[Any]_ - Sequence of values.
 - `n` _int_ - Number of values per chunk.
 
 **Yields**:
 
 - _Sequence[Any]_ - Chunk of values with length <= n.
 
+**Raises**:
+
+- `ValueError` - If `n` is 0 or negative.
+
 <a id="wvutils.general.is_iterable"></a>
 
 #### `is_iterable`
 
 ```python
 def is_iterable(obj: Any) -> bool
 ```
 
-Check if an Object is Iterable
+Check if an object is iterable.
 
 **Arguments**:
 
 - `obj` _Any_ - Object to check.
 
 **Returns**:
 
@@ -691,15 +838,35 @@
 ```python
 def rename_key(obj: dict,
                src_key: str,
                dest_key: str,
                in_place: bool = False) -> dict | None
 ```
 
-Rename a Dictionary Key
+Rename a dictionary key.
+
+**Todo**:
+
+  * Add support for nested keys.
+  * Add support for renaming multiple keys at once.
+  * Add support for non-string (built-in) key types.
+
+  All of the following are True:
+
+  ```python
+  isinstance(True, bool)
+  isinstance(True, int)
+  1 == True
+  1 in {1: "a"}
+  True in {1: "a"}
+  1 in {True: "a"}
+  True in {True: "a"}
+  1 in {1: "a", True: "b"}
+  True in {1: "a", True: "b"}
+  ```
 
 **Arguments**:
 
 - `obj` _dict_ - Reference to the dictionary to modify.
 - `src` _str_ - Name of the key to rename.
 - `dest` _str_ - Name of the key to change to.
 - `in_place` _bool, optional_ - Perform in-place using the provided reference. Defaults to False.
@@ -709,27 +876,338 @@
 - _dict | None_ - Copy of the dictionary if in_place is False, otherwise None.
 
 <a id="wvutils.general.unnest_key"></a>
 
 #### `unnest_key`
 
 ```python
-def unnest_key(obj: dict, *keys: str) -> Any
+def unnest_key(obj: dict, *keys: str) -> Any | None
 ```
 
-Fetch a Value from a Deeply Nested Dictionary
+Fetch a value from a deeply nested dictionary.
 
 **Arguments**:
 
 - `obj` _dict_ - Dictionary to recursively iterate.
 - `*keys` _str_ - Ordered keys to fetch.
 
 **Returns**:
 
-- _Any_ - The result of the provided keys.
+- _Any | None_ - The result of the provided keys, or None if any key is not found.
+
+<a id="wvutils.general.sort_dict_by_key"></a>
+
+#### `sort_dict_by_key`
+
+```python
+def sort_dict_by_key(obj: dict,
+                     reverse: bool = False,
+                     deep_copy: bool = False) -> dict | None
+```
+
+Sort a dictionary by key.
+
+**Arguments**:
+
+- `obj` _dict_ - Dictionary to sort.
+- `reverse` _bool, optional_ - Sort in reverse order. Defaults to False.
+- `deep_copy` _bool, optional_ - Return a deep copy of the dictionary. Defaults to False.
+
+**Returns**:
+
+- _dict | None_ - Dictionary sorted by key. If `in_place` is True, None is returned.
+
+**Raises**:
+
+- `ValueError` - If the dictionary keys are not of the same type.
+
+<a id="wvutils.general.dedupe_list"></a>
+
+#### `dedupe_list`
+
+```python
+def dedupe_list(values: list[Any], raise_on_dupe: bool = False) -> list[Any]
+```
+
+Remove duplicate values from a list.
+
+**Example**:
+
+```python
+dedupe_list([1, 2, 3, 1, 2, 3])
+# [1, 2, 3]
+```
+
+**Arguments**:
+
+- `values` _list[Any]_ - List of values to dedupe.
+- `raise_on_dupe` _bool, optional_ - Raise an error if a duplicate is found. Defaults to False.
+
+**Returns**:
+
+- _list[Any]_ - List of unique values.
+
+**Raises**:
+
+- `ValueError` - If a duplicate is found and `raise_on_dupe` is True.
+
+<a id="wvutils.general.dupe_in_list"></a>
+
+#### `dupe_in_list`
+
+```python
+def dupe_in_list(values: list[Any]) -> bool
+```
+
+Check if a list has duplicate values.
+
+**Arguments**:
+
+- `values` _list[Any]_ - List of values to check.
+
+**Returns**:
+
+- _bool_ - Whether the list has duplicate values.
+
+<a id="wvutils.general.invert_dict_of_str"></a>
+
+#### `invert_dict_of_str`
+
+```python
+def invert_dict_of_str(obj: dict[Any, str],
+                       deep_copy: bool = False,
+                       raise_on_dupe: bool = False) -> dict
+```
+
+Invert a dictionary of strings.
+
+**Notes**:
+
+  The value of the last key with a given value will be used.
+
+**Example**:
+
+```python
+invert_dict_of_str({"a": "b", "c": "d"})
+# {"b": "a", "d": "c"}
+```
+
+**Arguments**:
+
+- `obj` _dict[Any, str]_ - Dictionary to invert.
+- `deep_copy` _bool, optional_ - Return a deep copy of the dictionary. Defaults to False.
+- `raise_on_dupe` _bool, optional_ - Raise an error if a duplicate is found. Defaults to False.
+
+**Returns**:
+
+- _dict_ - Inverted dictionary.
+
+**Raises**:
+
+- `ValueError` - If a duplicate is found and `raise_on_dupe` is True.
+
+<a id="wvutils.dt"></a>
+
+# `wvutils.dt`
+
+Datetime utilities.
+
+This module contains functions and classes that are used to work with datetimes.
+
+<a id="wvutils.dt.dtformats"></a>
+
+## `dtformats` Objects
+
+```python
+class dtformats()
+```
+
+Datetime formats.
+
+**Attributes**:
+
+- `twitter` _str_ - Twitter datetime format.
+- `reddit` _str_ - Reddit datetime format.
+- `general` _str_ - General datetime format.
+- `db` _str_ - Database datetime format.
+- `date` _str_ - Date format.
+- `time_12h` _str_ - 12-hour time format with timezone.
+- `time_24h` _str_ - 24-hour time format with timezone.
+
+<a id="wvutils.dt.num_days_in_month"></a>
+
+#### `num_days_in_month`
+
+```python
+def num_days_in_month(year: int, month: int) -> int
+```
+
+Determine the number of days in a month.
+
+**Arguments**:
+
+- `year` _int_ - Year to check.
+- `month` _int_ - Month to check.
+
+**Returns**:
+
+- _int_ - Number of days in the month.
+
+<a id="wvutils.parquet"></a>
+
+# `wvutils.parquet`
+
+Parquet utilities.
+
+This module provides utilities for working with Parquet files.
+
+<a id="wvutils.parquet.get_parquet_session"></a>
+
+#### `get_parquet_session`
+
+```python
+def get_parquet_session(use_s3: bool,
+                        region_name: AWSRegion | None = None) -> fs.FileSystem
+```
+
+Get the globally shared Parquet filesystem session.
+
+**Todo**:
+
+  * Add support for other session parameters.
+
+**Arguments**:
+
+- `use_s3` _bool_ - Use S3 if True, otherwise uses local filesystem.
+- `region_name` _AWSRegion | None, optional_ - AWS region name. Defaults to None.
+
+  
+
+**Returns**:
+
+- _pyarrow.fs.FileSystem_ - The filesystem session.
+
+<a id="wvutils.parquet.clear_parquet_sessions"></a>
+
+#### `clear_parquet_sessions`
+
+```python
+def clear_parquet_sessions() -> int
+```
+
+Clear all globally shared Parquet filesystem sessions.
+
+**Returns**:
+
+- _int_ - Number of sessions cleared.
+
+<a id="wvutils.parquet.create_pa_schema"></a>
+
+#### `create_pa_schema`
+
+```python
+def create_pa_schema(schema_template: dict[str, str]) -> pa.schema
+```
+
+Create a parquet schema from a template.
+
+**Example**:
+
+```python
+{
+    "key_a": "string",
+    "key_b": "integer",
+    "key_c": "float",
+    "key_d": "bool",
+    "key_e": "timestamp[s]",
+    "key_f": "timestamp[ms]",
+    "key_g": "timestamp[ns]",
+}
+```
+
+  becomes
+
+```python
+pa.schema([
+    ("key_a", pa.string()),
+    ("key_b", pa.int64()),
+    ("key_c", pa.float64()),
+    ("key_d", pa.bool_()),
+    ("key_e", pa.timestamp("s",  tz=utc)),
+    ("key_f", pa.timestamp("ms", tz=utc)),
+    ("key_g", pa.timestamp("ns", tz=utc)),
+])
+```
+
+**Arguments**:
+
+- `schema_template` _Sequence[Sequence[str]]_ - Data names and parquet types for creating the schema.
+
+**Returns**:
+
+- _pa.schema_ - Final parquet schema.
+
+**Raises**:
+
+- `ValueError` - If an unknown type name is encountered.
+
+<a id="wvutils.parquet.force_dataframe_dtypes"></a>
+
+#### `force_dataframe_dtypes`
+
+```python
+def force_dataframe_dtypes(dataframe: pd.DataFrame,
+                           template: dict[str, str]) -> pd.DataFrame
+```
+
+Force the data types of a dataframe using a template.
+
+**Arguments**:
+
+- `dataframe` _pd.DataFrame_ - Dataframe to force types.
+- `template` _dict[str, str]_ - Template to use for forcing types.
+
+**Returns**:
+
+- _pd.DataFrame_ - Dataframe with forced types.
+
+**Raises**:
+
+- `ValueError` - If an unknown type name is encountered.
+
+<a id="wvutils.parquet.export_dataset"></a>
+
+#### `export_dataset`
+
+```python
+def export_dataset(data: list[dict] | deque[dict] | pd.DataFrame,
+                   output_location: str | FilePath,
+                   primary_template: dict[str, str],
+                   partitions_template: dict[str, str],
+                   *,
+                   basename_template: str | None = None,
+                   use_s3: bool = False,
+                   region_name: AWSRegion | None = None,
+                   use_threads: bool = False,
+                   overwrite: bool = False) -> None
+```
+
+Write to dataset to local filesystem or AWS S3.
+
+**Arguments**:
+
+- `data` _list[dict] | deque[dict] | pd.DataFrame]_ - List, deque, or dataframe of objects to be written.
+- `output_location` _str | FilePath_ - Location to write the dataset to.
+- `primary_template` _dict[str, str]_ - Parquet schema template to use for the table (excluding partitions).
+  partitions_template(dict[str, str]): Parquet schema template to use for the partitions.
+- `basename_template` _str, optional_ - Filename template to use when writing to S3 or locally. Defaults to None.
+- `use_s3` _bool, optional_ - Use S3 as the destination when exporting parquet files. Defaults to False.
+- `region_name` _AWSRegion, optional_ - AWS region to use when exporting to S3. Defaults to None.
+- `use_threads` _bool, optional_ - Use multiple threads when exporting. Defaults to False.
+- `overwrite` _bool, optional_ - Overwrite existing files. Defaults to False.
 
 <a id="wvutils.restruct"></a>
 
 # `wvutils.restruct`
 
 Utilities for restructuring data.
 
@@ -761,225 +1239,230 @@
 Read more: https://github.com/cloudpipe/cloudpickle/blob/master/README.md#overriding-pickles-serialization-mechanism-for-importable-constructs
 
 <a id="wvutils.restruct.json_dumps"></a>
 
 #### `json_dumps`
 
 ```python
-def json_dumps(obj: JSONEncodable) -> str
+def json_dumps(obj: JSONSerializable) -> str
 ```
 
 Encode an object as JSON.
 
 **Arguments**:
 
-- `obj` _JSONEncodable_ - Object to encode.
+- `obj` _JSONSerializable_ - Object to encode.
 
 **Returns**:
 
 - _str_ - Object encoded as JSON.
 
 **Raises**:
 
 - `JSONEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.jsonl_dumps"></a>
 
 #### `jsonl_dumps`
 
 ```python
-def jsonl_dumps(objs: Iterable[JSONEncodable]) -> str
+def jsonl_dumps(objs: Iterable[JSONSerializable]) -> str
 ```
 
 Encode objects as JSONL.
 
 **Arguments**:
 
-- `objs` _Iterable[JSONEncodable]_ - Objects to encode.
+- `objs` _Iterable[JSONSerializable]_ - Objects to encode.
 
 **Returns**:
 
 - _str_ - Objects encoded as JSONL.
 
 **Raises**:
 
-- `JSONEncodeError` - If the object could not be encoded.
+- `JSONEncodeError` - If the objects could not be encoded.
 
 <a id="wvutils.restruct.json_dump"></a>
 
 #### `json_dump`
 
 ```python
-def json_dump(file_path: str, obj: JSONEncodable) -> None
+def json_dump(obj: JSONSerializable, file_path: str) -> None
 ```
 
 Encode an object as JSON and write it to a file.
 
 **Arguments**:
 
 - `file_path` _str_ - Path of the file to open.
-- `obj` _JSONEncodable_ - Object to encode.
 
 **Raises**:
 
 - `JSONEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.jsonl_dump"></a>
 
 #### `jsonl_dump`
 
 ```python
-def jsonl_dump(file_path: str, objs: Iterable[JSONEncodable]) -> None
+def jsonl_dump(objs: Iterable[JSONSerializable], file_path: str) -> None
 ```
 
 Encode objects as JSONL and write them to a file.
 
 **Arguments**:
 
+- `objs` _Iterable[JSONSerializable]_ - Objects to encode.
 - `file_path` _str_ - Path of the file to open.
-- `objs` _Iterable[JSONEncodable]_ - Objects to encode.
 
 **Raises**:
 
-- `JSONEncodeError` - If the object could not be encoded.
+- `JSONEncodeError` - If the objects could not be encoded.
 
 <a id="wvutils.restruct.json_loads"></a>
 
 #### `json_loads`
 
 ```python
-def json_loads(encoded_obj: str) -> JSONEncodable
+def json_loads(encoded_obj: str) -> JSONSerializable
 ```
 
 Decode a JSON-encoded object.
 
 **Arguments**:
 
 - `encoded_obj` _str_ - Object to decode.
 
 **Returns**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the object could not be decoded.
 
 <a id="wvutils.restruct.json_load"></a>
 
 #### `json_load`
 
 ```python
-def json_load(file_path: FilePath) -> JSONEncodable
+def json_load(file_path: FilePath) -> JSONSerializable
 ```
 
 Decode a file containing a JSON-encoded object.
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to open.
 
 **Returns**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the file could not be decoded.
 
 <a id="wvutils.restruct.jsonl_loader"></a>
 
 #### `jsonl_loader`
 
 ```python
 def jsonl_loader(
-        file_path: FilePath,
-        *,
-        allow_empty_lines: bool = True
-) -> Generator[JSONEncodable, None, None]
+    file_path: FilePath,
+    *,
+    allow_empty_lines: bool = False
+) -> Generator[JSONSerializable, None, None]
 ```
 
 Decode a file containing JSON-encoded objects, one per line.
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to open.
-- `allow_empty_lines` _bool, optional_ - Whether to allow empty lines. Defaults to True.
+- `allow_empty_lines` _bool, optional_ - Whether to allow (skip) empty lines. Defaults to False.
 
 **Yields**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the line could not be decoded, or if an empty line was found and `allow_empty_lines` is False.
 
 <a id="wvutils.restruct.squeegee_loader"></a>
 
 #### `squeegee_loader`
 
 ```python
 def squeegee_loader(
-        file_path: FilePath) -> Generator[JSONEncodable, None, None]
+        file_path: FilePath) -> Generator[JSONSerializable, None, None]
 ```
 
 Automatically decode a file containing JSON-encoded objects.
 
 Supports multiple formats (JSON, JSONL, JSONL of JSONL, etc).
 
+**Todo**:
+
+  * Add support for pretty-printed JSON that has been appended to a file.
+
+  
+
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to open.
 
 **Yields**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the line could not be decoded.
 
 <a id="wvutils.restruct.gen_hash"></a>
 
 #### `gen_hash`
 
 ```python
-def gen_hash(obj: MD5Hashable) -> str | None
+def gen_hash(obj: MD5Hashable) -> str
 ```
 
 Create an MD5 hash from a hashable object.
 
-Note: Tuples and sets are not hashable, so they are converted to lists.
+Note: Tuples and deques are not hashable, so they are converted to lists.
 
 **Arguments**:
 
 - `obj` _MD5Hashable_ - Object to hash.
 
 **Returns**:
 
-- _str | None_ - MD5 hash of the object, or None if object was an empty iterable.
+- _str_ - MD5 hash of the object.
 
 **Raises**:
 
 - `HashEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.pickle_dump"></a>
 
 #### `pickle_dump`
 
 ```python
-def pickle_dump(file_path: FilePath, obj: PickleSerializable) -> None
+def pickle_dump(obj: PickleSerializable, file_path: FilePath) -> None
 ```
 
 Serialize an object as a pickle and write it to a file.
 
 **Arguments**:
 
+- `obj` _JSONSerializable_ - Object to serialize.
 - `file_path` _FilePath_ - Path of the file to write.
-- `obj` _JSONEncodable_ - Object to serialize.
 
 **Raises**:
 
 - `PickleEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.pickle_dumps"></a>
```

### Comparing `wvutils-1.0.2/pyproject.toml` & `wvutils-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,21 @@
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
   "boto3>=1.18.44",
   "botocore>=1.21.44",
   "cloudpickle>=2.0.0",
-  # "google-re2>=0.2.20210901",
-  # "lxml>=4.6.3",
-  # "numpy>=1.21.2",
-  # "pandas>=1.3.3",
-  # "pyarrow==7.0.0",
-  # "requests>=2.26.0",
-  # "s3fs>=0.4.2",
+  "google-re2>=0.2.20210901",
+  "lxml>=4.6.3",
+  "numpy>=1.21.2",
+  "pandas>=1.3.3",
+  "pyarrow==7.0.0",
+  "requests>=2.26.0",
+  "s3fs>=0.4.2",
   "python-rapidjson>=1.5",
   "urllib3>=1.26.6",
 ]
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://pypi.org/project/wvutils/"
```

### Comparing `wvutils-1.0.2/setup.py` & `wvutils-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `wvutils-1.0.2/src/wvutils/args.py` & `wvutils-1.0.3/src/wvutils/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,104 @@
 """Utilities for parsing arguments from the command line.
 
 This module provides utilities for parsing arguments from the command line.
 """
+from __future__ import annotations
 
 import logging
-from collections.abc import Callable
+from typing import TYPE_CHECKING
 
 from wvutils.constants import DEFAULT_SAFECHARS_ALLOWED_CHARS
 
+if TYPE_CHECKING:
+    from collections.abc import Callable, Collection
+
 __all__ = [
     "nonempty_string",
     "safechars_string",
 ]
 
-logger = logging.getLogger(__name__)
+logger: logging.Logger = logging.getLogger(__name__)
 
 
-def nonempty_string(name: str) -> Callable:
+def nonempty_string(name: str) -> Callable[[str], str]:
     """Ensure a string is non-empty.
 
-    Example Usage:
+    Example:
 
     ```python
     subparser.add_argument(
         "hashtag",
         type=nonempty_string("hashtag"),
         help="A hashtag (without #)",
     )
     ```
 
     Args:
         name (str): Name of the function, used for debugging.
 
     Returns:
-        Callable: The decorated function.
+        Callable[[str], str]: The decorated function.
     """
 
     def func(text):
         text = text.strip()
         if not text:
             raise ValueError("Must not be an empty string")
         return text
 
     func.__name__ = name
     return func
 
 
 def safechars_string(
     name: str,
-    allowed_chars: str | set[str] | tuple[str] | list[str] | None = None,
-) -> Callable:
+    allowed_chars: Collection[str] | None = None,
+) -> Callable[[str], str]:
     """Ensure a string contains only safe characters.
 
-    Example Usage:
+    Example:
 
     ```python
     subparser.add_argument(
         "--session-key",
         type=safechars_string,
         help="Key to share a single token across processes",
     )
     ```
 
     Args:
         name (str): Name of the function, used for debugging.
-        allowed_chars (str | set[str] | tuple[str] | list[str] | None, optional): Custom characters used to validate the function name. Defaults to None.
+        allowed_chars (Collection[str] | None, optional): Custom characters used to validate the function name. Defaults to None.
 
     Returns:
-        Callable: The decorated function.
+        Callable[[str], str]: The decorated function.
+
+    Raises:
+        ValueError: If empty collection of allowed characters is provided.
     """
     if allowed_chars is None:
         # Default to alphanum
         allowed_chars = DEFAULT_SAFECHARS_ALLOWED_CHARS
     else:
         # Prepare user-provided chars
         allowed_chars = set(allowed_chars)
 
+    if len(allowed_chars) == 0:
+        raise ValueError("Must provide at least one character")
+
     def func(text):
         text = text.strip()
         for char in text:
             if char not in allowed_chars:
                 msg = ""
-                msg += "Invalid string. Must consist of characters ["
+                msg += "Must consist of characters ["
                 if allowed_chars:
                     msg += "'"
                     msg += "', '".join(allowed_chars)
                     msg += "'"
-                msg += "]."
+                msg += "]"
                 raise ValueError(msg)
         return text
 
     func.__name__ = name
     return func
```

### Comparing `wvutils-1.0.2/src/wvutils/aws.py` & `wvutils-1.0.3/src/wvutils/aws.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 """Utilities for interacting with AWS services.
 
 This module provides utilities for interacting with AWS services.
 """
+from __future__ import annotations
 
 import io
 import logging
 import os
 from contextlib import contextmanager
+from typing import TYPE_CHECKING
 
 from boto3.session import Session
 from botocore.exceptions import ClientError
 
-from wvutils.typing import AWSRegion, FilePath
-
 from wvutils.general import unnest_key
 from wvutils.path import resolve_path
 from wvutils.restruct import json_loads
 
+if TYPE_CHECKING:
+    from wvutils.type_aliases import AWSRegion, FilePath
 __all__ = [
     "athena_execute_query",
     "athena_retrieve_query",
     "athena_stop_query",
     "clear_boto3_sessions",
     "download_from_s3",
     "get_boto3_session",
     "parse_s3_uri",
     "secrets_fetch",
     "boto3_client_ctx",
     "upload_bytes_to_s3",
     "upload_file_to_s3",
 ]
 
-logger = logging.getLogger(__name__)
+logger: logging.Logger = logging.getLogger(__name__)
 
-_global_boto3_sessions: dict[AWSRegion, Session] = {}
+_boto3_sessions: dict[AWSRegion, Session] = {}
 
 
 def get_boto3_session(region_name: AWSRegion) -> Session:
     """Get the globally shared Boto3 session for a region (thread-safe).
 
     Todo:
         * Add support for other session parameters.
 
     Args:
         region_name (AWSRegion): Region name for the session.
 
     Returns:
         Session: Boto3 session.
     """
-    if region_name not in _global_boto3_sessions:
-        _global_boto3_sessions[region_name] = Session(region_name=region_name)
-    return _global_boto3_sessions[region_name]
+    if region_name not in _boto3_sessions:
+        _boto3_sessions[region_name] = Session(region_name=region_name)
+    return _boto3_sessions[region_name]
 
 
-def clear_boto3_sessions():
+def clear_boto3_sessions() -> int:
     """Clear all globally shared Boto3 sessions (thread-safe).
 
     Returns:
-        bool: Whether any sessions were cleared.
+        int: Number of sessions cleared.
     """
-    had_sessions = bool(_global_boto3_sessions)
-    _global_boto3_sessions.clear()
-    return had_sessions
+    num_sessions_cleared = len(_boto3_sessions)
+    _boto3_sessions.clear()
+    return num_sessions_cleared
 
 
 @contextmanager
 def boto3_client_ctx(service_name: str, region_name: AWSRegion):
     """Context manager for a Boto3 client (thread-safe).
 
     Todo:
@@ -121,40 +123,40 @@
 
 
 def download_from_s3(
     file_path: FilePath,
     bucket_name: str,
     bucket_path: str,
     region_name: AWSRegion,
-    overwrite: bool = True,
+    overwrite: bool = False,
 ) -> None:
     """Download a file from S3.
 
     Args:
         file_path (FilePath): Output path to use while downloading the file.
         bucket_name (str): Name of the S3 bucket containing the file.
         bucket_path (str): Path of the S3 bucket containing the file.
         region_name (AWSRegion): Region name for S3.
-        overwrite (bool): Overwrite file on disk if already exists. Defaults to True.
+        overwrite (bool): Overwrite file on disk if already exists. Defaults to False.
 
     Raises:
         FileExistsError: If the file already exists and overwrite is False.
     """
     file_path = resolve_path(file_path)
     if os.path.isfile(file_path):
-        if overwrite:
-            logger.warning(f"Overwriting file: {file_path}")
-        else:
+        if not overwrite:
             raise FileExistsError(f"File already exists: {file_path}")
 
     bucket_path = bucket_path.removeprefix("/")
     with open(file_path, "wb") as wbf:
         with boto3_client_ctx("s3", region_name=region_name) as s3_client:
             s3_client.download_fileobj(bucket_name, bucket_path, wbf)
-            logger.info(f"Downloaded s3://{bucket_name}/{bucket_path} to {file_path}")
+            logger.info(
+                "Downloaded s3://%s/%s to %s", bucket_name, bucket_path, file_path
+            )
 
 
 def upload_file_to_s3(
     file_path: FilePath,
     bucket_name: str,
     bucket_path: str,
     region_name: AWSRegion,
@@ -173,15 +175,15 @@
     file_path = resolve_path(file_path)
     if not os.path.isfile(file_path):
         raise FileNotFoundError(f"File not found: {file_path}")
 
     bucket_path = bucket_path.removeprefix("/")
     with boto3_client_ctx("s3", region_name=region_name) as s3_client:
         s3_client.upload_file(file_path, bucket_name, bucket_path)
-        logger.info(f"Uploaded {file_path} to s3://{bucket_name}/{bucket_path}")
+        logger.info("Uploaded %s to s3://%s/%s", file_path, bucket_name, bucket_path)
 
 
 def upload_bytes_to_s3(
     raw_b: bytes,
     bucket_name: str,
     bucket_path: str,
     region_name: AWSRegion,
@@ -198,15 +200,15 @@
         TypeError: If `raw_b` is not bytes.
     """
     if not isinstance(raw_b, bytes):
         raise TypeError(f"Expected bytes, got {type(raw_b)}")
     bucket_path = bucket_path.removeprefix("/")
     with boto3_client_ctx("s3", region_name=region_name) as s3_client:
         s3_client.upload_fileobj(io.BytesIO(raw_b), bucket_name, bucket_path)
-        logger.info(f"Uploaded raw bytes to s3://{bucket_name}/{bucket_path}")
+        logger.info("Uploaded raw bytes to s3://%s/%s", bucket_name, bucket_path)
 
 
 def secrets_fetch(
     secret_name: str,
     region_name: AWSRegion,
 ) -> str | int | float | list | dict | None:
     """Request and decode a secret from Secrets.
@@ -246,18 +248,20 @@
             QueryString=query,
             QueryExecutionContext={"Database": database_name},
         )
 
     qeid = None
     if response.get("QueryExecutionId") is not None:
         qeid = response["QueryExecutionId"]
-        logger.info(f"Executing QEID {qeid} on {database_name} ({region_name})")
+        logger.info("Executing QEID %s on %s (%s)", qeid, database_name, region_name)
     else:
         logger.info(
-            f"Failure to execute QEID: Could not find query execution ID in response on {database_name} ({region_name}). Skipping ..."
+            "Failure to execute QEID: Could not find query execution ID in response on %s (%s). Skipping ...",
+            database_name,
+            region_name,
         )
     return qeid
 
 
 def athena_retrieve_query(
     qeid: str,
     database_name: str,
@@ -278,39 +282,43 @@
     """
     with boto3_client_ctx("athena", region_name=region_name) as athena_client:
         response = athena_client.get_query_execution(QueryExecutionId=qeid)
 
     state = unnest_key(response, "QueryExecution", "Status", "State")
     # Reference: https://docs.amazonaws.cn/athena/latest/APIReference/API_QueryExecutionStatus.html
     if state == "SUCCEEDED":
-        logger.info(f"QEID {qeid} succeeded on {database_name} ({region_name})")
+        logger.info("QEID %s succeeded on %s (%s)", qeid, database_name, region_name)
         # S3 URI where results are stored
         return unnest_key(
             response, "QueryExecution", "ResultConfiguration", "OutputLocation"
         )
     elif state == "RUNNING":
-        logger.debug(f"QEID {qeid} is running on {database_name} ({region_name})")
+        logger.debug("QEID %s is running on %s (%s)", qeid, database_name, region_name)
         return state
     elif state == "QUEUED":
-        logger.debug(f"QEID {qeid} is queued on {database_name} ({region_name})")
+        logger.debug("QEID %s is queued on %s (%s)", qeid, database_name, region_name)
         return state
     elif state == "FAILED":
-        logger.info(f"QEID {qeid} failed to execute on {database_name} ({region_name})")
+        logger.info(
+            "QEID %s failed to execute on %s (%s)", qeid, database_name, region_name
+        )
         return state
     elif state == "CANCELLED":
-        logger.info(f"QEID {qeid} was cancelled on {database_name} ({region_name})")
+        logger.info(
+            "QEID %s was cancelled on %s (%s)", qeid, database_name, region_name
+        )
         return state
     else:
         raise ValueError(f"Unknown or missing state {state} for QEID {qeid}")
 
 
 def athena_stop_query(qeid: str, region_name: AWSRegion) -> None:
     """Stop the execution of a query in Athena.
 
     Args:
         qeid (str): Query execution ID of the query to stop.
         region_name (AWSRegion): Region name for Athena.
     """
-    logger.info(f"Stopping QEID {qeid}")
+    logger.info("Stopping QEID %s", qeid)
     with boto3_client_ctx("athena", region_name=region_name) as athena_client:
         athena_client.stop_query_execution(QueryExecutionId=qeid)
-        logger.info(f"Halted execution of QEID {qeid}")
+        logger.info("Halted execution of QEID %s", qeid)
```

### Comparing `wvutils-1.0.2/src/wvutils/path.py` & `wvutils-1.0.3/src/wvutils/path.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,62 @@
 """Utilities for working with paths.
 
 This module provides utilities for working with paths.
 """
+from __future__ import annotations
+
+import logging
+import os
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Any
+
+    from wvutils.type_aliases import FilePath
 
 __all__ = [
     "cache_path",
     "ensure_abspath",
-    # "is_iolike",
     "is_pathlike",
     "resolve_path",
     "stringify_path",
     "xdg_cache_path",
 ]
 
-import logging
-import os
-from typing import Any
-
-from wvutils.typing import FilePath
-
-logger = logging.getLogger(__name__)
-
-
-# def is_iolike(potential_io: Any) -> bool:
-#     """Check if an object is IO-like.
-#
-#     Args:
-#         potential_io (Any): Object to check.
-#
-#     Returns:
-#         bool: True if the object is IO-like, otherwise False.
-#     """
-#     return hasattr(potential_io, "read") and hasattr(potential_io, "write")
+logger: logging.Logger = logging.getLogger(__name__)
 
 
 def is_pathlike(potential_path: Any) -> bool:
     """Check if an object is path-like.
 
+    An object is path-like if it is a string or has a `__fspath__` method.
+
     Args:
         potential_path (Any): Object to check.
 
     Returns:
         bool: True if the object is path-like, otherwise False.
     """
     return isinstance(potential_path, str) or hasattr(potential_path, "__fspath__")
 
 
 def stringify_path(file_path: FilePath) -> str:
     """Stringify a path-like object.
 
+    The path-like object is first converted to a string, then the user directory is expanded.
+    > An object is path-like if it is a string or has a `__fspath__` method.
+
     Args:
         file_path (FilePath): Path-like object to stringify.
 
     Returns:
         str: Path-like object as a string.
+
+    Raises:
+        TypeError: If the object is not path-like.
     """
     if not isinstance(file_path, str):
         # e.g. pathlib.Path('/home/ubuntu') -> '/home/ubuntu'
         try:
             file_path = file_path.__fspath__()
         except AttributeError:
             raise TypeError(f"Object is not path-like: {file_path!r}")
@@ -78,19 +77,25 @@
     """
     return file_path if os.path.isabs(file_path) else os.path.abspath(file_path)
 
 
 def resolve_path(file_path: FilePath) -> str:
     """Stringify and resolve a path-like object.
 
+    The path-like object is first converted to a string, then the user directory is expanded, and finally the path is resolved to an absolute path.
+    > An object is path-like if it is a string or has a `__fspath__` method.
+
     Args:
         file_path (FilePath): Path-like object to resolve.
 
     Returns:
         str: Absolute path of the path-like object as a string.
+
+    Raises:
+        TypeError: If the object is not path-like.
     """
     return ensure_abspath(stringify_path(file_path))
 
 
 def xdg_cache_path() -> str:
     """Base directory to store user-specific non-essential data files.
```

### Comparing `wvutils-1.0.2/src/wvutils/proxies.py` & `wvutils-1.0.3/src/wvutils/proxies.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Utilities for working with proxies.
 
 This module provides utilities for working with proxies.
 """
 
 import logging
 import random
+import warnings
 
 __all__ = [
     "ProxyManager",
     "https_to_http",
     "prepare_http_proxy_for_requests",
 ]
 
-logger = logging.getLogger(__name__)
+logger: logging.Logger = logging.getLogger(__name__)
 
 
 class ProxyManager:
     """Manages a list of proxies.
 
     This class manages a list of proxies, allowing for randomization, re-use, etc.
     """
@@ -45,23 +46,30 @@
         self._index: int = -1
         # Initialize
         self._reset()
 
     def add_proxies(self, proxies: list[str], include_duplicates: bool = False) -> None:
         """Add additional proxy addresses.
 
+        All proxy addresses added will be added to the end of the list.
+
         Args:
             proxies (list[str]): List of proxy addresses.
+            include_duplicates (bool, optional): Whether to include duplicates. Defaults to False.
         """
+        proxies_copy = proxies.copy()
+        if self._random_order:
+            random.shuffle(proxies_copy)
+
         if include_duplicates:
-            # Include duplicates
             self._proxy_store.extend(proxies)
         else:
-            # Exclude duplicates
-            self._proxy_store.extend(list(set(proxies) - set(self._proxy_store)))
+            for proxy in proxies:
+                if proxy not in self._proxy_store:
+                    self._proxy_store.append(proxy)
         self._reset()
 
     def set_proxies(self, proxies: list[str]) -> None:
         """Set the proxy addresses.
 
         Note: This will clear all existing proxies.
 
@@ -70,92 +78,106 @@
         """
         # Clear existing proxies
         self._proxy_store.clear()
         # Add new proxies
         self.add_proxies(proxies)
 
     def _reset(self) -> None:
-        """Full Internal Reset"""
+        """Full internal reset."""
         # Refill and prepare working proxies from store
         self._proxies = self._proxy_store.copy()
         if self._random_order:
             random.shuffle(self._proxies)
         # Starting index
-        self._index = -1 if len(self._proxies) == 0 else 0
+        if self._proxies:
+            self._index = 0
+        else:
+            self._index = -1
+
+    @property
+    def _is_locked(self) -> bool:
+        """Check if the proxy manager is locked.
+
+        Returns:
+            bool: True if locked, False otherwise.
+        """
+        return self._index == -1
 
     @property
     def can_cycle(self) -> bool:
         """Check if can cycle to the next proxy address.
 
         Returns:
             bool: True if can cycle, False otherwise.
         """
         # Already locked
-        if self._index == -1:
+        if self._is_locked:
             return False
         # Out of proxies
         if (self._index + 1 == len(self._proxies)) and not self._reuse:
             return False
         return True
 
     def cycle(self) -> None:
         """Attempt to cycle to the next proxy address."""
         # Cannot cycle when locked
-        if self._index > -1:
+        if not self._is_locked:
             # Increment to next
             self._index += 1
             if self._index + 1 > len(self._proxies):
                 # Passed end of list
                 if self._reuse:
-                    # Full reset
+                    # Unlock and reset the manager
                     self._reset()
                 else:
-                    # Lock - Out of proxies
+                    # Lock the manager
                     self._index = -1
         else:
-            # TODO: Should raise or use 'warnings' module?
-            logger.warning("Attempted to cycle proxies after having ran out previously")
+            warnings.warn("Attempted to cycle a locked proxy manager.")
 
     @property
     def proxy(self) -> str | None:
         """Current proxy address.
 
         Returns:
             str | None: Current proxy, or None if no proxies.
         """
-        return self._proxies[self._index] if self._index > -1 else None
+        return self._proxies[self._index] if not self._is_locked else None
 
 
 def https_to_http(address: str) -> str:
     """Convert a HTTPS proxy address to HTTP.
 
     Args:
         address (str): HTTPS proxy address.
 
     Returns:
         str: HTTP proxy address.
+
+    Raises:
+        ValueError: If the address does not start with 'http://' or 'https://'.
     """
     if address.startswith("https://"):
         return "http" + address.removeprefix("https")
     if address.startswith("http://"):
         return address
-    raise ValueError(f"Invalid proxy address: {address}")
+    raise ValueError(f"Invalid proxy address: {address!r}")
 
 
 def prepare_http_proxy_for_requests(address: str) -> dict[str, str]:
     """Prepare a HTTP(S) proxy address for use with the 'requests' library.
 
     Args:
         address (str): HTTP(S) proxy address.
 
     Returns:
         dict[str, str]: Dictionary of HTTP and HTTPS proxy addresses.
 
     Raises:
-        ValueError: If the address does not start with 'http(s)://'.
+        ValueError: If the address does not start with 'http://' or 'https://'.
     """
     if address.startswith("https://"):
         return {
             "HTTPS_PROXY": address,
             "HTTP_PROXY": https_to_http(address),
             "https_proxy": address,
             "http_proxy": https_to_http(address),
@@ -163,8 +185,8 @@
     elif address.startswith("http://"):
         return {
             "HTTPS_PROXY": address,
             "HTTP_PROXY": address,
             "https_proxy": address,
             "http_proxy": address,
         }
-    raise ValueError(f"Invalid proxy address: {address}")
+    raise ValueError(f"Invalid proxy address: {address!r}")
```

### Comparing `wvutils-1.0.2/src/wvutils/restruct.py` & `wvutils-1.0.3/src/wvutils/restruct.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,39 +23,46 @@
 > An important difference between cloudpickle and pickle is that cloudpickle can serialize a function or class by value, whereas pickle can only serialize it by reference.
 > Serialization by reference treats functions and classes as attributes of modules, and pickles them through instructions that trigger the import of their module at load time.
 > Serialization by reference is thus limited in that it assumes that the module containing the function or class is available/importable in the unpickling environment.
 > This assumption breaks when pickling constructs defined in an interactive session, a case that is automatically detected by cloudpickle, that pickles such constructs by value.
 
 Read more: https://github.com/cloudpipe/cloudpickle/blob/master/README.md#overriding-pickles-serialization-mechanism-for-importable-constructs
 """
+from __future__ import annotations
 
-import collections
+import json
 import logging
-from collections.abc import Generator, Iterable
+from collections import deque
 from hashlib import md5
+from typing import TYPE_CHECKING
 
 import cloudpickle
 import rapidjson
 
 from wvutils.errors import (
     HashEncodeError,
     JSONDecodeError,
     JSONEncodeError,
     PickleDecodeError,
     PickleEncodeError,
 )
-from wvutils.typing import (
-    FilePath,
-    JSONEncodable,
-    MD5Hashable,
-    PickleSerializable,
-)
 
 from wvutils.path import resolve_path
 
+if TYPE_CHECKING:
+    from collections.abc import Generator, Iterable
+
+    from wvutils.type_aliases import (
+        FilePath,
+        JSONSerializable,
+        MD5Hashable,
+        PickleSerializable,
+    )
+
+
 __all__ = [
     "gen_hash",
     "json_dump",
     "json_dumps",
     "json_load",
     "json_loads",
     "jsonl_dump",
@@ -64,162 +71,175 @@
     "pickle_dump",
     "pickle_dumps",
     "pickle_load",
     "pickle_loads",
     "squeegee_loader",
 ]
 
-logger = logging.getLogger(__name__)
+logger: logging.Logger = logging.getLogger(__name__)
 
 
-def json_dumps(obj: JSONEncodable) -> str:
+def json_dumps(obj: JSONSerializable) -> str:
     """Encode an object as JSON.
 
     Args:
-        obj (JSONEncodable): Object to encode.
+        obj (JSONSerializable): Object to encode.
 
     Returns:
         str: Object encoded as JSON.
 
     Raises:
         JSONEncodeError: If the object could not be encoded.
     """
     try:
         return rapidjson.dumps(obj, default=str, number_mode=rapidjson.NM_NATIVE)
-    except JSONEncodeError as err:
-        raise err
+    except (TypeError, ValueError) as err:
+        raise JSONEncodeError("Could not encode object") from err
 
 
-def jsonl_dumps(objs: Iterable[JSONEncodable]) -> str:
+def jsonl_dumps(objs: Iterable[JSONSerializable]) -> str:
     """Encode objects as JSONL.
 
     Args:
-        objs (Iterable[JSONEncodable]): Objects to encode.
+        objs (Iterable[JSONSerializable]): Objects to encode.
 
     Returns:
         str: Objects encoded as JSONL.
 
     Raises:
-        JSONEncodeError: If the object could not be encoded.
+        JSONEncodeError: If the objects could not be encoded.
     """
-    return "\n".join(map(lambda line: json_dumps(line), objs))
+    try:
+        return "\n".join(map(json_dumps, objs))
+    except JSONEncodeError as err:
+        raise JSONEncodeError("Could not encode objects") from err
 
 
-def json_dump(file_path: str, obj: JSONEncodable) -> None:
+def json_dump(obj: JSONSerializable, file_path: str) -> None:
     """Encode an object as JSON and write it to a file.
 
     Args:
         file_path (str): Path of the file to open.
-        obj (JSONEncodable): Object to encode.
 
     Raises:
         JSONEncodeError: If the object could not be encoded.
     """
     file_path = resolve_path(file_path)
-    with open(file_path, mode="w", encoding="utf-8") as wf:
-        try:
+    try:
+        with open(file_path, mode="w", encoding="utf-8") as wf:
             rapidjson.dump(obj, wf, default=str, number_mode=rapidjson.NM_NATIVE)
-        except JSONEncodeError as err:
-            raise err
+    except (TypeError, ValueError) as err:
+        raise JSONEncodeError("Could not encode object") from err
 
 
-def jsonl_dump(file_path: str, objs: Iterable[JSONEncodable]) -> None:
+def jsonl_dump(objs: Iterable[JSONSerializable], file_path: str) -> None:
     """Encode objects as JSONL and write them to a file.
 
     Args:
+        objs (Iterable[JSONSerializable]): Objects to encode.
         file_path (str): Path of the file to open.
-        objs (Iterable[JSONEncodable]): Objects to encode.
 
     Raises:
-        JSONEncodeError: If the object could not be encoded.
+        JSONEncodeError: If the objects could not be encoded.
     """
     file_path = resolve_path(file_path)
-    with open(file_path, mode="w", encoding="utf-8") as wf:
-        wf.write(jsonl_dumps(objs))
+    try:
+        with open(file_path, mode="w", encoding="utf-8") as wf:
+            wf.write(jsonl_dumps(objs))
+    except JSONEncodeError as err:
+        raise JSONEncodeError("Could not encode objects") from err
 
 
-def json_loads(encoded_obj: str) -> JSONEncodable:
+def json_loads(encoded_obj: str) -> JSONSerializable:
     """Decode a JSON-encoded object.
 
     Args:
         encoded_obj (str): Object to decode.
 
     Returns:
-        JSONEncodable: Decoded object.
+        JSONSerializable: Decoded object.
 
     Raises:
         JSONDecodeError: If the object could not be decoded.
     """
     try:
         return rapidjson.loads(encoded_obj, number_mode=rapidjson.NM_NATIVE)
-    except JSONDecodeError as err:
-        raise err
+    except (TypeError, rapidjson.JSONDecodeError) as err:  # OverflowError)
+        raise JSONDecodeError("Could not decode object") from err
 
 
-def json_load(file_path: FilePath) -> JSONEncodable:
+def json_load(file_path: FilePath) -> JSONSerializable:
     """Decode a file containing a JSON-encoded object.
 
     Args:
         file_path (FilePath): Path of the file to open.
 
     Returns:
-        JSONEncodable: Decoded object.
+        JSONSerializable: Decoded object.
 
     Raises:
         JSONDecodeError: If the file could not be decoded.
     """
     file_path = resolve_path(file_path)
-    with open(file_path, mode="r", encoding="utf-8") as rf:
-        try:
+    try:
+        with open(file_path, mode="r", encoding="utf-8") as rf:
             return rapidjson.load(rf, number_mode=rapidjson.NM_NATIVE)
-        except JSONDecodeError as err:
-            raise err
+    except (TypeError, rapidjson.JSONDecodeError) as err:  # OverflowError)
+        raise JSONDecodeError(f"Could not decode file '{file_path}'") from err
 
 
 def jsonl_loader(
     file_path: FilePath,
     *,
-    allow_empty_lines: bool = True,
-) -> Generator[JSONEncodable, None, None]:
+    allow_empty_lines: bool = False,
+) -> Generator[JSONSerializable, None, None]:
     """Decode a file containing JSON-encoded objects, one per line.
 
     Args:
         file_path (FilePath): Path of the file to open.
-        allow_empty_lines (bool, optional): Whether to allow empty lines. Defaults to True.
+        allow_empty_lines (bool, optional): Whether to allow (skip) empty lines. Defaults to False.
 
     Yields:
-        JSONEncodable: Decoded object.
+        JSONSerializable: Decoded object.
 
     Raises:
         JSONDecodeError: If the line could not be decoded, or if an empty line was found and `allow_empty_lines` is False.
     """
     file_path = resolve_path(file_path)
     with open(file_path, mode="r", encoding="utf-8") as rf:
         for line in rf:
-            # Remove trailing newline
-            line = line[:-1]
+            # Remove trailing whitespace
+            line = line.rstrip()
             # Handle empty lines
             if not line:
                 if allow_empty_lines:
                     continue
                 else:
-                    raise JSONDecodeError("Empty line found")
-            yield json_loads(line)
+                    raise JSONDecodeError(f"Could not decode file '{file_path}'")
+            try:
+                decoded_obj = json_loads(line)
+            except JSONDecodeError as err:
+                raise JSONDecodeError(f"Could not decode file '{file_path}'") from err
+            yield decoded_obj
 
 
-def squeegee_loader(file_path: FilePath) -> Generator[JSONEncodable, None, None]:
+def squeegee_loader(file_path: FilePath) -> Generator[JSONSerializable, None, None]:
     """Automatically decode a file containing JSON-encoded objects.
 
     Supports multiple formats (JSON, JSONL, JSONL of JSONL, etc).
 
+    Todo:
+        * Add support for pretty-printed JSON that has been appended to a file.
+
+
     Args:
         file_path (FilePath): Path of the file to open.
 
     Yields:
-        JSONEncodable: Decoded object.
+        JSONSerializable: Decoded object.
 
     Raises:
         JSONDecodeError: If the line could not be decoded.
     """
     file_path = resolve_path(file_path)
 
     # Try to decode as JSON standard
@@ -227,87 +247,80 @@
         decoded_obj = json_load(file_path)
     except JSONDecodeError:
         decoded_obj = None
 
     if decoded_obj is not None:
         # Recognized as JSON (JSON standard)
         if isinstance(decoded_obj, list):
-            # List of objects (multiline)
+            # List of objects on multiple lines
             for single_content in decoded_obj:
                 yield single_content
-        elif isinstance(decoded_obj, dict):
-            # Single object (multiline)
+        else:
+            # Single object on multiple lines
             yield decoded_obj
     else:
         # Recognized as JSONL (JSON line)
         for decoded_obj in jsonl_loader(file_path, allow_empty_lines=True):
-            if isinstance(decoded_obj, dict):
-                # Single object (single line)
-                yield decoded_obj
-            elif isinstance(decoded_obj, list):
-                # List of objects (single line)
+            if isinstance(decoded_obj, list):
+                # List of objects on single line
                 for single_content in decoded_obj:
                     yield single_content
+            else:
+                # Single object on single line
+                yield decoded_obj
+    # TODO: Add support for mix of pretty-printed JSON and JSONL
 
 
-def gen_hash(obj: MD5Hashable) -> str | None:
+def gen_hash(obj: MD5Hashable) -> str:
     """Create an MD5 hash from a hashable object.
 
-    Note: Tuples and sets are not hashable, so they are converted to lists.
+    Note: Tuples and deques are not hashable, so they are converted to lists.
 
     Args:
         obj (MD5Hashable): Object to hash.
 
     Returns:
-        str | None: MD5 hash of the object, or None if object was an empty iterable.
+        str: MD5 hash of the object.
 
     Raises:
         HashEncodeError: If the object could not be encoded.
     """
-    hashed_obj = None
+    obj_b = None
     try:
         if isinstance(obj, bytes):
-            # Already bytes
             obj_b = obj
         elif isinstance(obj, str):
-            # Encode string
             obj_b = obj.encode("utf-8")
-        elif isinstance(obj, list):
-            # Encode list as JSONL-encoded list
-            obj_b = jsonl_dumps(obj).encode("utf-8")
-        elif isinstance(obj, (tuple, collections.deque)):
-            # Encode tuple or deque as JSONL-encoded list
-            obj_list = list(obj)
-            obj_b = jsonl_dumps(obj_list).encode("utf-8")
-        elif isinstance(obj, (dict, int, float, bool)):
-            # Encode remaining built-ins as JSON
+        elif isinstance(obj, (dict, int, float, bool, list)):
             obj_b = json_dumps(obj).encode("utf-8")
-        # Hash if not empty iterable
-        if obj_b is not None:
-            hashed_obj = md5(obj_b).hexdigest()
-    except HashEncodeError as err:
-        raise err
-    return hashed_obj
+        elif isinstance(obj, (tuple, deque)):
+            obj_list = list(obj)
+            obj_b = json_dumps(obj_list).encode("utf-8")
+    except (TypeError, json.JSONDecodeError) as err:
+        raise HashEncodeError("Could not hash object") from err
+    if obj_b is None:
+        raise HashEncodeError("Could not hash object")
+    return md5(obj_b).hexdigest()
 
 
-def pickle_dump(file_path: FilePath, obj: PickleSerializable) -> None:
+def pickle_dump(obj: PickleSerializable, file_path: FilePath) -> None:
     """Serialize an object as a pickle and write it to a file.
 
     Args:
+        obj (JSONSerializable): Object to serialize.
         file_path (FilePath): Path of the file to write.
-        obj (JSONEncodable): Object to serialize.
 
     Raises:
         PickleEncodeError: If the object could not be encoded.
     """
     with open(file_path, mode="wb") as wb:
         try:
             cloudpickle.dump(obj, wb)
-        except PickleEncodeError as err:
-            raise err
+        except (TypeError, cloudpickle.pickle.PicklingError) as err:
+            raise PickleEncodeError("Could not pickle object") from err
 
 
 def pickle_dumps(obj: PickleSerializable) -> bytes:
     """Serialize an object as a pickle.
 
     Args:
         obj (PickleSerializable): Object to serialize.
@@ -316,16 +329,16 @@
         bytes: Serialized object.
 
     Raises:
         PickleEncodeError: If the object could not be encoded.
     """
     try:
         return cloudpickle.dumps(obj)
-    except PickleEncodeError as err:
-        raise err
+    except (TypeError, cloudpickle.pickle.PicklingError) as err:
+        raise PickleEncodeError("Could not pickle object") from err
 
 
 def pickle_load(file_path: FilePath) -> PickleSerializable:
     """Deserialize a pickle-serialized object from a file.
 
     Note: Not safe for large files.
 
@@ -337,16 +350,16 @@
 
     Raises:
         PickleDecodeError: If the object could not be decoded.
     """
     with open(file_path, mode="rb") as rb:
         try:
             return cloudpickle.load(rb)
-        except PickleDecodeError as err:
-            raise err
+        except (TypeError, cloudpickle.pickle.UnpicklingError) as err:
+            raise PickleDecodeError("Could not unpickle object") from err
 
 
 def pickle_loads(serialized_obj: bytes) -> PickleSerializable:
     """Deserialize a pickle-serialized object.
 
     Args:
         serialized_obj (bytes): Object to deserialize.
@@ -355,9 +368,9 @@
         PickleSerializable: Deserialized object.
 
     Raises:
         PickleDecodeError: If the object could not be decoded.
     """
     try:
         return cloudpickle.loads(serialized_obj)
-    except PickleDecodeError as err:
-        raise err
+    except (TypeError, cloudpickle.pickle.UnpicklingError) as err:
+        raise PickleDecodeError("Could not unpickle object") from err
```

### Comparing `wvutils-1.0.2/src/wvutils/typing.py` & `wvutils-1.0.3/src/wvutils/type_aliases.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,89 @@
 """Custom type aliases and type variables.
 
 This module contains custom type aliases and type variables used throughout the package.
 """
+from __future__ import annotations
 
 import collections
 import io
+import os
 from collections.abc import Hashable
-from os import PathLike
-from typing import Literal, TypeAlias  # TypeVar
+from typing import TYPE_CHECKING, Literal
+
+if TYPE_CHECKING:
+    from typing import TypeAlias
 
 __all__ = [
     "AWSRegion",
     "FileObject",
     "FilePath",
-    "JSONEncodable",
+    "JSONSerializable",
     "MD5Hashable",
     "Mask",
     "Masks",
     "PickleSerializable",
     "Span",
     "Spans",
 ]
 
-# Path-like object (likely str or pathlib.Path)
-FilePath: TypeAlias = str | PathLike
 
-# File Object
+# Python types
+# DictKey: TypeAlias = str | int | float | bool | object | None
+FilePath: TypeAlias = str | os.PathLike[str]
+# FileObject: TypeAlias = io.IOBase | io.RawIOBase | io.BufferedIOBase | io.TextIOBase
 FileObject: TypeAlias = io.TextIOBase | io.BytesIO
 
-# Spans and Masks
+# Spans and masks
 Span: TypeAlias = list[int] | tuple[int, int]
 Spans: TypeAlias = list[Span] | collections.deque[Span]
 Mask: TypeAlias = str
 Masks: TypeAlias = list[Mask] | collections.deque[Mask]
 
 # Serialization
-JSONEncodable: TypeAlias = str | int | float | bool | list | dict
+JSONSerializable: TypeAlias = str | int | float | bool | list | dict | None
 PickleSerializable: TypeAlias = object
-MD5Hashable: TypeAlias = JSONEncodable | tuple | set | Hashable
+MD5Hashable: TypeAlias = JSONSerializable | tuple | Hashable
 
 # AWS
 AWSRegion: TypeAlias = Literal[
-    "us-east-2",
     "us-east-1",
+    "us-east-2",
     "us-west-1",
     "us-west-2",
-    "af-south-1",
-    "ap-east-1",
+    "ca-central-1",
+    "eu-north-1",
+    "eu-west-3",
+    "eu-west-2",
+    "eu-west-1",
+    "eu-central-1",
+    "eu-south-1",
     "ap-south-1",
-    "ap-northeast-3",
+    "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-southeast-1",
     "ap-southeast-2",
-    "ap-northeast-1",
-    "ca-central-1",
-    "eu-central-1",
-    "eu-west-1",
-    "eu-west-2",
-    "eu-south-1",
-    "eu-west-3",
-    "eu-north-1",
-    "me-south-1",
+    "ap-southeast-3",
+    "ap-east-1",
     "sa-east-1",
+    "cn-north-1",
+    "cn-northwest-1",
     "us-gov-east-1",
     "us-gov-west-1",
+    "us-gov-secret-1",
+    "us-gov-topsecret-1",
+    "us-gov-topsecret-2",
+    "me-south-1",
+    "af-south-1",
+    "eu-east-1",
+    "eu-central-2",
+    "ap-south-2",
+    "ap-southeast-3",
+    "me-south-2",
+    "eu-north-1",
+    "eu-south-1",
+    "me-west-1",
+    "ru-central-1",
+    "ap-southeast-4",
+    "ca-west-1",
 ]
```

### Comparing `wvutils-1.0.2/src/wvutils.egg-info/PKG-INFO` & `wvutils-1.0.3/src/wvutils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wvutils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Collection of common utilities.
 Author-email: The Phosmic Development Team <dev@phosmic.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -789,22 +789,22 @@
 - _Session_ - Boto3 session.
 
 <a id="wvutils.aws.clear_boto3_sessions"></a>
 
 #### `clear_boto3_sessions`
 
 ```python
-def clear_boto3_sessions()
+def clear_boto3_sessions() -> int
 ```
 
 Clear all globally shared Boto3 sessions (thread-safe).
 
 **Returns**:
 
-- _bool_ - Whether any sessions were cleared.
+- _int_ - Number of sessions cleared.
 
 <a id="wvutils.aws.boto3_client_ctx"></a>
 
 #### `boto3_client_ctx`
 
 ```python
 @contextmanager
@@ -853,26 +853,26 @@
 #### `download_from_s3`
 
 ```python
 def download_from_s3(file_path: FilePath,
                      bucket_name: str,
                      bucket_path: str,
                      region_name: AWSRegion,
-                     overwrite: bool = True) -> None
+                     overwrite: bool = False) -> None
 ```
 
 Download a file from S3.
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Output path to use while downloading the file.
 - `bucket_name` _str_ - Name of the S3 bucket containing the file.
 - `bucket_path` _str_ - Path of the S3 bucket containing the file.
 - `region_name` _AWSRegion_ - Region name for S3.
-- `overwrite` _bool_ - Overwrite file on disk if already exists. Defaults to True.
+- `overwrite` _bool_ - Overwrite file on disk if already exists. Defaults to False.
 
 **Raises**:
 
 - `FileExistsError` - If the file already exists and overwrite is False.
 
 <a id="wvutils.aws.upload_file_to_s3"></a>
 
@@ -996,14 +996,112 @@
 Stop the execution of a query in Athena.
 
 **Arguments**:
 
 - `qeid` _str_ - Query execution ID of the query to stop.
 - `region_name` _AWSRegion_ - Region name for Athena.
 
+<a id="wvutils.errors"></a>
+
+# `wvutils.errors`
+
+Custom errors.
+
+This module contains custom exceptions that are used throughout the package.
+
+<a id="wvutils.errors.WVUtilsError"></a>
+
+## `WVUtilsError` Objects
+
+```python
+class WVUtilsError(Exception)
+```
+
+Base class for all wvutils exceptions.
+
+<a id="wvutils.errors.JSONError"></a>
+
+## `JSONError` Objects
+
+```python
+class JSONError(Exception)
+```
+
+Base class for all JSON exceptions.
+
+<a id="wvutils.errors.JSONEncodeError"></a>
+
+## `JSONEncodeError` Objects
+
+```python
+class JSONEncodeError(JSONError, TypeError)
+```
+
+Raised when JSON serializing fails.
+
+<a id="wvutils.errors.JSONDecodeError"></a>
+
+## `JSONDecodeError` Objects
+
+```python
+class JSONDecodeError(JSONError, ValueError)
+```
+
+Raised when JSON deserializing fails.
+
+<a id="wvutils.errors.PickleError"></a>
+
+## `PickleError` Objects
+
+```python
+class PickleError(Exception)
+```
+
+Base class for all pickle exceptions.
+
+<a id="wvutils.errors.PickleEncodeError"></a>
+
+## `PickleEncodeError` Objects
+
+```python
+class PickleEncodeError(PickleError, TypeError)
+```
+
+Raised when pickle serializing fails.
+
+<a id="wvutils.errors.PickleDecodeError"></a>
+
+## `PickleDecodeError` Objects
+
+```python
+class PickleDecodeError(PickleError, ValueError)
+```
+
+Raised when unpickling fails.
+
+<a id="wvutils.errors.HashError"></a>
+
+## `HashError` Objects
+
+```python
+class HashError(Exception)
+```
+
+Base class for all hashing exceptions.
+
+<a id="wvutils.errors.HashEncodeError"></a>
+
+## `HashEncodeError` Objects
+
+```python
+class HashEncodeError(HashError, TypeError)
+```
+
+Raised when hashing fails.
+
 <a id="wvutils.path"></a>
 
 # `wvutils.path`
 
 Utilities for working with paths.
 
 This module provides utilities for working with paths.
@@ -1014,14 +1112,16 @@
 
 ```python
 def is_pathlike(potential_path: Any) -> bool
 ```
 
 Check if an object is path-like.
 
+An object is path-like if it is a string or has a `__fspath__` method.
+
 **Arguments**:
 
 - `potential_path` _Any_ - Object to check.
 
 **Returns**:
 
 - _bool_ - True if the object is path-like, otherwise False.
@@ -1032,22 +1132,29 @@
 
 ```python
 def stringify_path(file_path: FilePath) -> str
 ```
 
 Stringify a path-like object.
 
+The path-like object is first converted to a string, then the user directory is expanded.
+> An object is path-like if it is a string or has a `__fspath__` method.
+
 **Arguments**:
 
 - `file_path` _FilePath_ - Path-like object to stringify.
 
 **Returns**:
 
 - _str_ - Path-like object as a string.
 
+**Raises**:
+
+- `TypeError` - If the object is not path-like.
+
 <a id="wvutils.path.ensure_abspath"></a>
 
 #### `ensure_abspath`
 
 ```python
 def ensure_abspath(file_path: str) -> str
 ```
@@ -1068,22 +1175,29 @@
 
 ```python
 def resolve_path(file_path: FilePath) -> str
 ```
 
 Stringify and resolve a path-like object.
 
+The path-like object is first converted to a string, then the user directory is expanded, and finally the path is resolved to an absolute path.
+> An object is path-like if it is a string or has a `__fspath__` method.
+
 **Arguments**:
 
 - `file_path` _FilePath_ - Path-like object to resolve.
 
 **Returns**:
 
 - _str_ - Absolute path of the path-like object as a string.
 
+**Raises**:
+
+- `TypeError` - If the object is not path-like.
+
 <a id="wvutils.path.xdg_cache_path"></a>
 
 #### `xdg_cache_path`
 
 ```python
 def xdg_cache_path() -> str
 ```
@@ -1123,17 +1237,20 @@
 
 ```python
 def add_proxies(proxies: list[str], include_duplicates: bool = False) -> None
 ```
 
 Add additional proxy addresses.
 
+All proxy addresses added will be added to the end of the list.
+
 **Arguments**:
 
 - `proxies` _list[str]_ - List of proxy addresses.
+- `include_duplicates` _bool, optional_ - Whether to include duplicates. Defaults to False.
 
 <a id="wvutils.proxies.ProxyManager.set_proxies"></a>
 
 #### `ProxyManager.set_proxies`
 
 ```python
 def set_proxies(proxies: list[str]) -> None
@@ -1201,14 +1318,18 @@
 
 - `address` _str_ - HTTPS proxy address.
 
 **Returns**:
 
 - _str_ - HTTP proxy address.
 
+**Raises**:
+
+- `ValueError` - If the address does not start with 'http://' or 'https://'.
+
 <a id="wvutils.proxies.prepare_http_proxy_for_requests"></a>
 
 #### `prepare_http_proxy_for_requests`
 
 ```python
 def prepare_http_proxy_for_requests(address: str) -> dict[str, str]
 ```
@@ -1221,35 +1342,35 @@
 
 **Returns**:
 
 - _dict[str, str]_ - Dictionary of HTTP and HTTPS proxy addresses.
 
 **Raises**:
 
-- `ValueError` - If the address does not start with 'http(s)://'.
+- `ValueError` - If the address does not start with 'http://' or 'https://'.
 
 <a id="wvutils.args"></a>
 
 # `wvutils.args`
 
 Utilities for parsing arguments from the command line.
 
 This module provides utilities for parsing arguments from the command line.
 
 <a id="wvutils.args.nonempty_string"></a>
 
 #### `nonempty_string`
 
 ```python
-def nonempty_string(name: str) -> Callable
+def nonempty_string(name: str) -> Callable[[str], str]
 ```
 
 Ensure a string is non-empty.
 
-Example Usage:
+**Example**:
 
 ```python
 subparser.add_argument(
     "hashtag",
     type=nonempty_string("hashtag"),
     help="A hashtag (without #)",
 )
@@ -1257,68 +1378,90 @@
 
 **Arguments**:
 
 - `name` _str_ - Name of the function, used for debugging.
 
 **Returns**:
 
-- _Callable_ - The decorated function.
+- _Callable[[str], str]_ - The decorated function.
 
 <a id="wvutils.args.safechars_string"></a>
 
 #### `safechars_string`
 
 ```python
 def safechars_string(
-    name: str,
-    allowed_chars: str | set[str] | tuple[str] | list[str] | None = None
-) -> Callable
+        name: str,
+        allowed_chars: Collection[str] | None = None) -> Callable[[str], str]
 ```
 
 Ensure a string contains only safe characters.
 
-Example Usage:
+**Example**:
 
 ```python
 subparser.add_argument(
     "--session-key",
     type=safechars_string,
     help="Key to share a single token across processes",
 )
 ```
 
 **Arguments**:
 
 - `name` _str_ - Name of the function, used for debugging.
-- `allowed_chars` _str | set[str] | tuple[str] | list[str] | None, optional_ - Custom characters used to validate the function name. Defaults to None.
+- `allowed_chars` _Collection[str] | None, optional_ - Custom characters used to validate the function name. Defaults to None.
 
 **Returns**:
 
-- _Callable_ - The decorated function.
+- _Callable[[str], str]_ - The decorated function.
+
+**Raises**:
+
+- `ValueError` - If empty collection of allowed characters is provided.
 
 <a id="wvutils.general"></a>
 
 # `wvutils.general`
 
 General utilities for working with Python.
 
 This module provides general utilities for working with Python.
 
+<a id="wvutils.general.is_iolike"></a>
+
+#### `is_iolike`
+
+```python
+def is_iolike(potential_io: Any) -> bool
+```
+
+Check if an object is IO-like.
+
+**Arguments**:
+
+- `potential_io` _Any_ - Object to check.
+
+**Returns**:
+
+- _bool_ - True if the object is IO-like, otherwise False.
+
 <a id="wvutils.general.count_lines_in_file"></a>
 
 #### `count_lines_in_file`
 
 ```python
 def count_lines_in_file(file_path: FilePath) -> int
 ```
 
-Count the Number of Lines in a File
+Count the number of lines in a file.
+
+**Notes**:
 
-All files have at least 1 line:
-number of lines = # of newlines + 1
+  All files have at least 1 line (# of lines = # of newlines + 1).
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to count lines in.
 
 **Returns**:
 
@@ -1328,15 +1471,15 @@
 
 #### `sys_set_recursion_limit`
 
 ```python
 def sys_set_recursion_limit() -> None
 ```
 
-Raise Recursion Limit to Allow for More Recurse
+Raise recursion limit to allow for more recurse.
 
 <a id="wvutils.general.gc_set_threshold"></a>
 
 #### `gc_set_threshold`
 
 ```python
 def gc_set_threshold() -> None
@@ -1353,34 +1496,38 @@
 #### `chunker`
 
 ```python
 def chunker(seq: Sequence[Any],
             n: int) -> Generator[Sequence[Any], None, None]
 ```
 
-Iterate a Sequence in Chunks
+Iterate a sequence in size `n` chunks.
 
 **Arguments**:
 
 - `seq` _Sequence[Any]_ - Sequence of values.
 - `n` _int_ - Number of values per chunk.
 
 **Yields**:
 
 - _Sequence[Any]_ - Chunk of values with length <= n.
 
+**Raises**:
+
+- `ValueError` - If `n` is 0 or negative.
+
 <a id="wvutils.general.is_iterable"></a>
 
 #### `is_iterable`
 
 ```python
 def is_iterable(obj: Any) -> bool
 ```
 
-Check if an Object is Iterable
+Check if an object is iterable.
 
 **Arguments**:
 
 - `obj` _Any_ - Object to check.
 
 **Returns**:
 
@@ -1393,15 +1540,35 @@
 ```python
 def rename_key(obj: dict,
                src_key: str,
                dest_key: str,
                in_place: bool = False) -> dict | None
 ```
 
-Rename a Dictionary Key
+Rename a dictionary key.
+
+**Todo**:
+
+  * Add support for nested keys.
+  * Add support for renaming multiple keys at once.
+  * Add support for non-string (built-in) key types.
+
+  All of the following are True:
+
+  ```python
+  isinstance(True, bool)
+  isinstance(True, int)
+  1 == True
+  1 in {1: "a"}
+  True in {1: "a"}
+  1 in {True: "a"}
+  True in {True: "a"}
+  1 in {1: "a", True: "b"}
+  True in {1: "a", True: "b"}
+  ```
 
 **Arguments**:
 
 - `obj` _dict_ - Reference to the dictionary to modify.
 - `src` _str_ - Name of the key to rename.
 - `dest` _str_ - Name of the key to change to.
 - `in_place` _bool, optional_ - Perform in-place using the provided reference. Defaults to False.
@@ -1411,27 +1578,338 @@
 - _dict | None_ - Copy of the dictionary if in_place is False, otherwise None.
 
 <a id="wvutils.general.unnest_key"></a>
 
 #### `unnest_key`
 
 ```python
-def unnest_key(obj: dict, *keys: str) -> Any
+def unnest_key(obj: dict, *keys: str) -> Any | None
 ```
 
-Fetch a Value from a Deeply Nested Dictionary
+Fetch a value from a deeply nested dictionary.
 
 **Arguments**:
 
 - `obj` _dict_ - Dictionary to recursively iterate.
 - `*keys` _str_ - Ordered keys to fetch.
 
 **Returns**:
 
-- _Any_ - The result of the provided keys.
+- _Any | None_ - The result of the provided keys, or None if any key is not found.
+
+<a id="wvutils.general.sort_dict_by_key"></a>
+
+#### `sort_dict_by_key`
+
+```python
+def sort_dict_by_key(obj: dict,
+                     reverse: bool = False,
+                     deep_copy: bool = False) -> dict | None
+```
+
+Sort a dictionary by key.
+
+**Arguments**:
+
+- `obj` _dict_ - Dictionary to sort.
+- `reverse` _bool, optional_ - Sort in reverse order. Defaults to False.
+- `deep_copy` _bool, optional_ - Return a deep copy of the dictionary. Defaults to False.
+
+**Returns**:
+
+- _dict | None_ - Dictionary sorted by key. If `in_place` is True, None is returned.
+
+**Raises**:
+
+- `ValueError` - If the dictionary keys are not of the same type.
+
+<a id="wvutils.general.dedupe_list"></a>
+
+#### `dedupe_list`
+
+```python
+def dedupe_list(values: list[Any], raise_on_dupe: bool = False) -> list[Any]
+```
+
+Remove duplicate values from a list.
+
+**Example**:
+
+```python
+dedupe_list([1, 2, 3, 1, 2, 3])
+# [1, 2, 3]
+```
+
+**Arguments**:
+
+- `values` _list[Any]_ - List of values to dedupe.
+- `raise_on_dupe` _bool, optional_ - Raise an error if a duplicate is found. Defaults to False.
+
+**Returns**:
+
+- _list[Any]_ - List of unique values.
+
+**Raises**:
+
+- `ValueError` - If a duplicate is found and `raise_on_dupe` is True.
+
+<a id="wvutils.general.dupe_in_list"></a>
+
+#### `dupe_in_list`
+
+```python
+def dupe_in_list(values: list[Any]) -> bool
+```
+
+Check if a list has duplicate values.
+
+**Arguments**:
+
+- `values` _list[Any]_ - List of values to check.
+
+**Returns**:
+
+- _bool_ - Whether the list has duplicate values.
+
+<a id="wvutils.general.invert_dict_of_str"></a>
+
+#### `invert_dict_of_str`
+
+```python
+def invert_dict_of_str(obj: dict[Any, str],
+                       deep_copy: bool = False,
+                       raise_on_dupe: bool = False) -> dict
+```
+
+Invert a dictionary of strings.
+
+**Notes**:
+
+  The value of the last key with a given value will be used.
+
+**Example**:
+
+```python
+invert_dict_of_str({"a": "b", "c": "d"})
+# {"b": "a", "d": "c"}
+```
+
+**Arguments**:
+
+- `obj` _dict[Any, str]_ - Dictionary to invert.
+- `deep_copy` _bool, optional_ - Return a deep copy of the dictionary. Defaults to False.
+- `raise_on_dupe` _bool, optional_ - Raise an error if a duplicate is found. Defaults to False.
+
+**Returns**:
+
+- _dict_ - Inverted dictionary.
+
+**Raises**:
+
+- `ValueError` - If a duplicate is found and `raise_on_dupe` is True.
+
+<a id="wvutils.dt"></a>
+
+# `wvutils.dt`
+
+Datetime utilities.
+
+This module contains functions and classes that are used to work with datetimes.
+
+<a id="wvutils.dt.dtformats"></a>
+
+## `dtformats` Objects
+
+```python
+class dtformats()
+```
+
+Datetime formats.
+
+**Attributes**:
+
+- `twitter` _str_ - Twitter datetime format.
+- `reddit` _str_ - Reddit datetime format.
+- `general` _str_ - General datetime format.
+- `db` _str_ - Database datetime format.
+- `date` _str_ - Date format.
+- `time_12h` _str_ - 12-hour time format with timezone.
+- `time_24h` _str_ - 24-hour time format with timezone.
+
+<a id="wvutils.dt.num_days_in_month"></a>
+
+#### `num_days_in_month`
+
+```python
+def num_days_in_month(year: int, month: int) -> int
+```
+
+Determine the number of days in a month.
+
+**Arguments**:
+
+- `year` _int_ - Year to check.
+- `month` _int_ - Month to check.
+
+**Returns**:
+
+- _int_ - Number of days in the month.
+
+<a id="wvutils.parquet"></a>
+
+# `wvutils.parquet`
+
+Parquet utilities.
+
+This module provides utilities for working with Parquet files.
+
+<a id="wvutils.parquet.get_parquet_session"></a>
+
+#### `get_parquet_session`
+
+```python
+def get_parquet_session(use_s3: bool,
+                        region_name: AWSRegion | None = None) -> fs.FileSystem
+```
+
+Get the globally shared Parquet filesystem session.
+
+**Todo**:
+
+  * Add support for other session parameters.
+
+**Arguments**:
+
+- `use_s3` _bool_ - Use S3 if True, otherwise uses local filesystem.
+- `region_name` _AWSRegion | None, optional_ - AWS region name. Defaults to None.
+
+  
+
+**Returns**:
+
+- _pyarrow.fs.FileSystem_ - The filesystem session.
+
+<a id="wvutils.parquet.clear_parquet_sessions"></a>
+
+#### `clear_parquet_sessions`
+
+```python
+def clear_parquet_sessions() -> int
+```
+
+Clear all globally shared Parquet filesystem sessions.
+
+**Returns**:
+
+- _int_ - Number of sessions cleared.
+
+<a id="wvutils.parquet.create_pa_schema"></a>
+
+#### `create_pa_schema`
+
+```python
+def create_pa_schema(schema_template: dict[str, str]) -> pa.schema
+```
+
+Create a parquet schema from a template.
+
+**Example**:
+
+```python
+{
+    "key_a": "string",
+    "key_b": "integer",
+    "key_c": "float",
+    "key_d": "bool",
+    "key_e": "timestamp[s]",
+    "key_f": "timestamp[ms]",
+    "key_g": "timestamp[ns]",
+}
+```
+
+  becomes
+
+```python
+pa.schema([
+    ("key_a", pa.string()),
+    ("key_b", pa.int64()),
+    ("key_c", pa.float64()),
+    ("key_d", pa.bool_()),
+    ("key_e", pa.timestamp("s",  tz=utc)),
+    ("key_f", pa.timestamp("ms", tz=utc)),
+    ("key_g", pa.timestamp("ns", tz=utc)),
+])
+```
+
+**Arguments**:
+
+- `schema_template` _Sequence[Sequence[str]]_ - Data names and parquet types for creating the schema.
+
+**Returns**:
+
+- _pa.schema_ - Final parquet schema.
+
+**Raises**:
+
+- `ValueError` - If an unknown type name is encountered.
+
+<a id="wvutils.parquet.force_dataframe_dtypes"></a>
+
+#### `force_dataframe_dtypes`
+
+```python
+def force_dataframe_dtypes(dataframe: pd.DataFrame,
+                           template: dict[str, str]) -> pd.DataFrame
+```
+
+Force the data types of a dataframe using a template.
+
+**Arguments**:
+
+- `dataframe` _pd.DataFrame_ - Dataframe to force types.
+- `template` _dict[str, str]_ - Template to use for forcing types.
+
+**Returns**:
+
+- _pd.DataFrame_ - Dataframe with forced types.
+
+**Raises**:
+
+- `ValueError` - If an unknown type name is encountered.
+
+<a id="wvutils.parquet.export_dataset"></a>
+
+#### `export_dataset`
+
+```python
+def export_dataset(data: list[dict] | deque[dict] | pd.DataFrame,
+                   output_location: str | FilePath,
+                   primary_template: dict[str, str],
+                   partitions_template: dict[str, str],
+                   *,
+                   basename_template: str | None = None,
+                   use_s3: bool = False,
+                   region_name: AWSRegion | None = None,
+                   use_threads: bool = False,
+                   overwrite: bool = False) -> None
+```
+
+Write to dataset to local filesystem or AWS S3.
+
+**Arguments**:
+
+- `data` _list[dict] | deque[dict] | pd.DataFrame]_ - List, deque, or dataframe of objects to be written.
+- `output_location` _str | FilePath_ - Location to write the dataset to.
+- `primary_template` _dict[str, str]_ - Parquet schema template to use for the table (excluding partitions).
+  partitions_template(dict[str, str]): Parquet schema template to use for the partitions.
+- `basename_template` _str, optional_ - Filename template to use when writing to S3 or locally. Defaults to None.
+- `use_s3` _bool, optional_ - Use S3 as the destination when exporting parquet files. Defaults to False.
+- `region_name` _AWSRegion, optional_ - AWS region to use when exporting to S3. Defaults to None.
+- `use_threads` _bool, optional_ - Use multiple threads when exporting. Defaults to False.
+- `overwrite` _bool, optional_ - Overwrite existing files. Defaults to False.
 
 <a id="wvutils.restruct"></a>
 
 # `wvutils.restruct`
 
 Utilities for restructuring data.
 
@@ -1463,225 +1941,230 @@
 Read more: https://github.com/cloudpipe/cloudpickle/blob/master/README.md#overriding-pickles-serialization-mechanism-for-importable-constructs
 
 <a id="wvutils.restruct.json_dumps"></a>
 
 #### `json_dumps`
 
 ```python
-def json_dumps(obj: JSONEncodable) -> str
+def json_dumps(obj: JSONSerializable) -> str
 ```
 
 Encode an object as JSON.
 
 **Arguments**:
 
-- `obj` _JSONEncodable_ - Object to encode.
+- `obj` _JSONSerializable_ - Object to encode.
 
 **Returns**:
 
 - _str_ - Object encoded as JSON.
 
 **Raises**:
 
 - `JSONEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.jsonl_dumps"></a>
 
 #### `jsonl_dumps`
 
 ```python
-def jsonl_dumps(objs: Iterable[JSONEncodable]) -> str
+def jsonl_dumps(objs: Iterable[JSONSerializable]) -> str
 ```
 
 Encode objects as JSONL.
 
 **Arguments**:
 
-- `objs` _Iterable[JSONEncodable]_ - Objects to encode.
+- `objs` _Iterable[JSONSerializable]_ - Objects to encode.
 
 **Returns**:
 
 - _str_ - Objects encoded as JSONL.
 
 **Raises**:
 
-- `JSONEncodeError` - If the object could not be encoded.
+- `JSONEncodeError` - If the objects could not be encoded.
 
 <a id="wvutils.restruct.json_dump"></a>
 
 #### `json_dump`
 
 ```python
-def json_dump(file_path: str, obj: JSONEncodable) -> None
+def json_dump(obj: JSONSerializable, file_path: str) -> None
 ```
 
 Encode an object as JSON and write it to a file.
 
 **Arguments**:
 
 - `file_path` _str_ - Path of the file to open.
-- `obj` _JSONEncodable_ - Object to encode.
 
 **Raises**:
 
 - `JSONEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.jsonl_dump"></a>
 
 #### `jsonl_dump`
 
 ```python
-def jsonl_dump(file_path: str, objs: Iterable[JSONEncodable]) -> None
+def jsonl_dump(objs: Iterable[JSONSerializable], file_path: str) -> None
 ```
 
 Encode objects as JSONL and write them to a file.
 
 **Arguments**:
 
+- `objs` _Iterable[JSONSerializable]_ - Objects to encode.
 - `file_path` _str_ - Path of the file to open.
-- `objs` _Iterable[JSONEncodable]_ - Objects to encode.
 
 **Raises**:
 
-- `JSONEncodeError` - If the object could not be encoded.
+- `JSONEncodeError` - If the objects could not be encoded.
 
 <a id="wvutils.restruct.json_loads"></a>
 
 #### `json_loads`
 
 ```python
-def json_loads(encoded_obj: str) -> JSONEncodable
+def json_loads(encoded_obj: str) -> JSONSerializable
 ```
 
 Decode a JSON-encoded object.
 
 **Arguments**:
 
 - `encoded_obj` _str_ - Object to decode.
 
 **Returns**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the object could not be decoded.
 
 <a id="wvutils.restruct.json_load"></a>
 
 #### `json_load`
 
 ```python
-def json_load(file_path: FilePath) -> JSONEncodable
+def json_load(file_path: FilePath) -> JSONSerializable
 ```
 
 Decode a file containing a JSON-encoded object.
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to open.
 
 **Returns**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the file could not be decoded.
 
 <a id="wvutils.restruct.jsonl_loader"></a>
 
 #### `jsonl_loader`
 
 ```python
 def jsonl_loader(
-        file_path: FilePath,
-        *,
-        allow_empty_lines: bool = True
-) -> Generator[JSONEncodable, None, None]
+    file_path: FilePath,
+    *,
+    allow_empty_lines: bool = False
+) -> Generator[JSONSerializable, None, None]
 ```
 
 Decode a file containing JSON-encoded objects, one per line.
 
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to open.
-- `allow_empty_lines` _bool, optional_ - Whether to allow empty lines. Defaults to True.
+- `allow_empty_lines` _bool, optional_ - Whether to allow (skip) empty lines. Defaults to False.
 
 **Yields**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the line could not be decoded, or if an empty line was found and `allow_empty_lines` is False.
 
 <a id="wvutils.restruct.squeegee_loader"></a>
 
 #### `squeegee_loader`
 
 ```python
 def squeegee_loader(
-        file_path: FilePath) -> Generator[JSONEncodable, None, None]
+        file_path: FilePath) -> Generator[JSONSerializable, None, None]
 ```
 
 Automatically decode a file containing JSON-encoded objects.
 
 Supports multiple formats (JSON, JSONL, JSONL of JSONL, etc).
 
+**Todo**:
+
+  * Add support for pretty-printed JSON that has been appended to a file.
+
+  
+
 **Arguments**:
 
 - `file_path` _FilePath_ - Path of the file to open.
 
 **Yields**:
 
-- _JSONEncodable_ - Decoded object.
+- _JSONSerializable_ - Decoded object.
 
 **Raises**:
 
 - `JSONDecodeError` - If the line could not be decoded.
 
 <a id="wvutils.restruct.gen_hash"></a>
 
 #### `gen_hash`
 
 ```python
-def gen_hash(obj: MD5Hashable) -> str | None
+def gen_hash(obj: MD5Hashable) -> str
 ```
 
 Create an MD5 hash from a hashable object.
 
-Note: Tuples and sets are not hashable, so they are converted to lists.
+Note: Tuples and deques are not hashable, so they are converted to lists.
 
 **Arguments**:
 
 - `obj` _MD5Hashable_ - Object to hash.
 
 **Returns**:
 
-- _str | None_ - MD5 hash of the object, or None if object was an empty iterable.
+- _str_ - MD5 hash of the object.
 
 **Raises**:
 
 - `HashEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.pickle_dump"></a>
 
 #### `pickle_dump`
 
 ```python
-def pickle_dump(file_path: FilePath, obj: PickleSerializable) -> None
+def pickle_dump(obj: PickleSerializable, file_path: FilePath) -> None
 ```
 
 Serialize an object as a pickle and write it to a file.
 
 **Arguments**:
 
+- `obj` _JSONSerializable_ - Object to serialize.
 - `file_path` _FilePath_ - Path of the file to write.
-- `obj` _JSONEncodable_ - Object to serialize.
 
 **Raises**:
 
 - `PickleEncodeError` - If the object could not be encoded.
 
 <a id="wvutils.restruct.pickle_dumps"></a>
```

### Comparing `wvutils-1.0.2/src/wvutils.egg-info/SOURCES.txt` & `wvutils-1.0.3/src/wvutils.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 pyproject.toml
 setup.py
 src/wvutils/__init__.py
 src/wvutils/args.py
 src/wvutils/aws.py
 src/wvutils/compat.py
 src/wvutils/constants.py
+src/wvutils/dt.py
 src/wvutils/errors.py
 src/wvutils/general.py
+src/wvutils/parquet.py
 src/wvutils/path.py
 src/wvutils/proxies.py
 src/wvutils/restruct.py
-src/wvutils/typing.py
+src/wvutils/type_aliases.py
 src/wvutils.egg-info/PKG-INFO
 src/wvutils.egg-info/SOURCES.txt
 src/wvutils.egg-info/dependency_links.txt
 src/wvutils.egg-info/requires.txt
 src/wvutils.egg-info/top_level.txt
 tests/test_args.py
 tests/test_aws.py
+tests/test_constants.py
+tests/test_dt.py
+tests/test_general.py
+tests/test_parquet.py
 tests/test_path.py
 tests/test_proxies.py
-tests/test_utils.py
+tests/test_restruct.py
```

### Comparing `wvutils-1.0.2/tests/test_aws.py` & `wvutils-1.0.3/tests/test_aws.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,68 @@
 import json
 import os
 import tempfile
 import unittest
 from unittest.mock import Mock, patch
 
 import boto3
+import pytest
 from botocore.exceptions import ClientError
 from moto import mock_s3, mock_secretsmanager
 
 from wvutils.aws import (
     athena_retrieve_query,
+    athena_stop_query,
+    boto3_client_ctx,
     clear_boto3_sessions,
     download_from_s3,
     get_boto3_session,
     parse_s3_uri,
     secrets_fetch,
-    shared_boto3_ctx,
     upload_bytes_to_s3,
     upload_file_to_s3,
 )
 
-
-class TestParseS3Uri(unittest.TestCase):
-    def test_parse_s3_uri(self):
-        self.assertTupleEqual(
-            parse_s3_uri("s3://my-bucket/my-path"),
-            ("my-bucket", "my-path"),
-        )
-
-    def test_parse_s3_uri_no_path(self):
-        self.assertTupleEqual(
-            parse_s3_uri("s3://my-bucket"),
-            ("my-bucket", ""),
-        )
-
-    def test_parse_s3_uri_no_scheme(self):
-        self.assertTupleEqual(
-            parse_s3_uri("my-bucket/my-path"),
-            ("my-bucket", "my-path"),
-        )
+# @pytest.fixture(scope="function")
+# def boto3_client_mock():
+#     client_mock = Mock()
+#     return client_mock
+
+
+# @pytest.fixture(scope="function")
+# def boto3_session_mock(boto3_client_mock):
+#     session_mock = Mock()
+#     session_mock.client.return_value = boto3_client_mock
+#     return session_mock
+
+
+# @pytest.fixture(scope="function")
+# def clear_boto3_sessions_fixture():
+#     yield
+#     clear_boto3_sessions()
+
+
+# @pytest.fixture(scope="function")
+# def s3_client_mock():
+#     with mock_s3():
+#         s3_client = boto3.client("s3", region_name="us-east-1")
+#         s3_client.create_bucket(Bucket="my-bucket")
+#         yield s3_client
+
+
+@pytest.mark.parametrize(
+    "s3_uri,expected",
+    [
+        ("s3://my-bucket/my-path", ("my-bucket", "my-path")),
+        ("s3://my-bucket", ("my-bucket", "")),
+        ("my-bucket/my-path", ("my-bucket", "my-path")),
+    ],
+)
+def test_parse_s3_uri(s3_uri, expected):
+    assert parse_s3_uri(s3_uri) == expected
 
 
 class TestAWSSessions(unittest.TestCase):
     def setUp(self):
         self.region_name1 = "us-east-1"
         self.region_name2 = "us-west-2"
 
@@ -60,15 +80,17 @@
         # Check that a different session is returned for a different region
         self.assertIsNot(session1, session3)
 
     def test_clear_boto3_sessions(self):
         # These sessions will persist for the duration of this method after clearing the global sessions
         session1 = get_boto3_session(self.region_name1)
         session2 = get_boto3_session(self.region_name2)
-        clear_boto3_sessions()
+        num_sessions_cleared = clear_boto3_sessions()
+        # Check that the correct number of sessions were cleared
+        self.assertEqual(num_sessions_cleared, 2)
         # Any new sessions will be different from the previous ones
         session3 = get_boto3_session(self.region_name1)
         session4 = get_boto3_session(self.region_name2)
         # Check that the sessions are different before/after clearing
         self.assertIsNot(session1, session3)
         self.assertIsNot(session2, session4)
 
@@ -76,15 +98,15 @@
 class TestAWSContextHelper(unittest.TestCase):
     def setUp(self):
         self.service_name = "s3"
         self.region_name = "us-east-1"
         self.session_mock = Mock()
         self.client_mock = Mock()
         self.session_mock.client.return_value = self.client_mock
-        self.context_manager = shared_boto3_ctx(self.service_name, self.region_name)
+        self.context_manager = boto3_client_ctx(self.service_name, self.region_name)
 
     def tearDown(self):
         # Reset the global boto3 sessions
         clear_boto3_sessions()
 
     def test_boto3_resource(self):
         with patch("wvutils.aws.Session", return_value=self.session_mock):
@@ -181,14 +203,15 @@
     def test_download_from_s3_with_overwrite_existing(self):
         overwrite = True
         with tempfile.NamedTemporaryFile() as twf:
             # Create a file with some content
             with open(twf.name, mode="wb") as wbf:
                 wbf.write("Some other content".encode("utf-8"))
             # Download the file from S3
+            # check for warnings.warn
             download_from_s3(
                 twf.name,
                 self.bucket_name,
                 self.bucket_path,
                 self.region_name,
                 overwrite=overwrite,
             )
@@ -231,18 +254,18 @@
                 Key=self.bucket_path,
             )
             self.assertEqual(
                 s3_object["Body"].read().decode("utf-8"),
                 "Hello World!",
             )
 
-    def test_upload_file_to_s3_with_non_existent_file(self):
+    def test_upload_file_to_s3_with_nonexistent_file(self):
         with self.assertRaises(FileNotFoundError):
             upload_file_to_s3(
-                "/tmp/non-existent-file",
+                "/tmp/nonexistent-file",
                 self.bucket_name,
                 self.bucket_path,
                 self.region_name,
             )
 
 
 @mock_s3
@@ -378,34 +401,64 @@
             state_or_s3_uri = athena_retrieve_query(
                 self.query_execution_id,
                 self.database_name,
                 self.region_name,
             )
         self.assertEqual(state_or_s3_uri, self.s3_output_location)
 
-    def test_query_state_unexpected_type(self):
+    def test_query_state_unexpected_value(self):
+        self.client_mock.get_query_execution.return_value = {
+            "QueryExecution": {
+                "QueryExecutionId": self.query_execution_id,
+                "Status": {"State": "SOMETHING ELSE"},
+            },
+        }
+        with patch("wvutils.aws.Session", return_value=self.session_mock):
+            with self.assertRaises(ValueError):
+                athena_retrieve_query(
+                    self.query_execution_id,
+                    self.database_name,
+                    self.region_name,
+                )
+
+    def test_query_state_unexpected_type_of_None(self):
+        self.client_mock.get_query_execution.return_value = {
+            "QueryExecution": {
+                "QueryExecutionId": self.query_execution_id,
+                "Status": {"State": None},
+            },
+        }
+        with patch("wvutils.aws.Session", return_value=self.session_mock):
+            with self.assertRaises(ValueError):
+                athena_retrieve_query(
+                    self.query_execution_id,
+                    self.database_name,
+                    self.region_name,
+                )
+
+    def test_query_state_unexpected_type_of_int(self):
         self.client_mock.get_query_execution.return_value = {
             "QueryExecution": {
                 "QueryExecutionId": self.query_execution_id,
                 "Status": {"State": 1},
             },
         }
         with patch("wvutils.aws.Session", return_value=self.session_mock):
             with self.assertRaises(ValueError):
                 athena_retrieve_query(
                     self.query_execution_id,
                     self.database_name,
                     self.region_name,
                 )
 
-    def test_query_state_unexpected_value(self):
+    def test_query_state_unexpected_type_of_float(self):
         self.client_mock.get_query_execution.return_value = {
             "QueryExecution": {
                 "QueryExecutionId": self.query_execution_id,
-                "Status": {"State": "SOMETHING ELSE"},
+                "Status": {"State": 1.1},
             },
         }
         with patch("wvutils.aws.Session", return_value=self.session_mock):
             with self.assertRaises(ValueError):
                 athena_retrieve_query(
                     self.query_execution_id,
                     self.database_name,
@@ -422,7 +475,27 @@
         with patch("wvutils.aws.Session", return_value=self.session_mock):
             with self.assertRaises(ValueError):
                 athena_retrieve_query(
                     self.query_execution_id,
                     self.database_name,
                     self.region_name,
                 )
+
+
+class TestAthenaStopQuery(unittest.TestCase):
+    def setUp(self):
+        self.region_name = "us-east-1"
+        self.query_execution_id = "abc1234d-5efg-67hi-jklm-89n0op12qr34"
+        self.session_mock = Mock()
+        self.client_mock = Mock()
+        self.session_mock.client.return_value = self.client_mock
+
+    def tearDown(self):
+        # Reset the global boto3 sessions
+        clear_boto3_sessions()
+
+    def test_stop_query(self):
+        with patch("wvutils.aws.Session", return_value=self.session_mock):
+            athena_stop_query(self.query_execution_id, self.region_name)
+        self.client_mock.stop_query_execution.assert_called_once_with(
+            QueryExecutionId=self.query_execution_id
+        )
```

### Comparing `wvutils-1.0.2/tests/test_proxies.py` & `wvutils-1.0.3/tests/test_proxies.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,110 +1,121 @@
-import unittest
+import pytest
 
 from wvutils.proxies import (
     ProxyManager,
     https_to_http,
     prepare_http_proxy_for_requests,
 )
 
 
-class TestHttpsToHttp(unittest.TestCase):
-    def test_https(self):
-        self.assertEqual(
-            https_to_http("https://localhost:8080"),
-            "http://localhost:8080",
-        )
+@pytest.mark.parametrize(
+    "address,expected",
+    [
+        ("https://localhost:8080", "http://localhost:8080"),
+        ("http://localhost:8080", "http://localhost:8080"),
+    ],
+)
+def test_https_to_http(address, expected):
+    assert https_to_http(address) == expected
 
-    def test_http(self):
-        self.assertEqual(
-            https_to_http("http://localhost:8080"),
-            "http://localhost:8080",
-        )
 
-    def test_invalid_address(self):
-        with self.assertRaises(ValueError):
-            https_to_http("localhost:8080")
+@pytest.mark.parametrize("address", ["localhost:8080", "ftp://localhost:8080", ""])
+def test_https_to_http_invalid_address(address):
+    with pytest.raises(ValueError, match=r"Invalid proxy address: .+"):
+        https_to_http(address)
 
 
-class TestProxies(unittest.TestCase):
-    def test_prepare_http_proxy_for_requests(self):
-        # Test using HTTP
-        address = "https://localhost:8080"
-        self.assertDictEqual(
-            prepare_http_proxy_for_requests(address),
+@pytest.mark.parametrize(
+    "address,expected",
+    [
+        (
+            "https://localhost:8080",
             {
                 "https_proxy": "https://localhost:8080",
                 "http_proxy": "http://localhost:8080",
                 "HTTPS_PROXY": "https://localhost:8080",
                 "HTTP_PROXY": "http://localhost:8080",
             },
-        )
-        # Test using HTTPS
-        address = "http://localhost:8080"
-        self.assertDictEqual(
-            prepare_http_proxy_for_requests(address),
+        ),
+        (
+            "http://localhost:8080",
             {
                 "https_proxy": "http://localhost:8080",
                 "http_proxy": "http://localhost:8080",
                 "HTTPS_PROXY": "http://localhost:8080",
                 "HTTP_PROXY": "http://localhost:8080",
             },
-        )
-        # Test using invalid (non-http/https) address
-        with self.assertRaises(ValueError):
-            prepare_http_proxy_for_requests("localhost:8080")
-
-    def test_proxy_manager(self):
-        proxies = ["https://proxy1.com", "https://proxy2.com", "https://proxy3.com"]
-        proxy_manager = ProxyManager(proxies, reuse=True)
-        # First cycle
-        self.assertEqual(proxy_manager.proxy, proxies[0])
-        self.assertTrue(proxy_manager.can_cycle)
-        # Second cycle
-        proxy_manager.cycle()
-        self.assertEqual(proxy_manager.proxy, proxies[1])
-        self.assertTrue(proxy_manager.can_cycle)
-        # Third cycle
-        proxy_manager.cycle()
-        self.assertEqual(proxy_manager.proxy, proxies[2])
-        self.assertTrue(proxy_manager.can_cycle)
-        # Cycle back to first proxy
-        proxy_manager.cycle()
-        self.assertEqual(proxy_manager.proxy, proxies[0])
-        self.assertTrue(proxy_manager.can_cycle)
-
-    def test_proxy_manager_no_reuse(self):
-        proxies = ["https://proxy1.com", "https://proxy2.com", "https://proxy3.com"]
-        proxy_manager = ProxyManager(proxies, reuse=False)
-        # First cycle
-        self.assertEqual(proxy_manager.proxy, proxies[0])
-        self.assertTrue(proxy_manager.can_cycle)
-        # Second cycle
-        proxy_manager.cycle()
-        self.assertEqual(proxy_manager.proxy, proxies[1])
-        self.assertTrue(proxy_manager.can_cycle)
-        # Third cycle
-        proxy_manager.cycle()
-        self.assertEqual(proxy_manager.proxy, proxies[2])
-        self.assertFalse(proxy_manager.can_cycle)
-        # Fourth cycle (no proxies left)
-        proxy_manager.cycle()
-        self.assertIsNone(proxy_manager.proxy)
-        self.assertFalse(proxy_manager.can_cycle)
+        ),
+    ],
+)
+def test_prepare_http_proxy_for_requests(address, expected):
+    assert prepare_http_proxy_for_requests(address) == expected
 
-    def test_proxy_manager_no_proxies(self):
-        proxy_manager = ProxyManager([], reuse=True)
-        # No proxies
-        self.assertIsNone(proxy_manager.proxy)
-        self.assertFalse(proxy_manager.can_cycle)
-        # Still no proxies
-        proxy_manager.cycle()
 
-    def test_proxy_manager_no_proxies_no_reuse(self):
-        proxy_manager = ProxyManager([], reuse=False)
-        # No proxies
-        self.assertIsNone(proxy_manager.proxy)
-        self.assertFalse(proxy_manager.can_cycle)
-        # Still no proxies
+@pytest.mark.parametrize("address", ["localhost:8080", "ftp://localhost:8080", ""])
+def test_prepare_http_proxy_for_requests_raises_ValueError_for_invalid_address(address):
+    with pytest.raises(ValueError, match=r"Invalid proxy address: .+"):
+        prepare_http_proxy_for_requests(address)
+
+
+def test_proxy_manager():
+    proxies = ["https://proxy1.com", "https://proxy2.com", "https://proxy3.com"]
+    proxy_manager = ProxyManager(proxies, reuse=True)
+    # First cycle
+    assert proxy_manager.proxy == proxies[0]
+    assert proxy_manager.can_cycle
+    # Second cycle
+    proxy_manager.cycle()
+    assert proxy_manager.proxy == proxies[1]
+    assert proxy_manager.can_cycle
+    # Third cycle
+    proxy_manager.cycle()
+    assert proxy_manager.proxy == proxies[2]
+    assert proxy_manager.can_cycle
+    # Cycle back to the first proxy
+    proxy_manager.cycle()
+    assert proxy_manager.proxy == proxies[0]
+    assert proxy_manager.can_cycle
+
+
+def test_proxy_manager_no_reuse():
+    proxies = ["https://proxy1.com", "https://proxy2.com", "https://proxy3.com"]
+    proxy_manager = ProxyManager(proxies, reuse=False)
+    # First cycle
+    assert proxy_manager.proxy == proxies[0]
+    assert proxy_manager.can_cycle
+    # Second cycle
+    proxy_manager.cycle()
+    assert proxy_manager.proxy == proxies[1]
+    assert proxy_manager.can_cycle
+    # Third cycle
+    proxy_manager.cycle()
+    assert proxy_manager.proxy == proxies[2]
+    assert not proxy_manager.can_cycle
+    # Fourth cycle (no proxies left)
+    proxy_manager.cycle()
+    assert proxy_manager.proxy is None
+    assert not proxy_manager.can_cycle
+
+
+def test_proxy_manager_no_proxies():
+    proxy_manager = ProxyManager([], reuse=True)
+    # No proxies
+    assert proxy_manager.proxy is None
+    assert not proxy_manager.can_cycle
+    # Still no proxies
+    with pytest.warns(UserWarning, match=r"Attempted to cycle a locked proxy manager"):
+        proxy_manager.cycle()
+    assert proxy_manager.proxy is None
+    assert not proxy_manager.can_cycle
+
+
+def test_proxy_manager_no_proxies_no_reuse():
+    proxy_manager = ProxyManager([], reuse=False)
+    # No proxies
+    assert proxy_manager.proxy is None
+    assert not proxy_manager.can_cycle
+    # Still no proxies
+    with pytest.warns(UserWarning, match=r"Attempted to cycle a locked proxy manager"):
         proxy_manager.cycle()
-        self.assertIsNone(proxy_manager.proxy)
-        self.assertFalse(proxy_manager.can_cycle)
+    assert proxy_manager.proxy is None
+    assert not proxy_manager.can_cycle
```


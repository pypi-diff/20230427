# Comparing `tmp/gooddata-pandas-1.2.1a3.tar.gz` & `tmp/gooddata-pandas-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-pandas-1.2.1a3.tar", last modified: Mon Feb  6 14:22:49 2023, max compression
+gzip compressed data, was "gooddata-pandas-1.3.0.tar", last modified: Fri Mar 10 09:53:32 2023, max compression
```

## Comparing `gooddata-pandas-1.2.1a3.tar` & `gooddata-pandas-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:49.395167 gooddata-pandas-1.2.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)    78103 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-02-06 14:22:49.395167 gooddata-pandas-1.2.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:49.395167 gooddata-pandas-1.2.1a3/gooddata_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/gooddata_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/gooddata_pandas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/gooddata_pandas/data_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/gooddata_pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/gooddata_pandas/good_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/gooddata_pandas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/gooddata_pandas/result_convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/gooddata_pandas/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-02-06 14:22:35.000000 gooddata-pandas-1.2.1a3/gooddata_pandas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:49.395167 gooddata-pandas-1.2.1a3/gooddata_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-02-06 14:22:49.000000 gooddata-pandas-1.2.1a3/gooddata_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-02-06 14:22:49.000000 gooddata-pandas-1.2.1a3/gooddata_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 14:22:49.000000 gooddata-pandas-1.2.1a3/gooddata_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-06 14:22:49.000000 gooddata-pandas-1.2.1a3/gooddata_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-06 14:22:49.000000 gooddata-pandas-1.2.1a3/gooddata_pandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 14:22:49.395167 gooddata-pandas-1.2.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-02-06 14:22:41.000000 gooddata-pandas-1.2.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:32.650490 gooddata-pandas-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    78103 2023-03-10 09:53:22.000000 gooddata-pandas-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-03-10 09:53:32.650490 gooddata-pandas-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:32.650490 gooddata-pandas-1.3.0/gooddata_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/gooddata_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/gooddata_pandas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/gooddata_pandas/data_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/gooddata_pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/gooddata_pandas/good_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/gooddata_pandas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/gooddata_pandas/result_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/gooddata_pandas/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/gooddata_pandas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:32.650490 gooddata-pandas-1.3.0/gooddata_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-03-10 09:53:32.000000 gooddata-pandas-1.3.0/gooddata_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-10 09:53:32.000000 gooddata-pandas-1.3.0/gooddata_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 09:53:32.000000 gooddata-pandas-1.3.0/gooddata_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-10 09:53:32.000000 gooddata-pandas-1.3.0/gooddata_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-10 09:53:32.000000 gooddata-pandas-1.3.0/gooddata_pandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 09:53:32.654490 gooddata-pandas-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-10 09:53:23.000000 gooddata-pandas-1.3.0/setup.py
```

### Comparing `gooddata-pandas-1.2.1a3/LICENSE.txt` & `gooddata-pandas-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.2.1a3/PKG-INFO` & `gooddata-pandas-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-pandas
-Version: 1.2.1a3
+Version: 1.3.0
 Summary: GoodData.CN to pandas
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.2.1a3
+Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.3.0
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,pandas,series,data,frame,data_frame,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gooddata-pandas-1.2.1a3/README.md` & `gooddata-pandas-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.2.1a3/gooddata_pandas/data_access.py` & `gooddata-pandas-1.3.0/gooddata_pandas/data_access.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.2.1a3/gooddata_pandas/dataframe.py` & `gooddata-pandas-1.3.0/gooddata_pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.2.1a3/gooddata_pandas/good_pandas.py` & `gooddata-pandas-1.3.0/gooddata_pandas/good_pandas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # (C) 2021 GoodData Corporation
 from __future__ import annotations
 
+from pathlib import Path
 from typing import Optional
 
 from gooddata_pandas import __version__
 from gooddata_pandas.dataframe import DataFrameFactory
 from gooddata_pandas.series import SeriesFactory
 from gooddata_sdk import GoodDataSdk
+from gooddata_sdk.utils import PROFILES_FILE_PATH, good_pandas_profile_content
 
 USER_AGENT = f"gooddata-pandas/{__version__}"
 """Extra segment of the User-Agent header that will be appended to standard gooddata-sdk user agent."""
 
 
 class GoodPandas:
     """
@@ -26,14 +28,19 @@
     ) -> None:
         if headers_host is not None:
             custom_headers_["Host"] = headers_host
         self._sdk = GoodDataSdk.create(host, token, USER_AGENT, **custom_headers_)
         self._series_per_ws: dict[str, SeriesFactory] = dict()
         self._frames_per_ws: dict[str, DataFrameFactory] = dict()
 
+    @classmethod
+    def create_from_profile(cls, profile: str = "default", profiles_path: Path = PROFILES_FILE_PATH) -> GoodPandas:
+        content, custom_headers = good_pandas_profile_content(profile, profiles_path)
+        return cls(**content, **custom_headers)
+
     @property
     def sdk(self) -> GoodDataSdk:
         return self._sdk
 
     def series(self, workspace_id: str) -> SeriesFactory:
         """
         Creates factory to use for construction of pandas.Series.
```

### Comparing `gooddata-pandas-1.2.1a3/gooddata_pandas/result_convertor.py` & `gooddata-pandas-1.3.0/gooddata_pandas/result_convertor.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.2.1a3/gooddata_pandas/series.py` & `gooddata-pandas-1.3.0/gooddata_pandas/series.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.2.1a3/gooddata_pandas/utils.py` & `gooddata-pandas-1.3.0/gooddata_pandas/utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.2.1a3/gooddata_pandas.egg-info/PKG-INFO` & `gooddata-pandas-1.3.0/gooddata_pandas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-pandas
-Version: 1.2.1a3
+Version: 1.3.0
 Summary: GoodData.CN to pandas
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.2.1a3
+Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.3.0
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,pandas,series,data,frame,data_frame,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gooddata-pandas-1.2.1a3/setup.py` & `gooddata-pandas-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-sdk~=1.2.1a3",
+    "gooddata-sdk~=1.3.0",
     "pandas>=1.0.0,<2.0.0",
     'importlib-metadata >= 1.0 ; python_version >= "3.7"',
 ]
 
 setup(
     name="gooddata-pandas",
     description="GoodData.CN to pandas",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.2.1a3",
+    version="1.3.0",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
     python_requires=">=3.7.0",
     project_urls={
-        "Documentation": "https://gooddata-pandas.readthedocs.io/en/v1.2.1a3",
+        "Documentation": "https://gooddata-pandas.readthedocs.io/en/v1.3.0",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```


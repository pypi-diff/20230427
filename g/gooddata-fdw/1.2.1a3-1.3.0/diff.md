# Comparing `tmp/gooddata-fdw-1.2.1a3.tar.gz` & `tmp/gooddata-fdw-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-fdw-1.2.1a3.tar", last modified: Mon Feb  6 14:22:58 2023, max compression
+gzip compressed data, was "gooddata-fdw-1.3.0.tar", last modified: Fri Mar 10 09:53:35 2023, max compression
```

## Comparing `gooddata-fdw-1.2.1a3.tar` & `gooddata-fdw-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:58.125520 gooddata-fdw-1.2.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-02-06 14:22:58.125520 gooddata-fdw-1.2.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:58.125520 gooddata-fdw-1.2.1a3/gooddata_fdw/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/column_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/column_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/fdw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/import_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/pg_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-02-06 14:22:38.000000 gooddata-fdw-1.2.1a3/gooddata_fdw/result_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:58.125520 gooddata-fdw-1.2.1a3/gooddata_fdw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-02-06 14:22:58.000000 gooddata-fdw-1.2.1a3/gooddata_fdw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-06 14:22:58.000000 gooddata-fdw-1.2.1a3/gooddata_fdw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 14:22:58.000000 gooddata-fdw-1.2.1a3/gooddata_fdw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-06 14:22:58.000000 gooddata-fdw-1.2.1a3/gooddata_fdw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-06 14:22:58.000000 gooddata-fdw-1.2.1a3/gooddata_fdw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 14:22:58.125520 gooddata-fdw-1.2.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-02-06 14:22:48.000000 gooddata-fdw-1.2.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:35.593873 gooddata-fdw-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-10 09:53:35.593873 gooddata-fdw-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:35.589872 gooddata-fdw-1.3.0/gooddata_fdw/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/column_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/column_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/fdw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/import_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/pg_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/gooddata_fdw/result_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:35.593873 gooddata-fdw-1.3.0/gooddata_fdw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-10 09:53:35.000000 gooddata-fdw-1.3.0/gooddata_fdw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-10 09:53:35.000000 gooddata-fdw-1.3.0/gooddata_fdw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 09:53:35.000000 gooddata-fdw-1.3.0/gooddata_fdw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-10 09:53:35.000000 gooddata-fdw-1.3.0/gooddata_fdw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-10 09:53:35.000000 gooddata-fdw-1.3.0/gooddata_fdw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 09:53:35.593873 gooddata-fdw-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-10 09:53:23.000000 gooddata-fdw-1.3.0/setup.py
```

### Comparing `gooddata-fdw-1.2.1a3/LICENSE.txt` & `gooddata-fdw-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/PKG-INFO` & `gooddata-fdw-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-fdw
-Version: 1.2.1a3
+Version: 1.3.0
 Summary: GoodData.CN Foreign Data Wrapper For PostgreSQL
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.2.1a3
+Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.3.0
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,fdw,postgresql,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gooddata-fdw-1.2.1a3/README.md` & `gooddata-fdw-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/column_utils.py` & `gooddata-fdw-1.3.0/gooddata_fdw/column_utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/column_validation.py` & `gooddata-fdw-1.3.0/gooddata_fdw/column_validation.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/environment.py` & `gooddata-fdw-1.3.0/gooddata_fdw/environment.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/executor.py` & `gooddata-fdw-1.3.0/gooddata_fdw/executor.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/fdw.py` & `gooddata-fdw-1.3.0/gooddata_fdw/fdw.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/filter.py` & `gooddata-fdw-1.3.0/gooddata_fdw/filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/import_workspace.py` & `gooddata-fdw-1.3.0/gooddata_fdw/import_workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/naming.py` & `gooddata-fdw-1.3.0/gooddata_fdw/naming.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/options.py` & `gooddata-fdw-1.3.0/gooddata_fdw/options.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/pg_logging.py` & `gooddata-fdw-1.3.0/gooddata_fdw/pg_logging.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw/result_reader.py` & `gooddata-fdw-1.3.0/gooddata_fdw/result_reader.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw.egg-info/PKG-INFO` & `gooddata-fdw-1.3.0/gooddata_fdw.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-fdw
-Version: 1.2.1a3
+Version: 1.3.0
 Summary: GoodData.CN Foreign Data Wrapper For PostgreSQL
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.2.1a3
+Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.3.0
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,fdw,postgresql,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gooddata-fdw-1.2.1a3/gooddata_fdw.egg-info/SOURCES.txt` & `gooddata-fdw-1.3.0/gooddata_fdw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.2.1a3/setup.py` & `gooddata-fdw-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-sdk~=1.2.1a3",
+    "gooddata-sdk~=1.3.0",
     'importlib-metadata >= 1.0 ; python_version >= "3.7"',
     #    "multicorn>=1.4.0",
 ]
 
 
 setup(
     name="gooddata-fdw",
     description="GoodData.CN Foreign Data Wrapper For PostgreSQL",
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
-        "Documentation": "https://gooddata-fdw.readthedocs.io/en/v1.2.1a3",
+        "Documentation": "https://gooddata-fdw.readthedocs.io/en/v1.3.0",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```


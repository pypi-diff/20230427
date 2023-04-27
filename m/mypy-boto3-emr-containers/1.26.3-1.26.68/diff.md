# Comparing `tmp/mypy-boto3-emr-containers-1.26.3.tar.gz` & `tmp/mypy-boto3-emr-containers-1.26.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-containers-1.26.3.tar", last modified: Fri Nov  4 20:33:48 2022, max compression
+gzip compressed data, was "mypy-boto3-emr-containers-1.26.68.tar", last modified: Thu Feb  9 20:26:50 2023, max compression
```

## Comparing `mypy-boto3-emr-containers-1.26.3.tar` & `mypy-boto3-emr-containers-1.26.68.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:33:48.937348 mypy-boto3-emr-containers-1.26.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-04 20:33:37.000000 mypy-boto3-emr-containers-1.26.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16085 2022-11-04 20:33:48.937348 mypy-boto3-emr-containers-1.26.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14623 2022-11-04 20:33:37.000000 mypy-boto3-emr-containers-1.26.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:33:48.937348 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-11-04 20:33:37.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-11-04 20:33:37.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-11-04 20:33:37.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17340 2022-11-04 20:33:38.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    17310 2022-11-04 20:33:37.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8529 2022-11-04 20:33:38.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8527 2022-11-04 20:33:38.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6300 2022-11-04 20:33:38.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6293 2022-11-04 20:33:38.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 20:33:37.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    23737 2022-11-04 20:33:38.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    23708 2022-11-04 20:33:38.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-04 20:33:37.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:33:48.937348 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16085 2022-11-04 20:33:48.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-04 20:33:48.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 20:33:48.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 20:33:48.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-04 20:33:48.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-04 20:33:48.000000 mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 20:33:48.937348 mypy-boto3-emr-containers-1.26.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-11-04 20:33:37.000000 mypy-boto3-emr-containers-1.26.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.994837 mypy-boto3-emr-containers-1.26.68/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-02-09 20:26:49.994837 mypy-boto3-emr-containers-1.26.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.990837 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-02-09 20:26:12.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-02-09 20:26:12.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-02-09 20:26:12.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.994837 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:49.994837 mypy-boto3-emr-containers-1.26.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/setup.py
```

### Comparing `mypy-boto3-emr-containers-1.26.3/LICENSE` & `mypy-boto3-emr-containers-1.26.68/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.26.3/PKG-INFO` & `mypy-boto3-emr-containers-1.26.68/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.26.3
-Summary: Type annotations for boto3.EMRContainers 1.26.3 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.68
+Summary: Type annotations for boto3.EMRContainers 1.26.68 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-containers?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.26.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,14 +357,16 @@
     DeleteVirtualClusterRequestRequestTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverTypeDef,
+    RetryPolicyConfigurationTypeDef,
+    RetryPolicyExecutionTypeDef,
     TemplateParameterConfigurationTypeDef,
     PaginatorConfigTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
```

### Comparing `mypy-boto3-emr-containers-1.26.3/README.md` & `mypy-boto3-emr-containers-1.26.68/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-containers?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.26.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,14 +325,16 @@
     DeleteVirtualClusterRequestRequestTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverTypeDef,
+    RetryPolicyConfigurationTypeDef,
+    RetryPolicyExecutionTypeDef,
     TemplateParameterConfigurationTypeDef,
     PaginatorConfigTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
```

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/__init__.py` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/__init__.pyi` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/__main__.py` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRContainers 1.26.3\nVersion:         1.26.3\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.EMRContainers 1.26.68\nVersion:         1.26.68\nBuilder"
+        " version: 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.3")
+    print("1.26.68")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/client.py` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     JobDriverTypeDef,
     JobTemplateDataTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
+    RetryPolicyConfigurationTypeDef,
     StartJobRunResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -325,15 +326,16 @@
         name: str = ...,
         executionRoleArn: str = ...,
         releaseLabel: str = ...,
         jobDriver: JobDriverTypeDef = ...,
         configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         jobTemplateId: str = ...,
-        jobTemplateParameters: Mapping[str, str] = ...
+        jobTemplateParameters: Mapping[str, str] = ...,
+        retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.start_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#start_job_run)
         """
```

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/client.pyi` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     JobDriverTypeDef,
     JobTemplateDataTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
+    RetryPolicyConfigurationTypeDef,
     StartJobRunResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -301,15 +302,16 @@
         name: str = ...,
         executionRoleArn: str = ...,
         releaseLabel: str = ...,
         jobDriver: JobDriverTypeDef = ...,
         configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         jobTemplateId: str = ...,
-        jobTemplateParameters: Mapping[str, str] = ...
+        jobTemplateParameters: Mapping[str, str] = ...,
+        retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.start_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#start_job_run)
         """
```

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/literals.py` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -94,27 +95,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -143,14 +148,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -198,14 +204,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -216,30 +223,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -271,28 +281,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -301,14 +315,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -319,38 +334,44 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/literals.pyi` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -92,27 +93,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -141,14 +146,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -196,14 +202,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -214,30 +221,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -269,28 +279,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -299,14 +313,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -317,38 +332,44 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/paginator.py` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/paginator.pyi` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/type_defs.py` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CertificateTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
     "ConfigurationTypeDef",
     "EksInfoTypeDef",
@@ -46,14 +45,16 @@
     "DeleteVirtualClusterRequestRequestTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
     "SparkSqlJobDriverTypeDef",
     "SparkSubmitJobDriverTypeDef",
+    "RetryPolicyConfigurationTypeDef",
+    "RetryPolicyExecutionTypeDef",
     "TemplateParameterConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
@@ -139,22 +140,20 @@
     "_OptionalCloudWatchMonitoringConfigurationTypeDef",
     {
         "logStreamNamePrefix": str,
     },
     total=False,
 )
 
-
 class CloudWatchMonitoringConfigurationTypeDef(
     _RequiredCloudWatchMonitoringConfigurationTypeDef,
     _OptionalCloudWatchMonitoringConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
@@ -162,19 +161,17 @@
     {
         "properties": Mapping[str, str],
         "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
-
 EksInfoTypeDef = TypedDict(
     "EksInfoTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
@@ -251,20 +248,32 @@
     {
         "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
-
 class SparkSubmitJobDriverTypeDef(
     _RequiredSparkSubmitJobDriverTypeDef, _OptionalSparkSubmitJobDriverTypeDef
 ):
     pass
 
+RetryPolicyConfigurationTypeDef = TypedDict(
+    "RetryPolicyConfigurationTypeDef",
+    {
+        "maxAttempts": int,
+    },
+)
+
+RetryPolicyExecutionTypeDef = TypedDict(
+    "RetryPolicyExecutionTypeDef",
+    {
+        "currentAttemptCount": int,
+    },
+)
 
 TemplateParameterConfigurationTypeDef = TypedDict(
     "TemplateParameterConfigurationTypeDef",
     {
         "type": TemplateParameterDataTypeType,
         "defaultValue": str,
     },
@@ -296,21 +305,19 @@
         "states": Sequence[JobRunStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "maxResults": int,
         "nextToken": str,
@@ -333,22 +340,20 @@
         "states": Sequence[EndpointStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListManagedEndpointsRequestRequestTypeDef(
     _RequiredListManagedEndpointsRequestRequestTypeDef,
     _OptionalListManagedEndpointsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -522,22 +527,20 @@
         "name": str,
         "states": Sequence[JobRunStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
-
 ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     {
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -558,22 +561,20 @@
         "types": Sequence[str],
         "states": Sequence[EndpointStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
     _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
 ):
     pass
 
-
 ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
         "containerProviderId": str,
         "containerProviderType": Literal["EKS"],
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
@@ -614,21 +615,19 @@
     "_OptionalContainerProviderTypeDef",
     {
         "info": ContainerInfoTypeDef,
     },
     total=False,
 )
 
-
 class ContainerProviderTypeDef(
     _RequiredContainerProviderTypeDef, _OptionalContainerProviderTypeDef
 ):
     pass
 
-
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
@@ -655,22 +654,20 @@
     "_OptionalCreateVirtualClusterRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateVirtualClusterRequestRequestTypeDef(
     _RequiredCreateVirtualClusterRequestRequestTypeDef,
     _OptionalCreateVirtualClusterRequestRequestTypeDef,
 ):
     pass
 
-
 VirtualClusterTypeDef = TypedDict(
     "VirtualClusterTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "state": VirtualClusterStateType,
@@ -698,22 +695,20 @@
         "certificateArn": str,
         "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateManagedEndpointRequestRequestTypeDef(
     _RequiredCreateManagedEndpointRequestRequestTypeDef,
     _OptionalCreateManagedEndpointRequestRequestTypeDef,
 ):
     pass
 
-
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
@@ -750,14 +745,16 @@
         "jobDriver": JobDriverTypeDef,
         "createdAt": datetime,
         "createdBy": str,
         "finishedAt": datetime,
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
+        "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
+        "retryPolicyExecution": RetryPolicyExecutionTypeDef,
     },
     total=False,
 )
 
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
@@ -772,25 +769,24 @@
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverTypeDef,
         "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Mapping[str, str],
         "jobTemplateId": str,
         "jobTemplateParameters": Mapping[str, str],
+        "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredJobTemplateDataTypeDef = TypedDict(
     "_RequiredJobTemplateDataTypeDef",
     {
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverTypeDef,
     },
@@ -801,19 +797,17 @@
         "configurationOverrides": ParametricConfigurationOverridesTypeDef,
         "parameterConfiguration": Mapping[str, TemplateParameterConfigurationTypeDef],
         "jobTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class JobTemplateDataTypeDef(_RequiredJobTemplateDataTypeDef, _OptionalJobTemplateDataTypeDef):
     pass
 
-
 DescribeVirtualClusterResponseTypeDef = TypedDict(
     "DescribeVirtualClusterResponseTypeDef",
     {
         "virtualCluster": VirtualClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -874,21 +868,19 @@
     {
         "tags": Mapping[str, str],
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredJobTemplateTypeDef = TypedDict(
     "_RequiredJobTemplateTypeDef",
     {
         "jobTemplateData": JobTemplateDataTypeDef,
     },
 )
 _OptionalJobTemplateTypeDef = TypedDict(
@@ -902,19 +894,17 @@
         "tags": Dict[str, str],
         "kmsKeyArn": str,
         "decryptionError": str,
     },
     total=False,
 )
 
-
 class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
     pass
 
-
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers/type_defs.pyi` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CertificateTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
     "ConfigurationTypeDef",
     "EksInfoTypeDef",
@@ -45,14 +46,16 @@
     "DeleteVirtualClusterRequestRequestTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
     "SparkSqlJobDriverTypeDef",
     "SparkSubmitJobDriverTypeDef",
+    "RetryPolicyConfigurationTypeDef",
+    "RetryPolicyExecutionTypeDef",
     "TemplateParameterConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
@@ -138,20 +141,22 @@
     "_OptionalCloudWatchMonitoringConfigurationTypeDef",
     {
         "logStreamNamePrefix": str,
     },
     total=False,
 )
 
+
 class CloudWatchMonitoringConfigurationTypeDef(
     _RequiredCloudWatchMonitoringConfigurationTypeDef,
     _OptionalCloudWatchMonitoringConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
@@ -159,17 +164,19 @@
     {
         "properties": Mapping[str, str],
         "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
+
 EksInfoTypeDef = TypedDict(
     "EksInfoTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
@@ -246,19 +253,35 @@
     {
         "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
+
 class SparkSubmitJobDriverTypeDef(
     _RequiredSparkSubmitJobDriverTypeDef, _OptionalSparkSubmitJobDriverTypeDef
 ):
     pass
 
+
+RetryPolicyConfigurationTypeDef = TypedDict(
+    "RetryPolicyConfigurationTypeDef",
+    {
+        "maxAttempts": int,
+    },
+)
+
+RetryPolicyExecutionTypeDef = TypedDict(
+    "RetryPolicyExecutionTypeDef",
+    {
+        "currentAttemptCount": int,
+    },
+)
+
 TemplateParameterConfigurationTypeDef = TypedDict(
     "TemplateParameterConfigurationTypeDef",
     {
         "type": TemplateParameterDataTypeType,
         "defaultValue": str,
     },
     total=False,
@@ -289,19 +312,21 @@
         "states": Sequence[JobRunStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "maxResults": int,
         "nextToken": str,
@@ -324,20 +349,22 @@
         "states": Sequence[EndpointStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListManagedEndpointsRequestRequestTypeDef(
     _RequiredListManagedEndpointsRequestRequestTypeDef,
     _OptionalListManagedEndpointsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -511,20 +538,22 @@
         "name": str,
         "states": Sequence[JobRunStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
+
 ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     {
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -545,20 +574,22 @@
         "types": Sequence[str],
         "states": Sequence[EndpointStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
     _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
 ):
     pass
 
+
 ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
         "containerProviderId": str,
         "containerProviderType": Literal["EKS"],
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
@@ -599,19 +630,21 @@
     "_OptionalContainerProviderTypeDef",
     {
         "info": ContainerInfoTypeDef,
     },
     total=False,
 )
 
+
 class ContainerProviderTypeDef(
     _RequiredContainerProviderTypeDef, _OptionalContainerProviderTypeDef
 ):
     pass
 
+
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
@@ -638,20 +671,22 @@
     "_OptionalCreateVirtualClusterRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateVirtualClusterRequestRequestTypeDef(
     _RequiredCreateVirtualClusterRequestRequestTypeDef,
     _OptionalCreateVirtualClusterRequestRequestTypeDef,
 ):
     pass
 
+
 VirtualClusterTypeDef = TypedDict(
     "VirtualClusterTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "state": VirtualClusterStateType,
@@ -679,20 +714,22 @@
         "certificateArn": str,
         "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateManagedEndpointRequestRequestTypeDef(
     _RequiredCreateManagedEndpointRequestRequestTypeDef,
     _OptionalCreateManagedEndpointRequestRequestTypeDef,
 ):
     pass
 
+
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
@@ -729,14 +766,16 @@
         "jobDriver": JobDriverTypeDef,
         "createdAt": datetime,
         "createdBy": str,
         "finishedAt": datetime,
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
+        "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
+        "retryPolicyExecution": RetryPolicyExecutionTypeDef,
     },
     total=False,
 )
 
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
@@ -751,23 +790,26 @@
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverTypeDef,
         "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Mapping[str, str],
         "jobTemplateId": str,
         "jobTemplateParameters": Mapping[str, str],
+        "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredJobTemplateDataTypeDef = TypedDict(
     "_RequiredJobTemplateDataTypeDef",
     {
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverTypeDef,
     },
@@ -778,17 +820,19 @@
         "configurationOverrides": ParametricConfigurationOverridesTypeDef,
         "parameterConfiguration": Mapping[str, TemplateParameterConfigurationTypeDef],
         "jobTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class JobTemplateDataTypeDef(_RequiredJobTemplateDataTypeDef, _OptionalJobTemplateDataTypeDef):
     pass
 
+
 DescribeVirtualClusterResponseTypeDef = TypedDict(
     "DescribeVirtualClusterResponseTypeDef",
     {
         "virtualCluster": VirtualClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -849,19 +893,21 @@
     {
         "tags": Mapping[str, str],
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredJobTemplateTypeDef = TypedDict(
     "_RequiredJobTemplateTypeDef",
     {
         "jobTemplateData": JobTemplateDataTypeDef,
     },
 )
 _OptionalJobTemplateTypeDef = TypedDict(
@@ -875,17 +921,19 @@
         "tags": Dict[str, str],
         "kmsKeyArn": str,
         "decryptionError": str,
     },
     total=False,
 )
 
+
 class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
     pass
 
+
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers.egg-info/PKG-INFO` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.26.3
-Summary: Type annotations for boto3.EMRContainers 1.26.3 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.68
+Summary: Type annotations for boto3.EMRContainers 1.26.68 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-containers?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.26.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,14 +357,16 @@
     DeleteVirtualClusterRequestRequestTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverTypeDef,
+    RetryPolicyConfigurationTypeDef,
+    RetryPolicyExecutionTypeDef,
     TemplateParameterConfigurationTypeDef,
     PaginatorConfigTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
```

### Comparing `mypy-boto3-emr-containers-1.26.3/mypy_boto3_emr_containers.egg-info/SOURCES.txt` & `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.26.3/setup.py` & `mypy-boto3-emr-containers-1.26.68/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-emr-containers",
-    version="1.26.3",
+    version="1.26.68",
     packages=["mypy_boto3_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRContainers 1.26.3 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.EMRContainers 1.26.68 service generated with mypy-boto3-builder"
+        " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 emr-containers type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_emr_containers": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_emr_containers": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```


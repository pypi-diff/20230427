# Comparing `tmp/dbterd-1.1.0b2.tar.gz` & `tmp/dbterd-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbterd-1.1.0b2.tar", max compression
+gzip compressed data, was "dbterd-1.1.1.tar", max compression
```

## Comparing `dbterd-1.1.0b2.tar` & `dbterd-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1067 2023-04-22 06:27:30.683149 dbterd-1.1.0b2/LICENSE
--rw-r--r--   0        0        0     4504 2023-04-22 06:27:30.683149 dbterd-1.1.0b2/README.md
--rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/__init__.py
--rw-r--r--   0        0        0       37 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/__main__.py
--rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/algos/__init__.py
--rw-r--r--   0        0        0     4465 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/algos/base.py
--rw-r--r--   0        0        0     3157 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/algos/filter.py
--rw-r--r--   0        0        0      545 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/algos/meta.py
--rw-r--r--   0        0        0     2505 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/algos/test_relationship.py
--rw-r--r--   0        0        0     2561 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/base.py
--rw-r--r--   0        0        0      560 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/factory.py
--rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/__init__.py
--rw-r--r--   0        0        0      132 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/constants.py
--rw-r--r--   0        0        0      304 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/dbml/__init__.py
--rw-r--r--   0        0        0     1373 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/dbml/dbml_test_relationship.py
--rw-r--r--   0        0        0      168 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/default.py
--rw-r--r--   0        0        0      316 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/mermaid/__init__.py
--rw-r--r--   0        0        0     1597 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
--rw-r--r--   0        0        0      222 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/worker.py
--rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/cli/__init__.py
--rw-r--r--   0        0        0     2026 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/cli/main.py
--rw-r--r--   0        0        0     1928 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/cli/params.py
--rw-r--r--   0        0        0      284 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/default.py
--rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/__init__.py
--rw-r--r--   0        0        0      721 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/cli_messaging.py
--rw-r--r--   0        0        0      877 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/dict.py
--rw-r--r--   0        0        0     4494 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/file.py
--rw-r--r--   0        0        0     1022 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/jsonify.py
--rw-r--r--   0        0        0      976 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/log.py
--rw-r--r--   0        0        0     1605 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/yaml.py
--rw-r--r--   0        0        0       94 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/main.py
--rw-r--r--   0        0        0     2113 2023-04-22 06:27:48.171863 dbterd-1.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     5553 1970-01-01 00:00:00.000000 dbterd-1.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-27 16:08:23.050140 dbterd-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4504 2023-04-27 16:08:23.050140 dbterd-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/algos/__init__.py
+-rw-r--r--   0        0        0     4465 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/algos/base.py
+-rw-r--r--   0        0        0     3157 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/algos/filter.py
+-rw-r--r--   0        0        0      545 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/algos/meta.py
+-rw-r--r--   0        0        0     2505 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/algos/test_relationship.py
+-rw-r--r--   0        0        0     2561 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/base.py
+-rw-r--r--   0        0        0      560 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/factory.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/constants.py
+-rw-r--r--   0        0        0      304 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/dbml/__init__.py
+-rw-r--r--   0        0        0     1373 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/dbml/dbml_test_relationship.py
+-rw-r--r--   0        0        0      168 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/default.py
+-rw-r--r--   0        0        0      316 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/mermaid/__init__.py
+-rw-r--r--   0        0        0     1597 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
+-rw-r--r--   0        0        0      222 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/adapters/worker.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/cli/__init__.py
+-rw-r--r--   0        0        0     2026 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/cli/main.py
+-rw-r--r--   0        0        0     1928 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/cli/params.py
+-rw-r--r--   0        0        0      284 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/default.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/__init__.py
+-rw-r--r--   0        0        0      721 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/cli_messaging.py
+-rw-r--r--   0        0        0      877 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/dict.py
+-rw-r--r--   0        0        0     4494 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/file.py
+-rw-r--r--   0        0        0     1022 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/jsonify.py
+-rw-r--r--   0        0        0      976 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/log.py
+-rw-r--r--   0        0        0     1605 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/helpers/yaml.py
+-rw-r--r--   0        0        0       94 2023-04-27 16:08:23.058139 dbterd-1.1.1/dbterd/main.py
+-rw-r--r--   0        0        0     2111 2023-04-27 16:08:46.922338 dbterd-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5551 1970-01-01 00:00:00.000000 dbterd-1.1.1/PKG-INFO
```

### Comparing `dbterd-1.1.0b2/LICENSE` & `dbterd-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/README.md` & `dbterd-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/adapters/algos/base.py` & `dbterd-1.1.1/dbterd/adapters/algos/base.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/adapters/algos/filter.py` & `dbterd-1.1.1/dbterd/adapters/algos/filter.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/adapters/algos/meta.py` & `dbterd-1.1.1/dbterd/adapters/algos/meta.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/adapters/algos/test_relationship.py` & `dbterd-1.1.1/dbterd/adapters/algos/test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/adapters/base.py` & `dbterd-1.1.1/dbterd/adapters/base.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/adapters/factory.py` & `dbterd-1.1.1/dbterd/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/adapters/targets/dbml/dbml_test_relationship.py` & `dbterd-1.1.1/dbterd/adapters/targets/dbml/dbml_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py` & `dbterd-1.1.1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/cli/main.py` & `dbterd-1.1.1/dbterd/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/cli/params.py` & `dbterd-1.1.1/dbterd/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/helpers/cli_messaging.py` & `dbterd-1.1.1/dbterd/helpers/cli_messaging.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/helpers/dict.py` & `dbterd-1.1.1/dbterd/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/helpers/file.py` & `dbterd-1.1.1/dbterd/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/helpers/jsonify.py` & `dbterd-1.1.1/dbterd/helpers/jsonify.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/helpers/log.py` & `dbterd-1.1.1/dbterd/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/dbterd/helpers/yaml.py` & `dbterd-1.1.1/dbterd/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b2/pyproject.toml` & `dbterd-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbterd"
-version = "1.1.0b2"
+version = "1.1.1"
 description = "dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file"
 authors = ["Dat Nguyen <datnguyen.it09@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/datnguye/dbterd"
 repository = "https://github.com/datnguye/dbterd"
 keywords = ["flake8", "markdown", "lint"]
```

### Comparing `dbterd-1.1.0b2/PKG-INFO` & `dbterd-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbterd
-Version: 1.1.0b2
+Version: 1.1.1
 Summary: dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file
 Home-page: https://github.com/datnguye/dbterd
 License: MIT
 Keywords: flake8,markdown,lint
 Author: Dat Nguyen
 Author-email: datnguyen.it09@gmail.com
 Requires-Python: >=3.9,<4.0
```


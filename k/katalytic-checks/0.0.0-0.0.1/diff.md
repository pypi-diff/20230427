# Comparing `tmp/katalytic-checks-0.0.0.tar.gz` & `tmp/katalytic-checks-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-checks-0.0.0.tar", last modified: Thu Apr 27 04:49:50 2023, max compression
+gzip compressed data, was "katalytic-checks-0.0.1.tar", last modified: Thu Apr 27 05:26:09 2023, max compression
```

## Comparing `katalytic-checks-0.0.0.tar` & `katalytic-checks-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-checks-0.0.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-checks-0.0.0/.gitignore
--rw-r--r--   0        0        0     3109 2023-04-16 15:20:55.636719 katalytic-checks-0.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     6393 2023-04-26 18:40:16.445220 katalytic-checks-0.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-checks-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2105 2023-04-26 19:33:49.669431 katalytic-checks-0.0.0/README.md
--rw-r--r--   0        0        0     1525 2023-04-26 19:29:15.014711 katalytic-checks-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     5722 2023-04-25 05:47:11.165924 katalytic-checks-0.0.0/src/katalytic/checks.py
--rw-r--r--   0        0        0    16327 2023-04-24 05:49:34.858602 katalytic-checks-0.0.0/tests/test_checks.py
--rw-r--r--   0        0        0     3156 1970-01-01 00:00:00.000000 katalytic-checks-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-checks-0.0.1/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-checks-0.0.1/.gitignore
+-rw-r--r--   0        0        0     3109 2023-04-16 15:20:55.636719 katalytic-checks-0.0.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     6569 2023-04-27 05:23:14.397929 katalytic-checks-0.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-checks-0.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1990 2023-04-27 05:10:58.838831 katalytic-checks-0.0.1/README.md
+-rw-r--r--   0        0        0     1525 2023-04-27 05:23:14.397929 katalytic-checks-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5722 2023-04-25 05:47:11.165924 katalytic-checks-0.0.1/src/katalytic/checks.py
+-rw-r--r--   0        0        0    16327 2023-04-24 05:49:34.858602 katalytic-checks-0.0.1/tests/test_checks.py
+-rw-r--r--   0        0        0     3041 1970-01-01 00:00:00.000000 katalytic-checks-0.0.1/PKG-INFO
```

### Comparing `katalytic-checks-0.0.0/.gitignore` & `katalytic-checks-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.0.0/.gitlab-ci.yml` & `katalytic-checks-0.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.0.0/CHANGELOG.md` & `katalytic-checks-0.0.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.0.1 (2023-04-27)
+### fix
+- [[`1c6b9b6`](https://gitlab.com/katalytic/katalytic-checks/commit/1c6b9b6f9fca9cde0b985fd0660c8030c6aafa1d)] remove wrong info from README.md
+
+
 ## 0.3.0 (2023-04-26)
 ### feat
 - [[`39cccc6`](https://gitlab.com/katalytic/katalytic-data/commit/39cccc664bd062e73fe80d63a21dedc8cffcb2d2)] add all_types_besides, flatten, flatten_recursive
 - [[`12706e2`](https://gitlab.com/katalytic/katalytic-data/commit/12706e2e40dc3127ca680c7121dd720e849d3fdc)] add are_equal
 - [[`fbe876b`](https://gitlab.com/katalytic/katalytic-data/commit/fbe876b80301be2ae917b93ee31954d576477af8)] add as_dict_of_lists(), and fix bugs in as_sequence_of_dicts() and as_sequence_of_sequences()
 - [[`2a4ac90`](https://gitlab.com/katalytic/katalytic-data/commit/2a4ac90ff94ced5ddbafc6d083d08a3720fb389c)] add as_sequence_of_dicts()
 - [[`ed4689c`](https://gitlab.com/katalytic/katalytic-data/commit/ed4689c231abf872c6f3fa130a286105548e69b1)] add as_sequence_of_sequences()
```

### Comparing `katalytic-checks-0.0.0/LICENSE.txt` & `katalytic-checks-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.0.0/README.md` & `katalytic-checks-0.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,15 @@
 pip install katalytic
 ```
 
 ## Usage
 TODO: Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
 
 ## Roadmap
-- converting data between formats
-- dict sorting by key/value
-- mapping dict keys/values
-- recursive map
-- recursive sort
+- TODO
 
 ## Contributing
 Contributions can be made in a number of ways:
 - Propose architectural or API improvements
 - Propose new features
 - Propose packaging, building, or deployment improvements
 - Report and fix bugs
```

### Comparing `katalytic-checks-0.0.0/pyproject.toml` & `katalytic-checks-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-checks"
-version = "0.0.0"
+version = "0.0.1"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-checks-0.0.0/src/katalytic/checks.py` & `katalytic-checks-0.0.1/src/katalytic/checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.0.0/tests/test_checks.py` & `katalytic-checks-0.0.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-checks-0.0.0/PKG-INFO` & `katalytic-checks-0.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-checks
-Version: 0.0.0
+Version: 0.0.1
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -44,19 +44,15 @@
 pip install katalytic
 ```
 
 ## Usage
 TODO: Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
 
 ## Roadmap
-- converting data between formats
-- dict sorting by key/value
-- mapping dict keys/values
-- recursive map
-- recursive sort
+- TODO
 
 ## Contributing
 Contributions can be made in a number of ways:
 - Propose architectural or API improvements
 - Propose new features
 - Propose packaging, building, or deployment improvements
 - Report and fix bugs
```


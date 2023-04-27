# Comparing `tmp/katalytic-data-0.2.0.tar.gz` & `tmp/katalytic-data-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.2.0.tar", last modified: Sun Apr 16 12:22:55 2023, max compression
+gzip compressed data, was "katalytic-data-0.4.0.tar", last modified: Thu Apr 27 05:39:58 2023, max compression
```

## Comparing `katalytic-data-0.2.0.tar` & `katalytic-data-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,12 @@
--rw-r--r--   0        0        0       87 2023-04-13 15:48:09.439894 katalytic-data-0.2.0/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-05 07:07:35.618314 katalytic-data-0.2.0/.gitignore
--rw-r--r--   0        0        0      841 2023-04-05 11:25:28.742970 katalytic-data-0.2.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      542 2023-04-15 03:06:48.732796 katalytic-data-0.2.0/.travis.yml
--rw-r--r--   0        0        0      884 2023-04-16 12:22:50.960034 katalytic-data-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-10 04:00:05.979612 katalytic-data-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2083 2023-04-15 15:52:39.144384 katalytic-data-0.2.0/README.md
--rw-r--r--   0        0        0     1516 2023-04-16 12:22:50.560034 katalytic-data-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-13 11:10:42.206595 katalytic-data-0.2.0/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-13 05:19:55.379205 katalytic-data-0.2.0/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-10 04:05:02.825570 katalytic-data-0.2.0/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-10 04:00:05.995612 katalytic-data-0.2.0/scripts/pytest.sh
--rw-r--r--   0        0        0     3267 2023-04-16 12:22:39.396035 katalytic-data-0.2.0/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-14 17:30:33.363765 katalytic-data-0.2.0/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-13 16:48:26.840531 katalytic-data-0.2.0/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-13 16:48:17.692461 katalytic-data-0.2.0/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-13 05:20:07.215328 katalytic-data-0.2.0/scripts/venv.sh
--rw-r--r--   0        0        0      381 2023-04-16 05:11:03.853269 katalytic-data-0.2.0/src/katalytic/checks.py
--rw-r--r--   0        0        0     2455 2023-04-16 05:01:47.932490 katalytic-data-0.2.0/src/katalytic/data.py
--rw-r--r--   0        0        0      772 2023-04-16 05:10:05.493474 katalytic-data-0.2.0/tests/test_checks.py
--rw-r--r--   0        0        0     5465 2023-04-16 05:05:41.482731 katalytic-data-0.2.0/tests/test_data.py
--rw-r--r--   0        0        0     3128 1970-01-01 00:00:00.000000 katalytic-data-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.4.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.4.0/.gitignore
+-rw-r--r--   0        0        0     3109 2023-04-16 15:20:55.636719 katalytic-data-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0    11927 2023-04-27 05:39:51.262487 katalytic-data-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.4.0/README.md
+-rw-r--r--   0        0        0     1548 2023-04-27 05:39:51.262487 katalytic-data-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5722 2023-04-25 05:47:11.165924 katalytic-data-0.4.0/src/katalytic/checks.py
+-rw-r--r--   0        0        0    20361 2023-04-25 05:38:24.309384 katalytic-data-0.4.0/src/katalytic/data.py
+-rw-r--r--   0        0        0    16327 2023-04-24 05:49:34.858602 katalytic-data-0.4.0/tests/test_checks.py
+-rw-r--r--   0        0        0    39853 2023-04-25 05:42:40.065433 katalytic-data-0.4.0/tests/test_data.py
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.4.0/PKG-INFO
```

### Comparing `katalytic-data-0.2.0/.gitignore` & `katalytic-data-0.4.0/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 dist/*
 sdist/*
 docs/api/*
 docs/_rst/*
 docs/_build/*
 cover/*
 MANIFEST
+scripts/*
 
 # Per-project virtualenvs
 venv
 .venv*/
 .conda*/
 .python-version
```

### Comparing `katalytic-data-0.2.0/LICENSE.txt` & `katalytic-data-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.2.0/README.md` & `katalytic-data-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.2.0/pyproject.toml` & `katalytic-data-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.2.0"
+version = "0.4.0"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -25,14 +25,15 @@
 	"data conversion",
 ]
 authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
 
 requires-python = ">=3.6"
 dependencies = [
     "katalytic-pkg>=0.2.0",
+    "katalytic-checks>=0.0.1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
     "pytest-randomly",
@@ -60,7 +61,8 @@
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version"
 branch = "main"
 
 [tool.flit.module]
 name = "katalytic.data"
+
```

### Comparing `katalytic-data-0.2.0/PKG-INFO` & `katalytic-data-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.2.0
+Version: 0.4.0
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Dist: katalytic-pkg>=0.2.0
+Requires-Dist: katalytic-checks>=0.0.1
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-data.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-data.git
 Provides-Extra: dev
```


# Comparing `tmp/ansys-platform-instancemanagement-1.1.0.tar.gz` & `tmp/ansys-platform-instancemanagement-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-platform-instancemanagement-1.1.0.tar", last modified: Thu Apr 20 10:10:32 2023, max compression
+gzip compressed data, was "ansys-platform-instancemanagement-1.1.1.tar", last modified: Thu Apr 27 15:17:42 2023, max compression
```

## Comparing `ansys-platform-instancemanagement-1.1.0.tar` & `ansys-platform-instancemanagement-1.1.1.tar`

### file list

```diff
@@ -1,42 +1,40 @@
--rw-r--r--   0        0        0      233 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/.flake8
--rw-r--r--   0        0        0      516 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2783 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     3019 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/.gitignore
--rw-r--r--   0        0        0      579 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1089 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/LICENSE
--rw-r--r--   0        0        0     5201 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/README.rst
--rwxr-xr-x   0        0        0      753 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/Makefile
--rw-r--r--   0        0        0      970 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/make.bat
--rw-r--r--   0        0        0       22 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/CNAME
--rw-r--r--   0        0        0       64 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/_templates/README.md
--rw-r--r--   0        0        0      451 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0       12 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/api/.gitignore
--rw-r--r--   0        0        0      592 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/api/index.rst
--rwxr-xr-x   0        0        0     2806 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/conf.py
--rw-r--r--   0        0        0     1911 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/contributing.rst
--rw-r--r--   0        0        0      254 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/index.rst
--rw-r--r--   0        0        0     8374 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/integration.rst
--rw-r--r--   0        0        0      201 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/protos/README.rst
--rw-r--r--   0        0        0     8485 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/protos/ansys/api/platform/instancemanagement/v1/product_instance_manager.proto
--rw-r--r--   0        0        0     1285 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       24 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/requirements/requirements_build.txt
--rw-r--r--   0        0        0      120 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/requirements/requirements_doc.txt
--rw-r--r--   0        0        0      126 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/requirements/requirements_tests.txt
--rw-r--r--   0        0        0     3090 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/__init__.py
--rw-r--r--   0        0        0     9848 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/client.py
--rw-r--r--   0        0        0     6248 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/configuration.py
--rw-r--r--   0        0        0     4497 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/definition.py
--rw-r--r--   0        0        0     3574 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/exceptions.py
--rw-r--r--   0        0        0    10514 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/instance.py
--rw-r--r--   0        0        0     3157 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/interceptor.py
--rw-r--r--   0        0        0     3363 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/service.py
--rw-r--r--   0        0        0     1021 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0    18868 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_client.py
--rw-r--r--   0        0        0     2349 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_configuration.py
--rw-r--r--   0        0        0     2804 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_definition.py
--rw-r--r--   0        0        0    15486 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_instance.py
--rw-r--r--   0        0        0      118 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_metadata.py
--rw-r--r--   0        0        0     2424 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_service.py
--rw-r--r--   0        0        0     1371 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tox.ini
--rw-r--r--   0        0        0     5874 1970-01-01 00:00:00.000000 ansys-platform-instancemanagement-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      233 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/.flake8
+-rw-r--r--   0        0        0      516 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2641 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     3019 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/.gitignore
+-rw-r--r--   0        0        0      579 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1089 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5201 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/README.rst
+-rwxr-xr-x   0        0        0      753 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/doc/Makefile
+-rw-r--r--   0        0        0      970 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/doc/make.bat
+-rw-r--r--   0        0        0       22 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/doc/source/CNAME
+-rw-r--r--   0        0        0       64 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/doc/source/_static/README.md
+-rw-r--r--   0        0        0       12 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/doc/source/api/.gitignore
+-rw-r--r--   0        0        0      592 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/doc/source/api/index.rst
+-rwxr-xr-x   0        0        0     2700 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/doc/source/conf.py
+-rw-r--r--   0        0        0     1911 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/doc/source/contributing.rst
+-rw-r--r--   0        0        0      254 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/doc/source/index.rst
+-rw-r--r--   0        0        0     8374 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/doc/source/integration.rst
+-rw-r--r--   0        0        0      201 2023-04-27 15:17:19.240451 ansys-platform-instancemanagement-1.1.1/protos/README.rst
+-rw-r--r--   0        0        0     8485 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/protos/ansys/api/platform/instancemanagement/v1/product_instance_manager.proto
+-rw-r--r--   0        0        0     1285 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/requirements/requirements_build.txt
+-rw-r--r--   0        0        0      120 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/requirements/requirements_doc.txt
+-rw-r--r--   0        0        0      126 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/requirements/requirements_tests.txt
+-rw-r--r--   0        0        0     3090 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/__init__.py
+-rw-r--r--   0        0        0     9848 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/client.py
+-rw-r--r--   0        0        0     6248 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/configuration.py
+-rw-r--r--   0        0        0     4497 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/definition.py
+-rw-r--r--   0        0        0     3574 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/exceptions.py
+-rw-r--r--   0        0        0    10514 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/instance.py
+-rw-r--r--   0        0        0     3157 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/interceptor.py
+-rw-r--r--   0        0        0     3363 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/service.py
+-rw-r--r--   0        0        0     1021 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0    18868 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/tests/test_client.py
+-rw-r--r--   0        0        0     2349 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/tests/test_configuration.py
+-rw-r--r--   0        0        0     2804 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/tests/test_definition.py
+-rw-r--r--   0        0        0    15486 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/tests/test_instance.py
+-rw-r--r--   0        0        0      118 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/tests/test_metadata.py
+-rw-r--r--   0        0        0     2424 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/tests/test_service.py
+-rw-r--r--   0        0        0     1371 2023-04-27 15:17:19.244451 ansys-platform-instancemanagement-1.1.1/tox.ini
+-rw-r--r--   0        0        0     5874 1970-01-01 00:00:00.000000 ansys-platform-instancemanagement-1.1.1/PKG-INFO
```

### Comparing `ansys-platform-instancemanagement-1.1.0/.github/dependabot.yml` & `ansys-platform-instancemanagement-1.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/.github/workflows/ci_cd.yml` & `ansys-platform-instancemanagement-1.1.1/.github/workflows/ci_cd.yml`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,18 @@
 
 jobs:
 
   style:
     name: Code style
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - name: Set up Python
-        uses: actions/setup-python@v4
+      - name: "Run PyAnsys code style checks"
+        uses: pyansys/actions/code-style@v4
         with:
-          python-version: 3.7
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip flit tox
-      - name: Test with tox
-        run: tox -e style
+          python-version: ${{ env.MAIN_PYTHON_VERSION }}
 
 
   tests:
     name: Tests and coverage
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
```

### Comparing `ansys-platform-instancemanagement-1.1.0/.gitignore` & `ansys-platform-instancemanagement-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/.pre-commit-config.yaml` & `ansys-platform-instancemanagement-1.1.1/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 repos:
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 23.3.0
   hooks:
   - id: black
     args: [
       src, tests
     ]
 
 - repo: https://github.com/pycqa/isort
@@ -16,18 +16,18 @@
 - repo: https://github.com/PyCQA/flake8
   rev: 4.0.1
   hooks:
   - id: flake8
     args: [src, tests, doc]
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.1.0
+  rev: v2.2.4
   hooks:
   - id: codespell
 
 - repo: https://github.com/pycqa/pydocstyle
-  rev: 6.1.1
+  rev: 6.3.0
   hooks:
   - id: pydocstyle
     additional_dependencies: [toml]
     args: ["--match-dir='^(src)'"]
     exclude: "^(tests/)"
```

### Comparing `ansys-platform-instancemanagement-1.1.0/LICENSE` & `ansys-platform-instancemanagement-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/README.rst` & `ansys-platform-instancemanagement-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/doc/Makefile` & `ansys-platform-instancemanagement-1.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/doc/make.bat` & `ansys-platform-instancemanagement-1.1.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/doc/source/api/index.rst` & `ansys-platform-instancemanagement-1.1.1/doc/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/doc/source/conf.py` & `ansys-platform-instancemanagement-1.1.1/doc/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,12 @@
 
 # static path
 html_static_path = ["_static"]
 
 # Include the cname in the generated documentation.
 html_extra_path = ["CNAME"]
 
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
-
 # The suffix(es) of source filenames.
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
```

### Comparing `ansys-platform-instancemanagement-1.1.0/doc/source/contributing.rst` & `ansys-platform-instancemanagement-1.1.1/doc/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/doc/source/integration.rst` & `ansys-platform-instancemanagement-1.1.1/doc/source/integration.rst`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/protos/ansys/api/platform/instancemanagement/v1/product_instance_manager.proto` & `ansys-platform-instancemanagement-1.1.1/protos/ansys/api/platform/instancemanagement/v1/product_instance_manager.proto`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/pyproject.toml` & `ansys-platform-instancemanagement-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-platform-instancemanagement"
-version = "1.1.0"
+version = "1.1.1"
 description = "A Python wrapper for Ansys platform instancemanagement"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.support@ansys.com"},
 ]
```

### Comparing `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/__init__.py` & `ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/client.py` & `ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/client.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/configuration.py` & `ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     @property
     def tls(self) -> bool:
         """Whether the connection to PIM requires encryption.
 
         If ``True``, the ``access_token`` property is used to create a secure connection.
 
-        If ``False``, an unsecure connection is used.
+        If ``False``, an insecure connection is used.
         """
         return self._tls
 
     @property
     def uri(self) -> str:
         """Uri of the PIM service."""
         return self._uri
```

### Comparing `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/definition.py` & `ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/definition.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/exceptions.py` & `ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/instance.py` & `ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/instance.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/interceptor.py` & `ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/interceptor.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/service.py` & `ansys-platform-instancemanagement-1.1.1/src/ansys/platform/instancemanagement/service.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/tests/conftest.py` & `ansys-platform-instancemanagement-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/tests/test_client.py` & `ansys-platform-instancemanagement-1.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/tests/test_configuration.py` & `ansys-platform-instancemanagement-1.1.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/tests/test_definition.py` & `ansys-platform-instancemanagement-1.1.1/tests/test_definition.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/tests/test_instance.py` & `ansys-platform-instancemanagement-1.1.1/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/tests/test_service.py` & `ansys-platform-instancemanagement-1.1.1/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/tox.ini` & `ansys-platform-instancemanagement-1.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.1.0/PKG-INFO` & `ansys-platform-instancemanagement-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-platform-instancemanagement
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python wrapper for Ansys platform instancemanagement
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```


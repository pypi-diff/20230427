# Comparing `tmp/circuitpython-qmc5883l-0.1.2.tar.gz` & `tmp/circuitpython-qmc5883l-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-qmc5883l-0.1.2.tar", last modified: Thu Apr 20 22:34:40 2023, max compression
+gzip compressed data, was "circuitpython-qmc5883l-0.1.3.tar", last modified: Thu Apr 27 15:08:22 2023, max compression
```

## Comparing `circuitpython-qmc5883l-0.1.2.tar` & `circuitpython-qmc5883l-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:34:40.861184 circuitpython-qmc5883l-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:34:40.857184 circuitpython-qmc5883l-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:34:40.857184 circuitpython-qmc5883l-0.1.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:34:40.857184 circuitpython-qmc5883l-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:34:40.861184 circuitpython-qmc5883l-0.1.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-20 22:34:40.861184 circuitpython-qmc5883l-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:34:40.861184 circuitpython-qmc5883l-0.1.2/circuitpython_qmc5883l.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-20 22:34:40.000000 circuitpython-qmc5883l-0.1.2/circuitpython_qmc5883l.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-20 22:34:40.000000 circuitpython-qmc5883l-0.1.2/circuitpython_qmc5883l.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:34:40.000000 circuitpython-qmc5883l-0.1.2/circuitpython_qmc5883l.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 22:34:40.000000 circuitpython-qmc5883l-0.1.2/circuitpython_qmc5883l.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 22:34:40.000000 circuitpython-qmc5883l-0.1.2/circuitpython_qmc5883l.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:34:40.861184 circuitpython-qmc5883l-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:34:40.861184 circuitpython-qmc5883l-0.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:34:40.861184 circuitpython-qmc5883l-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-20 22:34:33.000000 circuitpython-qmc5883l-0.1.2/examples/qmc5883l_advanced_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-20 22:34:33.000000 circuitpython-qmc5883l-0.1.2/examples/qmc5883l_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-20 22:34:33.000000 circuitpython-qmc5883l-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-04-20 22:34:33.000000 circuitpython-qmc5883l-0.1.2/qmc5883l.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 22:34:22.000000 circuitpython-qmc5883l-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:34:40.861184 circuitpython-qmc5883l-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:08:22.017873 circuitpython-qmc5883l-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:08:22.009873 circuitpython-qmc5883l-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:08:22.017873 circuitpython-qmc5883l-0.1.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:08:22.017873 circuitpython-qmc5883l-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:08:22.017873 circuitpython-qmc5883l-0.1.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-27 15:08:22.017873 circuitpython-qmc5883l-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:08:22.017873 circuitpython-qmc5883l-0.1.3/circuitpython_qmc5883l.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-27 15:08:21.000000 circuitpython-qmc5883l-0.1.3/circuitpython_qmc5883l.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-27 15:08:22.000000 circuitpython-qmc5883l-0.1.3/circuitpython_qmc5883l.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:08:21.000000 circuitpython-qmc5883l-0.1.3/circuitpython_qmc5883l.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-27 15:08:21.000000 circuitpython-qmc5883l-0.1.3/circuitpython_qmc5883l.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 15:08:21.000000 circuitpython-qmc5883l-0.1.3/circuitpython_qmc5883l.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:08:22.017873 circuitpython-qmc5883l-0.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:08:22.017873 circuitpython-qmc5883l-0.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:08:22.017873 circuitpython-qmc5883l-0.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-27 15:08:10.000000 circuitpython-qmc5883l-0.1.3/examples/qmc5883l_advanced_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-27 15:08:10.000000 circuitpython-qmc5883l-0.1.3/examples/qmc5883l_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 15:08:10.000000 circuitpython-qmc5883l-0.1.3/examples/qmc5883l_field_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-27 15:08:10.000000 circuitpython-qmc5883l-0.1.3/examples/qmc5883l_magnetic_compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-27 15:08:10.000000 circuitpython-qmc5883l-0.1.3/examples/qmc5883l_oversample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-27 15:08:10.000000 circuitpython-qmc5883l-0.1.3/examples/qmc5883l_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-27 15:08:10.000000 circuitpython-qmc5883l-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-04-27 15:08:10.000000 circuitpython-qmc5883l-0.1.3/qmc5883l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 15:07:50.000000 circuitpython-qmc5883l-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:08:22.017873 circuitpython-qmc5883l-0.1.3/setup.cfg
```

### Comparing `circuitpython-qmc5883l-0.1.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-qmc5883l-0.1.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.2/.gitignore` & `circuitpython-qmc5883l-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.2/.pre-commit-config.yaml` & `circuitpython-qmc5883l-0.1.3/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
     rev: 22.3.0
     hooks:
       - id: black
-  - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
-    hooks:
-      - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
```

### Comparing `circuitpython-qmc5883l-0.1.2/.pylintrc` & `circuitpython-qmc5883l-0.1.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.2/CODE_OF_CONDUCT.md` & `circuitpython-qmc5883l-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.2/LICENSE` & `circuitpython-qmc5883l-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.2/LICENSES/CC-BY-4.0.txt` & `circuitpython-qmc5883l-0.1.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.2/LICENSES/MIT.txt` & `circuitpython-qmc5883l-0.1.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.2/LICENSES/Unlicense.txt` & `circuitpython-qmc5883l-0.1.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.2/PKG-INFO` & `circuitpython-qmc5883l-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-qmc5883l
-Version: 0.1.2
+Version: 0.1.3
 Summary: CircuitPython driver for the qmc5883l magnetometer
 Author-email: "Jose D. Montoya" <qmc@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_qmc5883l
 Keywords: adafruit,blinka,circuitpython,micropython,qmc5883l,magnetometer,driver,sensor,qmc5883l
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -23,14 +23,22 @@
     :target: https://circuitpython-qmc5883l.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_qmc5883l/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_qmc5883l/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-qmc5883l.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-qmc5883l
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-qmc5883l?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-qmc5883l
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 CircuitPython driver for the qmc5883l magnetometer
```

### Comparing `circuitpython-qmc5883l-0.1.2/README.rst` & `circuitpython-qmc5883l-0.1.3/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,22 @@
     :target: https://circuitpython-qmc5883l.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_qmc5883l/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_qmc5883l/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-qmc5883l.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-qmc5883l
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-qmc5883l?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-qmc5883l
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 CircuitPython driver for the qmc5883l magnetometer
```

### Comparing `circuitpython-qmc5883l-0.1.2/circuitpython_qmc5883l.egg-info/PKG-INFO` & `circuitpython-qmc5883l-0.1.3/circuitpython_qmc5883l.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-qmc5883l
-Version: 0.1.2
+Version: 0.1.3
 Summary: CircuitPython driver for the qmc5883l magnetometer
 Author-email: "Jose D. Montoya" <qmc@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_qmc5883l
 Keywords: adafruit,blinka,circuitpython,micropython,qmc5883l,magnetometer,driver,sensor,qmc5883l
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -23,14 +23,22 @@
     :target: https://circuitpython-qmc5883l.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_qmc5883l/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_qmc5883l/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-qmc5883l.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-qmc5883l
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-qmc5883l?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-qmc5883l
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 CircuitPython driver for the qmc5883l magnetometer
```

### Comparing `circuitpython-qmc5883l-0.1.2/circuitpython_qmc5883l.egg-info/SOURCES.txt` & `circuitpython-qmc5883l-0.1.3/circuitpython_qmc5883l.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -27,11 +27,19 @@
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
+docs/_static/Logo.png
+docs/_static/Logo.png.license
+docs/_static/extra_css.css
+docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/qmc5883l_advanced_settings.py
+examples/qmc5883l_data_rate.py
+examples/qmc5883l_field_range.py
+examples/qmc5883l_magnetic_compass.py
+examples/qmc5883l_oversample.py
 examples/qmc5883l_simpletest.py
```

### Comparing `circuitpython-qmc5883l-0.1.2/examples/qmc5883l_advanced_settings.py` & `circuitpython-qmc5883l-0.1.3/examples/qmc5883l_advanced_settings.py`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.2/pyproject.toml` & `circuitpython-qmc5883l-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-qmc5883l"
 description = "CircuitPython driver for the qmc5883l magnetometer"
-version = "0.1.2"
+version = "0.1.3"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "qmc@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_qmc5883l"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-qmc5883l-0.1.2/qmc5883l.py` & `circuitpython-qmc5883l-0.1.3/qmc5883l.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from adafruit_register.i2c_bits import RWBits, ROBits
 
 try:
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __repo__ = "https://github.com/jposada202020/CircuitPython_qmc5883l.git"
 
 _I2C_ADDR = const(0xD)
 _REG_WHOAMI = const(0x0D)
 _REG_SET_RESET = const(0x0B)
 _REG_OPERATION_MODE = const(0x09)
 _REG_STATUS = const(0x06)
@@ -115,14 +115,19 @@
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
         self.resolution = 12000
 
         if self._device_id != 0xFF:
             raise RuntimeError("Failed to find QMC5883L")
         self._reset = 0x01
 
+        self.oversample = OVERSAMPLE_128
+        self.field_range = FIELDRANGE_2G
+        self.output_data_rate = OUTPUT_DATA_RATE_200
+        self.mode_control = MODE_CONTINUOUS
+
     @property
     def oversample(self) -> int:
         """
         Over sample Rate (OSR) registers are used to control bandwidth of an
         internal digital filter. Larger OSR value leads to smaller filter bandwidth,
         less in-band noise and higher power consumption. It could be used to reach a
         good balance between noise and power.
```


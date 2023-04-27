# Comparing `tmp/loggerml-0.1.2.tar.gz` & `tmp/loggerml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerml-0.1.2.tar", last modified: Thu Apr 27 02:59:13 2023, max compression
+gzip compressed data, was "loggerml-0.1.3.tar", last modified: Thu Apr 27 03:27:42 2023, max compression
```

## Comparing `loggerml-0.1.2.tar` & `loggerml-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:59:13.458993 loggerml-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 02:58:53.000000 loggerml-0.1.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:59:13.450993 loggerml-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:59:13.454993 loggerml-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 02:58:53.000000 loggerml-0.1.2/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 02:58:53.000000 loggerml-0.1.2/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 02:58:53.000000 loggerml-0.1.2/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 02:58:53.000000 loggerml-0.1.2/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-27 02:58:53.000000 loggerml-0.1.2/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-27 02:58:53.000000 loggerml-0.1.2/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-27 02:58:53.000000 loggerml-0.1.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 02:58:53.000000 loggerml-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-27 02:58:53.000000 loggerml-0.1.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-27 02:58:53.000000 loggerml-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-27 02:58:53.000000 loggerml-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-27 02:59:13.458993 loggerml-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-27 02:58:53.000000 loggerml-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:59:13.458993 loggerml-0.1.2/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-27 02:58:53.000000 loggerml-0.1.2/assets/advanced.gif
--rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-27 02:58:53.000000 loggerml-0.1.2/assets/base.gif
--rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-27 02:58:53.000000 loggerml-0.1.2/assets/no_n_batches.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:59:13.458993 loggerml-0.1.2/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 02:58:53.000000 loggerml-0.1.2/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 02:58:53.000000 loggerml-0.1.2/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 02:58:53.000000 loggerml-0.1.2/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 02:58:53.000000 loggerml-0.1.2/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 02:58:53.000000 loggerml-0.1.2/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:59:13.458993 loggerml-0.1.2/loggerml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-27 02:59:13.000000 loggerml-0.1.2/loggerml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 02:59:13.000000 loggerml-0.1.2/loggerml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 02:59:13.000000 loggerml-0.1.2/loggerml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 02:59:13.000000 loggerml-0.1.2/loggerml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 02:59:13.000000 loggerml-0.1.2/loggerml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:59:13.458993 loggerml-0.1.2/logml/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 02:58:53.000000 loggerml-0.1.2/logml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-27 02:58:53.000000 loggerml-0.1.2/logml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-27 02:58:53.000000 loggerml-0.1.2/logml/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-27 02:58:53.000000 loggerml-0.1.2/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-27 02:58:53.000000 loggerml-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 02:58:53.000000 loggerml-0.1.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 02:58:53.000000 loggerml-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 02:59:13.458993 loggerml-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 02:58:53.000000 loggerml-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:59:13.450993 loggerml-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:59:13.458993 loggerml-0.1.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-27 02:58:53.000000 loggerml-0.1.2/tests/integration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:59:13.458993 loggerml-0.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-27 02:58:53.000000 loggerml-0.1.2/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-27 02:58:53.000000 loggerml-0.1.2/tests/unit/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.187008 loggerml-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 03:27:24.000000 loggerml-0.1.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.179008 loggerml-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.183008 loggerml-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 03:27:24.000000 loggerml-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-27 03:27:24.000000 loggerml-0.1.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-27 03:27:24.000000 loggerml-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-27 03:27:24.000000 loggerml-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-27 03:27:42.187008 loggerml-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-04-27 03:27:24.000000 loggerml-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-27 03:27:24.000000 loggerml-0.1.3/README_pipy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.183008 loggerml-0.1.3/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-27 03:27:24.000000 loggerml-0.1.3/assets/advanced.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-27 03:27:24.000000 loggerml-0.1.3/assets/base.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-27 03:27:24.000000 loggerml-0.1.3/assets/no_n_batches.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.183008 loggerml-0.1.3/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 03:27:24.000000 loggerml-0.1.3/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 03:27:24.000000 loggerml-0.1.3/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 03:27:24.000000 loggerml-0.1.3/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 03:27:24.000000 loggerml-0.1.3/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 03:27:24.000000 loggerml-0.1.3/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.187008 loggerml-0.1.3/loggerml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-27 03:27:42.000000 loggerml-0.1.3/loggerml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 03:27:42.000000 loggerml-0.1.3/loggerml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:27:42.000000 loggerml-0.1.3/loggerml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 03:27:42.000000 loggerml-0.1.3/loggerml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 03:27:42.000000 loggerml-0.1.3/loggerml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.187008 loggerml-0.1.3/logml/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 03:27:24.000000 loggerml-0.1.3/logml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-27 03:27:24.000000 loggerml-0.1.3/logml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-27 03:27:24.000000 loggerml-0.1.3/logml/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-27 03:27:24.000000 loggerml-0.1.3/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-27 03:27:24.000000 loggerml-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 03:27:24.000000 loggerml-0.1.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 03:27:24.000000 loggerml-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 03:27:42.187008 loggerml-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 03:27:24.000000 loggerml-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.179008 loggerml-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.187008 loggerml-0.1.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-27 03:27:24.000000 loggerml-0.1.3/tests/integration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.187008 loggerml-0.1.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-27 03:27:24.000000 loggerml-0.1.3/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-27 03:27:24.000000 loggerml-0.1.3/tests/unit/test_time_utils.py
```

### Comparing `loggerml-0.1.2/.github/workflows/pipy_deployment.yaml` & `loggerml-0.1.3/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/.github/workflows/pydocstyle.yaml` & `loggerml-0.1.3/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/.github/workflows/pylint.yaml` & `loggerml-0.1.3/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/.github/workflows/tests.yaml` & `loggerml-0.1.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/.pylintrc` & `loggerml-0.1.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/CONTRIBUTING.md` & `loggerml-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/LICENSE` & `loggerml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/PKG-INFO` & `loggerml-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,48 @@
-Metadata-Version: 2.1
-Name: loggerml
-Version: 0.1.2
-Summary: Log your ml training in the console in an attractive way.
-Author-email: Valentin Goldite <valentin.goldite@gmail.com>
-Project-URL: Source, https://github.com/valentingol/logml
-Keywords: logging,machine,learning
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # LoggerML - Machine Learning Logger in the console
 
 Log your Machine Learning training in the console in a beautiful way ✨
 and with minimal code.
 
 Support all Unix and Emacs distribution and Windows 11.
 
-**Be careful, Windows 10 is not supported.**
-
-![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
+[![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
 ![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Ruff](https://github.com/valentingol/logml/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/ruff.yaml)
 [![Flake8](https://github.com/valentingol/logml/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/flake.yaml)
 [![Pydocstyle](https://github.com/valentingol/logml/actions/workflows/pydocstyle.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/pydocstyle.yaml)
 [![MyPy](https://github.com/valentingol/logml/actions/workflows/mypy.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/mypy.yaml)
 [![PyLint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_pylint.json)](https://github.com/valentingol/logml/actions/workflows/pylint.yaml)
 
 [![Tests](https://github.com/valentingol/logml/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_tests.json)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
-[![Bandit](https://github.com/valentingol/logml/actions/workflows/bandit.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/bandit.yaml)
 
 ## Installation
 
 In a new virtual environment, install simply the package via pipy:
 
 ```bash
-pip install logml
+pip install loggerml
 ```
 
-For **development**, install the package dynamically and dev requirements with:
-
-```bash
-pip install -e .
-pip install -r requirements-dev.txt
-```
+**Be careful, Windows 10 is not supported (but Windows 11 yes).**
 
 ## Quick start
 
 Integrate the LogML logger in your training loop. For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
+from logml import Logger
 
 logger = Logger(
     n_epochs=4,
     n_batches=20,
     log_interval=2,
 )
 for _ in range(4):
@@ -113,14 +94,21 @@
 
 - [ ] Manage a validation loop (then multiple loggers)
 - [ ] Enable not using `new_epoch/log()` if log config is minimal
 - [ ] Add color customization for message, epoch/batch number and time
 
 ## How to contribute
 
+For **development**, install the package dynamically and dev requirements with:
+
+```bash
+pip install -e .
+pip install -r requirements-dev.txt
+```
+
 Everyone can contribute to LogML, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
```

### Comparing `loggerml-0.1.2/README.md` & `loggerml-0.1.3/README_pipy.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,74 @@
 
 # LoggerML - Machine Learning Logger in the console
 
 Log your Machine Learning training in the console in a beautiful way ✨
 and with minimal code.
 
-Support all Unix and Emacs distribution and Windows 11.
+Support all Unix and Emacs distribution as well as Windows 11.
 
-**Be careful, Windows 10 is not supported.**
-
-![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
+[![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
 ![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Ruff](https://github.com/valentingol/logml/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/ruff.yaml)
 [![Flake8](https://github.com/valentingol/logml/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/flake.yaml)
 [![Pydocstyle](https://github.com/valentingol/logml/actions/workflows/pydocstyle.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/pydocstyle.yaml)
 [![MyPy](https://github.com/valentingol/logml/actions/workflows/mypy.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/mypy.yaml)
 [![PyLint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_pylint.json)](https://github.com/valentingol/logml/actions/workflows/pylint.yaml)
 
 [![Tests](https://github.com/valentingol/logml/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_tests.json)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
-[![Bandit](https://github.com/valentingol/logml/actions/workflows/bandit.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/bandit.yaml)
 
 ## Installation
 
 In a new virtual environment, install simply the package via pipy:
 
 ```bash
-pip install logml
+pip install loggerml
 ```
 
-For **development**, install the package dynamically and dev requirements with:
-
-```bash
-pip install -e .
-pip install -r requirements-dev.txt
-```
+**Be careful, Windows 10 is not supported (but Windows 11 yes).**
 
 ## Quick start
 
 Integrate the LogML logger in your training loop. For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
+from logml import Logger
 
 logger = Logger(
     n_epochs=4,
     n_batches=20,
     log_interval=2,
 )
 for _ in range(4):
     logger.start_epoch()  # Indicate the start of a new epoch
     for _ in range(20):
         logger.start_batch()  # Indicate the start of a new batch
-        # Log every 2 batches but you should call the log method at every batch
         logger.log({'loss': 0.54321256, 'accuracy': 0.85244777})
 ```
 
 Yields:
-![Alt Text](assets/base.gif)
+
+```script
+Epoch 1/4, batch 20/20
+[================================================][100%]
+[global 00:00:02 > 00:00:06 | epoch 00:00:02 > 00:00:00]
+loss: 0.5432 | accuracy: 0.8524 |
+
+Epoch 2/4, batch 8/20
+[=================>                              ][40%]
+[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
+loss: 0.5432 | accuracy: 0.8524 |
+```
 
 Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. For instance:
 
 ```python
 logger = Logger(
     n_epochs=4,
     n_batches=20,
@@ -85,30 +88,63 @@
             {'loss': 0.54321256, 'accuracy': 85.244777},
             styles={'loss': 'italic red'},
             message="Training is going well?\nYes!",
         )
 ```
 
 Yields:
-![Alt Text](assets/advanced.gif)
+
+```script
+Epoch 1/4, batch 20/20
+[================================================][100%]
+loss: 0.5432 | accuracy: 0.8524 |
+
+Epoch 2/4, batch 7/20
+[=================>                              ][35%]
+[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
+loss: 0.5432 | accuracy: 0.8524 |
+Training is going well?
+Yes!
+```
+
+With the following style and coloration:
+
+<span style="color:red">***loss***: *0.5432*</span> | <span style="color:yellow">**accuracy**: 0.8524</span> |
 
 Finally, if you don't have the number of batches in advance, you can initialize the logger with `n_batches=None`. Only the available information will be displayed. For instance with the configuration of the first example:
 
-![Alt Text](assets/no_n_batches.png)
+```script
+Epoch 1/4, batch 20/20
+[  *                                             ][ ? %]
+[global 00:00:02 >  ? | epoch 00:00:02 >  ? ]
+loss: 0.5432 | accuracy: 0.8524 |
+
+Epoch 2/4, batch 8/20
+[                           *                     ][ ? %]
+[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
+loss: 0.5432 | accuracy: 0.8524 |
+```
 
 The progress bar is replaced by a cyclic animation. The eta times are not know at the first epoch but was estimated after the second epoch.
 
 ## Todo
 
 - [ ] Manage a validation loop (then multiple loggers)
 - [ ] Enable not using `new_epoch/log()` if log config is minimal
 - [ ] Add color customization for message, epoch/batch number and time
 
 ## How to contribute
 
+For **development**, install the package dynamically and dev requirements with:
+
+```bash
+pip install -e .
+pip install -r requirements-dev.txt
+```
+
 Everyone can contribute to LogML, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
```

### Comparing `loggerml-0.1.2/assets/advanced.gif` & `loggerml-0.1.3/assets/advanced.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/assets/base.gif` & `loggerml-0.1.3/assets/base.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/assets/no_n_batches.png` & `loggerml-0.1.3/assets/no_n_batches.png`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/github_actions_utils/pydocstyle_manager.py` & `loggerml-0.1.3/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/github_actions_utils/pylint_manager.py` & `loggerml-0.1.3/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/github_actions_utils/pytest_manager.py` & `loggerml-0.1.3/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/loggerml.egg-info/PKG-INFO` & `loggerml-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,72 +12,75 @@
 
 
 # LoggerML - Machine Learning Logger in the console
 
 Log your Machine Learning training in the console in a beautiful way ✨
 and with minimal code.
 
-Support all Unix and Emacs distribution and Windows 11.
+Support all Unix and Emacs distribution as well as Windows 11.
 
-**Be careful, Windows 10 is not supported.**
-
-![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
+[![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
 ![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Ruff](https://github.com/valentingol/logml/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/ruff.yaml)
 [![Flake8](https://github.com/valentingol/logml/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/flake.yaml)
 [![Pydocstyle](https://github.com/valentingol/logml/actions/workflows/pydocstyle.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/pydocstyle.yaml)
 [![MyPy](https://github.com/valentingol/logml/actions/workflows/mypy.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/mypy.yaml)
 [![PyLint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_pylint.json)](https://github.com/valentingol/logml/actions/workflows/pylint.yaml)
 
 [![Tests](https://github.com/valentingol/logml/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_tests.json)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
-[![Bandit](https://github.com/valentingol/logml/actions/workflows/bandit.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/bandit.yaml)
 
 ## Installation
 
 In a new virtual environment, install simply the package via pipy:
 
 ```bash
-pip install logml
+pip install loggerml
 ```
 
-For **development**, install the package dynamically and dev requirements with:
-
-```bash
-pip install -e .
-pip install -r requirements-dev.txt
-```
+**Be careful, Windows 10 is not supported (but Windows 11 yes).**
 
 ## Quick start
 
 Integrate the LogML logger in your training loop. For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
+from logml import Logger
 
 logger = Logger(
     n_epochs=4,
     n_batches=20,
     log_interval=2,
 )
 for _ in range(4):
     logger.start_epoch()  # Indicate the start of a new epoch
     for _ in range(20):
         logger.start_batch()  # Indicate the start of a new batch
-        # Log every 2 batches but you should call the log method at every batch
         logger.log({'loss': 0.54321256, 'accuracy': 0.85244777})
 ```
 
 Yields:
-![Alt Text](assets/base.gif)
+
+```script
+Epoch 1/4, batch 20/20
+[================================================][100%]
+[global 00:00:02 > 00:00:06 | epoch 00:00:02 > 00:00:00]
+loss: 0.5432 | accuracy: 0.8524 |
+
+Epoch 2/4, batch 8/20
+[=================>                              ][40%]
+[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
+loss: 0.5432 | accuracy: 0.8524 |
+```
 
 Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. For instance:
 
 ```python
 logger = Logger(
     n_epochs=4,
     n_batches=20,
@@ -97,30 +100,63 @@
             {'loss': 0.54321256, 'accuracy': 85.244777},
             styles={'loss': 'italic red'},
             message="Training is going well?\nYes!",
         )
 ```
 
 Yields:
-![Alt Text](assets/advanced.gif)
+
+```script
+Epoch 1/4, batch 20/20
+[================================================][100%]
+loss: 0.5432 | accuracy: 0.8524 |
+
+Epoch 2/4, batch 7/20
+[=================>                              ][35%]
+[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
+loss: 0.5432 | accuracy: 0.8524 |
+Training is going well?
+Yes!
+```
+
+With the following style and coloration:
+
+<span style="color:red">***loss***: *0.5432*</span> | <span style="color:yellow">**accuracy**: 0.8524</span> |
 
 Finally, if you don't have the number of batches in advance, you can initialize the logger with `n_batches=None`. Only the available information will be displayed. For instance with the configuration of the first example:
 
-![Alt Text](assets/no_n_batches.png)
+```script
+Epoch 1/4, batch 20/20
+[  *                                             ][ ? %]
+[global 00:00:02 >  ? | epoch 00:00:02 >  ? ]
+loss: 0.5432 | accuracy: 0.8524 |
+
+Epoch 2/4, batch 8/20
+[                           *                     ][ ? %]
+[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
+loss: 0.5432 | accuracy: 0.8524 |
+```
 
 The progress bar is replaced by a cyclic animation. The eta times are not know at the first epoch but was estimated after the second epoch.
 
 ## Todo
 
 - [ ] Manage a validation loop (then multiple loggers)
 - [ ] Enable not using `new_epoch/log()` if log config is minimal
 - [ ] Add color customization for message, epoch/batch number and time
 
 ## How to contribute
 
+For **development**, install the package dynamically and dev requirements with:
+
+```bash
+pip install -e .
+pip install -r requirements-dev.txt
+```
+
 Everyone can contribute to LogML, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
```

### Comparing `loggerml-0.1.2/loggerml.egg-info/SOURCES.txt` & `loggerml-0.1.3/loggerml.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .flake8
 .gitignore
 .pylintrc
 CONTRIBUTING.md
 LICENSE
 README.md
+README_pipy.md
 pre-commit-checks.sh
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.py
 .github/workflows/flake.yaml
 .github/workflows/mypy.yaml
```

### Comparing `loggerml-0.1.2/logml/__init__.py` & `loggerml-0.1.3/logml/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/logml/logger.py` & `loggerml-0.1.3/logml/logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/logml/time_utils.py` & `loggerml-0.1.3/logml/time_utils.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/pre-commit-checks.sh` & `loggerml-0.1.3/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/pyproject.toml` & `loggerml-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [tool.setuptools_scm]
 
 [project.urls]
 Source = "https://github.com/valentingol/logml"
 
 [tool.setuptools.dynamic]
-readme = { file = ["README.md"] , content-type = "text/markdown" }
+readme = { file = ["README_pipy.md"] , content-type = "text/markdown" }
 dependencies = { file = ["requirements.txt"] }
 
 [tool.coverage.run]
 source = ["logml"]
 
 [tool.coverage.report]
 exclude_lines = ["if __name__ == '__main__':", "    main()"]
```

### Comparing `loggerml-0.1.2/tests/integration/logger.py` & `loggerml-0.1.3/tests/integration/logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/tests/unit/test_logger.py` & `loggerml-0.1.3/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.2/tests/unit/test_time_utils.py` & `loggerml-0.1.3/tests/unit/test_time_utils.py`

 * *Files identical despite different names*


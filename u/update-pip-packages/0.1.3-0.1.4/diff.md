# Comparing `tmp/update_pip_packages-0.1.3.tar.gz` & `tmp/update_pip_packages-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update_pip_packages-0.1.3.tar", max compression
+gzip compressed data, was "update_pip_packages-0.1.4.tar", max compression
```

## Comparing `update_pip_packages-0.1.3.tar` & `update_pip_packages-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     2232 2023-04-18 00:04:56.539638 update_pip_packages-0.1.3/README.md
--rw-r--r--   0        0        0      480 2023-04-18 00:03:24.315494 update_pip_packages-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-15 15:28:02.452473 update_pip_packages-0.1.3/update_project/__init__.py
--rw-r--r--   0        0        0     5650 2023-04-18 00:03:29.017160 update_pip_packages-0.1.3/update_project/update_packages.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 update_pip_packages-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2826 2023-04-27 21:04:40.759323 update_pip_packages-0.1.4/README.md
+-rw-r--r--   0        0        0      546 2023-04-27 19:09:40.845072 update_pip_packages-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-15 15:28:02.452473 update_pip_packages-0.1.4/update_project/__init__.py
+-rw-r--r--   0        0        0     5867 2023-04-27 17:30:55.745897 update_pip_packages-0.1.4/update_project/main.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:30:19.125534 update_pip_packages-0.1.4/update_project/update_app.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:30:06.938038 update_pip_packages-0.1.4/update_project/update_pip.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:32:34.379657 update_pip_packages-0.1.4/update_project/utils.py
+-rw-r--r--   0        0        0     3223 1970-01-01 00:00:00.000000 update_pip_packages-0.1.4/PKG-INFO
```

### Comparing `update_pip_packages-0.1.3/README.md` & `update_pip_packages-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Update Pip and App Packages
-## v0.1.3
+
+## v0.1.4
+
+![Python application](https://github.com/OleksandrMakarov/update-pip-project/actions/workflows/python-app.yml/badge.svg)
+[![Maintainability](https://api.codeclimate.com/v1/badges/af2bad1ec28de4bea881/maintainability)](https://codeclimate.com/github/OleksandrMakarov/update-pip-project/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/af2bad1ec28de4bea881/test_coverage)](https://codeclimate.com/github/OleksandrMakarov/update-pip-project/test_coverage)
 
 This Python script provides an efficient way to update Pip and app packages on various Linux distributions. The script supports Ubuntu, Debian, Fedora, CentOS, Red Hat, Arch, Manjaro, OpenSUSE, and SUSE distributions. It updates packages using the appropriate package manager for each distribution.
 
 **I know this script may seem useless. Moreover, updating all pip packages can lead to challenges in some projects.
 This script is only a part of my self-education journey.**
 
 ## Features
@@ -36,23 +41,27 @@
 
 
 ## Dependencies
 - [Python](https://www.python.org/) 3.6 or later
 - [Poetry](https://python-poetry.org/)
 - [pytest](https://pytest.org/)
 - [distro](https://pypi.org/project/distro/)
+- [toml](https://pypi.org/project/toml/)
 
 ## Installation
+From [PyPi.org](https://pypi.org/project/update-pip-packages/)
+
+In Linux:
 ```
 pip install update-pip-packages
 ```
 or
 ```
 python3 -m pip install update-pip-packages
 ```
 
 ## GitHub Repository
 For more information, source code, and installation instructions, please visit the GitHub repository: [GitHub: update-pip-packages](https://github.com/OleksandrMakarov/update-pip-project)
 
 ## Remarks
-There is also a [bash script](https://github.com/OleksandrMakarov/update-pip-project/blob/main/update_packages.sh), I started with it and developed it into this Python project. 
+There is also a [bash script](https://github.com/OleksandrMakarov/update-pip-project/blob/main/update_packages.sh). I started with it and developed it into this Python project. 
 It does not support Linux distribution detection, but you can use it for the same purposes as the main(python) application in a Debian or Ubuntu environment.
```

### Comparing `update_pip_packages-0.1.3/update_project/update_packages.py` & `update_pip_packages-0.1.4/update_project/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import json
 import subprocess
 import urllib.request
 import argparse
 import distro
+import toml
 
 
 def get_linux_distribution():
     return distro.id()
 
 
 def update_pip_packages() -> None:
@@ -127,14 +128,20 @@
     elif distro_id.lower() in ("opensuse", "suse"):
         update_zypper_packages()
     else:
         print(
             f"Unsupported distribution: {distro_id}. Cannot update packages.")
 
 
+def get_version_from_pyproject_toml() -> str:
+    with open("pyproject.toml") as f:
+        pyproject_toml = toml.load(f)
+    return pyproject_toml["tool"]["poetry"]["version"]
+
+
 def main() -> None:
     parser = argparse.ArgumentParser(description="Update pip and app packages")
     parser.add_argument('--pip', action='store_true',
                         help='Update pip packages')
     parser.add_argument('--app', action='store_true',
                         help='Update app packages')
     parser.add_argument('-v', '--version', action='store_true',
@@ -142,15 +149,15 @@
     args = parser.parse_args()
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
     if args.version:
-        version = "0.1.3"
+        version = get_version_from_pyproject_toml()
         print(f"update-pip-packages version: {version}")
         sys.exit(0)
 
     if args.pip:
         update_pip_packages()
     if args.app:
         update_app_packages()
```

### Comparing `update_pip_packages-0.1.3/PKG-INFO` & `update_pip_packages-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: update-pip-packages
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: OleksandrMakarov
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: distro (>=1.8.0,<2.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Update Pip and App Packages
-## v0.1.3
+
+## v0.1.4
+
+![Python application](https://github.com/OleksandrMakarov/update-pip-project/actions/workflows/python-app.yml/badge.svg)
+[![Maintainability](https://api.codeclimate.com/v1/badges/af2bad1ec28de4bea881/maintainability)](https://codeclimate.com/github/OleksandrMakarov/update-pip-project/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/af2bad1ec28de4bea881/test_coverage)](https://codeclimate.com/github/OleksandrMakarov/update-pip-project/test_coverage)
 
 This Python script provides an efficient way to update Pip and app packages on various Linux distributions. The script supports Ubuntu, Debian, Fedora, CentOS, Red Hat, Arch, Manjaro, OpenSUSE, and SUSE distributions. It updates packages using the appropriate package manager for each distribution.
 
 **I know this script may seem useless. Moreover, updating all pip packages can lead to challenges in some projects.
 This script is only a part of my self-education journey.**
 
 ## Features
@@ -48,24 +54,28 @@
 
 
 ## Dependencies
 - [Python](https://www.python.org/) 3.6 or later
 - [Poetry](https://python-poetry.org/)
 - [pytest](https://pytest.org/)
 - [distro](https://pypi.org/project/distro/)
+- [toml](https://pypi.org/project/toml/)
 
 ## Installation
+From [PyPi.org](https://pypi.org/project/update-pip-packages/)
+
+In Linux:
 ```
 pip install update-pip-packages
 ```
 or
 ```
 python3 -m pip install update-pip-packages
 ```
 
 ## GitHub Repository
 For more information, source code, and installation instructions, please visit the GitHub repository: [GitHub: update-pip-packages](https://github.com/OleksandrMakarov/update-pip-project)
 
 ## Remarks
-There is also a [bash script](https://github.com/OleksandrMakarov/update-pip-project/blob/main/update_packages.sh), I started with it and developed it into this Python project. 
+There is also a [bash script](https://github.com/OleksandrMakarov/update-pip-project/blob/main/update_packages.sh). I started with it and developed it into this Python project. 
 It does not support Linux distribution detection, but you can use it for the same purposes as the main(python) application in a Debian or Ubuntu environment.
```


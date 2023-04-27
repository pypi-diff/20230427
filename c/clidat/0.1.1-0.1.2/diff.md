# Comparing `tmp/clidat-0.1.1.tar.gz` & `tmp/clidat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidat-0.1.1.tar", max compression
+gzip compressed data, was "clidat-0.1.2.tar", max compression
```

## Comparing `clidat-0.1.1.tar` & `clidat-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1080 2023-03-02 10:34:24.005133 clidat-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      922 2023-03-08 16:58:36.191021 clidat-0.1.1/README.md
--rw-r--r--   0        0        0      552 2023-03-08 16:58:55.665336 clidat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-28 21:47:16.856299 clidat-0.1.1/src/clidat/__init__.py
--rw-r--r--   0        0        0      725 2023-03-08 15:28:22.676819 clidat-0.1.1/src/clidat/auth.py
--rw-r--r--   0        0        0        0 2023-03-02 20:56:17.317779 clidat-0.1.1/src/clidat/commands/__init__.py
--rw-r--r--   0        0        0     5230 2023-03-08 13:01:23.806590 clidat-0.1.1/src/clidat/commands/accounting.py
--rw-r--r--   0        0        0     2838 2023-03-08 13:19:00.712603 clidat-0.1.1/src/clidat/commands/platform.py
--rw-r--r--   0        0        0     1448 2023-03-08 15:09:54.747100 clidat-0.1.1/src/clidat/main.py
--rw-r--r--   0        0        0     2018 2023-03-08 11:01:51.419539 clidat-0.1.1/src/clidat/meta.py
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 clidat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-03-02 10:34:24.005133 clidat-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     1549 2023-04-26 21:55:06.099550 clidat-0.1.2/README.md
+-rw-r--r--   0        0        0      551 2023-04-27 14:48:13.912052 clidat-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-27 14:49:56.431180 clidat-0.1.2/src/clidat/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-23 18:09:08.316354 clidat-0.1.2/src/clidat/auth.py
+-rw-r--r--   0        0        0        0 2023-03-02 20:56:17.317779 clidat-0.1.2/src/clidat/commands/__init__.py
+-rw-r--r--   0        0        0     7148 2023-04-26 21:55:06.102566 clidat-0.1.2/src/clidat/commands/accounting.py
+-rw-r--r--   0        0        0     4060 2023-04-26 21:55:06.102882 clidat-0.1.2/src/clidat/commands/platform.py
+-rw-r--r--   0        0        0     1449 2023-04-26 21:55:06.103295 clidat-0.1.2/src/clidat/main.py
+-rw-r--r--   0        0        0     2568 2023-04-26 21:55:06.103694 clidat-0.1.2/src/clidat/meta.py
+-rw-r--r--   0        0        0     3179 2023-04-26 21:55:06.103916 clidat-0.1.2/src/clidat/tui/viewer.py
+-rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 clidat-0.1.2/PKG-INFO
```

### Comparing `clidat-0.1.1/LICENSE.md` & `clidat-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clidat-0.1.1/pyproject.toml` & `clidat-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "clidat"
-version = "0.1.1"
+version = "0.1.2"
 description = "CLI Tool for inspecting JSON Data from the Codat API"
 authors = ["Peter Simpson"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 pycompanydata = "^0.1.2"
-python-fx = "^0.2.0"
+textual = "^0.18.0"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.1"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
```

### Comparing `clidat-0.1.1/src/clidat/auth.py` & `clidat-0.1.2/src/clidat/auth.py`

 * *Files identical despite different names*

### Comparing `clidat-0.1.1/src/clidat/main.py` & `clidat-0.1.2/src/clidat/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import os
+
 import click
 from pycompanydata import Codat
-import os
 
 from clidat.auth import auth, get_token
 from clidat.commands.accounting import (
     get_account,
     get_account_transaction,
     get_account_transactions,
     get_accounts,
```

### Comparing `clidat-0.1.1/PKG-INFO` & `clidat-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,79 @@
 Metadata-Version: 2.1
 Name: clidat
-Version: 0.1.1
+Version: 0.1.2
 Summary: CLI Tool for inspecting JSON Data from the Codat API
 License: MIT
 Author: Peter Simpson
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pycompanydata (>=0.1.2,<0.2.0)
-Requires-Dist: python-fx (>=0.2.0,<0.3.0)
+Requires-Dist: textual (>=0.18.0,<0.19.0)
 Description-Content-Type: text/markdown
 
 # CLIdat
 
 CLIdat is a tool for inspecting Data from Codat.
 
 The Command Line Interface itself is written with [Click](https://github.com/pallets/click),
 whilst the output of the different commands is passed to
-a TUI from the [Pyfx](https://github.com/cielong/pyfx) package.
+a TUI from the [Textual](https://github.com/Textualize/textual) package.
+
+I work in support at Codat, and have built this tool as a personal project
+to help with my day-job. This isn't an officially 
+supported product.
 
 ## Installation
 
+CLIdat is distributed via the Python Package Index (PyPI). We reccomend installing
+it inside a [virtual environment](https://docs.python.org/3/library/venv.html)
+
 ```console
-pip install clidat
+(venv) user@host:~$ pip install clidat
 ```
+Thanks to Textual, this software is cross-platform and
+should work well on Windows, Linux and MacOS. 
+
 ## Quick Start
 
 ```console
-foo@bar:~$ clidat auth
+(venv) user@host:~$ clidat auth
 Your Codat API Key:
 
-foo@bar:~$ clidat --get-companies
+(venv) user@host:~$ clidat get-suppliers -id 2e14de3b-e2cf-4745-af24-a9a082b4c466
 ```
+![Clidat Get Companies](./clidat_get_suppliers_image.png)
+
 
 ## Docs
 
 To see a list of all avaliable commands run:
 ```console
-foo@bar:~$ run clidat --help
+(venv) user@host:~$ run clidat --help
 
   auth
   get-account
   get-account-transaction
   get-account-transactions
   ...
 
 ```
 To get details on a particular command, just append the --help 
 flag  onto the end of the command, for example: 
 
 ```console
-foo@bar:~$ clidat get-payment --help
+(venv) user@host:~$ clidat get-payment --help
 Options:
   --payment TEXT          [required]
   -id, --company-id TEXT  [required]
+  -j, --json              View plain JSON response
   --help                  Show this message and exit.
 
 
+
 ```
```


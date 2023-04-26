# Comparing `tmp/adafruit-circuitpython-ducky-1.0.9.tar.gz` & `tmp/adafruit-circuitpython-ducky-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ducky-1.0.9.tar", last modified: Mon Aug 22 18:58:58 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ducky-1.1.0.tar", last modified: Wed Apr 26 23:22:52 2023, max compression
```

## Comparing `adafruit-circuitpython-ducky-1.0.9.tar` & `adafruit-circuitpython-ducky-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:58:58.103019 adafruit-circuitpython-ducky-1.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:58:58.095018 adafruit-circuitpython-ducky-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:58:58.099019 adafruit-circuitpython-ducky-1.0.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:58:58.099019 adafruit-circuitpython-ducky-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:58:58.103019 adafruit-circuitpython-ducky-1.0.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4790 2022-08-22 18:58:58.103019 adafruit-circuitpython-ducky-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4034 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:58:58.103019 adafruit-circuitpython-ducky-1.0.9/adafruit_circuitpython_ducky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4790 2022-08-22 18:58:58.000000 adafruit-circuitpython-ducky-1.0.9/adafruit_circuitpython_ducky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-08-22 18:58:58.000000 adafruit-circuitpython-ducky-1.0.9/adafruit_circuitpython_ducky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:58:58.000000 adafruit-circuitpython-ducky-1.0.9/adafruit_circuitpython_ducky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-22 18:58:58.000000 adafruit-circuitpython-ducky-1.0.9/adafruit_circuitpython_ducky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-22 18:58:58.000000 adafruit-circuitpython-ducky-1.0.9/adafruit_circuitpython_ducky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6289 2022-08-22 18:58:50.000000 adafruit-circuitpython-ducky-1.0.9/adafruit_ducky.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:58:58.103019 adafruit-circuitpython-ducky-1.0.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:58:58.103019 adafruit-circuitpython-ducky-1.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5765 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:58:58.103019 adafruit-circuitpython-ducky-1.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-08-22 18:58:50.000000 adafruit-circuitpython-ducky-1.0.9/examples/ducky_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-08-22 18:58:50.000000 adafruit-circuitpython-ducky-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-22 18:58:40.000000 adafruit-circuitpython-ducky-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:58:58.103019 adafruit-circuitpython-ducky-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:22:52.052301 adafruit-circuitpython-ducky-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:22:52.044300 adafruit-circuitpython-ducky-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:22:52.048301 adafruit-circuitpython-ducky-1.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:22:52.048301 adafruit-circuitpython-ducky-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:22:52.048301 adafruit-circuitpython-ducky-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-26 23:22:52.052301 adafruit-circuitpython-ducky-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:22:52.048301 adafruit-circuitpython-ducky-1.1.0/adafruit_circuitpython_ducky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-26 23:22:52.000000 adafruit-circuitpython-ducky-1.1.0/adafruit_circuitpython_ducky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-26 23:22:52.000000 adafruit-circuitpython-ducky-1.1.0/adafruit_circuitpython_ducky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 23:22:52.000000 adafruit-circuitpython-ducky-1.1.0/adafruit_circuitpython_ducky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 23:22:52.000000 adafruit-circuitpython-ducky-1.1.0/adafruit_circuitpython_ducky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 23:22:52.000000 adafruit-circuitpython-ducky-1.1.0/adafruit_circuitpython_ducky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-26 23:22:43.000000 adafruit-circuitpython-ducky-1.1.0/adafruit_ducky.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:22:52.048301 adafruit-circuitpython-ducky-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:22:52.048301 adafruit-circuitpython-ducky-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:22:52.048301 adafruit-circuitpython-ducky-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-26 23:22:43.000000 adafruit-circuitpython-ducky-1.1.0/examples/ducky_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-26 23:22:43.000000 adafruit-circuitpython-ducky-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-26 23:22:29.000000 adafruit-circuitpython-ducky-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 23:22:52.052301 adafruit-circuitpython-ducky-1.1.0/setup.cfg
```

### Comparing `adafruit-circuitpython-ducky-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ducky-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ducky-1.0.9/.gitignore` & `adafruit-circuitpython-ducky-1.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-ducky-1.0.9/.pre-commit-config.yaml` & `adafruit-circuitpython-ducky-1.1.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.15.5
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-ducky-1.0.9/.pylintrc` & `adafruit-circuitpython-ducky-1.1.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-ducky-1.0.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ducky-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ducky-1.0.9/LICENSE` & `adafruit-circuitpython-ducky-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ducky-1.0.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ducky-1.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ducky-1.0.9/LICENSES/MIT.txt` & `adafruit-circuitpython-ducky-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ducky-1.0.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ducky-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ducky-1.0.9/PKG-INFO` & `adafruit-circuitpython-ducky-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ducky
-Version: 1.0.9
+Version: 1.1.0
 Summary: CircuitPython library for running DuckyScript
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Ducky.git
 Keywords: adafruit,blinka,circuitpython,micropython,ducky,ducky,,rubber,duckyscript
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ducky-1.0.9/README.rst` & `adafruit-circuitpython-ducky-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ducky-1.0.9/adafruit_circuitpython_ducky.egg-info/PKG-INFO` & `adafruit-circuitpython-ducky-1.1.0/adafruit_circuitpython_ducky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ducky
-Version: 1.0.9
+Version: 1.1.0
 Summary: CircuitPython library for running DuckyScript
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Ducky.git
 Keywords: adafruit,blinka,circuitpython,micropython,ducky,ducky,,rubber,duckyscript
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ducky-1.0.9/adafruit_circuitpython_ducky.egg-info/SOURCES.txt` & `adafruit-circuitpython-ducky-1.1.0/adafruit_circuitpython_ducky.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_ducky.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ducky.egg-info/PKG-INFO
 adafruit_circuitpython_ducky.egg-info/SOURCES.txt
 adafruit_circuitpython_ducky.egg-info/dependency_links.txt
 adafruit_circuitpython_ducky.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-ducky-1.0.9/adafruit_ducky.py` & `adafruit-circuitpython-ducky-1.1.0/adafruit_ducky.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,21 +22,20 @@
 """
 
 # imports
 import time
 from adafruit_hid.keycode import Keycode
 
 try:
-    from typing import Optional
     from adafruit_hid.keyboard import Keyboard
     from adafruit_hid.keyboard_layout_base import KeyboardLayoutBase
 except ImportError:
     pass
 
-__version__ = "1.0.9"
+__version__ = "1.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Ducky.git"
 
 commands = {
     "DELETE": Keycode.DELETE,
     "HOME": Keycode.HOME,
     "END": Keycode.END,
     "INSERT": Keycode.INSERT,
@@ -124,86 +123,84 @@
     def __init__(
         self, filename: str, keyboard: Keyboard, layout: KeyboardLayoutBase
     ) -> None:
         self.keyboard = keyboard
         self.layout = layout
         self.lines = []
         self.default_delay = 0
-        self.last = 0
+        self.prev_line = None
+        self.next_index = 0
+        self.wait_until = 0
+        self.repeat = 0
 
         with open(filename, "r") as duckyscript:
             for line in duckyscript:
-                self.lines.append(line[:-1])
+                line = line.lstrip(" ").rstrip("\n\r")
+                if len(line) > 0:
+                    self.lines.append(line)
 
     def loop(  # pylint: disable=too-many-return-statements
-        self, line: Optional[str] = None
+        self,
     ) -> bool:  # pylint: disable=too-many-branches
         """Function that sends a line of the DuckyScript file over hid every time it is called"""
-        if line is None:
-            try:
-                line = self.lines[0]
-            except IndexError:
-                print("Done!")
-                return False
-        if len(line) != 0:
-            words = line.split(" ", 1)
-            start = words[0]
-            if start == "REM":
-                print(words[1])
-                time.sleep(self.default_delay)
-                self.lines.pop(0)
-                return True
-
-            if start in ("DEFAULT_DELAY", "DEFAULTDELAY"):
-                self.default_delay = int(words[1]) / 1000
-                time.sleep(self.default_delay)
-                self.last = self.lines[0]
-                self.lines.pop(0)
-                return True
-
-            if start == "DELAY":
-                time.sleep(int(words[1]) / 1000)
-                time.sleep(self.default_delay)
-                self.last = self.lines[0]
-                self.lines.pop(0)
-                return True
-
-            if start == "STRING":
-                self.layout.write(words[1])
-                time.sleep(self.default_delay)
-                self.last = self.lines[0]
-                self.lines.pop(0)
-                return True
-
-            if start == "REPEAT":
-                print(int(words[1]))
-                for _ in range(int(words[1])):
-                    self.lines.insert(0, self.last)
-                    self.loop()
-                self.last = self.lines[0]
-                self.lines.pop(0)
-                return True
-
-            self.write_key(start)
-            if len(words) == 1:
-                time.sleep(self.default_delay)
-                self.last = self.lines[0]
-                self.lines.pop(0)
-                self.keyboard.release_all()
-                return True
-            if len(words[1]):
-                self.loop(line=words[1])
+
+        now = time.monotonic_ns()
+        if now < self.wait_until:
+            return True
+
+        try:
+            if self.repeat > 0:
+                self.repeat -= 1
+                line = self.prev_line
             else:
-                self.keyboard.release_all()
-                return True
+                line = self.lines[self.next_index]
+                self.next_index += 1
+        except IndexError:
+            print("  DONE!")
+            self.prev_line = None
+            self.next_index = 0
+            return False
+
+        words = line.split(" ", 1)
+        start = words[0]
+
+        if start == "REPEAT":
+            self.repeat = int(words[1])
+            return True
+
+        self.prev_line = line
+
+        # print(f"  {line}")
+
+        if start == "REM":
+            # print(words[1])
+            return True
+
+        self.wait_until = now + self.default_delay
+
+        if start in ("DEFAULT_DELAY", "DEFAULTDELAY"):
+            self.wait_until -= self.default_delay
+            self.default_delay = int(words[1]) * 1000000
+            self.wait_until += self.default_delay
+            return True
+
+        if start == "DELAY":
+            self.wait_until += int(words[1]) * 1000000
+            return True
+
+        if start == "STRING":
+            self.layout.write(words[1])
+            return True
+
+        self.write_key(start)
+        if len(words) > 1:
+            for key in filter(None, words[1].split(" ")):
+                self.write_key(key)
 
         self.keyboard.release_all()
-        time.sleep(self.default_delay)
-        self.last = self.lines[0]
-        self.lines.pop(0)
         return True
 
     def write_key(self, start: str) -> None:
         """Writes the keys over HID. Used to help with more complicated commands"""
         if start in commands:
             self.keyboard.press(commands[start])
         else:
```

### Comparing `adafruit-circuitpython-ducky-1.0.9/docs/_static/favicon.ico` & `adafruit-circuitpython-ducky-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ducky-1.0.9/docs/conf.py` & `adafruit-circuitpython-ducky-1.1.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -42,15 +43,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit CircuitPython Ducky Library"
-copyright = "2021 Eva Herrada"
+creation_year = "2021"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Eva Herrada"
 author = "Eva Herrada"
 
 # Ignore imports of these modules, which sphinx will not know about.
 autodoc_mock_imports = ["usb_hid"]
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
```

### Comparing `adafruit-circuitpython-ducky-1.0.9/docs/index.rst` & `adafruit-circuitpython-ducky-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ducky-1.0.9/examples/ducky_simpletest.py` & `adafruit-circuitpython-ducky-1.1.0/examples/ducky_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ducky-1.0.9/pyproject.toml` & `adafruit-circuitpython-ducky-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ducky"
 description = "CircuitPython library for running DuckyScript"
-version = "1.0.9"
+version = "1.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Ducky.git"}
 keywords = [
     "adafruit",
```


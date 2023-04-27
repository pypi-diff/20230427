# Comparing `tmp/code_genie-0.1.1.tar.gz` & `tmp/code_genie-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_genie-0.1.1.tar", last modified: Tue Apr 25 12:25:43 2023, max compression
+gzip compressed data, was "code_genie-0.1.2.tar", last modified: Thu Apr 27 10:15:44 2023, max compression
```

## Comparing `code_genie-0.1.1.tar` & `code_genie-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,26 @@
--rw-r--r--   0        0        0     1831 2023-04-25 05:29:52.444630 code_genie-0.1.1/.gitignore
--rw-r--r--   0        0        0       91 2023-04-25 05:29:52.445152 code_genie-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.1.1/LICENSE
--rw-r--r--   0        0        0     1272 2023-04-25 12:24:46.974510 code_genie-0.1.1/README.md
--rw-r--r--   0        0        0      456 2023-04-25 05:29:52.446244 code_genie-0.1.1/TODO.md
--rw-r--r--   0        0        0       72 2023-04-25 12:24:52.813699 code_genie-0.1.1/code_genie/__init__.py
--rw-r--r--   0        0        0     1752 2023-04-25 05:29:52.447321 code_genie-0.1.1/code_genie/client.py
--rw-r--r--   0        0        0     2384 2023-04-25 12:24:52.814422 code_genie-0.1.1/code_genie/genie.py
--rw-r--r--   0        0        0      998 2023-04-25 12:24:46.975841 code_genie-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      861 2023-04-25 12:24:52.815053 code_genie-0.1.1/tests/test_genie.py
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 code_genie-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      399 2023-04-27 10:15:39.146621 code_genie-0.1.2/.bumpversion.cfg
+-rw-r--r--   0        0        0     1831 2023-04-25 05:29:52.444630 code_genie-0.1.2/.gitignore
+-rw-r--r--   0        0        0      635 2023-04-27 10:15:39.147415 code_genie-0.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0       91 2023-04-25 05:29:52.445152 code_genie-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1556 2023-04-27 10:15:39.147818 code_genie-0.1.2/README.md
+-rw-r--r--   0        0        0      456 2023-04-25 05:29:52.446244 code_genie-0.1.2/TODO.md
+-rw-r--r--   0        0        0       72 2023-04-27 10:15:39.148170 code_genie-0.1.2/code_genie/__init__.py
+-rw-r--r--   0        0        0     1752 2023-04-25 05:29:52.447321 code_genie-0.1.2/code_genie/client.py
+-rw-r--r--   0        0        0     5153 2023-04-27 10:15:39.149106 code_genie-0.1.2/code_genie/genie.py
+-rw-r--r--   0        0        0      679 2023-04-27 10:15:39.149821 code_genie-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0       92 2023-04-27 10:15:39.151209 code_genie-0.1.2/docs/api.rst
+-rw-r--r--   0        0        0     1492 2023-04-27 10:15:39.151752 code_genie-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0       81 2023-04-27 10:15:39.152197 code_genie-0.1.2/docs/examples.rst
+-rw-r--r--   0        0        0      284 2023-04-27 10:15:39.153008 code_genie-0.1.2/docs/generated/code_genie.client.rst
+-rw-r--r--   0        0        0      226 2023-04-27 10:15:39.153533 code_genie-0.1.2/docs/generated/code_genie.genie.rst
+-rw-r--r--   0        0        0      123 2023-04-27 10:15:39.154001 code_genie-0.1.2/docs/genie.rst
+-rw-r--r--   0        0        0     1110 2023-04-27 10:15:39.154405 code_genie-0.1.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-04-27 10:15:39.155023 code_genie-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0    73251 2023-04-27 10:15:39.156165 code_genie-0.1.2/docs/notebooks/Starter.ipynb
+-rw-r--r--   0        0        0       54 2023-04-27 10:15:39.156660 code_genie-0.1.2/docs/requirements.in
+-rw-r--r--   0        0        0     3100 2023-04-27 10:15:39.156993 code_genie-0.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0     1212 2023-04-27 10:15:39.157311 code_genie-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      861 2023-04-27 07:56:53.649350 code_genie-0.1.2/tests/test_genie.py
+-rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 code_genie-0.1.2/PKG-INFO
```

### Comparing `code_genie-0.1.1/.gitignore` & `code_genie-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.1/LICENSE` & `code_genie-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.1/README.md` & `code_genie-0.1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # code-genie
 This library is your copilot for jupyter notebooks
 
+Latest version: 0.1.2
+
+## Documentation
+
+- [Started Notebook](https://code-genie.readthedocs.io/en/latest/notebooks/Starter.html)
+- [All Exampples](https://code-genie.readthedocs.io/en/latest/examples.html)
+- [API Documentation](https://code-genie.readthedocs.io/en/latest/api.html)
+
 ## Installation
 
 ```bash
 pip install code-genie
 ```
 
 ## Access Token
```

### Comparing `code_genie-0.1.1/code_genie/client.py` & `code_genie-0.1.2/code_genie/client.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.1/pyproject.toml` & `code_genie-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -30,15 +30,28 @@
 [project.optional-dependencies]
 build = [
     "coverage>=5,<6",
     "pytest>=6,<=7",
     "pytest-cov>=2.5,<3",
     "tox>=3.24,<4",
     "isort>=5.10,<6",
-    "python-dotenv"
+    "python-dotenv",
+    "pip-tools",
+    "bumpversion"
+]
+docs = [
+    "sphinx==5.3.0",
+    "autodocsumm",
+    "sphinx_rtd_theme",
+    "nbsphinx",
+    "sphinx_gallery"
+]
+notebook = [
+    "jupyterlab>=3.1,<4",
+    "ipykernel>=6.0,<7",
 ]
 
 [project.urls]
 Documentation = "https://TBD"
 Source = "https://github.com/thismlguy/code-genie"
 
 [tool.flit.sdist]
```

### Comparing `code_genie-0.1.1/tests/test_genie.py` & `code_genie-0.1.2/tests/test_genie.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.1/PKG-INFO` & `code_genie-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code_genie
-Version: 0.1.1
+Version: 0.1.2
 Summary: Copilot to supercharge your notebooks
 Keywords: copilot,jupyter
 Author-email: Aarshay Jain <aarshay.jain@columbia.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,21 +17,40 @@
 Requires-Dist: seaborn>=0.11,<1
 Requires-Dist: coverage>=5,<6 ; extra == "build"
 Requires-Dist: pytest>=6,<=7 ; extra == "build"
 Requires-Dist: pytest-cov>=2.5,<3 ; extra == "build"
 Requires-Dist: tox>=3.24,<4 ; extra == "build"
 Requires-Dist: isort>=5.10,<6 ; extra == "build"
 Requires-Dist: python-dotenv ; extra == "build"
+Requires-Dist: pip-tools ; extra == "build"
+Requires-Dist: bumpversion ; extra == "build"
+Requires-Dist: sphinx==5.3.0 ; extra == "docs"
+Requires-Dist: autodocsumm ; extra == "docs"
+Requires-Dist: sphinx_rtd_theme ; extra == "docs"
+Requires-Dist: nbsphinx ; extra == "docs"
+Requires-Dist: sphinx_gallery ; extra == "docs"
+Requires-Dist: jupyterlab>=3.1,<4 ; extra == "notebook"
+Requires-Dist: ipykernel>=6.0,<7 ; extra == "notebook"
 Project-URL: Documentation, https://TBD
 Project-URL: Source, https://github.com/thismlguy/code-genie
 Provides-Extra: build
+Provides-Extra: docs
+Provides-Extra: notebook
 
 # code-genie
 This library is your copilot for jupyter notebooks
 
+Latest version: 0.1.2
+
+## Documentation
+
+- [Started Notebook](https://code-genie.readthedocs.io/en/latest/notebooks/Starter.html)
+- [All Exampples](https://code-genie.readthedocs.io/en/latest/examples.html)
+- [API Documentation](https://code-genie.readthedocs.io/en/latest/api.html)
+
 ## Installation
 
 ```bash
 pip install code-genie
 ```
 
 ## Access Token
```


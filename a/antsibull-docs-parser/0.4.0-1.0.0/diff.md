# Comparing `tmp/antsibull_docs_parser-0.4.0.tar.gz` & `tmp/antsibull_docs_parser-1.0.0.tar.gz`

## Comparing `antsibull_docs_parser-0.4.0.tar` & `antsibull_docs_parser-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.flake8
--rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.pylintrc.automated
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/CHANGELOG.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/CHANGELOG.rst.license
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/codecov.yml
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/noxfile.py
--rw-r--r--   0        0        0   141180 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/test-vectors.yaml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.github/workflows/nox.yml
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.reuse/dep5
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/changelogs/changelog.yaml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/changelogs/changelog.yaml.license
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/changelogs/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/changelogs/fragments/.keep
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/__init__.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/_parser_impl.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/ansible_doc_text.py
--rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/dom.py
--rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/format.py
--rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/html.py
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/md.py
--rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/py.typed
--rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/rst.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/__init__.py
--rwxr-xr-x   0        0        0     2561 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/create-vectors.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_ansible_doc_text.py
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_dom.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_format.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_html.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_md.py
--rw-r--r--   0        0        0    24557 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_parser.py
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_parser_impl.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_rst.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_vectors.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/vectors.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.gitignore
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/README.md
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/LICENSES/BSD-2-Clause.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/.flake8
+-rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/.pylintrc.automated
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/CHANGELOG.rst.license
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/codecov.yml
+-rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/noxfile.py
+-rw-r--r--   0        0        0   141180 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/test-vectors.yaml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/.reuse/dep5
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/changelogs/changelog.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/changelogs/changelog.yaml.license
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/changelogs/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/changelogs/fragments/.keep
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/__init__.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/_parser_impl.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/ansible_doc_text.py
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/dom.py
+-rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/format.py
+-rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/html.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/md.py
+-rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/py.typed
+-rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/rst.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/__init__.py
+-rwxr-xr-x   0        0        0     2561 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/create-vectors.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/test_ansible_doc_text.py
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/test_dom.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/test_format.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/test_html.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/test_md.py
+-rw-r--r--   0        0        0    24557 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/test_parser.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/test_parser_impl.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/test_rst.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/test_vectors.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/tests/unit/vectors.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/.gitignore
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/README.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/LICENSES/BSD-2-Clause.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 antsibull_docs_parser-1.0.0/PKG-INFO
```

### Comparing `antsibull_docs_parser-0.4.0/.pylintrc.automated` & `antsibull_docs_parser-1.0.0/.pylintrc.automated`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/CHANGELOG.rst` & `antsibull_docs_parser-1.0.0/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 =================================================================================================
 antsibull-docs-parser -- Python library for processing Ansible documentation markup Release Notes
 =================================================================================================
 
 .. contents:: Topics
 
 
+v1.0.0
+======
+
+Release Summary
+---------------
+
+First stable release. This package is using semantic versioning, so there will be no more breaking changes until the release of 2.0.0.
+
 v0.4.0
 ======
 
 Release Summary
 ---------------
 
 Feature and bugfix release.
```

### Comparing `antsibull_docs_parser-0.4.0/LICENSE` & `antsibull_docs_parser-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/noxfile.py` & `antsibull_docs_parser-1.0.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,16 @@
     )
     session.run("reuse", "lint")
     session.run("antsibull-changelog", "lint")
 
 
 @nox.session
 def typing(session: nox.Session):
-    install(session, ".[typing]", editable=True)
+    # pyre does not work when we don't install ourself in editable mode 🙄.
+    install(session, "-e", ".[typing]")
     session.run("mypy", "src/antsibull_docs_parser")
     session.run("pyre", "--source-directory", "src")
 
 
 @nox.session
 def create_vectors(session: nox.Session):
     install(session, ".", "ruamel.yaml", editable=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `antsibull_docs_parser-0.4.0/test-vectors.yaml` & `antsibull_docs_parser-1.0.0/test-vectors.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/.github/workflows/nox.yml` & `antsibull_docs_parser-1.0.0/.github/workflows/nox.yml`

 * *Files 12% similar despite different names*

```diff
@@ -11,27 +11,30 @@
   pull_request:
     branches: [main]
   # Run once per week (Monday at 04:00 UTC)
   schedule:
     - cron: '0 4 * * 1'
   workflow_dispatch:
 
+env:
+  FORCE_COLOR: "1"
+
 jobs:
   nox-lint:
     runs-on: ubuntu-latest
     defaults:
       run:
         working-directory: antsibull-docs-parser
     steps:
       - name: Check out antsibull-docs-parser
         uses: actions/checkout@v3
         with:
           path: antsibull-docs-parser
       - name: Setup nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
         with:
           python-versions: "3.11"
       - run: |
           nox -v -e lint
   nox-test:
     runs-on: ubuntu-latest
     defaults:
@@ -39,61 +42,68 @@
         working-directory: antsibull-docs-parser
     steps:
       - name: Check out antsibull-docs-parser
         uses: actions/checkout@v3
         with:
           path: antsibull-docs-parser
       - name: Setup nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
         with:
           python-versions: "3.7, 3.8, 3.9, 3.10, 3.11"
       - name: Run unit tests
         run: |
           nox -v -e test -p 3.7 3.8 3.9 3.10 3.11
       - name: Report coverage
         run: |
           nox -v -e coverage
       - name: Upload coverage
         uses: codecov/codecov-action@v3
         with:
-          working-directory: antsibull-docs-parser
+          name: nox-test
+          directory: antsibull-docs-parser
   nox-test-36:
     # python3.6 is not available on ubuntu-latest
     runs-on: ubuntu-20.04
     defaults:
       run:
         working-directory: antsibull-docs-parser
     steps:
       - name: Check out antsibull-docs-parser
         uses: actions/checkout@v3
         with:
           path: antsibull-docs-parser
       - name: Setup nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
         with:
           python-versions: "3.6"
+      # https://github.com/ansible-community/antsibull-docs-parser/issues/25
+      # Newer virtualenv versions seem to cause failures with Python 3.6
+      - name: Setup nox - downgrade virtualenv
+        run: |
+          pipx inject nox 'virtualenv<20.22.0'
       - name: Run unit tests
         run: |
           nox -v -e test -p 3.6
       - name: Report coverage
         run: |
           nox -v -e coverage
       - name: Upload coverage
         uses: codecov/codecov-action@v3
         with:
-          working-directory: antsibull-docs-parser
+          name: nox-test-36
+          directory: antsibull-docs-parser
   nox-vectors:
     runs-on: ubuntu-latest
     defaults:
       run:
         working-directory: antsibull-docs-parser
     steps:
       - name: Check out antsibull-docs-parser
         uses: actions/checkout@v3
         with:
           path: antsibull-docs-parser
       - name: Setup nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
         with:
           python-versions: "3.11"
       - run: |
           nox -v -e create_vectors
```

### Comparing `antsibull_docs_parser-0.4.0/changelogs/changelog.yaml` & `antsibull_docs_parser-1.0.0/changelogs/changelog.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -53,7 +53,14 @@
       - Adjust URL escaping to be more similar to JavaScript's ``encodeURI()`` (https://github.com/ansible-community/antsibull-docs-parser/pull/24).
       - Also escape ``.`` in MarkDown (https://github.com/ansible-community/antsibull-docs-parser/pull/24).
       release_summary: Feature and bugfix release.
     fragments:
     - 0.4.0.yml
     - 24-urls-md.yml
     release_date: '2023-04-23'
+  1.0.0:
+    changes:
+      release_summary: First stable release. This package is using semantic versioning,
+        so there will be no more breaking changes until the release of 2.0.0.
+    fragments:
+    - 1.0.0.yml
+    release_date: '2023-04-27'
```

### Comparing `antsibull_docs_parser-0.4.0/changelogs/config.yaml` & `antsibull_docs_parser-1.0.0/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/_parser_impl.py` & `antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/_parser_impl.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/ansible_doc_text.py` & `antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/ansible_doc_text.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/dom.py` & `antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/dom.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/format.py` & `antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/format.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/html.py` & `antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/html.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/md.py` & `antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/md.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/parser.py` & `antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/parser.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/rst.py` & `antsibull_docs_parser-1.0.0/src/antsibull_docs_parser/rst.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/tests/unit/create-vectors.py` & `antsibull_docs_parser-1.0.0/tests/unit/create-vectors.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/tests/unit/test_dom.py` & `antsibull_docs_parser-1.0.0/tests/unit/test_dom.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/tests/unit/test_format.py` & `antsibull_docs_parser-1.0.0/tests/unit/test_format.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/tests/unit/test_html.py` & `antsibull_docs_parser-1.0.0/tests/unit/test_html.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/tests/unit/test_md.py` & `antsibull_docs_parser-1.0.0/tests/unit/test_md.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/tests/unit/test_parser.py` & `antsibull_docs_parser-1.0.0/tests/unit/test_parser.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/tests/unit/test_parser_impl.py` & `antsibull_docs_parser-1.0.0/tests/unit/test_parser_impl.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/tests/unit/test_rst.py` & `antsibull_docs_parser-1.0.0/tests/unit/test_rst.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/tests/unit/test_vectors.py` & `antsibull_docs_parser-1.0.0/tests/unit/test_vectors.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/tests/unit/vectors.py` & `antsibull_docs_parser-1.0.0/tests/unit/vectors.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/.gitignore` & `antsibull_docs_parser-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/README.md` & `antsibull_docs_parser-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/pyproject.toml` & `antsibull_docs_parser-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "antsibull-docs-parser"
-version = "0.4.0"
+version = "1.0.0"
 description = "Python library for processing Ansible documentation markup"
 readme = "README.md"
 requires-python = ">=3.6.1"
 license = "GPL-3.0-or-later AND BSD-2-Clause"
 license-files.globs = ["LICENSES/*.txt"]
 authors = [
   { name = "Felix Fontein", email = "felix@fontein.de" },
```

### Comparing `antsibull_docs_parser-0.4.0/LICENSES/BSD-2-Clause.txt` & `antsibull_docs_parser-1.0.0/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.4.0/PKG-INFO` & `antsibull_docs_parser-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antsibull-docs-parser
-Version: 0.4.0
+Version: 1.0.0
 Summary: Python library for processing Ansible documentation markup
 Project-URL: Source code, https://github.com/ansible-community/antsibull-docs-parser/
 Author-email: Felix Fontein <felix@fontein.de>
 Maintainer-email: Felix Fontein <felix@fontein.de>, Maxwell G <maxwell@gtmx.me>
 License-Expression: GPL-3.0-or-later AND BSD-2-Clause
 License-File: LICENSES/BSD-2-Clause.txt
 License-File: LICENSES/GPL-3.0-or-later.txt
```


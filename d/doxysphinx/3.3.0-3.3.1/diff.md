# Comparing `tmp/doxysphinx-3.3.0.tar.gz` & `tmp/doxysphinx-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doxysphinx-3.3.0.tar", max compression
+gzip compressed data, was "doxysphinx-3.3.1.tar", max compression
```

## Comparing `doxysphinx-3.3.0.tar` & `doxysphinx-3.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1068 2023-04-20 08:34:40.644352 doxysphinx-3.3.0/LICENSE
--rw-r--r--   0        0        0     1078 2023-04-20 08:34:40.644352 doxysphinx-3.3.0/LICENSE.md
--rw-r--r--   0        0        0     2602 2023-04-20 08:34:40.644352 doxysphinx-3.3.0/README.md
--rw-r--r--   0        0        0      926 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/__init__.py
--rw-r--r--   0        0        0      608 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/__main__.py
--rw-r--r--   0        0        0     8173 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/cli.py
--rw-r--r--   0        0        0    12644 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/doxygen.py
--rw-r--r--   0        0        0    21980 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/html_parser.py
--rw-r--r--   0        0        0     9102 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/process.py
--rw-r--r--   0        0        0     5925 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/resources/custom.scss
--rw-r--r--   0        0        0        0 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/resources/toc_template.html.j2
--rw-r--r--   0        0        0    11513 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/resources.py
--rw-r--r--   0        0        0     2943 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/sphinx.py
--rw-r--r--   0        0        0    10867 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/toc.py
--rw-r--r--   0        0        0      527 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/__init__.py
--rw-r--r--   0        0        0     2282 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/contexts.py
--rw-r--r--   0        0        0     1156 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/exceptions.py
--rw-r--r--   0        0        0     6235 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/files.py
--rw-r--r--   0        0        0     1757 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/iterators.py
--rw-r--r--   0        0        0     1431 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/pathlib_fix.py
--rw-r--r--   0        0        0      924 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/utils/rst.py
--rw-r--r--   0        0        0    12187 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/doxysphinx/writer.py
--rw-r--r--   0        0        0     4193 2023-04-20 08:34:40.660352 doxysphinx-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 doxysphinx-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-27 15:00:44.151461 doxysphinx-3.3.1/LICENSE
+-rw-r--r--   0        0        0     1078 2023-04-27 15:00:44.151461 doxysphinx-3.3.1/LICENSE.md
+-rw-r--r--   0        0        0     2602 2023-04-27 15:00:44.151461 doxysphinx-3.3.1/README.md
+-rw-r--r--   0        0        0      926 2023-04-27 15:00:44.163461 doxysphinx-3.3.1/doxysphinx/__init__.py
+-rw-r--r--   0        0        0      608 2023-04-27 15:00:44.163461 doxysphinx-3.3.1/doxysphinx/__main__.py
+-rw-r--r--   0        0        0     8173 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/cli.py
+-rw-r--r--   0        0        0    12644 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/doxygen.py
+-rw-r--r--   0        0        0    21980 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/html_parser.py
+-rw-r--r--   0        0        0     9102 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/process.py
+-rw-r--r--   0        0        0     5925 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/resources/custom.scss
+-rw-r--r--   0        0        0        0 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/resources/toc_template.html.j2
+-rw-r--r--   0        0        0    11513 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/resources.py
+-rw-r--r--   0        0        0     2943 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/sphinx.py
+-rw-r--r--   0        0        0    11504 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/toc.py
+-rw-r--r--   0        0        0      527 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/utils/__init__.py
+-rw-r--r--   0        0        0     2282 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/utils/contexts.py
+-rw-r--r--   0        0        0     1156 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/utils/exceptions.py
+-rw-r--r--   0        0        0     6235 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/utils/files.py
+-rw-r--r--   0        0        0     1757 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/utils/iterators.py
+-rw-r--r--   0        0        0     1431 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/utils/pathlib_fix.py
+-rw-r--r--   0        0        0      924 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/utils/rst.py
+-rw-r--r--   0        0        0    12187 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/doxysphinx/writer.py
+-rw-r--r--   0        0        0     4193 2023-04-27 15:00:44.167461 doxysphinx-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 doxysphinx-3.3.1/PKG-INFO
```

### Comparing `doxysphinx-3.3.0/LICENSE` & `doxysphinx-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/LICENSE.md` & `doxysphinx-3.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/README.md` & `doxysphinx-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/__init__.py` & `doxysphinx-3.3.1/doxysphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/__main__.py` & `doxysphinx-3.3.1/doxysphinx/__main__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/cli.py` & `doxysphinx-3.3.1/doxysphinx/cli.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/doxygen.py` & `doxysphinx-3.3.1/doxysphinx/doxygen.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/html_parser.py` & `doxysphinx-3.3.1/doxysphinx/html_parser.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/process.py` & `doxysphinx-3.3.1/doxysphinx/process.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/resources/custom.scss` & `doxysphinx-3.3.1/doxysphinx/resources/custom.scss`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/resources.py` & `doxysphinx-3.3.1/doxysphinx/resources.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/sphinx.py` & `doxysphinx-3.3.1/doxysphinx/sphinx.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/toc.py` & `doxysphinx-3.3.1/doxysphinx/toc.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #
 #  Author(s):
 #  - Markus Braun, :em engineering methods AG (contracted by Robert Bosch GmbH)
 # =====================================================================================
 """The toc module contains classes related to the toctree generation for doxygen htmls/rsts."""
 
 import re
+import unicodedata
 from dataclasses import dataclass, field, replace
 from pathlib import Path
 from typing import Any, Dict, Iterable, Iterator, List, Protocol, Tuple
 
 from doxysphinx.doxygen import read_js_data_file
 from doxysphinx.utils.files import write_file
 from doxysphinx.utils.iterators import apply
@@ -184,16 +185,30 @@
 
         # replace the original index title with a marker that we can easily replace afterwards
         replace_regex = re.compile('(?<=<div class="title">).*?(?=</div>)')
         prefix_replaced = replace_regex.sub("@@@-TITLE-@@@", prefix)
 
         return prefix_replaced + split_start_search.replace('\\"', '"'), split_end_search + suffix
 
+    def _sanitize_filename(self, value: str) -> str:
+        """Sanitize value to make it usable as a filename.
+
+        - Try to replace unicode characters with ascii fallbacks
+        - drop any remaining non-ascii characters
+        - converts to lower case
+        - replace whitespace and slashes with underscores
+        - keeps only alphanumerics, dash and underscore
+        """
+        value = unicodedata.normalize("NFKD", value)
+        value = value.encode("ascii", "ignore").decode("ascii")
+        value = re.sub(r"[\s/]", "_", value.lower())
+        return re.sub(r"[^\w\-_]", "", value)
+
     def _prepare_structural_dummy(self, structural_dummy: _MenuEntry):
-        clean_title = structural_dummy.title.replace(" ", "_").lower()
+        clean_title = self._sanitize_filename(structural_dummy.title)
         toc_docname = f"{structural_dummy.docname}_{clean_title}"
         structural_dummy.docname = toc_docname
 
     def _create_toc_file_for_structural_dummy(self, structural_dummy: _MenuEntry):
         prefix, suffix = self._doxy_html_template
 
         content = [
```

### Comparing `doxysphinx-3.3.0/doxysphinx/utils/__init__.py` & `doxysphinx-3.3.1/doxysphinx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/utils/contexts.py` & `doxysphinx-3.3.1/doxysphinx/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/utils/exceptions.py` & `doxysphinx-3.3.1/doxysphinx/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/utils/files.py` & `doxysphinx-3.3.1/doxysphinx/utils/files.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/utils/iterators.py` & `doxysphinx-3.3.1/doxysphinx/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/utils/pathlib_fix.py` & `doxysphinx-3.3.1/doxysphinx/utils/pathlib_fix.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/utils/rst.py` & `doxysphinx-3.3.1/doxysphinx/utils/rst.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/doxysphinx/writer.py` & `doxysphinx-3.3.1/doxysphinx/writer.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.0/pyproject.toml` & `doxysphinx-3.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ##
 ##  Author(s):
 ##  - Markus Braun, :em engineering methods AG (contracted by Robert Bosch GmbH)
 ## =====================================================================================
 
 [tool.poetry]
 name = "doxysphinx"
-version = "3.3.0"
+version = "3.3.1"
 description = "Integrates doxygen html documentation with sphinx."
 authors = [
     "Nirmal Sasidharan <nirmal.sasidharan@de.bosch.com>",
     "Markus Braun <markus.braun@em.ag>",
     "Aniket Salve <aniketdilip.salve@bosch.com>",
 ]
 maintainers = ["Nirmal Sasidharan <nirmal.sasidharan@de.bosch.com>"]
@@ -80,15 +80,15 @@
 commitizen = "^2.42.1"
 
 [tool.poetry.scripts]
 doxysphinx = "doxysphinx.cli:cli"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.3.0"
+version = "3.3.1"
 tag_format = "v$version"
 version_files = ["pyproject.toml:^version"]
 bump_message = """chore(release): release $current_version → $new_version by commitizen [skip-ci]
 
 Signed-off-by: github-actions <actions@github.com>
 """
```

### Comparing `doxysphinx-3.3.0/PKG-INFO` & `doxysphinx-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doxysphinx
-Version: 3.3.0
+Version: 3.3.1
 Summary: Integrates doxygen html documentation with sphinx.
 Home-page: https://github.com/boschglobal/doxysphinx
 License: MIT
 Keywords: DaC,docs-as-code,doxygen,sphinx
 Author: Nirmal Sasidharan
 Author-email: nirmal.sasidharan@de.bosch.com
 Maintainer: Nirmal Sasidharan
```


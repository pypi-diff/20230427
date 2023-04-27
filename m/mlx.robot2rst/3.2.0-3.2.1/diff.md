# Comparing `tmp/mlx.robot2rst-3.2.0.tar.gz` & `tmp/mlx.robot2rst-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mlx.robot2rst-3.2.0.tar", last modified: Tue Apr 25 09:42:07 2023, max compression
+gzip compressed data, was "dist/mlx.robot2rst-3.2.1.tar", last modified: Thu Apr 27 08:54:31 2023, max compression
```

## Comparing `mlx.robot2rst-3.2.0.tar` & `mlx.robot2rst-3.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/example.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/requirements.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/doc/source/robot/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/robot/example.robot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/mlx/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/mlx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/mlx/robot2rst.mako
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/mlx/robot2rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/mlx/robot_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/requirements.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/doc/source/robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/robot/example.robot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/mlx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/mlx/robot2rst.mako
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/mlx/robot2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/mlx/robot_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/tox.ini
```

### Comparing `mlx.robot2rst-3.2.0/.github/workflows/codeql-analysis.yml` & `mlx.robot2rst-3.2.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/.github/workflows/python-package.yml` & `mlx.robot2rst-3.2.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/.gitignore` & `mlx.robot2rst-3.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/LICENSE` & `mlx.robot2rst-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/PKG-INFO` & `mlx.robot2rst-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.robot2rst
-Version: 3.2.0
+Version: 3.2.1
 Summary: Python script for converting a Robot Framework file to a reStructuredText (.rst) file
 Home-page: https://github.com/melexis/robot2rst
 Author: Jasper Craeghs
 Author-email: jce@melexis.com
 License: Apache License Version 2.0
 Description: .. image:: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml/badge.svg?branch=master
             :target: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml
```

### Comparing `mlx.robot2rst-3.2.0/README.rst` & `mlx.robot2rst-3.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/doc/Makefile` & `mlx.robot2rst-3.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/doc/source/conf.py` & `mlx.robot2rst-3.2.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/doc/source/robot/example.robot` & `mlx.robot2rst-3.2.1/doc/source/robot/example.robot`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 *** Settings ***
 Documentation    Example using the space separated plain text format.
 Library          OperatingSystem
 
 *** Variables ***
+${NAMES}   Create List   First Name  Family Name  Email
 ${NAD}    ${0x63}
-${MESSAGE}       Hello,
+${MESSAGE}     Hello,
 ...    world!
 
 *** Test Cases ***
 First Test
     [Documentation]     Thorough and relatively lengthy documentation for the example test case that
-    ...  logs ${MESSAGE} and ${NAD}.
+    ...  logs ${MESSAGE} and ${NAD} and ${NAMES}.
     [Tags]              SWRQT-SOME_RQT  ANOTHER-TAG  SWRQT-OTHER_RQT  SYSRQT-SOME_SYSTEM_RQT
                         Log    ${MESSAGE}
                         Log    ${NAD}
                         My Keyword    /tmp
 
 Undocumented Test
                         Should Be Equal     ${MESSAGE}    Hello, world!
@@ -27,17 +28,17 @@
     ...  - Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
     ...
     ...      - Nested bullet point
                         Log  The line endings and indents in a docstring get preserved.
 
 Another Test
     [Documentation]
-    ...  Short documentation string.
+    ...  Test case with for-loop.
     [Tags]              RQT-SOME_RQT  SYSRQT-SOME_SYSTEM_RQT
-                        Log    ${MESSAGE}
-                        My Keyword    /tmp
+                        FOR     ${var}  IN  @{NAMES}
+                                Log     ${var}
 
 *** Keywords ***
 My Keyword
     [Documentation]     My keyword's documentation string.
     [Arguments]         ${path}
                         Directory Should Exist    ${path}
```

### Comparing `mlx.robot2rst-3.2.0/mlx/robot2rst.mako` & `mlx.robot2rst-3.2.1/mlx/robot2rst.mako`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/mlx/robot2rst.py` & `mlx.robot2rst-3.2.1/mlx/robot2rst.py`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/mlx/robot_parser.py` & `mlx.robot2rst-3.2.1/mlx/robot_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,37 +29,39 @@
         self.variables = {}
 
     def run(self):
         self.visit(self.model)
 
     def visit_VariableSection(self, node):
         for element in node.body:
-            if getattr(element, 'type') == Token.VARIABLE:
+            element_type = getattr(element, 'type', None)
+            if element_type == Token.VARIABLE:
                 name = element.get_value(Token.VARIABLE)
                 value = ' '.join(element.get_values(Token.ARGUMENT))
                 match = re.fullmatch(r"\${(.+)}", value)
                 if match:
                     value = match.group(1)
                 self.variables[name] = value
 
     def visit_TestCase(self, node):
         doc = ''
         tags = []
         for element in node.body:
-            if getattr(element, 'type') == Token.DOCUMENTATION:
+            element_type = getattr(element, 'type', None)
+            if element_type == Token.DOCUMENTATION:
                 in_docstring = False
                 previous_token = None
                 for token in element.tokens:
                     if in_docstring and token.type in (Token.ARGUMENT, Token.EOL, Token.SEPARATOR):
                         if previous_token is None or previous_token.type != Token.CONTINUATION:
                             doc += token.value
                         elif len(token.value) > 2:
                             doc += token.value[2:]  # remove two leading spaces, which are needed to separate the text
                     elif token.type == Token.CONTINUATION:
                         doc = doc.rstrip(' ')
                     elif token.type == Token.DOCUMENTATION:
                         in_docstring = True
                     previous_token = token
-            elif element.type == Token.TAGS:
+            elif element_type == Token.TAGS:
                 tags = [el.value for el in element.tokens if el.type == Token.ARGUMENT]
 
         self.tests.append(self.TestAttributes(node.name, doc, tags))
```

### Comparing `mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/PKG-INFO` & `mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.robot2rst
-Version: 3.2.0
+Version: 3.2.1
 Summary: Python script for converting a Robot Framework file to a reStructuredText (.rst) file
 Home-page: https://github.com/melexis/robot2rst
 Author: Jasper Craeghs
 Author-email: jce@melexis.com
 License: Apache License Version 2.0
 Description: .. image:: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml/badge.svg?branch=master
             :target: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml
```

### Comparing `mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/SOURCES.txt` & `mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/setup.py` & `mlx.robot2rst-3.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.0/tox.ini` & `mlx.robot2rst-3.2.1/tox.ini`

 * *Files identical despite different names*


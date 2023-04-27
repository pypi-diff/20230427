# Comparing `tmp/py-osc2-0.0.6.tar.gz` & `tmp/py-osc2-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-osc2-0.0.6.tar", last modified: Sun May  1 11:37:22 2022, max compression
+gzip compressed data, was "py-osc2-0.0.7.tar", last modified: Thu Apr 27 13:32:43 2023, max compression
```

## Comparing `py-osc2-0.0.6.tar` & `py-osc2-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 11:37:22.816757 py-osc2-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)    16890 2022-05-01 11:37:13.000000 py-osc2-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-01 11:37:13.000000 py-osc2-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-05-01 11:37:22.816757 py-osc2-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2946 2022-05-01 11:37:13.000000 py-osc2-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 11:37:22.816757 py-osc2-0.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-05-01 11:37:13.000000 py-osc2-0.0.6/examples/demo-error.osc
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-01 11:37:13.000000 py-osc2-0.0.6/examples/demo.osc
--rw-r--r--   0 runner    (1001) docker     (121)     4975 2022-05-01 11:37:13.000000 py-osc2-0.0.6/examples/swerving_side_vehicle.osc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 11:37:22.816757 py-osc2-0.0.6/osc2parser/
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-05-01 11:37:13.000000 py-osc2-0.0.6/osc2parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33722 2022-05-01 11:37:13.000000 py-osc2-0.0.6/osc2parser/openscenario2Lexer.py
--rw-r--r--   0 runner    (1001) docker     (121)    48910 2022-05-01 11:37:13.000000 py-osc2-0.0.6/osc2parser/openscenario2Listener.py
--rw-r--r--   0 runner    (1001) docker     (121)   422260 2022-05-01 11:37:13.000000 py-osc2-0.0.6/osc2parser/openscenario2Parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    28495 2022-05-01 11:37:13.000000 py-osc2-0.0.6/osc2parser/openscenario2Visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-05-01 11:37:13.000000 py-osc2-0.0.6/osc2parser/osc2parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 11:37:22.816757 py-osc2-0.0.6/py_osc2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-05-01 11:37:22.000000 py-osc2-0.0.6/py_osc2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-05-01 11:37:22.000000 py-osc2-0.0.6/py_osc2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-01 11:37:22.000000 py-osc2-0.0.6/py_osc2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-01 11:37:22.000000 py-osc2-0.0.6/py_osc2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-01 11:37:22.000000 py-osc2-0.0.6/py_osc2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-01 11:37:22.000000 py-osc2-0.0.6/py_osc2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-01 11:37:13.000000 py-osc2-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-05-01 11:37:22.816757 py-osc2-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-05-01 11:37:13.000000 py-osc2-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 11:37:22.816757 py-osc2-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-05-01 11:37:13.000000 py-osc2-0.0.6/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-05-01 11:37:13.000000 py-osc2-0.0.6/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-05-01 11:37:13.000000 py-osc2-0.0.6/tests/test_success.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 13:32:43.992493 py-osc2-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    16890 2023-04-27 13:32:38.000000 py-osc2-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-04-27 13:32:38.000000 py-osc2-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-04-27 13:32:43.992493 py-osc2-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-04-27 13:32:38.000000 py-osc2-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 13:32:43.988493 py-osc2-0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-04-27 13:32:38.000000 py-osc2-0.0.7/examples/demo-error.osc
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-27 13:32:38.000000 py-osc2-0.0.7/examples/demo.osc
+-rw-r--r--   0 runner    (1001) docker     (122)     4975 2023-04-27 13:32:38.000000 py-osc2-0.0.7/examples/swerving_side_vehicle.osc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 13:32:43.992493 py-osc2-0.0.7/osc2parser/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-04-27 13:32:38.000000 py-osc2-0.0.7/osc2parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33722 2023-04-27 13:32:38.000000 py-osc2-0.0.7/osc2parser/openscenario2Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48910 2023-04-27 13:32:38.000000 py-osc2-0.0.7/osc2parser/openscenario2Listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)   422260 2023-04-27 13:32:38.000000 py-osc2-0.0.7/osc2parser/openscenario2Parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28495 2023-04-27 13:32:38.000000 py-osc2-0.0.7/osc2parser/openscenario2Visitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-04-27 13:32:38.000000 py-osc2-0.0.7/osc2parser/osc2parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 13:32:43.992493 py-osc2-0.0.7/py_osc2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-04-27 13:32:43.000000 py-osc2-0.0.7/py_osc2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-04-27 13:32:43.000000 py-osc2-0.0.7/py_osc2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 13:32:43.000000 py-osc2-0.0.7/py_osc2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-04-27 13:32:43.000000 py-osc2-0.0.7/py_osc2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-27 13:32:43.000000 py-osc2-0.0.7/py_osc2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-27 13:32:43.000000 py-osc2-0.0.7/py_osc2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-27 13:32:38.000000 py-osc2-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-27 13:32:43.992493 py-osc2-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-04-27 13:32:38.000000 py-osc2-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 13:32:43.992493 py-osc2-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-27 13:32:38.000000 py-osc2-0.0.7/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-27 13:32:38.000000 py-osc2-0.0.7/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-04-27 13:32:38.000000 py-osc2-0.0.7/tests/test_success.py
```

### Comparing `py-osc2-0.0.6/LICENSE` & `py-osc2-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-osc2-0.0.6/PKG-INFO` & `py-osc2-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: py-osc2
-Version: 0.0.6
+Version: 0.0.7
 Summary: PMSF Python support for OpenSCENARIO 2.x
 Home-page: https://pmsf.eu/resources/osc2/py-osc2.html
 Author: PMSF IT Consulting
 Author-email: simulation@pmsf.eu
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: Bug Tracker, https://github.com/PMSFIT/py-osc2/issues
 Project-URL: Source Code, https://github.com/PMSFIT/py-osc2
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
@@ -100,15 +99,15 @@
 
 ```sh
 python setup.py antlr develop
 ```
 
 ## License
 
-(C) 2021-2022 PMSF IT Consulting Pierre R. Mai
+(C) 2021-2023 PMSF IT Consulting Pierre R. Mai
 
 [MPL 2.0](LICENSE)
 
 ## Documentation
 
 After installation of the package, an executable script, called
 `osc2parser`, is available to parse and check ASAM OpenSCENARIO 2.x
@@ -120,9 +119,7 @@
 
 This script can optionally also output a tree-view of the parsed file
 contents:
 
 ```sh
 osc2parser -t examples/demo.osc
 ```
-
-
```

### Comparing `py-osc2-0.0.6/README.md` & `py-osc2-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 ```sh
 python setup.py antlr develop
 ```
 
 ## License
 
-(C) 2021-2022 PMSF IT Consulting Pierre R. Mai
+(C) 2021-2023 PMSF IT Consulting Pierre R. Mai
 
 [MPL 2.0](LICENSE)
 
 ## Documentation
 
 After installation of the package, an executable script, called
 `osc2parser`, is available to parse and check ASAM OpenSCENARIO 2.x
```

### Comparing `py-osc2-0.0.6/examples/demo-error.osc` & `py-osc2-0.0.7/examples/demo-error.osc`

 * *Files identical despite different names*

### Comparing `py-osc2-0.0.6/examples/demo.osc` & `py-osc2-0.0.7/examples/demo.osc`

 * *Files identical despite different names*

### Comparing `py-osc2-0.0.6/examples/swerving_side_vehicle.osc` & `py-osc2-0.0.7/examples/swerving_side_vehicle.osc`

 * *Files identical despite different names*

### Comparing `py-osc2-0.0.6/osc2parser/openscenario2Lexer.py` & `py-osc2-0.0.7/osc2parser/openscenario2Lexer.py`

 * *Files identical despite different names*

### Comparing `py-osc2-0.0.6/osc2parser/openscenario2Listener.py` & `py-osc2-0.0.7/osc2parser/openscenario2Listener.py`

 * *Files identical despite different names*

### Comparing `py-osc2-0.0.6/osc2parser/openscenario2Parser.py` & `py-osc2-0.0.7/osc2parser/openscenario2Parser.py`

 * *Files identical despite different names*

### Comparing `py-osc2-0.0.6/osc2parser/openscenario2Visitor.py` & `py-osc2-0.0.7/osc2parser/openscenario2Visitor.py`

 * *Files identical despite different names*

### Comparing `py-osc2-0.0.6/osc2parser/osc2parser.py` & `py-osc2-0.0.7/osc2parser/osc2parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PMSF py-osc2 Framework osc2parser
 #
-# (C) 2021 -- 2022 PMSF IT Consulting Pierre R. Mai
+# (C) 2021 -- 2023 PMSF IT Consulting Pierre R. Mai
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import sys
 import re
@@ -40,15 +40,15 @@
     if not quiet:
         print(f"Parse of {file} completed {'without' if errors==0 else f'with {errors}'} error{'s' if abs(errors)!=1 else ''}.", file=sys.stderr)
     if print_tree:
         print_parse_tree(tree, parser.ruleNames)
     return 0 if errors==0 else 1
 
 def parse_file(file, quiet=True):
-    input_stream = FileStream(file)
+    input_stream = FileStream(file, 'utf-8')
     lexer = openscenario2Lexer(input_stream)
     stream = CommonTokenStream(lexer)
     parser = openscenario2Parser(stream)
     if quiet:
         parser.removeErrorListeners()
     tree = parser.osc_file()
     errors = parser.getNumberOfSyntaxErrors()
```

### Comparing `py-osc2-0.0.6/py_osc2.egg-info/PKG-INFO` & `py-osc2-0.0.7/py_osc2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: py-osc2
-Version: 0.0.6
+Version: 0.0.7
 Summary: PMSF Python support for OpenSCENARIO 2.x
 Home-page: https://pmsf.eu/resources/osc2/py-osc2.html
 Author: PMSF IT Consulting
 Author-email: simulation@pmsf.eu
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: Bug Tracker, https://github.com/PMSFIT/py-osc2/issues
 Project-URL: Source Code, https://github.com/PMSFIT/py-osc2
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
@@ -100,15 +99,15 @@
 
 ```sh
 python setup.py antlr develop
 ```
 
 ## License
 
-(C) 2021-2022 PMSF IT Consulting Pierre R. Mai
+(C) 2021-2023 PMSF IT Consulting Pierre R. Mai
 
 [MPL 2.0](LICENSE)
 
 ## Documentation
 
 After installation of the package, an executable script, called
 `osc2parser`, is available to parse and check ASAM OpenSCENARIO 2.x
@@ -120,9 +119,7 @@
 
 This script can optionally also output a tree-view of the parsed file
 contents:
 
 ```sh
 osc2parser -t examples/demo.osc
 ```
-
-
```

### Comparing `py-osc2-0.0.6/py_osc2.egg-info/SOURCES.txt` & `py-osc2-0.0.7/py_osc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-osc2-0.0.6/setup.py` & `py-osc2-0.0.7/setup.py`

 * *Files identical despite different names*


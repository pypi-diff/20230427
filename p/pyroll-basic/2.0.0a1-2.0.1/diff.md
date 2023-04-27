# Comparing `tmp/pyroll_basic-2.0.0a1.tar.gz` & `tmp/pyroll_basic-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroll_basic-2.0.0a1.tar", max compression
+gzip compressed data, was "pyroll_basic-2.0.1.tar", max compression
```

## Comparing `pyroll_basic-2.0.0a1.tar` & `pyroll_basic-2.0.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1526 2022-07-29 12:28:33.188685 pyroll_basic-2.0.0a1/LICENSE
--rw-r--r--   0        0        0      799 2022-07-29 13:04:49.031503 pyroll_basic-2.0.0a1/README.md
--rw-r--r--   0        0        0     1252 2022-12-21 13:27:07.212206 pyroll_basic-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      941 2022-12-21 13:15:34.159827 pyroll_basic-2.0.0a1/pyroll/basic.py
--rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 pyroll_basic-2.0.0a1/setup.py
--rw-r--r--   0        0        0     2352 1970-01-01 00:00:00.000000 pyroll_basic-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-03-29 18:39:00.371449 pyroll_basic-2.0.1/LICENSE
+-rw-r--r--   0        0        0      799 2023-03-29 18:39:00.371449 pyroll_basic-2.0.1/README.md
+-rw-r--r--   0        0        0     1208 2023-04-27 13:48:54.572821 pyroll_basic-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1125 2023-03-29 18:39:00.371449 pyroll_basic-2.0.1/pyroll/basic.py
+-rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 pyroll_basic-2.0.1/PKG-INFO
```

### Comparing `pyroll_basic-2.0.0a1/LICENSE` & `pyroll_basic-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroll_basic-2.0.0a1/README.md` & `pyroll_basic-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyroll_basic-2.0.0a1/pyproject.toml` & `pyroll_basic-2.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyroll-basic"
-version = "2.0.0a1"
+version = "2.0.1"
 description = "A meta package for installing quickly the PyRolL core and a set of basic plugins and extensions."
 authors = ["Max Weiner <max.weiner@imf.tu-freiberg.de>"]
 license = "BSD-3-Clause"
 homepage = "https://pyroll-project.github.io"
 repository = "https://github.com/pyroll-project/pyroll-core"
 documentation = "https://pyroll.readthedocs.io/en/latest"
 readme = "README.md"
@@ -15,26 +15,26 @@
     "Intended Audience :: Science/Research",
     "Intended Audience :: Manufacturing",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9, <4.0"
-pyroll-core = "^2.0.0a"
-pyroll-cli = "^2.0.0a"
-pyroll-report = "^2.0.0a"
-pyroll-export = "^2.0.0a"
-pyroll-integral-thermal = "^2.0.0a"
-pyroll-hensel-power-and-labour = "^2.0.0a"
-pyroll-wusatowski-spreading = "^2.0.0a1"
-pyroll-zouhar-contact = "^2.0.0a"
-pyroll-freiberg-flow-stress = "^2.0.0a"
-pyroll-hitchcock-roll-flattening = "^2.0.0a"
-pyroll-lendl-equivalent-method = "^2.0.0a"
+python = ">=3.9"
+pyroll-core = "^2.0"
+pyroll-cli = "^2.0"
+pyroll-report = "^2.0"
+pyroll-export = "^2.0"
+pyroll-integral-thermal = "^2.0"
+pyroll-hensel-power-and-labour = "^2.0"
+pyroll-wusatowski-spreading = "^2.0"
+pyroll-zouhar-contact = "^2.0"
+pyroll-freiberg-flow-stress = "^2.0"
+pyroll-hitchcock-roll-flattening = "^2.0"
+pyroll-lendl-equivalent-method = "^2.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
+pytest = "^7.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyroll_basic-2.0.0a1/pyroll/basic.py` & `pyroll_basic-2.0.1/pyroll/basic.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import pyroll.core as core
 from pyroll.core import (
-    BoxGroove, ConstrictedBoxGroove, SquareGroove, DiamondGroove, RoundGroove, FalseRoundGroove,
+    BoxGroove, ConstrictedBoxGroove, SquareGroove, DiamondGroove, RoundGroove, FalseRoundGroove, GothicGroove,
+    UpsetBoxGroove, UpsetOvalGroove,
     CircularOvalGroove, FlatOvalGroove, SwedishOvalGroove, ConstrictedSwedishOvalGroove, Oval3RadiiGroove,
     Oval3RadiiFlankedGroove, SplineGroove, GenericElongationGroove, FlatGroove, Transport, RollPass, Unit, Roll,
-    Profile, Rotator, PassSequence, Hook, HookHost, HookFunction
+    Profile, Rotator, PassSequence, Hook, HookHost, HookFunction,
+    DeformationUnit, DiskElementUnit, ConstrictedUpsetBoxGroove, ConstrictedCircularOvalGroove, HexagonalGroove,
+    ThreeRollPass,
 )
 
 import pyroll.freiberg_flow_stress as freiberg_flow_stress
 from pyroll.freiberg_flow_stress import FreibergFlowStressCoefficients
 
 import pyroll.integral_thermal as integral_thermal
 import pyroll.hensel_power_and_labour as hensel_power_and_labour
```

### Comparing `pyroll_basic-2.0.0a1/PKG-INFO` & `pyroll_basic-2.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pyroll-basic
-Version: 2.0.0a1
+Version: 2.0.1
 Summary: A meta package for installing quickly the PyRolL core and a set of basic plugins and extensions.
 Home-page: https://pyroll-project.github.io
 License: BSD-3-Clause
 Author: Max Weiner
 Author-email: max.weiner@imf.tu-freiberg.de
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: pyroll-cli (>=2.0.0a,<3.0.0)
-Requires-Dist: pyroll-core (>=2.0.0a,<3.0.0)
-Requires-Dist: pyroll-export (>=2.0.0a,<3.0.0)
-Requires-Dist: pyroll-freiberg-flow-stress (>=2.0.0a,<3.0.0)
-Requires-Dist: pyroll-hensel-power-and-labour (>=2.0.0a,<3.0.0)
-Requires-Dist: pyroll-hitchcock-roll-flattening (>=2.0.0a,<3.0.0)
-Requires-Dist: pyroll-integral-thermal (>=2.0.0a,<3.0.0)
-Requires-Dist: pyroll-lendl-equivalent-method (>=2.0.0a,<3.0.0)
-Requires-Dist: pyroll-report (>=2.0.0a,<3.0.0)
-Requires-Dist: pyroll-wusatowski-spreading (>=2.0.0a1,<3.0.0)
-Requires-Dist: pyroll-zouhar-contact (>=2.0.0a,<3.0.0)
+Requires-Dist: pyroll-cli (>=2.0,<3.0)
+Requires-Dist: pyroll-core (>=2.0,<3.0)
+Requires-Dist: pyroll-export (>=2.0,<3.0)
+Requires-Dist: pyroll-freiberg-flow-stress (>=2.0,<3.0)
+Requires-Dist: pyroll-hensel-power-and-labour (>=2.0,<3.0)
+Requires-Dist: pyroll-hitchcock-roll-flattening (>=2.0,<3.0)
+Requires-Dist: pyroll-integral-thermal (>=2.0,<3.0)
+Requires-Dist: pyroll-lendl-equivalent-method (>=2.0,<3.0)
+Requires-Dist: pyroll-report (>=2.0,<3.0)
+Requires-Dist: pyroll-wusatowski-spreading (>=2.0,<3.0)
+Requires-Dist: pyroll-zouhar-contact (>=2.0,<3.0)
 Project-URL: Documentation, https://pyroll.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/pyroll-project/pyroll-core
 Description-Content-Type: text/markdown
 
 # PyRolL Basic Meta Package
 
 This package does not introduce any new functionality, it works just as a meta-package to simplify the installation of
```


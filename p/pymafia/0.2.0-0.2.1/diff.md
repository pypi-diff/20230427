# Comparing `tmp/pymafia-0.2.0.tar.gz` & `tmp/pymafia-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymafia-0.2.0.tar", max compression
+gzip compressed data, was "pymafia-0.2.1.tar", max compression
```

## Comparing `pymafia-0.2.0.tar` & `pymafia-0.2.1.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0     1068 2023-04-21 15:26:57.097055 pymafia-0.2.0/LICENSE
--rw-r--r--   0        0        0     1896 2023-04-21 15:26:57.097055 pymafia-0.2.0/README.md
--rw-r--r--   0        0        0     1265 2023-04-21 15:27:38.661594 pymafia-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      384 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/__init__.py
--rw-r--r--   0        0        0      247 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/ash/__init__.py
--rw-r--r--   0        0        0     3193 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/ash/conversion.py
--rw-r--r--   0        0        0     1421 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/ash/library.py
--rw-r--r--   0        0        0     1431 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/combat.py
--rw-r--r--   0        0        0     1449 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/__init__.py
--rw-r--r--   0        0        0     2379 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/bounty.py
--rw-r--r--   0        0        0     1776 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/class_.py
--rw-r--r--   0        0        0     2389 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/coinmaster.py
--rw-r--r--   0        0        0     2445 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/effect.py
--rw-r--r--   0        0        0     1995 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/element.py
--rw-r--r--   0        0        0     6757 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/familiar.py
--rw-r--r--   0        0        0    11438 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/item.py
--rw-r--r--   0        0        0     5269 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/location.py
--rw-r--r--   0        0        0     6646 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/monster.py
--rw-r--r--   0        0        0     1914 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/path.py
--rw-r--r--   0        0        0     1359 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/phylum.py
--rw-r--r--   0        0        0     2699 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/servant.py
--rw-r--r--   0        0        0     3100 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/skill.py
--rw-r--r--   0        0        0      990 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/slot.py
--rw-r--r--   0        0        0     1059 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/stat.py
--rw-r--r--   0        0        0     2547 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/thrall.py
--rw-r--r--   0        0        0     2829 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/vykea.py
--rw-r--r--   0        0        0      545 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/__init__.py
--rw-r--r--   0        0        0      583 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/barrel_god.py
--rw-r--r--   0        0        0      890 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/boxing_daycare.py
--rw-r--r--   0        0        0     1350 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/cartography.py
--rw-r--r--   0        0        0     1030 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/cosplay_saber.py
--rw-r--r--   0        0        0     1784 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/crimbo_shrub.py
--rw-r--r--   0        0        0     1286 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/god_lobster.py
--rw-r--r--   0        0        0     1569 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/love_tunnel.py
--rw-r--r--   0        0        0     1044 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/mumming_trunk.py
--rw-r--r--   0        0        0     3518 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/pantogram.py
--rw-r--r--   0        0        0     1597 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/protonic_pack.py
--rw-r--r--   0        0        0     1139 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/snojo.py
--rw-r--r--   0        0        0     1299 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/songboom.py
--rw-r--r--   0        0        0      670 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/stomping_boots.py
--rw-r--r--   0        0        0     1408 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/witchess.py
--rw-r--r--   0        0        0      125 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/kolmafia/__init__.py
--rw-r--r--   0        0        0     1471 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/kolmafia/kolmafia.py
--rw-r--r--   0        0        0     1572 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/kolmafia/patch.py
--rw-r--r--   0        0        0     1689 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/player.py
--rw-r--r--   0        0        0     1148 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/preference.py
--rw-r--r--   0        0        0     1277 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/utils.py
--rw-r--r--   0        0        0     1350 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/wanderer.py
--rw-r--r--   0        0        0     2568 1970-01-01 00:00:00.000000 pymafia-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-27 18:27:20.603026 pymafia-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1964 2023-04-27 18:27:20.603026 pymafia-0.2.1/README.md
+-rw-r--r--   0        0        0     1283 2023-04-27 18:27:59.203652 pymafia-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      390 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/__init__.py
+-rw-r--r--   0        0        0      283 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/ash/__init__.py
+-rw-r--r--   0        0        0     3193 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/ash/conversion.py
+-rw-r--r--   0        0        0     1421 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/ash/library.py
+-rw-r--r--   0        0        0     3315 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/combat.py
+-rw-r--r--   0        0        0     1449 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/__init__.py
+-rw-r--r--   0        0        0     2442 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/bounty.py
+-rw-r--r--   0        0        0     1836 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/class_.py
+-rw-r--r--   0        0        0     2464 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/coinmaster.py
+-rw-r--r--   0        0        0     2526 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/effect.py
+-rw-r--r--   0        0        0     2653 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/element.py
+-rw-r--r--   0        0        0     6826 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/familiar.py
+-rw-r--r--   0        0        0    11495 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/item.py
+-rw-r--r--   0        0        0     5338 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/location.py
+-rw-r--r--   0        0        0     6712 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/monster.py
+-rw-r--r--   0        0        0     1976 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/path.py
+-rw-r--r--   0        0        0     2772 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/phylum.py
+-rw-r--r--   0        0        0     2765 2023-04-27 18:27:20.603026 pymafia-0.2.1/src/pymafia/datatypes/servant.py
+-rw-r--r--   0        0        0     3160 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/datatypes/skill.py
+-rw-r--r--   0        0        0     2542 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/datatypes/slot.py
+-rw-r--r--   0        0        0     1314 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/datatypes/stat.py
+-rw-r--r--   0        0        0     2610 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/datatypes/thrall.py
+-rw-r--r--   0        0        0     2889 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/datatypes/vykea.py
+-rw-r--r--   0        0        0      545 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/__init__.py
+-rw-r--r--   0        0        0      583 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/barrel_god.py
+-rw-r--r--   0        0        0      890 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/boxing_daycare.py
+-rw-r--r--   0        0        0     1350 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/cartography.py
+-rw-r--r--   0        0        0     1030 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/cosplay_saber.py
+-rw-r--r--   0        0        0     1784 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/crimbo_shrub.py
+-rw-r--r--   0        0        0     1286 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/god_lobster.py
+-rw-r--r--   0        0        0     1569 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/love_tunnel.py
+-rw-r--r--   0        0        0     1044 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/mumming_trunk.py
+-rw-r--r--   0        0        0     3518 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/pantogram.py
+-rw-r--r--   0        0        0     1597 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/protonic_pack.py
+-rw-r--r--   0        0        0     1139 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/snojo.py
+-rw-r--r--   0        0        0     1299 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/songboom.py
+-rw-r--r--   0        0        0      670 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/stomping_boots.py
+-rw-r--r--   0        0        0     1408 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/iotms/witchess.py
+-rw-r--r--   0        0        0      125 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/kolmafia/__init__.py
+-rw-r--r--   0        0        0     1759 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/kolmafia/kolmafia.py
+-rw-r--r--   0        0        0     1572 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/kolmafia/patch.py
+-rw-r--r--   0        0        0     1682 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/player.py
+-rw-r--r--   0        0        0     1148 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/preference.py
+-rw-r--r--   0        0        0     1277 2023-04-27 18:27:20.607025 pymafia-0.2.1/src/pymafia/utils.py
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 pymafia-0.2.1/PKG-INFO
```

### Comparing `pymafia-0.2.0/LICENSE` & `pymafia-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/README.md` & `pymafia-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,35 @@
-# pymafia
-
-A Python module and bridge for reflecting KoLmafia's Java environment.
+Metadata-Version: 2.1
+Name: pymafia
+Version: 0.2.1
+Summary: A Python module and bridge for reflecting KoLmafia's Java environment
+Home-page: https://github.com/MrFizzyBubbs/pymafia
+License: MIT
+Author: MrFizzyBubbs
+Author-email: MrFizzyBubbs@protonmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: JPype1 (>=1.4.1,<2.0.0)
+Requires-Dist: wrapt (>=1.15.0,<2.0.0)
+Project-URL: Repository, https://github.com/MrFizzyBubbs/pymafia
+Description-Content-Type: text/markdown
 
-## Overview
+# pymafia
 
-The aim of the `pymafia` module is to provide an easy-to-use environment for scripting [Kingdom of Loathing](https://www.kingdomofloathing.com/) in Python. It achieves this by reflecting and wrapping the community-developed [KoLmafia](https://github.com/kolmafia/kolmafia) desktop tool. While [other languages](https://loathing-associates-scripting-society.github.io/KoL-Scripting-Resources/) for scripting KoL exist, they are arguably less approachable to non-developers than Python (although the efforts of [LASS](https://github.com/Loathing-Associates-Scripting-Society) have made this less so). This project was inspired by Samuel Gaus's [frattlesnake repository](https://github.com/gausie/frattlesnake).
+*pymafia* is a Python module and bridge for reflecting KoLmafia's Java environment. It aims to provide an easy-to-use environment for scripting [Kingdom of Loathing](https://www.kingdomofloathing.com/) (KoL) in Python by reflecting and wrapping the community-developed [KoLmafia](https://github.com/kolmafia/kolmafia) desktop tool. While [other languages](https://loathing-associates-scripting-society.github.io/KoL-Scripting-Resources/) for scripting KoL exist, they are arguably less approachable to non-developers. 
 
 ## Installation
-
+*pymafia* is available at the [Python Package Index (PyPI)](https://pypi.org/project/pymafia/):
 ```
 pip install pymafia
 ```
-The `pymafia` module uses [PyJNIus](https://github.com/kivy/pyjnius) to access Java classes, so make sure a Java Development Kit (JDK) is installed on your operating system. On windows, make sure `JAVA_HOME` points to your java installation so PyJNIus can locate the `jvm.dll` file to start java. For more information see https://pyjnius.readthedocs.io/en/stable/installation.html.
+*pymafia* uses [JPype](https://github.com/kivy/pyjnius) to reflect KoLmafia's Java environment, so you will need to install a Java Development Kit (JDK) on your operating system — KoLmafia's developers recommend [Adoptium v17](https://adoptium.net/index.html). For more information on troubleshooting your Java installation, see [JPype's troubleshooting guide](https://jpype.readthedocs.io/en/latest/install.html#if-it-fails).
 
 ## Quickstart
 
 ```python
 >>> from pymafia import *
 
 >>> login("devster6")
@@ -42,7 +56,11 @@
 
 >>> boxing_daycare.have()
 True
 
 >>> witchess.fights_left()
 5
 ```
+
+## Acknowledgements
+
+This project was inspired by Samuel Gaus's [frattlesnake](https://github.com/gausie/frattlesnake) and tadpoleloop's [pymafia](https://github.com/tadpoleloop/pymafia) repositories.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymafia-0.2.0/pyproject.toml` & `pymafia-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "pymafia"
-version = "0.2.0"  # This is the standard placeholder for poetry-dynamic-versioning
+version = "0.2.1"  # This is the standard placeholder for poetry-dynamic-versioning
 description = "A Python module and bridge for reflecting KoLmafia's Java environment"
 license = "MIT"
 authors = ["MrFizzyBubbs <MrFizzyBubbs@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MrFizzyBubbs/pymafia"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 JPype1 = "^1.4.1"
 wrapt = "^1.15.0"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.15.1"
-black = "^23.3.0"
+ruff = "^0.0.262"
 isort = "^5.10.1"
+black = "^23.3.0"
+yamlfix = "^1.9.0"
 docformatter = "^1.5.0"
 mypy = "^0.971"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.2.2"
-yamlfix = "^1.9.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
 ignore = [
   "E501",  # Line too long, handled by black
```

### Comparing `pymafia-0.2.0/src/pymafia/ash/conversion.py` & `pymafia-0.2.1/src/pymafia/ash/conversion.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/ash/library.py` & `pymafia-0.2.1/src/pymafia/ash/library.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/__init__.py` & `pymafia-0.2.1/src/pymafia/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/bounty.py` & `pymafia-0.2.1/src/pymafia/datatypes/bounty.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, ClassVar
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
     from pymafia.datatypes.location import Location
     from pymafia.datatypes.monster import Monster
 
@@ -23,14 +23,16 @@
     LOW = BountyType.EASY
     HIGH = BountyType.HARD
     SPECIAL = BountyType.SPECIAL
 
 
 @dataclass(frozen=True, order=True)
 class Bounty:
+    NONE: ClassVar[Bounty]
+
     name: str = km.DataTypes.BOUNTY_INIT.contentString
 
     def __init__(self, key: str | None = None):
         if (
             isinstance(key, str) and key.casefold() == self.name.casefold()
         ) or key is None:
             return
@@ -85,7 +87,10 @@
         return Monster(km.BountyDatabase.getMonster(self.name))
 
     @property
     def location(self) -> Location:
         from pymafia.datatypes.location import Location
 
         return Location(km.BountyDatabase.getLocation(self.name))
+
+
+Bounty.NONE = Bounty()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/class_.py` & `pymafia-0.2.1/src/pymafia/datatypes/class_.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
     from pymafia.datatypes.stat import Stat
 
 
 @dataclass(frozen=True, order=True)
 class Class:
+    NONE: ClassVar[Class]
+
     ascension_class: Any = field(default=km.DataTypes.CLASS_INIT.content, compare=False)
     id: int = km.DataTypes.CLASS_INIT.contentLong
     name: str = km.DataTypes.CLASS_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
         if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
             self.id,
@@ -51,7 +53,10 @@
         from pymafia.datatypes.stat import Stat
 
         if self.ascension_class is None:
             return Stat()
         prime_index = self.ascension_class.getPrimeStatIndex()
         name = km.AdventureResult.STAT_NAMES[prime_index]
         return Stat(name)
+
+
+Class.NONE = Class()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/coinmaster.py` & `pymafia-0.2.1/src/pymafia/datatypes/coinmaster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
     from pymafia.datatypes.item import Item
 
 
 @dataclass(frozen=True, order=True)
 class Coinmaster:
+    NONE: ClassVar[Coinmaster]
+
     coinmaster: Any = field(default=km.DataTypes.COINMASTER_INIT.content, compare=False)
     name: str = km.DataTypes.COINMASTER_INIT.contentString
 
     def __init__(self, key: str | None = None):
         if (
             isinstance(key, str) and key.casefold() == self.name.casefold()
         ) or key is None:
@@ -75,7 +77,10 @@
         return (
             self.coinmaster is not None and self.coinmaster.getBuyAction() is not None
         )
 
     @property
     def nickname(self) -> str:
         return self.coinmaster.getNickname() if self.coinmaster is not None else ""
+
+
+Coinmaster.NONE = Coinmaster()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/effect.py` & `pymafia-0.2.1/src/pymafia/datatypes/effect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import IntEnum
+from typing import ClassVar
 
 from pymafia.kolmafia import km
 
 
 class EffectQuality(IntEnum):
     NONE = -1
     GOOD = 0
     NEUTRAL = 1
     BAD = 2
 
 
 @dataclass(frozen=True, order=True)
 class Effect:
+    NONE: ClassVar[Effect]
+
     id: int = km.DataTypes.EFFECT_INIT.contentLong
     name: str = km.DataTypes.EFFECT_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
         if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
             self.id,
             None,
@@ -82,7 +85,10 @@
     @property
     def candy_tier(self) -> int:
         return km.CandyDatabase.getEffectTier(self.id)
 
     @property
     def song(self) -> bool:
         return km.EffectDatabase.isSong(self.id)
+
+
+Effect.NONE = Effect()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/element.py` & `pymafia-0.2.1/src/pymafia/datatypes/skill.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,121 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
-from typing import Any
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, ClassVar
 
 from pymafia.kolmafia import km
 
+if TYPE_CHECKING:
+    from pymafia.datatypes.class_ import Class
+
 
 @dataclass(frozen=True, order=True)
-class Element:
-    element: Any = field(default=km.DataTypes.ELEMENT_INIT.content, compare=False)
-    name: str = km.DataTypes.ELEMENT_INIT.contentString
-
-    def __init__(self, key: str | None = None):
-        if (
-            isinstance(key, str) and key.casefold() == self.name.casefold()
-        ) or key is None:
+class Skill:
+    NONE: ClassVar[Skill]
+
+    id: int = km.DataTypes.SKILL_INIT.contentLong
+    name: str = km.DataTypes.SKILL_INIT.contentString
+
+    def __init__(self, key: int | str | None = None):
+        if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
+            self.id,
+            None,
+        ):
             return
 
-        element = km.MonsterDatabase.stringToElement(key)
-        if element == km.MonsterDatabase.Element.NONE:
+        id = km.SkillDatabase.getSkillId(key) if isinstance(key, str) else key
+        name = km.SkillDatabase.getSkillName(id)
+        if name is None:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        object.__setattr__(self, "element", element)
-        object.__setattr__(self, "name", element.toString())
+        object.__setattr__(self, "id", id)
+        object.__setattr__(self, "name", name)
 
     def __str__(self) -> str:
-        return self.name
+        ids = km.SkillDatabase.getSkillIds(self.name, False)
+        return f"[{self.id}]{self.name}" if len(ids) > 1 else self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
-    def all(cls) -> list[Element]:
+    def all(cls) -> list[Skill]:
         from pymafia.ash import from_java
 
-        values = km.DataTypes.ELEMENT_TYPE.allValues()
-        return from_java(values)
+        values = km.DataTypes.SKILL_TYPE.allValues()
+        return sorted(from_java(values))
+
+    @property
+    def type(self) -> str:
+        return km.SkillDatabase.getSkillTypeName(self.id)
+
+    @property
+    def level(self) -> int:
+        return km.SkillDatabase.getSkillLevel(self.id)
 
     @property
     def image(self) -> str:
-        # No image for Slime or Supercold in Manuel
-        if self.element in [
-            km.MonsterDatabase.Element.NONE,
-            km.MonsterDatabase.Element.SLIME,
-            km.MonsterDatabase.Element.SUPERCOLD,
-        ]:
-            return "circle.gif"
-        if self.element == km.MonsterDatabase.Element.COLD:
-            return "snowflake.gif"
-        if self.element == km.MonsterDatabase.Element.HOT:
-            return "fire.gif"
-        if self.element == km.MonsterDatabase.Element.SLEAZE:
-            return "wink.gif"
-        if self.element == km.MonsterDatabase.Element.SPOOKY:
-            return "skull.gif"
-        if self.element == km.MonsterDatabase.Element.STENCH:
-            return "stench.gif"
-        return ""
+        return km.SkillDatabase.getSkillImage(self.id)
+
+    @property
+    def traincost(self) -> int:
+        return km.SkillDatabase.getSkillPurchaseCost(self.id)
+
+    @property
+    def class_(self) -> Class:
+        from pymafia.datatypes.class_ import Class
+
+        try:
+            return Class(km.SkillDatabase.getSkillCategory(self.id).name)
+        except ValueError:
+            return Class()
+
+    @property
+    def libram(self) -> bool:
+        return km.SkillDatabase.isLibramSkill(self.id)
+
+    @property
+    def passive(self) -> bool:
+        return km.SkillDatabase.isPassive(self.id)
+
+    @property
+    def buff(self) -> bool:
+        return km.SkillDatabase.isBuff(self.id)
+
+    @property
+    def combat(self) -> bool:
+        return km.SkillDatabase.isCombat(self.id)
+
+    @property
+    def song(self) -> bool:
+        return km.SkillDatabase.isSong(self.id)
+
+    @property
+    def expression(self) -> bool:
+        return km.SkillDatabase.isExpression(self.id)
+
+    @property
+    def walk(self) -> bool:
+        return km.SkillDatabase.isWalk(self.id)
+
+    @property
+    def summon(self) -> bool:
+        return km.SkillDatabase.isSummon(self.id)
+
+    @property
+    def permable(self) -> bool:
+        return km.SkillDatabase.isPermable(self.id)
+
+    @property
+    def dailylimit(self) -> int:
+        return km.SkillDatabase.getMaxCasts(self.id)
+
+    @property
+    def timescast(self) -> int:
+        return km.SkillDatabase.getCasts(self.id)
+
+
+Skill.NONE = Skill()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/familiar.py` & `pymafia-0.2.1/src/pymafia/datatypes/familiar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, ClassVar
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
     from pymafia.datatypes.item import Item
 
 
 @dataclass(frozen=True, order=True)
 class Familiar:
+    NONE: ClassVar[Familiar]
+
     id: int = km.DataTypes.FAMILIAR_INIT.contentLong
     name: str = km.DataTypes.FAMILIAR_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
         if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
             self.id,
             None,
@@ -221,7 +223,10 @@
         data = km.FamiliarDatabase.getPokeDataById(self.id)
         return data.getMove3() if data is not None else ""
 
     @property
     def poke_attribute(self) -> str:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
         return data.getAttribute() if data is not None else ""
+
+
+Familiar.NONE = Familiar()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/item.py` & `pymafia-0.2.1/src/pymafia/datatypes/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, ClassVar
 
 from jpype import JClass
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
     from pymafia.datatypes.coinmaster import Coinmaster
@@ -20,14 +20,16 @@
     UNSPADED = km.CandyDatabase.CandyType.UNSPADED
     SIMPLE = km.CandyDatabase.CandyType.SIMPLE
     COMPLEX = km.CandyDatabase.CandyType.COMPLEX
 
 
 @dataclass(frozen=True, order=True)
 class Item:
+    NONE: ClassVar[Item]
+
     id: int = km.DataTypes.ITEM_INIT.contentLong
     name: str = km.DataTypes.ITEM_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
         if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
             self.id,
             None,
@@ -294,7 +296,10 @@
         """Return the noob Skill granted by absorbing this Item."""
         from pymafia.datatypes.skill import Skill
 
         try:
             return Skill(km.ItemDatabase.getNoobSkillId(self.id))
         except ValueError:
             return Skill()
+
+
+Item.NONE = Item()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/location.py` & `pymafia-0.2.1/src/pymafia/datatypes/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from jpype import JClass
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
     from pymafia.datatypes.bounty import Bounty
 
 Integer = JClass("java.lang.Integer")
 
 
 @dataclass(frozen=True, order=True)
 class Location:
+    NONE: ClassVar[Location]
+
     kol_adventure: Any = field(
         default=km.DataTypes.LOCATION_INIT.content, compare=False
     )
     id: int = -1  # LOCATION_INIT does not specify an id
     name: str = km.DataTypes.LOCATION_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
@@ -171,7 +173,10 @@
         return self.kol_adventure is not None and self.kol_adventure.hasWanderers()
 
     @property
     def fire_level(self) -> int:
         if self.kol_adventure is None or not km.KoLCharacter.inFirecore():
             return 0
         return km.WildfireCampRequest.getFireLevel(self.kol_adventure)
+
+
+Location.NONE = Location()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/monster.py` & `pymafia-0.2.1/src/pymafia/datatypes/monster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from jpype import JClass
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
     from pymafia.datatypes.effect import Effect
@@ -14,14 +14,16 @@
 
 
 Integer = JClass("java.lang.Integer")
 
 
 @dataclass(frozen=True, order=True)
 class Monster:
+    NONE: ClassVar[Monster]
+
     monster: Any = field(default=km.DataTypes.MONSTER_INIT.content, compare=False)
     id: int = km.DataTypes.MONSTER_INIT.contentLong
     name: str = km.DataTypes.MONSTER_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
         if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
             self.id,
@@ -211,7 +213,10 @@
     @property
     def wiki_name(self) -> str:
         return self.monster.getWikiName() if self.monster is not None else ""
 
     @property
     def attributes(self) -> str:
         return self.monster.getAttributes() if self.monster is not None else ""
+
+
+Monster.NONE = Monster()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/path.py` & `pymafia-0.2.1/src/pymafia/datatypes/path.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Any
+from typing import Any, ClassVar
 
 from pymafia.kolmafia import km
 
 
 @dataclass(frozen=True, order=True)
 class Path:
+    NONE: ClassVar[Path]
+
     ascension_path: Any = field(default=km.DataTypes.PATH_INIT.content, compare=False)
     id: int = km.DataTypes.PATH_INIT.contentLong
     name: str = km.DataTypes.PATH_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
         if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
             self.id,
@@ -58,7 +60,10 @@
     @property
     def points(self) -> int:
         return self.ascension_path.getPoints()
 
     @property
     def familiars(self) -> bool:
         return self.ascension_path.canUseFamiliars()
+
+
+Path.NONE = Path()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/servant.py` & `pymafia-0.2.1/src/pymafia/datatypes/servant.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Any
+from typing import Any, ClassVar
 
 from pymafia.kolmafia import km
 
 
 @dataclass(frozen=True, order=True)
 class Servant:
+    NONE: ClassVar[Servant]
+
     data: Any = field(default=km.DataTypes.SERVANT_INIT.content, compare=False)
     id: int = km.DataTypes.SERVANT_INIT.contentLong
     name: str = km.DataTypes.SERVANT_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
         if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
             self.id,
@@ -90,7 +92,10 @@
     @property
     def level21_ability(self) -> str:
         return (
             km.EdServantData.dataToLevel21Ability(self.data)
             if self.data is not None
             else ""
         )
+
+
+Servant.NONE = Servant()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/slot.py` & `pymafia-0.2.1/src/pymafia/datatypes/stat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
+from typing import ClassVar
 
 from pymafia.kolmafia import km
 
 
 @dataclass(frozen=True, order=True)
-class Slot:
-    name: str = km.DataTypes.SLOT_INIT.contentString
+class Stat:
+    NONE: ClassVar[Stat]
+    MUSCLE: ClassVar[Stat]
+    MYSTICALITY: ClassVar[Stat]
+    MOXIE: ClassVar[Stat]
+
+    name: str = km.DataTypes.STAT_INIT.contentString
 
     def __init__(self, key: str | None = None):
         if (
             isinstance(key, str) and key.casefold() == self.name.casefold()
         ) or key is None:
             return
 
-        slot = km.EquipmentRequest.slotNumber(key)
-        if slot == km.Slot.NONE:
-            raise ValueError(f"{type(self).__name__} {key!r} not found")
+        for stat in km.DataTypes.STAT_VALUES:
+            name = stat.toString()
+            if name.casefold() == key.casefold():
+                object.__setattr__(self, "name", name)
+                return
 
-        object.__setattr__(self, "name", slot.name)
+        raise ValueError(f"{type(self).__name__} {key!r} not found")
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
-    def all(cls) -> list[Slot]:
+    def all(cls) -> list[Stat]:
         from pymafia.ash import from_java
 
-        values = km.DataTypes.SLOT_TYPE.allValues()
+        values = km.DataTypes.STAT_TYPE.allValues()
         return from_java(values)
+
+
+Stat.NONE = Stat()
+Stat.MUSCLE = Stat("Muscle")
+Stat.MYSTICALITY = Stat("Mysticality")
+Stat.MOXIE = Stat("Moxie")
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/thrall.py` & `pymafia-0.2.1/src/pymafia/datatypes/thrall.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
     from pymafia.datatypes.skill import Skill
 
 
 @dataclass(frozen=True, order=True)
 class Thrall:
+    NONE: ClassVar[Thrall]
+
     data: Any = field(default=km.DataTypes.THRALL_INIT.content, compare=False)
     id: int = km.DataTypes.THRALL_INIT.contentLong
     type: str = km.DataTypes.THRALL_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
         if (isinstance(key, str) and key.casefold() == self.type.casefold()) or key in (
             self.id,
@@ -85,7 +87,10 @@
             if self.data is not None
             else None
         )
 
     @property
     def current_modifiers(self) -> str:
         return self.thrall.getCurrentModifiers() if self.thrall else ""
+
+
+Thrall.NONE = Thrall()
```

### Comparing `pymafia-0.2.0/src/pymafia/datatypes/vykea.py` & `pymafia-0.2.1/src/pymafia/datatypes/vykea.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
     from pymafia.datatypes.element import Element
 
 
@@ -25,14 +25,16 @@
     FRENZY = km.VYKEACompanionData.FRENZY_RUNE
     BLOOD = km.VYKEACompanionData.BLOOD_RUNE
     LIGHTNING = km.VYKEACompanionData.LIGHTNING_RUNE
 
 
 @dataclass(frozen=True, order=True)
 class Vykea:
+    NONE: ClassVar[Vykea]
+
     companion: Any = field(default=km.VYKEACompanionData.NO_COMPANION, compare=False)
     type: VykeaCompanionType = VykeaCompanionType(companion.default.getType())
     rune: VykeaRune = VykeaRune(companion.default.getRune())
     level: int = companion.default.getLevel()
 
     def __init__(self, key: str | None = None):
         if (
@@ -81,7 +83,10 @@
         return self.companion.getModifiers()
 
     @property
     def attack_element(self) -> Element:
         from pymafia.datatypes.element import Element
 
         return Element(self.companion.getAttackElement().toString())
+
+
+Vykea.NONE = Vykea()
```

### Comparing `pymafia-0.2.0/src/pymafia/iotms/__init__.py` & `pymafia-0.2.1/src/pymafia/iotms/__init__.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/barrel_god.py` & `pymafia-0.2.1/src/pymafia/iotms/barrel_god.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/boxing_daycare.py` & `pymafia-0.2.1/src/pymafia/iotms/boxing_daycare.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/cartography.py` & `pymafia-0.2.1/src/pymafia/iotms/cartography.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/cosplay_saber.py` & `pymafia-0.2.1/src/pymafia/iotms/cosplay_saber.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/crimbo_shrub.py` & `pymafia-0.2.1/src/pymafia/iotms/crimbo_shrub.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/god_lobster.py` & `pymafia-0.2.1/src/pymafia/iotms/god_lobster.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/love_tunnel.py` & `pymafia-0.2.1/src/pymafia/iotms/love_tunnel.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/mumming_trunk.py` & `pymafia-0.2.1/src/pymafia/iotms/mumming_trunk.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/pantogram.py` & `pymafia-0.2.1/src/pymafia/iotms/pantogram.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/protonic_pack.py` & `pymafia-0.2.1/src/pymafia/iotms/protonic_pack.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/snojo.py` & `pymafia-0.2.1/src/pymafia/iotms/snojo.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/songboom.py` & `pymafia-0.2.1/src/pymafia/iotms/songboom.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/stomping_boots.py` & `pymafia-0.2.1/src/pymafia/iotms/stomping_boots.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/iotms/witchess.py` & `pymafia-0.2.1/src/pymafia/iotms/witchess.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/kolmafia/patch.py` & `pymafia-0.2.1/src/pymafia/kolmafia/patch.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/player.py` & `pymafia-0.2.1/src/pymafia/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,14 @@
     match = re.search("<!-- MONSTERID: (\\d+) -->", page)
     if not match:
         raise RuntimeError("unable to identify monster")
     return int(match.group(1)) == monster.id
 
 
 def can_visit_url() -> bool:
-    """Return whether the player can safely visit an in-game url."""
+    """Return whether the player can visit an in-game url."""
     return not (
         ash.current_round() > 0
         or ash.in_multi_fight()
         or ash.fight_follows_choice()
         or ash.handling_choice()
     )
```

### Comparing `pymafia-0.2.0/src/pymafia/preference.py` & `pymafia-0.2.1/src/pymafia/preference.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/src/pymafia/utils.py` & `pymafia-0.2.1/src/pymafia/utils.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.0/PKG-INFO` & `pymafia-0.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,17 @@
-Metadata-Version: 2.1
-Name: pymafia
-Version: 0.2.0
-Summary: A Python module and bridge for reflecting KoLmafia's Java environment
-Home-page: https://github.com/MrFizzyBubbs/pymafia
-License: MIT
-Author: MrFizzyBubbs
-Author-email: MrFizzyBubbs@protonmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: JPype1 (>=1.4.1,<2.0.0)
-Requires-Dist: wrapt (>=1.15.0,<2.0.0)
-Project-URL: Repository, https://github.com/MrFizzyBubbs/pymafia
-Description-Content-Type: text/markdown
-
 # pymafia
 
-A Python module and bridge for reflecting KoLmafia's Java environment.
-
-## Overview
-
-The aim of the `pymafia` module is to provide an easy-to-use environment for scripting [Kingdom of Loathing](https://www.kingdomofloathing.com/) in Python. It achieves this by reflecting and wrapping the community-developed [KoLmafia](https://github.com/kolmafia/kolmafia) desktop tool. While [other languages](https://loathing-associates-scripting-society.github.io/KoL-Scripting-Resources/) for scripting KoL exist, they are arguably less approachable to non-developers than Python (although the efforts of [LASS](https://github.com/Loathing-Associates-Scripting-Society) have made this less so). This project was inspired by Samuel Gaus's [frattlesnake repository](https://github.com/gausie/frattlesnake).
+*pymafia* is a Python module and bridge for reflecting KoLmafia's Java environment. It aims to provide an easy-to-use environment for scripting [Kingdom of Loathing](https://www.kingdomofloathing.com/) (KoL) in Python by reflecting and wrapping the community-developed [KoLmafia](https://github.com/kolmafia/kolmafia) desktop tool. While [other languages](https://loathing-associates-scripting-society.github.io/KoL-Scripting-Resources/) for scripting KoL exist, they are arguably less approachable to non-developers. 
 
 ## Installation
-
+*pymafia* is available at the [Python Package Index (PyPI)](https://pypi.org/project/pymafia/):
 ```
 pip install pymafia
 ```
-The `pymafia` module uses [PyJNIus](https://github.com/kivy/pyjnius) to access Java classes, so make sure a Java Development Kit (JDK) is installed on your operating system. On windows, make sure `JAVA_HOME` points to your java installation so PyJNIus can locate the `jvm.dll` file to start java. For more information see https://pyjnius.readthedocs.io/en/stable/installation.html.
+*pymafia* uses [JPype](https://github.com/kivy/pyjnius) to reflect KoLmafia's Java environment, so you will need to install a Java Development Kit (JDK) on your operating system — KoLmafia's developers recommend [Adoptium v17](https://adoptium.net/index.html). For more information on troubleshooting your Java installation, see [JPype's troubleshooting guide](https://jpype.readthedocs.io/en/latest/install.html#if-it-fails).
 
 ## Quickstart
 
 ```python
 >>> from pymafia import *
 
 >>> login("devster6")
@@ -61,7 +39,10 @@
 >>> boxing_daycare.have()
 True
 
 >>> witchess.fights_left()
 5
 ```
 
+## Acknowledgements
+
+This project was inspired by Samuel Gaus's [frattlesnake](https://github.com/gausie/frattlesnake) and tadpoleloop's [pymafia](https://github.com/tadpoleloop/pymafia) repositories.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


# Comparing `tmp/tcod-ecs-1.1.0.tar.gz` & `tmp/tcod-ecs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod-ecs-1.1.0.tar", last modified: Sat Apr 22 05:31:06 2023, max compression
+gzip compressed data, was "tcod-ecs-1.2.0.tar", last modified: Wed Apr 26 22:04:51 2023, max compression
```

## Comparing `tcod-ecs-1.1.0.tar` & `tcod-ecs-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      110 2022-12-09 23:27:48.971884 tcod-ecs-1.1.0/.flake8
--rw-r--r--   0        0        0     2450 2022-12-09 22:01:20.751676 tcod-ecs-1.1.0/.gitattributes
--rw-r--r--   0        0        0      188 2022-12-07 02:28:46.295094 tcod-ecs-1.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1706 2023-04-09 03:23:14.272745 tcod-ecs-1.1.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     4409 2023-03-27 00:31:15.054038 tcod-ecs-1.1.0/.gitignore
--rw-r--r--   0        0        0      772 2023-03-25 01:31:11.142017 tcod-ecs-1.1.0/.readthedocs.yml
--rw-r--r--   0        0        0     1325 2023-03-23 23:46:53.826542 tcod-ecs-1.1.0/.vscode/launch.json
--rw-r--r--   0        0        0     1493 2023-04-12 00:56:27.890449 tcod-ecs-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0     1238 2023-03-23 23:46:52.209465 tcod-ecs-1.1.0/.vscode/tasks.json
--rw-r--r--   0        0        0      550 2023-04-22 05:22:42.237610 tcod-ecs-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1100 2023-03-26 20:09:04.799655 tcod-ecs-1.1.0/LICENSE
--rw-r--r--   0        0        0     8642 2023-04-12 01:06:47.372874 tcod-ecs-1.1.0/README.md
--rw-r--r--   0        0        0      581 2023-04-12 01:13:36.306949 tcod-ecs-1.1.0/conftest.py
--rw-r--r--   0        0        0      634 2022-12-10 22:58:25.072843 tcod-ecs-1.1.0/docs/Makefile
--rw-r--r--   0        0        0      115 2023-03-24 00:06:33.545046 tcod-ecs-1.1.0/docs/api.rst
--rw-r--r--   0        0        0     2072 2023-03-24 00:06:35.156705 tcod-ecs-1.1.0/docs/conf.py
--rw-r--r--   0        0        0       32 2022-12-10 23:30:30.594162 tcod-ecs-1.1.0/docs/head.md
--rw-r--r--   0        0        0      255 2023-01-06 20:05:00.073778 tcod-ecs-1.1.0/docs/index.rst
--rwxr-xr-x   0        0        0      800 2022-12-10 22:58:25.073843 tcod-ecs-1.1.0/docs/make.bat
--rw-r--r--   0        0        0       46 2023-03-25 01:28:10.449866 tcod-ecs-1.1.0/docs/requirements.txt
--rw-r--r--   0        0        0     3569 2023-04-12 08:17:44.588593 tcod-ecs-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    31850 2023-04-22 05:23:44.626693 tcod-ecs-1.1.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0     7530 2023-04-22 01:26:15.421648 tcod-ecs-1.1.0/tcod/ecs/test_ecs.py
--rw-r--r--   0        0        0     9609 1970-01-01 00:00:00.000000 tcod-ecs-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      110 2022-12-09 23:27:48.971884 tcod-ecs-1.2.0/.flake8
+-rw-r--r--   0        0        0     2450 2022-12-09 22:01:20.751676 tcod-ecs-1.2.0/.gitattributes
+-rw-r--r--   0        0        0      188 2022-12-07 02:28:46.295094 tcod-ecs-1.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1706 2023-04-09 03:23:14.272745 tcod-ecs-1.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     4409 2023-03-27 00:31:15.054038 tcod-ecs-1.2.0/.gitignore
+-rw-r--r--   0        0        0      772 2023-03-25 01:31:11.142017 tcod-ecs-1.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1325 2023-03-23 23:46:53.826542 tcod-ecs-1.2.0/.vscode/launch.json
+-rw-r--r--   0        0        0     1516 2023-04-26 21:46:29.875591 tcod-ecs-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1238 2023-03-23 23:46:52.209465 tcod-ecs-1.2.0/.vscode/tasks.json
+-rw-r--r--   0        0        0      777 2023-04-26 22:04:07.822052 tcod-ecs-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1100 2023-03-26 20:09:04.799655 tcod-ecs-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8642 2023-04-12 01:06:47.372874 tcod-ecs-1.2.0/README.md
+-rw-r--r--   0        0        0      581 2023-04-12 01:13:36.306949 tcod-ecs-1.2.0/conftest.py
+-rw-r--r--   0        0        0      634 2022-12-10 22:58:25.072843 tcod-ecs-1.2.0/docs/Makefile
+-rw-r--r--   0        0        0      115 2023-03-24 00:06:33.545046 tcod-ecs-1.2.0/docs/api.rst
+-rw-r--r--   0        0        0     2072 2023-03-24 00:06:35.156705 tcod-ecs-1.2.0/docs/conf.py
+-rw-r--r--   0        0        0       32 2022-12-10 23:30:30.594162 tcod-ecs-1.2.0/docs/head.md
+-rw-r--r--   0        0        0      255 2023-01-06 20:05:00.073778 tcod-ecs-1.2.0/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2022-12-10 22:58:25.073843 tcod-ecs-1.2.0/docs/make.bat
+-rw-r--r--   0        0        0       46 2023-03-25 01:28:10.449866 tcod-ecs-1.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0     3569 2023-04-12 08:17:44.588593 tcod-ecs-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    32536 2023-04-26 22:04:17.748971 tcod-ecs-1.2.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:09:12.939518 tcod-ecs-1.2.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0     7530 2023-04-22 05:35:25.347051 tcod-ecs-1.2.0/tcod/ecs/test_ecs.py
+-rw-r--r--   0        0        0     9609 1970-01-01 00:00:00.000000 tcod-ecs-1.2.0/PKG-INFO
```

### Comparing `tcod-ecs-1.1.0/.gitattributes` & `tcod-ecs-1.2.0/.gitattributes`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/.github/workflows/python-package.yml` & `tcod-ecs-1.2.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/.gitignore` & `tcod-ecs-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/.readthedocs.yml` & `tcod-ecs-1.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/.vscode/launch.json` & `tcod-ecs-1.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/.vscode/settings.json` & `tcod-ecs-1.2.0/.vscode/settings.json`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         "PAGEDOWN",
         "PAGEUP",
         "pytest",
         "quickstart",
         "RMASK",
         "rtype",
         "scancode",
+        "setdefault",
         "tcod",
         "toctree",
         "Traceback",
         "typehints",
         "undoc",
         "WASD",
         "WAXD",
```

### Comparing `tcod-ecs-1.1.0/.vscode/tasks.json` & `tcod-ecs-1.2.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/LICENSE` & `tcod-ecs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/README.md` & `tcod-ecs-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/conftest.py` & `tcod-ecs-1.2.0/conftest.py`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/docs/Makefile` & `tcod-ecs-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/docs/conf.py` & `tcod-ecs-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/docs/make.bat` & `tcod-ecs-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/pyproject.toml` & `tcod-ecs-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/tcod/ecs/__init__.py` & `tcod-ecs-1.2.0/tcod/ecs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """A type-hinted Entity Component System based on Python dictionaries and sets."""
 from __future__ import annotations
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 import sys
 from functools import partial
 from typing import (
+    TYPE_CHECKING,
     AbstractSet,
     Any,
     DefaultDict,
     Final,
     Generic,
     Iterable,
     Iterator,
@@ -52,15 +53,15 @@
 
         >>> import tcod.ecs
         >>> world = tcod.ecs.World()  # Create a new world.
         >>> entity = world.new_entity(name="entity")  # Create a new entity, name is optional.
         >>> other_entity = world.new_entity(name="other_entity")
     """  # Changes here should be reflected in conftest.py.
 
-    __slots__ = ("world",)
+    __slots__ = ("world", "__weakref__")
 
     def __init__(self, world: World) -> None:
         """Initialize a new unique entity."""
         self.world: Final = world
         """The :any:`World` this entity belongs to."""
 
     @property
@@ -240,14 +241,30 @@
         return len(self.entity.world._components_by_entity.get(self.entity, ()))
 
     def update_values(self, values: Iterable[object]) -> None:
         """Add or overwrite multiple components inplace, deriving the keys from the values."""
         for value in values:
             self.set(value)
 
+    if TYPE_CHECKING:  # Type-hinted overrides
+
+        @overload
+        def get(self, __key: _ComponentKey[T]) -> T | None:
+            ...
+
+        @overload
+        def get(self, __key: _ComponentKey[T], __default: T) -> T:
+            ...
+
+        def get(self, __key: _ComponentKey[T], __default: T | None = None) -> T | None:
+            """Return a component, returns None or a default value when the component is missing."""
+
+        def setdefault(self, __key: _ComponentKey[T], __default: T) -> T:  # type: ignore[override]
+            """Assign a default value if a component is missing, then returns the current value."""
+
 
 class EntityTags(MutableSet[Any]):
     """A proxy attribute to access an entities tags like a set.
 
     See :any:`Entity.tags`.
     """
```

### Comparing `tcod-ecs-1.1.0/tcod/ecs/test_ecs.py` & `tcod-ecs-1.2.0/tcod/ecs/test_ecs.py`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.1.0/PKG-INFO` & `tcod-ecs-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 1.1.0
+Version: 1.2.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


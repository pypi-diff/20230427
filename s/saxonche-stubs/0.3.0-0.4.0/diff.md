# Comparing `tmp/saxonche_stubs-0.3.0.tar.gz` & `tmp/saxonche_stubs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saxonche_stubs-0.3.0.tar", max compression
+gzip compressed data, was "saxonche_stubs-0.4.0.tar", max compression
```

## Comparing `saxonche_stubs-0.3.0.tar` & `saxonche_stubs-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      490 2023-04-21 15:06:15.152853 saxonche_stubs-0.3.0/README.md
--rw-r--r--   0        0        0     1572 2023-04-21 15:30:13.967154 saxonche_stubs-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7464 2023-04-21 15:27:32.263455 saxonche_stubs-0.3.0/saxonche-stubs/__init__.pyi
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 saxonche_stubs-0.3.0/setup.py
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 saxonche_stubs-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      490 2023-04-21 15:06:15.152853 saxonche_stubs-0.4.0/README.md
+-rw-r--r--   0        0        0     1572 2023-04-27 14:19:13.462861 saxonche_stubs-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9838 2023-04-27 14:19:07.274991 saxonche_stubs-0.4.0/saxonche-stubs/__init__.pyi
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 saxonche_stubs-0.4.0/setup.py
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 saxonche_stubs-0.4.0/PKG-INFO
```

### Comparing `saxonche_stubs-0.3.0/pyproject.toml` & `saxonche_stubs-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saxonche-stubs"
-version = "0.3.0"
+version = "0.4.0"
 description = "Type stubs for saxonche"
 authors = ["Bpolitycki <bastian.politycki@unisg.ch>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "saxonche-stubs"}]
 
 classifiers = [
```

### Comparing `saxonche_stubs-0.3.0/saxonche-stubs/__init__.pyi` & `saxonche_stubs-0.4.0/saxonche-stubs/__init__.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -209,14 +209,19 @@
         """Property which returns the string value.
 
         Returns:
             str: The string value of the atomic value
         """
         ...
 
+class PyXdmFunctionItem(PyXdmItem):
+    def __init__(self) -> None:
+        """Represents a function item in the XDM data model."""
+        ...
+
 class PyXdmAtomicValue(PyXdmItem):
     def __init__(self) -> None:
         """Reprensts an atomic value in the XDM data model. Atomic values are either
         built-in atomic values (such as xs:integer or xs:date) or user-defined atomic
         values."""
         ...
     @property
@@ -232,12 +237,87 @@
         """Property which returns the integer value.
 
         Returns:
             int: The integer value of the atomic value
         """
         ...
 
-class PyXdmMap(PyXdmItem):
-    def __init__(self) -> None: ...
+class PyXdmMap(PyXdmFunctionItem):
+    def __init__(self) -> None:
+        """The class PyXdmMap represents a map in the XDM data model. A map is a list of zero or more entries,
+        each consisting of a key-value pair. The map itself is an XDM item and is immutable.
+        """
+        ...
+    @property
+    def map_size(self) -> int:
+        """Property which returns the number of entries in the map.
+
+        Returns:
+            int: The number of entries in the map
+        """
+        ...
+    @property
+    def string_value(self) -> str:
+        """Property which returns the string value of the map.
+
+        Returns:
+            str: The string value of the map
+        """
+        ...
+    def contains_key(self, key: PyXdmAtomicValue) -> bool:
+        """Check whether the map contains a given key.
+
+        Args:
+            key (PyXdmAtomicValue): The key
+
+        Returns:
+            bool: True if the map contains the key, False otherwise
+        """
+        ...
+    def get(self, key: str | PyXdmAtomicValue | int | float) -> PyXdmValue | None:
+        """Get the value associated with a given key.
+
+        Args:
+            key (str | PyXdmAtomicValue | int | float): The key
+
+        Returns:
+            PyXdmValue | None: The value associated with the key or None if the key is not present in the map
+        """
+        ...
+    def keys(self) -> list[PyXdmAtomicValue]:
+        """Get the keys of the map.
+
+        Returns:
+            list[PyXdmAtomicValue]: The keys of the map
+        """
+        ...
+    def put(self, key: PyXdmAtomicValue, value: PyXdmValue) -> PyXdmMap:
+        """Put an entry into the map. And return a new map with the entry added.
+
+        Args:
+            key (PyXdmAtomicValue): The key
+            value (PyXdmValue): The value
+
+        Returns:
+            PyXdmMap: The map with the entry added
+        """
+        ...
+    def remove(self, key: PyXdmValue) -> PyXdmMap:
+        """Remove an entry from the map.
+
+        Args:
+            key (PyXdmValue): The key
+
+        Returns:
+            PyXdmMap: The map with the entry removed
+        """
+        ...
+    def values(self) -> list[PyXdmValue]:
+        """Get the values of the map.
+
+        Returns:
+            list[PyXdmValue]: The values of the map
+        """
+        ...
 
 class PyXdmNode(PyXdmItem):
     def __init__(self) -> None: ...
```

### Comparing `saxonche_stubs-0.3.0/setup.py` & `saxonche_stubs-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['saxonche>=12.1.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'saxonche-stubs',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Type stubs for saxonche',
     'long_description': '# saxonche-stubs\n\nType stubs for the [saxonche](https://pypi.org/project/saxonche/) python package. This package has no functionality itself, but is merely an addition to the completion within IDEs. The basis for type annotations and comments is the documentation of [the Saxon Python API](https://www.saxonica.com/saxon-c/doc11/html/saxonc.html).\n\nAt the moment not all APIs are fully typed.\n\n## Author / Contact\n\n- [Bastian Politycki](https://github.com/Bpolitycki) – Swiss Law Sources\n',
     'author': 'Bpolitycki',
     'author_email': 'bastian.politycki@unisg.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `saxonche_stubs-0.3.0/PKG-INFO` & `saxonche_stubs-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saxonche-stubs
-Version: 0.3.0
+Version: 0.4.0
 Summary: Type stubs for saxonche
 License: GPL-3.0-or-later
 Author: Bpolitycki
 Author-email: bastian.politycki@unisg.ch
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```


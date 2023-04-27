# Comparing `tmp/robotcode_plugin-0.34.1.tar.gz` & `tmp/robotcode_plugin-0.35.0.tar.gz`

## Comparing `robotcode_plugin-0.34.1.tar` & `robotcode_plugin-0.35.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/src/robotcode/plugin/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/src/robotcode/plugin/__version__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/src/robotcode/plugin/manager.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/src/robotcode/plugin/py.typed
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/src/robotcode/plugin/specs.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/src/robotcode/plugin/click_helper/helper.py
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/src/robotcode/plugin/click_helper/server_options.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/README.md
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/pyproject.toml
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_plugin-0.34.1/PKG-INFO
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/src/robotcode/plugin/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/src/robotcode/plugin/__version__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/src/robotcode/plugin/manager.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/src/robotcode/plugin/py.typed
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/src/robotcode/plugin/specs.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/src/robotcode/plugin/click_helper/aliases.py
+-rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/src/robotcode/plugin/click_helper/server_options.py
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/src/robotcode/plugin/click_helper/types.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/README.md
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/pyproject.toml
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 robotcode_plugin-0.35.0/PKG-INFO
```

### Comparing `robotcode_plugin-0.34.1/src/robotcode/plugin/__init__.py` & `robotcode_plugin-0.35.0/src/robotcode/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.34.1/src/robotcode/plugin/manager.py` & `robotcode_plugin-0.35.0/src/robotcode/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.34.1/src/robotcode/plugin/click_helper/helper.py` & `robotcode_plugin-0.35.0/src/robotcode/plugin/click_helper/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.34.1/src/robotcode/plugin/click_helper/server_options.py` & `robotcode_plugin-0.35.0/src/robotcode/plugin/click_helper/server_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional, Sequence, Set, Tuple
 
 import click
 from robotcode.core.types import ServerMode
 from robotcode.plugin import Application
-from robotcode.plugin.click_helper.helper import (
+from robotcode.plugin.click_helper.types import (
     AddressesPort,
     AddressParamType,
     AddressPortParamType,
     EnumChoice,
     MutuallyExclusiveOption,
     NameParamType,
     PortParamType,
 )
 
-from .helper import FC
+from .types import FC
 
 
 def server_options(
     default_server_mode: ServerMode, default_port: int, allowed_server_modes: Optional[Set[ServerMode]] = None
 ) -> Sequence[FC]:
     result = []
```

### Comparing `robotcode_plugin-0.34.1/.gitignore` & `robotcode_plugin-0.35.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.34.1/LICENSE.txt` & `robotcode_plugin-0.35.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.34.1/README.md` & `robotcode_plugin-0.35.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.34.1/pyproject.toml` & `robotcode_plugin-0.35.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.34.1/PKG-INFO` & `robotcode_plugin-0.35.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-plugin
-Version: 0.34.1
+Version: 0.35.0
 Summary: Some classes for RobotCode plugin management
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
 Author-email: Daniel Biehl <dbiehl@live.de>
```


# Comparing `tmp/robotcode_runner-0.34.1.tar.gz` & `tmp/robotcode_runner-0.35.0.tar.gz`

## Comparing `robotcode_runner-0.34.1.tar` & `robotcode_runner-0.35.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/PKG-INFO
```

### Comparing `robotcode_runner-0.34.1/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.35.0/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.34.1/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.35.0/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.34.1/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.35.0/src/robotcode/runner/cli/robot.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, List, Optional, Tuple, Union, cast
 
 import click
 from robot.errors import DataError, Information
 from robot.run import USAGE, RobotFramework
 from robot.version import get_full_version
 from robotcode.plugin import Application, pass_application
+from robotcode.plugin.click_helper.aliases import AliasedCommand
 from robotcode.robot.config.loader import load_config_from_path
 from robotcode.robot.config.utils import get_config_files
 
 from ..__version__ import __version__
 
 
 class RobotFrameworkEx(RobotFramework):
@@ -50,14 +51,16 @@
         if self.root_folder is not None:
             os.chdir(self.root_folder)
 
         return super().main(arguments, **options)
 
 
 @click.command(
+    cls=AliasedCommand,
+    aliases=["run"],
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
@@ -81,14 +84,19 @@
     by_longname: Tuple[str, ...],
     exclude_by_longname: Tuple[str, ...],
     robot_options_and_args: Tuple[str, ...],
 ) -> None:
     """Runs `robot` with the selected configuration, profiles, options and arguments.
 
     The options and arguments are passed to `robot` as is.
+
+    Examples:
+    ```
+    robotcode run
+    ```
     """
 
     robot_arguments: Optional[List[Union[str, Path]]] = None
     try:
         _, robot_arguments = RobotFramework().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
```

### Comparing `robotcode_runner-0.34.1/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.35.0/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.34.1/.gitignore` & `robotcode_runner-0.35.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.34.1/LICENSE.txt` & `robotcode_runner-0.35.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.34.1/README.md` & `robotcode_runner-0.35.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.34.1/pyproject.toml` & `robotcode_runner-0.35.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.34.1",
-  "robotcode-modifiers==0.34.1",
-  "robotcode==0.34.1",
+  "robotcode-robot==0.35.0",
+  "robotcode-modifiers==0.35.0",
+  "robotcode==0.35.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.34.1/PKG-INFO` & `robotcode_runner-0.35.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.34.1
+Version: 0.35.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.34.1
-Requires-Dist: robotcode-robot==0.34.1
-Requires-Dist: robotcode==0.34.1
+Requires-Dist: robotcode-modifiers==0.35.0
+Requires-Dist: robotcode-robot==0.35.0
+Requires-Dist: robotcode==0.35.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```


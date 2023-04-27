# Comparing `tmp/phases-1.0.3.tar.gz` & `tmp/phases-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phases-1.0.3.tar", last modified: Wed Mar  8 13:04:10 2023, max compression
+gzip compressed data, was "phases-1.0.4.tar", last modified: Thu Apr 27 11:23:07 2023, max compression
```

## Comparing `phases-1.0.3.tar` & `phases-1.0.4.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.932622 phases-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-03-08 13:03:46.000000 phases-1.0.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-08 13:03:46.000000 phases-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3077 2023-03-08 13:04:10.931622 phases-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-03-08 13:03:46.000000 phases-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.919621 phases-1.0.3/phases/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-03-08 13:03:47.000000 phases-1.0.3/phases/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-08 13:03:46.000000 phases-1.0.3/phases/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     2912 2023-03-08 13:03:46.000000 phases-1.0.3/phases/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.924621 phases-1.0.3/phases/commands/
--rw-rw-rw-   0 root         (0) root         (0)     5780 2023-03-08 13:03:46.000000 phases-1.0.3/phases/commands/Base.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-03-08 13:03:46.000000 phases-1.0.3/phases/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3606 2023-03-08 13:03:46.000000 phases-1.0.3/phases/commands/create.py
--rw-rw-rw-   0 root         (0) root         (0)     5585 2023-03-08 13:03:46.000000 phases-1.0.3/phases/commands/gridrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4967 2023-03-08 13:03:46.000000 phases-1.0.3/phases/commands/run.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-03-08 13:03:46.000000 phases-1.0.3/phases/commands/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.925621 phases-1.0.3/phases/generate-template/
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-03-08 13:03:46.000000 phases-1.0.3/phases/generate-template/Dockerfile.mustache
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-03-08 13:03:46.000000 phases-1.0.3/phases/generate-template/README.md.mustache
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-03-08 13:03:46.000000 phases-1.0.3/phases/generate-template/docker-compose.yml.mustache
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.925621 phases-1.0.3/phases/generate-template/docs/
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-03-08 13:03:46.000000 phases-1.0.3/phases/generate-template/docs/sequence.md.mustache
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-03-08 13:03:46.000000 phases-1.0.3/phases/generate-template/packages.m
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.927621 phases-1.0.3/phases/generate-template/{{name}}/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-08 13:03:46.000000 phases-1.0.3/phases/generate-template/{{name}}/__init__.py.mustache
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-03-08 13:03:46.000000 phases-1.0.3/phases/generate-template/{{name}}/__main__.py.mustache
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-03-08 13:03:46.000000 phases-1.0.3/phases/generate-template/{{name}}/exporter.mustache
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-03-08 13:03:46.000000 phases-1.0.3/phases/generate-template/{{name}}/phases.mustache
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.927621 phases-1.0.3/phases/static-template/
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-03-08 13:03:46.000000 phases-1.0.3/phases/static-template/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.922621 phases-1.0.3/phases.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3077 2023-03-08 13:04:10.000000 phases-1.0.3/phases.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1233 2023-03-08 13:04:10.000000 phases-1.0.3/phases.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 13:04:10.000000 phases-1.0.3/phases.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-03-08 13:04:10.000000 phases-1.0.3/phases.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-03-08 13:04:10.000000 phases-1.0.3/phases.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-08 13:04:10.000000 phases-1.0.3/phases.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-03-08 13:03:46.000000 phases-1.0.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-03-08 13:03:46.000000 phases-1.0.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-08 13:04:10.932622 phases-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-03-08 13:03:47.000000 phases-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.916621 phases-1.0.3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.929622 phases-1.0.3/tests/acceptance/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 13:03:46.000000 phases-1.0.3/tests/acceptance/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1337 2023-03-08 13:03:46.000000 phases-1.0.3/tests/acceptance/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      694 2023-03-08 13:03:46.000000 phases-1.0.3/tests/acceptance/test_create.py
--rw-rw-rw-   0 root         (0) root         (0)    13130 2023-03-08 13:03:46.000000 phases-1.0.3/tests/acceptance/test_grid.py
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-03-08 13:03:46.000000 phases-1.0.3/tests/acceptance/test_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:04:10.931622 phases-1.0.3/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 13:03:46.000000 phases-1.0.3/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5583 2023-03-08 13:03:46.000000 phases-1.0.3/tests/unit/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2023-03-08 13:03:46.000000 phases-1.0.3/tests/unit/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8932 2023-03-08 13:03:46.000000 phases-1.0.3/tests/unit/test_gridrun.py
--rw-rw-rw-   0 root         (0) root         (0)     7260 2023-03-08 13:03:46.000000 phases-1.0.3/tests/unit/test_run.py
--rw-rw-rw-   0 root         (0) root         (0)     4091 2023-03-08 13:03:46.000000 phases-1.0.3/tests/unit/test_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.965274 phases-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 11:22:43.000000 phases-1.0.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-27 11:22:43.000000 phases-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-04-27 11:23:07.965274 phases-1.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-04-27 11:22:43.000000 phases-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.952273 phases-1.0.4/phases/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-27 11:22:45.000000 phases-1.0.4/phases/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-04-27 11:22:43.000000 phases-1.0.4/phases/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2708 2023-04-27 11:22:43.000000 phases-1.0.4/phases/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.957273 phases-1.0.4/phases/commands/
+-rw-rw-rw-   0 root         (0) root         (0)     5780 2023-04-27 11:22:43.000000 phases-1.0.4/phases/commands/Base.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-27 11:22:43.000000 phases-1.0.4/phases/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3606 2023-04-27 11:22:43.000000 phases-1.0.4/phases/commands/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     5611 2023-04-27 11:22:43.000000 phases-1.0.4/phases/commands/gridrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4967 2023-04-27 11:22:43.000000 phases-1.0.4/phases/commands/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2023-04-27 11:22:43.000000 phases-1.0.4/phases/commands/savedata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-04-27 11:22:43.000000 phases-1.0.4/phases/commands/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.958273 phases-1.0.4/phases/generate-template/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-04-27 11:22:43.000000 phases-1.0.4/phases/generate-template/Dockerfile.mustache
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-27 11:22:43.000000 phases-1.0.4/phases/generate-template/README.md.mustache
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-27 11:22:43.000000 phases-1.0.4/phases/generate-template/docker-compose.yml.mustache
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.959273 phases-1.0.4/phases/generate-template/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-27 11:22:43.000000 phases-1.0.4/phases/generate-template/docs/sequence.md.mustache
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-27 11:22:43.000000 phases-1.0.4/phases/generate-template/packages.m
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.960273 phases-1.0.4/phases/generate-template/{{name}}/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-27 11:22:43.000000 phases-1.0.4/phases/generate-template/{{name}}/__init__.py.mustache
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-04-27 11:22:43.000000 phases-1.0.4/phases/generate-template/{{name}}/__main__.py.mustache
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-04-27 11:22:43.000000 phases-1.0.4/phases/generate-template/{{name}}/exporter.mustache
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-04-27 11:22:43.000000 phases-1.0.4/phases/generate-template/{{name}}/phases.mustache
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.960273 phases-1.0.4/phases/static-template/
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-04-27 11:22:43.000000 phases-1.0.4/phases/static-template/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.954273 phases-1.0.4/phases.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-04-27 11:23:07.000000 phases-1.0.4/phases.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-04-27 11:23:07.000000 phases-1.0.4/phases.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:23:07.000000 phases-1.0.4/phases.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-27 11:23:07.000000 phases-1.0.4/phases.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-27 11:23:07.000000 phases-1.0.4/phases.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 11:23:07.000000 phases-1.0.4/phases.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-04-27 11:22:43.000000 phases-1.0.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-27 11:22:43.000000 phases-1.0.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 11:23:07.965274 phases-1.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-04-27 11:22:45.000000 phases-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.949273 phases-1.0.4/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.962274 phases-1.0.4/tests/acceptance/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 11:22:43.000000 phases-1.0.4/tests/acceptance/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1337 2023-04-27 11:22:43.000000 phases-1.0.4/tests/acceptance/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      694 2023-04-27 11:22:43.000000 phases-1.0.4/tests/acceptance/test_create.py
+-rw-rw-rw-   0 root         (0) root         (0)    14148 2023-04-27 11:22:43.000000 phases-1.0.4/tests/acceptance/test_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-04-27 11:22:43.000000 phases-1.0.4/tests/acceptance/test_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:23:07.964274 phases-1.0.4/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 11:22:43.000000 phases-1.0.4/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5583 2023-04-27 11:22:43.000000 phases-1.0.4/tests/unit/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2023-04-27 11:22:43.000000 phases-1.0.4/tests/unit/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8932 2023-04-27 11:22:43.000000 phases-1.0.4/tests/unit/test_gridrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     7260 2023-04-27 11:22:43.000000 phases-1.0.4/tests/unit/test_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     4091 2023-04-27 11:22:43.000000 phases-1.0.4/tests/unit/test_test.py
```

### Comparing `phases-1.0.3/LICENSE` & `phases-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/PKG-INFO` & `phases-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phases
-Version: 1.0.3
+Version: 1.0.4
 Summary: An Execution Framework for pyPhase projects
 Home-page: https://gitlab.com/tud.ibmt/phases
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `phases-1.0.3/README.md` & `phases-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/phases/cli.py` & `phases-1.0.4/phases/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,18 +53,14 @@
     )
 
     # Here we'll try to dynamically match the command the user is trying to run
     # with a pre-defined command class we've already created.
     for (k, v) in options.items():
         if hasattr(phases.commands, k) and v:
             module = getattr(phases.commands, k)
-            commands = getmembers(module, isclass)
-            commands = list(filter(lambda c: c[0] != "Base" and issubclass(c[1], Base), commands))
+            className = k.title()
 
-            (
-                commandName,
-                command,
-            ) = commands.pop()  # get last defined class to skip imports
-            Logger.log("Run Command %s" % (commandName), "phases", LogLevel.DEBUG)
-            command = command(options)
+            commandClass = getattr(module, className)
+            command = commandClass(options)
+            Logger.log(f"Run Command {className}", "phases", LogLevel.DEBUG)
             command.run()
             sys.exit()
```

### Comparing `phases-1.0.3/phases/commands/Base.py` & `phases-1.0.4/phases/commands/Base.py`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/phases/commands/create.py` & `phases-1.0.4/phases/commands/create.py`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/phases/commands/gridrun.py` & `phases-1.0.4/phases/commands/gridrun.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,25 @@
         self.writer = None
         self.runSettings = None
         self.csvLogFile = "output.csv"
 
     def parseRunOptions(self):
         super().parseRunOptions()
         if self.options["<gridfile>"]:
-            self.projectGridFile = self.options["<gridfile>"]
+            self.projectGridFile = self.options["<gridfile>"].strip()
             self.logDebug("Set Gridfile file: %s" % (self.projectGridFile))
         if self.options["--csv"]:
             self.csvLogFile = self.options["--csv"]
             self.logDebug("Set CSV log file: %s" % (self.csvLogFile))
         if self.options["-r"]:
             self.resume = False
 
     def getGrid(self, config, path=None, grid=None):
         path = path or []
-        grid = grid or []
+        grid = [] if grid is None else grid
         config = pdict(config)
         for field in config:
             value = config[field]
             p = path + [field]
             key = field
 
             if isinstance(value, dict):
```

### Comparing `phases-1.0.3/phases/commands/run.py` & `phases-1.0.4/phases/commands/run.py`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/phases/commands/test.py` & `phases-1.0.4/phases/commands/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from phases.commands.run import Run
-from pyPhases.test import TestCase, TestCaseIntegration
-from unittest.loader import TestLoader
-from unittest.suite import TestSuite
-from unittest import TextTestRunner
 import os
 import sys
-
 from pathlib import Path
+from unittest import TextTestRunner
+from unittest.loader import TestLoader
+from unittest.suite import TestSuite
+
+from pyPhases.test import TestCase, TestCaseIntegration
+
+from phases.commands.run import Run
 
 
 class Test(Run):
     """test a Phase-Project by wrapping TestCases from pyPhase with the project and a configfile specified in project.test.yaml"""
 
     def __init__(self, options, *args, **kwargs):
         super().__init__(options, *args, **kwargs)
@@ -19,53 +20,49 @@
         self.testPattern = "test*.py"
 
     def parseRunOptions(self):
         super().parseRunOptions()
         if self.options["<testdir>"]:
             self.testDir = Path(self.outputDir).joinpath(self.options["<testdir>"]).as_posix()
             sys.path.insert(0, self.testDir)
-            self.logDebug("Set Testdir: %s" % (self.testDir))
+            self.logDebug(f"Set Testdir: {self.testDir}")
         if self.options["<testpattern>"]:
             self.testPattern = self.options["<testpattern>"]
         if self.options["-f"]:
             self.failFast = True
 
     def wrapTestsInSuite(self, testOrSuite, wrapMethod):
         tests = []
         if isinstance(testOrSuite, TestSuite):
             for subTestOrSuite in testOrSuite._tests:
                 tests += self.wrapTestsInSuite(subTestOrSuite, wrapMethod)
-        else:
-            check = wrapMethod(testOrSuite)
-            if check:
-                tests = [testOrSuite]
+        elif wrapMethod(testOrSuite):
+            tests = [testOrSuite]
         return tests
 
     def run(self):
         self.beforeRun()
         self.prepareConfig()
 
         project = self.createProjectFromConfig(self.config)
         TestCase.project = project
 
         loader = TestLoader()
-        self.logDebug("Discover Tests in %s for pattern %s (Basedir: %s)" % (self.testDir, self.testPattern, self.outputDir))
+        self.logDebug(f"Discover Tests in {self.testDir} for pattern {self.testPattern} (Basedir: {self.outputDir})")
         os.chdir(self.outputDir)
 
         if os.path.isdir(self.testDir):
             suite = loader.discover(self.testDir, self.testPattern)
         else:
             suite = loader.loadTestsFromName(self.testDir)
 
-        self.logDebug("Found Tests: %s" % (suite._tests))
+        self.logDebug(f"Found Tests: {suite._tests}")
 
         def wrapTestsInSuite(test):
-            if isinstance(test, TestCaseIntegration):
-                return False
-            return True
+            return not isinstance(test, TestCaseIntegration)
 
         noIntegrationTests = self.wrapTestsInSuite(suite, wrapTestsInSuite)
 
         suite = TestSuite()
         suite.addTests(noIntegrationTests)
         runner = TextTestRunner()
         runner.failfast = self.failFast
```

### Comparing `phases-1.0.3/phases/generate-template/{{name}}/__main__.py.mustache` & `phases-1.0.4/phases/generate-template/{{name}}/__main__.py.mustache`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/phases/generate-template/{{name}}/exporter.mustache` & `phases-1.0.4/phases/generate-template/{{name}}/exporter.mustache`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/phases/generate-template/{{name}}/phases.mustache` & `phases-1.0.4/phases/generate-template/{{name}}/phases.mustache`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/phases.egg-info/PKG-INFO` & `phases-1.0.4/phases.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phases
-Version: 1.0.3
+Version: 1.0.4
 Summary: An Execution Framework for pyPhase projects
 Home-page: https://gitlab.com/tud.ibmt/phases
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `phases-1.0.3/phases.egg-info/SOURCES.txt` & `phases-1.0.4/phases.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 phases.egg-info/requires.txt
 phases.egg-info/top_level.txt
 phases/commands/Base.py
 phases/commands/__init__.py
 phases/commands/create.py
 phases/commands/gridrun.py
 phases/commands/run.py
+phases/commands/savedata.py
 phases/commands/test.py
 phases/generate-template/Dockerfile.mustache
 phases/generate-template/README.md.mustache
 phases/generate-template/docker-compose.yml.mustache
 phases/generate-template/packages.m
 phases/generate-template/docs/sequence.md.mustache
 phases/generate-template/{{name}}/__init__.py.mustache
```

### Comparing `phases-1.0.3/setup.py` & `phases-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phases",
-    version="v1.0.3"[1:],
+    version="v1.0.4"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="An Execution Framework for pyPhase projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt/phases",
     packages=setuptools.find_packages(exclude=["tests", "example"]),
```

### Comparing `phases-1.0.3/tests/acceptance/test_cli.py` & `phases-1.0.4/tests/acceptance/test_cli.py`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/tests/acceptance/test_create.py` & `phases-1.0.4/tests/acceptance/test_create.py`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/tests/acceptance/test_grid.py` & `phases-1.0.4/tests/acceptance/test_grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,24 @@
         self.assertEqual(grid, self.fullGrid)
         flattenGrid = run.flattenGrid(grid)
         self.checkFullFlattenDiff(flattenGrid)
 
         project = Project()
         MockPhase.index = 0
         project.addPhase(MockPhase())
-        project.config = pdict()
+        project.config = pdict(
+            {
+                "p0": 0,
+                "p1": 0,
+                "p2": 0,
+                "p3": 0,
+                "p4": 0,
+                "p5": {"deep": 0},
+            }
+        )
         run.phaseName = "MockPhase"
 
         run.runProject(project)
         allEntries = run.csvLogger.getRowsAsList()
         dicts = run.csvLogger.getRowsAsDict()
 
         self.assertEqual(list(dicts[0].keys()), ["run", "p0", "p1", "p2", "p3", "p4", "p5/deep", "runIndex"])
@@ -61,14 +70,39 @@
         for index, resultGrid in enumerate(flattenGrid):
             resultConfig = [str(val) for i, val in resultGrid]
             row = allEntries[index]
             self.assertEqual(row[0], str(index + 1))
             self.assertEqual(row[1:7], resultConfig)
             self.assertEqual(row[7], str(index))
 
+    def testGridRunListKey(self):
+        config = pdict(
+            {
+                "mySteps": [
+                    {"name": "step1", "p0": 1},
+                    {"name": "step2", "p0": 4},
+                    {"name": "step3", "p0": 1},
+                ]
+            }
+        )
+        gridDict = {
+            "mySteps": {"1": {"p0": [0, 1]}},
+        }
+        run = Gridrun({})
+        grid = run.getGrid(gridDict)
+        flatten = run.flattenGrid(grid)
+
+        self.assertEqual(grid, [(["mySteps", "1", "p0"], [0, 1])])
+        self.assertEqual(flatten, [[(["mySteps", "1", "p0"], 0)], [(["mySteps", "1", "p0"], 1)]])
+
+        key, value = flatten[0][0]  #
+        config[key] = value
+        self.assertEqual(config["mySteps", 1, "name"], "step2")
+        self.assertEqual(config["mySteps", 1, "p0"], 0)
+
     def testGridRunRandom(self):
 
         allEntries, flattenGrid = self.runFullGrid(random=True)
 
         fixedRandomSeeds = self.getRandomOrder()
 
         for index in range(len(flattenGrid)):
```

### Comparing `phases-1.0.3/tests/acceptance/test_run.py` & `phases-1.0.4/tests/acceptance/test_run.py`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/tests/unit/test_base.py` & `phases-1.0.4/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/tests/unit/test_config.py` & `phases-1.0.4/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/tests/unit/test_gridrun.py` & `phases-1.0.4/tests/unit/test_gridrun.py`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/tests/unit/test_run.py` & `phases-1.0.4/tests/unit/test_run.py`

 * *Files identical despite different names*

### Comparing `phases-1.0.3/tests/unit/test_test.py` & `phases-1.0.4/tests/unit/test_test.py`

 * *Files identical despite different names*


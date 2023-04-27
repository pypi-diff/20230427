# Comparing `tmp/NREL-gaps-0.2.1.tar.gz` & `tmp/NREL-gaps-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-gaps-0.2.1.tar", last modified: Wed Apr 26 21:33:14 2023, max compression
+gzip compressed data, was "NREL-gaps-0.3.0.tar", last modified: Wed Apr 26 21:34:08 2023, max compression
```

## Comparing `NREL-gaps-0.2.1.tar` & `NREL-gaps-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwx---   0 ppinchuk (132335) ppinchuk (132335)        0 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     1526 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/LICENSE
-drwxrwx---   0 ppinchuk (132335) ppinchuk (132335)        0 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/NREL_gaps.egg-info/
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     2803 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/NREL_gaps.egg-info/PKG-INFO
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)      702 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/NREL_gaps.egg-info/SOURCES.txt
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)        1 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/NREL_gaps.egg-info/dependency_links.txt
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)        1 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/NREL_gaps.egg-info/not-zip-safe
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)      423 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/NREL_gaps.egg-info/requires.txt
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)        5 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/NREL_gaps.egg-info/top_level.txt
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     2803 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/PKG-INFO
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     2194 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/README.rst
-drwxrwx---   0 ppinchuk (132335) ppinchuk (132335)        0 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/gaps/
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)      436 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/__init__.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    15113 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/batch.py
-drwxrwx---   0 ppinchuk (132335) ppinchuk (132335)        0 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/gaps/cli/
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)       73 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/__init__.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     2369 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/batch.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     6633 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/cli.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     3262 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/collect.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    12497 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/command.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    16352 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/config.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    16907 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/documentation.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     5346 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/execution.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     4292 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/pipeline.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     5360 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/preprocessing.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     7766 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/status.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     3518 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/cli/templates.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    32534 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/collection.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     8418 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/config.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     1104 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/exceptions.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    23243 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/hpc.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    14059 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/legacy.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     5917 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/log.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    11008 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/pipeline.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    10414 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/project_points.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    25080 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/status.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     4717 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/utilities.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)       54 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/version.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)      589 2023-04-11 18:03:02.000000 NREL-gaps-0.2.1/gaps/warnings.py
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)       38 2023-04-26 21:33:14.000000 NREL-gaps-0.2.1/setup.cfg
--rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     1718 2023-04-26 21:33:09.000000 NREL-gaps-0.2.1/setup.py
+drwxrwx---   0 ppinchuk (132335) ppinchuk (132335)        0 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     1523 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/LICENSE
+drwxrwx---   0 ppinchuk (132335) ppinchuk (132335)        0 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/NREL_gaps.egg-info/
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     2848 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/NREL_gaps.egg-info/PKG-INFO
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)      702 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/NREL_gaps.egg-info/SOURCES.txt
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)        1 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/NREL_gaps.egg-info/dependency_links.txt
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)        1 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/NREL_gaps.egg-info/not-zip-safe
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)      423 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/NREL_gaps.egg-info/requires.txt
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)        5 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/NREL_gaps.egg-info/top_level.txt
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     2848 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/PKG-INFO
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     2239 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/README.rst
+drwxrwx---   0 ppinchuk (132335) ppinchuk (132335)        0 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/gaps/
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)      436 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/__init__.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    15113 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/batch.py
+drwxrwx---   0 ppinchuk (132335) ppinchuk (132335)        0 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/gaps/cli/
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)      139 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/__init__.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     2369 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/batch.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     6640 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/cli.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     3262 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/collect.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    27881 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/command.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    18475 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/config.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    18257 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/documentation.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     5960 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/execution.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     4292 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/pipeline.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     5360 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/preprocessing.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     9496 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/status.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     3518 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/cli/templates.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    32534 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/collection.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     8418 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/config.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     1104 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/exceptions.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    23886 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/hpc.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    14359 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/legacy.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     5917 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/log.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    11008 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/pipeline.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    10414 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/project_points.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)    25840 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/status.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     4717 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/utilities.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)       54 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/version.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)      694 2023-04-26 19:38:35.000000 NREL-gaps-0.3.0/gaps/warnings.py
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)       38 2023-04-26 21:34:08.000000 NREL-gaps-0.3.0/setup.cfg
+-rw-rw----   0 ppinchuk (132335) ppinchuk (132335)     1718 2023-04-26 21:34:03.000000 NREL-gaps-0.3.0/setup.py
```

### Comparing `NREL-gaps-0.2.1/LICENSE` & `NREL-gaps-0.3.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Alliance for Sustainable Energy LLC, All rights reserved.
+Copyright (c) 2023, Alliance for Sustainable Energy, LLC
 
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
-* Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `NREL-gaps-0.2.1/NREL_gaps.egg-info/PKG-INFO` & `NREL-gaps-0.3.0/NREL_gaps.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-gaps
-Version: 0.2.1
+Version: 0.3.0
 Summary: National Renewable Energy Laboratory's (NREL's) Geospatial Analysis Pipelines (GAPs) framework
 Home-page: https://nrel.github.io/gaps/
 Author: Paul Pinchuk
 Maintainer-email: ppinchuk@nrel.gov
 License: BSD 3-Clause
 Keywords: gaps
 Classifier: Intended Audience :: Science/Research
@@ -61,7 +61,12 @@
 Development
 ===========
 
 This repository uses `pylint <https://pylint.pycqa.org/en/latest/>`_ to lint the code and
 `black <https://black.readthedocs.io/en/stable/index.html>`_ to format it (check out the
 `black formatting style <https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html>`_).
 If you wish to contribute to this repository, your code will have to adhere to both of these guidelines and pass all existing tests.
+
+
+Authors
+=======
+Paul Pinchuk, Grant Buster
```

### Comparing `NREL-gaps-0.2.1/NREL_gaps.egg-info/SOURCES.txt` & `NREL-gaps-0.3.0/NREL_gaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/PKG-INFO` & `NREL-gaps-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-gaps
-Version: 0.2.1
+Version: 0.3.0
 Summary: National Renewable Energy Laboratory's (NREL's) Geospatial Analysis Pipelines (GAPs) framework
 Home-page: https://nrel.github.io/gaps/
 Author: Paul Pinchuk
 Maintainer-email: ppinchuk@nrel.gov
 License: BSD 3-Clause
 Keywords: gaps
 Classifier: Intended Audience :: Science/Research
@@ -61,7 +61,12 @@
 Development
 ===========
 
 This repository uses `pylint <https://pylint.pycqa.org/en/latest/>`_ to lint the code and
 `black <https://black.readthedocs.io/en/stable/index.html>`_ to format it (check out the
 `black formatting style <https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html>`_).
 If you wish to contribute to this repository, your code will have to adhere to both of these guidelines and pass all existing tests.
+
+
+Authors
+=======
+Paul Pinchuk, Grant Buster
```

### Comparing `NREL-gaps-0.2.1/README.rst` & `NREL-gaps-0.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -41,8 +41,13 @@
 
 Development
 ===========
 
 This repository uses `pylint <https://pylint.pycqa.org/en/latest/>`_ to lint the code and
 `black <https://black.readthedocs.io/en/stable/index.html>`_ to format it (check out the
 `black formatting style <https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html>`_).
-If you wish to contribute to this repository, your code will have to adhere to both of these guidelines and pass all existing tests.
+If you wish to contribute to this repository, your code will have to adhere to both of these guidelines and pass all existing tests.
+
+
+Authors
+=======
+Paul Pinchuk, Grant Buster
```

### Comparing `NREL-gaps-0.2.1/gaps/batch.py` & `NREL-gaps-0.3.0/gaps/batch.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/cli/batch.py` & `NREL-gaps-0.3.0/gaps/cli/batch.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/cli/cli.py` & `NREL-gaps-0.3.0/gaps/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,83 +8,86 @@
 
 from gaps import Pipeline
 from gaps.cli.batch import batch_command
 from gaps.cli.templates import template_command
 from gaps.cli.pipeline import pipeline_command, template_pipeline_config
 from gaps.cli.collect import collect
 from gaps.cli.config import from_config
-from gaps.cli.command import CLICommandConfiguration, _WrappedCommand
+from gaps.cli.command import (
+    CLICommandFromFunction,
+    _WrappedCommand,
+)
 from gaps.cli.preprocessing import preprocess_collect_config
 from gaps.cli.status import status_command
 
 
 class _CLICommandGenerator:
     """Generate commands from a list of configurations."""
 
     def __init__(self, command_configs):
         """
 
         Parameters
         ----------
-        command_configs : list of :class:`CLICommandConfiguration`
+        command_configs : list of :class:`CLICommandFromFunction`
             List of command configs to convert to click commands.
         """
         self.command_configs = command_configs
         self.commands, self.template_configs = [], {}
 
     def add_collect_command_configs(self):
         """Add collect command if the function is split spatially."""
         all_commands = []
         for command_configuration in self.command_configs:
             all_commands.append(command_configuration)
-            if command_configuration.is_split_spatially:
-                collect_configuration = CLICommandConfiguration(
+            if command_configuration.add_collect:
+                collect_configuration = CLICommandFromFunction(
                     name=f"collect-{command_configuration.name}",
                     function=collect,
                     split_keys=[("_out_path", "_pattern")],
                     config_preprocessor=preprocess_collect_config,
                 )
                 all_commands.append(collect_configuration)
         self.command_configs = all_commands
         return self
 
     def convert_to_commands(self):
         """Convert all of the command configs into click commands."""
         for command_config in self.command_configs:
-            func_doc = command_config.function_documentation
+            doc = command_config.documentation
             name = command_config.name
             params = [
                 click.Option(
                     param_decls=["--config_file", "-c"],
                     required=True,
                     type=click.Path(exists=True),
-                    help=func_doc.config_help(name),
+                    help=doc.config_help(name),
                 )
             ]
 
             command = _WrappedCommand(
                 name,
                 context_settings=None,
                 callback=partial(
                     from_config,
                     command_config=command_config,
                 ),
                 params=params,
-                help=func_doc.command_help(name),
+                help=doc.command_help(name),
                 epilog=None,
                 short_help=None,
                 options_metavar="[OPTIONS]",
                 add_help_option=True,
                 no_args_is_help=True,
                 hidden=False,
                 deprecated=False,
             )
             self.commands.append(command)
             Pipeline.COMMANDS[name] = command
-            self.template_configs[name] = func_doc.template_config
+            self.template_configs[name] = doc.template_config
         return self
 
     def add_pipeline_command(self):
         """Add pipeline command, which includes the previous commands."""
         tpc = template_pipeline_config(self.command_configs)
         pipeline = pipeline_command(tpc)
         self.commands = [pipeline] + self.commands
@@ -124,23 +127,24 @@
 
     This function generates a CLI for a package based on the input
     command configurations. Each command configuration is based around
     a function that is to be executed on one or more nodes.
 
     Parameters
     ----------
-    commands : list of :class:`~gaps.cli.command.CLICommandConfiguration`
+    commands : list of command configurations
         List of command configs to convert to click commands. See the
-        :class:`~gaps.cli.command.CLICommandConfiguration` documentation
-        for a description of the input options. Each command
-        configuration is converted into a subcommand. Any command
-        configuration with ``project_points`` in the `split_keys`
-        argument will get a corresponding ``collect-{command name}``
-        command that collects the outputs of the spatially-distributed
-        command.
+        :class:`~gaps.cli.command.CLICommandFromClass` or
+        :class:`~gaps.cli.command.CLICommandFromFunction`
+        documentation for a description of the input options. Each
+        command configuration is converted into a subcommand. Any
+        command configuration with ``project_points`` in the
+        `split_keys` argument will get a corresponding
+        ``collect-{command name}`` command that collects the outputs of
+        the spatially-distributed command.
     info : dict, optional
         A dictionary that contains optional info about the calling
         program to include in the CLI. Allowed keys include:
 
             name : str
                 Name of program to display at the top of the CLI help.
             version : str
```

### Comparing `NREL-gaps-0.2.1/gaps/cli/collect.py` & `NREL-gaps-0.3.0/gaps/cli/collect.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/cli/config.py` & `NREL-gaps-0.3.0/gaps/cli/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,42 @@
 GAPs CLI command for spatially distributed function runs.
 """
 import json
 import logging
 from copy import deepcopy
 from warnings import warn
 from pathlib import Path
-from inspect import signature
 from itertools import product
+from inspect import signature, isclass
 
 import click
 
 from rex.utilities.loggers import init_mult  # cspell:disable-line
 
 from gaps import ProjectPoints
-from gaps.status import StatusUpdates
+from gaps.status import StatusUpdates, QOSOption, HardwareOption
 from gaps.config import load_config
 from gaps.log import init_logger
 from gaps.cli.execution import kickoff_job
 from gaps.exceptions import gapsKeyError
 from gaps.warnings import gapsWarning
 
 logger = logging.getLogger(__name__)
 
 _CMD_LIST = [
     "from gaps.cli.config import run_with_status_updates",
     "from {run_func_module} import {run_func_name}",
-    "n_args = {node_specific_config}, {logging_options}",
     'su_args = "{project_dir}", "{command}", "{job_name}"',
     "run_with_status_updates("
-    "   {run_func_name}, n_args, su_args, {exclude_from_status}"
+    "   {run_func_name}, {node_specific_config}, {logging_options}, su_args, "
+    "   {exclude_from_status}"
     ")",
 ]
 TAG = "_j"
+MAX_AU_BEFORE_WARNING = 10_000
 
 
 class _FromConfig:
     """Utility class for running a function from a config file."""
 
     def __init__(self, ctx, config_file, command_config):
         """
@@ -45,15 +46,15 @@
         Parameters
         ----------
         ctx : click.Context
             Click context for the invoked command.
         config_file : path-like
             Path to input file containing key-value pairs as input to
             function.
-        command_config : `gaps.cli.cli.CLICommandConfiguration`
+        command_config : `gaps.cli.cli.CLICommandFromFunction`
             A command configuration object containing info such as the
             command name, run function, pre-processing function,
             function documentation, etc.
         """
         self.ctx = ctx
         self.config_file = Path(config_file).expanduser().resolve()
         self.command_config = command_config
@@ -97,17 +98,15 @@
             file=pipe_log_file.as_posix(),
         )
         return self
 
     def validate_config(self):
         """Validate the user input config file."""
         logger.debug("Validating %r", self.config_file)
-        _validate_config(
-            self.config, self.command_config.function_documentation
-        )
+        _validate_config(self.config, self.command_config.documentation)
         return self
 
     def preprocess_config(self):
         """Apply preprocessing function to config file."""
 
         preprocessor_kwargs = {
             "config": self.config,
@@ -193,14 +192,15 @@
 
     def kickoff_jobs(self):
         """Kickoff jobs across nodes based on config and run function."""
         keys_to_run, lists_to_run = self._keys_and_lists_to_run()
 
         jobs = sorted(product(*lists_to_run))
         num_jobs_submit = len(jobs)
+        self._warn_about_excessive_au_usage(num_jobs_submit)
         n_zfill = len(str(num_jobs_submit))
         max_workers_per_node = self.exec_kwargs.pop("max_workers", None)
         for node_index, values in enumerate(jobs):
             if num_jobs_submit > 1:
                 tag = f"{TAG}{str(node_index).zfill(n_zfill)}"
             else:
                 tag = ""
@@ -212,26 +212,29 @@
                     "tag": tag,
                     "command_name": self.command_name,
                     "config_file": self.config_file.as_posix(),
                     "project_dir": self.project_dir.as_posix(),
                     "job_name": job_name,
                     "out_dir": self.project_dir.as_posix(),
                     "max_workers": max_workers_per_node,
+                    "run_method": getattr(
+                        self.command_config, "run_method", None
+                    ),
                 }
             )
 
             for key, val in zip(keys_to_run, values):
                 if isinstance(key, str):
                     node_specific_config.update({key: val})
                 else:
                     node_specific_config.update(dict(zip(key, val)))
 
             cmd = "; ".join(_CMD_LIST).format(
-                run_func_module=self.command_config.function.__module__,
-                run_func_name=self.command_config.function.__name__,
+                run_func_module=self.command_config.runner.__module__,
+                run_func_name=self.command_config.runner.__name__,
                 node_specific_config=as_script_str(node_specific_config),
                 project_dir=self.project_dir.as_posix(),
                 logging_options=as_script_str(self.logging_options),
                 exclude_from_status=as_script_str(self.exclude_from_status),
                 command=self.command_name,
                 job_name=job_name,
             )
@@ -253,14 +256,42 @@
                 lists_to_run.append(
                     list(
                         zip(*[self.config.get(k) or [None] for k in key_group])
                     )
                 )
         return keys_to_run, lists_to_run
 
+    def _warn_about_excessive_au_usage(self, num_jobs):
+        """Warn if max job runtime exceeds AU threshold"""
+        max_walltime_per_job = self.exec_kwargs.get("walltime")
+        if max_walltime_per_job is None:
+            return
+
+        qos = self.exec_kwargs.get("qos") or str(QOSOption.UNSPECIFIED)
+        try:
+            qos_charge_factor = QOSOption(str(qos)).charge_factor
+        except ValueError:
+            qos_charge_factor = 1
+
+        hardware = self.exec_kwargs.get("option", "local")
+        try:
+            hardware_charge_factor = HardwareOption(hardware).charge_factor
+        except ValueError:
+            return
+
+        max_au_usage = int(
+            num_jobs
+            * max_walltime_per_job
+            * qos_charge_factor
+            * hardware_charge_factor
+        )
+        if max_au_usage > MAX_AU_BEFORE_WARNING:
+            msg = f"Job may use up to {max_au_usage:,} AUs!"
+            warn(msg, gapsWarning)
+
     def run(self):
         """Run the entire config pipeline."""
         return (
             self.enable_logging()
             .validate_config()
             .preprocess_config()
             .set_exec_kwargs()
@@ -273,29 +304,27 @@
 
 @click.pass_context
 def from_config(ctx, config_file, command_config):
     """Run command from a config file."""
     _FromConfig(ctx, config_file, command_config).run()
 
 
-def _validate_config(config, function_documentation):
+def _validate_config(config, documentation):
     """Ensure required keys exist and warn user about extra keys in config."""
-    _ensure_required_args_exist(config, function_documentation)
-    _warn_about_extra_args(config, function_documentation)
+    _ensure_required_args_exist(config, documentation)
+    _warn_about_extra_args(config, documentation)
 
 
-def _ensure_required_args_exist(config, function_documentation):
+def _ensure_required_args_exist(config, documentation):
     """Make sure that args required for func to run exist in config."""
     missing = {
-        name
-        for name in function_documentation.required_args
-        if name not in config
+        name for name in documentation.required_args if name not in config
     }
 
-    if function_documentation.max_workers_required:
+    if documentation.max_workers_required:
         missing = _mark_max_workers_missing_if_needed(config, missing)
 
     if any(missing):
         msg = (
             f"The following required keys are missing from the configuration "
             f"file: {missing}"
         )
@@ -307,36 +336,36 @@
 
     exec_control = config.get("execution_control", {})
     if "max_workers" not in config and "max_workers" not in exec_control:
         missing |= {"max_workers"}
     return missing
 
 
-def _warn_about_extra_args(config, function_documentation):
+def _warn_about_extra_args(config, documentation):
     """Warn user about extra unused keys in the config file."""
     extra = {
         name
         for name in config.keys()
-        if not _param_in_sig(name, function_documentation)
+        if not _param_in_sig(name, documentation)
     }
     extra -= {"execution_control", "project_points_split_range"}
     if any(extra):
         msg = (
             "Found unused keys in the configuration file: %s. To silence "
             "this warning, please remove these keys from the input "
             "configuration file."
         )
         warn(msg % extra, gapsWarning)
 
 
-def _param_in_sig(param, function_documentation):
+def _param_in_sig(param, documentation):
     """Determine if ``name`` is an argument in any func signatures"""
     return any(
         param in _public_args(signature)
-        for signature in function_documentation.signatures
+        for signature in documentation.signatures
     )
 
 
 def _public_args(func_signature):
     """Gather set of all "public" function args."""
     return {
         param
@@ -384,43 +413,81 @@
         json.dumps(input_)
         .replace("null", "None")
         .replace("false", "False")
         .replace("true", "True")
     )
 
 
-def run_with_status_updates(run_func, node_args, status_update_args, exclude):
+def run_with_status_updates(
+    run_func, config, logging_options, status_update_args, exclude
+):
     """Run a function and write status updated before/after execution.
 
     Parameters
     ----------
     run_func : callable
         A function to run.
-    node_args : iterable
-        An iterable containing the last three arguments to
-        :func:`node_kwargs`.
+    config : dict
+        Dictionary of node-specific inputs to `run_func`.
+    logging_options : dict
+        Dictionary of logging options containing at least the following
+        key-value pairs:
+
+            name : str
+                Job name; name of log file.
+            log_directory : path-like
+                Path to log file directory.
+            verbose : bool
+                Option to turn on debug logging.
+            node : bool
+                Flag for whether this is a node-level logger. If this is
+                a node logger, and the log level is info, the log_file
+                will be `None` (sent to stdout).
+
     status_update_args : iterable
         An iterable containing the first three initializer arguments for
         :class:`StatusUpdates`.
     exclude : collection | None
         A collection (list, set, dict, etc.) of keys that should be
         excluded from the job status file that is written before/after
         the function runs.
     """
-    run_kwargs = node_kwargs(run_func, *node_args)
+
+    # initialize loggers for multiple modules
+    init_mult(  # cspell:disable-line
+        logging_options["name"],
+        logging_options["log_directory"],
+        modules=[run_func.__module__.split(".")[0], "gaps", "rex"],
+        verbose=logging_options["verbose"],
+        node=logging_options["node"],
+    )
+
+    run_kwargs = node_kwargs(run_func, config)
     exclude = exclude or set()
     job_attrs = {
         key: value for key, value in run_kwargs.items() if key not in exclude
     }
     status_update_args = *status_update_args, job_attrs
     with StatusUpdates(*status_update_args) as status:
-        status.out_file = run_func(**run_kwargs)
+        out = run_func(**run_kwargs)
+        if method := config.get("run_method"):
+            func = getattr(out, method)
+            run_kwargs = node_kwargs(func, config)
+            status.job_attrs.update(
+                {
+                    key: value
+                    for key, value in run_kwargs.items()
+                    if key not in exclude
+                }
+            )
+            out = func(**run_kwargs)
+        status.out_file = out
 
 
-def node_kwargs(run_func, config, logging_options):
+def node_kwargs(run_func, config):
     """Compile the function inputs arguments for a particular node.
 
     Parameters
     ----------
     run_func : callable
         A function to run.
     config : dict
@@ -443,28 +510,20 @@
 
     Returns
     -------
     dict
         Function run kwargs to be used on this node.
     """
 
-    # initialize loggers for multiple modules
-    init_mult(  # cspell:disable-line
-        logging_options["name"],
-        logging_options["log_directory"],
-        modules=[run_func.__module__.split(".")[0], "gaps", "rex"],
-        verbose=logging_options["verbose"],
-        node=logging_options["node"],
-    )
-
     split_range = config.pop("project_points_split_range", None)
     if split_range is not None:
         config["project_points"] = ProjectPoints.from_range(
             split_range, config["project_points"]
         )
 
     sig = signature(run_func)
     run_kwargs = {
         k: v for k, v in config.items() if k in sig.parameters.keys()
     }
-    logger.debug("Running %r with kwargs: %s", run_func.__name__, run_kwargs)
+    verb = "Initializing" if isclass(run_func) else "Running"
+    logger.debug("%s %r with kwargs: %s", verb, run_func.__name__, run_kwargs)
     return run_kwargs
```

### Comparing `NREL-gaps-0.2.1/gaps/cli/documentation.py` & `NREL-gaps-0.3.0/gaps/cli/documentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 """
 CLI documentation utilities.
 """
 from copy import deepcopy
-from inspect import signature
+from inspect import signature, isclass
 
 from numpydoc.docscrape import NumpyDocString
 
 from gaps.config import config_as_str_for_docstring, ConfigType
 
 
 DEFAULT_EXEC_VALUES = {
     "option": "local",
     "allocation": "[REQUIRED IF ON HPC]",
     "walltime": "[REQUIRED IF ON HPC]",
+    "qos": "normal",
     "memory": None,
     "nodes": 1,
     "queue": None,
     "feature": None,
     "conda_env": None,
     "module": None,
     "sh_script": None,
@@ -200,19 +201,20 @@
 EXEC_CONTROL_DOC = """
 Parameters
 ----------
     execution_control : dict
         Dictionary containing execution control arguments. Allowed
         arguments are:
 
-        :option: ({{'local', 'slurm', 'eagle', 'pbs', 'peregrine'}})
-                 Hardware run option. 'eagle' and 'peregrine' are aliases for
-                 'slurm and 'pbs', respectively.
+        :option: ({{'local', 'kestrel', 'eagle', 'peregrine'}})
+                 Hardware run option. Determines the type of job scheduler
+                 tp use as well as the base AU cost.
         :allocation: (str) HPC project (allocation) handle.
         :walltime: (int) Node walltime request in hours.
+        :qos: (str) Quality-of-service specifier. By default, ``"normal"``.
         :memory: (int, optional) Node memory request in GB. Default is not to
                  specify.{n}{mw}
         :queue: (str, optional; PBS ONLY) HPC queue to submit job to.
                 Examples include: 'debug', 'short', 'batch', 'batch-h',
                 'long', etc. By default, `None`, which uses `test_queue`.
         :feature: (str, optional) Additional flags for SLURM job
                   (e.g. "--qos=high", "-p debug", etc). Default is not
@@ -224,28 +226,43 @@
         :sh_script: (str, optional) Extra shell script to run before
                     command call. Default is not to run any scripts.
 
         Only the "option" input is required for local execution. For
         execution on the HPC, the allocation and walltime are also
         required. All other options are populated with default values,
         as seen above.
+    log_directory : str
+        Path to directory where logs should be written. Path can be relative
+        and does not have to exist on disk (it will be created if missing).
+        By default, ``"./logs"``.
+    log_level : {{"DEBUG", "INFO", "WARNING", "ERROR"}}
+        String representation of desired logger verbosity. Suitable options
+        are ``DEBUG`` (most verbose), ``INFO`` (moderately verbose),
+        ``WARNING`` (only log warnings and errors), and ``ERROR`` (only log
+        errors). By default, ``"INFO"``.
 
 """
 NODES_DOC = (
     "\n        :nodes: (int, optional) Number of nodes to split the project "
     "\n                points across. Note that the total number of requested "
     "\n                nodes for a job may be larger than this value if the "
     "\n                command splits across other inputs (e.g. analysis "
     "\n                years) Default is 1."
 )
 MW_DOC = "\n        :max_workers: ({type}) {desc}"
 
 
-class FunctionDocumentation:
-    """Generate documentation for a function."""
+class CommandDocumentation:
+    """Generate documentation for a command.
+
+    Commands are typically comprised of one or more functions. This
+    definition includes class initializers and object methods.
+    Documentation is compiled from all input functions and used to
+    generate CLI help docs and template configuration files.
+    """
 
     REQUIRED_TAG = "[REQUIRED]"
 
     def __init__(self, *functions, skip_params=None, is_split_spatially=False):
         """
         Parameters
         ----------
@@ -259,16 +276,21 @@
             to specify these. By default, `None`.
         is_split_spatially : bool, optional
             Flag indicating wether or not this function is split
             spatially across nodes. If `True`, a "nodes" option is added
             to the execution control block of the generated
             documentation. By default, `False`.
         """
-        self.signatures = [signature(func) for func in functions]
-        self.docs = [NumpyDocString(func.__doc__ or "") for func in functions]
+        self.signatures = [
+            signature(func) for func in _as_functions(functions)
+        ]
+        self.docs = [
+            NumpyDocString(func.__doc__ or "")
+            for func in _as_functions(functions)
+        ]
         self.param_docs = {
             p.name: p for doc in self.docs for p in doc["Parameters"]
         }
         self.skip_params = set() if skip_params is None else set(skip_params)
         self.skip_params |= {"cls", "self", "max_workers"}
         self.is_split_spatially = is_split_spatially
 
@@ -348,15 +370,19 @@
             and name not in self.skip_params
         }
         return required_args
 
     @property
     def template_config(self):
         """dict: A template configuration file for this function."""
-        config = {"execution_control": self.default_exec_values}
+        config = {
+            "execution_control": self.default_exec_values,
+            "log_directory": "./logs",
+            "log_level": "INFO",
+        }
         config.update(
             {
                 x: self.REQUIRED_TAG if v.default is v.empty else v.default
                 for sig in self.signatures
                 for x, v in sig.parameters.items()
                 if not x.startswith("_") and x not in self.skip_params
             }
@@ -365,15 +391,15 @@
 
     @property
     def parameter_help(self):
         """str: Parameter help for the func, including execution control."""
         exec_dict_param = [
             p
             for p in NumpyDocString(self.exec_control_doc)["Parameters"]
-            if p.name == "execution_control"
+            if p.name in {"execution_control", "log_directory", "log_level"}
         ]
         param_only_doc = NumpyDocString("")
         param_only_doc["Parameters"] = exec_dict_param + [
             p
             for doc in self.docs
             for p in doc["Parameters"]
             if p.name in self.template_config
@@ -448,24 +474,24 @@
         )
     return PIPELINE_CONFIG_DOC.format(**format_inputs)
 
 
 def _batch_command_help():
     """Generate batch command help from a sample config."""
     template_config = {
-        "pipeline_config": FunctionDocumentation.REQUIRED_TAG,
+        "pipeline_config": CommandDocumentation.REQUIRED_TAG,
         "sets": [
             {
-                "args": FunctionDocumentation.REQUIRED_TAG,
-                "files": FunctionDocumentation.REQUIRED_TAG,
+                "args": CommandDocumentation.REQUIRED_TAG,
+                "files": CommandDocumentation.REQUIRED_TAG,
                 "set_tag": "set1",
             },
             {
-                "args": FunctionDocumentation.REQUIRED_TAG,
-                "files": FunctionDocumentation.REQUIRED_TAG,
+                "args": CommandDocumentation.REQUIRED_TAG,
+                "files": CommandDocumentation.REQUIRED_TAG,
                 "set_tag": "set2",
             },
         ],
     }
     sample_args_dict = {
         "args": {
             "input_constant_1": [18.02, 19.04],
@@ -517,7 +543,15 @@
         )
         if "json" in name:
             format_inputs[name] = "\n".join(
                 format_inputs[name].split("\n")[1:-1]
             ).lstrip()
 
     return BATCH_CONFIG_DOC.format(**format_inputs)
+
+
+def _as_functions(functions):
+    """Yield items from input, converting all classes to their init funcs"""
+    for func in functions:
+        if isclass(func):
+            func = func.__init__
+        yield func
```

### Comparing `NREL-gaps-0.2.1/gaps/cli/execution.py` & `NREL-gaps-0.3.0/gaps/cli/execution.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from gaps.hpc import submit
 from gaps.status import (
     DT_FMT,
     Status,
     HardwareOption,
     StatusOption,
     StatusField,
+    QOSOption,
 )
 from gaps.warnings import gapsWarning
 from gaps.exceptions import gapsConfigError
 
 logger = logging.getLogger(__name__)
 
 
@@ -54,20 +55,20 @@
     hardware_option = HardwareOption(exec_kwargs.pop("option", "local"))
     if hardware_option.manager is None:
         _kickoff_local_job(ctx, cmd)
         return
 
     ctx.obj["MANAGER"] = hardware_option.manager
     exec_kwargs = _filter_exec_kwargs(
-        exec_kwargs, hardware_option.manager.make_script_str
+        exec_kwargs, hardware_option.manager.make_script_str, hardware_option
     )
     _kickoff_hpc_job(ctx, cmd, **exec_kwargs)
 
 
-def _filter_exec_kwargs(kwargs, func):
+def _filter_exec_kwargs(kwargs, func, hardware_option):
     """Filter out extra keywords and raise error if any are missing."""
     sig = signature(func)
     kwargs_to_use = {
         k: v for k, v in kwargs.items() if k in sig.parameters.keys()
     }
     extra_keys = set(kwargs) - set(kwargs_to_use)
     if extra_keys:
@@ -85,14 +86,28 @@
     if missing:
         msg = (
             f"The 'execution_control' block is missing the following "
             f"required keys: {missing}"
         )
         raise gapsConfigError(msg)
 
+    if hardware_option.supports_categorical_qos:
+        qos = kwargs_to_use.get("qos", "normal")
+        try:
+            qos = QOSOption(qos)
+        except ValueError as err:
+            msg = (
+                f"Requested Quality-of-service option ({qos!r}) not "
+                f"recognized! Available options are: "
+                f"{QOSOption.members_as_str()}."
+            )
+            raise gapsConfigError(msg) from err
+
+        kwargs_to_use["qos"] = f"{qos}"
+
     return kwargs_to_use
 
 
 def _kickoff_local_job(ctx, cmd):
     """Run a job (command) locally."""
 
     if not _should_run(ctx):
@@ -137,15 +152,16 @@
     Status.mark_job_as_submitted(
         ctx.obj["OUT_DIR"],
         command=ctx.obj["COMMAND_NAME"],
         job_name=name,
         replace=True,
         job_attrs={
             StatusField.JOB_ID: out,
-            StatusField.HARDWARE: HardwareOption.SLURM,
+            StatusField.HARDWARE: HardwareOption.EAGLE,
+            StatusField.QOS: kwargs.get("qos") or QOSOption.UNSPECIFIED,
             StatusField.JOB_STATUS: StatusOption.SUBMITTED,
             StatusField.TIME_SUBMITTED: dt.datetime.now().strftime(DT_FMT),
         },
     )
     logger.info(msg)
```

### Comparing `NREL-gaps-0.2.1/gaps/cli/pipeline.py` & `NREL-gaps-0.3.0/gaps/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/cli/preprocessing.py` & `NREL-gaps-0.3.0/gaps/cli/preprocessing.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/cli/status.py` & `NREL-gaps-0.3.0/gaps/cli/status.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 # -*- coding: utf-8 -*-
 """GAPs Status Monitor"""
+import datetime as dt
 from pathlib import Path
 from warnings import warn
 from itertools import chain
 
 import click
 import psutil
+import pandas as pd
 from colorama import init, Fore, Style
 from tabulate import tabulate
 
-from gaps.status import Status, StatusField, StatusOption, _elapsed_time_as_str
+from gaps.status import (
+    DT_FMT,
+    Status,
+    StatusField,
+    StatusOption,
+    HardwareOption,
+    QOSOption,
+    _elapsed_time_as_str,
+)
 from gaps.warnings import gapsWarning
 from gaps.cli.command import _WrappedCommand
 
 
 FAILURE_STRINGS = ["failure", "fail", "failed", "f"]
 RUNNING_STRINGS = ["running", "run", "r"]
 SUBMITTED_STRINGS = ["submitted", "submit", "sb", "pending", "pend", "p"]
@@ -37,14 +47,22 @@
 STATUS_HELP = """
 Display the status of a project FOLDER.
 
 By default, the status of the current working directory is displayed.
 """
 
 
+def _extract_qos_charge_factor(option, enum_class):
+    """Get the charge factor of a value in a row"""
+    try:
+        return enum_class(str(option)).charge_factor
+    except ValueError:
+        return 1
+
+
 def _filter_df_for_status(df, status_request):
     """Check for a specific status."""
 
     filter_statuses = set()
     for request in status_request:
         request = request.lower()
         if request in FAILURE_STRINGS:
@@ -93,14 +111,16 @@
         extras = "; ".join(extras)
         extras = f" ({extras})"
     else:
         extras = ""
 
     pid = df.monitor_pid
     total_runtime_seconds = df.total_runtime_seconds
+    total_aus_used = int(df.total_aus_used)
+    walltime = df.walltime
     name = f"\n{Fore.CYAN}{print_folder}{extras}{Style.RESET_ALL}:"
     job_status = StatusField.JOB_STATUS
     df[job_status.value] = df[job_status].apply(color_string)
     df = df.fillna("--")
     pdf = tabulate(
         df,
         showindex=True,  # cspell:disable-line
@@ -118,17 +138,26 @@
         )
         # TODO: make prettier
         # divider = "".join(["-"] * len(runtime_str))
         # divider = "".join(["~"] * 3)
         divider = ""
         print(divider)
         print(f"{Style.BRIGHT}{runtime_str}{Style.RESET_ALL}")
+        if walltime > 2:
+            walltime_str = (
+                f"Total project time (including queue): "
+                f"{_elapsed_time_as_str(walltime)}"
+            )
+            print(f"{Style.BRIGHT}{walltime_str}{Style.RESET_ALL}")
+        if total_aus_used > 0:
+            au_str = f"Total AUs spent: {total_aus_used:,}"
+            print(f"{Style.BRIGHT}{au_str}{Style.RESET_ALL}")
         print(
-            f"{Style.BRIGHT}**Statistics only include shown jobs, excluding "
-            f"failed or duplicate runs**{Style.RESET_ALL}"
+            f"{Style.BRIGHT}**Statistics only include shown jobs (excluding "
+            f"any previous runs)**{Style.RESET_ALL}"
         )
     print()
 
 
 def main_monitor(folder, commands, status, include):
     """Run the appropriate monitor functions for a folder.
 
@@ -157,18 +186,42 @@
         include_with_runtime = list(include) + [StatusField.RUNTIME_SECONDS]
         df = pipe_status.as_df(
             commands=commands, include_cols=include_with_runtime
         )
         if status:
             df = _filter_df_for_status(df, status)
 
-        total_runtime = df[StatusField.RUNTIME_SECONDS].sum()
+        run_times_seconds = df[StatusField.RUNTIME_SECONDS]
+        hardware_charge_factors = df[StatusField.HARDWARE].apply(
+            _extract_qos_charge_factor, enum_class=HardwareOption
+        )
+        qos_charge_factors = df[StatusField.QOS].apply(
+            _extract_qos_charge_factor, enum_class=QOSOption
+        )
+        aus_used = (
+            run_times_seconds
+            / 3600
+            * hardware_charge_factors
+            * qos_charge_factors
+        )
         df = df[list(df.columns)[:-1]]
         df.monitor_pid = pipe_status.get(StatusField.MONITOR_PID)
-        df.total_runtime_seconds = total_runtime
+        df.total_runtime_seconds = run_times_seconds.sum()
+        df.total_aus_used = aus_used.sum()
+
+        start_time = df[StatusField.TIME_SUBMITTED].fillna(
+            dt.datetime.now().strftime(DT_FMT)
+        )
+        start_time = pd.to_datetime(start_time, format=DT_FMT).min()
+
+        end_time = df[StatusField.TIME_END].fillna(
+            dt.datetime.now().strftime(DT_FMT)
+        )
+        end_time = pd.to_datetime(end_time, format=DT_FMT).max()
+        df.walltime = (end_time - start_time).total_seconds()
         _color_print(df, directory.name, commands, status)
 
 
 def status_command():
     """A status CLI command."""
     filter_help = FILTER_HELP.format(
         fail_options=" ".join([f"``{s}``" for s in FAILURE_STRINGS]),
```

### Comparing `NREL-gaps-0.2.1/gaps/cli/templates.py` & `NREL-gaps-0.3.0/gaps/cli/templates.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/collection.py` & `NREL-gaps-0.3.0/gaps/collection.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/config.py` & `NREL-gaps-0.3.0/gaps/config.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/exceptions.py` & `NREL-gaps-0.3.0/gaps/exceptions.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/hpc.py` & `NREL-gaps-0.3.0/gaps/hpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,14 +347,15 @@
 
     def make_script_str(
         self,
         name,
         cmd,
         allocation,
         walltime,
+        qos=None,
         memory=None,
         queue=None,
         feature=None,
         stdout_path=DEFAULT_STDOUT_PATH,
         conda_env=None,
         sh_script=None,
     ):
@@ -367,41 +368,48 @@
         cmd :  str
             Command to be submitted in PBS shell script. Example:
                 'python -m reV.generation.cli_gen'
         allocation : str
             HPC allocation account. Example: 'rev'.
         walltime : int | float
             Node walltime request in hours. Example: 4.
+        qos : str, optional
+            Quality of service string for job. By default, `None`.
         memory : int , optional
             Node memory request in GB. By default, `None`.
         queue : str
             HPC queue to submit job to. Examples include: 'debug',
             'short', 'batch', 'batch-h', 'long', etc. By default,
             `None`, which uses `test_queue`.
         feature : str, optional
             PBS feature request (-l {feature}). Example:
-            'feature=24core', 'qos=high', etc... By default, `None`.
+            'feature=24core'. *Do not use this input for QOS. Use the
+            ``qos`` arg instead.* By default, `None`.
         stdout_path : str, optional
             Path to print .stdout and .stderr files.
             By default, :attr:`DEFAULT_STDOUT_PATH`.
         conda_env : str, optional
             Conda environment to activate. By default, `None`.
         sh_script : str, optional
             Script to run before executing command. By default, `None`.
 
         Returns
         -------
         str
             PBS script to submit.
         """
         features = [
-            str(feature).replace(" ", "") if feature else "",
+            str(feature).replace(" ", "")
+            if feature and "qos" not in feature
+            else "",
             f"walltime={format_walltime(walltime)}" if walltime else "",
             f"mem={memory}gb" if memory else "",
         ]
+        if qos:
+            features += [f"qos={qos}"]
         features = ",".join(filter(None, features))
         script_args = [
             "#!/bin/bash",
             f"#PBS -N {name} # job name",
             f"#PBS -A {allocation} # allocation account",
             f"#PBS -q {queue} # queue" if queue else "",
             # cspell:disable-next-line
@@ -464,14 +472,15 @@
 
     def make_script_str(
         self,
         name,
         cmd,
         allocation,
         walltime,
+        qos="normal",
         memory=None,
         feature=None,
         stdout_path=DEFAULT_STDOUT_PATH,
         conda_env=None,
         sh_script=None,
     ):
         """Generate the SLURM submission script.
@@ -483,19 +492,25 @@
         cmd : str
             Command to be submitted in SLURM shell script. Example:
                 'python -m reV.generation.cli_gen'
         allocation : str
             HPC allocation account. Example: 'rev'.
         walltime : int | float
             Node walltime request in hours. Example: 4.
+        qos : {"normal", "high"}
+            Quality of service specification for job. Jobs with "high"
+            priority will be charged at 2x the rate. By default,
+            ``"normal"``.
         memory : int , optional
             Node memory request in GB. By default, `None`.
         feature : str, optional
-            Additional flags for SLURM job. Format is "--qos=high"
-            or "--depend=[state:job_id]". By default, `None`.
+            Additional flags for SLURM job. Format is
+            "--partition=debug" or "--depend=[state:job_id]".
+            *Do not use this input to specify QOS. Use the ``qos`` input
+            instead.* By default, `None`.
         stdout_path : str, optional
             Path to print .stdout and .stderr files.
             By default, :attr:`DEFAULT_STDOUT_PATH`.
         conda_env : str, optional
             Conda environment to activate. By default, `None`.
         sh_script : str, optional
             Script to run before executing command. By default, `None`.
@@ -512,14 +527,15 @@
             "#!/bin/bash",
             f"#SBATCH --account={allocation}" if allocation else "",
             f"#SBATCH --time={walltime}" if walltime else "",
             f"#SBATCH --job-name={name}  # job name",
             "#SBATCH --nodes=1  # number of nodes",
             f"#SBATCH --output={stdout_path}/{name}_%j.o",
             f"#SBATCH --error={stdout_path}/{name}_%j.e",
+            f"#SBATCH --qos={qos}",
             f"#SBATCH {feature}  # extra feature" if feature else "",
             f"#SBATCH --mem={memory}  # node RAM in MB" if memory else "",
             format_env(conda_env),
             # cspell:disable-next-line
             "echo Running on: $HOSTNAME, Machine Type: $MACHTYPE",
             "echo Running python in directory `which python`",
             sh_script,
```

### Comparing `NREL-gaps-0.2.1/gaps/legacy.py` & `NREL-gaps-0.3.0/gaps/legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 import gaps.status
 import gaps.pipeline
 import gaps.hpc
 
 
 logger = logging.getLogger(__name__)
 
+_HARDWARE_MAP = {
+    "local": "local",
+    "eagle": "eagle",
+    "peregrine": "peregrine",
+    "kestrel": "kestrel",
+    "slurm": "kestrel",
+    "pbs": "peregrine",
+}
+
 
 class PipelineError(Exception):
     """Error for pipeline execution failure."""
 
 
 # pylint: disable=too-few-public-methods
 class HardwareStatusRetriever(gaps.status.HardwareStatusRetriever):
@@ -32,15 +41,17 @@
             slurm, local. Defaults to "slurm".
         subprocess_manager : PBS | SLURM | None, optional
             Optional initialized subprocess manager to use to check job
             statuses. This can be input with cached queue data to avoid
             constantly querying the HPC. By default, `None`.
         """
         super().__init__(subprocess_manager)
-        self.hardware = gaps.status._validate_hardware(hardware)
+        self.hardware = gaps.status._validate_hardware(
+            _HARDWARE_MAP.get(hardware.lower(), hardware)
+        )
 
     def __getitem__(self, key):
         """Get the job status using pre-defined hardware-specific methods."""
         job_id, __ = key
         if not job_id:
             return None
 
@@ -82,15 +93,17 @@
             constantly querying the HPC.
 
         Returns
         -------
         status : str | None
             Status string or None if job/module not found.
         """
-        hsr = HardwareStatusRetriever(hardware, subprocess_manager)
+        hsr = HardwareStatusRetriever(
+            _HARDWARE_MAP.get(hardware.lower(), hardware), subprocess_manager
+        )
         return cls(status_dir)._retrieve_job_status(module, job_name, hsr)
 
     @classmethod
     def add_job(
         cls, status_dir, module, job_name, replace=False, job_attrs=None
     ):
         """Add a job to status json.
```

### Comparing `NREL-gaps-0.2.1/gaps/log.py` & `NREL-gaps-0.3.0/gaps/log.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/pipeline.py` & `NREL-gaps-0.3.0/gaps/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/project_points.py` & `NREL-gaps-0.3.0/gaps/project_points.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/status.py` & `NREL-gaps-0.3.0/gaps/status.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,49 +32,55 @@
 class StatusField(CaseInsensitiveEnum):
     """A collection of required status fields in a status file."""
 
     JOB_ID = "job_id"
     JOB_STATUS = "job_status"
     PIPELINE_INDEX = "pipeline_index"
     HARDWARE = "hardware"
+    QOS = "qos"
     OUT_FILE = "out_file"
     TIME_SUBMITTED = "time_submitted"
     TIME_START = "time_start"
     TIME_END = "time_end"
     TOTAL_RUNTIME = "total_runtime"
     RUNTIME_SECONDS = "runtime_seconds"
     MONITOR_PID = "monitor_pid"
 
 
 class HardwareOption(CaseInsensitiveEnum):
     """A collection of hardware options."""
 
     LOCAL = "local"
-    SLURM = "slurm"
+    KESTREL = "kestrel"
     EAGLE = "eagle"
     PEREGRINE = "peregrine"
-    PBS = "pbs"
 
     @classmethod
     def _new_post_hook(cls, obj, value):
         """Hook for post-processing after __new__"""
         obj.is_hpc = value != "local"
-        if value in {"slurm", "eagle"}:
+        if value in {"eagle", "kestrel"}:
             obj.manager = SLURM()
             obj.check_status_using_job_id = (
                 obj.manager.check_status_using_job_id
             )
-        elif value in {"pbs", "peregrine"}:
+            obj.supports_categorical_qos = True
+            obj.charge_factor = 3
+        elif value in {"peregrine"}:
             obj.manager = PBS()
             obj.check_status_using_job_id = (
                 obj.manager.check_status_using_job_id
             )
+            obj.supports_categorical_qos = False
+            obj.charge_factor = 1
         else:
             obj.manager = None
             obj.check_status_using_job_id = lambda *__, **___: None
+            obj.supports_categorical_qos = False
+            obj.charge_factor = 0
         return obj
 
 
 class StatusOption(CaseInsensitiveEnum):
     """A collection of job status options."""
 
     NOT_SUBMITTED = "not submitted"
@@ -89,14 +95,31 @@
         """Hook for post-processing after __new__"""
         verb = "has" if value == "failed" else "is"
         obj.with_verb = " ".join([verb, value])
         obj.is_processing = value in {"submitted", "running"}
         return obj
 
 
+class QOSOption(CaseInsensitiveEnum):
+    """A collection of job QOS options."""
+
+    NORMAL = "normal"
+    HIGH = "high"
+    UNSPECIFIED = "unspecified"
+
+    @classmethod
+    def _new_post_hook(cls, obj, value):
+        """Hook for post-processing after __new__"""
+        if value in {"high"}:
+            obj.charge_factor = 2
+        else:
+            obj.charge_factor = 1
+        return obj
+
+
 # pylint: disable=too-few-public-methods
 class HardwareStatusRetriever:
     """Query hardware for job status."""
 
     def __init__(self, subprocess_manager=None):
         """Initialize `HardwareStatusRetriever`.
 
@@ -133,14 +156,15 @@
         StatusField.PIPELINE_INDEX.value,
         StatusField.JOB_ID.value,
         StatusField.TIME_SUBMITTED.value,
         StatusField.TIME_START.value,
         StatusField.TIME_END.value,
         StatusField.TOTAL_RUNTIME.value,
         StatusField.HARDWARE.value,
+        StatusField.QOS.value,
     ]
 
     def __init__(self, status_dir):
         """Initialize `Status`.
 
         Parameters
         ----------
@@ -233,15 +257,15 @@
     def reload(self):
         """Re-load the data from disk."""
         self.data = _load(self._fpath)
 
     def dump(self):
         """Dump status json w/ backup file in case process gets killed."""
 
-        self._fpath.parent.mkdir(exist_ok=True)
+        self._fpath.parent.mkdir(parents=True, exist_ok=True)
 
         backup = self._fpath.name.replace(".json", "_backup.json")
         backup = self._fpath.parent / backup
         if self._fpath.exists():
             shutil.copy(self._fpath, backup)
 
         with open(self._fpath, "w") as status:
@@ -685,14 +709,15 @@
         ~status_df[StatusField.TIME_START].isna()
         & status_df[StatusField.TIME_END].isna()
     )
     start_times = status_df.loc[mask, StatusField.TIME_START]
     start_times = pd.to_datetime(start_times, format=DT_FMT)
     elapsed_times = dt.datetime.now() - start_times
     elapsed_times = elapsed_times.apply(lambda dt: dt.total_seconds())
+    status_df.loc[mask, StatusField.RUNTIME_SECONDS] = elapsed_times
     elapsed_times = elapsed_times.apply(_elapsed_time_as_str)
     elapsed_times = elapsed_times.apply(lambda time_str: f"{time_str} (r)")
     status_df.loc[mask, StatusField.TOTAL_RUNTIME] = elapsed_times
     return status_df
 
 
 def _load(fpath):
```

### Comparing `NREL-gaps-0.2.1/gaps/utilities.py` & `NREL-gaps-0.3.0/gaps/utilities.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.2.1/gaps/warnings.py` & `NREL-gaps-0.3.0/gaps/warnings.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,7 +18,11 @@
 
 class gapsCollectionWarning(gapsWarning):
     """gaps Collection waring."""
 
 
 class gapsHPCWarning(gapsWarning):
     """gaps HPC warning."""
+
+
+class gapsDeprecationWarning(gapsWarning, DeprecationWarning):
+    """gaps deprecation warning."""
```

### Comparing `NREL-gaps-0.2.1/setup.py` & `NREL-gaps-0.3.0/setup.py`

 * *Files identical despite different names*


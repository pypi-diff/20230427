# Comparing `tmp/countess-0.0.22.tar.gz` & `tmp/countess-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.22.tar", last modified: Thu Apr 13 06:54:52 2023, max compression
+gzip compressed data, was "countess-0.0.24.tar", last modified: Thu Apr 27 04:26:41 2023, max compression
```

## Comparing `countess-0.0.22.tar` & `countess-0.0.24.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.581817 countess-0.0.22/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.22/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-13 06:54:52.581817 countess-0.0.22/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-04-13 01:06:20.000000 countess-0.0.22/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.569817 countess-0.0.22/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-04-13 01:06:30.000000 countess-0.0.22/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.569817 countess-0.0.22/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.22/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-03-01 01:42:03.000000 countess-0.0.22/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4271 2023-03-02 01:10:40.000000 countess-0.0.22/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1755 2023-03-30 03:12:18.000000 countess-0.0.22/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    14810 2023-04-11 06:55:31.000000 countess-0.0.22/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5289 2023-04-13 04:45:45.000000 countess-0.0.22/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    14246 2023-04-13 06:53:19.000000 countess-0.0.22/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.581817 countess-0.0.22/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-02-23 03:33:35.000000 countess-0.0.22/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    19707 2023-04-13 06:53:19.000000 countess-0.0.22/countess/gui/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5855 2023-04-13 05:47:03.000000 countess-0.0.22/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    33604 2023-04-13 06:53:20.000000 countess-0.0.22/countess/gui/main.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.581817 countess-0.0.22/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-02-23 03:33:47.000000 countess-0.0.22/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6110 2023-04-13 06:53:19.000000 countess-0.0.22/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1303 2023-04-11 06:55:31.000000 countess-0.0.22/countess/plugins/embed_python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1800 2023-04-11 06:55:31.000000 countess-0.0.22/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1465 2023-04-11 06:55:31.000000 countess-0.0.22/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1781 2023-04-11 06:55:31.000000 countess-0.0.22/countess/plugins/hdf5.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3107 2023-04-13 06:53:19.000000 countess-0.0.22/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      343 2023-03-06 22:57:42.000000 countess-0.0.22/countess/plugins/log_score.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5592 2023-04-13 06:53:19.000000 countess-0.0.22/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6953 2023-04-13 06:53:19.000000 countess-0.0.22/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2243 2023-04-13 06:53:19.000000 countess-0.0.22/countess/plugins/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.581817 countess-0.0.22/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.22/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2133 2023-04-11 06:55:31.000000 countess-0.0.22/countess/utils/dask.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     9681 2023-04-13 05:33:29.000000 countess-0.0.22/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.569817 countess-0.0.22/countess.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      931 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      238 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-04-13 06:54:52.000000 countess-0.0.22/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2365 2023-04-12 05:45:07.000000 countess-0.0.22/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)     1444 2023-04-13 06:54:52.581817 countess-0.0.22/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-02-28 22:32:19.000000 countess-0.0.22/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-13 06:54:52.581817 countess-0.0.22/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      636 2023-02-28 22:34:37.000000 countess-0.0.22/tests/test_gui.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.596055 countess-0.0.24/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.24/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-27 04:26:41.596055 countess-0.0.24/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-04-26 02:32:05.000000 countess-0.0.24/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.592055 countess-0.0.24/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-04-26 02:31:56.000000 countess-0.0.24/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.592055 countess-0.0.24/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.24/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-04-21 06:08:37.000000 countess-0.0.24/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4271 2023-04-21 06:08:37.000000 countess-0.0.24/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-04-21 06:08:37.000000 countess-0.0.24/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    15736 2023-04-26 23:25:45.000000 countess-0.0.24/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5024 2023-04-21 06:08:37.000000 countess-0.0.24/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13178 2023-04-26 23:25:45.000000 countess-0.0.24/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.592055 countess-0.0.24/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.24/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    21779 2023-04-26 02:38:33.000000 countess-0.0.24/countess/gui/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-04-26 02:29:55.000000 countess-0.0.24/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    33190 2023-04-26 23:25:45.000000 countess-0.0.24/countess/gui/main.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.596055 countess-0.0.24/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.24/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5795 2023-04-26 02:38:33.000000 countess-0.0.24/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1194 2023-04-26 02:29:55.000000 countess-0.0.24/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2038 2023-04-26 03:33:35.000000 countess-0.0.24/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4145 2023-04-26 02:38:33.000000 countess-0.0.24/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-04-26 02:29:55.000000 countess-0.0.24/countess/plugins/hdf5.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3051 2023-04-26 02:38:33.000000 countess-0.0.24/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-04-26 02:29:55.000000 countess-0.0.24/countess/plugins/log_score.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5520 2023-04-26 02:38:33.000000 countess-0.0.24/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6776 2023-04-26 23:25:45.000000 countess-0.0.24/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2200 2023-04-26 02:38:33.000000 countess-0.0.24/countess/plugins/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.596055 countess-0.0.24/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.24/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     9717 2023-04-26 02:29:55.000000 countess-0.0.24/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.592055 countess-0.0.24/countess.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      906 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      784 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      237 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2415 2023-04-27 04:26:35.000000 countess-0.0.24/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1444 2023-04-27 04:26:41.596055 countess-0.0.24/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-04-21 06:08:37.000000 countess-0.0.24/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.596055 countess-0.0.24/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      636 2023-04-21 06:08:37.000000 countess-0.0.24/tests/test_gui.py
```

### Comparing `countess-0.0.22/LICENSE.txt` & `countess-0.0.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.22/PKG-INFO` & `countess-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.22
+Version: 0.0.24
 Summary: CountESS
 Author: CountESS Developers
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer: Nick Moore
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.22
+# CountESS 0.0.24
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.22/README.md` & `countess-0.0.24/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.22
+# CountESS 0.0.24
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.22/countess/core/cmd.py` & `countess-0.0.24/countess/core/cmd.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.22/countess/core/config.py` & `countess-0.0.24/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.22/countess/core/logger.py` & `countess-0.0.24/countess/core/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Logger base classes"""
 
 import sys
+import traceback
 from typing import Optional
 
 
 class Logger:
     """Logger Base Class"""
 
     def __init__(self):
@@ -26,14 +27,17 @@
         """Log a message at level warning"""
         self.log("warning", message, detail)
 
     def error(self, message: str, detail: Optional[str] = None):
         """Log a message at level error"""
         self.log("error", message, detail)
 
+    def exception(self, exception: Exception):
+        self.error(str(exception), detail="".join(traceback.format_exception(exception)))
+
     def clear(self):
         """Clear logs (if possible)"""
         return None
 
 
 class ConsoleLogger(Logger):
     """A simple Logger which sends output to stdout and stderr"""
```

### Comparing `countess-0.0.22/countess/core/parameters.py` & `countess-0.0.24/countess/core/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 class BaseParam:
     """Represents the parameters which can be set on a plugin."""
 
     label: str = ""
     value: Any = None
+    hide: bool = False
 
     def copy(self):
         """Plugins declare their parameters with instances of BaseParam, these
         need to be copied so that multiple Plugins (and multiple rows in an
         ArrayParam) can have distinct values"""
         raise NotImplementedError(f"Implement {self.__class__.__name__}.copy()")
 
@@ -326,14 +327,18 @@
     def set_choices(self, choices: Iterable[str]):
         super().set_choices([self.NONE_VALUE] + list(choices))
 
     def is_none(self):
         return self.value == self.NONE_VALUE
 
 
+class MultipleChoiceParam(ChoiceParam):
+    pass
+
+
 class ArrayParam(BaseParam):
     """An ArrayParam contains zero or more copies of `param`, which can be a
     SimpleParam or a MultiParam."""
 
     # XXX the only real use for this is as an array of MultiParams so I think
     # maybe we should have a TabularParam which combines ArrayParam and
     # MultiParam more directly."""
@@ -430,14 +435,33 @@
 
     def set_column_choices(self, choices):
         self.param.set_column_choices(choices)
         for p in self.params:
             p.set_column_choices(choices)
 
 
+class PerColumnArrayParam(ArrayParam):
+    def __init__(self, *a, **k) -> None:
+        super().__init__(*a, **k)
+        self.params_by_column_name: Mapping[str, BaseParam] = {}
+        self.read_only = True
+
+    def set_column_choices(self, choices):
+        self.params = [None] * len(choices)
+        for num, name in enumerate(choices):
+            if name not in self.params_by_column_name:
+                self.params_by_column_name[name] = self.param.copy()
+            self.params[num] = self.params_by_column_name[name]
+            self.params[num].label = f'Column {num+1}: "{name}"'
+            self.params[num].set_column_choices(choices)
+        for name in list(self.params_by_column_name.keys()):
+            if name not in choices:
+                del self.params_by_column_name[name]
+
+
 class FileArrayParam(ArrayParam):
     """FileArrayParam is an ArrayParam arranged per-file.  Using this class
     really just marks it as expecting to be populated from an open file
     dialog."""
 
     def find_fileparam(self):
         if isinstance(self.param, FileParam):
@@ -519,7 +543,11 @@
         for k, p in self.params.items():
             digest.update((k + "\0" + p.get_hash_value()).encode("utf-8"))
         return digest.hexdigest()
 
     def set_column_choices(self, choices):
         for p in self.params.values():
             p.set_column_choices(choices)
+
+
+class TabularMultiParam(MultiParam):
+    pass
```

### Comparing `countess-0.0.22/countess/core/pipeline.py` & `countess-0.0.24/countess/core/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import traceback
 from dataclasses import dataclass, field
 from typing import Any, Optional
 
 from countess.core.logger import Logger
 from countess.core.plugins import BasePlugin, get_plugin_classes
 
 PRERUN_ROW_LIMIT = 10000
@@ -36,38 +35,33 @@
         if len(self.parent_nodes) == 0:
             return None
         elif len(self.parent_nodes) == 1:
             return list(self.parent_nodes)[0].result
         else:
             return dict((n.name, n.result) for n in self.parent_nodes if n.result is not None)
 
-    def exception_logger(self, exception, logger: Logger):
-        logger.error(str(exception), detail="".join(traceback.format_exception(exception)))
-
     def execute(self, logger: Logger, row_limit=None):
         assert row_limit is None or isinstance(row_limit, int)
         input_data = self.get_input_data()
         if self.plugin:
             try:
                 self.result = self.plugin.run(input_data, logger, row_limit)
             except Exception as exc:  # pylint: disable=W0718
-                self.result = None
-                self.exception_logger(exc, logger)
+                logger.exception(exc)
         else:
             self.result = input_data
 
     def prepare(self, logger: Logger):
         assert isinstance(logger, Logger)
         input_data = self.get_input_data()
         if self.plugin:
             try:
                 self.plugin.prepare(input_data, logger)
             except Exception as exc:  # pylint: disable=W0718
-                self.result = None
-                self.exception_logger(exc, logger)
+                logger.exception(exc)
         else:
             self.result = input_data
 
     def prerun(self, logger: Logger, row_limit=PRERUN_ROW_LIMIT):
         assert isinstance(logger, Logger)
         if self.is_dirty and self.plugin:
             for parent_node in self.parent_nodes:
```

### Comparing `countess-0.0.22/countess/core/plugins.py` & `countess-0.0.24/countess/core/plugins.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,31 +19,28 @@
 import importlib.metadata
 import logging
 import os.path
 import sys
 from collections.abc import Mapping, MutableMapping
 from typing import Any, List, Optional
 
-import dask.dataframe as dd
 import numpy as np
 import pandas as pd
-from dask.callbacks import Callback
 
 from countess.core.logger import Logger
 from countess.core.parameters import (
     ArrayParam,
     BaseParam,
     ChoiceParam,
     FileArrayParam,
     FileParam,
     FileSaveParam,
     MultiParam,
     StringParam,
 )
-from countess.utils.dask import concat_dataframes, crop_dataframe, empty_dask_dataframe
 
 PRERUN_ROW_LIMIT = 100
 
 
 def get_plugin_classes():
     plugin_classes = set()
     for ep in importlib.metadata.entry_points(group="countess_plugins"):
@@ -103,14 +100,20 @@
 
     def prepare(self, data: Any, logger: Logger):
         """The plugin gets a preview version of its input data so it can
         check types, column names, etc.  Should throw an exception if this
         isn't a suitable data input."""
         return True
 
+    def update(self):
+        """Notify the plugin that one or more of its parameters have been changed.
+        If this change affects other parameters, it can return True to indicate that
+        all parameters should be re-displayed"""
+        return False
+
     def run(
         self,
         data: Any,
         logger: Logger,
         row_limit: Optional[int] = None,
     ):
         """Plugins which support progress monitoring should override this
@@ -183,146 +186,129 @@
         row_limit: Optional[int] = None,
     ):
         df = self.load_files(logger, row_limit)
 
         return df
 
 
-class DaskProgressCallback(Callback):
-    """Matches Dask's idea of a progress callback to our logger class."""
-
-    def __init__(self, logger: Logger):
-        super().__init__()
-        self.logger = logger
-        self.total_tasks = None
-
-    def _start_state(self, dsk, state):  # pylint: disable=method-hidden
-        self.total_tasks = len(state["ready"]) + len(state["waiting"])
-
-    def _posttask(self, key, result, dsk, state, worker_id):  # pylint: disable=method-hidden
-        self.logger.progress("Running", 100 * len(state["finished"]) // self.total_tasks)
-
-    def _finish(self, dsk, state, failed):  # pylint: disable=method-hidden
-        # XXX do something with "failed"
-        self.logger.progress("Done", 100)
+def crop_dataframe(df: pd.DataFrame, row_limit: Optional[int]):
+    if row_limit is None:
+        return df
+    return df[0:row_limit]
 
 
-class DaskBasePlugin(BasePlugin):
-    """Base class for plugins which accept and return dask/pandas DataFrames"""
+class PandasBasePlugin(BasePlugin):
+    """Base class for plugins which accept and return pandas DataFrames"""
 
     def run(
         self,
         data: Any,
         logger: Logger,
         row_limit: Optional[int] = None,
     ):
         raise NotImplementedError(f"{self.__class__}.run()")
 
 
-class DaskTransformPlugin(DaskBasePlugin):
+class PandasTransformPlugin(PandasBasePlugin):
     input_columns: list[str] = []
 
-    def prepare_dask(self, df: dd.DataFrame | pd.DataFrame, logger: Logger):
-        assert isinstance(df, (pd.DataFrame, dd.DataFrame))
-        self.input_columns = sorted(df.columns)
+    def prepare_df(self, df: pd.DataFrame, logger: Logger):
+        assert isinstance(df, pd.DataFrame)
+        self.input_columns = list(df.columns)
 
         for p in self.parameters.values():
             p.set_column_choices(self.input_columns)
 
     # XXX prepare and run handle multiple inputs differntly?
 
     def prepare(
         self,
-        data: pd.DataFrame | dd.DataFrame | Mapping[str, pd.DataFrame | dd.DataFrame],
+        data: pd.DataFrame | Mapping[str, pd.DataFrame],
         logger: Logger,
     ) -> bool:
         if isinstance(data, Mapping):
-            data = concat_dataframes(data.values())
+            data = pd.concat(data.values())
 
-        return self.prepare_dask(data, logger)
+        return self.prepare_df(data, logger)
 
-    def run_dask(
-        self, df: pd.DataFrame | dd.DataFrame, logger: Logger
-    ) -> pd.DataFrame | dd.DataFrame:
-        raise NotImplementedError(f"Implement {self.__class__.__name__}.run_dask()")
+    def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
+        raise NotImplementedError(f"Implement {self.__class__.__name__}.run_df()")
 
     def run(
         self,
-        data: pd.DataFrame | dd.DataFrame | Mapping[str, pd.DataFrame | dd.DataFrame],
+        data: pd.DataFrame | Mapping[str, pd.DataFrame],
         logger: Logger,
         row_limit: Optional[int] = None,
-    ) -> pd.DataFrame | dd.DataFrame:
+    ) -> pd.DataFrame:
         assert isinstance(logger, Logger)
         assert row_limit is None or isinstance(row_limit, int)
 
-        with DaskProgressCallback(logger):
-            logger.progress("Starting", 0)
-            if isinstance(data, Mapping):
-                dfs = []
-                for obj in data.values():
-                    assert isinstance(obj, (pd.DataFrame, dd.DataFrame))
-                    df = self.run_dask(obj, logger)
-                    assert isinstance(df, (pd.DataFrame, dd.DataFrame))
-                    dfs.append(crop_dataframe(df, row_limit))
-                logger.progress("Finished", 100)
-                return concat_dataframes(dfs)
-            else:
-                assert isinstance(data, (pd.DataFrame, dd.DataFrame))
-                df = self.run_dask(data, logger)
-                assert isinstance(df, (pd.DataFrame, dd.DataFrame))
-                logger.progress("Finished", 100)
-                return crop_dataframe(df, row_limit)
+        logger.progress("Starting", 0)
+        if isinstance(data, Mapping):
+            dfs = []
+            for obj in data.values():
+                assert isinstance(obj, pd.DataFrame)
+                df = self.run_df(obj, logger)
+                assert isinstance(df, pd.DataFrame)
+                dfs.append(crop_dataframe(df, row_limit))
+            logger.progress("Finished", 100)
+            return pd.concat(dfs)
+        else:
+            assert isinstance(data, pd.DataFrame)
+            df = self.run_df(data, logger)
+            assert isinstance(df, pd.DataFrame)
+            logger.progress("Finished", 100)
+            return crop_dataframe(df, row_limit)
 
 
 # XXX Potentially there's a PandasBasePlugin which can use a technique much
 # like tqdm does in tqdm/std.py to monkeypatch pandas.apply and friends and
 # provide progress feedback.
 
 
-class DaskInputPlugin(FileInputMixin, DaskBasePlugin):
-    """A specialization of the DaskBasePlugin to allow it to follow nothing,
+class PandasInputPlugin(FileInputMixin, PandasBasePlugin):
+    """A specialization of the PandasBasePlugin to allow it to follow nothing,
     eg: come first."""
 
     def __init__(self, *a, **k):
         # Add in filenames
         super().__init__(*a, **k)
         file_params = {"filename": FileParam("Filename", file_types=self.file_types)}
         file_params.update(self.file_params)
 
         self.parameters = dict(
             [("files", FileArrayParam("Files", MultiParam("File", file_params)))]
             + list(self.parameters.items())
         )
 
-    def combine_dfs(self, dfs: list[pd.DataFrame | dd.DataFrame]) -> dd.DataFrame | pd.DataFrame:
+    def combine_dfs(self, dfs: list[pd.DataFrame]) -> pd.DataFrame:
         """First stage: collect all the files together in whatever
         way is appropriate.  Override this to do it differently
         or do more work on the dataframes (eg: counting, renaming, etc)"""
-        return concat_dataframes(dfs)
+        return pd.concat(dfs)
 
     def load_files(
         self,
         logger: Logger,
         row_limit: Optional[int] = None,
-    ) -> pd.DataFrame | dd.DataFrame:
+    ) -> pd.DataFrame:
         assert isinstance(self.parameters["files"], ArrayParam)
         fps = self.parameters["files"].params
         if not fps:
-            return empty_dask_dataframe()
+            return pd.DataFrame()
 
         if len(fps) == 1:
-            with DaskProgressCallback(logger):
-                file_param = self.parameters["files"].params[0]
-                assert isinstance(file_param, MultiParam)
-                ddf = self.read_file_to_dataframe(file_param, logger, row_limit)
-                ddf = self.combine_dfs([ddf])
+            file_param = self.parameters["files"].params[0]
+            assert isinstance(file_param, MultiParam)
+            ddf = self.read_file_to_dataframe(file_param, logger, row_limit)
+            ddf = self.combine_dfs([ddf])
         else:
             num_files = len(fps)
             # Input plugins are likely I/O bound so if there's more than one
-            # file, instead of using the Dask progress callback mechanism
+            # file, instead of using the Pandas progress callback mechanism
             # this uses a simple count of files read."""
             per_file_row_limit = int(row_limit / len(fps) + 1) if row_limit else None
             logger.progress("Loading", 0)
             dfs = []
             for num, fp in enumerate(fps):
                 assert isinstance(fp, MultiParam)
                 df = self.read_file_to_dataframe(fp, logger, per_file_row_limit)
@@ -332,19 +318,19 @@
             ddf = self.combine_dfs(dfs)
             logger.progress("Done", 100)
 
         return ddf
 
     def read_file_to_dataframe(
         self, file_params: MultiParam, logger: Logger, row_limit: Optional[int] = None
-    ) -> dd.DataFrame | pd.DataFrame:
+    ) -> pd.DataFrame:
         raise NotImplementedError(f"Implement {self.__class__.__name__}.read_file_to_dataframe")
 
 
-class DaskScoringPlugin(DaskTransformPlugin):
+class PandasScoringPlugin(PandasTransformPlugin):
     """Specific kind of transform which turns counts into scores"""
 
     # XXX not really useful?
 
     max_counts = 5
 
     parameters = {
@@ -359,53 +345,49 @@
                     ),
                 },
             ),
             min_size=1,
         )
     }
 
-    def prepare_dask(self, df, logger):
+    def prepare_df(self, df, logger):
         super().prepare(df, logger)
         for pp in self.parameters["scores"]:
             for ppp in pp.counts:
                 ppp.choices = self.input_columns
 
-    def run_dask(
-        self, df: pd.DataFrame | dd.DataFrame, logger: Logger
-    ) -> pd.DataFrame | dd.DataFrame:
+    def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
         assert isinstance(self.parameters["scores"], ArrayParam)
         score_cols = []
         for pp in self.parameters["scores"]:
             scol = pp.score.value
             ccols = [ppp.value for ppp in pp.counts]
 
             if scol and all(ccols):
                 df[scol] = self.score([df[col] for col in ccols])
                 score_cols.append(scol)
 
         df = df.replace([np.inf, -np.inf], np.nan)
-        assert isinstance(df, (pd.DataFrame, dd.DataFrame))
+        assert isinstance(df, pd.DataFrame)
         df.dropna(how="all", subset=score_cols, inplace=True)
         return df
 
-    def score(self, columns: List[dd.Series]) -> dd.Series:
-        raise NotImplementedError("Subclass DaskScoringPlugin and provide a score() method")
+    def score(self, columns: List[pd.Series]) -> pd.Series:
+        raise NotImplementedError("Subclass PandasScoringPlugin and provide a score() method")
 
 
-class DaskReindexPlugin(DaskTransformPlugin):
+class PandasReindexPlugin(PandasTransformPlugin):
     # XXX not really useful?
 
     translate_type = str
 
     def translate(self, value):
         raise NotImplementedError(f"Implement {self.__class__.__name__}.translate")
 
     def translate_row(self, row):
         return self.translate(row.name)
 
-    def run_dask(
-        self, df: pd.DataFrame | dd.DataFrame, logger: Logger
-    ) -> pd.DataFrame | dd.DataFrame:
+    def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
         df["__reindex"] = df.apply(
             self.translate_row, axis=1, meta=pd.Series(self.translate_type())
         )
         return df.groupby("__reindex").sum()
```

### Comparing `countess-0.0.22/countess/gui/config.py` & `countess-0.0.24/countess/gui/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # TK based GUI for CountESS
 import math
 import tkinter as tk
 from functools import partial
 from tkinter import filedialog, ttk
-from typing import Mapping, Optional
+from typing import Mapping, MutableMapping, Optional
 
-import dask.dataframe as dd
 import numpy as np
 import pandas as pd
+from pandas.api.types import is_numeric_dtype  # type: ignore
 
 from ..core.parameters import (
     ArrayParam,
     BaseParam,
     BooleanParam,
     ChoiceParam,
     FileArrayParam,
     FileParam,
     FileSaveParam,
     FloatParam,
     IntegerParam,
     MultiParam,
     SimpleParam,
+    TabularMultiParam,
     TextParam,
 )
 from ..core.plugins import BasePlugin
-from ..utils.dask import crop_dataframe
 
 UNICODE_CHECK = "\u2714"
 UNICODE_UNCHECK = "\u2717"
 UNICODE_CROSS = "\u2715"
 UNICODE_PLUS = "\u2795"
 
 
@@ -58,28 +58,29 @@
         self.subwrapper_buttons: list[tk.Button] = []
 
         self.subwrappers: Mapping[BaseParam, ParameterWrapper] = {}
 
         self.var: Optional[tk.Variable] = None
         self.entry: Optional[tk.Widget] = None
         self.label: Optional[tk.Widget] = None
+        self.row_labels: list[tk.Widget] = []
 
         if isinstance(parameter, ArrayParam):
             self.label = None
         else:
             self.label = ttk.Label(tk_parent, text=parameter.label)
 
         if isinstance(parameter, ChoiceParam):
             self.var = tk.StringVar(tk_parent, value=parameter.value)
             self.entry = ttk.Combobox(tk_parent, textvariable=self.var)
             self.entry["values"] = parameter.choices
-            self.entry.state(["readonly"])
+            self.entry.state(["readonly"])  # don't allow other options
         elif isinstance(parameter, BooleanParam):
             self.entry = tk.Button(tk_parent, width=2, command=self.toggle_checkbox_callback)
-            self.set_checkbox_value(parameter.value)
+            self.set_checkbox_value()
         elif isinstance(parameter, FileParam):
             self.var = tk.StringVar(tk_parent, value=parameter.value)
             self.entry = ttk.Entry(tk_parent, textvariable=self.var)
             self.entry.state(["readonly"])
             self.button = tk.Button(
                 tk_parent, text="Select", width=3, command=self.change_file_callback
             )
@@ -101,44 +102,53 @@
             else:
                 self.var = tk.StringVar(tk_parent, value=parameter.value)
 
             self.entry = ttk.Entry(tk_parent, textvariable=self.var)
             if parameter.read_only:
                 self.entry.state(["readonly"])
 
-        elif isinstance(parameter, ArrayParam) and self.level == 0:
+        elif (
+            isinstance(parameter, ArrayParam)
+            and self.level == 0
+            and not isinstance(parameter.param, TabularMultiParam)
+        ):
             self.entry = ttk.Frame(tk_parent)
             self.entry.columnconfigure(0, weight=1)
             drc = self.delete_row_callback if not parameter.read_only else None
             self.update_subwrappers_framed(parameter.params, drc)
             if not parameter.read_only:
                 self.button = tk.Button(
                     self.entry,
                     text=f"Add {parameter.param.label}",
                     command=self.add_row_callback,
                 )
                 self.button.grid(row=len(parameter.params) + 1)
 
-        elif isinstance(parameter, ArrayParam) and self.level < 3:
+        elif isinstance(parameter, ArrayParam) and (
+            self.level < 3 or isinstance(parameter.param, TabularMultiParam)
+        ):
             label_frame_label = tk.Frame(tk_parent)
             tk.Label(label_frame_label, text=parameter.label).grid(row=0, column=0, padx=5)
             self.entry = tk.LabelFrame(tk_parent, labelwidget=label_frame_label, padx=10, pady=5)
-            self.button = tk.Button(
-                label_frame_label,
-                text=UNICODE_PLUS,
-                width=2,
-                command=self.add_row_callback,
-            )
-            self.button.grid(row=0, column=1, padx=10)
+            if not parameter.read_only:
+                self.button = tk.Button(
+                    label_frame_label,
+                    text=UNICODE_PLUS,
+                    width=2,
+                    command=self.add_row_callback,
+                )
+                self.button.grid(row=0, column=1, padx=10)
 
             drc = self.delete_row_callback if not parameter.read_only else None
             if isinstance(parameter.param, MultiParam):
                 for n, pp in enumerate(parameter.param.values()):
-                    tk.Label(self.entry, text=pp.label).grid(row=0, column=n, sticky=tk.EW, padx=10)
-                    self.entry.columnconfigure(n, weight=1)
+                    tk.Label(self.entry, text=pp.label).grid(
+                        row=0, column=n + 1, sticky=tk.EW, padx=10
+                    )
+                    self.entry.columnconfigure(n + 1, weight=1)
 
                 self.update_subwrappers_tabular(parameter.params, drc)
             else:
                 self.entry.columnconfigure(0, weight=0)
                 self.entry.columnconfigure(1, weight=0)
                 self.entry.columnconfigure(2, weight=1)
 
@@ -176,42 +186,66 @@
                 command=lambda: delete_callback(self),
             )
 
         if not isinstance(parameter, BooleanParam):
             self.entry.grid(sticky=tk.EW, padx=10, pady=5)
 
     def update(self):
-        if isinstance(self.parameter, ArrayParam) and self.level == 0:
+        if self.parameter.hide:
+            self.entry["fg"] = self.entry["bg"]
+        else:
+            self.entry["fg"] = None
+
+        if (
+            isinstance(self.parameter, ArrayParam)
+            and self.level == 0
+            and not isinstance(self.parameter.param, TabularMultiParam)
+        ):
             self.update_subwrappers_framed(self.parameter.params, self.delete_row_callback)
             if self.button:
                 self.button.grid(row=len(self.parameter.params) + 1, padx=10)
         elif (
             isinstance(self.parameter, ArrayParam)
             and isinstance(self.parameter.param, MultiParam)
             and self.level < 3
         ):
-            self.update_subwrappers_tabular(self.parameter.params, self.delete_row_callback)
+            self.update_subwrappers_tabular(
+                self.parameter.params,
+                self.delete_row_callback if not self.parameter.read_only else None,
+            )
         elif isinstance(self.parameter, ArrayParam):
-            self.update_subwrappers(self.parameter.params, self.delete_row_callback)
+            self.update_subwrappers(
+                self.parameter.params,
+                self.delete_row_callback if not self.parameter.read_only else None,
+            )
             if self.button:
                 self.button["state"] = (
                     tk.DISABLED
                     if self.parameter.max_size is not None
                     and len(self.subwrappers) >= self.parameter.max_size
                     else tk.NORMAL
                 )
         elif isinstance(self.parameter, MultiParam):
             self.update_subwrappers(self.parameter.params.values(), None)
+        elif isinstance(self.parameter, ChoiceParam):
+            self.entry["values"] = self.parameter.choices
+        elif isinstance(self.parameter, BooleanParam):
+            self.set_checkbox_value()
+        elif isinstance(self.parameter, TextParam):
+            if self.parameter.read_only:
+                self.entry["state"] = "normal"
+            self.entry.replace("1.0", tk.END, self.parameter.value)
+            if self.parameter.read_only:
+                self.entry["state"] = "disabled"
+        else:
+            self.var.set(self.parameter.value)
 
         if self.label:
             self.label["text"] = self.parameter.label
 
-        if isinstance(self.parameter, ChoiceParam):
-            self.entry["values"] = self.parameter.choices
-
     def cull_subwrappers(self, params):
         params_set = set(params)
         for p, pw in self.subwrappers.items():
             if p not in params_set:
                 pw.destroy()
 
     def update_subwrappers(self, params, delete_row_callback):
@@ -230,36 +264,44 @@
 
         self.cull_subwrappers(params)
 
     def update_subwrappers_tabular(self, params, delete_row_callback):
         while self.subwrapper_buttons:
             self.subwrapper_buttons.pop().destroy()
 
+        for rl in self.row_labels:
+            rl.destroy()
+        self.row_labels = []
+
         for n, p in enumerate(params):
+            row_label = tk.Label(self.entry, text=p.label)
+            row_label.grid(row=n + 1, column=0, padx=10)
+            self.row_labels.append(row_label)
+
             subparams = p.params.values()
             for m, pp in enumerate(subparams):
                 if pp in self.subwrappers:
                     self.subwrappers[pp].update()
                 else:
                     self.subwrappers[pp] = ParameterWrapper(
                         self.entry,
                         pp,
                         self.callback,
                         delete_row_callback,
                         level=self.level + 1,
                     )
-                self.subwrappers[pp].entry.grid(row=n + 1, column=m, padx=10)
+                self.subwrappers[pp].entry.grid(row=n + 1, column=m + 1, padx=10)
             if delete_row_callback:
                 button = tk.Button(
                     self.entry,
                     text=UNICODE_CROSS,
                     width=2,
                     command=partial(delete_row_callback, self, n),
                 )
-                button.grid(row=n + 1, column=len(subparams), padx=10)
+                button.grid(row=n + 1, column=len(subparams) + 1, padx=10)
                 self.subwrapper_buttons.append(button)
 
         self.cull_subwrappers([pp for p in params for pp in p.params.values()])
 
     def update_subwrappers_framed(self, params, delete_row_callback):
         for n, p in enumerate(params):
             if p in self.subwrappers:
@@ -323,14 +365,15 @@
         if self.callback is not None:
             self.callback(self.parameter)
 
         self.update()
 
     def delete_row_callback(self, parameter_wrapper, row=None):
         assert isinstance(self.parameter, ArrayParam)
+
         if row is not None:
             self.parameter.del_row(row)
         else:
             self.parameter.del_subparam(parameter_wrapper.parameter)
 
         self.update()
         if self.callback is not None:
@@ -359,26 +402,38 @@
     def widget_modified_callback(self, *_):
         # only gets called the *first* time a modification happens, unless
         # we reset the flag which says a change has happened ...
         value = self.entry.get(1.0, tk.END)
         self.entry.edit_modified(False)
         self.set_value(value)
 
-    def set_checkbox_value(self, value):
-        if value:
+    def set_checkbox_value(self):
+        if self.parameter.hide:
+            self.entry["text"] = ""
+            self.entry["fg"] = self.entry["bg"]
+            self.entry["state"] = tk.DISABLED
+            self.entry["bd"] = 0
+        elif self.parameter.value:
             self.entry["text"] = UNICODE_CHECK
             self.entry["fg"] = "black"
+            self.entry["state"] = tk.NORMAL
+            self.entry["bd"] = 1
         else:
             self.entry["text"] = UNICODE_UNCHECK
             self.entry["fg"] = "grey"
+            self.entry["state"] = tk.NORMAL
+            self.entry["bd"] = 1
 
     def toggle_checkbox_callback(self, *_):
+        if self.parameter.read_only or self.parameter.hide:
+            # XXX warn?
+            return
         value = not self.parameter.value
         self.parameter.value = value
-        self.set_checkbox_value(value)
+        self.set_checkbox_value()
         if self.callback is not None:
             self.callback(self.parameter)
 
     def clear_value_callback(self, *_):
         self.set_value("")
 
     def destroy(self):
@@ -396,31 +451,32 @@
         self.plugin = plugin
         self.change_callback = change_callback
 
         self.frame = ttk.Frame(tk_parent)
         self.frame.columnconfigure(0, weight=1)
         self.frame.grid(sticky=tk.NSEW)
 
-        self.wrapper_cache: Mapping[str, ParameterWrapper] = {}
+        self.wrapper_cache: MutableMapping[str, ParameterWrapper] = {}
 
         self.subframe = ttk.Frame(self.frame)
         self.subframe.columnconfigure(0, weight=0)
         self.subframe.columnconfigure(1, weight=0)
         self.subframe.columnconfigure(2, weight=1)
         self.subframe.grid(row=1, sticky=tk.NSEW)
 
         self.update()
 
     def change_parameter(self, parameter):
         """Called whenever a parameter gets changed"""
-        self.update()
+        if self.plugin.update():
+            self.update()
         if self.change_callback:
             self.change_callback(self)
 
-    def update(self):
+    def update(self) -> None:
         # If there's only a single parameter it is presented a little differently.
         top_level = 0 if len(self.plugin.parameters) == 1 else 1
 
         # Create any new parameter wrappers needed & update existing ones
         for n, (key, parameter) in enumerate(self.plugin.parameters.items()):
             if key in self.wrapper_cache:
                 self.wrapper_cache[key].update()
@@ -439,17 +495,18 @@
 
 class DataFramePreview:
     """Provides a visual preview of a Dask dataframe arranged as a table."""
 
     # XXX uses a treeview, which seemed like a good match but actually a grid-layout
     # of custom styled labels might work better.
 
-    def __init__(self, tk_parent, ddf: Optional[dd.DataFrame] = None):
+    def __init__(self, tk_parent, ddf: Optional[pd.DataFrame] = None, max_rows: int = 10000):
         self.frame = ttk.Frame(tk_parent)
         self.label = ttk.Label(self.frame, text="DataFrame Preview")
+        self.max_rows = max_rows
 
         self.treeview = ttk.Treeview(self.frame, selectmode=tk.NONE)
 
         self.scrollbar_x = ttk.Scrollbar(
             self.frame, orient=tk.HORIZONTAL, command=self.treeview.xview
         )
         self.scrollbar_y = ttk.Scrollbar(
@@ -466,34 +523,31 @@
         self.treeview.grid(row=1, column=0, sticky=tk.NSEW)
         self.scrollbar_x.grid(row=2, column=0, sticky=tk.EW)
         self.scrollbar_y.grid(row=1, column=1, stick=tk.NS)
 
         if ddf is not None:
             self.update(ddf)
 
-    def update(self, ddf: pd.DataFrame | dd.DataFrame):
-        if len(ddf) > 1000:
-            self.label["text"] = f"DataFrame Preview (1000 rows out of {len(ddf)})"
-            ddf = crop_dataframe(ddf, 1000)
+    def update(self, ddf: pd.DataFrame):
+        if len(ddf) > self.max_rows:
+            self.label["text"] = f"DataFrame Preview ({self.max_rows} rows out of {len(ddf)})"
+            ddf = ddf[0:1000]
         else:
             self.label["text"] = f"DataFrame Preview {len(ddf)} rows"
 
         # XXX could handle multiindex columns more elegantly than this
         # (but maybe not in a ttk.Treeview)
-        column_names = [".".join(c) if isinstance(c, tuple) else c for c in ddf.columns]
-        column_types = [dt.kind for dt in ddf.dtypes]
+        column_names = ["__".join(c) if isinstance(c, tuple) else c for c in ddf.columns]
 
         self.treeview["columns"] = column_names
 
-        for n, cn in enumerate(column_names):
-            self.treeview.heading(n, text=cn)
-
-        for n, ct in enumerate(column_types):
+        for n, (column_name, column_dtype) in enumerate(zip(column_names, ddf.dtypes)):
+            self.treeview.heading(n, text=f"{column_name} ({column_dtype.name})")
             # XXX it'd be nicer if we could do "real" decimal point alignment
-            anchor = tk.E if ct in ("i", "f") else tk.W
+            anchor = tk.E if is_numeric_dtype(column_dtype) else tk.W
             # XXX type signature appears to be wrong, or at least overly restrictive.
             # I think I'm going to replace treeview anyway so I'm ignoring it for now.
             self.treeview.column(
                 n, anchor=anchor, width=100, minwidth=100, stretch=tk.YES
             )  # type: ignore
 
         for row in self.treeview.get_children():
```

### Comparing `countess-0.0.22/countess/gui/logger.py` & `countess-0.0.24/countess/gui/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,21 +74,24 @@
         return TreeviewLogger(self.treeview, self.progress_frame, name)
 
 
 class TreeviewDetailWindow(tk.Toplevel):
     def __init__(self, detail, *a, **k):
         super().__init__(*a, **k)
 
+        self.rowconfigure(0, weight=1)
+        self.columnconfigure(0, weight=1)
+
         text = tk.Text(self)
         text.insert("1.0", detail)
         text["state"] = "disabled"
-        text.pack(anchor=tk.CENTER)
+        text.grid(sticky=tk.NSEW)
 
         button = tk.Button(self, text="CLOSE", command=self.destroy)
-        button.pack()
+        button.grid(sticky=tk.EW)
 
 
 class TreeviewLogger(Logger):
     def __init__(self, treeview: ttk.Treeview, progress_frame: tk.Frame, name: str):
         self.treeview = treeview
         self.progress_bar = LabeledProgressbar(progress_frame, mode="determinate", value=0)
         self.progress_bar.update_label(name)
```

### Comparing `countess-0.0.22/countess/gui/main.py` & `countess-0.0.24/countess/gui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import random
 import re
 import sys
 import tkinter as tk
 import webbrowser
 from enum import Enum, IntFlag
 from functools import partial
-from tkinter import filedialog, messagebox, ttk
+from tkinter import filedialog, font, messagebox, ttk
 from typing import Optional
 
-import dask.dataframe as dd
 import pandas as pd
 
 from countess import VERSION
 from countess.core.config import export_config_graphviz, read_config, write_config
 from countess.core.logger import ConsoleLogger
 from countess.core.pipeline import PipelineGraph, PipelineNode
 from countess.core.plugins import get_plugin_classes
@@ -91,22 +90,23 @@
         self["cursor"] = TkCursors.HAND.value
 
     def __on_button(self, event):
         if event.state & TkEventState.CONTROL or event.num == 3:
             self.__state = self.__state.LINK_WAIT
         else:
             self.__state = self.__state.DRAG_WAIT
-        self.after(500, self.__on_timeout)
+        self.after(100, self.__on_timeout)
 
     def __place(self, event=None):
+        x, y, w, h = _geometry(self)
+        x = x + (event.x if event else (w // 2))
+        y = y + (event.y if event else (h // 2))
         return {
-            "relx": (self.winfo_x() + (event.x if event else self.winfo_width() // 2))
-            / self.master.winfo_width(),
-            "rely": (self.winfo_y() + (event.y if event else self.winfo_height() // 2))
-            / self.master.winfo_height(),
+            "relx": _limit( x / self.master.winfo_width(), 0.05, 0.95),
+            "rely": _limit( y / self.master.winfo_height(), 0.05, 0.95),
             "anchor": "c",
         }
 
     def __on_timeout(self):
         if self.__state == self.__state.DRAG_WAIT:
             self.__state = self.__state.DRAGGING
             self["cursor"] = TkCursors.ARROWS.value
@@ -174,73 +174,52 @@
         x2, y2, w2, h2 = _geometry(self.widget2)
 
         # special case for dragging invisible frames
         # XXX bit of a hack just to get it to look nice
         if w2 == 1 and h2 == 1:
             x2, y2, w2, h2 = x2 - 20, y2 - 20, 40, 40
 
-        # If there's enough room, extra control points set
-        # up a nice spline, and a little extra padding
+        # Control points set up a nice spline, and a little extra padding
         # on the destination end to allow for the arrow head.
         _xc, _yc, wc, hc = _geometry(self.canvas)
 
         if wc > hc:
             if self.switch and x1 > x2:
                 x1, y1, w1, h1, x2, y2, w2, h2 = x2, y2, w2, h2, x1, y1, w1, h1
-            if 0 < x2 - (x1 + w1) < 50:
-                coords = (
-                    x1 + w1,
-                    y1 + h1 // 2,
-                    x2 - 20,
-                    y2 + h2 // 2,
-                    x2,
-                    y2 + h2 // 2,
-                )
-            else:
-                coords = (
-                    x1 + w1,
-                    y1 + h1 // 2,
-                    x1 + w1 + 20,
-                    y1 + h1 // 2,
-                    x2 - 40,
-                    y2 + h2 // 2,
-                    x2,
-                    y2 + h2 // 2,
-                )
+            coords = (
+                x1 + w1,
+                y1 + h1 // 2,
+                x1 + w1 + 20,
+                y1 + h1 // 2,
+                x2 - 40,
+                y2 + h2 // 2,
+                x2,
+                y2 + h2 // 2,
+            )
         else:
             if self.switch and y1 > y2:
                 x1, y1, w1, h1, x2, y2, w2, h2 = x2, y2, w2, h2, x1, y1, w1, h1
-            if 0 < y2 - (y1 + h1) < 50:
-                coords = (
-                    x1 + w1 // 2,
-                    y1 + h1,
-                    x2 + w2 // 2,
-                    y2 - 20,
-                    x2 + w2 // 2,
-                    y2,
-                )
-            else:
-                coords = (
-                    x1 + w1 // 2,
-                    y1 + h1,
-                    x1 + w1 // 2,
-                    y1 + h1 + 20,
-                    x2 + w2 // 2,
-                    y2 - 40,
-                    x2 + w2 // 2,
-                    y2,
-                )
+            coords = (
+                x1 + w1 // 2,
+                y1 + h1,
+                x1 + w1 // 2,
+                y1 + h1 + 20,
+                x2 + w2 // 2,
+                y2 - 40,
+                x2 + w2 // 2,
+                y2,
+            )
 
         if self.line:
             self.canvas.coords(self.line, *coords)
             self.canvas.itemconfig(self.line, smooth=len(coords) > 6)
         else:
             self.line = self.canvas.create_line(
                 *coords,
-                smooth=len(coords) > 6,
+                smooth=True,
                 width=3,
                 arrow="last",
                 arrowshape=(15, 15, 6),
                 fill=self.color,
             )
 
     def destroy(self):
@@ -328,14 +307,15 @@
             for parent_node, connecting_line in lines_for_child.items()
         )
 
         self.canvas.bind("<Button-1>", self.on_canvas_button1)
         self.canvas.bind("<Button-3>", self.on_canvas_button3)
         self.canvas.bind("<Motion>", self.on_canvas_motion)
         self.canvas.bind("<Leave>", self.on_canvas_leave)
+        self.canvas.bind("<Key-Delete>", self.on_canvas_delete)
 
     def label_for_node(self, node):
         label = DraggableLabel(
             self.canvas, text=node.name, wraplength=125, cursor="hand1", takefocus=True
         )
         if not node.position:
             node.position = (random.random() * 0.8 + 0.1, random.random() * 0.8 + 0.1)
@@ -377,24 +357,18 @@
             self.canvas.delete(self.highlight_rectangle)
             self.highlight_rectangle = None
         self.highlight_node(node)
         self.node_select_callback(node)
 
     def on_configure(self, node, event):
         """Stores the updated position of the label in node.position"""
-        place_info = event.widget.place_info()
-        # XXX should be more elegant way of answering the question "are we flipped?"
-        width = self.canvas.winfo_width()
-        height = self.canvas.winfo_height()
-        if width > height:
-            node.position = (float(place_info["relx"]), float(place_info["rely"]))
-        else:
-            node.position = (float(place_info["rely"]), float(place_info["relx"]))
+        node.position = self.new_node_position(event.x, event.y)
 
         # Adapt label sizes to suit the window size, as best we can ...
+        width = self.canvas.winfo_width()
         label_max_width = max(width // 10, 25)
         label_font_size = int(math.sqrt(width) / math.pi)
         for label in self.labels.values():
             label["wraplength"] = label_max_width
             label["font"] = ("TkDefaultFont", label_font_size)
 
     def on_enter(self, node, event):
@@ -412,58 +386,64 @@
             x - 3, y - 3, x + w + 3, y + h + 3, fill="red", width=0
         )
 
     def on_leave(self, node, event):
         if self.highlight_rectangle is not None:
             self.canvas.delete(self.highlight_rectangle)
             self.highlight_rectangle = None
+        self.canvas.focus_set()
 
     def on_canvas_motion(self, event):
         """Show a preview of line selection when the cursor is over line(s)"""
         items = self.canvas.find_overlapping(event.x - 10, event.y - 10, event.x + 10, event.y + 10)
         for connecting_line, _, _ in self.lines_lookup.values():
             color = "red" if connecting_line.line in items else "black"
             self.canvas.itemconfig(connecting_line.line, fill=color)
 
     def on_canvas_leave(self, event):
         """Called when the mouse leaves the canvas *OR* the mouse enters
         any of the labels, to clear the line selection preview."""
         for connecting_line, _, _ in self.lines_lookup.values():
             self.canvas.itemconfig(connecting_line.line, fill="black")
 
+    def new_node_position(self, x, y):
+        flipped = self.canvas.winfo_height() > self.canvas.winfo_width()
+        xp = _limit(x / self.canvas.winfo_width(), 0.05, 0.95)
+        yp = _limit(y / self.canvas.winfo_height(), 0.05, 0.95)
+        return (yp, xp) if flipped else (xp,yp)
+
     def on_canvas_button1(self, event):
+        pass
+
+    def on_canvas_button3(self, event):
         """Click to create a new node, if it is created on top of a line
         that line is broken and the node is included."""
 
         items = self.canvas.find_overlapping(event.x - 10, event.y - 10, event.x + 10, event.y + 10)
 
         # XXX creating a new node every time you click on the background
         # is proving quite annoying.  Lets see how it is to go without it.
         # (you can still create a new node by button-3-dragging from an
         # existing node, and if you really want a disconnected graph you can
         # delete the link to the new node!)
-        if not items:
-            return
+        #if not items:
+        #    return
 
-        position = (
-            event.x / self.canvas.winfo_width(),
-            event.y / self.canvas.winfo_height(),
-        )
+        position = self.new_node_position(event.x, event.y)
         new_node = self.add_new_node(position)
 
         for item in items:
             _, child_node, parent_node = self.lines_lookup[item]
             self.del_parent(parent_node, child_node)
             self.add_parent(new_node, child_node)
             self.add_parent(parent_node, new_node)
 
-    def on_canvas_button3(self, event):
+    def on_canvas_delete(self, event):
         """Button3 on canvas: delete line(s)."""
         items = self.canvas.find_overlapping(event.x - 10, event.y - 10, event.x + 10, event.y + 10)
-
         for item in items:
             _, child_node, parent_node = self.lines_lookup[item]
             self.del_parent(parent_node, child_node)
 
     def on_delete(self, node, event):
         """<Delete> disconnects a node from the graph, connects it parents to its children,
         and deletes the node.  <Shift-Delete> removes and deletes the node, but doesn't
@@ -520,38 +500,33 @@
         if select:
             self.highlight_node(new_node)
             self.node_select_callback(new_node)
         return new_node
 
     def on_ghost_release(self, start_node, event):
         xl, yl, _wl, _hl = _geometry(event.widget)
+        flipped = self.canvas.winfo_height() > self.canvas.winfo_width()
         other_node = self.find_node_at_position(event.x + xl, event.y + yl)
         if other_node is None:
-            position = (event.x + xl) / self.canvas.winfo_width(), (
-                event.y + yl
-            ) / self.canvas.winfo_height()
+            position = self.new_node_position(event.x+xl,event.y+yl)
             other_node = self.add_new_node(position)
         elif other_node == start_node:
             return
         elif start_node in other_node.parent_nodes:
             other_node.del_parent(start_node)
             return
         elif other_node in start_node.parent_nodes:
             start_node.del_parent(other_node)
             return
 
         if start_node.is_ancestor_of(other_node):
             self.add_parent(start_node, other_node)
         elif other_node.is_ancestor_of(start_node):
             self.add_parent(other_node, start_node)
-        elif (
-            (event.x > 0)
-            if self.canvas.winfo_width() > self.canvas.winfo_height()
-            else (event.y > 0)
-        ):
+        elif (flipped and event.y > 0) or (not flipped and event.x > 0):
             self.add_parent(start_node, other_node)
         else:
             self.add_parent(other_node, start_node)
 
         self.highlight_node(other_node)
         self.node_select_callback(other_node)
 
@@ -615,15 +590,18 @@
         self.notes_widget.bind("<<Modified>>", self.notes_modified_callback)
 
         self.logger_subframe = LoggerFrame(self.frame)
         self.logger = self.logger_subframe.get_logger(node.name)
 
         self.show_config_subframe()
         if self.node.plugin:
-            self.show_preview_subframe()
+            if self.node.is_dirty:
+                self.config_change_callback()
+            else:
+                self.show_preview_subframe()
 
     def show_config_subframe(self):
         if self.config_subframe:
             self.config_subframe.destroy()
         self.node.prepare(self.logger)
         if self.node.plugin:
             self.label["text"] = "%s %s — %s" % (
@@ -632,14 +610,16 @@
                 self.node.plugin.description,
             )
             if self.node.plugin.link:
                 tk.Button(
                     self.frame, text=UNICODE_INFO, fg="blue", command=self.on_info_button_press
                 ).grid(row=1, column=1, sticky=tk.SE, padx=10)
             self.notes_widget.grid(row=2, columnspan=2, sticky=tk.EW, padx=10, pady=5)
+            self.node.prepare(self.logger)
+            self.node.plugin.update()
             self.configurator = PluginConfigurator(
                 self.frame, self.node.plugin, self.config_change_callback
             )
             self.config_subframe = self.configurator.frame
         else:
             self.config_subframe = PluginChooserFrame(
                 self.frame, "Choose Plugin", self.choose_plugin
@@ -651,15 +631,15 @@
 
     def on_info_button_press(self, *_):
         webbrowser.open_new_tab(self.node.plugin.link)
 
     def show_preview_subframe(self):
         if self.preview_subframe:
             self.preview_subframe.destroy()
-        if isinstance(self.node.result, (dd.DataFrame, pd.DataFrame)):
+        if isinstance(self.node.result, pd.DataFrame):
             self.preview_subframe = DataFramePreview(self.frame, self.node.result).frame
         elif isinstance(self.node.result, str):
             self.preview_subframe = tk.Frame(self.frame)
             self.preview_subframe.rowconfigure(1, weight=1)
             n_lines = len(self.node.result.splitlines())
             tk.Label(self.preview_subframe, text=f"Text Preview {n_lines} Lines").grid(
                 sticky=tk.NSEW
@@ -881,16 +861,18 @@
             if t in themes:
                 root.set_theme(t)
     except ImportError:
         root = tk.Tk()
         # XXX some kind of ttk style setup goes here as a fallback
 
     # Set up treeview font and row heights.
+    linespace = font.Font(None, 10).metrics()["linespace"]
     style = ttk.Style()
-    style.configure("Treeview", font=(None, 10), rowheight=25)
+    style.configure("Treeview", font=(None, 10), rowheight=linespace)
+    style.configure("Treeview.Heading", font=(None, 10, "bold"), rowheight=linespace)
 
     root.title(f"CountESS {VERSION}")
     root.rowconfigure(0, weight=0)
     root.rowconfigure(1, weight=1)
     root.columnconfigure(0, weight=1)
 
     # Try to start off maximized, but this option doesn't exist
```

### Comparing `countess-0.0.22/countess/plugins/csv.py` & `countess-0.0.24/countess/plugins/csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import csv
 from io import StringIO
 from typing import Any, Optional
 
-import dask.dataframe as dd
 import pandas as pd
 
 from countess import VERSION
 from countess.core.parameters import (
     ArrayParam,
     BooleanParam,
     ChoiceParam,
     DataTypeOrNoneChoiceParam,
     FileSaveParam,
     MultiParam,
     StringParam,
 )
-from countess.core.plugins import DaskBasePlugin, DaskInputPlugin
+from countess.core.plugins import PandasBasePlugin, PandasInputPlugin
 
 # XXX it would be better to do the same this Regex Tool does and get the user to assign
 # data types to each column
 
 
 def maybe_number(x):
     """CSV is never clear on if something is actually a number so ... try it I guess ..."""
@@ -36,15 +35,15 @@
     return x
 
 
 def clean_row(row):
     return [maybe_number(x) for x in row]
 
 
-class LoadCsvPlugin(DaskInputPlugin):
+class LoadCsvPlugin(PandasInputPlugin):
     """Load CSV files"""
 
     name = "CSV Load"
     description = "Loads data from CSV or similar delimited text files and assigns types to columns"
     link = "https://countess-project.github.io/CountESS/plugins/#csv-reader"
     version = VERSION
 
@@ -110,15 +109,14 @@
             options["doublequote"] = False
             options["escapechar"] = "\\"
 
         comment = self.parameters["comment"].value
         if comment != "None":
             options["comment"] = comment
 
-        # XXX dd.read_csv().set_index() is very very slow!
         # XXX pd.read_csv(index_col=) is half the speed of pd.read_csv().set_index()
 
         df = pd.read_csv(filename, **options)
 
         while len(df.columns) > len(self.parameters["columns"]):
             self.parameters["columns"].add_row()
 
@@ -136,15 +134,15 @@
         ]
         if index_cols:
             df = df.set_index(index_cols)
 
         return df
 
 
-class SaveCsvPlugin(DaskBasePlugin):
+class SaveCsvPlugin(PandasBasePlugin):
     name = "CSV Save"
     description = "Save data as CSV or similar delimited text files"
     link = "https://countess-project.github.io/CountESS/plugins/#csv-writer"
     version = VERSION
 
     file_types = [("CSV", "*.csv"), ("TSV", "*.tsv"), ("TXT", "*.txt")]
 
@@ -174,19 +172,13 @@
             "sep": sep,
             "quoting": csv.QUOTE_NONNUMERIC
             if self.parameters["quoting"].value
             else csv.QUOTE_MINIMAL,
         }
 
         if row_limit is None:
-            if isinstance(data, dd.DataFrame):
-                data.to_csv(filename, single_file=True, compute=True, **options)
-            else:
-                data.to_csv(filename, **options)
+            data.to_csv(filename, **options)
             return None
         else:
-            if isinstance(data, dd.DataFrame):
-                data = data.compute()
-
             buf = StringIO()
             data.to_csv(buf, **options)
             return buf.getvalue()
```

### Comparing `countess-0.0.22/countess/plugins/embed_python.py` & `countess-0.0.24/countess/plugins/expression.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-import dask.dataframe as dd
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
-from countess.core.parameters import ArrayParam, TextParam
-from countess.core.plugins import DaskTransformPlugin
+from countess.core.parameters import TextParam
+from countess.core.plugins import PandasTransformPlugin
 
 
-def process(df: pd.DataFrame, codes):
+def process(df: pd.DataFrame, codes, logger: Logger):
     for code in codes:
-        result = df.eval(code)
-        if isinstance(result, (dd.Series, pd.Series)):
+        try:
+            result = df.eval(code)
+        except Exception as exc:  # pylint: disable=W0718
+            logger.error(str(exc))
+            continue
+
+        if isinstance(result, pd.Series):
             # this was a filter
             df = df.copy()
             df["__filter"] = result
             df = df.query("__filter != 0").drop(columns="__filter")
         else:
             # this was a column assignment
             df = result
 
     return df
 
 
-class EmbeddedPythonPlugin(DaskTransformPlugin):
-    name = "Embedded Python"
-    description = "Embed Python code into CountESS"
+class ExpressionPlugin(PandasTransformPlugin):
+    name = "Expression"
+    description = "Apply simple expressions"
     version = VERSION
 
-    parameters = {"code": ArrayParam("Code", TextParam("Code"))}
+    parameters = {"code": TextParam("Expressions")}
 
-    def run_dask(self, df, logger: Logger) -> dd.DataFrame:
-        assert isinstance(self.parameters["code"], ArrayParam)
+    def run_df(self, df, logger: Logger) -> pd.DataFrame:
+        assert isinstance(self.parameters["code"], TextParam)
 
-        codes = [
-            p.value.replace("\n", " ")
-            for p in self.parameters["code"]
-            if isinstance(p, TextParam) and p.value.strip()
-        ]
+        codes = [c.replace("\n", " ").strip() for c in self.parameters["code"].value.split("\n\n")]
 
-        if isinstance(df, dd.DataFrame):
-            return df.map_partitions(process, codes)
-        else:
-            return process(df, codes)
+        return process(df, codes, logger)
```

### Comparing `countess-0.0.22/countess/plugins/fastq.py` & `countess-0.0.24/countess/plugins/fastq.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 from itertools import islice
 
 import pandas as pd
 from fqfa.fastq.fastq import parse_fastq_reads  # type: ignore
 
 from countess import VERSION
 from countess.core.parameters import BooleanParam, FloatParam
-from countess.core.plugins import DaskInputPlugin
-from countess.utils.dask import concat_dataframes
+from countess.core.plugins import PandasInputPlugin
 
 
-class LoadFastqPlugin(DaskInputPlugin):
+class LoadFastqPlugin(PandasInputPlugin):
     """Load counts from one or more FASTQ files, by first building a dask dataframe of raw sequences
     with count=1 and then grouping by sequence and summing counts.  It supports counting
     in multiple columns."""
 
     name = "FASTQ Load"
     description = "Loads counts from FASTQ files containing either variant or barcodes"
     version = VERSION
 
     file_types = [("FASTQ", "*.fastq"), ("FASTQ (gzipped)", "*.fastq.gz")]
 
     parameters = {
-        "group": BooleanParam("Group by Sequence?", True),
         "min_avg_quality": FloatParam("Minimum Average Quality", 10),
+        "group": BooleanParam("Group by Sequence?", True),
     }
 
     def read_file_to_dataframe(self, file_params, logger, row_limit=None):
+        # XXX this should be a bit smarter than building up the entire
+        # structure in an array ...
         records = []
-        count_column_name = "count"
 
-        with open(file_params["filename"].value, "r", encoding="utf-8") as fh:
+        filename = file_params["filename"].value
+        with open(filename, "r", encoding="utf-8") as fh:
             for fastq_read in islice(parse_fastq_reads(fh), 0, row_limit):
                 if fastq_read.average_quality() >= self.parameters["min_avg_quality"].value:
-                    records.append((fastq_read.sequence, 1))
-        return pd.DataFrame.from_records(records, columns=("sequence", count_column_name))
+                    records.append((fastq_read.sequence, fastq_read.header, filename))
+
+        return pd.DataFrame.from_records(records, columns=("sequence", "header", "filename"))
 
     def combine_dfs(self, dfs):
         """first concatenate the count dataframes, then (optionally) group them by sequence"""
 
-        combined_df = concat_dataframes(dfs)
+        combined_df = pd.concat(dfs)
 
         if len(combined_df) and self.parameters["group"].value:
-            combined_df = combined_df.groupby(by=["sequence"]).sum()
+            combined_df = combined_df.groupby(by=["sequence", "filename"]).agg(
+                {"sequence": "first", "filename": "first", "header": "count"}
+            )
+            combined_df.rename({"header": "count"}, axis=1)
 
         return combined_df
```

### Comparing `countess-0.0.22/countess/plugins/hdf5.py` & `countess-0.0.24/countess/plugins/hdf5.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 from typing import Optional
 
-import dask.dataframe as dd
 import pandas as pd
 
 try:
     import tables  # type: ignore  # pylint: disable=unused-import
 except ImportError as exc:
     raise NotImplementedError("HDF5 Plugin needs Pytables") from exc
 
 from countess import VERSION
 from countess.core.parameters import ChoiceParam, MultiParam
-from countess.core.plugins import DaskInputPlugin
+from countess.core.plugins import PandasInputPlugin
 
 
-class LoadHdfPlugin(DaskInputPlugin):
+class LoadHdfPlugin(PandasInputPlugin):
     name = "HDF5 Load"
     description = "Loads counts from HDF5 files"
     version = VERSION
 
     file_types = [("HDF5 File", "*.hdf5")]
     file_params = {
         "key": ChoiceParam("HDF Key"),
     }
 
     keys: list[str] = []
 
     def read_file_to_dataframe(
         self, file_params: MultiParam, logger, row_limit: Optional[int] = None
-    ) -> pd.DataFrame | dd.DataFrame:
+    ) -> pd.DataFrame:
         kp = file_params.key
         filename = file_params.filename.value
         with pd.HDFStore(filename) as hs:
             kp.set_choices(sorted(hs.keys()))
 
         if kp.value is None:
             return pd.DataFrame([])
@@ -40,15 +39,15 @@
             df = hs.select(kp.value, start=0, stop=row_limit)
 
         assert isinstance(df, pd.DataFrame)
 
         return df
 
 
-# class StoreHdfPlugin(DaskBasePlugin):
+# class StoreHdfPlugin(PandasBasePlugin):
 #    name = "HDF Writer"
 #    description = "Write to HDF5"
 #
 #    params = {
 #        "pattern": {
 #            "label": "Filename Pattern",
 #            "type": str,
```

### Comparing `countess-0.0.22/countess/plugins/join.py` & `countess-0.0.24/countess/plugins/join.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from collections.abc import Mapping, MutableMapping
 from typing import Optional
 
-import dask.dataframe as dd
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
 from countess.core.parameters import ArrayParam, BooleanParam, ChoiceParam, MultiParam
-from countess.core.plugins import DaskBasePlugin
+from countess.core.plugins import PandasBasePlugin
 
 INDEX = "— INDEX —"
 
 
-class DaskJoinPlugin(DaskBasePlugin):
-    """Joins Dask Dataframes"""
+class JoinPlugin(PandasBasePlugin):
+    """Joins Pandas Dataframes"""
 
     name = "Join"
-    description = "Joins two Dask Dataframes by indexes or columns"
+    description = "Joins two Pandas Dataframes by indexes or columns"
     version = VERSION
 
     parameters = {
         "inputs": ArrayParam(
             "Inputs",
             MultiParam(
                 "Input",
@@ -38,15 +37,15 @@
     def prepare(self, data, logger: Logger):
         data_items = list(data.items())
         inputs_param = self.parameters["inputs"]
         assert isinstance(inputs_param, ArrayParam)
 
         if len(data_items) != 2 or len(inputs_param) != 2:
             raise NotImplementedError("Only two-way joins supported right now")
-        if not all((isinstance(df, (dd.DataFrame, pd.DataFrame)) for _, df in data_items)):
+        if not all((isinstance(df, pd.DataFrame) for _, df in data_items)):
             raise NotImplementedError("Feed me dataframes")
 
         enumerate_inputs = enumerate(zip(inputs_param, data.items()))
         for number, (input_param, (source_name, source_ddf)) in enumerate_inputs:
             input_param.label = f"Input {number+1}: {source_name}"
             input_param["join_on"].choices = [INDEX] + list(source_ddf.columns)
 
@@ -57,15 +56,15 @@
         row_limit: Optional[int] = None,
     ):
         inputs_param = self.parameters["inputs"]
         assert isinstance(inputs_param, ArrayParam)
         assert len(inputs_param) == 2
         assert isinstance(data, Mapping)
         assert len(data) == 2
-        assert all(isinstance(d, (dd.DataFrame, pd.DataFrame)) for d in data.values())
+        assert all(isinstance(d, pd.DataFrame) for d in data.values())
 
         ip1 = inputs_param[0]
         ip2 = inputs_param[1]
 
         if ip1.required.value and ip2.required.value:
             join_how = "inner"
         elif ip1.required.value:
```

### Comparing `countess-0.0.22/countess/plugins/pivot.py` & `countess-0.0.24/countess/plugins/pivot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import itertools
 from collections import defaultdict
 
-import dask.dataframe as dd
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
 from countess.core.parameters import (
     ArrayParam,
     ChoiceParam,
     ColumnChoiceParam,
     MultiParam,
     StringParam,
 )
-from countess.core.plugins import DaskTransformPlugin
+from countess.core.plugins import PandasTransformPlugin
 
 AGG_FUNCTIONS = ["first", "sum", "count", "mean"]
 
 
-class DaskPivotPlugin(DaskTransformPlugin):
-    """Groups a Dask Dataframe by an arbitrary column and rolls up rows"""
+class PivotPlugin(PandasTransformPlugin):
+    """Groups a Pandas Dataframe by an arbitrary column and rolls up rows"""
 
     name = "Pivot Tool"
     description = "Groups a dataframe and pivots column values into columns"
     version = VERSION
     link = "https://countess-project.github.io/CountESS/plugins/#pivot-tool"
 
     parameters = {
@@ -40,17 +39,15 @@
                 },
             ),
         ),
     }
 
     # XXX It'd be nice to also have "non pivoted" aggregated columns as well.
 
-    def run_dask(
-        self, df: pd.DataFrame | dd.DataFrame, logger: Logger
-    ) -> pd.DataFrame | dd.DataFrame:
+    def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
         assert isinstance(self.parameters["index"], ArrayParam)
         assert isinstance(self.parameters["pivot"], ArrayParam)
         assert isinstance(self.parameters["agg"], ArrayParam)
 
         index_cols = [
             p.value
             for p in self.parameters["index"].params
@@ -106,15 +103,15 @@
                 rename_cols = {}
                 for col, agg_op, out_col in agg_cols:
                     output_column = (out_col or col) + suffix
                     aggregate_ops[output_column].append(agg_op)
                     rename_cols[col] = output_column
 
                 dfs.append(df.query(query).rename(columns=rename_cols))
-            df = dd.concat(dfs)
+            df = pd.concat(dfs)
 
             # XXX because of the way the concat operation collects pivot groups, a bunch of records
             # end up getting generated with NULLs in integer columns, forcing those columns
             # to become floats, which looks odd for a 'sum' or 'count' operation.
         else:
             rename_cols = {}
             for col, agg_op, out_col in agg_cols:
```

### Comparing `countess-0.0.22/countess/plugins/regex.py` & `countess-0.0.24/countess/plugins/regex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import re
 from functools import partial
 
-import dask.dataframe as dd
 import pandas as pd
 
 from countess import VERSION
 from countess.core.parameters import (
     ArrayParam,
     BooleanParam,
     ColumnOrIndexChoiceParam,
     DataTypeChoiceParam,
     MultiParam,
     StringParam,
 )
-from countess.core.plugins import DaskInputPlugin, DaskTransformPlugin
-from countess.utils.dask import concat_dataframes
+from countess.core.plugins import PandasInputPlugin, PandasTransformPlugin
 
 
-class RegexToolPlugin(DaskTransformPlugin):
+class RegexToolPlugin(PandasTransformPlugin):
     name = "Regex Tool"
     description = "Apply regular expressions to column(s) to make new column(s)"
     link = "https://countess-project.github.io/CountESS/plugins/#regex-tool"
     version = VERSION
 
     parameters = {
         "regexes": ArrayParam(
@@ -41,29 +39,32 @@
                                     "Column Type",
                                     "string",
                                 ),
                             },
                         ),
                     ),
                     "drop_column": BooleanParam("Drop Column", False),
+                    "drop_unmatch": BooleanParam("Drop Unmatched Rows", False),
                 },
             ),
         ),
     }
 
     def apply_func(self, column_name, compiled_re, output_params, logger, row):
         value = str(row[column_name])
         match = compiled_re.match(value)
         if match:
-            return [output_params[n].datatype.cast_value(g) for n, g in enumerate(match.groups())]
+            return [1] + [
+                output_params[n].datatype.cast_value(g) for n, g in enumerate(match.groups())
+            ]
         else:
             logger.warning("Didn't Match", detail=repr(value))
-            return [None] * compiled_re.groups
+            return [0] + [None] * compiled_re.groups
 
-    def run_dask(self, df, logger):
+    def run_df(self, df, logger):
         # prevent added columns from propagating backwards in
         # the pipeline!
         df = df.copy()
 
         # the index doesn't seem to be available from within the applied function,
         # which is annoying, so we copy it into a column here.
         if any(rp["column"].is_index() for rp in self.parameters["regexes"]):
@@ -76,45 +77,42 @@
             compiled_re = re.compile(regex_parameter["regex"].value)
 
             while compiled_re.groups > len(regex_parameter["output"].params):
                 regex_parameter["output"].add_row()
 
             output_params = regex_parameter["output"].params
             output_names = [pp["name"].value for pp in output_params]
-            output_types = [pp["datatype"].get_selected_type() for pp in output_params]
 
             if regex_parameter["column"].is_index():
                 column_name = "__index"
             else:
                 column_name = regex_parameter["column"].value
 
             # XXX not totally happy with this
             func = partial(self.apply_func, column_name, compiled_re, output_params, logger)
 
-            if isinstance(df, dd.DataFrame):
-                # dask likes a hint about column types
-                meta = dict(enumerate(output_types))
-                re_groups_df = df.apply(func, axis=1, result_type="expand", meta=meta)
-            else:
-                # pandas infers the column types
-                re_groups_df = df.apply(func, axis=1, result_type="expand")
+            re_groups_df = df.apply(func, axis=1, result_type="expand")
 
             for n in range(0, compiled_re.groups):
-                df[output_names[n]] = re_groups_df[n]
+                df[output_names[n]] = re_groups_df[n + 1]
+
+            if regex_parameter["drop_unmatch"].value:
+                df["__filter"] = re_groups_df[0]
+                df = df.query("__filter != 0").drop(columns="__filter")
 
         drop_columns = set(
             rp["column"].value for rp in self.parameters["regexes"] if rp["drop_column"].value
         )
         if "__index" in df:
             drop_columns.add("__index")
 
         return df.drop(columns=drop_columns) if drop_columns else df
 
 
-class RegexReaderPlugin(DaskInputPlugin):
+class RegexReaderPlugin(PandasInputPlugin):
     name = "Regex Reader"
     description = """Loads arbitrary data from line-delimited files, applying a regular expression
       to each line to extract fields.  If you're trying to read generic CSV or TSV files, use the CSV
       plugin instead as it handles escaping correctly."""
     link = "https://countess-project.github.io/CountESS/plugins/#regex-reader"
     version = VERSION
 
@@ -178,8 +176,8 @@
                         pd.DataFrame.from_records(records, columns=columns, index=index_columns)
                     )
                     records = []
 
         if len(records) > 0:
             pdfs.append(pd.DataFrame.from_records(records, columns=columns, index=index_columns))
 
-        return concat_dataframes(pdfs)
+        return pd.concat(pdfs)
```

### Comparing `countess-0.0.22/countess/plugins/variant.py` & `countess-0.0.24/countess/plugins/variant.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,60 @@
-import dask.dataframe as dd
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
-from countess.core.parameters import ColumnChoiceParam, IntegerParam, StringParam
-from countess.core.plugins import DaskTransformPlugin
+from countess.core.parameters import ColumnOrIndexChoiceParam, IntegerParam, StringParam
+from countess.core.plugins import PandasTransformPlugin
 from countess.utils.variant import find_variant_string
 
 
 def process_row(var_seq: str, ref_seq: str, max_mutations: int, logger: Logger):
     try:
         return find_variant_string("g.", ref_seq, var_seq, max_mutations)
     except ValueError as exc:
         logger.warning(str(exc))
         return None
 
 
-def process_partition(
-    df: pd.DataFrame, column: str, sequence: str, output: str, max_mutations: int, logger: Logger
-):
-    dfo = df.copy()
-    dfo[output] = dfo[column].apply(process_row, args=(sequence, max_mutations, logger))
-    return dfo
-
-
-class VariantPlugin(DaskTransformPlugin):
+class VariantPlugin(PandasTransformPlugin):
     """Turns a DNA sequence into a HGVS variant code"""
 
     name = "Variant Translator"
     description = "Turns a DNA sequence into a HGVS variant code"
     version = VERSION
     link = "https://countess-project.github.io/CountESS/plugins/#variant"
 
     parameters = {
-        "column": ColumnChoiceParam("Input Column"),
+        "column": ColumnOrIndexChoiceParam("Input Column"),
         "sequence": StringParam("Reference Sequence"),
-        "output": StringParam("Output Column"),
+        "output": StringParam("Output Column", "variant"),
         "max_mutations": IntegerParam("Max Mutations", 10),
     }
 
-    def run_dask(
-        self, df: pd.DataFrame | dd.DataFrame, logger: Logger
-    ) -> pd.DataFrame | dd.DataFrame:
-        assert isinstance(self.parameters["column"], ColumnChoiceParam)
+    def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
+        assert isinstance(self.parameters["column"], ColumnOrIndexChoiceParam)
         assert isinstance(self.parameters["sequence"], StringParam)
         assert isinstance(self.parameters["output"], StringParam)
         assert isinstance(self.parameters["max_mutations"], IntegerParam)
 
-        args = (
-            self.parameters["column"].value,
-            self.parameters["sequence"].value,
-            self.parameters["output"].value,
-            self.parameters["max_mutations"].value,
-            logger,
-        )
+        dfo = df.copy()
+
+        output = self.parameters["output"].value
+
+        if self.parameters["column"].is_index():
+            dfo["__index"] = df.index
+            column_name = "__index"
+        else:
+            column_name = self.parameters["column"].value
+
+        if self.parameters["sequence"].value == "":
+            self.parameters["sequence"].value = dfo[column_name][0]
+
+        sequence = self.parameters["sequence"].value
+        max_mutations = self.parameters["max_mutations"].value
 
-        meta = dict(df.dtypes)
-        meta[self.parameters["output"].value] = str
+        dfo[output] = dfo[column_name].apply(process_row, args=(sequence, max_mutations, logger))
 
-        if isinstance(df, dd.DataFrame):
-            return df.map_partitions(process_partition, *args, meta=meta)
+        if self.parameters["column"].is_index():
+            return dfo.drop(columns=["__index"])
         else:
-            return process_partition(df, *args)
+            return dfo
```

### Comparing `countess-0.0.22/countess/utils/variant.py` & `countess-0.0.24/countess/utils/variant.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,10 +255,10 @@
 
     variations = list(find_variant_dna(ref_seq, var_seq))
 
     if len(variations) == 0:
         return prefix + "="
 
     if max_mutations is not None and len(variations) > max_mutations:
-        raise ValueError("Too many variations")
+        raise ValueError("Too many variations (%d) in {var_seq}" % len(variations))
 
     return prefix + "(;)".join(variations)
```

### Comparing `countess-0.0.22/countess.egg-info/PKG-INFO` & `countess-0.0.24/countess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.22
+Version: 0.0.24
 Summary: CountESS
 Author: CountESS Developers
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer: Nick Moore
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.22
+# CountESS 0.0.24
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.22/countess.egg-info/SOURCES.txt` & `countess-0.0.24/countess.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,20 +19,19 @@
 countess/core/plugins.py
 countess/gui/__init__.py
 countess/gui/config.py
 countess/gui/logger.py
 countess/gui/main.py
 countess/plugins/__init__.py
 countess/plugins/csv.py
-countess/plugins/embed_python.py
+countess/plugins/expression.py
 countess/plugins/fastq.py
 countess/plugins/group_by.py
 countess/plugins/hdf5.py
 countess/plugins/join.py
 countess/plugins/log_score.py
 countess/plugins/pivot.py
 countess/plugins/regex.py
 countess/plugins/variant.py
 countess/utils/__init__.py
-countess/utils/dask.py
 countess/utils/variant.py
 tests/test_gui.py
```

### Comparing `countess-0.0.22/countess.egg-info/entry_points.txt` & `countess-0.0.24/countess.egg-info/entry_points.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [console_scripts]
 countess_cmd = countess.core.cmd:main
 
 [countess_plugins]
-embed_py = countess.plugins.embed_python:EmbeddedPythonPlugin
+expression = countess.plugins.expression:ExpressionPlugin
 group_by = countess.plugins.group_by:GroupByPlugin
-join = countess.plugins.join:DaskJoinPlugin
+group_by_expr = countess.plugins.group_by:GroupByExprPlugin
+join = countess.plugins.join:JoinPlugin
 load_csv = countess.plugins.csv:LoadCsvPlugin
 load_fastq = countess.plugins.fastq:LoadFastqPlugin
 load_hdf = countess.plugins.hdf5:LoadHdfPlugin
 log_score = countess.plugins.log_score:LogScorePlugin
-pivot = countess.plugins.pivot:DaskPivotPlugin
+pivot = countess.plugins.pivot:PivotPlugin
 regex_reader = countess.plugins.regex:RegexReaderPlugin
 regex_tool = countess.plugins.regex:RegexToolPlugin
 save_csv = countess.plugins.csv:SaveCsvPlugin
 variants = countess.plugins.variant:VariantPlugin
 
 [gui_scripts]
 countess_gui = countess.gui.main:main
```

### Comparing `countess-0.0.22/pyproject.toml` & `countess-0.0.24/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,47 +16,48 @@
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
 dependencies = [
-    'dask>=2022.8.0',
-    'distributed>=2022.8.0',
     'fqfa~=1.2.3',
-    'more_itertools>=8.14.0',
-    'numpy~=1.23',
-    'pandas~=1.4',
-    'rapidfuzz~=2.13',
-    'ttkthemes~=3.2',
+    'more_itertools~=9.1.0',
+    'numpy~=1.24.2',
+    'pandas~=2.0.0',
+    'rapidfuzz~=2.15.1',
+    'ttkthemes~=3.2.2',
 ]
 
 [project.optional-dependencies]
 dev = [
-    'black<24',
+    'black<24', 
+    'build==0.10.0',
     'mypy~=1.0.1',
     'pylint~=2.16',
     'types-ttkthemes~=3.2',
+    'twine==4.0.2',
     'pandas-stubs~=1.4',
     'pytest~=7.2',
 ]
 
 hdf = [
-     'tables~=3.7',
+     'tables~=3.8.0',
 ]
 
 [project.entry-points.countess_plugins]
 load_fastq = "countess.plugins.fastq:LoadFastqPlugin"
 load_hdf = "countess.plugins.hdf5:LoadHdfPlugin"
 load_csv = "countess.plugins.csv:LoadCsvPlugin"
 log_score = "countess.plugins.log_score:LogScorePlugin"
 group_by = "countess.plugins.group_by:GroupByPlugin"
-embed_py = "countess.plugins.embed_python:EmbeddedPythonPlugin"
-pivot = "countess.plugins.pivot:DaskPivotPlugin"
-join = "countess.plugins.join:DaskJoinPlugin"
+group_by_expr = "countess.plugins.group_by:GroupByExprPlugin"
+expression = "countess.plugins.expression:ExpressionPlugin"
+pivot = "countess.plugins.pivot:PivotPlugin"
+join = "countess.plugins.join:JoinPlugin"
 save_csv = "countess.plugins.csv:SaveCsvPlugin"
 regex_tool = "countess.plugins.regex:RegexToolPlugin"
 regex_reader = "countess.plugins.regex:RegexReaderPlugin"
 variants = "countess.plugins.variant:VariantPlugin"
 
 [project.entry-points.gui_scripts]
 countess_gui = "countess.gui.main:main"
```

### Comparing `countess-0.0.22/setup.cfg` & `countess-0.0.24/setup.cfg`

 * *Files identical despite different names*

### Comparing `countess-0.0.22/tests/test_gui.py` & `countess-0.0.24/tests/test_gui.py`

 * *Files identical despite different names*


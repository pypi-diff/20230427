# Comparing `tmp/robocorp_tasks-0.1.5.tar.gz` & `tmp/robocorp_tasks-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-0.1.5.tar", max compression
+gzip compressed data, was "robocorp_tasks-0.1.6.tar", max compression
```

## Comparing `robocorp_tasks-0.1.5.tar` & `robocorp_tasks-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4799 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/README.md
--rw-r--r--   0        0        0     1214 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      721 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     3371 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1230 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5048 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0     5284 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0      638 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_decorators.py
--rw-r--r--   0        0        0      182 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0      599 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     4519 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0     2335 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     1699 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0      933 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0      809 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 robocorp_tasks-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4799 2023-04-27 17:49:20.287384 robocorp_tasks-0.1.6/README.md
+-rw-r--r--   0        0        0     1214 2023-04-27 17:49:20.287384 robocorp_tasks-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      721 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     3371 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1230 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5048 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0     5284 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0      638 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_decorators.py
+-rw-r--r--   0        0        0      182 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0      599 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     4940 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0     2335 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     1699 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0      933 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0      809 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 robocorp_tasks-0.1.6/PKG-INFO
```

### Comparing `robocorp_tasks-0.1.5/README.md` & `robocorp_tasks-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/pyproject.toml` & `robocorp_tasks-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "0.1.5"
+version = "0.1.6"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/tasks", from = "src"}]
 classifiers = [
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-log = "0.0.12"
+robocorp-log = "0.0.13"
 
 [tool.mypy]
 mypy_path = "src:tests"
 
 [[tool.mypy.overrides]]
 module = "setuptools.*"
 ignore_missing_imports = true
```

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/__init__.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 Note: Using the `cli.main(args)` is possible to run tasks programmatically, but
 clients using this approach MUST make sure that any code which must be
 automatically logged is not imported prior the the `cli.main` call.
 """
 
 from ._decorators import task
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 version_info = [int(x) for x in __version__.split(".")]
```

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/_callback.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/_commands.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/_commands.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/_decorators.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/_decorators.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/_log_auto_setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from typing import Optional, List, Any
 
 from ._protocols import ITask
 from robocorp import log
 
 
 def read_filters_from_pyproject_toml(context, path: Path) -> log.BaseConfig:
-    filters: List[log.Filter] = []
-
     while True:
         pyproject = path / "pyproject.toml"
         try:
             if pyproject.exists():
                 break
         except OSError:
             continue
@@ -35,83 +33,95 @@
         except ImportError:
             import tomli as tomllib  # type: ignore
 
         obj = tomllib.loads(toml_contents)
     except Exception:
         raise RuntimeError(f"Could not interpret the contents of {pyproject} as toml.")
 
-    # Filter(name="RPA", kind=FilterKind.log_on_project_call),
-    # Filter("selenium", FilterKind.log_on_project_call),
-    # Filter("SeleniumLibrary", FilterKind.log_on_project_call),
-
-    read_parts: List[str] = []
-    for part in "tool.robocorp.log".split("."):
-        read_parts.append(part)
-
-        obj = obj.get(part)
-        if not obj:
-            break
-
-        elif not isinstance(obj, dict):
-            context.show_error(
-                f"Expected {'.'.join(read_parts)} to be a dict in {pyproject}."
-            )
-            break
+    filters: List[log.Filter] = []
+    if isinstance(obj, dict):
+        # Filter(name="RPA", kind=FilterKind.log_on_project_call),
+        # Filter("selenium", FilterKind.log_on_project_call),
+        # Filter("SeleniumLibrary", FilterKind.log_on_project_call),
+
+        read_parts: List[str] = []
+        for part in "tool.robocorp.log".split("."):
+            read_parts.append(part)
 
-    log_filter_rules: list = []
-    obj = obj.get("log_filter_rules")
-    if obj:
-        if isinstance(obj, list):
-            log_filter_rules = obj
+            obj = obj.get(part)
+            if not obj:
+                break
+
+            elif not isinstance(obj, dict):
+                context.show_error(
+                    f"Expected {'.'.join(read_parts)} to be a dict in {pyproject}."
+                )
+                break
         else:
-            context.show_error(
-                f"Expected {'.'.join(read_parts)} to be a list in {pyproject}."
-            )
+            if isinstance(obj, dict):
+                filters = _load_filters(obj, context, pyproject)
+
+    return log.ConfigFilesFiltering(filters=filters)
+
+
+def _load_filters(obj: dict, context, pyproject) -> List[log.Filter]:
+    filters: List[log.Filter] = []
+    log_filter_rules: list = []
+    list_obj = obj.get("log_filter_rules")
+    if not list_obj:
+        return filters
+
+    if isinstance(list_obj, list):
+        log_filter_rules = list_obj
+    else:
+        context.show_error(
+            f"Expected 'tool.robocorp.log.log_filter_rules' to be a list in {pyproject}."
+        )
+        return filters
 
     # If we got here we have the 'log_filter_rules', which should be a list of
     # dicts in a structure such as: {name = "difflib", kind = "log_on_project_call"}
     # expected kinds are the values of the FilterKind.
     for rule in log_filter_rules:
         if isinstance(rule, dict):
             name = rule.get("name")
             kind = rule.get("kind")
             if not name:
                 context.show_error(
-                    f"Expected a rule from 'tool.robocorp.log.log_filter_rules' to have a 'name' in {pyproject}."
+                    f"Expected rule: {rule} from 'tool.robocorp.log.log_filter_rules' to have a 'name' in {pyproject}."
                 )
                 continue
 
             if not kind:
                 context.show_error(
-                    f"Expected a rule from 'tool.robocorp.log.log_filter_rules' to have a 'kind' in {pyproject}."
+                    f"Expected rule: {rule} from 'tool.robocorp.log.log_filter_rules' to have a 'kind' in {pyproject}."
                 )
                 continue
 
             if not isinstance(name, str):
                 context.show_error(
-                    f"Expected a rule from 'tool.robocorp.log.log_filter_rules' to have 'name' as a str in {pyproject}."
+                    f"Expected rule: {rule} from 'tool.robocorp.log.log_filter_rules' to have 'name' as a str in {pyproject}."
                 )
                 continue
 
             if not isinstance(kind, str):
                 context.show_error(
-                    f"Expected a rule from 'tool.robocorp.log.log_filter_rules' to have 'kind' as a str in {pyproject}."
+                    f"Expected rule: {rule} from 'tool.robocorp.log.log_filter_rules' to have 'kind' as a str in {pyproject}."
                 )
                 continue
 
             f: Optional[log.FilterKind] = getattr(log.FilterKind, kind, None)
             if f is None:
                 context.show_error(
-                    f"Rule from 'tool.robocorp.log.log_filter_rules' has invalid 'kind': >>{kind}<< in {pyproject}."
+                    f"Rule from 'tool.robocorp.log.log_filter_rules' ({rule}) has invalid 'kind': >>{kind}<< in {pyproject}."
                 )
                 continue
 
             filters.append(log.Filter(name, f))
-
-    return log.ConfigFilesFiltering(filters=filters)
+    return filters
 
 
 def _log_before_task_run(task: ITask):
     log.start_task(
         task.name,
         task.module_name,
         task.filename,
```

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/_log_output_setup.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/_task.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/src/robocorp/tasks/cli.py` & `robocorp_tasks-0.1.6/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.5/PKG-INFO` & `robocorp_tasks-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 0.1.5
+Version: 0.1.6
 Summary: The automation framework for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Dist: robocorp-log (==0.0.12)
+Requires-Dist: robocorp-log (==0.0.13)
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
 
 `robocorp-tasks` is a Python framework to simplify RPA development in Python.
 
 > Note: The current version is still alpha but its public API is already meant
```


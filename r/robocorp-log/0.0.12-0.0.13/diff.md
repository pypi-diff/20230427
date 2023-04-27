# Comparing `tmp/robocorp_log-0.0.12.tar.gz` & `tmp/robocorp_log-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_log-0.0.12.tar", max compression
+gzip compressed data, was "robocorp_log-0.0.13.tar", max compression
```

## Comparing `robocorp_log-0.0.12.tar` & `robocorp_log-0.0.13.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    10142 2023-04-24 19:07:45.261923 robocorp_log-0.0.12/LICENSE
--rw-r--r--   0        0        0     3086 2023-04-24 19:07:45.261923 robocorp_log-0.0.12/README.md
--rw-r--r--   0        0        0      904 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/pyproject.toml
--rw-r--r--   0        0        0    21137 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/__init__.py
--rw-r--r--   0        0        0     8406 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_ast_utils.py
--rw-r--r--   0        0        0     8441 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_auto_logging_setup.py
--rw-r--r--   0        0        0     5361 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_config.py
--rw-r--r--   0        0        0      572 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_convert_units.py
--rw-r--r--   0        0        0     6699 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_decoder.py
--rw-r--r--   0        0        0    43217 2023-04-24 19:08:29.798847 robocorp_log-0.0.12/src/robocorp/log/_index.py
--rw-r--r--   0        0        0    55054 2023-04-24 19:08:32.106892 robocorp_log-0.0.12/src/robocorp/log/_index_v2.py
--rw-r--r--   0        0        0     2305 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_lifecycle_hooks.py
--rw-r--r--   0        0        0      493 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_logger_instances.py
--rw-r--r--   0        0        0     1208 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_null.py
--rw-r--r--   0        0        0      385 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_obj_info_repr.py
--rw-r--r--   0        0        0    18981 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_rewrite_ast_add_callbacks.py
--rw-r--r--   0        0        0     8900 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_rewrite_filtering.py
--rw-r--r--   0        0        0    12339 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_rewrite_importhook.py
--rw-r--r--   0        0        0     8710 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_robo_logger.py
--rw-r--r--   0        0        0    51335 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_robo_output_impl.py
--rw-r--r--   0        0        0     1436 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_sensitive_variable_names.py
--rw-r--r--   0        0        0     1915 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_suppress_helper.py
--rw-r--r--   0        0        0     1057 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/protocols.py
--rw-r--r--   0        0        0        0 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/py.typed
--rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 robocorp_log-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-04-27 17:46:21.376182 robocorp_log-0.0.13/LICENSE
+-rw-r--r--   0        0        0     3086 2023-04-27 17:46:21.376182 robocorp_log-0.0.13/README.md
+-rw-r--r--   0        0        0     1200 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/pyproject.toml
+-rw-r--r--   0        0        0    22821 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/__init__.py
+-rw-r--r--   0        0        0    11808 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_ast_utils.py
+-rw-r--r--   0        0        0     9778 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_auto_logging_setup.py
+-rw-r--r--   0        0        0     5361 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_config.py
+-rw-r--r--   0        0        0      572 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_convert_units.py
+-rw-r--r--   0        0        0     7310 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_decoder.py
+-rw-r--r--   0        0        0    43500 2023-04-27 17:47:06.536794 robocorp_log-0.0.13/src/robocorp/log/_index.py
+-rw-r--r--   0        0        0    55337 2023-04-27 17:47:08.820825 robocorp_log-0.0.13/src/robocorp/log/_index_v2.py
+-rw-r--r--   0        0        0     2497 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0      493 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_logger_instances.py
+-rw-r--r--   0        0        0     1208 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_null.py
+-rw-r--r--   0        0        0      385 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_obj_info_repr.py
+-rw-r--r--   0        0        0    19391 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0     8900 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12453 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_rewrite_importhook.py
+-rw-r--r--   0        0        0     9425 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_robo_logger.py
+-rw-r--r--   0        0        0    53386 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_robo_output_impl.py
+-rw-r--r--   0        0        0     1436 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_sensitive_variable_names.py
+-rw-r--r--   0        0        0     1915 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/_suppress_helper.py
+-rw-r--r--   0        0        0     1057 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/protocols.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:46:21.380182 robocorp_log-0.0.13/src/robocorp/log/py.typed
+-rw-r--r--   0        0        0     3885 1970-01-01 00:00:00.000000 robocorp_log-0.0.13/PKG-INFO
```

### Comparing `robocorp_log-0.0.12/LICENSE` & `robocorp_log-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.12/README.md` & `robocorp_log-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.12/src/robocorp/log/__init__.py` & `robocorp_log-0.0.13/src/robocorp/log/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from .protocols import OptExcInfo, LogHTMLStyle, Status, IReadLines
 from ._suppress_helper import SuppressHelper as _SuppressHelper
 
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
 
-__version__ = "0.0.12"
+__version__ = "0.0.13"
 version_info = [int(x) for x in __version__.split(".")]
 
 from . import _config
 
 # --- Make these a part of the public API.
 
 Filter = _config.Filter
@@ -44,72 +44,121 @@
 BaseConfig = _config.BaseConfig
 ConfigFilesFiltering = _config.ConfigFilesFiltering
 
 
 # --- Logging methods for custom messaging.
 
 
-def _log(level, message: str, html: bool = False) -> None:
+def _log(level, message: Sequence[Any], html: bool = False) -> None:
     back_frame = sys._getframe(2)
     source = back_frame.f_code.co_filename
     lineno = back_frame.f_lineno
 
+    m = " ".join(str(x) for x in message)
     for robo_logger in _get_logger_instances():
-        robo_logger.log_message(level, message, html, source, lineno)
+        robo_logger.log_message(level, m, html, source, lineno)
 
 
-def critical(message: str, html: bool = False) -> None:
+def critical(*message: Any) -> None:
     """
     Adds a new logging message with a critical (error) level.
 
     Args:
         message: The message which should be logged.
         html: If True the message passed should be rendered as HTML.
+
+    Example:
+        critical('Failed because', obj, 'is not', expected)
+
+    Note:
+        Formatting converts all objects given to `str`. If you need custom
+        formatting please pre-format the string.
+        i.e.:
+        critical(f'Failed because {obj!r} is not {expected!r}.')
     """
-    _log(Status.ERROR, message, html)
+    _log(Status.ERROR, message)
 
 
-def warn(message: str, html: bool = False) -> None:
+def warn(*message: Any) -> None:
     """
     Adds a new logging message with a warn level.
 
     Args:
         message: The message which should be logged.
         html: If True the message passed should be rendered as HTML.
+
+    Example:
+        warn('Did not expect', obj)
+
+    Note:
+        Formatting converts all objects given to `str`. If you need custom
+        formatting please pre-format the string.
+        i.e.:
+        warn(f'Did not expect {obj!r}.')
     """
-    _log(Status.WARN, message, html)
+    _log(Status.WARN, message)
 
 
-def info(message: str, html: bool = False) -> None:
+def info(*message: Any) -> None:
     """
     Adds a new logging message with an info level.
 
     Args:
         message: The message which should be logged.
         html: If True the message passed should be rendered as HTML.
+
+
+    Example:
+        info('Received value', obj)
+
+    Note:
+        Formatting converts all objects given to `str`. If you need custom
+        formatting please pre-format the string.
+        i.e.:
+        info(f'Received value {obj!r}.')
+
     """
-    _log(Status.INFO, message, html)
+    _log(Status.INFO, message)
 
 
-def exception(message: Optional[str] = None, html: bool = False):
+def exception(*message: Any):
     """
     Adds to the logging the exceptions that's currently raised.
 
     Args:
         message: If given an additional error message to be shown.
         html: If True the message passed should be rendered as HTML.
     """
     if message:
-        _log(Status.ERROR, message, html)
+        _log(Status.ERROR, message)
 
     exc_info = sys.exc_info()
     for robo_logger in _get_logger_instances():
         robo_logger.log_method_except(exc_info, unhandled=True)
 
 
+def html(html: str, level: str = "INFO"):
+    """
+    Adds html contents to the log.
+
+    Args:
+        html: The html content to be embedded in the page.
+        level: The level of the message ("INFO", "WARN" or "ERROR")
+
+    Example adding an image:
+
+        html(
+            '<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAnBAMAAACGbbfxAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAbUExURR4nOzpCVI+Tnf///+Pk5qqutXN4hVZdbMbJzod39mUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAETSURBVDjLnZIxT8MwFITPqDQdG1rBGjX8AOBS0hG1ghnUhbFSBlZvMFbqH+fZaeMLBJA4KZHzyb7ce374l1we3vm0Ty/Ix7era1YvSjOeVBWCZx3mveBDwlWyH1OUXM5t0yJqS+4V33xdwWFCrvOoOfmA1r30Z+r9jHV7zmeKd7ADQEOvATkFlzGz13JqIGanYbexYLOldcY+IsniqrEyRrUj7xBwccRm/lSuPqysI3YBjzUfQproNOr/0tLEgE3CK8P2YG54K401XIeWHDw2Uo5H5UP1l1ZXr9+7U2ffRfhTC9HwFVMmqOzl7vTDnEwSvhXsNLaoGbIGurvf97ArhzYbj01sm6TKXm3yC3yX8/hdwCdipl9ujxriXgAAAABJRU5ErkJggg=="/>'
+        )
+    """
+
+    assert level in ("ERROR", "WARN", "INFO")
+    _log(level, (html,), html=True)
+
+
 # --- Methods related to hiding logging information.
 
 
 @contextmanager
 def _suppress_contextmanager(variables=True, methods=True):
     instances = _get_logger_instances()
     for robo_logger in instances:
```

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_auto_logging_setup.py` & `robocorp_log-0.0.13/src/robocorp/log/_auto_logging_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -180,14 +180,55 @@
             return
 
         self.status_stack.append(_StackEntry(mod_name, name, "PASS"))
 
         for robo_logger in _get_logger_instances():
             robo_logger.yield_resume(name, mod_name, filename, lineno)
 
+    def call_before_yield_from(
+        self,
+        mod_name: str,
+        filename: str,
+        name: str,
+        lineno: int,
+    ) -> None:
+        if self.tid != threading.get_ident():
+            return
+
+        try:
+            pop_stack_entry = self.status_stack.pop(-1)
+        except IndexError:
+            # oops, something bad happened, the stack is unsynchronized
+            critical("On before yield from the status_stack was empty.")
+            return
+        else:
+            if pop_stack_entry.mod_name != mod_name or pop_stack_entry.name != name:
+                critical(
+                    f"On before yield from status stack package/name was: {pop_stack_entry.mod_name}.{pop_stack_entry.name}. Received: {mod_name}.{name}."
+                )
+                return
+
+        for robo_logger in _get_logger_instances():
+            robo_logger.yield_from_suspend(name, mod_name, filename, lineno)
+
+    def call_after_yield_from(
+        self,
+        mod_name: str,
+        filename: str,
+        name: str,
+        lineno: int,
+    ) -> None:
+        if self.tid != threading.get_ident():
+            return
+
+        self.status_stack.append(_StackEntry(mod_name, name, "PASS"))
+
+        for robo_logger in _get_logger_instances():
+            robo_logger.yield_from_resume(name, mod_name, filename, lineno)
+
     def call_after_assign(
         self,
         mod_name: str,
         filename: str,
         name: str,
         lineno: int,
         assign_name: str,
```

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_config.py` & `robocorp_log-0.0.13/src/robocorp/log/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_convert_units.py` & `robocorp_log-0.0.13/src/robocorp/log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_decoder.py` & `robocorp_log-0.0.13/src/robocorp/log/_decoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,14 +105,19 @@
     memo_value = json.loads(memo_value)
     decoder.memo[memo_id] = memo_value
 
 
 # Whenever the decoding changes we should bump up this version.
 DOC_VERSION = "0.0.1"
 
+MESSAGE_TYPE_YIELD_RESUME = "YR"
+MESSAGE_TYPE_YIELD_SUSPEND = "YS"
+MESSAGE_TYPE_YIELD_FROM_RESUME = "YFR"
+MESSAGE_TYPE_YIELD_FROM_SUSPEND = "YFS"
+
 _MESSAGE_TYPE_INFO: Dict[str, Callable[[Decoder, str], Any]] = {
     # Version of the log output
     "V": _decode("version:str"),
     # Some information message
     "I": lambda _decoder, message: {"info": json.loads(message)},
     # The log has an id that may be split into multiple parts.
     "ID": _decode("part:int, id:str"),
@@ -141,22 +146,30 @@
     # End Task
     "ET": _decode("status:oid, message:oid, time_delta_in_seconds:float"),
     # Start Element (some element we're tracking such as method, for, while, etc).
     "SE": _decode(
         "name:oid, libname:oid, type:oid, doc:oid, source:oid, lineno:int, time_delta_in_seconds:float",
     ),
     # Yield Resume (coming back to a suspended frame).
-    "YR": _decode(
+    MESSAGE_TYPE_YIELD_RESUME: _decode(
+        "name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float",
+    ),
+    # Yield From Resume (coming back to a suspended frame).
+    MESSAGE_TYPE_YIELD_FROM_RESUME: _decode(
         "name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float",
     ),
     # End Element
     "EE": _decode("type:oid, status:oid, time_delta_in_seconds:float"),
-    # Yield Suspend
-    "YS": _decode(
-        "source:oid, lineno:int, type:oid, value:oid, time_delta_in_seconds:float",
+    # Yield Suspend (pausing a frame)
+    MESSAGE_TYPE_YIELD_SUSPEND: _decode(
+        "name:oid, libname:oid, source:oid, lineno:int, type:oid, value:oid, time_delta_in_seconds:float",
+    ),
+    # Yield From Suspend (pausing a frame)
+    MESSAGE_TYPE_YIELD_FROM_SUSPEND: _decode(
+        "name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float",
     ),
     # Assign
     "AS": _decode(
         "source:oid, lineno:int, target:oid, type:oid, value:oid, time_delta_in_seconds:float"
     ),
     # Element/method argument (name and value of the argument).
     "EA": _decode("name:oid, type:oid, value:oid"),
```

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_index.py` & `robocorp_log-0.0.13/src/robocorp/log/_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Note: autogenerated file.
 # To regenerate this file use: python -m dev build-output-view.
 
 # The FILE_CONTENTS contains the contents of the files with
 # html/javascript code which can be used to visualize the contents of the
 # output generated by robocorp-log (i.e.: the .log files).
 
-FILE_CONTENTS = {'index.html': '<!doctype html><html style="padding: 0 0 0 0; margin: 0 0 0 0; height: 100%"><head><meta charset="utf-8"/><title>Robot Output</title><meta name="viewport" content="width=device-width,initial-scale=1"/></head><body class="vscode-dark" style="padding: 0 0 0 0; margin: 0 0 0 0; height: 100%; display: flex; flex-direction: column"><div style="display: flex"><div class="summaryField" style="flex-grow: 1; white-space: nowrap" id="summary" class="NOT_RUN">Total:&nbsp;&nbsp;&nbsp;&nbsp;Failures:&nbsp;&nbsp;&nbsp;&nbsp;</div><div class="summaryField" style="flex-grow: 1"><div style="display: flex"><span>Filter:&nbsp;</span> <select name="filterLevel" id="filterLevel" style="flex-grow: 1" onchange="window.onChangedFilterLevel()"><option value="FAIL">FAIL</option><option value="WARN">WARN</option><option value="PASS" selected="selected">PASS</option><option value="NOT RUN">NOT RUN</option></select></div></div><div class="summaryField" id="selectRunContainer" style="flex-grow: 2; display: none"><select name="selectedRun" id="selectedRun" onchange="window.onChangedRun()" style="width: 100%"><option value="NO_RUN" selected="selected">No runs available...</option></select></div></div><div id="mainTree" style="white-space: nowrap; overflow: auto; flex-grow: 1"></div><script>(()=>{"use strict";var e={426:(e,t,n)=>{n.d(t,{Z:()=>a});var o=n(645),s=n.n(o)()((function(e){return e[1]}));s.push([e.id,":root {\\n    --fg-color: var(--vscode-editor-foreground, black);\\n    --bg-color: var(--vscode-editor-background, white);\\n    --font-family: var(--vscode-editor-font-family, monospace, courier);\\n    --font-size: var(--vscode-editor-font-size, 14px);\\n    --font-weight: var(--vscode-font-weight);\\n    --menu-background: var(--vscode-menu-background, rgb(235, 235, 235));\\n    --menu-foreground: var(--vscode-menu-foreground, rgb(0, 0, 0));\\n\\n    /* background-color: var(--vscode-editorError-foreground); */\\n    /* background-color: var(--vscode-inputValidation-errorBorder);  high-contrast doesn\'t have a good color */\\n    /* background-color: var(--vscode-testing-iconErrored);  red and green always (not always ideal...) */\\n    --error-background-color: var(--vscode-terminalCommandDecoration-errorBackground, rgb(201, 28, 28));\\n    --error-color: var(--vscode-button-foreground, white);\\n\\n    --hidden-background-color: var(--vscode-foobarcolornotthere, rgb(243, 152, 16));\\n    --hidden-color: var(--vscode-button-foreground, white);\\n\\n    /* background-color: var(--vscode-inputValidation-infoBorder); */\\n    /* background-color: var(--vscode-testing-iconPassed); */\\n    --pass-background-color: var(--vscode-terminalCommandDecoration-successBackground, rgb(36, 47, 202));\\n    --pass-color: var(--vscode-button-foreground, white);\\n\\n    --warn-background-color: var(--vscode-debugConsole-warningForeground, rgb(190, 159, 20));\\n    --warn-color: var(--vscode-button-foreground, white);\\n\\n    --not-run-background-color: var(--vscode-editor-foreground, rgb(102, 102, 102));\\n    --not-run-color: var(--vscode-editor-background, white);\\n\\n    --summary-hover-background-color: var(--vscode-editor-hoverHighlightBackground, rgb(222, 222, 222));\\n\\n    /* \\n    --fg-color: white;\\n    --bg-color: #4b4a4a;\\n    --font-family: \\"Segoe UI\\", Tahoma, Geneva, Verdana, sans-serif; \\n    */\\n}\\n\\n.summaryField {\\n    margin-left: 3px;\\n    margin-right: 3px;\\n}\\n\\n.summaryFileName {\\n    opacity: 0.6;\\n    margin-left: 1rem;\\n}\\n\\n.timeLabel {\\n    opacity: 0.6;\\n}\\n\\n/* .summaryInput {\\n    opacity: 0.6;\\n} */\\n\\n.summaryInput::before {\\n    margin-left: 3px;\\n    content: \\"(\\";\\n}\\n.summaryInput::after {\\n    margin-right: 3px;\\n    content: \\")\\";\\n}\\n\\n/* nesting level vertical line */\\n.detailInfo {\\n    border-left: 1px solid var(--error-background-color);\\n\\n    /* centering the line with the icon */\\n    margin-left: 1.5rem;\\n\\n    /* nesting indentation */\\n    padding-left: 0.8rem;\\n}\\n\\nbody {\\n    font-family: var(--font-family);\\n    font-size: var(--font-size);\\n    font-weight: var(--font-weight);\\n    color: var(--fg-color);\\n    background-color: var(--bg-color);\\n}\\n\\n#mainTree {\\n    margin-top: 5px;\\n}\\n\\nul {\\n    list-style-type: none;\\n    padding-inline-start: 0px;\\n    margin-block-start: 0px;\\n}\\n\\ndiv ul:not(:first-child) {\\n    border-left: 1px dotted rgb(141, 141, 141);\\n}\\n\\n.tree li {\\n    display: block;\\n    position: relative;\\n    padding-left: 0px;\\n}\\n\\n.tree ul {\\n    margin-left: 10px;\\n    padding-left: 0;\\n}\\n\\n.toolbarButton {\\n    display: inline;\\n    border-radius: 5px;\\n    background: var(--bg-color);\\n    color: var(--fg-color);\\n    margin-left: 3px;\\n    width: 15px;\\n    height: 15px;\\n    border: 0;\\n    padding: 0;\\n    vertical-align: middle;\\n}\\n\\n.toolbarContainer {\\n    display: inline-block;\\n}\\n\\n.summaryDiv {\\n    display: inline;\\n}\\n\\ndetails > summary {\\n    /* Note: couldn\'t get proper color with the svg approach */\\n    /* list-style-image: url(\\"data:image/svg+xml;utf8,<svg width=\'12px\' height=\'12px\' viewBox=\'0 0 20 20\' xmlns=\'http://www.w3.org/2000/svg\'><g data-name=\'Layer 2\'><g data-name=\'arrow-ios-forward\'><rect width=\'24\' height=\'24\' transform=\'rotate(-90 12 12)\' opacity=\'0\'/><path fill=\'currentColor\' stroke=\'currentColor\' d=\'M10 19a1 1 0 0 1-.64-.23 1 1 0 0 1-.13-1.41L13.71 12 9.39 6.63a1 1 0 0 1 .15-1.41 1 1 0 0 1 1.46.15l4.83 6a1 1 0 0 1 0 1.27l-5 6A1 1 0 0 1 10 19z\'/></g></g></svg>\\"); */\\n    /* list-style-type: \\"⮞ \\"; */\\n    /* list-style-type: \\"⏵\\"; */\\n    list-style-type: \\"+ \\";\\n}\\n\\ndetails[open] > summary {\\n    /* list-style-image: url(\\"data:image/svg+xml;utf8,<svg width=\'12px\' height=\'12px\' viewBox=\'0 0 20 20\' xmlns=\'http://www.w3.org/2000/svg\'><g data-name=\'Layer 2\'><g data-name=\'arrow-ios-downward\'><rect width=\'24\' height=\'24\' opacity=\'0\'/><path fill=\'currentColor\' stroke=\'currentColor\' d=\'M12 16a1 1 0 0 1-.64-.23l-6-5a1 1 0 1 1 1.28-1.54L12 13.71l5.36-4.32a1 1 0 0 1 1.41.15 1 1 0 0 1-.14 1.46l-6 4.83A1 1 0 0 1 12 16z\'/></g></g></svg>\\"); */\\n    /* list-style-type: \\"⮟ \\"; */\\n    /* list-style-type: \\"⏷\\"; */\\n    list-style-type: \\"- \\";\\n}\\n\\n.NO_CHILDREN > summary {\\n    list-style-type: \\"\xa0\xa0\\" !important;\\n}\\n\\nselect {\\n    background-color: var(--menu-background);\\n    color: var(--menu-foreground);\\n}\\n\\nsummary {\\n    padding: 3px;\\n}\\n\\na:link {\\n    color: var(--fg-color);\\n}\\n\\na:visited {\\n    color: var(--fg-color);\\n}\\n\\na:hover {\\n    color: var(--fg-color);\\n}\\n\\na:active {\\n    color: var(--fg-color);\\n}\\n\\n.label {\\n    padding: 2px 2px;\\n    font-size: 0.65em;\\n    letter-spacing: 1px;\\n    white-space: nowrap;\\n    border-radius: 3px;\\n    margin-right: 5px;\\n    font-weight: bold;\\n}\\n\\n.timeLabel {\\n    padding: 2px 2px;\\n    font-size: 0.85em;\\n    letter-spacing: 1px;\\n    white-space: nowrap;\\n    border-radius: 3px;\\n    margin-right: 5px;\\n    font-weight: lighter;\\n}\\n\\n.label.F,\\n.label.E,\\n.label.FAIL,\\n.label.ERROR {\\n    border-radius: 3px;\\n    background-color: var(--error-background-color);\\n    color: var(--error-color);\\n    font-weight: bolder;\\n}\\n\\n.label.PASS,\\n.label.I,\\n.label.INFO {\\n    border-radius: 3px;\\n    background-color: var(--pass-background-color);\\n    color: var(--pass-color);\\n    font-weight: bolder;\\n}\\n\\n.label.W,\\n.label.WARN {\\n    border-radius: 3px;\\n    background-color: var(--warn-background-color);\\n    color: var(--warn-color);\\n    font-weight: bolder;\\n}\\n\\n.label.HIDDEN {\\n    border-radius: 3px;\\n    background-color: var(--hidden-background-color);\\n    color: var(--hidden-color);\\n    font-weight: bolder;\\n}\\n.label.HIDDEN.inline {\\n    margin-left: 5px;\\n}\\n\\nsummary.HIDDEN {\\n    margin-top: 10px;\\n    margin-bottom: 10px;\\n}\\n\\n.label.NOT_RUN {\\n    border-radius: 3px;\\n    background-color: var(--not-run-background-color);\\n    color: var(--not-run-color);\\n    font-weight: bolder;\\n}\\n\\n#summary.FAIL,\\n#summary.ERROR {\\n    border-bottom: 5px solid var(--error-background-color);\\n}\\n\\n#summary.PASS {\\n    border-bottom: 5px solid var(--pass-background-color);\\n}\\n\\n#summary.NOT_RUN {\\n    border-bottom: 5px solid var(--not-run-background-color);\\n}\\n\\n/* .span_link::after {\\n    content: \\" ⮳\\";\\n} */\\n.span_link {\\n    cursor: pointer;\\n    /* text-decoration: underline; */\\n}\\n\\nsummary:hover {\\n    background-color: var(--summary-hover-background-color);\\n}\\n",""]);const a=s},645:e=>{e.exports=function(e){var t=[];return t.toString=function(){return this.map((function(t){var n=e(t);return t[2]?"@media ".concat(t[2]," {").concat(n,"}"):n})).join("")},t.i=function(e,n,o){"string"==typeof e&&(e=[[null,e,""]]);var s={};if(o)for(var a=0;a<this.length;a++){var r=this[a][0];null!=r&&(s[r]=!0)}for(var i=0;i<e.length;i++){var d=[].concat(e[i]);o&&s[d[0]]||(n&&(d[2]?d[2]="".concat(n," and ").concat(d[2]):d[2]=n),t.push(d))}},t}},391:(e,t,n)=>{let o;window.setVSCodeAPI=function(e){o=e};let s={};function a(e){let t;try{t=o}catch(e){}t&&t.postMessage(e)}let r={output:void 0},i={setContents:void 0,appendContents:void 0,updateLabel:void 0};window.addEventListener("message",(e=>{let t=e.data;if(t)switch(t.type){case"response":let e=t,n=s[e.request_seq];n&&(delete s[e.request_seq],n(e));break;case"event":let o=r[t.event];o?o(t):console.log("Unhandled event: ",t);break;case"request":let a=i[t.command];a?a(t):console.log("Unhandled request: ",t)}}));let d=0;function l(){return d+=1,d}let c={filterLevel:"PASS",runIdToTreeState:{},runIdLRU:[]},u={initialContents:void 0,runId:void 0,state:void 0,onClickReference:void 0,appendedContents:[],allRunIdsToLabel:{},showTime:!0,showExpand:!0};function m(){return void 0===u.state&&(u.state=function(){let e;try{e=o}catch(e){}if(e){let t=e.getState();return t||(t=c),void 0===t.filterLevel&&(t.filterLevel="PASS"),void 0===t.runIdToTreeState&&(t.runIdToTreeState={}),void 0===!t.runIdLRU&&(t.runIdLRU=[]),t}return c}()),u}function h(e){return document.getElementById(e)}function p(e){return h(e)}function f(e){return h(e)}function g(e){const t=document.createElement("ul");return t.setAttribute("data-tree-id",e),t}function v(){return document.createElement("span")}function E(){return document.createElement("button")}function y(){return document.createElement("div")}function b(e){return e.getAttribute("data-tree-id")}function S(e,t=undefined){if(void 0===t)return"1"===e.getAttribute("data-hidden");t?e.setAttribute("data-hidden","1"):e.removeAttribute("data-hidden")}function C(e){var t=document.createElement("template");return e=e.trim(),t.innerHTML=e,t.content.firstChild}function T(e,t){for(let n of t.childNodes)if(n instanceof HTMLDetailsElement){for(let t of n.childNodes)t instanceof HTMLUListElement&&N(e,t);n.open?e.openNodes[b(t)]="open":delete e.openNodes[b(t)]}}function N(e,t){for(let n of t.childNodes)n instanceof HTMLLIElement&&T(e,n)}const L=((e,t)=>{let n;return function(...e){clearTimeout(n),n=setTimeout((()=>{clearTimeout(n),(()=>{w()})(...e)}),500)}})();function w(){const e=m();!function(e,t){const n=p("mainTree");let o={openNodes:{}};if(void 0===e.runIdLRU&&(e.runIdLRU=[]),void 0===e.runIdToTreeState)e.runIdToTreeState={};else{const n=e.runIdToTreeState[t];n&&(o=n)}for(let e of n.childNodes)e instanceof HTMLUListElement&&N(o,e);e.runIdToTreeState[t]=o;const s=e.runIdLRU.indexOf(t);for(s>-1&&e.runIdLRU.splice(s,1),e.runIdLRU.push(t);e.runIdLRU.length>15;){const t=e.runIdLRU.splice(0,1);delete e.runIdToTreeState[t[0]]}}(e.state,e.runId),function(e){let t;try{t=o}catch(e){}t?t.setState(e):c=e}(e.state)}function I(e,t){if(void 0===e)return;const n=f("selectedRun"),o=new Map;for(let s of n.childNodes)if(s instanceof HTMLOptionElement){const n=s,a=n.value,r=e[a];if(void 0===r)s.remove();else{n.text!==r&&(n.text=r),o.set(a,r);const e=t==a;n.selected=e}}for(const s of Object.keys(e)){if(void 0===s)continue;const a=t==s;if(!o.has(s)){const t=document.createElement("option"),r=e[s];t.value=s,n.appendChild(t),t.selected=a,t.text=r,o.set(s,r)}}}Math.pow(10,8);var x=36e5;function M(e,t){var n;!function(e,t){if(t.length<1)throw new TypeError("1 argument required, but only "+t.length+" present")}(0,arguments);var o=function(e){if(null===e||!0===e||!1===e)return NaN;var t=Number(e);return isNaN(t)?t:t<0?Math.ceil(t):Math.floor(t)}(null!==(n=null==t?void 0:t.additionalDigits)&&void 0!==n?n:2);if(2!==o&&1!==o&&0!==o)throw new RangeError("additionalDigits must be 0, 1 or 2");if("string"!=typeof e&&"[object String]"!==Object.prototype.toString.call(e))return new Date(NaN);var s,a=function(e){var t,n={},o=e.split(R.dateTimeDelimiter);if(o.length>2)return n;if(/:/.test(o[0])?t=o[0]:(n.date=o[0],t=o[1],R.timeZoneDelimiter.test(n.date)&&(n.date=e.split(R.timeZoneDelimiter)[0],t=e.substr(n.date.length,e.length))),t){var s=R.timezone.exec(t);s?(n.time=t.replace(s[1],""),n.timezone=s[1]):n.time=t}return n}(e);if(a.date){var r=function(e,t){var n=new RegExp("^(?:(\\\\d{4}|[+-]\\\\d{"+(4+t)+"})|(\\\\d{2}|[+-]\\\\d{"+(2+t)+"})$)"),o=e.match(n);if(!o)return{year:NaN,restDateString:""};var s=o[1]?parseInt(o[1]):null,a=o[2]?parseInt(o[2]):null;return{year:null===a?s:100*a,restDateString:e.slice((o[1]||o[2]).length)}}(a.date,o);s=function(e,t){if(null===t)return new Date(NaN);var n=e.match(k);if(!n)return new Date(NaN);var o=!!n[4],s=D(n[1]),a=D(n[2])-1,r=D(n[3]),i=D(n[4]),d=D(n[5])-1;if(o)return function(e,t,n){return t>=1&&t<=53&&n>=0&&n<=6}(0,i,d)?function(e,t,n){var o=new Date(0);o.setUTCFullYear(e,0,4);var s=7*(t-1)+n+1-(o.getUTCDay()||7);return o.setUTCDate(o.getUTCDate()+s),o}(t,i,d):new Date(NaN);var l=new Date(0);return function(e,t,n){return t>=0&&t<=11&&n>=1&&n<=(O[t]||(H(e)?29:28))}(t,a,r)&&function(e,t){return t>=1&&t<=(H(e)?366:365)}(t,s)?(l.setUTCFullYear(t,a,Math.max(s,r)),l):new Date(NaN)}(r.restDateString,r.year)}if(!s||isNaN(s.getTime()))return new Date(NaN);var i,d=s.getTime(),l=0;if(a.time&&(l=function(e){var t=e.match(_);if(!t)return NaN;var n=F(t[1]),o=F(t[2]),s=F(t[3]);return function(e,t,n){return 24===e?0===t&&0===n:n>=0&&n<60&&t>=0&&t<60&&e>=0&&e<25}(n,o,s)?n*x+6e4*o+1e3*s:NaN}(a.time),isNaN(l)))return new Date(NaN);if(!a.timezone){var c=new Date(d+l),u=new Date(0);return u.setFullYear(c.getUTCFullYear(),c.getUTCMonth(),c.getUTCDate()),u.setHours(c.getUTCHours(),c.getUTCMinutes(),c.getUTCSeconds(),c.getUTCMilliseconds()),u}return i=function(e){if("Z"===e)return 0;var t=e.match(A);if(!t)return 0;var n="+"===t[1]?-1:1,o=parseInt(t[2]),s=t[3]&&parseInt(t[3])||0;return function(e,t){return t>=0&&t<=59}(0,s)?n*(o*x+6e4*s):NaN}(a.timezone),isNaN(i)?new Date(NaN):new Date(d+l+i)}var R={dateTimeDelimiter:/[T ]/,timeZoneDelimiter:/[Z ]/i,timezone:/([Z+-].*)$/},k=/^-?(?:(\\d{3})|(\\d{2})(?:-?(\\d{2}))?|W(\\d{2})(?:-?(\\d{1}))?|)$/,_=/^(\\d{2}(?:[.,]\\d*)?)(?::?(\\d{2}(?:[.,]\\d*)?))?(?::?(\\d{2}(?:[.,]\\d*)?))?$/,A=/^([+-])(\\d{2})(?::?(\\d{2}))?$/;function D(e){return e?parseInt(e):1}function F(e){return e&&parseFloat(e.replace(",","."))||0}var O=[31,null,31,30,31,30,31,31,30,31,30,31];function H(e){return e%400==0||e%4==0&&e%100!=0}function U(e,t){const n=e.memo[t];return void 0===n?`<ref not found: ${t}>`:n}function B(e,t){return parseFloat(t)}function P(e,t){return parseInt(t)}function $(e,t){return t}function j(e){const t=[],n=new Map;for(let o of e.split(",")){o=o.trim();let e="oid";if(-1!=o.indexOf(":")&&([o,e]=o.split(":",2)),t.push(o),"oid"===e)n.set(o,U);else if("int"===e)n.set(o,P);else if("float"===e)n.set(o,B);else{if("str"!==e)throw new Error("Unexpected: "+e);n.set(o,$)}}return function(e,o){const s=o.split("|",t.length),a={};for(let o=0;o<s.length;o++){const r=s[o],i=t[o];a[i]=n.get(i)(e,r)}return a}}const z=j("part:int, id:str"),V={V:j("version:str"),ID:z,I:function(e,t){return JSON.parse(t)},T:function(e,t){return{time:M(t).toString()}},M:function(e,t){var n,o;const s=W(t,":");if(s){[n,o]=s;try{o=JSON.parse(o)}catch(e){return console.log("Error parsing json: "+o),console.log(e),null}e.memo[n]=o}return null},SR:j("name:oid, time_delta_in_seconds:float"),ER:j("status:oid, time_delta_in_seconds:float"),ST:j("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),ET:j("status:oid, message:oid, time_delta_in_seconds:float"),SE:j("name:oid, libname:oid, type:oid, doc:oid, source:oid, lineno:int, time_delta_in_seconds:float"),EE:j("type:oid, status:oid, time_delta_in_seconds:float"),EA:j("name:oid, type:oid, value:oid"),AS:j("source:oid, lineno:int, target:oid, type:oid, value:oid, time_delta_in_seconds:float"),L:j("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),LH:j("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),TG:j("tag:oid"),S:j("start_time_delta:float"),STB:j("message:oid, time_delta_in_seconds:float"),RTB:j("message:oid, time_delta_in_seconds:float"),TBE:j("source:oid, lineno:int, method:oid, line_content:oid"),TBV:j("name:oid, type:oid, value:oid"),ETB:j("time_delta_in_seconds:float"),YS:j("source:oid, lineno:int, type:oid, value:oid, time_delta_in_seconds:float"),YR:j("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float")};V.RR=V.SR,V.RT=V.ST,V.RE=V.SE,V.RYR=V.YR;class Y{constructor(){this.memo={}}decode_message_type(e,t){return(0,V[e])(this,t)}}function W(e,t){const n=e.indexOf(t);if(n>0)return[e.substring(0,n),e.substring(n+1)]}function*q(e,t){var n,o,s;for(let a of e.split(/\\r?\\n/))if(a=a.trim(),a)try{const e=W(a," ");if(e&&([s,o]=e,n=t.decode_message_type(s,o))){const e={message_type:s,decoded:n};yield e}}catch(e){console.log("Unable to decode message: "+a),console.log(e)}}function J(e,t){const n=document.createElement("span");n.textContent=t,n.classList.add("label"),n.classList.add(t.replace(" ","_")),e.summaryDiv.insertBefore(n,e.summaryDiv.firstChild)}function G(e,t){switch(e.state.filterLevel){case"FAIL":return t>=2;case"WARN":return t>=1;case"PASS":return t>=0;case"NOT RUN":return!0}}function Z(e){switch(e){case"FAIL":case"ERROR":return 2;case"WARN":return 1;case"NOT RUN":case"NOT_RUN":return-1;default:return 0}}class K{constructor(e){this.stack=[],this.exceptionMsg=e}pushEntry(e,t,n,o){const s=new Map;this.stack.push({source:e,lineno:t,method:n,lineContent:o,variables:s})}pushVar(e,t,n){this.stack.at(-1).variables.set(e,[t,n])}}class Q{constructor(){this.totalTests=0,this.totalFailures=0}clear(){this.totalTests=0,this.totalFailures=0,this.updateSummary()}onTestEndUpdateSummary(e){const t=e.decoded.status;this.totalTests+=1,"FAIL"!=t&&"ERROR"!=t||(this.totalFailures+=1),this.updateSummary()}updateSummary(){const e=p("summary");if(!e)return;const t=(""+this.totalTests).padStart(4),n=(""+this.totalFailures).padStart(4);if(e.textContent=`Total: ${t} Failures: ${n}`,0==this.totalFailures&&0==this.totalTests){const e=p("summary");e.classList.add("NOT_RUN"),e.classList.remove("PASS"),e.classList.remove("FAIL")}else if(1==this.totalFailures){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("PASS"),e.classList.add("FAIL")}else if(0==this.totalFailures&&1==this.totalTests){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("FAIL")}}}function X(e,t){const n=function(e){const t=document.createElement("li");return t.setAttribute("data-tree-id",e),t}(t),o=document.createElement("details");e&&(o.open=e),o.classList.add("NO_CHILDREN"),n.appendChild(o);const s=y();s.classList.add("detailContainer"),o.appendChild(s);const a=document.createElement("summary"),r=y();r.classList.add("summaryDiv"),a.appendChild(r);const i=v();i.className="summaryName",i.textContent="[summaryName]",r.appendChild(i);const d=v();return d.className="summaryInput emptySummaryInput",d.textContent="",r.appendChild(d),o.appendChild(a),{li:n,details:o,summary:a,summaryDiv:r,summaryName:i,summaryInput:d,detailContainer:s}}function ee(e,t){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${t}`,e.summaryInput.classList.remove("emptySummaryInput")):e.summaryInput.textContent+=`, ${t}`}function te(e,t,n,o,s,a,r,i,d,l){const c=e.state.runIdToTreeState[e.runId],u="li_"+l;if(c){const e=c.openNodes;e&&(a=e[u])}const m=X(a,u),h=m.li,p=m.details,f=m.detailContainer,v=m.summary,E=m.summaryDiv,y=m.summaryName,b=m.summaryInput;if("LH"===s.message_type){y.textContent="";const e=C(n);y.appendChild(e)}else y.textContent=n;o&&(y.title=o),e.onClickReference&&(y.classList.add("span_link"),y.onclick=t=>{const n=[];let o=d.parent;for(;void 0!==o&&void 0!==o.message;)n.push(o.message),o=o.parent;t.preventDefault(),e.onClickReference({source:r,lineno:i,message:s.decoded,messageType:s.message_type,scope:n})});const S=g("ul_"+l);p.appendChild(S);const T={ul:S,li:h,details:p,detailContainer:f,summary:v,summaryName:y,summaryInput:b,source:r,lineno:i,appendContentChild:void 0,decodedMessage:s,maxLevelFoundInHierarchy:-1,summaryDiv:E};return T.appendContentChild=re.bind(T),t.appendContentChild(T),T}let ne,oe;function*se(e){for(let t of e.childNodes)if(t instanceof HTMLDetailsElement){for(let e of t.childNodes)if(e instanceof HTMLUListElement)for(let t of ae(e))yield t;yield t}}function*ae(e){for(let t of e.childNodes)if(t instanceof HTMLLIElement)for(let e of se(t))yield e}function re(e){const t=this;t.ul.appendChild(e.li),t.details.classList.contains("NO_CHILDREN")&&(t.details.classList.remove("NO_CHILDREN"),t.details.addEventListener("toggle",(function(){L()})),m().showExpand&&t.summary.addEventListener("mouseover",(e=>{!function(e){if(void 0===ne){ne=y(),ne.classList.add("toolbarContainer");const e=E();e.appendChild(C(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path d="M7 12V7H6v5h1z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),e.onclick=()=>{!function(){if(void 0!==oe){oe.details.open=!0;for(let e of ae(oe.ul))e.classList.contains("NO_CHILDREN")||(e.open=!0)}}()},e.classList.add("toolbarButton");const t=E();return t.appendChild(C(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),t.classList.add("toolbarButton"),t.onclick=()=>{!function(){if(void 0!==oe){oe.details.open=!1;for(let e of ae(oe.ul))e.open=!1}}()},ne.appendChild(t),void ne.appendChild(e)}oe=e,e.summaryDiv.appendChild(ne)}(t)})))}var ie=(e,t,n)=>new Promise(((o,s)=>{var a=e=>{try{i(n.next(e))}catch(e){s(e)}},r=e=>{try{i(n.throw(e))}catch(e){s(e)}},i=e=>e.done?o(e.value):Promise.resolve(e.value).then(a,r);i((n=n.apply(e,t)).next())}));let de=0,le=-1;class ce{constructor(){this.stack=[]}handle(e){let t;switch(e.message_type){case"STB":return void this.stack.push(new K(e.decoded.message));case"TBE":return t=this.stack.at(-1),void t.pushEntry(e.decoded.source,e.decoded.lineno,e.decoded.method,e.decoded.line_content);case"TBV":return;case"ETB":return t=this.stack.pop(),t.stack.reverse(),t}}}class ue{constructor(){this.stack=[],this.messageNode={parent:void 0,message:void 0},this.id=0,this.finishedAddingInitialContents=!1,this.appendedMessagesIndex=-1,this.decoder=new Y,this.seenSuiteTaskOrElement=!1,this.tbHandler=new ce,this.suiteErrored=!1,this.opts=m(),this.runId=this.opts.runId,this.summaryBuilder=new Q,this.lease=(de+=1,le=de,de),this.resetState()}resetState(){this.seenSuiteTaskOrElement=!1}isCurrentTreeBuilder(){return this.lease===le&&this.runId==this.opts.runId}clearAndInitializeTree(){this.summaryBuilder.clear(),this.resetState();const e=f("filterLevel");e&&(e.value=this.opts.state.filterLevel);const t=p("mainTree");t.replaceChildren();const n=g("ul_root");n.classList.add("tree"),t.appendChild(n),this.parent={ul:void 0,li:void 0,details:void 0,detailContainer:void 0,summary:void 0,summaryName:void 0,summaryInput:void 0,source:void 0,lineno:void 0,decodedMessage:void 0,appendContentChild:function(e){n.appendChild(e.li)},maxLevelFoundInHierarchy:-1,summaryDiv:void 0},this.stack.push(this.parent)}addInitialContents(){return ie(this,null,(function*(){for(const e of q(this.opts.initialContents,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}this.finishedAddingInitialContents=!0,yield this.onAppendedContents()}))}onAppendedContents(){return ie(this,null,(function*(){if(!this.finishedAddingInitialContents)return;if(!this.isCurrentTreeBuilder())return;const e=m();for(;this.appendedMessagesIndex+1<e.appendedContents.length;){this.appendedMessagesIndex+=1;const t=e.appendedContents[this.appendedMessagesIndex];for(const e of q(t,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}}}))}addOneMessage(e){return ie(this,null,(function*(){if(this.isCurrentTreeBuilder())try{this.addOneMessageSync(e)}catch(t){console.log("Error: handling message: "+JSON.stringify(e)+": "+t+" - "+JSON.stringify(t))}}))}addOneMessageSync(e){var t,n;let o,s,a=e.message_type;switch(a){case"SR":case"ST":case"SE":case"STB":this.seenSuiteTaskOrElement=!0;break;case"RR":if(this.seenSuiteTaskOrElement)return;a="SR";break;case"RT":if(this.seenSuiteTaskOrElement)return;a="ST";break;case"RE":if(this.seenSuiteTaskOrElement)return;a="SE";break;case"RTB":if(this.seenSuiteTaskOrElement)return;a="STB"}switch(this.id+=1,a){case"SR":this.messageNode={parent:this.messageNode,message:e};for(const t of document.querySelectorAll(".suiteHeader"))t.textContent=e.decoded.name;break;case"AS":s=te(this.opts,this.parent,`${e.decoded.target} = `,`Assign to name: ${e.decoded.target}\\nAn object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),ee(s,e.decoded.value),this.addAssignCssClass(s);break;case"ST":this.messageNode={parent:this.messageNode,message:e},this.parent=te(this.opts,this.parent,`${e.decoded.libname}.${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"SE":case"YR":if("SE"!=a||"UNTRACKED_GENERATOR"!=e.decoded.type){this.messageNode={parent:this.messageNode,message:e};let t=e.decoded.name;"YR"==a&&(t+=" (resumed)"),this.parent=te(this.opts,this.parent,t,e.decoded.libname,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),"YR"==a&&this.addResumedCSSClass(this.parent),this.stack.push(this.parent)}else{const t=te(this.opts,this.parent,`Create Generator: ${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addGeneratorCSSClass(t)}break;case"ER":this.messageNode=this.messageNode.parent;{const t=p("suiteResult");t.style.display="block",this.suiteErrored?(t.classList.add("ERROR"),t.textContent="Run Failed"):(t.classList.add("PASS"),t.textContent="Run Passed");const n=p("suiteRunStart");n&&(n.textContent+=` - Finished in: ${e.decoded.time_delta_in_seconds.toFixed(2)}s.`)}break;case"ET":this.messageNode=this.messageNode.parent;const r=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(r,this.parent,e),this.onEndSetStatusOrRemove(this.opts,r,e.decoded,this.parent,!1),this.summaryBuilder.onTestEndUpdateSummary(e),o=this.addDetailsCSSClasses(e.decoded.status,r),o&&(this.suiteErrored=!0,r.details.open=!0);break;case"EE":case"YS":if("EE"!=a||"UNTRACKED_GENERATOR"!=e.decoded.type){if("YS"==a){const t=te(this.opts,this.parent,"Yielded",`Suspending function with yield.\\nYielding an object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addYieldedCSSClass(t),ee(t,e.decoded.value)}this.messageNode=this.messageNode.parent;let t=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(t,this.parent,e),this.onEndSetStatusOrRemove(this.opts,t,e.decoded,this.parent,!0),o=this.addDetailsCSSClasses(e.decoded.status,t),o&&(t.details.open=!0)}break;case"S":const i=e.decoded.start_time_delta;(null==(n=null==(t=this.parent)?void 0:t.decodedMessage)?void 0:n.decoded)&&(this.parent.decodedMessage.decoded.time_delta_in_seconds=i);break;case"EA":s=this.stack.at(-1),function(e,t,n,o){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${t} = ${o}`,e.summaryInput.title=`Argument: ${t}\\nArgument type: ${n}\\nRepresentation:\\n${o}`,e.summaryInput.classList.remove("emptySummaryInput")):(e.summaryInput.title+=`\\n\\nArgument: ${t}\\nArgument type: ${n}\\nRepresentation:\\n${o}`,e.summaryInput.textContent+=`, ${t} = ${o}`)}(s,e.decoded.name,e.decoded.type,e.decoded.value);break;case"L":case"LH":const d=e.decoded.level,l=function(e){switch(e){case"E":case"F":return 2;case"W":return 1;default:return 0}}(d);if(l>this.parent.maxLevelFoundInHierarchy&&(this.parent.maxLevelFoundInHierarchy=l),G(this.opts,l)){const t=te(this.opts,this.parent,e.decoded.message,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());t.maxLevelFoundInHierarchy=l,function(e,t){const n=document.createElement("span");n.textContent=`LOG ${function(e){switch(e){case"E":return"ERROR";case"F":return"FAIL";case"W":return"WARN";case"I":return"INFO";default:return e}}(t)}`,n.classList.add("label"),n.classList.add(t.replace(" ","_")),e.summaryDiv.insertBefore(n,e.summaryDiv.firstChild)}(t,d),this.addDetailsCSSClasses(l,t)}break;case"STB":case"TBE":case"TBV":case"ETB":const c=this.tbHandler.handle(e);if(c&&c.stack.length>0){const t=c.stack[0];s=te(this.opts,this.parent,c.exceptionMsg,"",e,!1,t.source,t.lineno,this.messageNode,this.id.toString()),this.addExceptionCssClass(s)}break;case"T":const u=p("suiteRunStart");u&&(u.textContent=e.decoded.time)}}addAssignCssClass(e){e.details.classList.add("variableParent"),e.details.classList.add("leafNode")}addExceptionCssClass(e){e.details.classList.add("exceptionParent"),e.details.classList.add("leafNode")}addYieldedCSSClass(e){e.details.classList.add("yiededParent"),e.details.classList.add("leafNode")}addResumedCSSClass(e){e.details.classList.add("resumedParent")}addGeneratorCSSClass(e){e.details.classList.add("generatorParent"),e.details.classList.add("leafNode")}addDetailsCSSClasses(e,t){let n,o=!1;return n="string"==typeof e?Z(e):e,n>=2?(t.details.classList.add("errorParent"),o=!0):1==n?t.details.classList.add("warnParent"):t.details.classList.add("passParent"),t.details.classList.contains("parentNode")||t.details.classList.contains("leafNode")||(0===t.ul.children.length?t.details.classList.add("leafNode"):t.details.classList.add("parentNode")),o}onEndUpdateMaxLevelFoundInHierarchyFromStatus(e,t,n){const o=Z(n.decoded.status);o>e.maxLevelFoundInHierarchy&&(e.maxLevelFoundInHierarchy=o),e.maxLevelFoundInHierarchy>t.maxLevelFoundInHierarchy&&(t.maxLevelFoundInHierarchy=e.maxLevelFoundInHierarchy)}onEndSetStatusOrRemove(e,t,n,o,s){const a=n.status;if(G(e,t.maxLevelFoundInHierarchy)){if(s&&t.maxLevelFoundInHierarchy<=0){const e=50;if(o.ul.childElementCount>e){const e=t.summaryName.textContent;if(e&&e.toLowerCase().includes("iteration")){const e=t.li.previousSibling,n=b(t.li);if(t.li.remove(),S(e))e.getElementsByClassName("FINAL_SPAN")[0].textContent=t.summaryName.textContent;else{const e=X(!1,n);e.summaryName.textContent=t.summaryName.textContent,e.summary.classList.add("HIDDEN");const s=v();s.setAttribute("role","button"),s.textContent="...",s.classList.add("label"),s.classList.add("HIDDEN"),s.classList.add("inline"),e.summaryDiv.appendChild(s);const a=v();a.setAttribute("role","button"),a.classList.add("FINAL_SPAN"),e.summaryDiv.appendChild(a),J(e,"HIDDEN"),S(e.li,!0),o.ul.appendChild(e.li)}return}}}if(t.summary,J(t,a),null!=t.source&&t.source.length>0){const e=function(e){let t=e,n=Math.max(e.lastIndexOf("/"),e.lastIndexOf("\\\\"));return n>0&&(t=e.substring(n+1)),t}(t.source),n=document.createElement("span");n.textContent=e,n.classList.add("summaryFileName"),n.title=t.source,t.summaryDiv.appendChild(n)}if(this.opts.showTime){const e=t.decodedMessage.decoded.time_delta_in_seconds;void 0!==e&&e>=0&&function(e,t){const n=document.createElement("span");n.textContent=` (${t.toFixed(2)}s)`,n.classList.add("timeLabel"),e.summaryDiv.appendChild(n)}(t,n.time_delta_in_seconds-e)}}else t.li.remove()}}var me=(e,t,n)=>new Promise(((o,s)=>{var a=e=>{try{i(n.next(e))}catch(e){s(e)}},r=e=>{try{i(n.throw(e))}catch(e){s(e)}},i=e=>e.done?o(e.value):Promise.resolve(e.value).then(a,r);i((n=n.apply(e,t)).next())}));let he;function pe(){return me(this,null,(function*(){he=new ue,he.clearAndInitializeTree(),yield he.addInitialContents()}))}function fe(e){let t={type:"event",seq:l(),event:"onClickReference"};t.data=e,a(t)}function ge(e){w();const t=m();t.runId=e.runId,t.initialContents=e.initialContents,void 0!==o&&(t.onClickReference=fe),t.appendedContents=[],t.allRunIdsToLabel=e.allRunIdsToLabel,I(t.allRunIdsToLabel,t.runId),pe()}n(320),i.setContents=ge,i.appendContents=function(e){const t=m();t.runId===e.runId&&(t.appendedContents.push(e.appendContents),void 0!==he&&he.onAppendedContents())},i.updateLabel=function(e){const t=m();t.allRunIdsToLabel[e.runId]=e.label,I(t.allRunIdsToLabel,t.runId)},window.onChangedRun=function(){const e=f("selectedRun").value;let t={type:"event",seq:l(),event:"onSetCurrentRunId"};t.data={runId:e},a(t)},window.onChangedFilterLevel=function(){!function(e){const t=m();t.state.filterLevel!==e&&(t.state.filterLevel=e,w(),pe())}(f("filterLevel").value)},window.setContents=ge,window.setShowTime=function(e){m().showTime=e},window.setShowExpand=function(e){m().showExpand=e},window.getSampleContents=function(){return JSON.parse(\'"V 1\\\\nI \\\\"sys.platform=win32\\\\"\\\\nI \\\\"python=3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)]\\\\"\\\\nI \\\\"robot=5.1a3.dev1\\\\"\\\\nT 2022-10-19T09:48:34.018\\\\nM a:\\\\"Robot1\\\\"\\\\nM b:\\\\"s1\\\\"\\\\nM c:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\robot1.robot\\\\"\\\\nSR a|b|c|0.035\\\\nM d:\\\\"Simple Task\\\\"\\\\nM e:\\\\"s1-t1\\\\"\\\\nST d|e|16|0.036\\\\nM f:\\\\"First keyword\\\\"\\\\nM g:\\\\"\\\\"\\\\nM h:\\\\"KEYWORD\\\\"\\\\nSE f|g|h|g|c|17|0.036\\\\nM i:\\\\"No Operation\\\\"\\\\nM j:\\\\"BuiltIn\\\\"\\\\nM k:\\\\"Does absolutely nothing.\\\\"\\\\nSE i|j|h|k|c|8|0.037\\\\nM l:\\\\"PASS\\\\"\\\\nEE l|0.037\\\\nM m:\\\\"Log\\\\"\\\\nM n:\\\\"Logs the given message with the given level.\\\\"\\\\nSE m|j|h|n|c|10|0.037\\\\nM o:\\\\"Some warning message\\\\"\\\\nEA o\\\\nM p:\\\\"level=WARN\\\\"\\\\nEA p\\\\nEE l|0.046\\\\nM q:\\\\"Another keyword\\\\"\\\\nM r:\\\\"another\\\\"\\\\nSE q|r|h|g|c|11|0.047\\\\nM s:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\another.robot\\\\"\\\\nSE i|j|h|k|s|3|0.047\\\\nEE l|0.047\\\\nEE l|0.047\\\\nM t:\\\\"Another in sub keyword\\\\"\\\\nM u:\\\\"another_sub\\\\"\\\\nSE t|u|h|g|c|12|0.047\\\\nM v:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\sub\\\\\\\\\\\\\\\\another_sub.robot\\\\"\\\\nSE i|j|h|k|v|6|0.048\\\\nEE l|0.048\\\\nSE m|j|h|n|v|7|0.048\\\\nM w:\\\\"Some error message\\\\"\\\\nEA w\\\\nM x:\\\\"level=ERROR\\\\"\\\\nEA x\\\\nEE l|0.049\\\\nEE l|0.049\\\\nEE l|0.049\\\\nSE m|j|h|n|c|18|0.049\\\\nM y:\\\\"Some <data &encode <\\/script>\\\\"\\\\nEA y\\\\nEE l|0.049\\\\nM z:\\\\"Create Dictionary\\\\"\\\\nM A:\\\\"Creates and returns a dictionary based on the given ``items``.\\\\"\\\\nSE z|j|h|A|c|19|0.049\\\\nM B:\\\\"a=1\\\\"\\\\nEA B\\\\nM C:\\\\"b=1\\\\"\\\\nEA C\\\\nEE l|0.05\\\\nSE m|j|h|n|c|20|0.05\\\\nM D:\\\\"${dct}\\\\"\\\\nEA D\\\\nEE l|0.051\\\\nET l|g|0.051\\\\nM E:\\\\"Check 1\\\\"\\\\nM F:\\\\"s1-t2\\\\"\\\\nST E|F|22|0.051\\\\nSE f|g|h|g|c|23|0.051\\\\nSE i|j|h|k|c|8|0.052\\\\nEE l|0.052\\\\nSE m|j|h|n|c|10|0.052\\\\nEA o\\\\nEA p\\\\nEE l|0.052\\\\nSE q|r|h|g|c|11|0.053\\\\nSE i|j|h|k|s|3|0.053\\\\nEE l|0.053\\\\nEE l|0.053\\\\nSE t|u|h|g|c|12|0.053\\\\nSE i|j|h|k|v|6|0.054\\\\nEE l|0.054\\\\nSE m|j|h|n|v|7|0.054\\\\nEA w\\\\nEA x\\\\nEE l|0.054\\\\nEE l|0.055\\\\nEE l|0.055\\\\nM G:\\\\"${counter} IN RANGE [ 0 | 3 ]\\\\"\\\\nM H:\\\\"FOR\\\\"\\\\nSE G|g|H|g|c|25|0.055\\\\nM I:\\\\"${counter} = 0\\\\"\\\\nM J:\\\\"ITERATION\\\\"\\\\nSE I|g|J|g|c|25|0.055\\\\nM K:\\\\"${counter} == 2\\\\"\\\\nM L:\\\\"IF\\\\"\\\\nSE K|g|L|g|c|26|0.055\\\\nM M:\\\\"Fail\\\\"\\\\nM N:\\\\"Fails the test with the given message and optionally alters its tags.\\\\"\\\\nSE M|j|h|N|c|27|0.056\\\\nM O:\\\\"Failed execution for some reason...\\\\"\\\\nEA O\\\\nM P:\\\\"NOT RUN\\\\"\\\\nEE P|0.056\\\\nEE P|0.056\\\\nSE m|j|h|n|c|29|0.056\\\\nM Q:\\\\"${counter}\\\\"\\\\nEA Q\\\\nEE l|0.056\\\\nEE l|0.057\\\\nM R:\\\\"${counter} = 1\\\\"\\\\nSE R|g|J|g|c|25|0.057\\\\nSE K|g|L|g|c|26|0.057\\\\nSE M|j|h|N|c|27|0.057\\\\nEA O\\\\nEE P|0.057\\\\nEE P|0.057\\\\nSE m|j|h|n|c|29|0.058\\\\nEA Q\\\\nEE l|0.058\\\\nEE l|0.058\\\\nM S:\\\\"${counter} = 2\\\\"\\\\nSE S|g|J|g|c|25|0.058\\\\nSE K|g|L|g|c|26|0.058\\\\nSE M|j|h|N|c|27|0.059\\\\nEA O\\\\nM T:\\\\"FAIL\\\\"\\\\nEE T|0.059\\\\nEE T|0.059\\\\nSE m|j|h|n|c|29|0.059\\\\nEA Q\\\\nEE P|0.059\\\\nEE T|0.06\\\\nEE T|0.06\\\\nET T|O|0.06\\\\nM U:\\\\"Check 2\\\\"\\\\nM V:\\\\"s1-t3\\\\"\\\\nST U|V|32|0.06\\\\nM W:\\\\"Set Variable\\\\"\\\\nM X:\\\\"Returns the given values which can then be assigned to a variables.\\\\"\\\\nSE W|j|h|X|c|33|0.061\\\\nM Y:\\\\"3\\\\"\\\\nEA Y\\\\nEE l|0.061\\\\nM Z:\\\\"${counter} <= 2\\\\"\\\\nM 0:\\\\"WHILE\\\\"\\\\nSE Z|g|0|g|c|34|0.061\\\\nSE g|g|J|g|c|34|0.062\\\\nM 1:\\\\"Evaluate\\\\"\\\\nM 2:\\\\"Evaluates the given expression in Python and returns the result.\\\\"\\\\nSE 1|j|h|2|c|35|0.062\\\\nM 4:\\\\"$counter-1\\\\"\\\\nEA 4\\\\nEE P|0.062\\\\nSE m|j|h|n|c|36|0.062\\\\nM 5:\\\\"Current counter: ${counter}\\\\"\\\\nEA 5\\\\nEA p\\\\nEE P|0.062\\\\nEE P|0.062\\\\nEE P|0.063\\\\nET l|g|0.063\\\\nM 6:\\\\"Check 3\\\\"\\\\nM 7:\\\\"s1-t4\\\\"\\\\nST 6|7|39|0.064\\\\nM 8:\\\\"TRY\\\\"\\\\nSE g|g|8|g|c|40|0.064\\\\nSE i|j|h|k|c|41|0.064\\\\nEE l|0.064\\\\nEE l|0.064\\\\nM 9:\\\\"message\\\\"\\\\nM aa:\\\\"EXCEPT\\\\"\\\\nSE 9|g|aa|g|c|42|0.064\\\\nSE i|j|h|k|c|43|0.065\\\\nEE P|0.065\\\\nEE P|0.065\\\\nM ab:\\\\"FINALLY\\\\"\\\\nSE g|g|ab|g|c|44|0.065\\\\nSE i|j|h|k|c|45|0.065\\\\nEE l|0.065\\\\nEE l|0.065\\\\nET l|g|0.066\\\\nER T|0.067\\\\n"\')}},320:(e,t,n)=>{var o=n(379),s=n.n(o),a=n(426),r={injectType:"singletonStyleTag",insert:"head",singleton:!0};s()(a.Z,r),a.Z.locals},379:(e,t,n)=>{var o,s=function(){var e={};return function(t){if(void 0===e[t]){var n=document.querySelector(t);if(window.HTMLIFrameElement&&n instanceof window.HTMLIFrameElement)try{n=n.contentDocument.head}catch(e){n=null}e[t]=n}return e[t]}}(),a=[];function r(e){for(var t=-1,n=0;n<a.length;n++)if(a[n].identifier===e){t=n;break}return t}function i(e,t){for(var n={},o=[],s=0;s<e.length;s++){var i=e[s],d=t.base?i[0]+t.base:i[0],l=n[d]||0,c="".concat(d," ").concat(l);n[d]=l+1;var u=r(c),m={css:i[1],media:i[2],sourceMap:i[3]};-1!==u?(a[u].references++,a[u].updater(m)):a.push({identifier:c,updater:f(m,t),references:1}),o.push(c)}return o}function d(e){var t=document.createElement("style"),o=e.attributes||{};if(void 0===o.nonce){var a=n.nc;a&&(o.nonce=a)}if(Object.keys(o).forEach((function(e){t.setAttribute(e,o[e])})),"function"==typeof e.insert)e.insert(t);else{var r=s(e.insert||"head");if(!r)throw new Error("Couldn\'t find a style target. This probably means that the value for the \'insert\' parameter is invalid.");r.appendChild(t)}return t}var l,c=(l=[],function(e,t){return l[e]=t,l.filter(Boolean).join("\\n")});function u(e,t,n,o){var s=n?"":o.media?"@media ".concat(o.media," {").concat(o.css,"}"):o.css;if(e.styleSheet)e.styleSheet.cssText=c(t,s);else{var a=document.createTextNode(s),r=e.childNodes;r[t]&&e.removeChild(r[t]),r.length?e.insertBefore(a,r[t]):e.appendChild(a)}}function m(e,t,n){var o=n.css,s=n.media,a=n.sourceMap;if(s?e.setAttribute("media",s):e.removeAttribute("media"),a&&"undefined"!=typeof btoa&&(o+="\\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a))))," */")),e.styleSheet)e.styleSheet.cssText=o;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(o))}}var h=null,p=0;function f(e,t){var n,o,s;if(t.singleton){var a=p++;n=h||(h=d(t)),o=u.bind(null,n,a,!1),s=u.bind(null,n,a,!0)}else n=d(t),o=m.bind(null,n,t),s=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(n)};return o(e),function(t){if(t){if(t.css===e.css&&t.media===e.media&&t.sourceMap===e.sourceMap)return;o(e=t)}else s()}}e.exports=function(e,t){(t=t||{}).singleton||"boolean"==typeof t.singleton||(t.singleton=(void 0===o&&(o=Boolean(window&&document&&document.all&&!window.atob)),o));var n=i(e=e||[],t);return function(e){if(e=e||[],"[object Array]"===Object.prototype.toString.call(e)){for(var o=0;o<n.length;o++){var s=r(n[o]);a[s].references--}for(var d=i(e,t),l=0;l<n.length;l++){var c=r(n[l]);0===a[c].references&&(a[c].updater(),a.splice(c,1))}n=d}}}}},t={};function n(o){var s=t[o];if(void 0!==s)return s.exports;var a=t[o]={id:o,exports:{}};return e[o](a,a.exports,n),a.exports}n.n=e=>{var t=e&&e.__esModule?()=>e.default:()=>e;return n.d(t,{a:t}),t},n.d=(e,t)=>{for(var o in t)n.o(t,o)&&!n.o(e,o)&&Object.defineProperty(e,o,{enumerable:!0,get:t[o]})},n.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),n.nc=void 0,n(391),n(320)})();</script></body><script>window.setShowTime(true);\n    window.setShowExpand(true);\n    try {\n        const vscode = acquireVsCodeApi();\n        window.setVSCodeAPI(vscode);\n        document.getElementById("selectRunContainer").style.display = "block";\n    } catch (err) {\n        // That\'s ok (not running in VSCode).\n        window.setContents({\n            "initialContents": window.getSampleContents(),\n        });\n    }</script></html>'}
+FILE_CONTENTS = {'index.html': '<!doctype html><html style="padding: 0 0 0 0; margin: 0 0 0 0; height: 100%"><head><meta charset="utf-8"/><title>Robot Output</title><meta name="viewport" content="width=device-width,initial-scale=1"/></head><body class="vscode-dark" style="padding: 0 0 0 0; margin: 0 0 0 0; height: 100%; display: flex; flex-direction: column"><div style="display: flex"><div class="summaryField" style="flex-grow: 1; white-space: nowrap" id="summary" class="NOT_RUN">Total:&nbsp;&nbsp;&nbsp;&nbsp;Failures:&nbsp;&nbsp;&nbsp;&nbsp;</div><div class="summaryField" style="flex-grow: 1"><div style="display: flex"><span>Filter:&nbsp;</span> <select name="filterLevel" id="filterLevel" style="flex-grow: 1" onchange="window.onChangedFilterLevel()"><option value="FAIL">FAIL</option><option value="WARN">WARN</option><option value="PASS" selected="selected">PASS</option><option value="NOT RUN">NOT RUN</option></select></div></div><div class="summaryField" id="selectRunContainer" style="flex-grow: 2; display: none"><select name="selectedRun" id="selectedRun" onchange="window.onChangedRun()" style="width: 100%"><option value="NO_RUN" selected="selected">No runs available...</option></select></div></div><div id="mainTree" style="white-space: nowrap; overflow: auto; flex-grow: 1"></div><script>(()=>{"use strict";var e={426:(e,t,n)=>{n.d(t,{Z:()=>a});var o=n(645),s=n.n(o)()((function(e){return e[1]}));s.push([e.id,":root {\\n    --fg-color: var(--vscode-editor-foreground, black);\\n    --bg-color: var(--vscode-editor-background, white);\\n    --font-family: var(--vscode-editor-font-family, monospace, courier);\\n    --font-size: var(--vscode-editor-font-size, 14px);\\n    --font-weight: var(--vscode-font-weight);\\n    --menu-background: var(--vscode-menu-background, rgb(235, 235, 235));\\n    --menu-foreground: var(--vscode-menu-foreground, rgb(0, 0, 0));\\n\\n    /* background-color: var(--vscode-editorError-foreground); */\\n    /* background-color: var(--vscode-inputValidation-errorBorder);  high-contrast doesn\'t have a good color */\\n    /* background-color: var(--vscode-testing-iconErrored);  red and green always (not always ideal...) */\\n    --error-background-color: var(--vscode-terminalCommandDecoration-errorBackground, rgb(201, 28, 28));\\n    --error-color: var(--vscode-button-foreground, white);\\n\\n    --hidden-background-color: var(--vscode-foobarcolornotthere, rgb(243, 152, 16));\\n    --hidden-color: var(--vscode-button-foreground, white);\\n\\n    /* background-color: var(--vscode-inputValidation-infoBorder); */\\n    /* background-color: var(--vscode-testing-iconPassed); */\\n    --pass-background-color: var(--vscode-terminalCommandDecoration-successBackground, rgb(36, 47, 202));\\n    --pass-color: var(--vscode-button-foreground, white);\\n\\n    --warn-background-color: var(--vscode-debugConsole-warningForeground, rgb(190, 159, 20));\\n    --warn-color: var(--vscode-button-foreground, white);\\n\\n    --not-run-background-color: var(--vscode-editor-foreground, rgb(102, 102, 102));\\n    --not-run-color: var(--vscode-editor-background, white);\\n\\n    --summary-hover-background-color: var(--vscode-editor-hoverHighlightBackground, rgb(222, 222, 222));\\n\\n    /* \\n    --fg-color: white;\\n    --bg-color: #4b4a4a;\\n    --font-family: \\"Segoe UI\\", Tahoma, Geneva, Verdana, sans-serif; \\n    */\\n}\\n\\n.summaryField {\\n    margin-left: 3px;\\n    margin-right: 3px;\\n}\\n\\n.summaryFileName {\\n    opacity: 0.6;\\n    margin-left: 1rem;\\n}\\n\\n.timeLabel {\\n    opacity: 0.6;\\n}\\n\\n/* .summaryInput {\\n    opacity: 0.6;\\n} */\\n\\n.summaryInput::before {\\n    margin-left: 3px;\\n    content: \\"(\\";\\n}\\n.summaryInput::after {\\n    margin-right: 3px;\\n    content: \\")\\";\\n}\\n\\n/* nesting level vertical line */\\n.detailInfo {\\n    border-left: 1px solid var(--error-background-color);\\n\\n    /* centering the line with the icon */\\n    margin-left: 1.5rem;\\n\\n    /* nesting indentation */\\n    padding-left: 0.8rem;\\n}\\n\\nbody {\\n    font-family: var(--font-family);\\n    font-size: var(--font-size);\\n    font-weight: var(--font-weight);\\n    color: var(--fg-color);\\n    background-color: var(--bg-color);\\n}\\n\\n#mainTree {\\n    margin-top: 5px;\\n}\\n\\nul {\\n    list-style-type: none;\\n    padding-inline-start: 0px;\\n    margin-block-start: 0px;\\n}\\n\\ndiv ul:not(:first-child) {\\n    border-left: 1px dotted rgb(141, 141, 141);\\n}\\n\\n.tree li {\\n    display: block;\\n    position: relative;\\n    padding-left: 0px;\\n}\\n\\n.tree ul {\\n    margin-left: 10px;\\n    padding-left: 0;\\n}\\n\\n.toolbarButton {\\n    display: inline;\\n    border-radius: 5px;\\n    background: var(--bg-color);\\n    color: var(--fg-color);\\n    margin-left: 3px;\\n    width: 15px;\\n    height: 15px;\\n    border: 0;\\n    padding: 0;\\n    vertical-align: middle;\\n}\\n\\n.toolbarContainer {\\n    display: inline-block;\\n}\\n\\n.summaryDiv {\\n    display: inline;\\n}\\n\\ndetails > summary {\\n    /* Note: couldn\'t get proper color with the svg approach */\\n    /* list-style-image: url(\\"data:image/svg+xml;utf8,<svg width=\'12px\' height=\'12px\' viewBox=\'0 0 20 20\' xmlns=\'http://www.w3.org/2000/svg\'><g data-name=\'Layer 2\'><g data-name=\'arrow-ios-forward\'><rect width=\'24\' height=\'24\' transform=\'rotate(-90 12 12)\' opacity=\'0\'/><path fill=\'currentColor\' stroke=\'currentColor\' d=\'M10 19a1 1 0 0 1-.64-.23 1 1 0 0 1-.13-1.41L13.71 12 9.39 6.63a1 1 0 0 1 .15-1.41 1 1 0 0 1 1.46.15l4.83 6a1 1 0 0 1 0 1.27l-5 6A1 1 0 0 1 10 19z\'/></g></g></svg>\\"); */\\n    /* list-style-type: \\"⮞ \\"; */\\n    /* list-style-type: \\"⏵\\"; */\\n    list-style-type: \\"+ \\";\\n}\\n\\ndetails[open] > summary {\\n    /* list-style-image: url(\\"data:image/svg+xml;utf8,<svg width=\'12px\' height=\'12px\' viewBox=\'0 0 20 20\' xmlns=\'http://www.w3.org/2000/svg\'><g data-name=\'Layer 2\'><g data-name=\'arrow-ios-downward\'><rect width=\'24\' height=\'24\' opacity=\'0\'/><path fill=\'currentColor\' stroke=\'currentColor\' d=\'M12 16a1 1 0 0 1-.64-.23l-6-5a1 1 0 1 1 1.28-1.54L12 13.71l5.36-4.32a1 1 0 0 1 1.41.15 1 1 0 0 1-.14 1.46l-6 4.83A1 1 0 0 1 12 16z\'/></g></g></svg>\\"); */\\n    /* list-style-type: \\"⮟ \\"; */\\n    /* list-style-type: \\"⏷\\"; */\\n    list-style-type: \\"- \\";\\n}\\n\\n.NO_CHILDREN > summary {\\n    list-style-type: \\"\xa0\xa0\\" !important;\\n}\\n\\nselect {\\n    background-color: var(--menu-background);\\n    color: var(--menu-foreground);\\n}\\n\\nsummary {\\n    padding: 3px;\\n}\\n\\na:link {\\n    color: var(--fg-color);\\n}\\n\\na:visited {\\n    color: var(--fg-color);\\n}\\n\\na:hover {\\n    color: var(--fg-color);\\n}\\n\\na:active {\\n    color: var(--fg-color);\\n}\\n\\n.label {\\n    padding: 2px 2px;\\n    font-size: 0.65em;\\n    letter-spacing: 1px;\\n    white-space: nowrap;\\n    border-radius: 3px;\\n    margin-right: 5px;\\n    font-weight: bold;\\n}\\n\\n.timeLabel {\\n    padding: 2px 2px;\\n    font-size: 0.85em;\\n    letter-spacing: 1px;\\n    white-space: nowrap;\\n    border-radius: 3px;\\n    margin-right: 5px;\\n    font-weight: lighter;\\n}\\n\\n.label.F,\\n.label.E,\\n.label.FAIL,\\n.label.ERROR {\\n    border-radius: 3px;\\n    background-color: var(--error-background-color);\\n    color: var(--error-color);\\n    font-weight: bolder;\\n}\\n\\n.label.PASS,\\n.label.I,\\n.label.INFO {\\n    border-radius: 3px;\\n    background-color: var(--pass-background-color);\\n    color: var(--pass-color);\\n    font-weight: bolder;\\n}\\n\\n.label.W,\\n.label.WARN {\\n    border-radius: 3px;\\n    background-color: var(--warn-background-color);\\n    color: var(--warn-color);\\n    font-weight: bolder;\\n}\\n\\n.label.HIDDEN {\\n    border-radius: 3px;\\n    background-color: var(--hidden-background-color);\\n    color: var(--hidden-color);\\n    font-weight: bolder;\\n}\\n.label.HIDDEN.inline {\\n    margin-left: 5px;\\n}\\n\\nsummary.HIDDEN {\\n    margin-top: 10px;\\n    margin-bottom: 10px;\\n}\\n\\n.label.NOT_RUN {\\n    border-radius: 3px;\\n    background-color: var(--not-run-background-color);\\n    color: var(--not-run-color);\\n    font-weight: bolder;\\n}\\n\\n#summary.FAIL,\\n#summary.ERROR {\\n    border-bottom: 5px solid var(--error-background-color);\\n}\\n\\n#summary.PASS {\\n    border-bottom: 5px solid var(--pass-background-color);\\n}\\n\\n#summary.NOT_RUN {\\n    border-bottom: 5px solid var(--not-run-background-color);\\n}\\n\\n/* .span_link::after {\\n    content: \\" ⮳\\";\\n} */\\n.span_link {\\n    cursor: pointer;\\n    /* text-decoration: underline; */\\n}\\n\\nsummary:hover {\\n    background-color: var(--summary-hover-background-color);\\n}\\n",""]);const a=s},645:e=>{e.exports=function(e){var t=[];return t.toString=function(){return this.map((function(t){var n=e(t);return t[2]?"@media ".concat(t[2]," {").concat(n,"}"):n})).join("")},t.i=function(e,n,o){"string"==typeof e&&(e=[[null,e,""]]);var s={};if(o)for(var a=0;a<this.length;a++){var r=this[a][0];null!=r&&(s[r]=!0)}for(var i=0;i<e.length;i++){var d=[].concat(e[i]);o&&s[d[0]]||(n&&(d[2]?d[2]="".concat(n," and ").concat(d[2]):d[2]=n),t.push(d))}},t}},391:(e,t,n)=>{let o;window.setVSCodeAPI=function(e){o=e};let s={};function a(e){let t;try{t=o}catch(e){}t&&t.postMessage(e)}let r={output:void 0},i={setContents:void 0,appendContents:void 0,updateLabel:void 0};window.addEventListener("message",(e=>{let t=e.data;if(t)switch(t.type){case"response":let e=t,n=s[e.request_seq];n&&(delete s[e.request_seq],n(e));break;case"event":let o=r[t.event];o?o(t):console.log("Unhandled event: ",t);break;case"request":let a=i[t.command];a?a(t):console.log("Unhandled request: ",t)}}));let d=0;function l(){return d+=1,d}let c={filterLevel:"PASS",runIdToTreeState:{},runIdLRU:[]},u={initialContents:void 0,runId:void 0,state:void 0,onClickReference:void 0,appendedContents:[],allRunIdsToLabel:{},showTime:!0,showExpand:!0};function m(){return void 0===u.state&&(u.state=function(){let e;try{e=o}catch(e){}if(e){let t=e.getState();return t||(t=c),void 0===t.filterLevel&&(t.filterLevel="PASS"),void 0===t.runIdToTreeState&&(t.runIdToTreeState={}),void 0===!t.runIdLRU&&(t.runIdLRU=[]),t}return c}()),u}function h(e){return document.getElementById(e)}function p(e){return h(e)}function f(e){return h(e)}function g(e){const t=document.createElement("ul");return t.setAttribute("data-tree-id",e),t}function v(){return document.createElement("span")}function E(){return document.createElement("button")}function y(){return document.createElement("div")}function b(e){return e.getAttribute("data-tree-id")}function S(e,t=void 0){if(void 0===t)return"1"===e.getAttribute("data-hidden");t?e.setAttribute("data-hidden","1"):e.removeAttribute("data-hidden")}function C(e){var t=document.createElement("template");return e=e.trim(),t.innerHTML=e,t.content.firstChild}function T(e,t){for(let n of t.childNodes)if(n instanceof HTMLDetailsElement){for(let t of n.childNodes)t instanceof HTMLUListElement&&N(e,t);n.open?e.openNodes[b(t)]="open":delete e.openNodes[b(t)]}}function N(e,t){for(let n of t.childNodes)n instanceof HTMLLIElement&&T(e,n)}const L=((e,t)=>{let n;return function(...e){clearTimeout(n),n=setTimeout((()=>{clearTimeout(n),(()=>{w()})(...e)}),500)}})();function w(){const e=m();!function(e,t){const n=p("mainTree");let o={openNodes:{}};if(void 0===e.runIdLRU&&(e.runIdLRU=[]),void 0===e.runIdToTreeState)e.runIdToTreeState={};else{const n=e.runIdToTreeState[t];n&&(o=n)}for(let e of n.childNodes)e instanceof HTMLUListElement&&N(o,e);e.runIdToTreeState[t]=o;const s=e.runIdLRU.indexOf(t);for(s>-1&&e.runIdLRU.splice(s,1),e.runIdLRU.push(t);e.runIdLRU.length>15;){const t=e.runIdLRU.splice(0,1);delete e.runIdToTreeState[t[0]]}}(e.state,e.runId),function(e){let t;try{t=o}catch(e){}t?t.setState(e):c=e}(e.state)}function I(e,t){if(void 0===e)return;const n=f("selectedRun"),o=new Map;for(let s of n.childNodes)if(s instanceof HTMLOptionElement){const n=s,a=n.value,r=e[a];if(void 0===r)s.remove();else{n.text!==r&&(n.text=r),o.set(a,r);const e=t==a;n.selected=e}}for(const s of Object.keys(e)){if(void 0===s)continue;const a=t==s;if(!o.has(s)){const t=document.createElement("option"),r=e[s];t.value=s,n.appendChild(t),t.selected=a,t.text=r,o.set(s,r)}}}Math.pow(10,8);var x=36e5;function M(e,t){var n;!function(e,t){if(t.length<1)throw new TypeError("1 argument required, but only "+t.length+" present")}(0,arguments);var o=function(e){if(null===e||!0===e||!1===e)return NaN;var t=Number(e);return isNaN(t)?t:t<0?Math.ceil(t):Math.floor(t)}(null!==(n=null==t?void 0:t.additionalDigits)&&void 0!==n?n:2);if(2!==o&&1!==o&&0!==o)throw new RangeError("additionalDigits must be 0, 1 or 2");if("string"!=typeof e&&"[object String]"!==Object.prototype.toString.call(e))return new Date(NaN);var s,a=function(e){var t,n={},o=e.split(R.dateTimeDelimiter);if(o.length>2)return n;if(/:/.test(o[0])?t=o[0]:(n.date=o[0],t=o[1],R.timeZoneDelimiter.test(n.date)&&(n.date=e.split(R.timeZoneDelimiter)[0],t=e.substr(n.date.length,e.length))),t){var s=R.timezone.exec(t);s?(n.time=t.replace(s[1],""),n.timezone=s[1]):n.time=t}return n}(e);if(a.date){var r=function(e,t){var n=new RegExp("^(?:(\\\\d{4}|[+-]\\\\d{"+(4+t)+"})|(\\\\d{2}|[+-]\\\\d{"+(2+t)+"})$)"),o=e.match(n);if(!o)return{year:NaN,restDateString:""};var s=o[1]?parseInt(o[1]):null,a=o[2]?parseInt(o[2]):null;return{year:null===a?s:100*a,restDateString:e.slice((o[1]||o[2]).length)}}(a.date,o);s=function(e,t){if(null===t)return new Date(NaN);var n=e.match(_);if(!n)return new Date(NaN);var o=!!n[4],s=D(n[1]),a=D(n[2])-1,r=D(n[3]),i=D(n[4]),d=D(n[5])-1;if(o)return function(e,t,n){return t>=1&&t<=53&&n>=0&&n<=6}(0,i,d)?function(e,t,n){var o=new Date(0);o.setUTCFullYear(e,0,4);var s=7*(t-1)+n+1-(o.getUTCDay()||7);return o.setUTCDate(o.getUTCDate()+s),o}(t,i,d):new Date(NaN);var l=new Date(0);return function(e,t,n){return t>=0&&t<=11&&n>=1&&n<=(O[t]||(H(e)?29:28))}(t,a,r)&&function(e,t){return t>=1&&t<=(H(e)?366:365)}(t,s)?(l.setUTCFullYear(t,a,Math.max(s,r)),l):new Date(NaN)}(r.restDateString,r.year)}if(!s||isNaN(s.getTime()))return new Date(NaN);var i,d=s.getTime(),l=0;if(a.time&&(l=function(e){var t=e.match(k);if(!t)return NaN;var n=F(t[1]),o=F(t[2]),s=F(t[3]);return function(e,t,n){return 24===e?0===t&&0===n:n>=0&&n<60&&t>=0&&t<60&&e>=0&&e<25}(n,o,s)?n*x+6e4*o+1e3*s:NaN}(a.time),isNaN(l)))return new Date(NaN);if(!a.timezone){var c=new Date(d+l),u=new Date(0);return u.setFullYear(c.getUTCFullYear(),c.getUTCMonth(),c.getUTCDate()),u.setHours(c.getUTCHours(),c.getUTCMinutes(),c.getUTCSeconds(),c.getUTCMilliseconds()),u}return i=function(e){if("Z"===e)return 0;var t=e.match(A);if(!t)return 0;var n="+"===t[1]?-1:1,o=parseInt(t[2]),s=t[3]&&parseInt(t[3])||0;return function(e,t){return t>=0&&t<=59}(0,s)?n*(o*x+6e4*s):NaN}(a.timezone),isNaN(i)?new Date(NaN):new Date(d+l+i)}var R={dateTimeDelimiter:/[T ]/,timeZoneDelimiter:/[Z ]/i,timezone:/([Z+-].*)$/},_=/^-?(?:(\\d{3})|(\\d{2})(?:-?(\\d{2}))?|W(\\d{2})(?:-?(\\d{1}))?|)$/,k=/^(\\d{2}(?:[.,]\\d*)?)(?::?(\\d{2}(?:[.,]\\d*)?))?(?::?(\\d{2}(?:[.,]\\d*)?))?$/,A=/^([+-])(\\d{2})(?::?(\\d{2}))?$/;function D(e){return e?parseInt(e):1}function F(e){return e&&parseFloat(e.replace(",","."))||0}var O=[31,null,31,30,31,30,31,31,30,31,30,31];function H(e){return e%400==0||e%4==0&&e%100!=0}function U(e,t){const n=e.memo[t];return void 0===n?`<ref not found: ${t}>`:n}function B(e,t){return parseFloat(t)}function P(e,t){return parseInt(t)}function $(e,t){return t}function j(e){const t=[],n=new Map;for(let o of e.split(",")){o=o.trim();let e="oid";if(-1!=o.indexOf(":")&&([o,e]=o.split(":",2)),t.push(o),"oid"===e)n.set(o,U);else if("int"===e)n.set(o,P);else if("float"===e)n.set(o,B);else{if("str"!==e)throw new Error("Unexpected: "+e);n.set(o,$)}}return function(e,o){const s=o.split("|",t.length),a={};for(let o=0;o<s.length;o++){const r=s[o],i=t[o];a[i]=n.get(i)(e,r)}return a}}const Y=j("part:int, id:str"),z={V:j("version:str"),ID:Y,I:function(e,t){return JSON.parse(t)},T:function(e,t){return{time:M(t).toString()}},M:function(e,t){var n,o;const s=W(t,":");if(s){[n,o]=s;try{o=JSON.parse(o)}catch(e){return console.log("Error parsing json: "+o),console.log(e),null}e.memo[n]=o}return null},SR:j("name:oid, time_delta_in_seconds:float"),ER:j("status:oid, time_delta_in_seconds:float"),ST:j("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),ET:j("status:oid, message:oid, time_delta_in_seconds:float"),SE:j("name:oid, libname:oid, type:oid, doc:oid, source:oid, lineno:int, time_delta_in_seconds:float"),EE:j("type:oid, status:oid, time_delta_in_seconds:float"),EA:j("name:oid, type:oid, value:oid"),AS:j("source:oid, lineno:int, target:oid, type:oid, value:oid, time_delta_in_seconds:float"),L:j("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),LH:j("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),TG:j("tag:oid"),S:j("start_time_delta:float"),STB:j("message:oid, time_delta_in_seconds:float"),RTB:j("message:oid, time_delta_in_seconds:float"),TBE:j("source:oid, lineno:int, method:oid, line_content:oid"),TBV:j("name:oid, type:oid, value:oid"),ETB:j("time_delta_in_seconds:float"),YS:j("name:oid, libname:oid, source:oid, lineno:int, type:oid, value:oid, time_delta_in_seconds:float"),YR:j("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),YFS:j("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),YFR:j("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float")};z.RR=z.SR,z.RT=z.ST,z.RE=z.SE,z.RYR=z.YR;class V{constructor(){this.memo={}}decode_message_type(e,t){return(0,z[e])(this,t)}}function W(e,t){const n=e.indexOf(t);if(n>0)return[e.substring(0,n),e.substring(n+1)]}function*q(e,t){var n,o,s;for(let a of e.split(/\\r?\\n/))if(a=a.trim(),a)try{const e=W(a," ");if(e&&([s,o]=e,n=t.decode_message_type(s,o))){const e={message_type:s,decoded:n};yield e}}catch(e){console.log("Unable to decode message: "+a),console.log(e)}}function J(e,t){const n=document.createElement("span");n.textContent=t,n.classList.add("label"),n.classList.add(t.replace(" ","_")),e.summaryDiv.insertBefore(n,e.summaryDiv.firstChild)}function G(e,t){switch(e.state.filterLevel){case"FAIL":return t>=2;case"WARN":return t>=1;case"PASS":return t>=0;case"NOT RUN":return!0}}function Z(e){switch(e){case"FAIL":case"ERROR":return 2;case"WARN":return 1;case"NOT RUN":case"NOT_RUN":return-1;default:return 0}}class K{constructor(e){this.stack=[],this.exceptionMsg=e}pushEntry(e,t,n,o){const s=new Map;this.stack.push({source:e,lineno:t,method:n,lineContent:o,variables:s})}pushVar(e,t,n){this.stack.at(-1).variables.set(e,[t,n])}}class Q{constructor(){this.totalTests=0,this.totalFailures=0}clear(){this.totalTests=0,this.totalFailures=0,this.updateSummary()}onTestEndUpdateSummary(e){const t=e.decoded.status;this.totalTests+=1,"FAIL"!=t&&"ERROR"!=t||(this.totalFailures+=1),this.updateSummary()}updateSummary(){const e=p("summary");if(!e)return;const t=(""+this.totalTests).padStart(4),n=(""+this.totalFailures).padStart(4);if(e.textContent=`Total: ${t} Failures: ${n}`,0==this.totalFailures&&0==this.totalTests){const e=p("summary");e.classList.add("NOT_RUN"),e.classList.remove("PASS"),e.classList.remove("FAIL")}else if(1==this.totalFailures){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("PASS"),e.classList.add("FAIL")}else if(0==this.totalFailures&&1==this.totalTests){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("FAIL")}}}function X(e,t){const n=function(e){const t=document.createElement("li");return t.setAttribute("data-tree-id",e),t}(t),o=document.createElement("details");e&&(o.open=e),o.classList.add("NO_CHILDREN"),n.appendChild(o);const s=y();s.classList.add("detailContainer"),o.appendChild(s);const a=document.createElement("summary"),r=y();r.classList.add("summaryDiv"),a.appendChild(r);const i=v();i.className="summaryName",i.textContent="[summaryName]",r.appendChild(i);const d=v();return d.className="summaryInput emptySummaryInput",d.textContent="",r.appendChild(d),o.appendChild(a),{li:n,details:o,summary:a,summaryDiv:r,summaryName:i,summaryInput:d,detailContainer:s}}function ee(e,t){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${t}`,e.summaryInput.classList.remove("emptySummaryInput")):e.summaryInput.textContent+=`, ${t}`}function te(e,t,n,o,s,a,r,i,d,l){const c=e.state.runIdToTreeState[e.runId],u="li_"+l;if(c){const e=c.openNodes;e&&(a=e[u])}const m=X(a,u),h=m.li,p=m.details,f=m.detailContainer,v=m.summary,E=m.summaryDiv,y=m.summaryName,b=m.summaryInput;if("LH"===s.message_type){y.textContent="";const e=C(n);y.appendChild(e)}else y.textContent=n;o&&(y.title=o),e.onClickReference&&(y.classList.add("span_link"),y.onclick=t=>{const n=[];let o=d.parent;for(;void 0!==o&&void 0!==o.message;)n.push(o.message),o=o.parent;t.preventDefault(),e.onClickReference({source:r,lineno:i,message:s.decoded,messageType:s.message_type,scope:n})});const S=g("ul_"+l);p.appendChild(S);const T={ul:S,li:h,details:p,detailContainer:f,summary:v,summaryName:y,summaryInput:b,source:r,lineno:i,appendContentChild:void 0,decodedMessage:s,maxLevelFoundInHierarchy:-1,summaryDiv:E};return T.appendContentChild=re.bind(T),t.appendContentChild(T),T}let ne,oe;function*se(e){for(let t of e.childNodes)if(t instanceof HTMLDetailsElement){for(let e of t.childNodes)if(e instanceof HTMLUListElement)for(let t of ae(e))yield t;yield t}}function*ae(e){for(let t of e.childNodes)if(t instanceof HTMLLIElement)for(let e of se(t))yield e}function re(e){const t=this;t.ul.appendChild(e.li),t.details.classList.contains("NO_CHILDREN")&&(t.details.classList.remove("NO_CHILDREN"),t.details.addEventListener("toggle",(function(){L()})),m().showExpand&&t.summary.addEventListener("mouseover",(e=>{!function(e){if(void 0===ne){ne=y(),ne.classList.add("toolbarContainer");const e=E();e.appendChild(C(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path d="M7 12V7H6v5h1z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),e.onclick=()=>{!function(){if(void 0!==oe){oe.details.open=!0;for(let e of ae(oe.ul))e.classList.contains("NO_CHILDREN")||(e.open=!0)}}()},e.classList.add("toolbarButton");const t=E();return t.appendChild(C(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),t.classList.add("toolbarButton"),t.onclick=()=>{!function(){if(void 0!==oe){oe.details.open=!1;for(let e of ae(oe.ul))e.open=!1}}()},ne.appendChild(t),void ne.appendChild(e)}oe=e,e.summaryDiv.appendChild(ne)}(t)})))}var ie=(e,t,n)=>new Promise(((o,s)=>{var a=e=>{try{i(n.next(e))}catch(e){s(e)}},r=e=>{try{i(n.throw(e))}catch(e){s(e)}},i=e=>e.done?o(e.value):Promise.resolve(e.value).then(a,r);i((n=n.apply(e,t)).next())}));let de=0,le=-1;class ce{constructor(){this.stack=[]}handle(e){let t;switch(e.message_type){case"STB":return void this.stack.push(new K(e.decoded.message));case"TBE":return t=this.stack.at(-1),void t.pushEntry(e.decoded.source,e.decoded.lineno,e.decoded.method,e.decoded.line_content);case"TBV":return;case"ETB":return t=this.stack.pop(),t.stack.reverse(),t}}}class ue{constructor(){this.stack=[],this.messageNode={parent:void 0,message:void 0},this.id=0,this.finishedAddingInitialContents=!1,this.appendedMessagesIndex=-1,this.decoder=new V,this.seenSuiteTaskOrElement=!1,this.tbHandler=new ce,this.suiteErrored=!1,this.opts=m(),this.runId=this.opts.runId,this.summaryBuilder=new Q,this.lease=(de+=1,le=de,de),this.resetState()}resetState(){this.seenSuiteTaskOrElement=!1}isCurrentTreeBuilder(){return this.lease===le&&this.runId==this.opts.runId}clearAndInitializeTree(){this.summaryBuilder.clear(),this.resetState();const e=f("filterLevel");e&&(e.value=this.opts.state.filterLevel);const t=p("mainTree");t.replaceChildren();const n=g("ul_root");n.classList.add("tree"),t.appendChild(n),this.parent={ul:void 0,li:void 0,details:void 0,detailContainer:void 0,summary:void 0,summaryName:void 0,summaryInput:void 0,source:void 0,lineno:void 0,decodedMessage:void 0,appendContentChild:function(e){n.appendChild(e.li)},maxLevelFoundInHierarchy:-1,summaryDiv:void 0},this.stack.push(this.parent)}addInitialContents(){return ie(this,null,(function*(){for(const e of q(this.opts.initialContents,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}this.finishedAddingInitialContents=!0,yield this.onAppendedContents()}))}onAppendedContents(){return ie(this,null,(function*(){if(!this.finishedAddingInitialContents)return;if(!this.isCurrentTreeBuilder())return;const e=m();for(;this.appendedMessagesIndex+1<e.appendedContents.length;){this.appendedMessagesIndex+=1;const t=e.appendedContents[this.appendedMessagesIndex];for(const e of q(t,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}}}))}addOneMessage(e){return ie(this,null,(function*(){if(this.isCurrentTreeBuilder())try{this.addOneMessageSync(e)}catch(t){console.log("Error: handling message: "+JSON.stringify(e)+": "+t+" - "+JSON.stringify(t))}}))}addOneMessageSync(e){var t,n;let o,s,a=e.message_type;switch(a){case"SR":case"ST":case"SE":case"STB":this.seenSuiteTaskOrElement=!0;break;case"RR":if(this.seenSuiteTaskOrElement)return;a="SR";break;case"RT":if(this.seenSuiteTaskOrElement)return;a="ST";break;case"RE":if(this.seenSuiteTaskOrElement)return;a="SE";break;case"RTB":if(this.seenSuiteTaskOrElement)return;a="STB"}switch(this.id+=1,a){case"SR":this.messageNode={parent:this.messageNode,message:e};for(const t of document.querySelectorAll(".suiteHeader"))t.textContent=e.decoded.name;break;case"AS":s=te(this.opts,this.parent,`${e.decoded.target} = `,`Assign to name: ${e.decoded.target}\\nAn object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),ee(s,e.decoded.value),this.addAssignCssClass(s);break;case"ST":this.messageNode={parent:this.messageNode,message:e},this.parent=te(this.opts,this.parent,`${e.decoded.libname}.${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"SE":case"YR":case"YFR":if("SE"!=a||"UNTRACKED_GENERATOR"!=e.decoded.type){this.messageNode={parent:this.messageNode,message:e};let t=e.decoded.name;"YR"==a&&(t+=" (resumed)"),this.parent=te(this.opts,this.parent,t,e.decoded.libname,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),"YR"==a&&this.addResumedCSSClass(this.parent),this.argsTarget=this.parent,this.stack.push(this.parent)}else{const t=te(this.opts,this.parent,`Create Generator: ${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addGeneratorCSSClass(t),this.argsTarget=t}break;case"ER":this.messageNode=this.messageNode.parent;{const t=p("suiteResult");t.style.display="block",this.suiteErrored?(t.classList.add("ERROR"),t.textContent="Run Failed"):(t.classList.add("PASS"),t.textContent="Run Passed");const n=p("suiteRunStart");n&&(n.textContent+=` - Finished in: ${e.decoded.time_delta_in_seconds.toFixed(2)}s.`)}break;case"ET":this.messageNode=this.messageNode.parent;const r=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(r,this.parent,e),this.onEndSetStatusOrRemove(this.opts,r,e.decoded,this.parent,!1),this.summaryBuilder.onTestEndUpdateSummary(e),o=this.addDetailsCSSClasses(e.decoded.status,r),o&&(this.suiteErrored=!0,r.details.open=!0);break;case"EE":case"YS":case"YFS":if("EE"!=a||"UNTRACKED_GENERATOR"!=e.decoded.type){if("YS"==a||"YFS"==a){const t=te(this.opts,this.parent,"Yielded",`Suspending function with yield.\\nYielding an object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addYieldedCSSClass(t),ee(t,e.decoded.value),e.decoded.status="PASS"}this.messageNode=this.messageNode.parent;let t=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(t,this.parent,e),this.onEndSetStatusOrRemove(this.opts,t,e.decoded,this.parent,!0),o=this.addDetailsCSSClasses(e.decoded.status,t),o&&(t.details.open=!0)}break;case"S":const i=e.decoded.start_time_delta;(null==(n=null==(t=this.parent)?void 0:t.decodedMessage)?void 0:n.decoded)&&(this.parent.decodedMessage.decoded.time_delta_in_seconds=i);break;case"EA":!function(e,t,n,o){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${t} = ${o}`,e.summaryInput.title=`Argument: ${t}\\nArgument type: ${n}\\nRepresentation:\\n${o}`,e.summaryInput.classList.remove("emptySummaryInput")):(e.summaryInput.title+=`\\n\\nArgument: ${t}\\nArgument type: ${n}\\nRepresentation:\\n${o}`,e.summaryInput.textContent+=`, ${t} = ${o}`)}(this.argsTarget,e.decoded.name,e.decoded.type,e.decoded.value);break;case"L":case"LH":const d=e.decoded.level,l=function(e){switch(e){case"E":case"F":return 2;case"W":return 1;default:return 0}}(d);if(l>this.parent.maxLevelFoundInHierarchy&&(this.parent.maxLevelFoundInHierarchy=l),G(this.opts,l)){const t=te(this.opts,this.parent,e.decoded.message,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());t.maxLevelFoundInHierarchy=l,function(e,t){const n=document.createElement("span");n.textContent=`LOG ${function(e){switch(e){case"E":return"ERROR";case"F":return"FAIL";case"W":return"WARN";case"I":return"INFO";default:return e}}(t)}`,n.classList.add("label"),n.classList.add(t.replace(" ","_")),e.summaryDiv.insertBefore(n,e.summaryDiv.firstChild)}(t,d),this.addDetailsCSSClasses(l,t)}break;case"STB":case"TBE":case"TBV":case"ETB":const c=this.tbHandler.handle(e);if(c&&c.stack.length>0){const t=c.stack[0];s=te(this.opts,this.parent,c.exceptionMsg,"",e,!1,t.source,t.lineno,this.messageNode,this.id.toString()),this.addExceptionCssClass(s)}break;case"T":const u=p("suiteRunStart");u&&(u.textContent=e.decoded.time)}}addAssignCssClass(e){e.details.classList.add("variableParent"),e.details.classList.add("leafNode")}addExceptionCssClass(e){e.details.classList.add("exceptionParent"),e.details.classList.add("leafNode")}addYieldedCSSClass(e){e.details.classList.add("yiededParent"),e.details.classList.add("leafNode")}addResumedCSSClass(e){e.details.classList.add("resumedParent")}addGeneratorCSSClass(e){e.details.classList.add("generatorParent"),e.details.classList.add("leafNode")}addDetailsCSSClasses(e,t){let n,o=!1;return n="string"==typeof e?Z(e):e,n>=2?(t.details.classList.add("errorParent"),o=!0):1==n?t.details.classList.add("warnParent"):t.details.classList.add("passParent"),t.details.classList.contains("parentNode")||t.details.classList.contains("leafNode")||(0===t.ul.children.length?t.details.classList.add("leafNode"):t.details.classList.add("parentNode")),o}onEndUpdateMaxLevelFoundInHierarchyFromStatus(e,t,n){const o=Z(n.decoded.status);o>e.maxLevelFoundInHierarchy&&(e.maxLevelFoundInHierarchy=o),e.maxLevelFoundInHierarchy>t.maxLevelFoundInHierarchy&&(t.maxLevelFoundInHierarchy=e.maxLevelFoundInHierarchy)}onEndSetStatusOrRemove(e,t,n,o,s){const a=n.status;if(G(e,t.maxLevelFoundInHierarchy)){if(s&&t.maxLevelFoundInHierarchy<=0){const e=50;if(o.ul.childElementCount>e){const e=t.summaryName.textContent;if(e&&e.toLowerCase().includes("iteration")){const e=t.li.previousSibling,n=b(t.li);if(t.li.remove(),S(e))e.getElementsByClassName("FINAL_SPAN")[0].textContent=t.summaryName.textContent;else{const e=X(!1,n);e.summaryName.textContent=t.summaryName.textContent,e.summary.classList.add("HIDDEN");const s=v();s.setAttribute("role","button"),s.textContent="...",s.classList.add("label"),s.classList.add("HIDDEN"),s.classList.add("inline"),e.summaryDiv.appendChild(s);const a=v();a.setAttribute("role","button"),a.classList.add("FINAL_SPAN"),e.summaryDiv.appendChild(a),J(e,"HIDDEN"),S(e.li,!0),o.ul.appendChild(e.li)}return}}}if(t.summary,J(t,a),null!=t.source&&t.source.length>0){const e=function(e){let t=e,n=Math.max(e.lastIndexOf("/"),e.lastIndexOf("\\\\"));return n>0&&(t=e.substring(n+1)),t}(t.source),n=document.createElement("span");n.textContent=e,n.classList.add("summaryFileName"),n.title=t.source,t.summaryDiv.appendChild(n)}if(this.opts.showTime){const e=t.decodedMessage.decoded.time_delta_in_seconds;void 0!==e&&e>=0&&function(e,t){const n=document.createElement("span");n.textContent=` (${t.toFixed(2)}s)`,n.classList.add("timeLabel"),e.summaryDiv.appendChild(n)}(t,n.time_delta_in_seconds-e)}}else t.li.remove()}}var me=(e,t,n)=>new Promise(((o,s)=>{var a=e=>{try{i(n.next(e))}catch(e){s(e)}},r=e=>{try{i(n.throw(e))}catch(e){s(e)}},i=e=>e.done?o(e.value):Promise.resolve(e.value).then(a,r);i((n=n.apply(e,t)).next())}));let he;function pe(){return me(this,null,(function*(){he=new ue,he.clearAndInitializeTree(),yield he.addInitialContents()}))}function fe(e){let t={type:"event",seq:l(),event:"onClickReference"};t.data=e,a(t)}function ge(e){w();const t=m();t.runId=e.runId,t.initialContents=e.initialContents,void 0!==o&&(t.onClickReference=fe),t.appendedContents=[],t.allRunIdsToLabel=e.allRunIdsToLabel,I(t.allRunIdsToLabel,t.runId),pe()}n(320),i.setContents=ge,i.appendContents=function(e){const t=m();t.runId===e.runId&&(t.appendedContents.push(e.appendContents),void 0!==he&&he.onAppendedContents())},i.updateLabel=function(e){const t=m();t.allRunIdsToLabel[e.runId]=e.label,I(t.allRunIdsToLabel,t.runId)},window.onChangedRun=function(){const e=f("selectedRun").value;let t={type:"event",seq:l(),event:"onSetCurrentRunId"};t.data={runId:e},a(t)},window.onChangedFilterLevel=function(){!function(e){const t=m();t.state.filterLevel!==e&&(t.state.filterLevel=e,w(),pe())}(f("filterLevel").value)},window.setContents=ge,window.setShowTime=function(e){m().showTime=e},window.setShowExpand=function(e){m().showExpand=e},window.getSampleContents=function(){return JSON.parse(\'"V 1\\\\nI \\\\"sys.platform=win32\\\\"\\\\nI \\\\"python=3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)]\\\\"\\\\nI \\\\"robot=5.1a3.dev1\\\\"\\\\nT 2022-10-19T09:48:34.018\\\\nM a:\\\\"Robot1\\\\"\\\\nM b:\\\\"s1\\\\"\\\\nM c:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\robot1.robot\\\\"\\\\nSR a|b|c|0.035\\\\nM d:\\\\"Simple Task\\\\"\\\\nM e:\\\\"s1-t1\\\\"\\\\nST d|e|16|0.036\\\\nM f:\\\\"First keyword\\\\"\\\\nM g:\\\\"\\\\"\\\\nM h:\\\\"KEYWORD\\\\"\\\\nSE f|g|h|g|c|17|0.036\\\\nM i:\\\\"No Operation\\\\"\\\\nM j:\\\\"BuiltIn\\\\"\\\\nM k:\\\\"Does absolutely nothing.\\\\"\\\\nSE i|j|h|k|c|8|0.037\\\\nM l:\\\\"PASS\\\\"\\\\nEE l|0.037\\\\nM m:\\\\"Log\\\\"\\\\nM n:\\\\"Logs the given message with the given level.\\\\"\\\\nSE m|j|h|n|c|10|0.037\\\\nM o:\\\\"Some warning message\\\\"\\\\nEA o\\\\nM p:\\\\"level=WARN\\\\"\\\\nEA p\\\\nEE l|0.046\\\\nM q:\\\\"Another keyword\\\\"\\\\nM r:\\\\"another\\\\"\\\\nSE q|r|h|g|c|11|0.047\\\\nM s:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\another.robot\\\\"\\\\nSE i|j|h|k|s|3|0.047\\\\nEE l|0.047\\\\nEE l|0.047\\\\nM t:\\\\"Another in sub keyword\\\\"\\\\nM u:\\\\"another_sub\\\\"\\\\nSE t|u|h|g|c|12|0.047\\\\nM v:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\sub\\\\\\\\\\\\\\\\another_sub.robot\\\\"\\\\nSE i|j|h|k|v|6|0.048\\\\nEE l|0.048\\\\nSE m|j|h|n|v|7|0.048\\\\nM w:\\\\"Some error message\\\\"\\\\nEA w\\\\nM x:\\\\"level=ERROR\\\\"\\\\nEA x\\\\nEE l|0.049\\\\nEE l|0.049\\\\nEE l|0.049\\\\nSE m|j|h|n|c|18|0.049\\\\nM y:\\\\"Some <data &encode <\\/script>\\\\"\\\\nEA y\\\\nEE l|0.049\\\\nM z:\\\\"Create Dictionary\\\\"\\\\nM A:\\\\"Creates and returns a dictionary based on the given ``items``.\\\\"\\\\nSE z|j|h|A|c|19|0.049\\\\nM B:\\\\"a=1\\\\"\\\\nEA B\\\\nM C:\\\\"b=1\\\\"\\\\nEA C\\\\nEE l|0.05\\\\nSE m|j|h|n|c|20|0.05\\\\nM D:\\\\"${dct}\\\\"\\\\nEA D\\\\nEE l|0.051\\\\nET l|g|0.051\\\\nM E:\\\\"Check 1\\\\"\\\\nM F:\\\\"s1-t2\\\\"\\\\nST E|F|22|0.051\\\\nSE f|g|h|g|c|23|0.051\\\\nSE i|j|h|k|c|8|0.052\\\\nEE l|0.052\\\\nSE m|j|h|n|c|10|0.052\\\\nEA o\\\\nEA p\\\\nEE l|0.052\\\\nSE q|r|h|g|c|11|0.053\\\\nSE i|j|h|k|s|3|0.053\\\\nEE l|0.053\\\\nEE l|0.053\\\\nSE t|u|h|g|c|12|0.053\\\\nSE i|j|h|k|v|6|0.054\\\\nEE l|0.054\\\\nSE m|j|h|n|v|7|0.054\\\\nEA w\\\\nEA x\\\\nEE l|0.054\\\\nEE l|0.055\\\\nEE l|0.055\\\\nM G:\\\\"${counter} IN RANGE [ 0 | 3 ]\\\\"\\\\nM H:\\\\"FOR\\\\"\\\\nSE G|g|H|g|c|25|0.055\\\\nM I:\\\\"${counter} = 0\\\\"\\\\nM J:\\\\"ITERATION\\\\"\\\\nSE I|g|J|g|c|25|0.055\\\\nM K:\\\\"${counter} == 2\\\\"\\\\nM L:\\\\"IF\\\\"\\\\nSE K|g|L|g|c|26|0.055\\\\nM M:\\\\"Fail\\\\"\\\\nM N:\\\\"Fails the test with the given message and optionally alters its tags.\\\\"\\\\nSE M|j|h|N|c|27|0.056\\\\nM O:\\\\"Failed execution for some reason...\\\\"\\\\nEA O\\\\nM P:\\\\"NOT RUN\\\\"\\\\nEE P|0.056\\\\nEE P|0.056\\\\nSE m|j|h|n|c|29|0.056\\\\nM Q:\\\\"${counter}\\\\"\\\\nEA Q\\\\nEE l|0.056\\\\nEE l|0.057\\\\nM R:\\\\"${counter} = 1\\\\"\\\\nSE R|g|J|g|c|25|0.057\\\\nSE K|g|L|g|c|26|0.057\\\\nSE M|j|h|N|c|27|0.057\\\\nEA O\\\\nEE P|0.057\\\\nEE P|0.057\\\\nSE m|j|h|n|c|29|0.058\\\\nEA Q\\\\nEE l|0.058\\\\nEE l|0.058\\\\nM S:\\\\"${counter} = 2\\\\"\\\\nSE S|g|J|g|c|25|0.058\\\\nSE K|g|L|g|c|26|0.058\\\\nSE M|j|h|N|c|27|0.059\\\\nEA O\\\\nM T:\\\\"FAIL\\\\"\\\\nEE T|0.059\\\\nEE T|0.059\\\\nSE m|j|h|n|c|29|0.059\\\\nEA Q\\\\nEE P|0.059\\\\nEE T|0.06\\\\nEE T|0.06\\\\nET T|O|0.06\\\\nM U:\\\\"Check 2\\\\"\\\\nM V:\\\\"s1-t3\\\\"\\\\nST U|V|32|0.06\\\\nM W:\\\\"Set Variable\\\\"\\\\nM X:\\\\"Returns the given values which can then be assigned to a variables.\\\\"\\\\nSE W|j|h|X|c|33|0.061\\\\nM Y:\\\\"3\\\\"\\\\nEA Y\\\\nEE l|0.061\\\\nM Z:\\\\"${counter} <= 2\\\\"\\\\nM 0:\\\\"WHILE\\\\"\\\\nSE Z|g|0|g|c|34|0.061\\\\nSE g|g|J|g|c|34|0.062\\\\nM 1:\\\\"Evaluate\\\\"\\\\nM 2:\\\\"Evaluates the given expression in Python and returns the result.\\\\"\\\\nSE 1|j|h|2|c|35|0.062\\\\nM 4:\\\\"$counter-1\\\\"\\\\nEA 4\\\\nEE P|0.062\\\\nSE m|j|h|n|c|36|0.062\\\\nM 5:\\\\"Current counter: ${counter}\\\\"\\\\nEA 5\\\\nEA p\\\\nEE P|0.062\\\\nEE P|0.062\\\\nEE P|0.063\\\\nET l|g|0.063\\\\nM 6:\\\\"Check 3\\\\"\\\\nM 7:\\\\"s1-t4\\\\"\\\\nST 6|7|39|0.064\\\\nM 8:\\\\"TRY\\\\"\\\\nSE g|g|8|g|c|40|0.064\\\\nSE i|j|h|k|c|41|0.064\\\\nEE l|0.064\\\\nEE l|0.064\\\\nM 9:\\\\"message\\\\"\\\\nM aa:\\\\"EXCEPT\\\\"\\\\nSE 9|g|aa|g|c|42|0.064\\\\nSE i|j|h|k|c|43|0.065\\\\nEE P|0.065\\\\nEE P|0.065\\\\nM ab:\\\\"FINALLY\\\\"\\\\nSE g|g|ab|g|c|44|0.065\\\\nSE i|j|h|k|c|45|0.065\\\\nEE l|0.065\\\\nEE l|0.065\\\\nET l|g|0.066\\\\nER T|0.067\\\\n"\')}},320:(e,t,n)=>{var o=n(379),s=n.n(o),a=n(426),r={injectType:"singletonStyleTag",insert:"head",singleton:!0};s()(a.Z,r),a.Z.locals},379:(e,t,n)=>{var o,s=function(){var e={};return function(t){if(void 0===e[t]){var n=document.querySelector(t);if(window.HTMLIFrameElement&&n instanceof window.HTMLIFrameElement)try{n=n.contentDocument.head}catch(e){n=null}e[t]=n}return e[t]}}(),a=[];function r(e){for(var t=-1,n=0;n<a.length;n++)if(a[n].identifier===e){t=n;break}return t}function i(e,t){for(var n={},o=[],s=0;s<e.length;s++){var i=e[s],d=t.base?i[0]+t.base:i[0],l=n[d]||0,c="".concat(d," ").concat(l);n[d]=l+1;var u=r(c),m={css:i[1],media:i[2],sourceMap:i[3]};-1!==u?(a[u].references++,a[u].updater(m)):a.push({identifier:c,updater:f(m,t),references:1}),o.push(c)}return o}function d(e){var t=document.createElement("style"),o=e.attributes||{};if(void 0===o.nonce){var a=n.nc;a&&(o.nonce=a)}if(Object.keys(o).forEach((function(e){t.setAttribute(e,o[e])})),"function"==typeof e.insert)e.insert(t);else{var r=s(e.insert||"head");if(!r)throw new Error("Couldn\'t find a style target. This probably means that the value for the \'insert\' parameter is invalid.");r.appendChild(t)}return t}var l,c=(l=[],function(e,t){return l[e]=t,l.filter(Boolean).join("\\n")});function u(e,t,n,o){var s=n?"":o.media?"@media ".concat(o.media," {").concat(o.css,"}"):o.css;if(e.styleSheet)e.styleSheet.cssText=c(t,s);else{var a=document.createTextNode(s),r=e.childNodes;r[t]&&e.removeChild(r[t]),r.length?e.insertBefore(a,r[t]):e.appendChild(a)}}function m(e,t,n){var o=n.css,s=n.media,a=n.sourceMap;if(s?e.setAttribute("media",s):e.removeAttribute("media"),a&&"undefined"!=typeof btoa&&(o+="\\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a))))," */")),e.styleSheet)e.styleSheet.cssText=o;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(o))}}var h=null,p=0;function f(e,t){var n,o,s;if(t.singleton){var a=p++;n=h||(h=d(t)),o=u.bind(null,n,a,!1),s=u.bind(null,n,a,!0)}else n=d(t),o=m.bind(null,n,t),s=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(n)};return o(e),function(t){if(t){if(t.css===e.css&&t.media===e.media&&t.sourceMap===e.sourceMap)return;o(e=t)}else s()}}e.exports=function(e,t){(t=t||{}).singleton||"boolean"==typeof t.singleton||(t.singleton=(void 0===o&&(o=Boolean(window&&document&&document.all&&!window.atob)),o));var n=i(e=e||[],t);return function(e){if(e=e||[],"[object Array]"===Object.prototype.toString.call(e)){for(var o=0;o<n.length;o++){var s=r(n[o]);a[s].references--}for(var d=i(e,t),l=0;l<n.length;l++){var c=r(n[l]);0===a[c].references&&(a[c].updater(),a.splice(c,1))}n=d}}}}},t={};function n(o){var s=t[o];if(void 0!==s)return s.exports;var a=t[o]={id:o,exports:{}};return e[o](a,a.exports,n),a.exports}n.n=e=>{var t=e&&e.__esModule?()=>e.default:()=>e;return n.d(t,{a:t}),t},n.d=(e,t)=>{for(var o in t)n.o(t,o)&&!n.o(e,o)&&Object.defineProperty(e,o,{enumerable:!0,get:t[o]})},n.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),n.nc=void 0,n(391),n(320)})();</script></body><script>window.setShowTime(true);\n    window.setShowExpand(true);\n    try {\n        const vscode = acquireVsCodeApi();\n        window.setVSCodeAPI(vscode);\n        document.getElementById("selectRunContainer").style.display = "block";\n    } catch (err) {\n        // That\'s ok (not running in VSCode).\n        window.setContents({\n            "initialContents": window.getSampleContents(),\n        });\n    }</script></html>'}
```

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_index_v2.py` & `robocorp_log-0.0.13/src/robocorp/log/_index_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Note: autogenerated file.
 # To regenerate this file use: python -m dev build-output-view.
 
 # The FILE_CONTENTS contains the contents of the files with
 # html/javascript code which can be used to visualize the contents of the
 # output generated by robocorp-log (i.e.: the .log files).
 
-FILE_CONTENTS = {'index.html': '<!doctype html><html><head><meta charset="utf-8"/><title class="suiteHeader">Robocorp Log</title><meta name="viewport" content="width=device-width,initial-scale=1"/></head><body><div class="headerTitleSection"><h3 class="suiteHeader">Robocorp Log</h3><span id="suiteResult" class="label" style="display: none;"></span></div><div id="suiteRunStart" class="headerRunDetails"></div><div class="headers"><span class="headerSource"></span> <span class="headerInputs">Details</span></div><div id="mainTree"></div><script>(()=>{"use strict";var e={599:(e,n,t)=>{t.d(n,{Z:()=>o});var s=t(645),a=t.n(s)()((function(e){return e[1]}));a.push([e.id,\'/* ******************************* */\\n/* CONTAINERS ETC */\\n\\n/* box model reset */\\n* {\\n    box-sizing: border-box;\\n}\\n\\nhtml,\\nbody {\\n    margin: 0;\\n    padding: 0;\\n    height: 100%;\\n}\\n\\n:root {\\n    --right-column-width-narrow: 50vw;\\n    --right-column-width-wide: 60vw;\\n    /* from here: https://qwtel.com/posts/software/the-monospaced-system-ui-css-font-stack/ */\\n    --sans-font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen", "Ubuntu",\\n        "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue", Arial, sans-serif;\\n    /* from here: https://qwtel.com/posts/software/the-monospaced-system-ui-css-font-stack/ */\\n    --fixed-font-family: ui-monospace, Menlo, Monaco, "Cascadia Mono", "Segoe UI Mono", "Roboto Mono", "Oxygen Mono",\\n        "Ubuntu Monospace", "Source Code Pro", "Fira Mono", "Droid Sans Mono", "Courier New", monospace;\\n}\\n\\n/* ******************************* */\\n/* THEMING SUPPORT */\\n\\n@media (prefers-color-scheme: light) {\\n    :root {\\n        --log-color-error: #e84f5c;\\n        --log-color-success: #219f7f;\\n        --log-color-variable: #5070b4;\\n\\n        --log-color-warn: #93801c;\\n        --log-color-disabled: #999999;\\n        --log-color-border: #dddddd;\\n\\n        --log-color-text: #000000;\\n        --log-color-text-weaker: #444444;\\n        --log-color-text-weakest: #666666;\\n\\n        --log-color-bg: #ffffff;\\n        --log-color-bg-raised: #f3f3f3;\\n    }\\n}\\n\\n@media (prefers-color-scheme: dark) {\\n    :root {\\n        --log-color-error: #e84f5c;\\n        --log-color-success: #219f7f;\\n        --log-color-warn: #fff565;\\n        --log-color-variable: #4094c5;\\n\\n        --log-color-disabled: #666666;\\n        --log-color-border: #444444;\\n\\n        --log-color-text: #eeeeee;\\n        --log-color-text-weaker: #bbbbbb;\\n        --log-color-text-weakest: #666666;\\n\\n        --log-color-bg: #222222;\\n        --log-color-bg-raised: #333333;\\n    }\\n}\\n\\nbody {\\n    display: flex;\\n    flex-direction: column;\\n    padding: 1rem;\\n    font-size: 0.8rem;\\n    font-family: var(--sans-font-family);\\n    color: var(--log-color-text);\\n    background-color: var(--log-color-bg);\\n}\\n\\nul {\\n    list-style-type: none;\\n    padding-inline-start: 0px;\\n    margin-block-start: 0px;\\n}\\n\\n#mainTree {\\n    white-space: nowrap;\\n    overflow: auto;\\n    flex-grow: 1;\\n}\\n\\n/* ******************************* */\\n/* TREE */\\n\\n.tree li {\\n    display: block;\\n    position: relative;\\n    padding-left: 0px;\\n}\\n\\n/* nesting level vertical line */\\n.tree ul:not(:first-child),\\n.detailContainer {\\n    border-left: 1px solid var(--log-color-border);\\n\\n    /* centering the line with the icon */\\n    margin-left: 0.65rem;\\n\\n    /* nesting indentation */\\n    padding-left: 0.8rem;\\n}\\n\\ndetails.errorParent .tree ul:not(:first-child),\\ndetails.errorParent .detailContainer {\\n    border-color: var(--log-color-error);\\n}\\n\\n/* ******************************* */\\n/* SUMMARY ROW FOR EACH CODE ROW */\\n\\ndetails.parentNode > summary,\\ndetails.errorParent.leafNode > summary {\\n    cursor: pointer;\\n}\\n\\ndetails > summary {\\n    padding-top: 0.25rem;\\n    padding-bottom: 0.25rem;\\n    padding-left: 0.25rem;\\n\\n    /* chrome needs this, safari doesn\\\'t */\\n    list-style: none;\\n}\\n\\ndetails > summary:hover {\\n    background-color: var(--log-color-bg-raised);\\n    border-radius: 2px;\\n}\\n\\ndetails > summary::-webkit-details-marker {\\n    display: none;\\n}\\n\\ndetails > summary::marker {\\n    display: none;\\n}\\n\\ndetails > summary::before {\\n    background-color: var(--log-color-success);\\n}\\n\\ndetails.errorParent > summary::before {\\n    background-color: var(--log-color-error);\\n}\\n\\ndetails.warnParent > summary::before {\\n    background-color: var(--log-color-warn);\\n}\\n\\n/* icon from: https://github.com/twbs/icons/blob/main/icons/caret-right-square-fill.svg */\\ndetails > summary::before {\\n    position: absolute;\\n    left: 0.25rem;\\n    top: 4px;\\n\\n    /* chrome seems to need the \\\'-webkit\\\' prefix here */\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="black" class="bi bi-caret-right-square-fill" viewBox="0 0 16 16"><path d="M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm5.5 10a.5.5 0 0 0 .832.374l4.5-4a.5.5 0 0 0 0-.748l-4.5-4A.5.5 0 0 0 5.5 4v8z"/></svg>\\\');\\n    width: 1rem;\\n    height: 1rem;\\n    display: inline-block;\\n    content: "";\\n}\\n\\n/* filled icon */\\n/*details.leafNode.passParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square-fill" viewBox="0 0 16 16"><path d="M2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2zm10.03 4.97a.75.75 0 0 1 .011 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.75.75 0 0 1 1.08-.022z"/></svg>\\\');\\n}*/\\n\\ndetails.leafNode.passParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M14 1a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1h12zM2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2z"/><path d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.235.235 0 0 1 .02-.022z"/></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (debug-pause) */\\ndetails.leafNode.yiededParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M4.5 3H6v10H4.5V3zm7 0v10H10V3h1.5z"></path></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (circuit-board) */\\ndetails.leafNode.generatorParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M14.5 1h-13l-.5.5v13l.5.5h13l.5-.5v-13l-.5-.5zM14 14H5v-2h2.3c.3.6 1 1 1.7 1 1.1 0 2-.9 2-2s-.9-2-2-2-2 .9-2 2H4v3H2V2h2v2.3c-.6.3-1 1-1 1.7 0 1.1.9 2 2 2s2-.9 2-2h2c0 1.1.9 2 2 2s2-.9 2-2-.9-2-2-2c-.7 0-1.4.4-1.7 1H6.7c-.3-.6-1-1-1.7-1V2h9v12zm-6-3c0-.6.4-1 1-1s1 .4 1 1-.4 1-1 1-1-.4-1-1zM5 5c.6 0 1 .4 1 1s-.4 1-1 1-1-.4-1-1 .4-1 1-1zm6 0c.6 0 1 .4 1 1s-.4 1-1 1-1-.4-1-1 .4-1 1-1z"></path></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (debug-restart-frame) */\\ndetails.resumedParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M1 10V9h5.207a5.48 5.48 0 0 0-.185 1H1zm6.257-3a5.54 5.54 0 0 1 1.08-1H1v1h6.257zM6.6 13a5.465 5.465 0 0 1-.393-1H1v1h5.6zM15 3v1H1V3h14zm-3.36 10.031a2.531 2.531 0 1 0-2.192-3.797h1.068v.844h-1.97l-.421-.422v-2.25h.844v1.032a3.375 3.375 0 1 1-.423 3.412l.782-.318a2.532 2.532 0 0 0 2.313 1.5z"></path></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (symbol-variable) */\\ndetails.leafNode.variableParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M2 5h2V4H1.5l-.5.5v8l.5.5H4v-1H2V5zm12.5-1H12v1h2v7h-2v1h2.5l.5-.5v-8l-.5-.5zm-2.74 2.57L12 7v2.51l-.3.45-4.5 2h-.46l-2.5-1.5-.24-.43v-2.5l.3-.46 4.5-2h.46l2.5 1.5zM5 9.71l1.5.9V9.28L5 8.38v1.33zm.58-2.15l1.45.87 3.39-1.5-1.45-.87-3.39 1.5zm1.95 3.17l3.5-1.56v-1.4l-3.5 1.55v1.41z"></path></svg>\\\');\\n    background-color: var(--log-color-variable);\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (bracket-error) */\\ndetails.leafNode.exceptionParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M6 2.97184V2.98361H5.91083C5.71113 2.98361 5.5238 3.02427 5.34802 3.10513C5.17461 3.18275 5.02193 3.28942 4.89086 3.42437C4.76421 3.55475 4.66135 3.71034 4.58238 3.89205C4.50833 4.07152 4.47134 4.26019 4.47134 4.45902C4.47134 4.68725 4.4753 4.9134 4.48321 5.13749C4.49125 5.36105 4.49127 5.58262 4.48324 5.80219C4.47914 6.01973 4.46082 6.2333 4.42826 6.44285C4.39513 6.65175 4.33913 6.85263 4.26039 7.04464C4.18091 7.23843 4.07258 7.42254 3.93616 7.59702C3.82345 7.74119 3.68538 7.87538 3.52283 8C3.68538 8.12462 3.82345 8.25881 3.93616 8.40298C4.07258 8.57746 4.18091 8.76157 4.26039 8.95536C4.33921 9.14757 4.39513 9.35024 4.42823 9.56312C4.46084 9.76883 4.47914 9.98246 4.48324 10.2039C4.49127 10.4195 4.49125 10.6411 4.48321 10.8686C4.4753 11.0885 4.47134 11.3127 4.47134 11.541C4.47134 11.744 4.50838 11.9346 4.58223 12.1137C4.66104 12.2911 4.76386 12.4469 4.89086 12.5818C5.02194 12.7126 5.17396 12.8191 5.34763 12.9008C5.52346 12.9777 5.71095 13.0164 5.91083 13.0164H6V13.2V14H5.91083C5.59743 14 5.29407 13.9384 5.00128 13.8153C4.70818 13.692 4.44942 13.5153 4.22578 13.285C4.00311 13.0558 3.83793 12.805 3.73283 12.5323L3.73232 12.531C3.63387 12.265 3.56819 11.9903 3.53535 11.7072L3.53516 11.7055C3.50677 11.4215 3.4987 11.1316 3.51084 10.8357C3.52272 10.5462 3.52866 10.2567 3.52866 9.96721C3.52866 9.76883 3.48986 9.58047 3.41201 9.40108L3.41129 9.39942C3.33659 9.21871 3.23428 9.0637 3.10412 8.93352L3.10221 8.93161C2.97577 8.79762 2.82457 8.69157 2.64742 8.61396L2.64601 8.61334C2.47001 8.53238 2.28465 8.4918 2.08917 8.4918H2V8.4V7.6V7.5082H2.08917C2.28497 7.5082 2.4706 7.46954 2.64672 7.3925C2.82466 7.31055 2.97644 7.20405 3.10317 7.07359C3.23423 6.93866 3.33687 6.78296 3.4116 6.60601L3.412 6.60507C3.48974 6.42594 3.52866 6.23556 3.52866 6.03279C3.52866 5.74329 3.52272 5.45379 3.51084 5.16428C3.4987 4.86844 3.50678 4.5805 3.53519 4.30053L3.53533 4.29917C3.56814 4.01201 3.63382 3.7352 3.73233 3.46898L3.73282 3.46766C3.83792 3.19498 4.00311 2.94422 4.22578 2.71498C4.44942 2.48474 4.70818 2.30798 5.00128 2.18473C5.29407 2.06161 5.59743 2 5.91083 2H6V2.97184ZM13.9232 8.4918H14V8.4V7.6V7.5082H13.9108C13.7153 7.5082 13.53 7.46762 13.354 7.38666L13.3526 7.38604C13.1754 7.30844 13.0242 7.20238 12.8978 7.06839L12.8959 7.06648C12.7657 6.9363 12.6634 6.78129 12.5887 6.60058L12.588 6.59892C12.5101 6.41953 12.4713 6.23117 12.4713 6.03279C12.4713 5.74329 12.4773 5.45379 12.4892 5.16428C12.5013 4.86842 12.4932 4.57848 12.4648 4.29454L12.4646 4.29285C12.4318 4.00971 12.3661 3.73502 12.2677 3.46897L12.2672 3.46766C12.1621 3.19499 11.9969 2.94422 11.7742 2.71498C11.5506 2.48474 11.2918 2.30798 10.9987 2.18473C10.7059 2.06161 10.4026 2 10.0892 2H10V2.8V2.98361H10.0892C10.2891 2.98361 10.4765 3.0223 10.6524 3.09917C10.826 3.18092 10.9781 3.28736 11.1091 3.41823C11.2361 3.55305 11.339 3.70889 11.4178 3.88628C11.4916 4.0654 11.5287 4.25596 11.5287 4.45902C11.5287 4.68727 11.5247 4.91145 11.5168 5.13142C11.5088 5.35894 11.5087 5.58049 11.5168 5.79605C11.5209 6.01754 11.5392 6.23117 11.5718 6.43688C11.6049 6.64976 11.6608 6.85243 11.7396 7.04464C11.8191 7.23843 11.9274 7.42254 12.0638 7.59702C12.1765 7.74119 12.3146 7.87538 12.4772 8L12.4456 8.02455C12.9764 8.08338 13.4758 8.24605 13.9232 8.4918Z"></path><path fill-rule="evenodd" clip-rule="evenodd" d="M10.3333 9.50559C10.8266 9.17595 11.4067 9 12 9C12.7954 9.00098 13.5578 9.31736 14.1202 9.87976C14.6826 10.4422 14.999 11.2047 15 12C15 12.5933 14.8241 13.1734 14.4944 13.6667C14.1648 14.1601 13.6962 14.5446 13.1481 14.7716C12.5999 14.9987 11.9967 15.0581 11.4147 14.9424C10.8328 14.8266 10.2982 14.5409 9.87868 14.1213C9.45912 13.7018 9.1734 13.1672 9.05765 12.5853C8.94189 12.0033 9.0013 11.4001 9.22836 10.8519C9.45543 10.3038 9.83994 9.83524 10.3333 9.50559ZM13.1464 10.1464L12 11.2929L10.8536 10.1464L10.1465 10.8535L11.2929 12L10.1464 13.1464L10.8536 13.8536L12 12.7071L13.1465 13.8535L13.8536 13.1464L12.7071 12L13.8536 10.8536L13.1464 10.1464Z"></path></svg>\\\');\\n    background-color: var(--log-color-error);\\n}\\n.exceptionParent {\\n    font-weight: bold;\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (error) */\\ndetails.leafNode.errorParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M8.6 1c1.6.1 3.1.9 4.2 2 1.3 1.4 2 3.1 2 5.1 0 1.6-.6 3.1-1.6 4.4-1 1.2-2.4 2.1-4 2.4-1.6.3-3.2.1-4.6-.7-1.4-.8-2.5-2-3.1-3.5C.9 9.2.8 7.5 1.3 6c.5-1.6 1.4-2.9 2.8-3.8C5.4 1.3 7 .9 8.6 1zm.5 12.9c1.3-.3 2.5-1 3.4-2.1.8-1.1 1.3-2.4 1.2-3.8 0-1.6-.6-3.2-1.7-4.3-1-1-2.2-1.6-3.6-1.7-1.3-.1-2.7.2-3.8 1-1.1.8-1.9 1.9-2.3 3.3-.4 1.3-.4 2.7.2 4 .6 1.3 1.5 2.3 2.7 3 1.2.7 2.6.9 3.9.6zM7.9 7.5L10.3 5l.7.7-2.4 2.5 2.4 2.5-.7.7-2.4-2.5-2.4 2.5-.7-.7 2.4-2.5-2.4-2.5.7-.7 2.4 2.5z"/></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (warn) */\\ndetails.leafNode.warnParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M7.56 1h.88l6.54 12.26-.44.74H1.44L1 13.26 7.56 1zM8 2.28L2.28 13H13.7L8 2.28zM8.625 12v-1h-1.25v1h1.25zm-1.25-2V6h1.25v4h-1.25z"/></svg>\\\');\\n}\\n\\ndetails.parentNode > summary::before,\\ndetails.parentNode.errorParent > summary::before {\\n    transform-origin: 8px 8px;\\n    transform: rotate(0deg);\\n    transition: transform 0.2s ease-out !important;\\n}\\n\\ndetails[open].parentNode > summary::before,\\ndetails[open].parentNode.errorParent > summary::before {\\n    transform: rotate(90deg);\\n}\\n\\ndetails[open] > summary > .summaryDiv > .summaryInput {\\n    /* Display full input parameters when expanded by adjusting the\\n       white-space to wrap the contents. Even nodes that don\\\'t have\\n       children can be expanded in this way, but it is not obvious\\n       since there is no triangle icon next to them. */\\n    white-space: initial;\\n}\\n\\n.summaryDiv {\\n    /* aligns code line correctly with the icon */\\n    display: flex;\\n    margin-left: 1.2rem;\\n}\\n\\n.summaryDiv > .label {\\n    order: 2;\\n}\\n\\n.summaryDiv > .summaryName {\\n    order: 1;\\n\\n    margin-left: 0.5rem;\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n}\\n\\n.summaryDiv > .summaryName,\\n.detailContainer > .detailInfo {\\n    /* this forces the correct column size, see:\\n       https://makandracards.com/makandra/66994-css-flex-and-min-width */\\n    min-width: 0;\\n}\\n\\ndetails.errorParent > summary > .summaryDiv > .summaryName {\\n    font-weight: bold;\\n}\\n\\n.summaryDiv > .summaryInput {\\n    order: 4;\\n    margin-left: auto;\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n.summaryDiv > .summaryInput.emptySummaryInput {\\n    color: var(--log-color-text-weakest);\\n}\\n\\n.detailContainer {\\n    display: flex;\\n}\\n\\n.detailContainer > .detailInfo {\\n    margin-right: auto;\\n}\\n\\n.summaryDiv > .summaryInput,\\n.detailContainer > .detailInputs {\\n    flex: 0 0 var(--right-column-width-wide);\\n    padding-left: 0.5rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n}\\n\\n.summaryDiv .timeLabel,\\n.summaryDiv .summaryFileName {\\n    order: 3;\\n    color: var(--log-color-text-weakest);\\n    margin-left: 0.5rem;\\n}\\n\\ndetails > summary:hover .timeLabel,\\ndetails > summary:hover .summaryFileName {\\n    color: var(--log-color-text-weaker);\\n}\\n\\ndetails > summary:hover .summaryInput:not(.emptySummaryInput) {\\n    color: var(--log-color-text) !important;\\n}\\n\\n/* ******************************* */\\n/* RESPONSIVE SIZING */\\n\\n@media only screen and (max-width: 840px) {\\n    .summaryDiv > .summaryInput,\\n    .detailContainer > .detailInputs,\\n    .headerInputs {\\n        display: none;\\n    }\\n}\\n\\n@media only screen and (max-width: 960px) {\\n    .headerInputs {\\n        width: var(--right-column-width-narrow) !important;\\n    }\\n\\n    .summaryDiv > .summaryInput,\\n    .detailContainer > .detailInputs {\\n        flex: 0 0 var(--right-column-width-narrow) !important;\\n    }\\n}\\n\\n/* ******************************* */\\n/* ERROR OUTPUT */\\n\\n.detailInfo {\\n    margin: 0.25rem 0;\\n    padding: 0.25rem 0;\\n    border-radius: 3px;\\n    font-size: 0.8rem;\\n}\\n\\n.errorHeader {\\n    font-weight: bold;\\n    margin-bottom: 0.35rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n\\n    /* forces wrapping */\\n    white-space: initial;\\n}\\n\\n.errorDetails {\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n\\n    /* forces wrapping */\\n    white-space: initial;\\n\\n    color: var(--log-color-text-weaker);\\n}\\n\\n/* ******************************* */\\n/* HEADERS */\\n\\n.headers {\\n    display: flex;\\n    border-bottom: 1px solid var(--log-color-border);\\n    padding-bottom: 1rem;\\n    margin-bottom: 1rem;\\n}\\n\\n.headerSource,\\n.headerInputs {\\n    font-weight: 600;\\n    text-transform: uppercase;\\n    font-size: 0.75rem;\\n    letter-spacing: 0.3px;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n.headerInputs {\\n    margin-left: auto;\\n    width: var(--right-column-width-wide);\\n    padding-left: 0.5rem;\\n}\\n\\n.headerRunDetails {\\n    margin: 0;\\n    margin-bottom: 1.5rem;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n/* ******************************* */\\n/* LABEL IS THE PASS/ERROR BADGE */\\n\\n.label {\\n    display: inline-block;\\n    margin-left: 0.5rem;\\n    color: white;\\n    font-weight: 600;\\n    font-size: 10px;\\n    border-radius: 2px;\\n    padding: 0 4px;\\n    height: 1rem;\\n    line-height: 1rem;\\n    letter-spacing: 0;\\n    display: none;\\n}\\n\\n.errorParent.leafNode .label.F,\\n.errorParent.leafNode .label.E,\\n.errorParent.leafNode .label.FAIL,\\n.errorParent.leafNode .label.ERROR {\\n    display: block;\\n    background-color: var(--log-color-error);\\n}\\n\\n/* hide labels when everything was successful */\\n/*\\n.label.PASS,\\n.label.I,\\n.label.INFO {\\n}\\n*/\\n.errorParent.leafNode .label.W,\\n.errorParent.leafNode .label.WARN {\\n    background-color: var(--log-color-warn);\\n}\\n\\n.label.NOT_RUN {\\n    background-color: var(--log-color-disabled);\\n}\\n\\n/* ******************************* */\\n/* HEADER TITLE ROW */\\n\\n.headerTitleSection {\\n    display: flex;\\n    align-items: center;\\n    margin-top: 0.3rem;\\n    margin-bottom: 0.5rem;\\n}\\n\\n.headerTitleSection h3 {\\n    margin: 0;\\n    padding: 0;\\n    font-size: 1.5rem;\\n}\\n\\n#suiteResult {\\n    font-size: 0.82rem;\\n    padding: 0.1rem 0.3rem 0.15rem 0.3rem;\\n    height: auto;\\n    margin-left: 0.75rem;\\n    display: inline-block;\\n}\\n.headerTitleSection .ERROR {\\n    background-color: var(--log-color-error);\\n}\\n.headerTitleSection .PASS {\\n    background-color: var(--log-color-success);\\n}\\n\',""]);const o=a},645:e=>{e.exports=function(e){var n=[];return n.toString=function(){return this.map((function(n){var t=e(n);return n[2]?"@media ".concat(n[2]," {").concat(t,"}"):t})).join("")},n.i=function(e,t,s){"string"==typeof e&&(e=[[null,e,""]]);var a={};if(s)for(var o=0;o<this.length;o++){var r=this[o][0];null!=r&&(a[r]=!0)}for(var i=0;i<e.length;i++){var l=[].concat(e[i]);s&&a[l[0]]||(t&&(l[2]?l[2]="".concat(t," and ").concat(l[2]):l[2]=t),n.push(l))}},n}},457:(e,n,t)=>{let s;window.setVSCodeAPI=function(e){s=e};let a={};function o(e){let n;try{n=s}catch(e){}n&&n.postMessage(e)}let r={output:void 0},i={setContents:void 0,appendContents:void 0,updateLabel:void 0};window.addEventListener("message",(e=>{let n=e.data;if(n)switch(n.type){case"response":let e=n,t=a[e.request_seq];t&&(delete a[e.request_seq],t(e));break;case"event":let s=r[n.event];s?s(n):console.log("Unhandled event: ",n);break;case"request":let o=i[n.command];o?o(n):console.log("Unhandled request: ",n)}}));let l=0;function d(){return l+=1,l}let c={filterLevel:"PASS",runIdToTreeState:{},runIdLRU:[]},u={initialContents:void 0,runId:void 0,state:void 0,onClickReference:void 0,appendedContents:[],allRunIdsToLabel:{},showTime:!0,showExpand:!0};function m(){return void 0===u.state&&(u.state=function(){let e;try{e=s}catch(e){}if(e){let n=e.getState();return n||(n=c),void 0===n.filterLevel&&(n.filterLevel="PASS"),void 0===n.runIdToTreeState&&(n.runIdToTreeState={}),void 0===!n.runIdLRU&&(n.runIdLRU=[]),n}return c}()),u}function h(e){return document.getElementById(e)}function p(e){return h(e)}function f(e){return h(e)}function g(e){const n=document.createElement("ul");return n.setAttribute("data-tree-id",e),n}function v(){return document.createElement("span")}function E(){return document.createElement("button")}function y(){return document.createElement("div")}function C(e){return e.getAttribute("data-tree-id")}function b(e,n=undefined){if(void 0===n)return"1"===e.getAttribute("data-hidden");n?e.setAttribute("data-hidden","1"):e.removeAttribute("data-hidden")}function w(e){var n=document.createElement("template");return e=e.trim(),n.innerHTML=e,n.content.firstChild}function S(e,n){for(let t of n.childNodes)if(t instanceof HTMLDetailsElement){for(let n of t.childNodes)n instanceof HTMLUListElement&&L(e,n);t.open?e.openNodes[C(n)]="open":delete e.openNodes[C(n)]}}function L(e,n){for(let t of n.childNodes)t instanceof HTMLLIElement&&S(e,t)}const x=((e,n)=>{let t;return function(...e){clearTimeout(t),t=setTimeout((()=>{clearTimeout(t),(()=>{N()})(...e)}),500)}})();function N(){const e=m();!function(e,n){const t=p("mainTree");let s={openNodes:{}};if(void 0===e.runIdLRU&&(e.runIdLRU=[]),void 0===e.runIdToTreeState)e.runIdToTreeState={};else{const t=e.runIdToTreeState[n];t&&(s=t)}for(let e of t.childNodes)e instanceof HTMLUListElement&&L(s,e);e.runIdToTreeState[n]=s;const a=e.runIdLRU.indexOf(n);for(a>-1&&e.runIdLRU.splice(a,1),e.runIdLRU.push(n);e.runIdLRU.length>15;){const n=e.runIdLRU.splice(0,1);delete e.runIdToTreeState[n[0]]}}(e.state,e.runId),function(e){let n;try{n=s}catch(e){}n?n.setState(e):c=e}(e.state)}function T(e,n){if(void 0===e)return;const t=f("selectedRun"),s=new Map;for(let a of t.childNodes)if(a instanceof HTMLOptionElement){const t=a,o=t.value,r=e[o];if(void 0===r)a.remove();else{t.text!==r&&(t.text=r),s.set(o,r);const e=n==o;t.selected=e}}for(const a of Object.keys(e)){if(void 0===a)continue;const o=n==a;if(!s.has(a)){const n=document.createElement("option"),r=e[a];n.value=a,t.appendChild(n),n.selected=o,n.text=r,s.set(a,r)}}}Math.pow(10,8);var I=36e5;function M(e,n){var t;!function(e,n){if(n.length<1)throw new TypeError("1 argument required, but only "+n.length+" present")}(0,arguments);var s=function(e){if(null===e||!0===e||!1===e)return NaN;var n=Number(e);return isNaN(n)?n:n<0?Math.ceil(n):Math.floor(n)}(null!==(t=null==n?void 0:n.additionalDigits)&&void 0!==t?t:2);if(2!==s&&1!==s&&0!==s)throw new RangeError("additionalDigits must be 0, 1 or 2");if("string"!=typeof e&&"[object String]"!==Object.prototype.toString.call(e))return new Date(NaN);var a,o=function(e){var n,t={},s=e.split(k.dateTimeDelimiter);if(s.length>2)return t;if(/:/.test(s[0])?n=s[0]:(t.date=s[0],n=s[1],k.timeZoneDelimiter.test(t.date)&&(t.date=e.split(k.timeZoneDelimiter)[0],n=e.substr(t.date.length,e.length))),n){var a=k.timezone.exec(n);a?(t.time=n.replace(a[1],""),t.timezone=a[1]):t.time=n}return t}(e);if(o.date){var r=function(e,n){var t=new RegExp("^(?:(\\\\d{4}|[+-]\\\\d{"+(4+n)+"})|(\\\\d{2}|[+-]\\\\d{"+(2+n)+"})$)"),s=e.match(t);if(!s)return{year:NaN,restDateString:""};var a=s[1]?parseInt(s[1]):null,o=s[2]?parseInt(s[2]):null;return{year:null===o?a:100*o,restDateString:e.slice((s[1]||s[2]).length)}}(o.date,s);a=function(e,n){if(null===n)return new Date(NaN);var t=e.match(R);if(!t)return new Date(NaN);var s=!!t[4],a=D(t[1]),o=D(t[2])-1,r=D(t[3]),i=D(t[4]),l=D(t[5])-1;if(s)return function(e,n,t){return n>=1&&n<=53&&t>=0&&t<=6}(0,i,l)?function(e,n,t){var s=new Date(0);s.setUTCFullYear(e,0,4);var a=7*(n-1)+t+1-(s.getUTCDay()||7);return s.setUTCDate(s.getUTCDate()+a),s}(n,i,l):new Date(NaN);var d=new Date(0);return function(e,n,t){return n>=0&&n<=11&&t>=1&&t<=(F[n]||(O(e)?29:28))}(n,o,r)&&function(e,n){return n>=1&&n<=(O(e)?366:365)}(n,a)?(d.setUTCFullYear(n,o,Math.max(a,r)),d):new Date(NaN)}(r.restDateString,r.year)}if(!a||isNaN(a.getTime()))return new Date(NaN);var i,l=a.getTime(),d=0;if(o.time&&(d=function(e){var n=e.match(_);if(!n)return NaN;var t=H(n[1]),s=H(n[2]),a=H(n[3]);return function(e,n,t){return 24===e?0===n&&0===t:t>=0&&t<60&&n>=0&&n<60&&e>=0&&e<25}(t,s,a)?t*I+6e4*s+1e3*a:NaN}(o.time),isNaN(d)))return new Date(NaN);if(!o.timezone){var c=new Date(l+d),u=new Date(0);return u.setFullYear(c.getUTCFullYear(),c.getUTCMonth(),c.getUTCDate()),u.setHours(c.getUTCHours(),c.getUTCMinutes(),c.getUTCSeconds(),c.getUTCMilliseconds()),u}return i=function(e){if("Z"===e)return 0;var n=e.match(A);if(!n)return 0;var t="+"===n[1]?-1:1,s=parseInt(n[2]),a=n[3]&&parseInt(n[3])||0;return function(e,n){return n>=0&&n<=59}(0,a)?t*(s*I+6e4*a):NaN}(o.timezone),isNaN(i)?new Date(NaN):new Date(l+d+i)}var k={dateTimeDelimiter:/[T ]/,timeZoneDelimiter:/[Z ]/i,timezone:/([Z+-].*)$/},R=/^-?(?:(\\d{3})|(\\d{2})(?:-?(\\d{2}))?|W(\\d{2})(?:-?(\\d{1}))?|)$/,_=/^(\\d{2}(?:[.,]\\d*)?)(?::?(\\d{2}(?:[.,]\\d*)?))?(?::?(\\d{2}(?:[.,]\\d*)?))?$/,A=/^([+-])(\\d{2})(?::?(\\d{2}))?$/;function D(e){return e?parseInt(e):1}function H(e){return e&&parseFloat(e.replace(",","."))||0}var F=[31,null,31,30,31,30,31,31,30,31,30,31];function O(e){return e%400==0||e%4==0&&e%100!=0}function P(e,n){const t=e.memo[n];return void 0===t?`<ref not found: ${n}>`:t}function U(e,n){return parseFloat(n)}function z(e,n){return parseInt(n)}function B(e,n){return n}function V(e){const n=[],t=new Map;for(let s of e.split(",")){s=s.trim();let e="oid";if(-1!=s.indexOf(":")&&([s,e]=s.split(":",2)),n.push(s),"oid"===e)t.set(s,P);else if("int"===e)t.set(s,z);else if("float"===e)t.set(s,U);else{if("str"!==e)throw new Error("Unexpected: "+e);t.set(s,B)}}return function(e,s){const a=s.split("|",n.length),o={};for(let s=0;s<a.length;s++){const r=a[s],i=n[s];o[i]=t.get(i)(e,r)}return o}}const j=V("part:int, id:str"),$={V:V("version:str"),ID:j,I:function(e,n){return JSON.parse(n)},T:function(e,n){return{time:M(n).toString()}},M:function(e,n){var t,s;const a=Y(n,":");if(a){[t,s]=a;try{s=JSON.parse(s)}catch(e){return console.log("Error parsing json: "+s),console.log(e),null}e.memo[t]=s}return null},SR:V("name:oid, time_delta_in_seconds:float"),ER:V("status:oid, time_delta_in_seconds:float"),ST:V("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),ET:V("status:oid, message:oid, time_delta_in_seconds:float"),SE:V("name:oid, libname:oid, type:oid, doc:oid, source:oid, lineno:int, time_delta_in_seconds:float"),EE:V("type:oid, status:oid, time_delta_in_seconds:float"),EA:V("name:oid, type:oid, value:oid"),AS:V("source:oid, lineno:int, target:oid, type:oid, value:oid, time_delta_in_seconds:float"),L:V("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),LH:V("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),TG:V("tag:oid"),S:V("start_time_delta:float"),STB:V("message:oid, time_delta_in_seconds:float"),RTB:V("message:oid, time_delta_in_seconds:float"),TBE:V("source:oid, lineno:int, method:oid, line_content:oid"),TBV:V("name:oid, type:oid, value:oid"),ETB:V("time_delta_in_seconds:float"),YS:V("source:oid, lineno:int, type:oid, value:oid, time_delta_in_seconds:float"),YR:V("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float")};$.RR=$.SR,$.RT=$.ST,$.RE=$.SE,$.RYR=$.YR;class q{constructor(){this.memo={}}decode_message_type(e,n){return(0,$[e])(this,n)}}function Y(e,n){const t=e.indexOf(n);if(t>0)return[e.substring(0,t),e.substring(t+1)]}function*W(e,n){var t,s,a;for(let o of e.split(/\\r?\\n/))if(o=o.trim(),o)try{const e=Y(o," ");if(e&&([a,s]=e,t=n.decode_message_type(a,s))){const e={message_type:a,decoded:t};yield e}}catch(e){console.log("Unable to decode message: "+o),console.log(e)}}function Z(e,n){const t=document.createElement("span");t.textContent=n,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}function G(e,n){switch(e.state.filterLevel){case"FAIL":return n>=2;case"WARN":return n>=1;case"PASS":return n>=0;case"NOT RUN":return!0}}function J(e){switch(e){case"FAIL":case"ERROR":return 2;case"WARN":return 1;case"NOT RUN":case"NOT_RUN":return-1;default:return 0}}class K{constructor(e){this.stack=[],this.exceptionMsg=e}pushEntry(e,n,t,s){const a=new Map;this.stack.push({source:e,lineno:n,method:t,lineContent:s,variables:a})}pushVar(e,n,t){this.stack.at(-1).variables.set(e,[n,t])}}class Q{constructor(){this.totalTests=0,this.totalFailures=0}clear(){this.totalTests=0,this.totalFailures=0,this.updateSummary()}onTestEndUpdateSummary(e){const n=e.decoded.status;this.totalTests+=1,"FAIL"!=n&&"ERROR"!=n||(this.totalFailures+=1),this.updateSummary()}updateSummary(){const e=p("summary");if(!e)return;const n=(""+this.totalTests).padStart(4),t=(""+this.totalFailures).padStart(4);if(e.textContent=`Total: ${n} Failures: ${t}`,0==this.totalFailures&&0==this.totalTests){const e=p("summary");e.classList.add("NOT_RUN"),e.classList.remove("PASS"),e.classList.remove("FAIL")}else if(1==this.totalFailures){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("PASS"),e.classList.add("FAIL")}else if(0==this.totalFailures&&1==this.totalTests){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("FAIL")}}}function X(e,n){const t=function(e){const n=document.createElement("li");return n.setAttribute("data-tree-id",e),n}(n),s=document.createElement("details");e&&(s.open=e),s.classList.add("NO_CHILDREN"),t.appendChild(s);const a=y();a.classList.add("detailContainer"),s.appendChild(a);const o=document.createElement("summary"),r=y();r.classList.add("summaryDiv"),o.appendChild(r);const i=v();i.className="summaryName",i.textContent="[summaryName]",r.appendChild(i);const l=v();return l.className="summaryInput emptySummaryInput",l.textContent="",r.appendChild(l),s.appendChild(o),{li:t,details:s,summary:o,summaryDiv:r,summaryName:i,summaryInput:l,detailContainer:a}}function ee(e,n){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${n}`,e.summaryInput.classList.remove("emptySummaryInput")):e.summaryInput.textContent+=`, ${n}`}function ne(e,n,t,s,a,o,r,i,l,d){const c=e.state.runIdToTreeState[e.runId],u="li_"+d;if(c){const e=c.openNodes;e&&(o=e[u])}const m=X(o,u),h=m.li,p=m.details,f=m.detailContainer,v=m.summary,E=m.summaryDiv,y=m.summaryName,C=m.summaryInput;if("LH"===a.message_type){y.textContent="";const e=w(t);y.appendChild(e)}else y.textContent=t;s&&(y.title=s),e.onClickReference&&(y.classList.add("span_link"),y.onclick=n=>{const t=[];let s=l.parent;for(;void 0!==s&&void 0!==s.message;)t.push(s.message),s=s.parent;n.preventDefault(),e.onClickReference({source:r,lineno:i,message:a.decoded,messageType:a.message_type,scope:t})});const b=g("ul_"+d);p.appendChild(b);const S={ul:b,li:h,details:p,detailContainer:f,summary:v,summaryName:y,summaryInput:C,source:r,lineno:i,appendContentChild:void 0,decodedMessage:a,maxLevelFoundInHierarchy:-1,summaryDiv:E};return S.appendContentChild=re.bind(S),n.appendContentChild(S),S}let te,se;function*ae(e){for(let n of e.childNodes)if(n instanceof HTMLDetailsElement){for(let e of n.childNodes)if(e instanceof HTMLUListElement)for(let n of oe(e))yield n;yield n}}function*oe(e){for(let n of e.childNodes)if(n instanceof HTMLLIElement)for(let e of ae(n))yield e}function re(e){const n=this;n.ul.appendChild(e.li),n.details.classList.contains("NO_CHILDREN")&&(n.details.classList.remove("NO_CHILDREN"),n.details.addEventListener("toggle",(function(){x()})),m().showExpand&&n.summary.addEventListener("mouseover",(e=>{!function(e){if(void 0===te){te=y(),te.classList.add("toolbarContainer");const e=E();e.appendChild(w(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path d="M7 12V7H6v5h1z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),e.onclick=()=>{!function(){if(void 0!==se){se.details.open=!0;for(let e of oe(se.ul))e.classList.contains("NO_CHILDREN")||(e.open=!0)}}()},e.classList.add("toolbarButton");const n=E();return n.appendChild(w(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),n.classList.add("toolbarButton"),n.onclick=()=>{!function(){if(void 0!==se){se.details.open=!1;for(let e of oe(se.ul))e.open=!1}}()},te.appendChild(n),void te.appendChild(e)}se=e,e.summaryDiv.appendChild(te)}(n)})))}var ie=(e,n,t)=>new Promise(((s,a)=>{var o=e=>{try{i(t.next(e))}catch(e){a(e)}},r=e=>{try{i(t.throw(e))}catch(e){a(e)}},i=e=>e.done?s(e.value):Promise.resolve(e.value).then(o,r);i((t=t.apply(e,n)).next())}));let le=0,de=-1;class ce{constructor(){this.stack=[]}handle(e){let n;switch(e.message_type){case"STB":return void this.stack.push(new K(e.decoded.message));case"TBE":return n=this.stack.at(-1),void n.pushEntry(e.decoded.source,e.decoded.lineno,e.decoded.method,e.decoded.line_content);case"TBV":return;case"ETB":return n=this.stack.pop(),n.stack.reverse(),n}}}class ue{constructor(){this.stack=[],this.messageNode={parent:void 0,message:void 0},this.id=0,this.finishedAddingInitialContents=!1,this.appendedMessagesIndex=-1,this.decoder=new q,this.seenSuiteTaskOrElement=!1,this.tbHandler=new ce,this.suiteErrored=!1,this.opts=m(),this.runId=this.opts.runId,this.summaryBuilder=new Q,this.lease=(le+=1,de=le,le),this.resetState()}resetState(){this.seenSuiteTaskOrElement=!1}isCurrentTreeBuilder(){return this.lease===de&&this.runId==this.opts.runId}clearAndInitializeTree(){this.summaryBuilder.clear(),this.resetState();const e=f("filterLevel");e&&(e.value=this.opts.state.filterLevel);const n=p("mainTree");n.replaceChildren();const t=g("ul_root");t.classList.add("tree"),n.appendChild(t),this.parent={ul:void 0,li:void 0,details:void 0,detailContainer:void 0,summary:void 0,summaryName:void 0,summaryInput:void 0,source:void 0,lineno:void 0,decodedMessage:void 0,appendContentChild:function(e){t.appendChild(e.li)},maxLevelFoundInHierarchy:-1,summaryDiv:void 0},this.stack.push(this.parent)}addInitialContents(){return ie(this,null,(function*(){for(const e of W(this.opts.initialContents,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}this.finishedAddingInitialContents=!0,yield this.onAppendedContents()}))}onAppendedContents(){return ie(this,null,(function*(){if(!this.finishedAddingInitialContents)return;if(!this.isCurrentTreeBuilder())return;const e=m();for(;this.appendedMessagesIndex+1<e.appendedContents.length;){this.appendedMessagesIndex+=1;const n=e.appendedContents[this.appendedMessagesIndex];for(const e of W(n,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}}}))}addOneMessage(e){return ie(this,null,(function*(){if(this.isCurrentTreeBuilder())try{this.addOneMessageSync(e)}catch(n){console.log("Error: handling message: "+JSON.stringify(e)+": "+n+" - "+JSON.stringify(n))}}))}addOneMessageSync(e){var n,t;let s,a,o=e.message_type;switch(o){case"SR":case"ST":case"SE":case"STB":this.seenSuiteTaskOrElement=!0;break;case"RR":if(this.seenSuiteTaskOrElement)return;o="SR";break;case"RT":if(this.seenSuiteTaskOrElement)return;o="ST";break;case"RE":if(this.seenSuiteTaskOrElement)return;o="SE";break;case"RTB":if(this.seenSuiteTaskOrElement)return;o="STB"}switch(this.id+=1,o){case"SR":this.messageNode={parent:this.messageNode,message:e};for(const n of document.querySelectorAll(".suiteHeader"))n.textContent=e.decoded.name;break;case"AS":a=ne(this.opts,this.parent,`${e.decoded.target} = `,`Assign to name: ${e.decoded.target}\\nAn object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),ee(a,e.decoded.value),this.addAssignCssClass(a);break;case"ST":this.messageNode={parent:this.messageNode,message:e},this.parent=ne(this.opts,this.parent,`${e.decoded.libname}.${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"SE":case"YR":if("SE"!=o||"UNTRACKED_GENERATOR"!=e.decoded.type){this.messageNode={parent:this.messageNode,message:e};let n=e.decoded.name;"YR"==o&&(n+=" (resumed)"),this.parent=ne(this.opts,this.parent,n,e.decoded.libname,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),"YR"==o&&this.addResumedCSSClass(this.parent),this.stack.push(this.parent)}else{const n=ne(this.opts,this.parent,`Create Generator: ${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addGeneratorCSSClass(n)}break;case"ER":this.messageNode=this.messageNode.parent;{const n=p("suiteResult");n.style.display="block",this.suiteErrored?(n.classList.add("ERROR"),n.textContent="Run Failed"):(n.classList.add("PASS"),n.textContent="Run Passed");const t=p("suiteRunStart");t&&(t.textContent+=` - Finished in: ${e.decoded.time_delta_in_seconds.toFixed(2)}s.`)}break;case"ET":this.messageNode=this.messageNode.parent;const r=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(r,this.parent,e),this.onEndSetStatusOrRemove(this.opts,r,e.decoded,this.parent,!1),this.summaryBuilder.onTestEndUpdateSummary(e),s=this.addDetailsCSSClasses(e.decoded.status,r),s&&(this.suiteErrored=!0,r.details.open=!0);break;case"EE":case"YS":if("EE"!=o||"UNTRACKED_GENERATOR"!=e.decoded.type){if("YS"==o){const n=ne(this.opts,this.parent,"Yielded",`Suspending function with yield.\\nYielding an object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addYieldedCSSClass(n),ee(n,e.decoded.value)}this.messageNode=this.messageNode.parent;let n=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(n,this.parent,e),this.onEndSetStatusOrRemove(this.opts,n,e.decoded,this.parent,!0),s=this.addDetailsCSSClasses(e.decoded.status,n),s&&(n.details.open=!0)}break;case"S":const i=e.decoded.start_time_delta;(null==(t=null==(n=this.parent)?void 0:n.decodedMessage)?void 0:t.decoded)&&(this.parent.decodedMessage.decoded.time_delta_in_seconds=i);break;case"EA":a=this.stack.at(-1),function(e,n,t,s){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${n} = ${s}`,e.summaryInput.title=`Argument: ${n}\\nArgument type: ${t}\\nRepresentation:\\n${s}`,e.summaryInput.classList.remove("emptySummaryInput")):(e.summaryInput.title+=`\\n\\nArgument: ${n}\\nArgument type: ${t}\\nRepresentation:\\n${s}`,e.summaryInput.textContent+=`, ${n} = ${s}`)}(a,e.decoded.name,e.decoded.type,e.decoded.value);break;case"L":case"LH":const l=e.decoded.level,d=function(e){switch(e){case"E":case"F":return 2;case"W":return 1;default:return 0}}(l);if(d>this.parent.maxLevelFoundInHierarchy&&(this.parent.maxLevelFoundInHierarchy=d),G(this.opts,d)){const n=ne(this.opts,this.parent,e.decoded.message,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());n.maxLevelFoundInHierarchy=d,function(e,n){const t=document.createElement("span");t.textContent=`LOG ${function(e){switch(e){case"E":return"ERROR";case"F":return"FAIL";case"W":return"WARN";case"I":return"INFO";default:return e}}(n)}`,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}(n,l),this.addDetailsCSSClasses(d,n)}break;case"STB":case"TBE":case"TBV":case"ETB":const c=this.tbHandler.handle(e);if(c&&c.stack.length>0){const n=c.stack[0];a=ne(this.opts,this.parent,c.exceptionMsg,"",e,!1,n.source,n.lineno,this.messageNode,this.id.toString()),this.addExceptionCssClass(a)}break;case"T":const u=p("suiteRunStart");u&&(u.textContent=e.decoded.time)}}addAssignCssClass(e){e.details.classList.add("variableParent"),e.details.classList.add("leafNode")}addExceptionCssClass(e){e.details.classList.add("exceptionParent"),e.details.classList.add("leafNode")}addYieldedCSSClass(e){e.details.classList.add("yiededParent"),e.details.classList.add("leafNode")}addResumedCSSClass(e){e.details.classList.add("resumedParent")}addGeneratorCSSClass(e){e.details.classList.add("generatorParent"),e.details.classList.add("leafNode")}addDetailsCSSClasses(e,n){let t,s=!1;return t="string"==typeof e?J(e):e,t>=2?(n.details.classList.add("errorParent"),s=!0):1==t?n.details.classList.add("warnParent"):n.details.classList.add("passParent"),n.details.classList.contains("parentNode")||n.details.classList.contains("leafNode")||(0===n.ul.children.length?n.details.classList.add("leafNode"):n.details.classList.add("parentNode")),s}onEndUpdateMaxLevelFoundInHierarchyFromStatus(e,n,t){const s=J(t.decoded.status);s>e.maxLevelFoundInHierarchy&&(e.maxLevelFoundInHierarchy=s),e.maxLevelFoundInHierarchy>n.maxLevelFoundInHierarchy&&(n.maxLevelFoundInHierarchy=e.maxLevelFoundInHierarchy)}onEndSetStatusOrRemove(e,n,t,s,a){const o=t.status;if(G(e,n.maxLevelFoundInHierarchy)){if(a&&n.maxLevelFoundInHierarchy<=0){const e=50;if(s.ul.childElementCount>e){const e=n.summaryName.textContent;if(e&&e.toLowerCase().includes("iteration")){const e=n.li.previousSibling,t=C(n.li);if(n.li.remove(),b(e))e.getElementsByClassName("FINAL_SPAN")[0].textContent=n.summaryName.textContent;else{const e=X(!1,t);e.summaryName.textContent=n.summaryName.textContent,e.summary.classList.add("HIDDEN");const a=v();a.setAttribute("role","button"),a.textContent="...",a.classList.add("label"),a.classList.add("HIDDEN"),a.classList.add("inline"),e.summaryDiv.appendChild(a);const o=v();o.setAttribute("role","button"),o.classList.add("FINAL_SPAN"),e.summaryDiv.appendChild(o),Z(e,"HIDDEN"),b(e.li,!0),s.ul.appendChild(e.li)}return}}}if(n.summary,Z(n,o),null!=n.source&&n.source.length>0){const e=function(e){let n=e,t=Math.max(e.lastIndexOf("/"),e.lastIndexOf("\\\\"));return t>0&&(n=e.substring(t+1)),n}(n.source),t=document.createElement("span");t.textContent=e,t.classList.add("summaryFileName"),t.title=n.source,n.summaryDiv.appendChild(t)}if(this.opts.showTime){const e=n.decodedMessage.decoded.time_delta_in_seconds;void 0!==e&&e>=0&&function(e,n){const t=document.createElement("span");t.textContent=` (${n.toFixed(2)}s)`,t.classList.add("timeLabel"),e.summaryDiv.appendChild(t)}(n,t.time_delta_in_seconds-e)}}else n.li.remove()}}var me=(e,n,t)=>new Promise(((s,a)=>{var o=e=>{try{i(t.next(e))}catch(e){a(e)}},r=e=>{try{i(t.throw(e))}catch(e){a(e)}},i=e=>e.done?s(e.value):Promise.resolve(e.value).then(o,r);i((t=t.apply(e,n)).next())}));let he;function pe(){return me(this,null,(function*(){he=new ue,he.clearAndInitializeTree(),yield he.addInitialContents()}))}function fe(e){let n={type:"event",seq:d(),event:"onClickReference"};n.data=e,o(n)}function ge(e){N();const n=m();n.runId=e.runId,n.initialContents=e.initialContents,void 0!==s&&(n.onClickReference=fe),n.appendedContents=[],n.allRunIdsToLabel=e.allRunIdsToLabel,T(n.allRunIdsToLabel,n.runId),pe()}t(739),i.setContents=ge,i.appendContents=function(e){const n=m();n.runId===e.runId&&(n.appendedContents.push(e.appendContents),void 0!==he&&he.onAppendedContents())},i.updateLabel=function(e){const n=m();n.allRunIdsToLabel[e.runId]=e.label,T(n.allRunIdsToLabel,n.runId)},window.onChangedRun=function(){const e=f("selectedRun").value;let n={type:"event",seq:d(),event:"onSetCurrentRunId"};n.data={runId:e},o(n)},window.onChangedFilterLevel=function(){!function(e){const n=m();n.state.filterLevel!==e&&(n.state.filterLevel=e,N(),pe())}(f("filterLevel").value)},window.setContents=ge,window.setShowTime=function(e){m().showTime=e},window.setShowExpand=function(e){m().showExpand=e},window.getSampleContents=function(){return JSON.parse(\'"V 1\\\\nI \\\\"sys.platform=win32\\\\"\\\\nI \\\\"python=3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)]\\\\"\\\\nI \\\\"robot=5.1a3.dev1\\\\"\\\\nT 2022-10-19T09:48:34.018\\\\nM a:\\\\"Robot1\\\\"\\\\nM b:\\\\"s1\\\\"\\\\nM c:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\robot1.robot\\\\"\\\\nSR a|b|c|0.035\\\\nM d:\\\\"Simple Task\\\\"\\\\nM e:\\\\"s1-t1\\\\"\\\\nST d|e|16|0.036\\\\nM f:\\\\"First keyword\\\\"\\\\nM g:\\\\"\\\\"\\\\nM h:\\\\"KEYWORD\\\\"\\\\nSE f|g|h|g|c|17|0.036\\\\nM i:\\\\"No Operation\\\\"\\\\nM j:\\\\"BuiltIn\\\\"\\\\nM k:\\\\"Does absolutely nothing.\\\\"\\\\nSE i|j|h|k|c|8|0.037\\\\nM l:\\\\"PASS\\\\"\\\\nEE l|0.037\\\\nM m:\\\\"Log\\\\"\\\\nM n:\\\\"Logs the given message with the given level.\\\\"\\\\nSE m|j|h|n|c|10|0.037\\\\nM o:\\\\"Some warning message\\\\"\\\\nEA o\\\\nM p:\\\\"level=WARN\\\\"\\\\nEA p\\\\nEE l|0.046\\\\nM q:\\\\"Another keyword\\\\"\\\\nM r:\\\\"another\\\\"\\\\nSE q|r|h|g|c|11|0.047\\\\nM s:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\another.robot\\\\"\\\\nSE i|j|h|k|s|3|0.047\\\\nEE l|0.047\\\\nEE l|0.047\\\\nM t:\\\\"Another in sub keyword\\\\"\\\\nM u:\\\\"another_sub\\\\"\\\\nSE t|u|h|g|c|12|0.047\\\\nM v:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\sub\\\\\\\\\\\\\\\\another_sub.robot\\\\"\\\\nSE i|j|h|k|v|6|0.048\\\\nEE l|0.048\\\\nSE m|j|h|n|v|7|0.048\\\\nM w:\\\\"Some error message\\\\"\\\\nEA w\\\\nM x:\\\\"level=ERROR\\\\"\\\\nEA x\\\\nEE l|0.049\\\\nEE l|0.049\\\\nEE l|0.049\\\\nSE m|j|h|n|c|18|0.049\\\\nM y:\\\\"Some <data &encode <\\/script>\\\\"\\\\nEA y\\\\nEE l|0.049\\\\nM z:\\\\"Create Dictionary\\\\"\\\\nM A:\\\\"Creates and returns a dictionary based on the given ``items``.\\\\"\\\\nSE z|j|h|A|c|19|0.049\\\\nM B:\\\\"a=1\\\\"\\\\nEA B\\\\nM C:\\\\"b=1\\\\"\\\\nEA C\\\\nEE l|0.05\\\\nSE m|j|h|n|c|20|0.05\\\\nM D:\\\\"${dct}\\\\"\\\\nEA D\\\\nEE l|0.051\\\\nET l|g|0.051\\\\nM E:\\\\"Check 1\\\\"\\\\nM F:\\\\"s1-t2\\\\"\\\\nST E|F|22|0.051\\\\nSE f|g|h|g|c|23|0.051\\\\nSE i|j|h|k|c|8|0.052\\\\nEE l|0.052\\\\nSE m|j|h|n|c|10|0.052\\\\nEA o\\\\nEA p\\\\nEE l|0.052\\\\nSE q|r|h|g|c|11|0.053\\\\nSE i|j|h|k|s|3|0.053\\\\nEE l|0.053\\\\nEE l|0.053\\\\nSE t|u|h|g|c|12|0.053\\\\nSE i|j|h|k|v|6|0.054\\\\nEE l|0.054\\\\nSE m|j|h|n|v|7|0.054\\\\nEA w\\\\nEA x\\\\nEE l|0.054\\\\nEE l|0.055\\\\nEE l|0.055\\\\nM G:\\\\"${counter} IN RANGE [ 0 | 3 ]\\\\"\\\\nM H:\\\\"FOR\\\\"\\\\nSE G|g|H|g|c|25|0.055\\\\nM I:\\\\"${counter} = 0\\\\"\\\\nM J:\\\\"ITERATION\\\\"\\\\nSE I|g|J|g|c|25|0.055\\\\nM K:\\\\"${counter} == 2\\\\"\\\\nM L:\\\\"IF\\\\"\\\\nSE K|g|L|g|c|26|0.055\\\\nM M:\\\\"Fail\\\\"\\\\nM N:\\\\"Fails the test with the given message and optionally alters its tags.\\\\"\\\\nSE M|j|h|N|c|27|0.056\\\\nM O:\\\\"Failed execution for some reason...\\\\"\\\\nEA O\\\\nM P:\\\\"NOT RUN\\\\"\\\\nEE P|0.056\\\\nEE P|0.056\\\\nSE m|j|h|n|c|29|0.056\\\\nM Q:\\\\"${counter}\\\\"\\\\nEA Q\\\\nEE l|0.056\\\\nEE l|0.057\\\\nM R:\\\\"${counter} = 1\\\\"\\\\nSE R|g|J|g|c|25|0.057\\\\nSE K|g|L|g|c|26|0.057\\\\nSE M|j|h|N|c|27|0.057\\\\nEA O\\\\nEE P|0.057\\\\nEE P|0.057\\\\nSE m|j|h|n|c|29|0.058\\\\nEA Q\\\\nEE l|0.058\\\\nEE l|0.058\\\\nM S:\\\\"${counter} = 2\\\\"\\\\nSE S|g|J|g|c|25|0.058\\\\nSE K|g|L|g|c|26|0.058\\\\nSE M|j|h|N|c|27|0.059\\\\nEA O\\\\nM T:\\\\"FAIL\\\\"\\\\nEE T|0.059\\\\nEE T|0.059\\\\nSE m|j|h|n|c|29|0.059\\\\nEA Q\\\\nEE P|0.059\\\\nEE T|0.06\\\\nEE T|0.06\\\\nET T|O|0.06\\\\nM U:\\\\"Check 2\\\\"\\\\nM V:\\\\"s1-t3\\\\"\\\\nST U|V|32|0.06\\\\nM W:\\\\"Set Variable\\\\"\\\\nM X:\\\\"Returns the given values which can then be assigned to a variables.\\\\"\\\\nSE W|j|h|X|c|33|0.061\\\\nM Y:\\\\"3\\\\"\\\\nEA Y\\\\nEE l|0.061\\\\nM Z:\\\\"${counter} <= 2\\\\"\\\\nM 0:\\\\"WHILE\\\\"\\\\nSE Z|g|0|g|c|34|0.061\\\\nSE g|g|J|g|c|34|0.062\\\\nM 1:\\\\"Evaluate\\\\"\\\\nM 2:\\\\"Evaluates the given expression in Python and returns the result.\\\\"\\\\nSE 1|j|h|2|c|35|0.062\\\\nM 4:\\\\"$counter-1\\\\"\\\\nEA 4\\\\nEE P|0.062\\\\nSE m|j|h|n|c|36|0.062\\\\nM 5:\\\\"Current counter: ${counter}\\\\"\\\\nEA 5\\\\nEA p\\\\nEE P|0.062\\\\nEE P|0.062\\\\nEE P|0.063\\\\nET l|g|0.063\\\\nM 6:\\\\"Check 3\\\\"\\\\nM 7:\\\\"s1-t4\\\\"\\\\nST 6|7|39|0.064\\\\nM 8:\\\\"TRY\\\\"\\\\nSE g|g|8|g|c|40|0.064\\\\nSE i|j|h|k|c|41|0.064\\\\nEE l|0.064\\\\nEE l|0.064\\\\nM 9:\\\\"message\\\\"\\\\nM aa:\\\\"EXCEPT\\\\"\\\\nSE 9|g|aa|g|c|42|0.064\\\\nSE i|j|h|k|c|43|0.065\\\\nEE P|0.065\\\\nEE P|0.065\\\\nM ab:\\\\"FINALLY\\\\"\\\\nSE g|g|ab|g|c|44|0.065\\\\nSE i|j|h|k|c|45|0.065\\\\nEE l|0.065\\\\nEE l|0.065\\\\nET l|g|0.066\\\\nER T|0.067\\\\n"\')}},739:(e,n,t)=>{var s=t(379),a=t.n(s),o=t(599),r={injectType:"singletonStyleTag",insert:"head",singleton:!0};a()(o.Z,r),o.Z.locals},379:(e,n,t)=>{var s,a=function(){var e={};return function(n){if(void 0===e[n]){var t=document.querySelector(n);if(window.HTMLIFrameElement&&t instanceof window.HTMLIFrameElement)try{t=t.contentDocument.head}catch(e){t=null}e[n]=t}return e[n]}}(),o=[];function r(e){for(var n=-1,t=0;t<o.length;t++)if(o[t].identifier===e){n=t;break}return n}function i(e,n){for(var t={},s=[],a=0;a<e.length;a++){var i=e[a],l=n.base?i[0]+n.base:i[0],d=t[l]||0,c="".concat(l," ").concat(d);t[l]=d+1;var u=r(c),m={css:i[1],media:i[2],sourceMap:i[3]};-1!==u?(o[u].references++,o[u].updater(m)):o.push({identifier:c,updater:f(m,n),references:1}),s.push(c)}return s}function l(e){var n=document.createElement("style"),s=e.attributes||{};if(void 0===s.nonce){var o=t.nc;o&&(s.nonce=o)}if(Object.keys(s).forEach((function(e){n.setAttribute(e,s[e])})),"function"==typeof e.insert)e.insert(n);else{var r=a(e.insert||"head");if(!r)throw new Error("Couldn\'t find a style target. This probably means that the value for the \'insert\' parameter is invalid.");r.appendChild(n)}return n}var d,c=(d=[],function(e,n){return d[e]=n,d.filter(Boolean).join("\\n")});function u(e,n,t,s){var a=t?"":s.media?"@media ".concat(s.media," {").concat(s.css,"}"):s.css;if(e.styleSheet)e.styleSheet.cssText=c(n,a);else{var o=document.createTextNode(a),r=e.childNodes;r[n]&&e.removeChild(r[n]),r.length?e.insertBefore(o,r[n]):e.appendChild(o)}}function m(e,n,t){var s=t.css,a=t.media,o=t.sourceMap;if(a?e.setAttribute("media",a):e.removeAttribute("media"),o&&"undefined"!=typeof btoa&&(s+="\\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o))))," */")),e.styleSheet)e.styleSheet.cssText=s;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(s))}}var h=null,p=0;function f(e,n){var t,s,a;if(n.singleton){var o=p++;t=h||(h=l(n)),s=u.bind(null,t,o,!1),a=u.bind(null,t,o,!0)}else t=l(n),s=m.bind(null,t,n),a=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(t)};return s(e),function(n){if(n){if(n.css===e.css&&n.media===e.media&&n.sourceMap===e.sourceMap)return;s(e=n)}else a()}}e.exports=function(e,n){(n=n||{}).singleton||"boolean"==typeof n.singleton||(n.singleton=(void 0===s&&(s=Boolean(window&&document&&document.all&&!window.atob)),s));var t=i(e=e||[],n);return function(e){if(e=e||[],"[object Array]"===Object.prototype.toString.call(e)){for(var s=0;s<t.length;s++){var a=r(t[s]);o[a].references--}for(var l=i(e,n),d=0;d<t.length;d++){var c=r(t[d]);0===o[c].references&&(o[c].updater(),o.splice(c,1))}t=l}}}}},n={};function t(s){var a=n[s];if(void 0!==a)return a.exports;var o=n[s]={id:s,exports:{}};return e[s](o,o.exports,t),o.exports}t.n=e=>{var n=e&&e.__esModule?()=>e.default:()=>e;return t.d(n,{a:n}),n},t.d=(e,n)=>{for(var s in n)t.o(n,s)&&!t.o(e,s)&&Object.defineProperty(e,s,{enumerable:!0,get:n[s]})},t.o=(e,n)=>Object.prototype.hasOwnProperty.call(e,n),t.nc=void 0,t(457),t(739)})();</script></body><script>window.setShowTime(true);\n    window.setShowExpand(false);\n    try {\n        const vscode = acquireVsCodeApi();\n        window.setVSCodeAPI(vscode);\n        document.getElementById("selectRunContainer").style.display = "block";\n    } catch (err) {\n        // That\'s ok (not running in VSCode).\n        window.setContents({\n            "initialContents": window.getSampleContents(),\n        });\n    }</script></html>'}
+FILE_CONTENTS = {'index.html': '<!doctype html><html><head><meta charset="utf-8"/><title class="suiteHeader">Robocorp Log</title><meta name="viewport" content="width=device-width,initial-scale=1"/></head><body><div class="headerTitleSection"><h3 class="suiteHeader">Robocorp Log</h3><span id="suiteResult" class="label" style="display: none;"></span></div><div id="suiteRunStart" class="headerRunDetails"></div><div class="headers"><span class="headerSource"></span> <span class="headerInputs">Details</span></div><div id="mainTree"></div><script>(()=>{"use strict";var e={599:(e,n,t)=>{t.d(n,{Z:()=>o});var s=t(645),a=t.n(s)()((function(e){return e[1]}));a.push([e.id,\'/* ******************************* */\\n/* CONTAINERS ETC */\\n\\n/* box model reset */\\n* {\\n    box-sizing: border-box;\\n}\\n\\nhtml,\\nbody {\\n    margin: 0;\\n    padding: 0;\\n    height: 100%;\\n}\\n\\n:root {\\n    --right-column-width-narrow: 50vw;\\n    --right-column-width-wide: 60vw;\\n    /* from here: https://qwtel.com/posts/software/the-monospaced-system-ui-css-font-stack/ */\\n    --sans-font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen", "Ubuntu",\\n        "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue", Arial, sans-serif;\\n    /* from here: https://qwtel.com/posts/software/the-monospaced-system-ui-css-font-stack/ */\\n    --fixed-font-family: ui-monospace, Menlo, Monaco, "Cascadia Mono", "Segoe UI Mono", "Roboto Mono", "Oxygen Mono",\\n        "Ubuntu Monospace", "Source Code Pro", "Fira Mono", "Droid Sans Mono", "Courier New", monospace;\\n}\\n\\n/* ******************************* */\\n/* THEMING SUPPORT */\\n\\n@media (prefers-color-scheme: light) {\\n    :root {\\n        --log-color-error: #e84f5c;\\n        --log-color-success: #219f7f;\\n        --log-color-variable: #5070b4;\\n\\n        --log-color-warn: #93801c;\\n        --log-color-disabled: #999999;\\n        --log-color-border: #dddddd;\\n\\n        --log-color-text: #000000;\\n        --log-color-text-weaker: #444444;\\n        --log-color-text-weakest: #666666;\\n\\n        --log-color-bg: #ffffff;\\n        --log-color-bg-raised: #f3f3f3;\\n    }\\n}\\n\\n@media (prefers-color-scheme: dark) {\\n    :root {\\n        --log-color-error: #e84f5c;\\n        --log-color-success: #219f7f;\\n        --log-color-warn: #fff565;\\n        --log-color-variable: #4094c5;\\n\\n        --log-color-disabled: #666666;\\n        --log-color-border: #444444;\\n\\n        --log-color-text: #eeeeee;\\n        --log-color-text-weaker: #bbbbbb;\\n        --log-color-text-weakest: #666666;\\n\\n        --log-color-bg: #222222;\\n        --log-color-bg-raised: #333333;\\n    }\\n}\\n\\nbody {\\n    display: flex;\\n    flex-direction: column;\\n    padding: 1rem;\\n    font-size: 0.8rem;\\n    font-family: var(--sans-font-family);\\n    color: var(--log-color-text);\\n    background-color: var(--log-color-bg);\\n}\\n\\nul {\\n    list-style-type: none;\\n    padding-inline-start: 0px;\\n    margin-block-start: 0px;\\n}\\n\\n#mainTree {\\n    white-space: nowrap;\\n    overflow: auto;\\n    flex-grow: 1;\\n}\\n\\n/* ******************************* */\\n/* TREE */\\n\\n.tree li {\\n    display: block;\\n    position: relative;\\n    padding-left: 0px;\\n}\\n\\n/* nesting level vertical line */\\n.tree ul:not(:first-child),\\n.detailContainer {\\n    border-left: 1px solid var(--log-color-border);\\n\\n    /* centering the line with the icon */\\n    margin-left: 0.65rem;\\n\\n    /* nesting indentation */\\n    padding-left: 0.8rem;\\n}\\n\\ndetails.errorParent .tree ul:not(:first-child),\\ndetails.errorParent .detailContainer {\\n    border-color: var(--log-color-error);\\n}\\n\\n/* ******************************* */\\n/* SUMMARY ROW FOR EACH CODE ROW */\\n\\ndetails.parentNode > summary,\\ndetails.errorParent.leafNode > summary {\\n    cursor: pointer;\\n}\\n\\ndetails > summary {\\n    padding-top: 0.25rem;\\n    padding-bottom: 0.25rem;\\n    padding-left: 0.25rem;\\n\\n    /* chrome needs this, safari doesn\\\'t */\\n    list-style: none;\\n}\\n\\ndetails > summary:hover {\\n    background-color: var(--log-color-bg-raised);\\n    border-radius: 2px;\\n}\\n\\ndetails > summary::-webkit-details-marker {\\n    display: none;\\n}\\n\\ndetails > summary::marker {\\n    display: none;\\n}\\n\\ndetails > summary::before {\\n    background-color: var(--log-color-success);\\n}\\n\\ndetails.errorParent > summary::before {\\n    background-color: var(--log-color-error);\\n}\\n\\ndetails.warnParent > summary::before {\\n    background-color: var(--log-color-warn);\\n}\\n\\n/* icon from: https://github.com/twbs/icons/blob/main/icons/caret-right-square-fill.svg */\\ndetails > summary::before {\\n    position: absolute;\\n    left: 0.25rem;\\n    top: 4px;\\n\\n    /* chrome seems to need the \\\'-webkit\\\' prefix here */\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="black" class="bi bi-caret-right-square-fill" viewBox="0 0 16 16"><path d="M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm5.5 10a.5.5 0 0 0 .832.374l4.5-4a.5.5 0 0 0 0-.748l-4.5-4A.5.5 0 0 0 5.5 4v8z"/></svg>\\\');\\n    width: 1rem;\\n    height: 1rem;\\n    display: inline-block;\\n    content: "";\\n}\\n\\n/* filled icon */\\n/*details.leafNode.passParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square-fill" viewBox="0 0 16 16"><path d="M2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2zm10.03 4.97a.75.75 0 0 1 .011 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.75.75 0 0 1 1.08-.022z"/></svg>\\\');\\n}*/\\n\\ndetails.leafNode.passParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M14 1a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1h12zM2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2z"/><path d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.235.235 0 0 1 .02-.022z"/></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (debug-pause) */\\ndetails.leafNode.yiededParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M4.5 3H6v10H4.5V3zm7 0v10H10V3h1.5z"></path></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (circuit-board) */\\ndetails.leafNode.generatorParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M14.5 1h-13l-.5.5v13l.5.5h13l.5-.5v-13l-.5-.5zM14 14H5v-2h2.3c.3.6 1 1 1.7 1 1.1 0 2-.9 2-2s-.9-2-2-2-2 .9-2 2H4v3H2V2h2v2.3c-.6.3-1 1-1 1.7 0 1.1.9 2 2 2s2-.9 2-2h2c0 1.1.9 2 2 2s2-.9 2-2-.9-2-2-2c-.7 0-1.4.4-1.7 1H6.7c-.3-.6-1-1-1.7-1V2h9v12zm-6-3c0-.6.4-1 1-1s1 .4 1 1-.4 1-1 1-1-.4-1-1zM5 5c.6 0 1 .4 1 1s-.4 1-1 1-1-.4-1-1 .4-1 1-1zm6 0c.6 0 1 .4 1 1s-.4 1-1 1-1-.4-1-1 .4-1 1-1z"></path></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (debug-restart-frame) */\\ndetails.resumedParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M1 10V9h5.207a5.48 5.48 0 0 0-.185 1H1zm6.257-3a5.54 5.54 0 0 1 1.08-1H1v1h6.257zM6.6 13a5.465 5.465 0 0 1-.393-1H1v1h5.6zM15 3v1H1V3h14zm-3.36 10.031a2.531 2.531 0 1 0-2.192-3.797h1.068v.844h-1.97l-.421-.422v-2.25h.844v1.032a3.375 3.375 0 1 1-.423 3.412l.782-.318a2.532 2.532 0 0 0 2.313 1.5z"></path></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (symbol-variable) */\\ndetails.leafNode.variableParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M2 5h2V4H1.5l-.5.5v8l.5.5H4v-1H2V5zm12.5-1H12v1h2v7h-2v1h2.5l.5-.5v-8l-.5-.5zm-2.74 2.57L12 7v2.51l-.3.45-4.5 2h-.46l-2.5-1.5-.24-.43v-2.5l.3-.46 4.5-2h.46l2.5 1.5zM5 9.71l1.5.9V9.28L5 8.38v1.33zm.58-2.15l1.45.87 3.39-1.5-1.45-.87-3.39 1.5zm1.95 3.17l3.5-1.56v-1.4l-3.5 1.55v1.41z"></path></svg>\\\');\\n    background-color: var(--log-color-variable);\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (bracket-error) */\\ndetails.leafNode.exceptionParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M6 2.97184V2.98361H5.91083C5.71113 2.98361 5.5238 3.02427 5.34802 3.10513C5.17461 3.18275 5.02193 3.28942 4.89086 3.42437C4.76421 3.55475 4.66135 3.71034 4.58238 3.89205C4.50833 4.07152 4.47134 4.26019 4.47134 4.45902C4.47134 4.68725 4.4753 4.9134 4.48321 5.13749C4.49125 5.36105 4.49127 5.58262 4.48324 5.80219C4.47914 6.01973 4.46082 6.2333 4.42826 6.44285C4.39513 6.65175 4.33913 6.85263 4.26039 7.04464C4.18091 7.23843 4.07258 7.42254 3.93616 7.59702C3.82345 7.74119 3.68538 7.87538 3.52283 8C3.68538 8.12462 3.82345 8.25881 3.93616 8.40298C4.07258 8.57746 4.18091 8.76157 4.26039 8.95536C4.33921 9.14757 4.39513 9.35024 4.42823 9.56312C4.46084 9.76883 4.47914 9.98246 4.48324 10.2039C4.49127 10.4195 4.49125 10.6411 4.48321 10.8686C4.4753 11.0885 4.47134 11.3127 4.47134 11.541C4.47134 11.744 4.50838 11.9346 4.58223 12.1137C4.66104 12.2911 4.76386 12.4469 4.89086 12.5818C5.02194 12.7126 5.17396 12.8191 5.34763 12.9008C5.52346 12.9777 5.71095 13.0164 5.91083 13.0164H6V13.2V14H5.91083C5.59743 14 5.29407 13.9384 5.00128 13.8153C4.70818 13.692 4.44942 13.5153 4.22578 13.285C4.00311 13.0558 3.83793 12.805 3.73283 12.5323L3.73232 12.531C3.63387 12.265 3.56819 11.9903 3.53535 11.7072L3.53516 11.7055C3.50677 11.4215 3.4987 11.1316 3.51084 10.8357C3.52272 10.5462 3.52866 10.2567 3.52866 9.96721C3.52866 9.76883 3.48986 9.58047 3.41201 9.40108L3.41129 9.39942C3.33659 9.21871 3.23428 9.0637 3.10412 8.93352L3.10221 8.93161C2.97577 8.79762 2.82457 8.69157 2.64742 8.61396L2.64601 8.61334C2.47001 8.53238 2.28465 8.4918 2.08917 8.4918H2V8.4V7.6V7.5082H2.08917C2.28497 7.5082 2.4706 7.46954 2.64672 7.3925C2.82466 7.31055 2.97644 7.20405 3.10317 7.07359C3.23423 6.93866 3.33687 6.78296 3.4116 6.60601L3.412 6.60507C3.48974 6.42594 3.52866 6.23556 3.52866 6.03279C3.52866 5.74329 3.52272 5.45379 3.51084 5.16428C3.4987 4.86844 3.50678 4.5805 3.53519 4.30053L3.53533 4.29917C3.56814 4.01201 3.63382 3.7352 3.73233 3.46898L3.73282 3.46766C3.83792 3.19498 4.00311 2.94422 4.22578 2.71498C4.44942 2.48474 4.70818 2.30798 5.00128 2.18473C5.29407 2.06161 5.59743 2 5.91083 2H6V2.97184ZM13.9232 8.4918H14V8.4V7.6V7.5082H13.9108C13.7153 7.5082 13.53 7.46762 13.354 7.38666L13.3526 7.38604C13.1754 7.30844 13.0242 7.20238 12.8978 7.06839L12.8959 7.06648C12.7657 6.9363 12.6634 6.78129 12.5887 6.60058L12.588 6.59892C12.5101 6.41953 12.4713 6.23117 12.4713 6.03279C12.4713 5.74329 12.4773 5.45379 12.4892 5.16428C12.5013 4.86842 12.4932 4.57848 12.4648 4.29454L12.4646 4.29285C12.4318 4.00971 12.3661 3.73502 12.2677 3.46897L12.2672 3.46766C12.1621 3.19499 11.9969 2.94422 11.7742 2.71498C11.5506 2.48474 11.2918 2.30798 10.9987 2.18473C10.7059 2.06161 10.4026 2 10.0892 2H10V2.8V2.98361H10.0892C10.2891 2.98361 10.4765 3.0223 10.6524 3.09917C10.826 3.18092 10.9781 3.28736 11.1091 3.41823C11.2361 3.55305 11.339 3.70889 11.4178 3.88628C11.4916 4.0654 11.5287 4.25596 11.5287 4.45902C11.5287 4.68727 11.5247 4.91145 11.5168 5.13142C11.5088 5.35894 11.5087 5.58049 11.5168 5.79605C11.5209 6.01754 11.5392 6.23117 11.5718 6.43688C11.6049 6.64976 11.6608 6.85243 11.7396 7.04464C11.8191 7.23843 11.9274 7.42254 12.0638 7.59702C12.1765 7.74119 12.3146 7.87538 12.4772 8L12.4456 8.02455C12.9764 8.08338 13.4758 8.24605 13.9232 8.4918Z"></path><path fill-rule="evenodd" clip-rule="evenodd" d="M10.3333 9.50559C10.8266 9.17595 11.4067 9 12 9C12.7954 9.00098 13.5578 9.31736 14.1202 9.87976C14.6826 10.4422 14.999 11.2047 15 12C15 12.5933 14.8241 13.1734 14.4944 13.6667C14.1648 14.1601 13.6962 14.5446 13.1481 14.7716C12.5999 14.9987 11.9967 15.0581 11.4147 14.9424C10.8328 14.8266 10.2982 14.5409 9.87868 14.1213C9.45912 13.7018 9.1734 13.1672 9.05765 12.5853C8.94189 12.0033 9.0013 11.4001 9.22836 10.8519C9.45543 10.3038 9.83994 9.83524 10.3333 9.50559ZM13.1464 10.1464L12 11.2929L10.8536 10.1464L10.1465 10.8535L11.2929 12L10.1464 13.1464L10.8536 13.8536L12 12.7071L13.1465 13.8535L13.8536 13.1464L12.7071 12L13.8536 10.8536L13.1464 10.1464Z"></path></svg>\\\');\\n    background-color: var(--log-color-error);\\n}\\n.exceptionParent {\\n    font-weight: bold;\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (error) */\\ndetails.leafNode.errorParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M8.6 1c1.6.1 3.1.9 4.2 2 1.3 1.4 2 3.1 2 5.1 0 1.6-.6 3.1-1.6 4.4-1 1.2-2.4 2.1-4 2.4-1.6.3-3.2.1-4.6-.7-1.4-.8-2.5-2-3.1-3.5C.9 9.2.8 7.5 1.3 6c.5-1.6 1.4-2.9 2.8-3.8C5.4 1.3 7 .9 8.6 1zm.5 12.9c1.3-.3 2.5-1 3.4-2.1.8-1.1 1.3-2.4 1.2-3.8 0-1.6-.6-3.2-1.7-4.3-1-1-2.2-1.6-3.6-1.7-1.3-.1-2.7.2-3.8 1-1.1.8-1.9 1.9-2.3 3.3-.4 1.3-.4 2.7.2 4 .6 1.3 1.5 2.3 2.7 3 1.2.7 2.6.9 3.9.6zM7.9 7.5L10.3 5l.7.7-2.4 2.5 2.4 2.5-.7.7-2.4-2.5-2.4 2.5-.7-.7 2.4-2.5-2.4-2.5.7-.7 2.4 2.5z"/></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (warn) */\\ndetails.leafNode.warnParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M7.56 1h.88l6.54 12.26-.44.74H1.44L1 13.26 7.56 1zM8 2.28L2.28 13H13.7L8 2.28zM8.625 12v-1h-1.25v1h1.25zm-1.25-2V6h1.25v4h-1.25z"/></svg>\\\');\\n}\\n\\ndetails.parentNode > summary::before,\\ndetails.parentNode.errorParent > summary::before {\\n    transform-origin: 8px 8px;\\n    transform: rotate(0deg);\\n    transition: transform 0.2s ease-out !important;\\n}\\n\\ndetails[open].parentNode > summary::before,\\ndetails[open].parentNode.errorParent > summary::before {\\n    transform: rotate(90deg);\\n}\\n\\ndetails[open] > summary > .summaryDiv > .summaryInput {\\n    /* Display full input parameters when expanded by adjusting the\\n       white-space to wrap the contents. Even nodes that don\\\'t have\\n       children can be expanded in this way, but it is not obvious\\n       since there is no triangle icon next to them. */\\n    white-space: initial;\\n}\\n\\n.summaryDiv {\\n    /* aligns code line correctly with the icon */\\n    display: flex;\\n    margin-left: 1.2rem;\\n}\\n\\n.summaryDiv > .label {\\n    order: 2;\\n}\\n\\n.summaryDiv > .summaryName {\\n    order: 1;\\n\\n    margin-left: 0.5rem;\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n}\\n\\n.summaryDiv > .summaryName,\\n.detailContainer > .detailInfo {\\n    /* this forces the correct column size, see:\\n       https://makandracards.com/makandra/66994-css-flex-and-min-width */\\n    min-width: 0;\\n}\\n\\ndetails.errorParent > summary > .summaryDiv > .summaryName {\\n    font-weight: bold;\\n}\\n\\n.summaryDiv > .summaryInput {\\n    order: 4;\\n    margin-left: auto;\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n.summaryDiv > .summaryInput.emptySummaryInput {\\n    color: var(--log-color-text-weakest);\\n}\\n\\n.detailContainer {\\n    display: flex;\\n}\\n\\n.detailContainer > .detailInfo {\\n    margin-right: auto;\\n}\\n\\n.summaryDiv > .summaryInput,\\n.detailContainer > .detailInputs {\\n    flex: 0 0 var(--right-column-width-wide);\\n    padding-left: 0.5rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n}\\n\\n.summaryDiv .timeLabel,\\n.summaryDiv .summaryFileName {\\n    order: 3;\\n    color: var(--log-color-text-weakest);\\n    margin-left: 0.5rem;\\n}\\n\\ndetails > summary:hover .timeLabel,\\ndetails > summary:hover .summaryFileName {\\n    color: var(--log-color-text-weaker);\\n}\\n\\ndetails > summary:hover .summaryInput:not(.emptySummaryInput) {\\n    color: var(--log-color-text) !important;\\n}\\n\\n/* ******************************* */\\n/* RESPONSIVE SIZING */\\n\\n@media only screen and (max-width: 840px) {\\n    .summaryDiv > .summaryInput,\\n    .detailContainer > .detailInputs,\\n    .headerInputs {\\n        display: none;\\n    }\\n}\\n\\n@media only screen and (max-width: 960px) {\\n    .headerInputs {\\n        width: var(--right-column-width-narrow) !important;\\n    }\\n\\n    .summaryDiv > .summaryInput,\\n    .detailContainer > .detailInputs {\\n        flex: 0 0 var(--right-column-width-narrow) !important;\\n    }\\n}\\n\\n/* ******************************* */\\n/* ERROR OUTPUT */\\n\\n.detailInfo {\\n    margin: 0.25rem 0;\\n    padding: 0.25rem 0;\\n    border-radius: 3px;\\n    font-size: 0.8rem;\\n}\\n\\n.errorHeader {\\n    font-weight: bold;\\n    margin-bottom: 0.35rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n\\n    /* forces wrapping */\\n    white-space: initial;\\n}\\n\\n.errorDetails {\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n\\n    /* forces wrapping */\\n    white-space: initial;\\n\\n    color: var(--log-color-text-weaker);\\n}\\n\\n/* ******************************* */\\n/* HEADERS */\\n\\n.headers {\\n    display: flex;\\n    border-bottom: 1px solid var(--log-color-border);\\n    padding-bottom: 1rem;\\n    margin-bottom: 1rem;\\n}\\n\\n.headerSource,\\n.headerInputs {\\n    font-weight: 600;\\n    text-transform: uppercase;\\n    font-size: 0.75rem;\\n    letter-spacing: 0.3px;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n.headerInputs {\\n    margin-left: auto;\\n    width: var(--right-column-width-wide);\\n    padding-left: 0.5rem;\\n}\\n\\n.headerRunDetails {\\n    margin: 0;\\n    margin-bottom: 1.5rem;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n/* ******************************* */\\n/* LABEL IS THE PASS/ERROR BADGE */\\n\\n.label {\\n    display: inline-block;\\n    margin-left: 0.5rem;\\n    color: white;\\n    font-weight: 600;\\n    font-size: 10px;\\n    border-radius: 2px;\\n    padding: 0 4px;\\n    height: 1rem;\\n    line-height: 1rem;\\n    letter-spacing: 0;\\n    display: none;\\n}\\n\\n.errorParent.leafNode .label.F,\\n.errorParent.leafNode .label.E,\\n.errorParent.leafNode .label.FAIL,\\n.errorParent.leafNode .label.ERROR {\\n    display: block;\\n    background-color: var(--log-color-error);\\n}\\n\\n/* hide labels when everything was successful */\\n/*\\n.label.PASS,\\n.label.I,\\n.label.INFO {\\n}\\n*/\\n.errorParent.leafNode .label.W,\\n.errorParent.leafNode .label.WARN {\\n    background-color: var(--log-color-warn);\\n}\\n\\n.label.NOT_RUN {\\n    background-color: var(--log-color-disabled);\\n}\\n\\n/* ******************************* */\\n/* HEADER TITLE ROW */\\n\\n.headerTitleSection {\\n    display: flex;\\n    align-items: center;\\n    margin-top: 0.3rem;\\n    margin-bottom: 0.5rem;\\n}\\n\\n.headerTitleSection h3 {\\n    margin: 0;\\n    padding: 0;\\n    font-size: 1.5rem;\\n}\\n\\n#suiteResult {\\n    font-size: 0.82rem;\\n    padding: 0.1rem 0.3rem 0.15rem 0.3rem;\\n    height: auto;\\n    margin-left: 0.75rem;\\n    display: inline-block;\\n}\\n.headerTitleSection .ERROR {\\n    background-color: var(--log-color-error);\\n}\\n.headerTitleSection .PASS {\\n    background-color: var(--log-color-success);\\n}\\n\',""]);const o=a},645:e=>{e.exports=function(e){var n=[];return n.toString=function(){return this.map((function(n){var t=e(n);return n[2]?"@media ".concat(n[2]," {").concat(t,"}"):t})).join("")},n.i=function(e,t,s){"string"==typeof e&&(e=[[null,e,""]]);var a={};if(s)for(var o=0;o<this.length;o++){var r=this[o][0];null!=r&&(a[r]=!0)}for(var i=0;i<e.length;i++){var l=[].concat(e[i]);s&&a[l[0]]||(t&&(l[2]?l[2]="".concat(t," and ").concat(l[2]):l[2]=t),n.push(l))}},n}},457:(e,n,t)=>{let s;window.setVSCodeAPI=function(e){s=e};let a={};function o(e){let n;try{n=s}catch(e){}n&&n.postMessage(e)}let r={output:void 0},i={setContents:void 0,appendContents:void 0,updateLabel:void 0};window.addEventListener("message",(e=>{let n=e.data;if(n)switch(n.type){case"response":let e=n,t=a[e.request_seq];t&&(delete a[e.request_seq],t(e));break;case"event":let s=r[n.event];s?s(n):console.log("Unhandled event: ",n);break;case"request":let o=i[n.command];o?o(n):console.log("Unhandled request: ",n)}}));let l=0;function d(){return l+=1,l}let c={filterLevel:"PASS",runIdToTreeState:{},runIdLRU:[]},u={initialContents:void 0,runId:void 0,state:void 0,onClickReference:void 0,appendedContents:[],allRunIdsToLabel:{},showTime:!0,showExpand:!0};function m(){return void 0===u.state&&(u.state=function(){let e;try{e=s}catch(e){}if(e){let n=e.getState();return n||(n=c),void 0===n.filterLevel&&(n.filterLevel="PASS"),void 0===n.runIdToTreeState&&(n.runIdToTreeState={}),void 0===!n.runIdLRU&&(n.runIdLRU=[]),n}return c}()),u}function h(e){return document.getElementById(e)}function p(e){return h(e)}function f(e){return h(e)}function g(e){const n=document.createElement("ul");return n.setAttribute("data-tree-id",e),n}function v(){return document.createElement("span")}function E(){return document.createElement("button")}function y(){return document.createElement("div")}function b(e){return e.getAttribute("data-tree-id")}function C(e,n=void 0){if(void 0===n)return"1"===e.getAttribute("data-hidden");n?e.setAttribute("data-hidden","1"):e.removeAttribute("data-hidden")}function w(e){var n=document.createElement("template");return e=e.trim(),n.innerHTML=e,n.content.firstChild}function S(e,n){for(let t of n.childNodes)if(t instanceof HTMLDetailsElement){for(let n of t.childNodes)n instanceof HTMLUListElement&&L(e,n);t.open?e.openNodes[b(n)]="open":delete e.openNodes[b(n)]}}function L(e,n){for(let t of n.childNodes)t instanceof HTMLLIElement&&S(e,t)}const x=((e,n)=>{let t;return function(...e){clearTimeout(t),t=setTimeout((()=>{clearTimeout(t),(()=>{T()})(...e)}),500)}})();function T(){const e=m();!function(e,n){const t=p("mainTree");let s={openNodes:{}};if(void 0===e.runIdLRU&&(e.runIdLRU=[]),void 0===e.runIdToTreeState)e.runIdToTreeState={};else{const t=e.runIdToTreeState[n];t&&(s=t)}for(let e of t.childNodes)e instanceof HTMLUListElement&&L(s,e);e.runIdToTreeState[n]=s;const a=e.runIdLRU.indexOf(n);for(a>-1&&e.runIdLRU.splice(a,1),e.runIdLRU.push(n);e.runIdLRU.length>15;){const n=e.runIdLRU.splice(0,1);delete e.runIdToTreeState[n[0]]}}(e.state,e.runId),function(e){let n;try{n=s}catch(e){}n?n.setState(e):c=e}(e.state)}function N(e,n){if(void 0===e)return;const t=f("selectedRun"),s=new Map;for(let a of t.childNodes)if(a instanceof HTMLOptionElement){const t=a,o=t.value,r=e[o];if(void 0===r)a.remove();else{t.text!==r&&(t.text=r),s.set(o,r);const e=n==o;t.selected=e}}for(const a of Object.keys(e)){if(void 0===a)continue;const o=n==a;if(!s.has(a)){const n=document.createElement("option"),r=e[a];n.value=a,t.appendChild(n),n.selected=o,n.text=r,s.set(a,r)}}}Math.pow(10,8);var I=36e5;function M(e,n){var t;!function(e,n){if(n.length<1)throw new TypeError("1 argument required, but only "+n.length+" present")}(0,arguments);var s=function(e){if(null===e||!0===e||!1===e)return NaN;var n=Number(e);return isNaN(n)?n:n<0?Math.ceil(n):Math.floor(n)}(null!==(t=null==n?void 0:n.additionalDigits)&&void 0!==t?t:2);if(2!==s&&1!==s&&0!==s)throw new RangeError("additionalDigits must be 0, 1 or 2");if("string"!=typeof e&&"[object String]"!==Object.prototype.toString.call(e))return new Date(NaN);var a,o=function(e){var n,t={},s=e.split(R.dateTimeDelimiter);if(s.length>2)return t;if(/:/.test(s[0])?n=s[0]:(t.date=s[0],n=s[1],R.timeZoneDelimiter.test(t.date)&&(t.date=e.split(R.timeZoneDelimiter)[0],n=e.substr(t.date.length,e.length))),n){var a=R.timezone.exec(n);a?(t.time=n.replace(a[1],""),t.timezone=a[1]):t.time=n}return t}(e);if(o.date){var r=function(e,n){var t=new RegExp("^(?:(\\\\d{4}|[+-]\\\\d{"+(4+n)+"})|(\\\\d{2}|[+-]\\\\d{"+(2+n)+"})$)"),s=e.match(t);if(!s)return{year:NaN,restDateString:""};var a=s[1]?parseInt(s[1]):null,o=s[2]?parseInt(s[2]):null;return{year:null===o?a:100*o,restDateString:e.slice((s[1]||s[2]).length)}}(o.date,s);a=function(e,n){if(null===n)return new Date(NaN);var t=e.match(k);if(!t)return new Date(NaN);var s=!!t[4],a=D(t[1]),o=D(t[2])-1,r=D(t[3]),i=D(t[4]),l=D(t[5])-1;if(s)return function(e,n,t){return n>=1&&n<=53&&t>=0&&t<=6}(0,i,l)?function(e,n,t){var s=new Date(0);s.setUTCFullYear(e,0,4);var a=7*(n-1)+t+1-(s.getUTCDay()||7);return s.setUTCDate(s.getUTCDate()+a),s}(n,i,l):new Date(NaN);var d=new Date(0);return function(e,n,t){return n>=0&&n<=11&&t>=1&&t<=(F[n]||(O(e)?29:28))}(n,o,r)&&function(e,n){return n>=1&&n<=(O(e)?366:365)}(n,a)?(d.setUTCFullYear(n,o,Math.max(a,r)),d):new Date(NaN)}(r.restDateString,r.year)}if(!a||isNaN(a.getTime()))return new Date(NaN);var i,l=a.getTime(),d=0;if(o.time&&(d=function(e){var n=e.match(_);if(!n)return NaN;var t=H(n[1]),s=H(n[2]),a=H(n[3]);return function(e,n,t){return 24===e?0===n&&0===t:t>=0&&t<60&&n>=0&&n<60&&e>=0&&e<25}(t,s,a)?t*I+6e4*s+1e3*a:NaN}(o.time),isNaN(d)))return new Date(NaN);if(!o.timezone){var c=new Date(l+d),u=new Date(0);return u.setFullYear(c.getUTCFullYear(),c.getUTCMonth(),c.getUTCDate()),u.setHours(c.getUTCHours(),c.getUTCMinutes(),c.getUTCSeconds(),c.getUTCMilliseconds()),u}return i=function(e){if("Z"===e)return 0;var n=e.match(A);if(!n)return 0;var t="+"===n[1]?-1:1,s=parseInt(n[2]),a=n[3]&&parseInt(n[3])||0;return function(e,n){return n>=0&&n<=59}(0,a)?t*(s*I+6e4*a):NaN}(o.timezone),isNaN(i)?new Date(NaN):new Date(l+d+i)}var R={dateTimeDelimiter:/[T ]/,timeZoneDelimiter:/[Z ]/i,timezone:/([Z+-].*)$/},k=/^-?(?:(\\d{3})|(\\d{2})(?:-?(\\d{2}))?|W(\\d{2})(?:-?(\\d{1}))?|)$/,_=/^(\\d{2}(?:[.,]\\d*)?)(?::?(\\d{2}(?:[.,]\\d*)?))?(?::?(\\d{2}(?:[.,]\\d*)?))?$/,A=/^([+-])(\\d{2})(?::?(\\d{2}))?$/;function D(e){return e?parseInt(e):1}function H(e){return e&&parseFloat(e.replace(",","."))||0}var F=[31,null,31,30,31,30,31,31,30,31,30,31];function O(e){return e%400==0||e%4==0&&e%100!=0}function P(e,n){const t=e.memo[n];return void 0===t?`<ref not found: ${n}>`:t}function U(e,n){return parseFloat(n)}function z(e,n){return parseInt(n)}function B(e,n){return n}function V(e){const n=[],t=new Map;for(let s of e.split(",")){s=s.trim();let e="oid";if(-1!=s.indexOf(":")&&([s,e]=s.split(":",2)),n.push(s),"oid"===e)t.set(s,P);else if("int"===e)t.set(s,z);else if("float"===e)t.set(s,U);else{if("str"!==e)throw new Error("Unexpected: "+e);t.set(s,B)}}return function(e,s){const a=s.split("|",n.length),o={};for(let s=0;s<a.length;s++){const r=a[s],i=n[s];o[i]=t.get(i)(e,r)}return o}}const j=V("part:int, id:str"),$={V:V("version:str"),ID:j,I:function(e,n){return JSON.parse(n)},T:function(e,n){return{time:M(n).toString()}},M:function(e,n){var t,s;const a=q(n,":");if(a){[t,s]=a;try{s=JSON.parse(s)}catch(e){return console.log("Error parsing json: "+s),console.log(e),null}e.memo[t]=s}return null},SR:V("name:oid, time_delta_in_seconds:float"),ER:V("status:oid, time_delta_in_seconds:float"),ST:V("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),ET:V("status:oid, message:oid, time_delta_in_seconds:float"),SE:V("name:oid, libname:oid, type:oid, doc:oid, source:oid, lineno:int, time_delta_in_seconds:float"),EE:V("type:oid, status:oid, time_delta_in_seconds:float"),EA:V("name:oid, type:oid, value:oid"),AS:V("source:oid, lineno:int, target:oid, type:oid, value:oid, time_delta_in_seconds:float"),L:V("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),LH:V("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),TG:V("tag:oid"),S:V("start_time_delta:float"),STB:V("message:oid, time_delta_in_seconds:float"),RTB:V("message:oid, time_delta_in_seconds:float"),TBE:V("source:oid, lineno:int, method:oid, line_content:oid"),TBV:V("name:oid, type:oid, value:oid"),ETB:V("time_delta_in_seconds:float"),YS:V("name:oid, libname:oid, source:oid, lineno:int, type:oid, value:oid, time_delta_in_seconds:float"),YR:V("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),YFS:V("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),YFR:V("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float")};$.RR=$.SR,$.RT=$.ST,$.RE=$.SE,$.RYR=$.YR;class Y{constructor(){this.memo={}}decode_message_type(e,n){return(0,$[e])(this,n)}}function q(e,n){const t=e.indexOf(n);if(t>0)return[e.substring(0,t),e.substring(t+1)]}function*W(e,n){var t,s,a;for(let o of e.split(/\\r?\\n/))if(o=o.trim(),o)try{const e=q(o," ");if(e&&([a,s]=e,t=n.decode_message_type(a,s))){const e={message_type:a,decoded:t};yield e}}catch(e){console.log("Unable to decode message: "+o),console.log(e)}}function Z(e,n){const t=document.createElement("span");t.textContent=n,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}function G(e,n){switch(e.state.filterLevel){case"FAIL":return n>=2;case"WARN":return n>=1;case"PASS":return n>=0;case"NOT RUN":return!0}}function J(e){switch(e){case"FAIL":case"ERROR":return 2;case"WARN":return 1;case"NOT RUN":case"NOT_RUN":return-1;default:return 0}}class K{constructor(e){this.stack=[],this.exceptionMsg=e}pushEntry(e,n,t,s){const a=new Map;this.stack.push({source:e,lineno:n,method:t,lineContent:s,variables:a})}pushVar(e,n,t){this.stack.at(-1).variables.set(e,[n,t])}}class Q{constructor(){this.totalTests=0,this.totalFailures=0}clear(){this.totalTests=0,this.totalFailures=0,this.updateSummary()}onTestEndUpdateSummary(e){const n=e.decoded.status;this.totalTests+=1,"FAIL"!=n&&"ERROR"!=n||(this.totalFailures+=1),this.updateSummary()}updateSummary(){const e=p("summary");if(!e)return;const n=(""+this.totalTests).padStart(4),t=(""+this.totalFailures).padStart(4);if(e.textContent=`Total: ${n} Failures: ${t}`,0==this.totalFailures&&0==this.totalTests){const e=p("summary");e.classList.add("NOT_RUN"),e.classList.remove("PASS"),e.classList.remove("FAIL")}else if(1==this.totalFailures){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("PASS"),e.classList.add("FAIL")}else if(0==this.totalFailures&&1==this.totalTests){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("FAIL")}}}function X(e,n){const t=function(e){const n=document.createElement("li");return n.setAttribute("data-tree-id",e),n}(n),s=document.createElement("details");e&&(s.open=e),s.classList.add("NO_CHILDREN"),t.appendChild(s);const a=y();a.classList.add("detailContainer"),s.appendChild(a);const o=document.createElement("summary"),r=y();r.classList.add("summaryDiv"),o.appendChild(r);const i=v();i.className="summaryName",i.textContent="[summaryName]",r.appendChild(i);const l=v();return l.className="summaryInput emptySummaryInput",l.textContent="",r.appendChild(l),s.appendChild(o),{li:t,details:s,summary:o,summaryDiv:r,summaryName:i,summaryInput:l,detailContainer:a}}function ee(e,n){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${n}`,e.summaryInput.classList.remove("emptySummaryInput")):e.summaryInput.textContent+=`, ${n}`}function ne(e,n,t,s,a,o,r,i,l,d){const c=e.state.runIdToTreeState[e.runId],u="li_"+d;if(c){const e=c.openNodes;e&&(o=e[u])}const m=X(o,u),h=m.li,p=m.details,f=m.detailContainer,v=m.summary,E=m.summaryDiv,y=m.summaryName,b=m.summaryInput;if("LH"===a.message_type){y.textContent="";const e=w(t);y.appendChild(e)}else y.textContent=t;s&&(y.title=s),e.onClickReference&&(y.classList.add("span_link"),y.onclick=n=>{const t=[];let s=l.parent;for(;void 0!==s&&void 0!==s.message;)t.push(s.message),s=s.parent;n.preventDefault(),e.onClickReference({source:r,lineno:i,message:a.decoded,messageType:a.message_type,scope:t})});const C=g("ul_"+d);p.appendChild(C);const S={ul:C,li:h,details:p,detailContainer:f,summary:v,summaryName:y,summaryInput:b,source:r,lineno:i,appendContentChild:void 0,decodedMessage:a,maxLevelFoundInHierarchy:-1,summaryDiv:E};return S.appendContentChild=re.bind(S),n.appendContentChild(S),S}let te,se;function*ae(e){for(let n of e.childNodes)if(n instanceof HTMLDetailsElement){for(let e of n.childNodes)if(e instanceof HTMLUListElement)for(let n of oe(e))yield n;yield n}}function*oe(e){for(let n of e.childNodes)if(n instanceof HTMLLIElement)for(let e of ae(n))yield e}function re(e){const n=this;n.ul.appendChild(e.li),n.details.classList.contains("NO_CHILDREN")&&(n.details.classList.remove("NO_CHILDREN"),n.details.addEventListener("toggle",(function(){x()})),m().showExpand&&n.summary.addEventListener("mouseover",(e=>{!function(e){if(void 0===te){te=y(),te.classList.add("toolbarContainer");const e=E();e.appendChild(w(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path d="M7 12V7H6v5h1z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),e.onclick=()=>{!function(){if(void 0!==se){se.details.open=!0;for(let e of oe(se.ul))e.classList.contains("NO_CHILDREN")||(e.open=!0)}}()},e.classList.add("toolbarButton");const n=E();return n.appendChild(w(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),n.classList.add("toolbarButton"),n.onclick=()=>{!function(){if(void 0!==se){se.details.open=!1;for(let e of oe(se.ul))e.open=!1}}()},te.appendChild(n),void te.appendChild(e)}se=e,e.summaryDiv.appendChild(te)}(n)})))}var ie=(e,n,t)=>new Promise(((s,a)=>{var o=e=>{try{i(t.next(e))}catch(e){a(e)}},r=e=>{try{i(t.throw(e))}catch(e){a(e)}},i=e=>e.done?s(e.value):Promise.resolve(e.value).then(o,r);i((t=t.apply(e,n)).next())}));let le=0,de=-1;class ce{constructor(){this.stack=[]}handle(e){let n;switch(e.message_type){case"STB":return void this.stack.push(new K(e.decoded.message));case"TBE":return n=this.stack.at(-1),void n.pushEntry(e.decoded.source,e.decoded.lineno,e.decoded.method,e.decoded.line_content);case"TBV":return;case"ETB":return n=this.stack.pop(),n.stack.reverse(),n}}}class ue{constructor(){this.stack=[],this.messageNode={parent:void 0,message:void 0},this.id=0,this.finishedAddingInitialContents=!1,this.appendedMessagesIndex=-1,this.decoder=new Y,this.seenSuiteTaskOrElement=!1,this.tbHandler=new ce,this.suiteErrored=!1,this.opts=m(),this.runId=this.opts.runId,this.summaryBuilder=new Q,this.lease=(le+=1,de=le,le),this.resetState()}resetState(){this.seenSuiteTaskOrElement=!1}isCurrentTreeBuilder(){return this.lease===de&&this.runId==this.opts.runId}clearAndInitializeTree(){this.summaryBuilder.clear(),this.resetState();const e=f("filterLevel");e&&(e.value=this.opts.state.filterLevel);const n=p("mainTree");n.replaceChildren();const t=g("ul_root");t.classList.add("tree"),n.appendChild(t),this.parent={ul:void 0,li:void 0,details:void 0,detailContainer:void 0,summary:void 0,summaryName:void 0,summaryInput:void 0,source:void 0,lineno:void 0,decodedMessage:void 0,appendContentChild:function(e){t.appendChild(e.li)},maxLevelFoundInHierarchy:-1,summaryDiv:void 0},this.stack.push(this.parent)}addInitialContents(){return ie(this,null,(function*(){for(const e of W(this.opts.initialContents,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}this.finishedAddingInitialContents=!0,yield this.onAppendedContents()}))}onAppendedContents(){return ie(this,null,(function*(){if(!this.finishedAddingInitialContents)return;if(!this.isCurrentTreeBuilder())return;const e=m();for(;this.appendedMessagesIndex+1<e.appendedContents.length;){this.appendedMessagesIndex+=1;const n=e.appendedContents[this.appendedMessagesIndex];for(const e of W(n,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}}}))}addOneMessage(e){return ie(this,null,(function*(){if(this.isCurrentTreeBuilder())try{this.addOneMessageSync(e)}catch(n){console.log("Error: handling message: "+JSON.stringify(e)+": "+n+" - "+JSON.stringify(n))}}))}addOneMessageSync(e){var n,t;let s,a,o=e.message_type;switch(o){case"SR":case"ST":case"SE":case"STB":this.seenSuiteTaskOrElement=!0;break;case"RR":if(this.seenSuiteTaskOrElement)return;o="SR";break;case"RT":if(this.seenSuiteTaskOrElement)return;o="ST";break;case"RE":if(this.seenSuiteTaskOrElement)return;o="SE";break;case"RTB":if(this.seenSuiteTaskOrElement)return;o="STB"}switch(this.id+=1,o){case"SR":this.messageNode={parent:this.messageNode,message:e};for(const n of document.querySelectorAll(".suiteHeader"))n.textContent=e.decoded.name;break;case"AS":a=ne(this.opts,this.parent,`${e.decoded.target} = `,`Assign to name: ${e.decoded.target}\\nAn object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),ee(a,e.decoded.value),this.addAssignCssClass(a);break;case"ST":this.messageNode={parent:this.messageNode,message:e},this.parent=ne(this.opts,this.parent,`${e.decoded.libname}.${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"SE":case"YR":case"YFR":if("SE"!=o||"UNTRACKED_GENERATOR"!=e.decoded.type){this.messageNode={parent:this.messageNode,message:e};let n=e.decoded.name;"YR"==o&&(n+=" (resumed)"),this.parent=ne(this.opts,this.parent,n,e.decoded.libname,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),"YR"==o&&this.addResumedCSSClass(this.parent),this.argsTarget=this.parent,this.stack.push(this.parent)}else{const n=ne(this.opts,this.parent,`Create Generator: ${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addGeneratorCSSClass(n),this.argsTarget=n}break;case"ER":this.messageNode=this.messageNode.parent;{const n=p("suiteResult");n.style.display="block",this.suiteErrored?(n.classList.add("ERROR"),n.textContent="Run Failed"):(n.classList.add("PASS"),n.textContent="Run Passed");const t=p("suiteRunStart");t&&(t.textContent+=` - Finished in: ${e.decoded.time_delta_in_seconds.toFixed(2)}s.`)}break;case"ET":this.messageNode=this.messageNode.parent;const r=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(r,this.parent,e),this.onEndSetStatusOrRemove(this.opts,r,e.decoded,this.parent,!1),this.summaryBuilder.onTestEndUpdateSummary(e),s=this.addDetailsCSSClasses(e.decoded.status,r),s&&(this.suiteErrored=!0,r.details.open=!0);break;case"EE":case"YS":case"YFS":if("EE"!=o||"UNTRACKED_GENERATOR"!=e.decoded.type){if("YS"==o||"YFS"==o){const n=ne(this.opts,this.parent,"Yielded",`Suspending function with yield.\\nYielding an object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addYieldedCSSClass(n),ee(n,e.decoded.value),e.decoded.status="PASS"}this.messageNode=this.messageNode.parent;let n=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(n,this.parent,e),this.onEndSetStatusOrRemove(this.opts,n,e.decoded,this.parent,!0),s=this.addDetailsCSSClasses(e.decoded.status,n),s&&(n.details.open=!0)}break;case"S":const i=e.decoded.start_time_delta;(null==(t=null==(n=this.parent)?void 0:n.decodedMessage)?void 0:t.decoded)&&(this.parent.decodedMessage.decoded.time_delta_in_seconds=i);break;case"EA":!function(e,n,t,s){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${n} = ${s}`,e.summaryInput.title=`Argument: ${n}\\nArgument type: ${t}\\nRepresentation:\\n${s}`,e.summaryInput.classList.remove("emptySummaryInput")):(e.summaryInput.title+=`\\n\\nArgument: ${n}\\nArgument type: ${t}\\nRepresentation:\\n${s}`,e.summaryInput.textContent+=`, ${n} = ${s}`)}(this.argsTarget,e.decoded.name,e.decoded.type,e.decoded.value);break;case"L":case"LH":const l=e.decoded.level,d=function(e){switch(e){case"E":case"F":return 2;case"W":return 1;default:return 0}}(l);if(d>this.parent.maxLevelFoundInHierarchy&&(this.parent.maxLevelFoundInHierarchy=d),G(this.opts,d)){const n=ne(this.opts,this.parent,e.decoded.message,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());n.maxLevelFoundInHierarchy=d,function(e,n){const t=document.createElement("span");t.textContent=`LOG ${function(e){switch(e){case"E":return"ERROR";case"F":return"FAIL";case"W":return"WARN";case"I":return"INFO";default:return e}}(n)}`,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}(n,l),this.addDetailsCSSClasses(d,n)}break;case"STB":case"TBE":case"TBV":case"ETB":const c=this.tbHandler.handle(e);if(c&&c.stack.length>0){const n=c.stack[0];a=ne(this.opts,this.parent,c.exceptionMsg,"",e,!1,n.source,n.lineno,this.messageNode,this.id.toString()),this.addExceptionCssClass(a)}break;case"T":const u=p("suiteRunStart");u&&(u.textContent=e.decoded.time)}}addAssignCssClass(e){e.details.classList.add("variableParent"),e.details.classList.add("leafNode")}addExceptionCssClass(e){e.details.classList.add("exceptionParent"),e.details.classList.add("leafNode")}addYieldedCSSClass(e){e.details.classList.add("yiededParent"),e.details.classList.add("leafNode")}addResumedCSSClass(e){e.details.classList.add("resumedParent")}addGeneratorCSSClass(e){e.details.classList.add("generatorParent"),e.details.classList.add("leafNode")}addDetailsCSSClasses(e,n){let t,s=!1;return t="string"==typeof e?J(e):e,t>=2?(n.details.classList.add("errorParent"),s=!0):1==t?n.details.classList.add("warnParent"):n.details.classList.add("passParent"),n.details.classList.contains("parentNode")||n.details.classList.contains("leafNode")||(0===n.ul.children.length?n.details.classList.add("leafNode"):n.details.classList.add("parentNode")),s}onEndUpdateMaxLevelFoundInHierarchyFromStatus(e,n,t){const s=J(t.decoded.status);s>e.maxLevelFoundInHierarchy&&(e.maxLevelFoundInHierarchy=s),e.maxLevelFoundInHierarchy>n.maxLevelFoundInHierarchy&&(n.maxLevelFoundInHierarchy=e.maxLevelFoundInHierarchy)}onEndSetStatusOrRemove(e,n,t,s,a){const o=t.status;if(G(e,n.maxLevelFoundInHierarchy)){if(a&&n.maxLevelFoundInHierarchy<=0){const e=50;if(s.ul.childElementCount>e){const e=n.summaryName.textContent;if(e&&e.toLowerCase().includes("iteration")){const e=n.li.previousSibling,t=b(n.li);if(n.li.remove(),C(e))e.getElementsByClassName("FINAL_SPAN")[0].textContent=n.summaryName.textContent;else{const e=X(!1,t);e.summaryName.textContent=n.summaryName.textContent,e.summary.classList.add("HIDDEN");const a=v();a.setAttribute("role","button"),a.textContent="...",a.classList.add("label"),a.classList.add("HIDDEN"),a.classList.add("inline"),e.summaryDiv.appendChild(a);const o=v();o.setAttribute("role","button"),o.classList.add("FINAL_SPAN"),e.summaryDiv.appendChild(o),Z(e,"HIDDEN"),C(e.li,!0),s.ul.appendChild(e.li)}return}}}if(n.summary,Z(n,o),null!=n.source&&n.source.length>0){const e=function(e){let n=e,t=Math.max(e.lastIndexOf("/"),e.lastIndexOf("\\\\"));return t>0&&(n=e.substring(t+1)),n}(n.source),t=document.createElement("span");t.textContent=e,t.classList.add("summaryFileName"),t.title=n.source,n.summaryDiv.appendChild(t)}if(this.opts.showTime){const e=n.decodedMessage.decoded.time_delta_in_seconds;void 0!==e&&e>=0&&function(e,n){const t=document.createElement("span");t.textContent=` (${n.toFixed(2)}s)`,t.classList.add("timeLabel"),e.summaryDiv.appendChild(t)}(n,t.time_delta_in_seconds-e)}}else n.li.remove()}}var me=(e,n,t)=>new Promise(((s,a)=>{var o=e=>{try{i(t.next(e))}catch(e){a(e)}},r=e=>{try{i(t.throw(e))}catch(e){a(e)}},i=e=>e.done?s(e.value):Promise.resolve(e.value).then(o,r);i((t=t.apply(e,n)).next())}));let he;function pe(){return me(this,null,(function*(){he=new ue,he.clearAndInitializeTree(),yield he.addInitialContents()}))}function fe(e){let n={type:"event",seq:d(),event:"onClickReference"};n.data=e,o(n)}function ge(e){T();const n=m();n.runId=e.runId,n.initialContents=e.initialContents,void 0!==s&&(n.onClickReference=fe),n.appendedContents=[],n.allRunIdsToLabel=e.allRunIdsToLabel,N(n.allRunIdsToLabel,n.runId),pe()}t(739),i.setContents=ge,i.appendContents=function(e){const n=m();n.runId===e.runId&&(n.appendedContents.push(e.appendContents),void 0!==he&&he.onAppendedContents())},i.updateLabel=function(e){const n=m();n.allRunIdsToLabel[e.runId]=e.label,N(n.allRunIdsToLabel,n.runId)},window.onChangedRun=function(){const e=f("selectedRun").value;let n={type:"event",seq:d(),event:"onSetCurrentRunId"};n.data={runId:e},o(n)},window.onChangedFilterLevel=function(){!function(e){const n=m();n.state.filterLevel!==e&&(n.state.filterLevel=e,T(),pe())}(f("filterLevel").value)},window.setContents=ge,window.setShowTime=function(e){m().showTime=e},window.setShowExpand=function(e){m().showExpand=e},window.getSampleContents=function(){return JSON.parse(\'"V 1\\\\nI \\\\"sys.platform=win32\\\\"\\\\nI \\\\"python=3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)]\\\\"\\\\nI \\\\"robot=5.1a3.dev1\\\\"\\\\nT 2022-10-19T09:48:34.018\\\\nM a:\\\\"Robot1\\\\"\\\\nM b:\\\\"s1\\\\"\\\\nM c:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\robot1.robot\\\\"\\\\nSR a|b|c|0.035\\\\nM d:\\\\"Simple Task\\\\"\\\\nM e:\\\\"s1-t1\\\\"\\\\nST d|e|16|0.036\\\\nM f:\\\\"First keyword\\\\"\\\\nM g:\\\\"\\\\"\\\\nM h:\\\\"KEYWORD\\\\"\\\\nSE f|g|h|g|c|17|0.036\\\\nM i:\\\\"No Operation\\\\"\\\\nM j:\\\\"BuiltIn\\\\"\\\\nM k:\\\\"Does absolutely nothing.\\\\"\\\\nSE i|j|h|k|c|8|0.037\\\\nM l:\\\\"PASS\\\\"\\\\nEE l|0.037\\\\nM m:\\\\"Log\\\\"\\\\nM n:\\\\"Logs the given message with the given level.\\\\"\\\\nSE m|j|h|n|c|10|0.037\\\\nM o:\\\\"Some warning message\\\\"\\\\nEA o\\\\nM p:\\\\"level=WARN\\\\"\\\\nEA p\\\\nEE l|0.046\\\\nM q:\\\\"Another keyword\\\\"\\\\nM r:\\\\"another\\\\"\\\\nSE q|r|h|g|c|11|0.047\\\\nM s:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\another.robot\\\\"\\\\nSE i|j|h|k|s|3|0.047\\\\nEE l|0.047\\\\nEE l|0.047\\\\nM t:\\\\"Another in sub keyword\\\\"\\\\nM u:\\\\"another_sub\\\\"\\\\nSE t|u|h|g|c|12|0.047\\\\nM v:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\sub\\\\\\\\\\\\\\\\another_sub.robot\\\\"\\\\nSE i|j|h|k|v|6|0.048\\\\nEE l|0.048\\\\nSE m|j|h|n|v|7|0.048\\\\nM w:\\\\"Some error message\\\\"\\\\nEA w\\\\nM x:\\\\"level=ERROR\\\\"\\\\nEA x\\\\nEE l|0.049\\\\nEE l|0.049\\\\nEE l|0.049\\\\nSE m|j|h|n|c|18|0.049\\\\nM y:\\\\"Some <data &encode <\\/script>\\\\"\\\\nEA y\\\\nEE l|0.049\\\\nM z:\\\\"Create Dictionary\\\\"\\\\nM A:\\\\"Creates and returns a dictionary based on the given ``items``.\\\\"\\\\nSE z|j|h|A|c|19|0.049\\\\nM B:\\\\"a=1\\\\"\\\\nEA B\\\\nM C:\\\\"b=1\\\\"\\\\nEA C\\\\nEE l|0.05\\\\nSE m|j|h|n|c|20|0.05\\\\nM D:\\\\"${dct}\\\\"\\\\nEA D\\\\nEE l|0.051\\\\nET l|g|0.051\\\\nM E:\\\\"Check 1\\\\"\\\\nM F:\\\\"s1-t2\\\\"\\\\nST E|F|22|0.051\\\\nSE f|g|h|g|c|23|0.051\\\\nSE i|j|h|k|c|8|0.052\\\\nEE l|0.052\\\\nSE m|j|h|n|c|10|0.052\\\\nEA o\\\\nEA p\\\\nEE l|0.052\\\\nSE q|r|h|g|c|11|0.053\\\\nSE i|j|h|k|s|3|0.053\\\\nEE l|0.053\\\\nEE l|0.053\\\\nSE t|u|h|g|c|12|0.053\\\\nSE i|j|h|k|v|6|0.054\\\\nEE l|0.054\\\\nSE m|j|h|n|v|7|0.054\\\\nEA w\\\\nEA x\\\\nEE l|0.054\\\\nEE l|0.055\\\\nEE l|0.055\\\\nM G:\\\\"${counter} IN RANGE [ 0 | 3 ]\\\\"\\\\nM H:\\\\"FOR\\\\"\\\\nSE G|g|H|g|c|25|0.055\\\\nM I:\\\\"${counter} = 0\\\\"\\\\nM J:\\\\"ITERATION\\\\"\\\\nSE I|g|J|g|c|25|0.055\\\\nM K:\\\\"${counter} == 2\\\\"\\\\nM L:\\\\"IF\\\\"\\\\nSE K|g|L|g|c|26|0.055\\\\nM M:\\\\"Fail\\\\"\\\\nM N:\\\\"Fails the test with the given message and optionally alters its tags.\\\\"\\\\nSE M|j|h|N|c|27|0.056\\\\nM O:\\\\"Failed execution for some reason...\\\\"\\\\nEA O\\\\nM P:\\\\"NOT RUN\\\\"\\\\nEE P|0.056\\\\nEE P|0.056\\\\nSE m|j|h|n|c|29|0.056\\\\nM Q:\\\\"${counter}\\\\"\\\\nEA Q\\\\nEE l|0.056\\\\nEE l|0.057\\\\nM R:\\\\"${counter} = 1\\\\"\\\\nSE R|g|J|g|c|25|0.057\\\\nSE K|g|L|g|c|26|0.057\\\\nSE M|j|h|N|c|27|0.057\\\\nEA O\\\\nEE P|0.057\\\\nEE P|0.057\\\\nSE m|j|h|n|c|29|0.058\\\\nEA Q\\\\nEE l|0.058\\\\nEE l|0.058\\\\nM S:\\\\"${counter} = 2\\\\"\\\\nSE S|g|J|g|c|25|0.058\\\\nSE K|g|L|g|c|26|0.058\\\\nSE M|j|h|N|c|27|0.059\\\\nEA O\\\\nM T:\\\\"FAIL\\\\"\\\\nEE T|0.059\\\\nEE T|0.059\\\\nSE m|j|h|n|c|29|0.059\\\\nEA Q\\\\nEE P|0.059\\\\nEE T|0.06\\\\nEE T|0.06\\\\nET T|O|0.06\\\\nM U:\\\\"Check 2\\\\"\\\\nM V:\\\\"s1-t3\\\\"\\\\nST U|V|32|0.06\\\\nM W:\\\\"Set Variable\\\\"\\\\nM X:\\\\"Returns the given values which can then be assigned to a variables.\\\\"\\\\nSE W|j|h|X|c|33|0.061\\\\nM Y:\\\\"3\\\\"\\\\nEA Y\\\\nEE l|0.061\\\\nM Z:\\\\"${counter} <= 2\\\\"\\\\nM 0:\\\\"WHILE\\\\"\\\\nSE Z|g|0|g|c|34|0.061\\\\nSE g|g|J|g|c|34|0.062\\\\nM 1:\\\\"Evaluate\\\\"\\\\nM 2:\\\\"Evaluates the given expression in Python and returns the result.\\\\"\\\\nSE 1|j|h|2|c|35|0.062\\\\nM 4:\\\\"$counter-1\\\\"\\\\nEA 4\\\\nEE P|0.062\\\\nSE m|j|h|n|c|36|0.062\\\\nM 5:\\\\"Current counter: ${counter}\\\\"\\\\nEA 5\\\\nEA p\\\\nEE P|0.062\\\\nEE P|0.062\\\\nEE P|0.063\\\\nET l|g|0.063\\\\nM 6:\\\\"Check 3\\\\"\\\\nM 7:\\\\"s1-t4\\\\"\\\\nST 6|7|39|0.064\\\\nM 8:\\\\"TRY\\\\"\\\\nSE g|g|8|g|c|40|0.064\\\\nSE i|j|h|k|c|41|0.064\\\\nEE l|0.064\\\\nEE l|0.064\\\\nM 9:\\\\"message\\\\"\\\\nM aa:\\\\"EXCEPT\\\\"\\\\nSE 9|g|aa|g|c|42|0.064\\\\nSE i|j|h|k|c|43|0.065\\\\nEE P|0.065\\\\nEE P|0.065\\\\nM ab:\\\\"FINALLY\\\\"\\\\nSE g|g|ab|g|c|44|0.065\\\\nSE i|j|h|k|c|45|0.065\\\\nEE l|0.065\\\\nEE l|0.065\\\\nET l|g|0.066\\\\nER T|0.067\\\\n"\')}},739:(e,n,t)=>{var s=t(379),a=t.n(s),o=t(599),r={injectType:"singletonStyleTag",insert:"head",singleton:!0};a()(o.Z,r),o.Z.locals},379:(e,n,t)=>{var s,a=function(){var e={};return function(n){if(void 0===e[n]){var t=document.querySelector(n);if(window.HTMLIFrameElement&&t instanceof window.HTMLIFrameElement)try{t=t.contentDocument.head}catch(e){t=null}e[n]=t}return e[n]}}(),o=[];function r(e){for(var n=-1,t=0;t<o.length;t++)if(o[t].identifier===e){n=t;break}return n}function i(e,n){for(var t={},s=[],a=0;a<e.length;a++){var i=e[a],l=n.base?i[0]+n.base:i[0],d=t[l]||0,c="".concat(l," ").concat(d);t[l]=d+1;var u=r(c),m={css:i[1],media:i[2],sourceMap:i[3]};-1!==u?(o[u].references++,o[u].updater(m)):o.push({identifier:c,updater:f(m,n),references:1}),s.push(c)}return s}function l(e){var n=document.createElement("style"),s=e.attributes||{};if(void 0===s.nonce){var o=t.nc;o&&(s.nonce=o)}if(Object.keys(s).forEach((function(e){n.setAttribute(e,s[e])})),"function"==typeof e.insert)e.insert(n);else{var r=a(e.insert||"head");if(!r)throw new Error("Couldn\'t find a style target. This probably means that the value for the \'insert\' parameter is invalid.");r.appendChild(n)}return n}var d,c=(d=[],function(e,n){return d[e]=n,d.filter(Boolean).join("\\n")});function u(e,n,t,s){var a=t?"":s.media?"@media ".concat(s.media," {").concat(s.css,"}"):s.css;if(e.styleSheet)e.styleSheet.cssText=c(n,a);else{var o=document.createTextNode(a),r=e.childNodes;r[n]&&e.removeChild(r[n]),r.length?e.insertBefore(o,r[n]):e.appendChild(o)}}function m(e,n,t){var s=t.css,a=t.media,o=t.sourceMap;if(a?e.setAttribute("media",a):e.removeAttribute("media"),o&&"undefined"!=typeof btoa&&(s+="\\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o))))," */")),e.styleSheet)e.styleSheet.cssText=s;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(s))}}var h=null,p=0;function f(e,n){var t,s,a;if(n.singleton){var o=p++;t=h||(h=l(n)),s=u.bind(null,t,o,!1),a=u.bind(null,t,o,!0)}else t=l(n),s=m.bind(null,t,n),a=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(t)};return s(e),function(n){if(n){if(n.css===e.css&&n.media===e.media&&n.sourceMap===e.sourceMap)return;s(e=n)}else a()}}e.exports=function(e,n){(n=n||{}).singleton||"boolean"==typeof n.singleton||(n.singleton=(void 0===s&&(s=Boolean(window&&document&&document.all&&!window.atob)),s));var t=i(e=e||[],n);return function(e){if(e=e||[],"[object Array]"===Object.prototype.toString.call(e)){for(var s=0;s<t.length;s++){var a=r(t[s]);o[a].references--}for(var l=i(e,n),d=0;d<t.length;d++){var c=r(t[d]);0===o[c].references&&(o[c].updater(),o.splice(c,1))}t=l}}}}},n={};function t(s){var a=n[s];if(void 0!==a)return a.exports;var o=n[s]={id:s,exports:{}};return e[s](o,o.exports,t),o.exports}t.n=e=>{var n=e&&e.__esModule?()=>e.default:()=>e;return t.d(n,{a:n}),n},t.d=(e,n)=>{for(var s in n)t.o(n,s)&&!t.o(e,s)&&Object.defineProperty(e,s,{enumerable:!0,get:n[s]})},t.o=(e,n)=>Object.prototype.hasOwnProperty.call(e,n),t.nc=void 0,t(457),t(739)})();</script></body><script>window.setShowTime(true);\n    window.setShowExpand(false);\n    try {\n        const vscode = acquireVsCodeApi();\n        window.setVSCodeAPI(vscode);\n        document.getElementById("selectRunContainer").style.display = "block";\n    } catch (err) {\n        // That\'s ok (not running in VSCode).\n        window.setContents({\n            "initialContents": window.getSampleContents(),\n        });\n    }</script></html>'}
```

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_lifecycle_hooks.py` & `robocorp_log-0.0.13/src/robocorp/log/_lifecycle_hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,14 +63,20 @@
 
 # Called as: before_yield(__name__, filename, name, lineno, yielded_value)
 before_yield = Callback()
 
 # Called as: after_yield(__name__, filename, name, lineno)
 after_yield = Callback()
 
+# Called as: before_yield_from(__name__, filename, name, lineno)
+before_yield_from = Callback()
+
+# Called as: after_yield_from(__name__, filename, name, lineno)
+after_yield_from = Callback()
+
 
 def iter_all_callbacks() -> Iterator[Callback]:
     for _key, val in globals().items():
         if isinstance(val, Callback):
             yield val
```

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_null.py` & `robocorp_log-0.0.13/src/robocorp/log/_null.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_rewrite_ast_add_callbacks.py` & `robocorp_log-0.0.13/src/robocorp/log/_rewrite_ast_add_callbacks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,22 @@
 import ast
-from typing import Any, Union, List, Optional, Tuple, Dict, Callable, Sequence, Iterator
-import typing
+from typing import Any, Union, List, Optional, Tuple, Dict, Callable
 from . import _ast_utils
 from ._config import BaseConfig, FilterKind
 from .protocols import LogElementType
+from ._ast_utils import ASTRewriter
+from robocorp.log._ast_utils import NodeFactory
 
 DEBUG = False
 
 
 def is_rewrite_disabled(docstring: str) -> bool:
     return "NO_LOG" in docstring
 
 
-class _RewriteCtx:
-    def __init__(self):
-        self._memo = {}
-
-    def save_func_to_before_method_call(
-        self, function: ast.FunctionDef, call: ast.Call
-    ):
-        self._memo.setdefault(function, []).append(call)
-
-    def save_func_to_except_method_call(self, function, call):
-        self._memo.setdefault(function, []).append(call)
-
-    def save_func_to_after_method_call(self, function, call):
-        self._memo.setdefault(function, []).append(call)
-
-    def iter_func_calls_from_func(self, func: ast.FunctionDef) -> Iterator[ast.Call]:
-        yield from iter(self._memo[func])
-
-
 def _make_import_aliases_ast(lineno, filter_kind: FilterKind):
     aliases = [
         ast.alias(
             "robocorp.log._lifecycle_hooks",
             "@robo_lifecycle_hooks",
             lineno=lineno,
             col_offset=0,
@@ -76,16 +58,15 @@
     if function.name.startswith("_"):
         return None
 
     factory = _ast_utils.NodeFactory(node.lineno, node.col_offset)
 
     result: List[ast.stmt] = []
 
-    call = factory.Call()
-    call.func = factory.NameLoadRewriteCallback("method_return")
+    call = factory.Call(factory.NameLoadRewriteCallback("method_return"))
     call.args.append(factory.NameLoad("__name__"))
     call.args.append(factory.NameLoad("__file__"))
     call.args.append(factory.Str(f"{class_name}{function.name}"))
     call.args.append(factory.LineConstant())
 
     if node.value:
         assign = factory.Assign()
@@ -101,140 +82,82 @@
         call.args.append(factory.NoneConstant())
 
     result.append(factory.Expr(call))
     result.append(node)
     return result
 
 
-def _rewrite_assign(function, class_name, node: ast.Assign) -> Optional[list]:
-    factory = _ast_utils.NodeFactory(node.lineno, node.col_offset)
-
-    result: List[ast.stmt] = []
-
-    if isinstance(node.value, ast.Yield):
-        result.extend(_make_before_yield_exprs(factory, function, class_name, node))
-
-    result.append(node)
-
-    if isinstance(node.value, ast.Yield):
-        result.append(_make_after_yield_expr(factory, function, class_name))
-
-    for target in node.targets:
-        if isinstance(target, ast.Name):
-            call = _make_func_with_args(
-                factory,
-                "after_assign",
-                factory.NameLoad("__name__"),
-                factory.NameLoad("__file__"),
-                factory.Str(f"{class_name}{function.name}"),
-                factory.LineConstant(),
-                factory.Str(target.id),
-                factory.NameLoad(target.id),
-            )
-
-            result.append(factory.Expr(call))
-
-    return result
-
-
 def _make_func_with_args(factory, func_name, *args):
-    call = factory.Call()
-    call.func = factory.NameLoadRewriteCallback(func_name)
+    call = factory.Call(factory.NameLoadRewriteCallback(func_name))
     call.args.extend(args)
     return call
 
 
-class INodeWithValueExpr(typing.Protocol):
-    value: ast.expr
-
-
-def _make_before_yield_exprs(
-    factory, function, class_name, node_with_yield_val: INodeWithValueExpr
-) -> Sequence[ast.Expr]:
-    assert isinstance(node_with_yield_val.value, ast.Yield)
-    yield_expr: ast.Yield = node_with_yield_val.value
-
-    result = []
-    if yield_expr.value is not None:
-        assign = factory.Assign()
-        store_name = factory.NameTempStore()
-        assign.targets = [store_name]
-        assign.value = yield_expr.value
-
-        yield_expr.value = factory.NameLoad(store_name.id)
-
-        value_yielded = factory.NameLoad(store_name.id)
-        result.append(assign)
-    else:
-        value_yielded = factory.NoneConstant()
-
-    result.append(
-        factory.Expr(
-            _make_func_with_args(
-                factory,
-                "before_yield",
-                factory.NameLoad("__name__"),
-                factory.NameLoad("__file__"),
-                factory.Str(f"{class_name}{function.name}"),
-                factory.LineConstant(),
-                value_yielded,
-            )
+def _make_after_yield_expr(factory, function, class_name) -> ast.Expr:
+    return factory.Expr(
+        _make_func_with_args(
+            factory,
+            "after_yield",
+            factory.NameLoad("__name__"),
+            factory.NameLoad("__file__"),
+            factory.Str(f"{class_name}{function.name}"),
+            factory.LineConstant(),
         )
     )
-    return result
 
 
-def _make_after_yield_expr(factory, function, class_name):
+def _make_before_yield_from_exprs(factory, function, class_name) -> ast.Expr:
     return factory.Expr(
         _make_func_with_args(
             factory,
-            "after_yield",
+            "before_yield_from",
             factory.NameLoad("__name__"),
             factory.NameLoad("__file__"),
             factory.Str(f"{class_name}{function.name}"),
             factory.LineConstant(),
         )
     )
 
 
-def _rewrite_yield(function, class_name, node: ast.Expr) -> Optional[list]:
-    factory = _ast_utils.NodeFactory(node.lineno, node.col_offset)
-
-    result: List[ast.stmt] = []
-    result.extend(_make_before_yield_exprs(factory, function, class_name, node))
-    result.append(node)
-    result.append(_make_after_yield_expr(factory, function, class_name))
-    return result
+def _make_after_yield_from_expr(factory, function, class_name) -> ast.Expr:
+    return factory.Expr(
+        _make_func_with_args(
+            factory,
+            "after_yield_from",
+            factory.NameLoad("__name__"),
+            factory.NameLoad("__file__"),
+            factory.Str(f"{class_name}{function.name}"),
+            factory.LineConstant(),
+        )
+    )
 
 
 _EMPTY_LIST: list = []
 
 
 def _create_before_method_ast(
-    rewrite_ctx: _RewriteCtx, factory, class_name, function, filter_kind
+    rewrite_ctx: ASTRewriter, factory, class_name, function, filter_kind
 ) -> list:
     # Target code:
     # def method(a, b):
     #     before_method(__name, __file__, "method_name", 11, {'a': a, 'b': b})
     stmts: list = []
 
     if filter_kind == FilterKind.log_on_project_call:
         # In this case we need to create a local variable signaling whether
         # the caller is in the project (as if it's not we won't log the calls).
-        call = factory.Call()
-        call.func = factory.NameLoadRobo("_caller_in_project_roots")
+        call = factory.Call(factory.NameLoadRobo("_caller_in_project_roots"))
 
         assign = factory.Assign()
         caller_in_proj_name = factory.NameStore("@caller_in_proj")
         assign.targets = [caller_in_proj_name]
         assign.value = call
         stmts.append(assign)
 
-    call = factory.Call()
-    call.func = factory.NameLoadRewriteCallback("before_method")
+    call = factory.Call(factory.NameLoadRewriteCallback("before_method"))
     log_method_type: LogElementType = "METHOD"
     call.args.append(factory.Str(log_method_type))
     call.args.append(factory.NameLoad("__name__"))
     call.args.append(factory.NameLoad("__file__"))
     call.args.append(factory.Str(f"{class_name}{function.name}"))
     call.args.append(factory.LineConstant())
 
@@ -264,15 +187,15 @@
         stmts.append(factory.AndExpr(factory.NameLoad("@caller_in_proj"), call))
     else:
         stmts.append(factory.Expr(call))
     return stmts
 
 
 def _create_except_handler_ast(
-    rewrite_ctx: _RewriteCtx,
+    rewrite_ctx: ASTRewriter,
     factory,
     class_name: str,
     function: ast.FunctionDef,
     last_body_lineno,
     filter_kind: FilterKind,
 ) -> ast.ExceptHandler:
     # Target code:
@@ -306,21 +229,19 @@
         if_stmt = factory.If(factory.NameLoad("@caller_in_proj"))
         add_to_body = if_stmt.body = []
         if_stmt.orelse = []
         except_handler.body.append(if_stmt)
     else:
         add_to_body = except_handler.body
 
-    exc_info_attr = factory.Attribute(factory.NameLoad("@py_sys"), "exc_info")
-    call_exc_info = factory.Call()
-    call_exc_info.func = exc_info_attr
-
-    method_except = factory.NameLoadRewriteCallback("method_except")
-    call_method_except = factory.Call()
-    call_method_except.func = method_except
+    call_exc_info = factory.Call(
+        factory.Attribute(factory.NameLoad("@py_sys"), "exc_info")
+    )
+
+    call_method_except = factory.Call(factory.NameLoadRewriteCallback("method_except"))
     log_method_type: LogElementType = "METHOD"
     call_method_except.args.append(factory.Str(log_method_type))
     call_method_except.args.append(factory.NameLoad("__name__"))
     call_method_except.args.append(factory.NameLoad("__file__"))
     call_method_except.args.append(factory.Str(f"{class_name}{function.name}"))
     call_method_except.args.append(factory.LineConstant())
     call_method_except.args.append(call_exc_info)
@@ -330,18 +251,17 @@
     add_to_body.append(factory.Expr(call_method_except))
 
     except_handler.body.append(factory.Raise())
     return except_handler
 
 
 def _create_after_method_ast(
-    rewrite_ctx: _RewriteCtx, factory, class_name, function, filter_kind
+    rewrite_ctx: ASTRewriter, factory: NodeFactory, class_name, function, filter_kind
 ) -> ast.Expr:
-    call = factory.Call()
-    call.func = factory.NameLoadRewriteCallback("after_method")
+    call = factory.Call(factory.NameLoadRewriteCallback("after_method"))
     log_method_type: LogElementType = "METHOD"
     call.args.append(factory.Str(log_method_type))
     call.args.append(factory.NameLoad("__name__"))
     call.args.append(factory.NameLoad("__file__"))
     call.args.append(factory.Str(f"{class_name}{function.name}"))
     call.args.append(factory.LineConstant())
 
@@ -359,15 +279,15 @@
 
     if not function.body:
         return False
     return True
 
 
 def _rewrite_funcdef(
-    rewrite_ctx: _RewriteCtx, stack, function: ast.FunctionDef, filter_kind
+    rewrite_ctx: ASTRewriter, stack, function: ast.FunctionDef, filter_kind
 ) -> None:
     parent: Any
     # Only rewrite functions which actually have some content.
 
     class_name = ""
     if stack:
         parent = stack[-1]
@@ -482,53 +402,48 @@
         lineno = item.decorator_list[0].lineno
     else:
         lineno = item.lineno
     # Now actually insert the special imports.
     imports = _make_import_aliases_ast(lineno, filter_kind)
     mod.body[pos:pos] = imports
 
-    it: Any = _ast_utils.iter_and_replace_nodes(mod)
-    node: Any
+    rewrite_ctx = ASTRewriter(mod)
 
-    rewrite_ctx = _RewriteCtx()
-    while True:
-        try:
-            stack, node = next(it)
-        except StopIteration:
-            break
+    node: ast.AST
 
+    for stack, node in rewrite_ctx.iter_and_replace_nodes():
         handler = _dispatch.get(node.__class__)
         if handler:
             result = handler(rewrite_ctx, config, module_path, stack, filter_kind, node)
             if result is not None:
-                it.send(result)
+                rewrite_ctx.cursor.current = result
 
     if DEBUG:
         print("\n============ New AST (with hooks in place) ==============\n")
         # Note: only python 3.9 onwards.
         print(ast.unparse(mod))  # type: ignore
 
 
 def _handle_funcdef(
-    rewrite_ctx: _RewriteCtx, config, module_path, stack, filter_kind, node
+    rewrite_ctx: ASTRewriter, config, module_path, stack, filter_kind, node
 ):
     try:
         function: ast.FunctionDef = node
         if not _accept_function_rewrite(function):
             return
 
         _rewrite_funcdef(rewrite_ctx, stack, node, filter_kind)
     except Exception:
         raise RuntimeError(
             f"Error when rewriting function: {node.name} line: {node.lineno} at: {module_path}"
         )
 
 
 def _handle_return(
-    rewrite_ctx: _RewriteCtx, config, module_path, stack, filter_kind, node
+    rewrite_ctx: ASTRewriter, config, module_path, stack, filter_kind, node
 ):
     func_and_class_name = _get_function_and_class_name(stack)
     if not func_and_class_name:
         return None
 
     function, class_name = func_and_class_name
     if not _accept_function_rewrite(function):
@@ -539,74 +454,162 @@
     except Exception:
         raise RuntimeError(
             f"Error when rewriting function return: {function.name} line: {node.lineno} at: {module_path}"
         )
 
 
 def _handle_assign(
-    rewrite_ctx: _RewriteCtx, config: BaseConfig, module_path, stack, filter_kind, node
+    rewrite_ctx: ASTRewriter, config: BaseConfig, module_path, stack, filter_kind, node
 ):
     if filter_kind != FilterKind.full_log or not config.get_rewrite_assigns():
         return None
 
     func_and_class_name = _get_function_and_class_name(stack)
     if not func_and_class_name:
         return None
 
     function, class_name = func_and_class_name
     if not _accept_function_rewrite(function):
         return
 
     try:
-        return _rewrite_assign(function, class_name, node)
+        factory = _ast_utils.NodeFactory(node.lineno, node.col_offset)
+        for target in node.targets:
+            if isinstance(target, ast.Name):
+                call = _make_func_with_args(
+                    factory,
+                    "after_assign",
+                    factory.NameLoad("__name__"),
+                    factory.NameLoad("__file__"),
+                    factory.Str(f"{class_name}{function.name}"),
+                    factory.LineConstant(),
+                    factory.Str(target.id),
+                    factory.NameLoad(target.id),
+                )
+
+                rewrite_ctx.stmts_cursor.after_append(factory.Expr(call))
     except Exception:
         raise RuntimeError(
             f"Error when rewriting assign: {function.name} line: {node.lineno} at: {module_path}"
         )
 
 
-def _handle_expr(
-    rewrite_ctx: _RewriteCtx, config, module_path, stack, filter_kind, node: ast.Expr
+def _update_calls_from_func_to_generator(
+    rewrite_ctx: ASTRewriter, function, filter_kind: FilterKind
 ):
-    if isinstance(node.value, ast.Yield):
-        func_and_class_name = _get_function_and_class_name(stack)
-        if not func_and_class_name:
+    before_call: ast.Call
+    for before_call in rewrite_ctx.iter_func_calls_from_func(function):
+        assert isinstance(before_call.args[0], ast.Str)
+        before_call_method_type: ast.Str = before_call.args[0]
+
+        log_method_type: LogElementType = "GENERATOR"
+        if filter_kind == FilterKind.log_on_project_call:
+            log_method_type = "UNTRACKED_GENERATOR"
+        before_call_method_type.s = log_method_type
+
+
+def _handle_yield(
+    rewrite_ctx: ASTRewriter,
+    config,
+    module_path,
+    stack,
+    filter_kind,
+    node: Union[ast.Yield, ast.YieldFrom],
+):
+    func_and_class_name = _get_function_and_class_name(stack)
+    if not func_and_class_name:
+        return None
+
+    function, class_name = func_and_class_name
+    if not _accept_function_rewrite(function):
+        return None
+
+    try:
+        _update_calls_from_func_to_generator(rewrite_ctx, function, filter_kind)
+
+        if filter_kind != FilterKind.full_log:
             return None
 
-        function, class_name = func_and_class_name
-        if not _accept_function_rewrite(function):
-            return
+        # Wrapping of before/after for yield statements.
+        factory = _ast_utils.NodeFactory(node.lineno, node.col_offset)
+        stmts_cursor = rewrite_ctx.stmts_cursor
+        yield_cursor = rewrite_ctx.cursor
+
+        if isinstance(node, ast.Yield):
+            value_yielded: ast.AST
+            if isinstance(yield_cursor.parent, ast.stmt):
+                # We can only rewrite in the simple case where we have something
+                # as:
+                # yield 2
+                #
+                # or
+                #
+                # a = yield call()
+                #
+                # Because we can't risk rewriting something as:
+                #
+                # a = call1() and (yield call2())
+                #
+                # as it'd change the order of the calls
+                #
+                # If the assumption above is correct than we can do something as:
+                #
+                # @tmp = call()
+                # before_yield(..., @tmp)
+                # yield @tmp
+                #
+                # and properly report the yield value.
+
+                if node.value is not None:
+                    assign = factory.Assign()
+                    store_name = factory.NameTempStore()
+                    assign.targets = [store_name]
+                    assign.value = node.value
+
+                    node.value = factory.NameLoad(store_name.id)
+
+                    value_yielded = factory.NameLoad(store_name.id)
+                    stmts_cursor.before_append(assign)
+                else:
+                    value_yielded = factory.NoneConstant()
+            else:
+                value_yielded = factory.NoneConstant()
+
+            stmts_cursor.before_append(
+                factory.Expr(
+                    _make_func_with_args(
+                        factory,
+                        "before_yield",
+                        factory.NameLoad("__name__"),
+                        factory.NameLoad("__file__"),
+                        factory.Str(f"{class_name}{function.name}"),
+                        factory.LineConstant(),
+                        value_yielded,
+                    )
+                )
+            )
 
-        try:
-            before_call: ast.Call
-            for before_call in rewrite_ctx.iter_func_calls_from_func(function):
-                assert isinstance(before_call.args[0], ast.Str)
-                before_call_method_type: ast.Str = before_call.args[0]
-
-                log_method_type: LogElementType = "GENERATOR"
-                if filter_kind == FilterKind.log_on_project_call:
-                    log_method_type = "UNTRACKED_GENERATOR"
-                before_call_method_type.s = log_method_type
-
-            if filter_kind != FilterKind.full_log:
-                return None
-
-            return _rewrite_yield(function, class_name, node)
-        except Exception:
-            raise RuntimeError(
-                f"Error when rewriting assign: {function.name} line: {node.lineno} at: {module_path}"
+            stmts_cursor.after_prepend(
+                _make_after_yield_expr(factory, function, class_name)
+            )
+        else:
+            stmts_cursor.before_append(
+                _make_before_yield_from_exprs(factory, function, class_name)
+            )
+            stmts_cursor.after_prepend(
+                _make_after_yield_from_expr(factory, function, class_name)
             )
+    except Exception:
+        raise RuntimeError(
+            f"Error when rewriting assign: {function.name} line: {node.lineno} at: {module_path}"
+        )
 
 
 _dispatch: Dict[
     type,
-    Callable[[_RewriteCtx, BaseConfig, str, list, FilterKind, Any], Optional[list]],
+    Callable[[ASTRewriter, BaseConfig, str, list, FilterKind, Any], Optional[list]],
 ] = {}
 _dispatch[ast.Return] = _handle_return
 _dispatch[ast.Assign] = _handle_assign
 _dispatch[ast.FunctionDef] = _handle_funcdef
-
-# We can't deal with the Yield directly because it's a field of the Expr statement
-# and we can't rewrite a field (so, we have to go to the stmt level to be able to
-# rewrite it and then check if it's some expr we want to deal with -- and we also
-# need to check whether a yield appears in an assign).
-_dispatch[ast.Expr] = _handle_expr
+_dispatch[ast.Yield] = _handle_yield
+_dispatch[ast.YieldFrom] = _handle_yield
```

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_rewrite_filtering.py` & `robocorp_log-0.0.13/src/robocorp/log/_rewrite_filtering.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_rewrite_importhook.py` & `robocorp_log-0.0.13/src/robocorp/log/_rewrite_importhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 # 0.0.6: Option to log just 1 level deep into library modules.
 # 0.0.7: Just include __name__, note __package__.
 # 0.0.9: Rewrite assign statements
 # 0.0.10: Rewrite yields
 # 0.0.11: Add method type as first parameter for start_method/except/end_method
 # 0.0.12: Changed to use robocorp namespace.
 # 0.0.13: Changed to use robocorp.log name.
-version = "0.0.13"
+# 0.0.14: Rewrite yield from
+version = "0.0.14"
 NAME_WITH_TAG = f"{sys.implementation.cache_tag}-log-{version}"
 PYC_EXT = ".py" + (__debug__ and "c" or "o")
 PYC_TAIL = "." + NAME_WITH_TAG + PYC_EXT
 
 FORCE_CODE_GENERATION = False
 DEBUG = False
 
@@ -255,14 +256,17 @@
     from ._rewrite_ast_add_callbacks import rewrite_ast_add_callbacks
 
     stat = os.stat(fn)
     source = fn.read_bytes()
     strfn = str(fn)
     tree = ast.parse(source, filename=strfn)
     rewrite_ast_add_callbacks(tree, filter_kind, source, strfn, config)
+    if DEBUG:
+        print(f"Changed {strfn} to:")
+        print(ast.unparse(tree))
     co = compile(tree, strfn, "exec", dont_inherit=True)
     return stat, co, tree
 
 
 def _read_pyc(
     source: Path, pyc: Path, trace: Callable[[str], None] = lambda x: None
 ) -> Optional[types.CodeType]:
```

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_robo_logger.py` & `robocorp_log-0.0.13/src/robocorp/log/_robo_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -250,14 +250,47 @@
             source,
             lineno,
             yielded_value_type,
             yielded_value_repr,
             self._get_time_delta(),
         )
 
+    def yield_from_resume(
+        self,
+        name: str,
+        libname: str,
+        source: str,
+        lineno: int,
+    ):
+        hide_from_logs = bool(self._skip_log_methods)
+
+        return self._robot_output_impl.yield_from_resume(
+            name,
+            libname,
+            source,
+            lineno,
+            self._get_time_delta(),
+            hide_from_logs,
+        )
+
+    def yield_from_suspend(
+        self,
+        name: str,
+        libname: str,
+        source: str,
+        lineno: int,
+    ):
+        return self._robot_output_impl.yield_from_suspend(
+            name,
+            libname,
+            source,
+            lineno,
+            self._get_time_delta(),
+        )
+
     @_log_error
     def after_assign(
         self,
         filename: str,
         lineno: int,
         assign_name: str,
         assign_type: str,
```

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_robo_output_impl.py` & `robocorp_log-0.0.13/src/robocorp/log/_robo_output_impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -563,47 +563,14 @@
         stack_entry = self._stack_handler.pop("traceback", entry_id)
         assert stack_entry
 
         self._write_with_separator("ETB ", [self._number(self.get_time_delta())])
 
         return True
 
-    def yield_resume(
-        self,
-        name: str,
-        libname: str,
-        source: str,
-        lineno: int,
-        time_delta: float,
-        hide_from_logs: bool,
-    ):
-        """
-        Note that a yield resume is semantically very close to a start element
-        but it doesn't have any arguments.
-        """
-        oid = self._obtain_id
-        element_id = f"{libname}.{name}"
-        with self._stack_handler.push_record(
-            "element", element_id, "YR", "RYR", hide_from_logs
-        ):
-            if hide_from_logs:
-                # I.e.: add to internal stack but don't write it.
-                return
-
-            self._write_with_separator(
-                "YR ",
-                [
-                    oid(name),
-                    oid(libname),
-                    oid(source),
-                    self._number(lineno),
-                    self._number(time_delta),
-                ],
-            )
-
     def start_element(
         self,
         name: str,
         libname: str,
         element_type: LogElementType,
         doc: str,
         source: str,
@@ -713,22 +680,124 @@
         hide_strings_re = self._hide_strings_re
         if hide_strings_re:
             yielded_value_repr = hide_strings_re.sub("<redacted>", yielded_value_repr)
 
         self._write_with_separator(
             "YS ",
             [
+                oid(name),
+                oid(libname),
                 oid(source),
                 self._number(lineno),
                 oid(yielded_value_type),
                 oid(yielded_value_repr),
                 self._number(time_delta),
             ],
         )
 
+    def yield_resume(
+        self,
+        name: str,
+        libname: str,
+        source: str,
+        lineno: int,
+        time_delta: float,
+        hide_from_logs: bool,
+    ):
+        """
+        Note that a yield resume is semantically very close to a start element
+        but it doesn't have any arguments.
+        """
+        oid = self._obtain_id
+        element_id = f"{libname}.{name}"
+        with self._stack_handler.push_record(
+            "element", element_id, "YR", "RYR", hide_from_logs
+        ):
+            if hide_from_logs:
+                # I.e.: add to internal stack but don't write it.
+                return
+
+            self._write_with_separator(
+                "YR ",
+                [
+                    oid(name),
+                    oid(libname),
+                    oid(source),
+                    self._number(lineno),
+                    self._number(time_delta),
+                ],
+            )
+
+    def yield_from_suspend(
+        self,
+        name: str,
+        libname: str,
+        source: str,
+        lineno: int,
+        time_delta: float,
+    ):
+        """
+        Note: the yield_suspend is effectively the same thing as the `end_method`
+        because we're leaving the method (the difference being that it can be
+        resumed afterwards and we have the yielded value right now).
+        """
+
+        element_id = f"{libname}.{name}"
+        stack_entry = self._stack_handler.pop("element", element_id)
+        if stack_entry is None or stack_entry.hide_from_logs:
+            # If the start wasn't logged, the stop shouldn't be logged either
+            # (and if it was logged, the stop should be also logged).
+            return
+
+        oid = self._obtain_id
+
+        self._write_with_separator(
+            "YFS ",
+            [
+                oid(name),
+                oid(libname),
+                oid(source),
+                self._number(lineno),
+                self._number(time_delta),
+            ],
+        )
+
+    def yield_from_resume(
+        self,
+        name: str,
+        libname: str,
+        source: str,
+        lineno: int,
+        time_delta: float,
+        hide_from_logs: bool,
+    ):
+        """
+        Note that a yield resume is semantically very close to a start element
+        but it doesn't have any arguments.
+        """
+        oid = self._obtain_id
+        element_id = f"{libname}.{name}"
+        with self._stack_handler.push_record(
+            "element", element_id, "YR", "RYR", hide_from_logs
+        ):
+            if hide_from_logs:
+                # I.e.: add to internal stack but don't write it.
+                return
+
+            self._write_with_separator(
+                "YFR ",
+                [
+                    oid(name),
+                    oid(libname),
+                    oid(source),
+                    self._number(lineno),
+                    self._number(time_delta),
+                ],
+            )
+
     def after_assign(
         self,
         filename: str,
         lineno: int,
         assign_name: str,
         assign_type: str,
         assign_repr: str,
```

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_sensitive_variable_names.py` & `robocorp_log-0.0.13/src/robocorp/log/_sensitive_variable_names.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.12/src/robocorp/log/_suppress_helper.py` & `robocorp_log-0.0.13/src/robocorp/log/_suppress_helper.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.12/src/robocorp/log/protocols.py` & `robocorp_log-0.0.13/src/robocorp/log/protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.12/PKG-INFO` & `robocorp_log-0.0.13/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: robocorp-log
-Version: 0.0.12
+Version: 0.0.13
 Summary: Automatic trace logging for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Logging
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # robocorp-log
 
 `robocorp-log` is a library which provides comprehensible logging for python 
 with a focus on RPA, where detailed information on what happened and why a
```


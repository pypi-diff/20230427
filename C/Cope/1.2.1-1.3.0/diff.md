# Comparing `tmp/Cope-1.2.1.tar.gz` & `tmp/Cope-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cope-1.2.1.tar", last modified: Thu Apr 20 02:18:10 2023, max compression
+gzip compressed data, was "Cope-1.3.0.tar", last modified: Thu Apr 27 00:33:22 2023, max compression
```

## Comparing `Cope-1.2.1.tar` & `Cope-1.3.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 02:18:10.876068 Cope-1.2.1/
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 02:18:10.874069 Cope-1.2.1/Cope/
--rw-r--r--   0 leonard   (1000) leonard   (1000)      509 2023-04-19 19:49:02.000000 Cope-1.2.1/Cope/Psuedonym.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)       56 2023-04-19 19:39:52.000000 Cope-1.2.1/Cope/_None.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      415 2023-04-20 02:14:29.000000 Cope-1.2.1/Cope/__init__.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2410 2023-04-19 19:39:57.000000 Cope-1.2.1/Cope/bak.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     5659 2023-04-19 19:40:20.000000 Cope-1.2.1/Cope/colors.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1680 2023-04-19 19:41:11.000000 Cope-1.2.1/Cope/constants.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    16853 2023-04-20 00:39:52.000000 Cope-1.2.1/Cope/debugging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     6994 2023-04-19 19:43:42.000000 Cope-1.2.1/Cope/decorators.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)       41 2023-04-19 20:53:26.000000 Cope-1.2.1/Cope/errors.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1678 2023-04-19 19:43:55.000000 Cope-1.2.1/Cope/func.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1762 2023-04-19 19:54:46.000000 Cope-1.2.1/Cope/geometry.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     4771 2023-04-20 01:04:12.000000 Cope-1.2.1/Cope/imports.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    19332 2023-04-19 20:04:30.000000 Cope-1.2.1/Cope/iterables.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    29346 2023-04-19 19:48:23.000000 Cope-1.2.1/Cope/key.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    10139 2023-04-20 02:17:50.000000 Cope-1.2.1/Cope/linalg.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      757 2023-04-19 19:48:30.000000 Cope-1.2.1/Cope/logging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    12141 2023-04-19 20:47:52.000000 Cope-1.2.1/Cope/misc.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2838 2023-04-19 19:48:50.000000 Cope-1.2.1/Cope/point.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      818 2023-04-19 19:48:58.000000 Cope-1.2.1/Cope/prettyTable.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1226 2023-04-19 19:49:09.000000 Cope-1.2.1/Cope/pygame.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2325 2023-04-19 19:49:10.000000 Cope-1.2.1/Cope/timing.py
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 02:18:10.875069 Cope-1.2.1/Cope.egg-info/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2132 2023-04-20 02:18:10.000000 Cope-1.2.1/Cope.egg-info/PKG-INFO
--rw-r--r--   0 leonard   (1000) leonard   (1000)      796 2023-04-20 02:18:10.000000 Cope-1.2.1/Cope.egg-info/SOURCES.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)        1 2023-04-20 02:18:10.000000 Cope-1.2.1/Cope.egg-info/dependency_links.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)        5 2023-04-20 02:18:10.000000 Cope-1.2.1/Cope.egg-info/top_level.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)     9755 2023-04-20 01:57:58.000000 Cope-1.2.1/LICENSE-APACHE
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1072 2023-04-20 01:57:58.000000 Cope-1.2.1/LICENSE-MIT
--rw-r--r--   0 leonard   (1000) leonard   (1000)       61 2023-04-20 01:57:58.000000 Cope-1.2.1/MANIFEST.in
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2132 2023-04-20 02:18:10.876068 Cope-1.2.1/PKG-INFO
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1117 2023-04-20 02:04:21.000000 Cope-1.2.1/README.md
--rw-r--r--   0 leonard   (1000) leonard   (1000)      448 2023-04-20 02:14:44.000000 Cope-1.2.1/pyproject.toml
--rw-r--r--   0 leonard   (1000) leonard   (1000)       38 2023-04-20 02:18:10.876068 Cope-1.2.1/setup.cfg
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2115 2023-04-20 02:14:35.000000 Cope-1.2.1/setup.py
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 02:18:10.876068 Cope-1.2.1/tests/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1186 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_colors.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2353 2022-10-28 20:40:40.000000 Cope-1.2.1/tests/test_debugging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     3045 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_decorators.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      194 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_func.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      943 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_geometry.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      309 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_imports.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1743 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_iterables.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1262 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_key.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      228 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_logging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1717 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_misc.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      462 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_point.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      437 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_psuedonym.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      280 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_timing.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-27 00:33:22.625489 Cope-1.3.0/
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-27 00:33:22.623489 Cope-1.3.0/Cope/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      509 2023-04-19 19:49:02.000000 Cope-1.3.0/Cope/Psuedonym.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       56 2023-04-19 19:39:52.000000 Cope-1.3.0/Cope/_None.py
+-rw-------   0 leonard   (1000) leonard   (1000)      476 2023-04-26 23:05:58.000000 Cope-1.3.0/Cope/__init__.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      440 2023-04-26 23:38:47.000000 Cope-1.3.0/Cope/_config.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2410 2023-04-19 19:39:57.000000 Cope-1.3.0/Cope/bak.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     5659 2023-04-19 19:40:20.000000 Cope-1.3.0/Cope/colors.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)        0 2023-04-24 20:08:10.000000 Cope-1.3.0/Cope/constants.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    18283 2023-04-26 23:45:31.000000 Cope-1.3.0/Cope/debugging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     6995 2023-04-26 23:32:38.000000 Cope-1.3.0/Cope/decorators.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       41 2023-04-19 20:53:26.000000 Cope-1.3.0/Cope/errors.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1678 2023-04-19 19:43:55.000000 Cope-1.3.0/Cope/func.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1762 2023-04-19 19:54:46.000000 Cope-1.3.0/Cope/geometry.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     4937 2023-04-24 19:14:51.000000 Cope-1.3.0/Cope/imports.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    19332 2023-04-19 20:04:30.000000 Cope-1.3.0/Cope/iterables.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    29346 2023-04-19 19:48:23.000000 Cope-1.3.0/Cope/key.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    10240 2023-04-20 21:06:35.000000 Cope-1.3.0/Cope/linalg.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      760 2023-04-26 23:08:59.000000 Cope-1.3.0/Cope/logging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    12942 2023-04-27 00:24:32.000000 Cope-1.3.0/Cope/misc.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2838 2023-04-19 19:48:50.000000 Cope-1.3.0/Cope/point.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      818 2023-04-19 19:48:58.000000 Cope-1.3.0/Cope/prettyTable.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1226 2023-04-19 19:49:09.000000 Cope-1.3.0/Cope/pygame.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2325 2023-04-19 19:49:10.000000 Cope-1.3.0/Cope/timing.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-27 00:33:22.624489 Cope-1.3.0/Cope.egg-info/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2239 2023-04-27 00:33:22.000000 Cope-1.3.0/Cope.egg-info/PKG-INFO
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      867 2023-04-27 00:33:22.000000 Cope-1.3.0/Cope.egg-info/SOURCES.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)        1 2023-04-27 00:33:22.000000 Cope-1.3.0/Cope.egg-info/dependency_links.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       24 2023-04-27 00:33:22.000000 Cope-1.3.0/Cope.egg-info/requires.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)        5 2023-04-27 00:33:22.000000 Cope-1.3.0/Cope.egg-info/top_level.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     9755 2023-04-20 01:57:58.000000 Cope-1.3.0/LICENSE-APACHE
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1072 2023-04-20 01:57:58.000000 Cope-1.3.0/LICENSE-MIT
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       61 2023-04-20 01:57:58.000000 Cope-1.3.0/MANIFEST.in
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2239 2023-04-27 00:33:22.624489 Cope-1.3.0/PKG-INFO
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1117 2023-04-20 02:04:21.000000 Cope-1.3.0/README.md
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      666 2023-04-20 20:36:07.000000 Cope-1.3.0/pyproject.toml
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       38 2023-04-27 00:33:22.625489 Cope-1.3.0/setup.cfg
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2125 2023-04-20 22:23:00.000000 Cope-1.3.0/setup.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-27 00:33:22.624489 Cope-1.3.0/tests/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1186 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_colors.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2659 2023-04-26 23:49:56.000000 Cope-1.3.0/tests/test_debugging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     3045 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_decorators.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      194 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_func.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      943 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_geometry.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      309 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_imports.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1743 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_iterables.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1262 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_key.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      228 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_logging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1680 2023-04-27 00:33:06.000000 Cope-1.3.0/tests/test_misc.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      462 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_point.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      437 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_psuedonym.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      714 2023-04-27 00:21:44.000000 Cope-1.3.0/tests/test_replace_lines.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      280 2022-09-10 20:02:11.000000 Cope-1.3.0/tests/test_timing.py
```

### Comparing `Cope-1.2.1/Cope/bak.py` & `Cope-1.3.0/Cope/bak.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/Cope/colors.py` & `Cope-1.3.0/Cope/colors.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/Cope/debugging.py` & `Cope-1.3.0/Cope/debugging.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,57 @@
-from .imports import ensureImported
-from .colors import coloredOutput, darken, resetColor, printColor, COUNT, CONTEXT, DEFAULT_DEBUG, WARN, ALERT, DEBUG_METADATA_DARKEN, DEBUG_TYPE_DARKEN, DEBUG_NAME_DARKEN, DEBUG_EQUALS, DEBUG_VALUE_DARKEN, NOTE_CALL, STACK_TRACE
-from re import search as re_search
-# import .colors as colors
-from ._None import _None
-from .constants import VERBOSE
+from inspect import stack
 from os import get_terminal_size
-from os.path import basename
+from os.path import basename, relpath
+from re import search as re_search
+from re import match as re_match
 from typing import Union
-from inspect import stack
-# from . import colors
-# from varname import VarnameRetrievingError, argname, nameof
 
-DISPLAY_FILE = ''
-DISPLAY_FUNC = ''
-DISPLAY_LINK = ''
-DISPLAY_PATH = ''
-ROOT = ''
+# varnameImported = ensureImported('varname', ('VarnameRetrievingError', 'argname', 'nameof'))
+from varname import VarnameRetrievingError, argname, nameof
 
-varnameImported = ensureImported('varname', ('ImproperUseError', 'VarnameRetrievingError', 'argname', 'nameof'))
-_debugCount = 0
+# from .imports import ensureImported
+from ._config import config
+from ._None import _None
+# from . import colors
+from .colors import (ALERT, CONTEXT, COUNT, DEBUG_EQUALS,
+                     DEBUG_METADATA_DARKEN, DEBUG_NAME_DARKEN,
+                     DEBUG_TYPE_DARKEN, DEBUG_VALUE_DARKEN, DEFAULT_DEBUG,
+                     EMPTY, NOTE_CALL, STACK_TRACE, WARN, coloredOutput,
+                     darken, printColor, resetColor)
 
-DEBUGGING_DEBUG = False
 _repr = repr
 
+# def test():
+#     print('display_file:', config.display_file)
+#     print('display_func:', config.display_func)
+#     print('display_path:', config.display_path)
+
 def printArgs(*args, **kwargs):
     print('args:', args)
     print('kwargs:', kwargs)
 
-def getMetaData(calls=1):
+def get_metadata(calls=1):
     """ Gets the meta data of the line you're calling this function from.
         Calls is for how many function calls to look back from.
     """
     try:
         s = stack()[calls]
         return s
     except IndexError:
         return None
 
-def getLink(calls=0, full=False, customMetaData=None):
+def get_link(calls=0, full=False, customMetaData=None):
     if customMetaData is not None:
         d = customMetaData
     else:
-        d = getMetaData(calls+2)
+        d = get_metadata(calls+2)
 
-    printLink(d.filename, d.lineno, d.function if full else None)
+    print_link(d.filename, d.lineno, d.function if full else None)
 
-def getListStr(iterable: Union[tuple, list, set, dict], useMultiline:bool=True, limitToLine: bool=False, minItems: int=2, maxItems: int=50) -> str:
+def get_iterable_str(iterable: Union[tuple, list, set, dict], useMultiline:bool=True, limitToLine: bool=False, minItems: int=2, maxItems: int=50) -> str:
     """ "Cast" a tuple, list, set or dict to a string, automatically shorten
         it if it's long, and display how long it is.
 
         Params:
             limitToLine: if True, limit the length of list to a single line
             minItems: show at least this many items in the list
             maxItems: show at most this many items in the list
@@ -120,15 +122,15 @@
 
         return firstHalf + ellipsis + secondHalf + length
 
     else:
         return str(v) + f'(len={len(v)})'
     """
 
-def getTypename(var, addBraces=True):
+def get_typename(var, addBraces=True):
     def getUniqueType(item):
         returnMe = type(item).__name__
         while type(item) in (tuple, list, set):
             try:
                 item = item[0]
             except (KeyError, IndexError, TypeError):
                 returnMe += '('
@@ -155,15 +157,15 @@
         if len(types) == 1:
             fullName = fullName[:-2] + ')'
         rtn = fullName
     else:
         rtn = type(var).__name__
     return f'<{rtn}>' if addBraces else rtn
 
-def printLink(filename, lineNum, function=None):
+def print_link(filename, lineNum, function=None):
     """ Print a VSCodium clickable file and line number
         If function is specified, a full python error message style line is printed
     """
     try:
         printColor('', color=(40, 43, 46))
         if function is None:  #    \|/  Oddly enough, this double quote is nessicary
             print('\t', filename, '", line ', lineNum, '\033[0m', sep='')
@@ -172,121 +174,148 @@
 
         resetColor()
     finally:
         resetColor()
     resetColor()
     print('\033[0m', end='')
 
-def debugCount(leftAdjust=2, color: int=COUNT):
-    global _debugCount
-    _debugCount += 1
+def print_debug_count(leftAdjust=2, color: int=COUNT):
+    config._debug_count += 1
     with coloredOutput(color):
-        print(f'{str(_debugCount)+":":<{leftAdjust+2}}', end='')
+        print(f'{str(config._debug_count)+":":<{leftAdjust+2}}', end='')
 
-def manualGetVarName(var, full=True, calls=2, metadata=None):
-    try:
-        return re_search(r'(?<=debug\().+(?=,(\s)?[name color showFunc showFile showPath useRepr calls background limitToLine minItems maxItems stackTrace raiseError clr _repr trace bg throwError throw \) ])',
-                         metadata.code_context[0]).group()
-    except:
+# Doesn't work
+def get_varname_manually(var, full=True, calls=2, metadata=None):
+    # Not quite sure why it's plus 2?...
+    line = get_metadata(calls=calls+2).code_context[0]
+    # Made with ezregex
+    # optional(stuff) + 'debug(' + group(stuff + multiOptional('(' + optional(stuff) + ')')) + ')' + optional(stuff)
+    match = re_match(r"(?:.+)?debug\((.+(?:\((?:.+)?\))*)\)(?:.+)?", line)
+    if match is None:
         return '?'
+    else:
+        return match.groups()[0]
+    # ans.test('abc = lambda a: 6+ debug(parseColorParams((5, 5, 5)), name=8, clr=(a,b,c))\n')
+    return '?'
 
-def getVarName(var, full=True, calls=1, metadata=None):
+def get_varname(var, full=True, calls=1, metadata=None):
     try:
-        return argname('var', frame=calls+1)
+        rtn = argname('var', frame=calls+1)
     # It's a *likely* string literal
     except Exception as e:
         if type(var) is str:
-            return None
+            rtn = None
         else:
             try:
                 # print('var:', var)
                 # print('var type:', type(var))
-                return nameof(var, frame=calls+1)
-            except Exception as e:
-                if VERBOSE and DEBUGGING_DEBUG and not isinstance(var, Exception):
-                    raise e
+                rtn = nameof(var, frame=calls+1, vars_only=False)
+            except Exception as e2:
+                if config.verbosity >= 2 and not isinstance(var, Exception):
+                    raise e2
                 else:
-                    return manualGetVarName(var, full, calls+1, metadata)
+                    rtn = get_varname_manually(var, full, calls+1, metadata)
     except VarnameRetrievingError as e:
-        if VERBOSE:
+        if config.verbosity:
             raise e
         else:
-            return manualGetVarName(var, full, calls+1, metadata)
+            rtn = get_varname_manually(var, full, calls+1, metadata)
 
-def getAdjustedFilename(filename):
-    if ROOT:
-        return filename[len(ROOT)+1:]
+    try:
+        # It auto-adds ' around strings
+        if rtn == str(var) or rtn == f"'{var}'":
+            # If the value is the same as the name, it must be a literal
+            return None
+        else:
+            return rtn
+    except:
+        return rtn
+
+
+def get_adjusted_filename(filename):
+    # Default behavior
+    if config.root_dir is None:
+        return relpath(filename)
+    elif len(config.root_dir):
+        return relpath(filename, config.root_dir)
     else:
         return filename
 
-def getContext(metadata, useVscodeStyle, showFunc, showFile, showPath):
-    #* Set the stuff in the [] (the "context")
-    if metadata is not None:
-        if useVscodeStyle:
-            s = f'["{metadata.filename if showPath else getAdjustedFilename(metadata.filename)}", line {metadata.lineno}'
-            if showFunc:
-                if metadata.function.startswith('<'):
-                    s += ', in Global Scope'
-                else:
-                    s += f', in {metadata.function}()'
-            s += '] '
-            return s
-        else:
-            context = str(metadata.lineno)
-            if showFunc:
-                if metadata.function.startswith('<'):
-                    context = 'Global Scope' + context
-                else:
-                    context = metadata.function + '()->' + context
-
-            if showFile:
-                context = (metadata.filename if showPath else basename(metadata.filename)) + '->' + context
+def get_context(metadata, showFunc, showFile, showPath) -> str:
+    """ Returns the stuff in the [] (the "context") """
+    if metadata is None:
+        return ''
 
-            return f'[{context}] '
+    # This logically must be true
+    if showPath:
+        showFile = True
+
+    s = '['
+    if showPath:
+        s += f'"{metadata.filename}", line {metadata.lineno}, in '
+    elif showFile:
+        s += f'"{get_adjusted_filename(metadata.filename)}", line {metadata.lineno}, in '
+    # We apparently don't want any context at all (for whatever reason)
+    elif not showFunc:
+        return ''
+
+    if showFunc:
+        if metadata.function.startswith('<'):
+            s += 'Global Scope'
+        else:
+            s += f'{metadata.function}()'
     else:
-        return ' '
+        # Take out the comma and the space, if we're not using them
+        s = s[:-5]
+    s += '] '
+    return s
 
-def printStackTrace(calls, useVscodeStyle, showFunc, showFile, showPath):
+
+def print_stack_trace(calls, showFunc, showFile, showPath):
     for i in reversed(stack()[3:]):
-        print('\t', getContext(i, useVscodeStyle, showFunc, showFile, showPath))
+        print('\t', get_context(i, showFunc, showFile, showPath))
 
-def beingUsedAsDecorator(funcName, metadata=None, calls=1) -> 'Union[1, 2, 3, False]':
+def called_as_decorator(funcName, metadata=None, calls=1) -> 'Union[1, 2, 3, False]':
     """ Return 1 if being used as a function decorator, 2 if as a class decorator, 3 if not sure, and False if neither. """
     if metadata is None:
-        metadata = getMetaData(calls+1)
+        metadata = get_metadata(calls+1)
 
     # print(metadata.code_context)
-    line = metadata.code_context[0]
+    context = metadata.code_context
+    # I think this means we're using python from the command line
+    if context is None:
+        return False
+    line = context[0]
 
     if funcName not in line:
         if 'def ' in line:
             return 1
         elif 'class ' in line:
             return 2
         elif '@' in line:
             return 3
     elif '@' in line:
         return 3
 
     return False
 
-def printContext(calls=1, color=CONTEXT, showFunc=True, showFile=True, showPath=True):
-    debugCount()
+def print_context(calls=1, color=CONTEXT, showFunc=True, showFile=True, showPath=True):
+    print_debug_count()
     with coloredOutput(color):
-        print(getContext(getMetaData(1 + calls), True,
-                               showFunc or DISPLAY_FUNC,
-                               showFile or DISPLAY_FILE,
-                               showPath or DISPLAY_PATH), end='')
+        print(get_context(get_metadata(1 + calls),
+                               showFunc or config.display_func,
+                               showFile or config.display_file,
+                               showPath or config.display_path), end='')
 
 def debug(var=_None,                # The variable to debug
           name: str=None,           # Don't try to get the name, use this one instead
           color=_None,              # A number (0-5), a 3 item tuple/list, or None
-          showFunc: bool=True,      # Expressly show what function we're called from
-          showFile: bool=True,      # Expressly show what file we're called from
-          showPath: bool=False,     # Show just the file name, or the full filepath
+          showFunc: bool=None,      # Expressly show what function we're called from
+          showFile: bool=None,      # Expressly show what file we're called from
+          showPath: bool=None,      # Show just the file name, or the full filepath
           useRepr: bool=False,      # Whether we should print the repr of var instead of str
           calls: int=1,             # Add extra calls
           active: bool=True,        # If this is false, don't do anything
           background: bool=False,   # Whether the color parameter applies to the forground or the background
           limitToLine: bool=True,   # When printing iterables, whether we should only print items to the end of the line
           minItems: int=50,         # Minimum number of items to print when printing iterables (overrides limitToLine)
           maxItems: int=-1,         # Maximum number of items to print when printing iterables, use None or negative to specify no limit
@@ -324,106 +353,119 @@
             background: Changes the background color instead of the forground color
             active: Conditionally disables the function
             clr: Alias of color
             _repr: Alias of useRepr
             trace: Alias of stackTrace
             bg: Alias of background
     """
-    if not active or not __debug__:
-        return var
+    try:
+        if not active or not __debug__:
+            return var
 
-    stackTrace = stackTrace or trace
-    useRepr = useRepr or repr
-    background = background or bg
-    throwError = throw or throwError or raiseError
-    useColor = (DEFAULT_DEBUG if clr is _None else clr) if color is _None else color
-
-    if maxItems < 0 or maxItems is None:
-        maxItems = 1000000
-
-    if isinstance(var, Warning):
-        useColor = WARN
-    elif isinstance(var, Exception):
-        useColor = ALERT
-
-    # +1 call because we don't want to get this line, but the one before it
-    metadata = getMetaData(calls+1)
-
-    #* First see if we're being called as a decorator
-    if callable(var) and beingUsedAsDecorator('debug', metadata):
-        def wrap(*args, **kwargs):
-            # +1 call because we don't want to get this line, but the one before it
-            metadata = getMetaData(2)
-
-            debugCount()
-
-            if stackTrace:
-                with coloredOutput(STACK_TRACE):
-                    printStackTrace(2, True, showFunc, showFile, showPath)
-
-            with coloredOutput(NOTE_CALL):
-                print(getContext(metadata, True, showFunc or DISPLAY_FUNC, showFile or DISPLAY_FILE, showPath or DISPLAY_PATH), end='')
-                print(f'{var.__name__}() called!')
-                # print(args)
-            return var(*args, **kwargs)
-
-        return wrap
-
-    debugCount()
-
-    if stackTrace:
-        with coloredOutput(STACK_TRACE):
-            printStackTrace(calls+1, True, showFunc, showFile, showPath)
-
-    #* Only print the "HERE! HERE!" message
-    if var is _None:
-        with coloredOutput(useColor if color is not _None else EMPTY, not background):
-            print(getContext(metadata, True, showFunc or DISPLAY_FUNC, showFile or DISPLAY_FILE, showPath or DISPLAY_PATH), end='')
-            if not metadata.function.startswith('<'):
-                print(f'{metadata.function}() called ', end='')
-            print('HERE!')
-        return
-
-    metadataColor = darken(DEBUG_METADATA_DARKEN,  useColor)
-    typeColor     = darken(DEBUG_TYPE_DARKEN,  useColor)
-    nameColor     = darken(DEBUG_NAME_DARKEN, useColor)
-    equalsColor   = DEBUG_EQUALS
-    valueColor    = darken(DEBUG_VALUE_DARKEN, useColor)
-    #* Print the standard line
-    with coloredOutput(metadataColor, not background):
-        print(getContext(metadata, True,
-                                showFunc or DISPLAY_FUNC,
-                                showFile or DISPLAY_FILE,
-                                showPath or DISPLAY_PATH), end='')
-
-    #* Seperate the variables into a tuple of (typeStr, varString)
-    varType = getTypename(var)
-    if useRepr:
-        varVal = _repr(var)
-    else:
-        if isinstance(var, (tuple, list, set, dict)):
-            varVal  = getListStr(var, limitToLine, minItems, maxItems)
+        stackTrace = stackTrace or trace
+        useRepr = useRepr or repr
+        background = background or bg
+        throwError = throw or throwError or raiseError
+        useColor = (DEFAULT_DEBUG if clr is _None else clr) if color is _None else color
+
+        if maxItems < 0 or maxItems is None:
+            maxItems = 1000000
+
+        if isinstance(var, Warning):
+            useColor = WARN
+        elif isinstance(var, Exception):
+            useColor = ALERT
+
+        # +1 call because we don't want to get this line, but the one before it
+        metadata = get_metadata(calls+1)
+
+        #* First see if we're being called as a decorator
+        if callable(var) and called_as_decorator('debug', metadata):
+            def wrap(*args, **kwargs):
+                # +1 call because we don't want to get this line, but the one before it
+                metadata = get_metadata(2)
+
+                print_debug_count()
+
+                if stackTrace:
+                    with coloredOutput(STACK_TRACE):
+                        print_stack_trace(2, showFunc, showFile, showPath)
+
+                with coloredOutput(NOTE_CALL):
+                    print(get_context(metadata,
+                        showFunc or config.display_func,
+                        showFile or config.display_file,
+                        showPath or config.display_path), end='')
+                    print(f'{var.__name__}() called!')
+                    # print(args)
+                return var(*args, **kwargs)
+
+            return wrap
+
+        print_debug_count()
+
+        if stackTrace:
+            with coloredOutput(STACK_TRACE):
+                print_stack_trace(calls+1, showFunc, showFile, showPath)
+
+        #* Only print the "HERE! HERE!" message
+        if var is _None:
+            with coloredOutput(useColor if color is not _None else EMPTY, not background):
+                print(get_context(metadata,
+                    showFunc or config.display_func,
+                    showFile or config.display_file,
+                    showPath or config.display_path), end='')
+                if not metadata.function.startswith('<'):
+                    print(f'{metadata.function}() called ', end='')
+                print('HERE!')
+            return
+
+        metadataColor = darken(DEBUG_METADATA_DARKEN,  useColor)
+        typeColor     = darken(DEBUG_TYPE_DARKEN,  useColor)
+        nameColor     = darken(DEBUG_NAME_DARKEN, useColor)
+        equalsColor   = DEBUG_EQUALS
+        valueColor    = darken(DEBUG_VALUE_DARKEN, useColor)
+        #* Print the standard line
+        with coloredOutput(metadataColor, not background):
+            print(get_context(metadata,
+                                    showFunc or config.display_func,
+                                    showFile or config.display_file,
+                                    showPath or config.display_path), end='')
+
+        #* Seperate the variables into a tuple of (typeStr, varString)
+        varType = get_typename(var)
+        if useRepr:
+            varVal = _repr(var)
         else:
-            varVal  = str(var)
+            if isinstance(var, (tuple, list, set, dict)):
+                varVal  = get_iterable_str(var, limitToLine, minItems, maxItems)
+            else:
+                varVal  = str(var)
+
+        with coloredOutput(nameColor, not background):
+            #* Actually get the name
+            varName = get_varname(var, calls=calls, metadata=metadata) if name is None else name
+            # It's a string literal
 
-    with coloredOutput(nameColor, not background):
-        #* Actually get the name
-        varName = getVarName(var, calls=calls, metadata=metadata) if name is None else name
-        # It's a string literal
         if varName is None:
-            print(var)
+            with coloredOutput(typeColor, not background):
+                print('<literal> ', end='')
+            with coloredOutput(nameColor, not background):
+                print(var)
             return var
 
-    with coloredOutput(typeColor, not background):
-        print(varType, end=' ')
-    with coloredOutput(nameColor, not background):
-        print(varName, end=' ')
-    with coloredOutput(equalsColor, not background):
-        print('=', end=' ')
-    with coloredOutput(valueColor, not background):
-        print(varVal)
+        with coloredOutput(typeColor, not background):
+            print(varType, end=' ')
+        with coloredOutput(nameColor, not background):
+            print(varName, end=' ')
+        with coloredOutput(equalsColor, not background):
+            print('=', end=' ')
+        with coloredOutput(valueColor, not background):
+            print(varVal)
 
-    if isinstance(var, Exception) and throwError:
-        raise var
+        if isinstance(var, Exception) and throwError:
+            raise var
 
-    # Does the same this as debugged used to
-    return var
+        # Does the same this as debugged used to
+        return var
+    finally:
+        resetColor()
```

### Comparing `Cope-1.2.1/Cope/decorators.py` & `Cope-1.3.0/Cope/decorators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from .debugging import getMetaData, beingUsedAsDecorator, debugCount, getContext, printContext
-from .constants import HIDE_TODO, DISPLAY_PATH, DISPLAY_FILE, DISPLAY_FUNC
+from .debugging import get_metadata, called_as_decorator, print_debug_count, get_context, print_context
 from .misc import CommonResponses
 from .colors import coloredOutput, darken
+from ._config import config
 
 
 ################################### Decorators ###################################
 __todoCalls = set()
 def todo(featureName=None, enabled=True, blocking=False, limitCalls=True,
          showFunc=True, showFile=True, showPath=False):
     """ Leave reminders for yourself to finish parts of your code.
         Can be manually turned on or off with hideAllTodos(bool).
         Can also be used as a decorator (function, or class) to print a reminder
         and also throw a NotImplemented error on being called/constructed.
     """
     if not __debug__: return
 
-    metadata  = getMetaData(2)
-    situation = beingUsedAsDecorator('todo', metadata)
+    metadata  = get_metadata(2)
+    situation = called_as_decorator('todo', metadata)
     # First off, if we're limiting calls, check if we've already been called
     uniqueID = (metadata.lineno, metadata.filename)
     if limitCalls and uniqueID in __todoCalls:
         return
     else:
         __todoCalls.add(uniqueID)
 
@@ -28,21 +28,21 @@
     #     def wrap(func):
     #         def innerWrap(*funcArgs, **funcKwArgs):
     #             return func(*funcArgs, **funcKwArgs)
     #         return innerWrap
     #     return wrap
 
     def printTodo(disableFunc):
-        if not HIDE_TODO and enabled:
-            debugCount()
+        if not config.hide_todo and enabled:
+            print_debug_count()
             with coloredOutput(Colors.TODO):
-                print(getContext(metadata, True,
-                                (showFunc or DISPLAY_FUNC) and not disableFunc,
-                                showFile or DISPLAY_FILE,
-                                showPath or DISPLAY_PATH), end='')
+                print(get_context(metadata, True,
+                                (showFunc or config.display_func) and not disableFunc,
+                                showFile or config.display_file,
+                                showPath or config.display_path), end='')
                 # This is coincidental, but it works
                 print(f'TODO: {featureName.__name__ if disableFunc else featureName}')
             if blocking:
                 raise NotImplementedError()
 
     # Being used as a function decorator, or we're not sure
     if situation in (1, 3):
@@ -82,20 +82,20 @@
                     assert(type(level) in (int, float))
                     return f'({level}% confidence)'
 
             def definiteFail():
                 raise UserWarning(f"{func.__name__} is going to fail. {getPrettyLevel()}")
 
             def probablyFail():
-                printContext(3, darken(80, Colors.ALERT), showFunc=False)
+                print_context(3, darken(80, Colors.ALERT), showFunc=False)
                 with coloredOutput(Colors.ALERT):
                     print(f"Warning: {func.__name__} will probably fail. {getPrettyLevel()}")
 
             def possiblyFail():
-                printContext(3, darken(80, Colors.CONFIDENCE_WARNING), showFunc=False)
+                print_context(3, darken(80, Colors.CONFIDENCE_WARNING), showFunc=False)
                 with coloredOutput(Colors.CONFIDENCE_WARNING):
                     print(f"Warning: {func.__name__} might not work. {getPrettyLevel()}")
 
             def unknownInput():
                 # If we don't understand the input, just give a soft warning (it will display what the input is, anyway)
                 possiblyFail()
                 return
@@ -156,15 +156,15 @@
 tested = confidence(80)
 
 def depricated(why=''):
     if not __debug__: return
 
     def wrap(func):
         def innerWrap(*funcArgs, **funcKwArgs):
-            printContext(2, darken(80, Colors.DEPRICATED_WARNING))
+            print_context(2, darken(80, Colors.DEPRICATED_WARNING))
             with coloredOutput(Colors.DEPRICATED_WARNING):
                 print(f"{func.__name__} is Depricated{': ' if len(why) else '.'}{why}")
             return func(*funcArgs, **funcKwArgs)
         return innerWrap
     return wrap
 
 def reprise(obj, *args, **kwargs):
```

### Comparing `Cope-1.2.1/Cope/func.py` & `Cope-1.3.0/Cope/func.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/Cope/geometry.py` & `Cope-1.3.0/Cope/geometry.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/Cope/imports.py` & `Cope-1.3.0/Cope/imports.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Union, Iterable, Literal
 import importlib
+from varname import nameof
 
 
 def installLib(libs:Iterable):
     libs = ' '.join(libs)
 
     def useSubprocess():
         import subprocess
@@ -52,19 +53,21 @@
             raise ImportError(package)
             return False
         else:
             raise TypeError(f'Unknown if_unavailable value given: {if_unavailable}')
             return False
     else:
         if len(specificModules):
-            for i in specificModules[:-1]:
-                globals()[i] = imported.__getattribute__(i)
-            globals()[as_ if as_ else specificModules[-1]] = imported.__getattribute__(specificModules[-1])
+            # print('returning imported')
+            # return imported
+            for i in specificModules:
+                _globals[i] = imported.__getattribute__(i)
+            # globals()[as_ if as_ else specificModules[-1]] = imported.__getattribute__(specificModules[-1])
         else:
-            globals()[as_ if as_ else package] = imported
+            _globals[as_ if as_ else package] = imported
     return True
 
 # todo
 def checkImport(package:str, specificModules=[], _as=None,
                 fatal:bool=False, printWarning:Union[str, bool]=True,
                 _globals=globals(), _locals=locals(), level=0
                 ) -> "(Union[package, (packages,)], worked)":
@@ -99,14 +102,15 @@
                     _globals=globals(), _locals=locals(),
                     level=0):
     def wrap(func):
         def innerWrap(*funcArgs, **funcKwArgs):
             if ensureImported(package, specificModules, as_, if_unavailable, globals, locals, level):
                 return func(*funcArgs, **funcKwArgs)
             else:
+                print(f'Failed to import {package} for {nameof(func)}')
                 return None
         return innerWrap
     return wrap
 
 def importpath(path, name, moduleName):
     spec = importlib.util.spec_from_file_location(name, path)
     module = importlib.util.module_from_spec(spec)
```

### Comparing `Cope-1.2.1/Cope/iterables.py` & `Cope-1.3.0/Cope/iterables.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/Cope/key.py` & `Cope-1.3.0/Cope/key.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/Cope/linalg.py` & `Cope-1.3.0/Cope/linalg.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 ensureImported('sympy')
 import sympy as sp
 
 
 @dependsOnPackage('clipboard', 'copy')
 @dependsOnPackage('sympy', ('Matrix', 'ImmutableMatrix', 'latex', 'sympify'))
 def matrix(string, rows=None, cols=None, cp=False, np=False, immutable=False, verbose=False):
+    # print('test')
+    # ensureImported('sympy', ('Matrix', 'ImmutableMatrix', 'latex', 'sympify'))
     # from sympy import latex
     # Parse params
     assert rows is None or cols is None
     if np:
         type_ = _np.array
         # Yes, this is a despicable line of code, I know.
         # All this does is makes a function that casts everything in a nested list to a float
```

### Comparing `Cope-1.2.1/Cope/logging.py` & `Cope-1.3.0/Cope/logging.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from .colors import LOG_COLOR, coloredOutput, WARN
-from .constants import LOG_LEVEL
-from .debugging import printContext
+from .debugging import print_context
 from enum import Enum
+from ._config import config
 
 class LogLevel(Enum):
     NONE = 0
     LOGGING = 1
     WARNINGS = 2
     ERRORS = 3
 
-
 def log(message, levelReq=LogLevel.LOGGING, color=LOG_COLOR):
     if not __debug__: return
-    if LOG_LEVEL >= levelReq.value:
-        printContext(2)
+    if config.verbosity >= levelReq.value:
+        print_context(2)
         with coloredOutput(color):
             print(message)
 
 def warn(message):
     if not __debug__: return
     log(message, color=WARN)
 warning = warn
```

### Comparing `Cope-1.2.1/Cope/misc.py` & `Cope-1.3.0/Cope/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # from .decorators import todo, confidence
 from .imports import dependsOnPackage
-from .debugging import getVarName, beingUsedAsDecorator, debug, getMetaData
+from .debugging import get_varname, called_as_decorator, debug, get_metadata
 from .colors import ERROR
 import re
 import subprocess
 from os.path import join
 from random import randint
 import sys
-
+from math import floor
 from unicodedata import normalize
 
 def available(*args, fail_if_none=True):
     """ Returns the parameter passed to it which is not None, failing if more than one is None,
         and optionally failing if none of them are None """
     from varname import argname
 
@@ -177,32 +177,31 @@
         # add the word to the current line and a space character after it
         current_line += word + " "
         # add the current line to the result
         result += current_line
     return result
 
 def assertValue(param, *values, blocking=True):
-    paramName = getVarName(param)
-    if not beingUsedAsDecorator('assertValue'):
+    paramName = get_varname(param)
+    if not called_as_decorator('assertValue'):
         if param not in values:
             err = TypeError(f"Invalid value for {paramName}, must be one of: {values}")
             if blocking:
                 raise err
             else:
                 debug(err)
     else:
         print('TODO: AssertValue usage as a decorator')
 
-# @confidence(72)
-def replaceLine(line, offset=0, keepTabs=True, convertTabs=True, additionalCalls=0):
+def replaceLine(line, offset=0, keepTabs=True, convertTabs=True, calls=0):
     """ Replaces the line of code this is called from with the give line parameter.
-        This is probably a very bad idea to actually use.
-        Don't forget to add tabs! Newline is already taken care of (unless you want to add more).
+        This is a very bad idea and you should not use it
+        Automatically adds a newline to the end, but does not automatically add tabs.
     """
-    meta = getMetaData(calls=2 + additionalCalls)
+    meta = get_metadata(calls=calls+2)
 
     with open(meta.filename, 'r') as f:
         file = f.readlines()
 
     # Not really sure of the reason for the -1.
     if file[meta.lineno-1] == meta.code_context[0]:
         if keepTabs:
@@ -218,19 +217,38 @@
     else:
         debug(f"Error: lines don't match, not replacing line.\n\tMetadata: \"{meta.code_context}\"\n\tFile: \"{file[meta.lineno-1]}\"", clr=ERROR)
         return
 
     with open(meta.filename, 'w') as f:
         f.writelines(file)
 
-# @confidence(85)
-def fancyComment(title='', char='#', endChar='#', lineLimit=80):
-    """ Replaces the call with a nicely formatted comment line """
-    halfLen = ((lineLimit / len(char)) - len(title) - 1 - (2 if len(title) else 0) - len(endChar)) / 2
-    seperateChar = ' ' if len(title) else ''
+def comment(comment='', char='#', start='', end='', line_limit=80):
+    """ Replaces the call with a nicely formatted comment line next time the line is run
+        CAVIAT: This is a terrible, terrible function that you should NOT use.
+                I'm pretty confident it won't overwrite your source code.
+                And it's surprisingly useful.
+                But still, use at your own risk.
+    """
+    if not len(char):
+        replaceLine('# ' + comment, calls=1)
+        return
+    if not len(start):
+        start = char
+    if not len(end):
+        end = char
+
+    # Calculate half the distance - comment
+    half = (((line_limit // len(char)) - len(comment) - 1 - (2 if len(comment) else 0) - len(end)) // 2) - 1
+    # We want the comment to be nicely seperated
+    seperateChar = ' ' if len(comment) else ''
+    # Add them all together
+    c = '#' + start + (char * half) + seperateChar + comment + seperateChar + (char * half)
+    # If it doesn't quite reach the max number of characters, make sure it does
+    c += ((line_limit - len(c) - len(end)) // len(char)) * char
+    replaceLine(c + end, calls=1)
 
 def confirm(prompt='Continue?', returnIfInvalid=False, failedFunc=lambda: None, includeYN=True, quit=False, quitMsg='Okay then, exiting...'):
     response = input(prompt + (" (y/N): " if includeYN else '')).lower()
     if response in ('y', 'yes'):
         return True
     elif response in ('n', 'no'):
         if quit:
```

### Comparing `Cope-1.2.1/Cope/point.py` & `Cope-1.3.0/Cope/point.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/Cope/prettyTable.py` & `Cope-1.3.0/Cope/prettyTable.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/Cope/pygame.py` & `Cope-1.3.0/Cope/pygame.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/Cope/timing.py` & `Cope-1.3.0/Cope/timing.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/Cope.egg-info/PKG-INFO` & `Cope-1.3.0/Cope.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: Cope
-Version: 1.2.1
+Version: 1.3.0
+Summary: A bunch of generic functions and classes useful in multiple projects
 Home-page: https://github.com/smartycope/Cope
 Author: Copeland Carter
 Author-email: smartycope@gmail.com
 Maintainer: Copeland Carter
 Maintainer-email: smartycope@gmail.com
 License: MIT/Apache-2.0
 Classifier: Development Status :: 4 - Beta
@@ -16,16 +17,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires: varname
-Requires: sympy
+Description-Content-Type: text/markdown
+Provides-Extra: linalg
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 
 # Cope
 
 This is my personal "standard library" of all the generally useful code I've written for various projects over the years. Pretty much any time I've written a function or class and thought "this might be useful later", I've stuffed it in here. As such, a lot of it is super useful, a lot of it is garbage, and a lot of it has become obsoleted as I've learned more and found new libraries. I've tried to keep it clean and organized, but there is a lot of it. I also have tests written for a bunch of it, but not all. The debug function in particular I'm especially proud of. I've spent more time than is reasonable on it.
```

### Comparing `Cope-1.2.1/Cope.egg-info/SOURCES.txt` & `Cope-1.3.0/Cope.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 Cope/Psuedonym.py
 Cope/_None.py
 Cope/__init__.py
+Cope/_config.py
 Cope/bak.py
 Cope/colors.py
 Cope/constants.py
 Cope/debugging.py
 Cope/decorators.py
 Cope/errors.py
 Cope/func.py
@@ -24,21 +25,23 @@
 Cope/point.py
 Cope/prettyTable.py
 Cope/pygame.py
 Cope/timing.py
 Cope.egg-info/PKG-INFO
 Cope.egg-info/SOURCES.txt
 Cope.egg-info/dependency_links.txt
+Cope.egg-info/requires.txt
 Cope.egg-info/top_level.txt
 tests/test_colors.py
 tests/test_debugging.py
 tests/test_decorators.py
 tests/test_func.py
 tests/test_geometry.py
 tests/test_imports.py
 tests/test_iterables.py
 tests/test_key.py
 tests/test_logging.py
 tests/test_misc.py
 tests/test_point.py
 tests/test_psuedonym.py
+tests/test_replace_lines.py
 tests/test_timing.py
```

### Comparing `Cope-1.2.1/LICENSE-APACHE` & `Cope-1.3.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/LICENSE-MIT` & `Cope-1.3.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/PKG-INFO` & `Cope-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: Cope
-Version: 1.2.1
+Version: 1.3.0
+Summary: A bunch of generic functions and classes useful in multiple projects
 Home-page: https://github.com/smartycope/Cope
 Author: Copeland Carter
 Author-email: smartycope@gmail.com
 Maintainer: Copeland Carter
 Maintainer-email: smartycope@gmail.com
 License: MIT/Apache-2.0
 Classifier: Development Status :: 4 - Beta
@@ -16,16 +17,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires: varname
-Requires: sympy
+Description-Content-Type: text/markdown
+Provides-Extra: linalg
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 
 # Cope
 
 This is my personal "standard library" of all the generally useful code I've written for various projects over the years. Pretty much any time I've written a function or class and thought "this might be useful later", I've stuffed it in here. As such, a lot of it is super useful, a lot of it is garbage, and a lot of it has become obsoleted as I've learned more and found new libraries. I've tried to keep it clean and organized, but there is a lot of it. I also have tests written for a bunch of it, but not all. The debug function in particular I'm especially proud of. I've spent more time than is reasonable on it.
```

### Comparing `Cope-1.2.1/README.md` & `Cope-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/setup.py` & `Cope-1.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,10 +53,8 @@
 }
 
 #################### BEGIN USER OVERRIDES ####################
 # Add your customizations in this section.
 
 ###################### END USER OVERRIDES ####################
 
-setup(**kwargs,
-    requires=['varname', 'sympy'],
-)
+setup(**kwargs, long_description_content_type='text/markdown')
```

### Comparing `Cope-1.2.1/tests/test_colors.py` & `Cope-1.3.0/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/tests/test_decorators.py` & `Cope-1.3.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/tests/test_geometry.py` & `Cope-1.3.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/tests/test_iterables.py` & `Cope-1.3.0/tests/test_iterables.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/tests/test_key.py` & `Cope-1.3.0/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.1/tests/test_misc.py` & `Cope-1.3.0/tests/test_misc.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,33 +51,31 @@
     replaceLine("\t\t# This Line has been replaced! 2")
     replaceLine("# This Line has been replaced! 3")
 
     # replaceLine("\t\t# This Line has been replaced! 1", -1)
     # replaceLine("\t\t# This Line has been replaced! 2")
     # replaceLine("# This Line has been replaced! 3")
 
-
 def test_fancyComment():
-    fancyComment()
-    fancyComment(char='~')
-    fancyComment(lineLimit=30)
-    fancyComment('Seperator!')
-    fancyComment('Seperator!', '~')
-    fancyComment('Seperator!', '~', '{')
-    fancyComment('Seperator!', '~', '{', 50)
+    comment()
+    comment(char='~')
+    comment(lineLimit=30)
+    comment('Seperator!')
+    comment('Seperator!', '~')
+    comment('Seperator!', '~', '{')
+    comment('Seperator!', '~', '{', 50)
 
     # fancyComment()
     # fancyComment(char='~')
     # fancyComment(lineLimit=30)
     # fancyComment('Seperator!')
     # fancyComment('Seperator!', '~')
     # fancyComment('Seperator!', '~', '{')
     # fancyComment('Seperator!', '~', '{', 50)
 
-
 def test_confirm():
     confirm()
 
 def test_slugify():
     slugify()
 
 def test_umpteenthName():
```


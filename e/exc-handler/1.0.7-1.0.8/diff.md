# Comparing `tmp/exc_handler-1.0.7.tar.gz` & `tmp/exc_handler-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exc_handler-1.0.7.tar", last modified: Thu Apr 27 16:03:31 2023, max compression
+gzip compressed data, was "exc_handler-1.0.8.tar", last modified: Thu Apr 27 18:03:12 2023, max compression
```

## Comparing `exc_handler-1.0.7.tar` & `exc_handler-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 16:03:31.860806 exc_handler-1.0.7/
--rw-rw-rw-   0        0        0      427 2023-04-27 16:03:31.858809 exc_handler-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-04-25 13:55:46.000000 exc_handler-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 16:03:31.821830 exc_handler-1.0.7/exc_handler/
--rw-rw-rw-   0        0        0     2389 2023-04-27 16:01:16.000000 exc_handler-1.0.7/exc_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 16:03:31.853811 exc_handler-1.0.7/exc_handler.egg-info/
--rw-rw-rw-   0        0        0      427 2023-04-27 16:03:31.000000 exc_handler-1.0.7/exc_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-27 16:03:31.000000 exc_handler-1.0.7/exc_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 16:03:31.000000 exc_handler-1.0.7/exc_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 16:03:31.000000 exc_handler-1.0.7/exc_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 16:03:31.860806 exc_handler-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-04-27 16:03:22.000000 exc_handler-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:03:12.899907 exc_handler-1.0.8/
+-rw-rw-rw-   0        0        0      427 2023-04-27 18:03:12.895904 exc_handler-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-04-25 13:55:46.000000 exc_handler-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 18:03:12.845937 exc_handler-1.0.8/exc_handler/
+-rw-rw-rw-   0        0        0     2563 2023-04-27 17:49:16.000000 exc_handler-1.0.8/exc_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:03:12.867922 exc_handler-1.0.8/exc_handler.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-04-27 18:03:12.000000 exc_handler-1.0.8/exc_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-27 18:03:12.000000 exc_handler-1.0.8/exc_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 18:03:12.000000 exc_handler-1.0.8/exc_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 18:03:12.000000 exc_handler-1.0.8/exc_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 18:03:12.901903 exc_handler-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-04-27 18:02:55.000000 exc_handler-1.0.8/setup.py
```

### Comparing `exc_handler-1.0.7/README.md` & `exc_handler-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `exc_handler-1.0.7/exc_handler/__init__.py` & `exc_handler-1.0.8/exc_handler/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies:
     - datetime: for getting the date and time of the exception
     - sys: for setting the excepthook
     - traceback: for extracting the traceback info
     - types: for the TracebackType
     - termcolor: for color-coding the stack trace
-    
+
 Usage:
     - Just import this module
 """
 
 
 import sys
 from datetime import datetime as dt
@@ -23,50 +23,58 @@
 from types import TracebackType
 
 from termcolor import colored
 
 def exc_hook(exc: Exception, value = None, tb: TracebackType | None = None) -> str:
 
     """
-    A system exception hook that prints out the details of the exception and its traceback.
+A system exception hook that prints out the details of the exception and its traceback.
 
-    Args:
-        exc (Exception): The exception that needs to be handled.\n
-        value (Optional[Any]): The exception error message. Defaults to None.\n
-        tb (Optional[TracebackType]): The traceback object. Defaults to None.\n
+Args:
+    exc (Exception): The exception that needs to be handled.\n
+    value (Optional[Any]): The exception error message. Defaults to None.\n
+    tb (Optional[TracebackType]): The traceback object. Defaults to None.\n
 
-    Raises:
-        TypeError: If `exc` is not of type `Exception`.
+Raises:
+    TypeError: If `exc` is not of type `Exception`.
 
-    Returns:
-        str: A string containing the current timestamp, the exception name and its error message.
+Returns:
+    str: A string containing the current timestamp, the exception name and its error message.
     """
 
     current_time = dt.strftime(dt.now(), '%d.%m.%Y %H:%M:%S')
 
     if not value or not tb:
         exc_type = type(exc)
 
         if not issubclass(exc_type, Exception):
             raise TypeError(f"exc must be Exception, not {exc_type}")
 
         tb = extract_tb(exc.__traceback__)
 
         frame = exc.__traceback__.tb_frame
         tb = extract_stack(frame)[:-1] + tb
-    
+
         exc = exc.__class__
         value = exc
 
     else:
         tb: StackSummary = extract_tb(tb)
+
     print()
     for frame in tb:
-        raised = colored(f"file '{frame.filename}', line {frame.lineno} in {frame.name}:", 'dark_grey')
-        print(raised, frame.line.strip(), '', sep='\n')
 
+        raised = colored(f"file '{frame.filename}', line {frame.lineno} in {frame.name}:\n", 'dark_grey')
+        print(raised, f'    {frame.line}', sep='')
+
+    with open(frame.filename, 'r') as file:
+        full_line: str = file.readlines()[frame.lineno-1]
+
+    indentation = len(full_line) - len(full_line.lstrip())
+
+    print(" "*(frame.colno-indentation+3), "^")
     message = current_time + ' > ' + colored(f'{exc.__name__}', 'blue') + ': ' + colored(f'{value}', 'red')
     print(message, '\n')
     return f"{exc.__name__}: {value}"
 
 
 sys.excepthook = exc_hook
```

### Comparing `exc_handler-1.0.7/setup.py` & `exc_handler-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 
 Usage:
     - Just import this module
 """
 
 setup(
     name="exc_handler",
-    version="1.0.7",
+    version="1.0.8",
     description=doc,
     author="iineolineii",
     packages=["exc_handler"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
 	]
 )
+
```


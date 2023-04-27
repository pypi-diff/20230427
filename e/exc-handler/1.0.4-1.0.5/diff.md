# Comparing `tmp/exc_handler-1.0.4.tar.gz` & `tmp/exc_handler-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exc_handler-1.0.4.tar", last modified: Tue Apr 25 15:35:43 2023, max compression
+gzip compressed data, was "exc_handler-1.0.5.tar", last modified: Thu Apr 27 12:46:00 2023, max compression
```

## Comparing `exc_handler-1.0.4.tar` & `exc_handler-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 15:35:43.341974 exc_handler-1.0.4/
--rw-rw-rw-   0        0        0      427 2023-04-25 15:35:43.339973 exc_handler-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-04-25 13:55:46.000000 exc_handler-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 15:35:43.302997 exc_handler-1.0.4/exc_handler/
--rw-rw-rw-   0        0        0     1345 2023-04-25 15:34:20.000000 exc_handler-1.0.4/exc_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 15:35:43.336978 exc_handler-1.0.4/exc_handler.egg-info/
--rw-rw-rw-   0        0        0      427 2023-04-25 15:35:43.000000 exc_handler-1.0.4/exc_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-25 15:35:43.000000 exc_handler-1.0.4/exc_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 15:35:43.000000 exc_handler-1.0.4/exc_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-25 15:35:43.000000 exc_handler-1.0.4/exc_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 15:35:43.342974 exc_handler-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1016 2023-04-25 15:34:25.000000 exc_handler-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:46:00.199527 exc_handler-1.0.5/
+-rw-rw-rw-   0        0        0      427 2023-04-27 12:46:00.198536 exc_handler-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-04-25 13:55:46.000000 exc_handler-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 12:46:00.150561 exc_handler-1.0.5/exc_handler/
+-rw-rw-rw-   0        0        0     2389 2023-04-27 12:44:46.000000 exc_handler-1.0.5/exc_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:46:00.188534 exc_handler-1.0.5/exc_handler.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-04-27 12:45:59.000000 exc_handler-1.0.5/exc_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-27 12:46:00.000000 exc_handler-1.0.5/exc_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 12:45:59.000000 exc_handler-1.0.5/exc_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 12:45:59.000000 exc_handler-1.0.5/exc_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 12:46:00.200525 exc_handler-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2023-04-27 12:45:55.000000 exc_handler-1.0.5/setup.py
```

### Comparing `exc_handler-1.0.4/README.md` & `exc_handler-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `exc_handler-1.0.4/exc_handler/__init__.py` & `exc_handler-1.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,31 @@
-"""
+from setuptools import setup
+doc = """
 This module handles exception handling for Python applications. It catches exceptions thrown by the application and prints out a stack trace with color-coded syntax for better readability.\n
 It also displays the date and time the exception occurred, the exception name and value.
 
 Functions:
     - exc_handler(): handles exception thrown by the application
 
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
 
-from datetime import datetime as dt
-import sys
-from traceback import extract_tb, StackSummary
-from types import TracebackType
-from termcolor import colored
-
-def exc_handler(exc: Exception, value, tb: TracebackType):
-
-	current_time = dt.strftime(dt.now(), '%d.%m.%Y %H:%M:%S')
-
-	tb: StackSummary = extract_tb(tb)
-
-	print()
-	for frame in tb:
-		raised = colored(f"file '{frame.filename}', line {frame.lineno}:", 'dark_grey')
-		print(raised, frame.line)
-
-	message = current_time + ' > ' + colored(f'{exc.__name__}', 'blue') + ': ' + colored(f'{value}', 'red')
-	print(message)
-	return f"{exc.__class__.__name__}: {exc}"
-
-sys.excepthook = exc_handler
+setup(
+    name="exc_handler",
+    version="1.0.5",
+    description=doc,
+    author="iineolineii",
+    packages=["exc_handler"],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent"
+	]
+)
```


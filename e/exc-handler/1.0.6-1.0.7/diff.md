# Comparing `tmp/exc_handler-1.0.6.tar.gz` & `tmp/exc_handler-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exc_handler-1.0.6.tar", last modified: Thu Apr 27 15:23:42 2023, max compression
+gzip compressed data, was "exc_handler-1.0.7.tar", last modified: Thu Apr 27 16:03:31 2023, max compression
```

## Comparing `exc_handler-1.0.6.tar` & `exc_handler-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:23:42.800511 exc_handler-1.0.6/
--rw-rw-rw-   0        0        0      427 2023-04-27 15:23:42.798513 exc_handler-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-04-25 13:55:46.000000 exc_handler-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 15:23:42.715565 exc_handler-1.0.6/exc_handler/
--rw-rw-rw-   0        0        0     2573 2023-04-27 15:23:10.000000 exc_handler-1.0.6/exc_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:23:42.795520 exc_handler-1.0.6/exc_handler.egg-info/
--rw-rw-rw-   0        0        0      427 2023-04-27 15:23:41.000000 exc_handler-1.0.6/exc_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-27 15:23:41.000000 exc_handler-1.0.6/exc_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:23:41.000000 exc_handler-1.0.6/exc_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 15:23:41.000000 exc_handler-1.0.6/exc_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 15:23:42.800511 exc_handler-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1016 2023-04-27 15:23:15.000000 exc_handler-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 16:03:31.860806 exc_handler-1.0.7/
+-rw-rw-rw-   0        0        0      427 2023-04-27 16:03:31.858809 exc_handler-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-04-25 13:55:46.000000 exc_handler-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 16:03:31.821830 exc_handler-1.0.7/exc_handler/
+-rw-rw-rw-   0        0        0     2389 2023-04-27 16:01:16.000000 exc_handler-1.0.7/exc_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 16:03:31.853811 exc_handler-1.0.7/exc_handler.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-04-27 16:03:31.000000 exc_handler-1.0.7/exc_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-27 16:03:31.000000 exc_handler-1.0.7/exc_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 16:03:31.000000 exc_handler-1.0.7/exc_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 16:03:31.000000 exc_handler-1.0.7/exc_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 16:03:31.860806 exc_handler-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-04-27 16:03:22.000000 exc_handler-1.0.7/setup.py
```

### Comparing `exc_handler-1.0.6/README.md` & `exc_handler-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `exc_handler-1.0.6/exc_handler/__init__.py` & `exc_handler-1.0.7/exc_handler/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,34 +45,28 @@
 
     if not value or not tb:
         exc_type = type(exc)
 
         if not issubclass(exc_type, Exception):
             raise TypeError(f"exc must be Exception, not {exc_type}")
 
-        tb = extract_stack(frame)[:-1] + extract_tb(exc.__traceback__)
+        tb = extract_tb(exc.__traceback__)
+
+        frame = exc.__traceback__.tb_frame
+        tb = extract_stack(frame)[:-1] + tb
     
         exc = exc.__class__
         value = exc
 
     else:
         tb: StackSummary = extract_tb(tb)
-
     print()
     for frame in tb:
-        
-        with open(frame.filename, 'r') as file:
-            full_line: str = file.readlines()[frame.lineno-1]
-
-        indentation = len(full_line) - len(full_line.lstrip())
-
         raised = colored(f"file '{frame.filename}', line {frame.lineno} in {frame.name}:", 'dark_grey')
-        print(raised, f"    {frame.line}", sep='\n')
-
-    print(" "*(frame.colno-indentation+4)+'^')
+        print(raised, frame.line.strip(), '', sep='\n')
 
     message = current_time + ' > ' + colored(f'{exc.__name__}', 'blue') + ': ' + colored(f'{value}', 'red')
-    print(message, '\n', sep='')
+    print(message, '\n')
     return f"{exc.__name__}: {value}"
 
 
 sys.excepthook = exc_hook
```

### Comparing `exc_handler-1.0.6/setup.py` & `exc_handler-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from setuptools import setup
+
 doc = """
 This module handles exception handling for Python applications. It catches exceptions thrown by the application and prints out a stack trace with color-coded syntax for better readability.\n
 It also displays the date and time the exception occurred, the exception name and value.
 
 Functions:
     - exc_handler(): handles exception thrown by the application
 
@@ -15,15 +16,15 @@
 
 Usage:
     - Just import this module
 """
 
 setup(
     name="exc_handler",
-    version="1.0.6",
+    version="1.0.7",
     description=doc,
     author="iineolineii",
     packages=["exc_handler"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
```


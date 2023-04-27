# Comparing `tmp/exc_handler-1.0.5.tar.gz` & `tmp/exc_handler-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exc_handler-1.0.5.tar", last modified: Thu Apr 27 12:46:00 2023, max compression
+gzip compressed data, was "exc_handler-1.0.6.tar", last modified: Thu Apr 27 15:23:42 2023, max compression
```

## Comparing `exc_handler-1.0.5.tar` & `exc_handler-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:46:00.199527 exc_handler-1.0.5/
--rw-rw-rw-   0        0        0      427 2023-04-27 12:46:00.198536 exc_handler-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-04-25 13:55:46.000000 exc_handler-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 12:46:00.150561 exc_handler-1.0.5/exc_handler/
--rw-rw-rw-   0        0        0     2389 2023-04-27 12:44:46.000000 exc_handler-1.0.5/exc_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:46:00.188534 exc_handler-1.0.5/exc_handler.egg-info/
--rw-rw-rw-   0        0        0      427 2023-04-27 12:45:59.000000 exc_handler-1.0.5/exc_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-27 12:46:00.000000 exc_handler-1.0.5/exc_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:45:59.000000 exc_handler-1.0.5/exc_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 12:45:59.000000 exc_handler-1.0.5/exc_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 12:46:00.200525 exc_handler-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1016 2023-04-27 12:45:55.000000 exc_handler-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:23:42.800511 exc_handler-1.0.6/
+-rw-rw-rw-   0        0        0      427 2023-04-27 15:23:42.798513 exc_handler-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-04-25 13:55:46.000000 exc_handler-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 15:23:42.715565 exc_handler-1.0.6/exc_handler/
+-rw-rw-rw-   0        0        0     2573 2023-04-27 15:23:10.000000 exc_handler-1.0.6/exc_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:23:42.795520 exc_handler-1.0.6/exc_handler.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-04-27 15:23:41.000000 exc_handler-1.0.6/exc_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-27 15:23:41.000000 exc_handler-1.0.6/exc_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 15:23:41.000000 exc_handler-1.0.6/exc_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 15:23:41.000000 exc_handler-1.0.6/exc_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 15:23:42.800511 exc_handler-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2023-04-27 15:23:15.000000 exc_handler-1.0.6/setup.py
```

### Comparing `exc_handler-1.0.5/README.md` & `exc_handler-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `exc_handler-1.0.5/exc_handler/__init__.py` & `exc_handler-1.0.6/exc_handler/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,28 +45,34 @@
 
     if not value or not tb:
         exc_type = type(exc)
 
         if not issubclass(exc_type, Exception):
             raise TypeError(f"exc must be Exception, not {exc_type}")
 
-        tb = extract_tb(exc.__traceback__)
-
-        frame = exc.__traceback__.tb_frame
-        tb = extract_stack(frame)[:-1] + tb
+        tb = extract_stack(frame)[:-1] + extract_tb(exc.__traceback__)
     
         exc = exc.__class__
         value = exc
 
     else:
         tb: StackSummary = extract_tb(tb)
+
     print()
     for frame in tb:
+        
+        with open(frame.filename, 'r') as file:
+            full_line: str = file.readlines()[frame.lineno-1]
+
+        indentation = len(full_line) - len(full_line.lstrip())
+
         raised = colored(f"file '{frame.filename}', line {frame.lineno} in {frame.name}:", 'dark_grey')
-        print(raised, frame.line.strip(), '', sep='\n')
+        print(raised, f"    {frame.line}", sep='\n')
+
+    print(" "*(frame.colno-indentation+4)+'^')
 
     message = current_time + ' > ' + colored(f'{exc.__name__}', 'blue') + ': ' + colored(f'{value}', 'red')
-    print(message, '\n')
+    print(message, '\n', sep='')
     return f"{exc.__name__}: {value}"
 
 
 sys.excepthook = exc_hook
```

### Comparing `exc_handler-1.0.5/setup.py` & `exc_handler-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 Usage:
     - Just import this module
 """
 
 setup(
     name="exc_handler",
-    version="1.0.5",
+    version="1.0.6",
     description=doc,
     author="iineolineii",
     packages=["exc_handler"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
```


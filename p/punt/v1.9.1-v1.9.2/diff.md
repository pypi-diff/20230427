# Comparing `tmp/punt-v1.9.1.tar.gz` & `tmp/punt-v1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/punt-v1.9.1.tar", last modified: Thu Feb  4 18:56:40 2016, max compression
+gzip compressed data, was "dist/punt-v1.9.2.tar", last modified: Thu Feb  4 19:18:10 2016, max compression
```

## Comparing `punt-v1.9.1.tar` & `punt-v1.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 colinta    (501) staff       (20)        0 2016-02-04 18:56:40.000000 punt-v1.9.1/
--rw-r--r--   0 colinta    (501) staff       (20)     1516 2012-07-06 17:16:41.000000 punt-v1.9.1/LICENSE
--rw-r--r--   0 colinta    (501) staff       (20)       35 2012-07-06 17:30:11.000000 punt-v1.9.1/MANIFEST.in
--rw-r--r--   0 colinta    (501) staff       (20)     2317 2016-02-04 18:56:40.000000 punt-v1.9.1/PKG-INFO
-drwxr-xr-x   0 colinta    (501) staff       (20)        0 2016-02-04 18:56:40.000000 punt-v1.9.1/punt/
--rw-r--r--   0 colinta    (501) staff       (20)     2620 2016-02-04 18:55:06.000000 punt-v1.9.1/punt/__init__.py
-drwxr-xr-x   0 colinta    (501) staff       (20)        0 2016-02-04 18:56:40.000000 punt-v1.9.1/punt.egg-info/
--rw-r--r--   0 colinta    (501) staff       (20)        1 2016-02-04 18:56:40.000000 punt-v1.9.1/punt.egg-info/dependency_links.txt
--rw-r--r--   0 colinta    (501) staff       (20)       35 2016-02-04 18:56:40.000000 punt-v1.9.1/punt.egg-info/entry_points.txt
--rw-r--r--   0 colinta    (501) staff       (20)       47 2016-02-04 18:56:40.000000 punt-v1.9.1/punt.egg-info/pbr.json
--rw-r--r--   0 colinta    (501) staff       (20)     2317 2016-02-04 18:56:40.000000 punt-v1.9.1/punt.egg-info/PKG-INFO
--rw-r--r--   0 colinta    (501) staff       (20)       15 2016-02-04 18:56:40.000000 punt-v1.9.1/punt.egg-info/requires.txt
--rw-r--r--   0 colinta    (501) staff       (20)      249 2016-02-04 18:56:40.000000 punt-v1.9.1/punt.egg-info/SOURCES.txt
--rw-r--r--   0 colinta    (501) staff       (20)        5 2016-02-04 18:56:40.000000 punt-v1.9.1/punt.egg-info/top_level.txt
--rw-r--r--   0 colinta    (501) staff       (20)     1210 2012-08-13 18:21:13.000000 punt-v1.9.1/README.rst
--rw-r--r--   0 colinta    (501) staff       (20)       59 2016-02-04 18:56:40.000000 punt-v1.9.1/setup.cfg
--rw-r--r--   0 colinta    (501) staff       (20)     1233 2016-02-04 18:55:10.000000 punt-v1.9.1/setup.py
+drwxr-xr-x   0 colinta    (501) staff       (20)        0 2016-02-04 19:18:10.000000 punt-v1.9.2/
+-rw-r--r--   0 colinta    (501) staff       (20)     1516 2012-07-06 17:16:41.000000 punt-v1.9.2/LICENSE
+-rw-r--r--   0 colinta    (501) staff       (20)       35 2012-07-06 17:30:11.000000 punt-v1.9.2/MANIFEST.in
+-rw-r--r--   0 colinta    (501) staff       (20)     2317 2016-02-04 19:18:10.000000 punt-v1.9.2/PKG-INFO
+drwxr-xr-x   0 colinta    (501) staff       (20)        0 2016-02-04 19:18:10.000000 punt-v1.9.2/punt/
+-rw-r--r--   0 colinta    (501) staff       (20)     2841 2016-02-04 19:17:28.000000 punt-v1.9.2/punt/__init__.py
+drwxr-xr-x   0 colinta    (501) staff       (20)        0 2016-02-04 19:18:10.000000 punt-v1.9.2/punt.egg-info/
+-rw-r--r--   0 colinta    (501) staff       (20)        1 2016-02-04 19:18:09.000000 punt-v1.9.2/punt.egg-info/dependency_links.txt
+-rw-r--r--   0 colinta    (501) staff       (20)       35 2016-02-04 19:18:09.000000 punt-v1.9.2/punt.egg-info/entry_points.txt
+-rw-r--r--   0 colinta    (501) staff       (20)       47 2016-02-04 19:18:09.000000 punt-v1.9.2/punt.egg-info/pbr.json
+-rw-r--r--   0 colinta    (501) staff       (20)     2317 2016-02-04 19:18:09.000000 punt-v1.9.2/punt.egg-info/PKG-INFO
+-rw-r--r--   0 colinta    (501) staff       (20)       15 2016-02-04 19:18:09.000000 punt-v1.9.2/punt.egg-info/requires.txt
+-rw-r--r--   0 colinta    (501) staff       (20)      249 2016-02-04 19:18:10.000000 punt-v1.9.2/punt.egg-info/SOURCES.txt
+-rw-r--r--   0 colinta    (501) staff       (20)        5 2016-02-04 19:18:09.000000 punt-v1.9.2/punt.egg-info/top_level.txt
+-rw-r--r--   0 colinta    (501) staff       (20)     1210 2012-08-13 18:21:13.000000 punt-v1.9.2/README.rst
+-rw-r--r--   0 colinta    (501) staff       (20)       59 2016-02-04 19:18:10.000000 punt-v1.9.2/setup.cfg
+-rw-r--r--   0 colinta    (501) staff       (20)     1233 2016-02-04 19:15:26.000000 punt-v1.9.2/setup.py
```

### Comparing `punt-v1.9.1/LICENSE` & `punt-v1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `punt-v1.9.1/PKG-INFO` & `punt-v1.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: punt
-Version: v1.9.1
+Version: v1.9.2
 Summary: Monitor file changes, and run script on changes.
 Home-page: https://github.com/colinta/punt
 Author: Colin T.A. Gray
 Author-email: colinta@gmail.com
 License: BSD
 Description: ====
         punt
```

### Comparing `punt-v1.9.1/punt/__init__.py` & `punt-v1.9.2/punt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,30 +18,37 @@
 import traceback
 from subprocess import call
 
 from docopt import docopt
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 
+import pkg_resources  # part of setuptools
+version = pkg_resources.require("punt")[0].version
+
 
 def run():
-    arguments = docopt(__doc__, version='punt v1.9.1')
+    arguments = docopt(__doc__, version='punt ' + version)
 
     if not arguments['-w']:
         watch_paths = [os.getcwd()]
     else:
         watch_paths = []
         for watch in arguments['-w']:
             watch = os.path.abspath(watch)
             if not os.path.isdir(watch):
                 sys.stderr.write("Error: {watch} does not exist".format(watch=watch))
             watch_paths.append(watch)
 
     recursive = not arguments['-l']
-    timeout = arguments['-t']
+    try:
+        timeout = float(arguments['-t'])
+    except ValueError:
+        sys.stderr.write("Error: 'timeout' must be a number\n")
+        return
     commands = arguments['<commands>']
 
     class Regenerate(FileSystemEventHandler):
         last_run = None
 
         def on_any_event(self, event, alert=True):
             if self.last_run and time.time() - self.last_run < timeout:
```

### Comparing `punt-v1.9.1/punt.egg-info/PKG-INFO` & `punt-v1.9.2/punt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: punt
-Version: v1.9.1
+Version: v1.9.2
 Summary: Monitor file changes, and run script on changes.
 Home-page: https://github.com/colinta/punt
 Author: Colin T.A. Gray
 Author-email: colinta@gmail.com
 License: BSD
 Description: ====
         punt
```

### Comparing `punt-v1.9.1/README.rst` & `punt-v1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `punt-v1.9.1/setup.py` & `punt-v1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
         name="punt",
-        version="v1.9.1",
+        version="v1.9.2",
         author="Colin T.A. Gray",
         author_email="colinta@gmail.com",
         url="https://github.com/colinta/punt",
         install_requires=['docopt', 'watchdog'],
 
         entry_points={
             'console_scripts': [
```


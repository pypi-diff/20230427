# Comparing `tmp/ErCore-1.0.tar.gz` & `tmp/ErCore-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ErCore-1.0.tar", last modified: Tue Apr 25 04:31:02 2023, max compression
+gzip compressed data, was "ErCore-1.1.tar", last modified: Thu Apr 27 08:53:07 2023, max compression
```

## Comparing `ErCore-1.0.tar` & `ErCore-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 04:31:02.593178 ErCore-1.0/
-drwxrwxrwx   0        0        0        0 2023-04-25 04:31:02.568179 ErCore-1.0/ErCore/
--rw-rw-rw-   0        0        0     2101 2023-04-25 04:23:54.000000 ErCore-1.0/ErCore/Core.py
--rw-rw-rw-   0        0        0       33 2023-03-30 02:42:05.000000 ErCore-1.0/ErCore/__init__.py
--rw-rw-rw-   0        0        0     3188 2023-04-25 04:23:54.000000 ErCore-1.0/ErCore/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-25 04:31:02.590179 ErCore-1.0/ErCore/std/
--rw-rw-rw-   0        0        0      375 2023-04-25 04:21:27.000000 ErCore-1.0/ErCore/std/Base.py
--rw-rw-rw-   0        0        0       33 2023-04-25 04:21:27.000000 ErCore-1.0/ErCore/std/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 04:31:02.588191 ErCore-1.0/ErCore.egg-info/
--rw-rw-rw-   0        0        0      475 2023-04-25 04:31:02.000000 ErCore-1.0/ErCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-25 04:31:02.000000 ErCore-1.0/ErCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 04:31:02.000000 ErCore-1.0/ErCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-04-25 04:31:02.000000 ErCore-1.0/ErCore.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-25 04:31:02.000000 ErCore-1.0/ErCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-04-21 12:30:11.000000 ErCore-1.0/LICENSE
--rw-rw-rw-   0        0        0      475 2023-04-25 04:31:02.592178 ErCore-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-04-25 04:23:54.000000 ErCore-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 04:31:02.593178 ErCore-1.0/setup.cfg
--rw-rw-rw-   0        0        0      679 2023-04-21 12:03:04.000000 ErCore-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:53:07.560261 ErCore-1.1/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:53:07.516245 ErCore-1.1/ErCore/
+-rw-rw-rw-   0        0        0     2114 2023-04-27 08:34:53.000000 ErCore-1.1/ErCore/Core.py
+-rw-rw-rw-   0        0        0       70 2023-04-26 11:12:02.000000 ErCore-1.1/ErCore/__init__.py
+-rw-rw-rw-   0        0        0     3190 2023-04-27 08:26:30.000000 ErCore-1.1/ErCore/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:53:07.557245 ErCore-1.1/ErCore/std/
+-rw-rw-rw-   0        0        0      375 2023-04-25 04:21:27.000000 ErCore-1.1/ErCore/std/Base.py
+-rw-rw-rw-   0        0        0       33 2023-04-25 04:21:27.000000 ErCore-1.1/ErCore/std/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:53:07.530244 ErCore-1.1/ErCore.egg-info/
+-rw-rw-rw-   0        0        0      475 2023-04-27 08:53:07.000000 ErCore-1.1/ErCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-27 08:53:07.000000 ErCore-1.1/ErCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 08:53:07.000000 ErCore-1.1/ErCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-27 08:53:07.000000 ErCore-1.1/ErCore.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 08:53:07.000000 ErCore-1.1/ErCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-04-21 12:30:11.000000 ErCore-1.1/LICENSE
+-rw-rw-rw-   0        0        0      475 2023-04-27 08:53:07.560261 ErCore-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-04-27 08:27:25.000000 ErCore-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 08:53:07.561244 ErCore-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      679 2023-04-27 08:26:47.000000 ErCore-1.1/setup.py
```

### Comparing `ErCore-1.0/ErCore/Core.py` & `ErCore-1.1/ErCore/Core.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import platform
 
 from std import colors, style
 
 
 class ECore:
     def __init__(self):
-        self.version = 1.0
+        self.version = 1.1
         self.IS_WINDOWS = (platform.system() == 'Windows')
         self.IS_LINUX = (platform.system() == 'Linux')
         self.IS_MAC = (platform.system() == 'Darwin')
 
     def info(self):
         try:
             print(f'Autor: Eragod\nProject: ErCore\nVersion: {self.version}')
@@ -25,15 +25,16 @@
         if self.IS_LINUX:
             with open(f'run.sh', 'w') as runner:
                 runner.write(f'#!/bin/bash\n\npython3 {file}.py')
         if self.IS_MAC:
             with open(f'run.sh', 'w') as runner:
                 runner.write(f'#!/bin/bash\n\npython3 {file}.py')
 
-    def logger(self, function):
+    @staticmethod
+    def logger(function):
         try:
             if function is not None:
                 second = time.localtime().tm_sec
                 minute = time.localtime().tm_min
                 hour = time.localtime().tm_hour
                 print(f'{style["BOLD"]}{colors["Red"]}{hour}:{minute}:{second}:{colors["Reset"]}',
                       f'{function.__name__} Start work!')
```

### Comparing `ErCore-1.0/ErCore/cli.py` & `ErCore-1.1/ErCore/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-import datetime
+import time
 import platform
 
 from std import colors
 
 
 def make_project():
     try:
@@ -20,15 +20,15 @@
             with open('main.py', 'w') as py:
                 py.write(f'# {name}\ndef main(name):\n    print("Hello " + name)')
         if license.lower() == 'y':
             print('only MIT work')
             license_type = str(input('Enter license type:'))
             if license_type.lower() == 'mit':
                 mit_l = f"""MIT License
-                Copyright © {datetime.date.year} {name}
+                Copyright © {time.localtime().tm_year} {name}
                 Permission is hereby granted, free of charge, to any person obtaining a copy of this software
                 and associated documentation files (the “Software”), to deal in the Software without
                 restriction, including without limitation the rights to use, copy, modify, merge, publish,
                 distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the
                 Software is furnished to do so, subject to the following conditions:
 
                 The above copyright notice and this permission notice shall be included in all copies or
```

### Comparing `ErCore-1.0/LICENSE` & `ErCore-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ErCore-1.0/setup.py` & `ErCore-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ErCore',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     author='Eragod',
     description='Core for projects',
     url="https://github.com/Eragod/ErCore",
     long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     entry_points={'console_scripts': ['ErCore-project = ErCore.cli:make_project',
```


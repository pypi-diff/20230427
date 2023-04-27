# Comparing `tmp/efshape-0.1.0.tar.gz` & `tmp/efshape-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efshape-0.1.0.tar", last modified: Thu Apr 27 10:52:50 2023, max compression
+gzip compressed data, was "efshape-0.1.1.tar", last modified: Thu Apr 27 10:56:21 2023, max compression
```

## Comparing `efshape-0.1.0.tar` & `efshape-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:52:50.149411 efshape-0.1.0/
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       52 2023-04-22 02:05:01.000000 efshape-0.1.0/MANIFEST.in
-drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:52:50.149411 efshape-0.1.0/Main/
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)        6 2023-04-22 02:05:01.000000 efshape-0.1.0/Main/__init__.py
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1652 2023-04-27 10:52:50.149411 efshape-0.1.0/PKG-INFO
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1171 2023-04-22 02:05:01.000000 efshape-0.1.0/README.md
-drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:52:50.149411 efshape-0.1.0/efshape/
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       31 2023-04-22 02:05:01.000000 efshape-0.1.0/efshape/__init__.py
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    33057 2023-04-23 15:21:35.000000 efshape-0.1.0/efshape/efa.py
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    88190 2023-04-27 10:31:20.000000 efshape-0.1.0/efshape/efgui.py
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    85967 2023-04-27 10:36:23.000000 efshape-0.1.0/efshape/fgui.py
-drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:52:50.149411 efshape-0.1.0/efshape.egg-info/
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1652 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/PKG-INFO
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      303 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/SOURCES.txt
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)        1 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/dependency_links.txt
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      107 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/entry_points.txt
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      133 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/requires.txt
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       13 2023-04-27 10:52:50.000000 efshape-0.1.0/efshape.egg-info/top_level.txt
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       38 2023-04-27 10:52:50.149411 efshape-0.1.0/setup.cfg
--rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1687 2023-04-27 10:47:25.000000 efshape-0.1.0/setup.py
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:56:21.344350 efshape-0.1.1/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       52 2023-04-22 02:05:01.000000 efshape-0.1.1/MANIFEST.in
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:56:21.340350 efshape-0.1.1/Main/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)        6 2023-04-22 02:05:01.000000 efshape-0.1.1/Main/__init__.py
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1652 2023-04-27 10:56:21.340350 efshape-0.1.1/PKG-INFO
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1171 2023-04-22 02:05:01.000000 efshape-0.1.1/README.md
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:56:21.340350 efshape-0.1.1/efshape/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       31 2023-04-22 02:05:01.000000 efshape-0.1.1/efshape/__init__.py
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    33057 2023-04-27 10:55:57.000000 efshape-0.1.1/efshape/efa.py
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    88178 2023-04-27 10:55:52.000000 efshape-0.1.1/efshape/efgui.py
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    85967 2023-04-27 10:36:23.000000 efshape-0.1.1/efshape/fgui.py
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-04-27 10:56:21.340350 efshape-0.1.1/efshape.egg-info/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1652 2023-04-27 10:56:21.000000 efshape-0.1.1/efshape.egg-info/PKG-INFO
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      303 2023-04-27 10:56:21.000000 efshape-0.1.1/efshape.egg-info/SOURCES.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)        1 2023-04-27 10:56:21.000000 efshape-0.1.1/efshape.egg-info/dependency_links.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      107 2023-04-27 10:56:21.000000 efshape-0.1.1/efshape.egg-info/entry_points.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      133 2023-04-27 10:56:21.000000 efshape-0.1.1/efshape.egg-info/requires.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       13 2023-04-27 10:56:21.000000 efshape-0.1.1/efshape.egg-info/top_level.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       38 2023-04-27 10:56:21.344350 efshape-0.1.1/setup.cfg
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1687 2023-04-27 10:56:18.000000 efshape-0.1.1/setup.py
```

### Comparing `efshape-0.1.0/PKG-INFO` & `efshape-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efshape
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package Dependency: Validates package requirements
 Home-page: https://github.com/SojiroFukuda/efshape
 Author: SojiroFukuda
 Author-email: S.Fukuda-2018@hull.ac.uk
 Maintainer: SojiroFukuda
 Maintainer-email: S.Fukuda-2018@hull.ac.uk
 License: SojiroFukuda
```

### Comparing `efshape-0.1.0/README.md` & `efshape-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `efshape-0.1.0/efshape/efa.py` & `efshape-0.1.1/efshape/efa.py`

 * *Files identical despite different names*

### Comparing `efshape-0.1.0/efshape/efgui.py` & `efshape-0.1.1/efshape/efgui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1612,10 +1612,8 @@
         self.fig32.savefig(file_name+"fig_32.pdf",bbox_inches='tight')
         self.fig33.savefig(file_name+"fig_33.pdf",bbox_inches='tight')
    
 def buildGUI():
     app = Qw.QApplication(sys.argv)         
     wmain = MyForm()                        
     wmain.show()                            
-    sys.exit(app.exec())
-
-buildGUI()
+    sys.exit(app.exec())
```

### Comparing `efshape-0.1.0/efshape/fgui.py` & `efshape-0.1.1/efshape/fgui.py`

 * *Files identical despite different names*

### Comparing `efshape-0.1.0/efshape.egg-info/PKG-INFO` & `efshape-0.1.1/efshape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efshape
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package Dependency: Validates package requirements
 Home-page: https://github.com/SojiroFukuda/efshape
 Author: SojiroFukuda
 Author-email: S.Fukuda-2018@hull.ac.uk
 Maintainer: SojiroFukuda
 Maintainer-email: S.Fukuda-2018@hull.ac.uk
 License: SojiroFukuda
```

### Comparing `efshape-0.1.0/setup.py` & `efshape-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # version
 here = os.path.dirname(os.path.abspath(__file__))
 version = next((line.split('=')[1].strip().replace("'", '')
                 for line in open(os.path.join(here,
                                               'efshape',
                                               '__init__.py'))
-                if line.startswith('__version__ = ')),'0.1.0')
+                if line.startswith('__version__ = ')),'0.1.1')
 
 
 setup(
     name="efshape",
     version=version,
     url='https://github.com/SojiroFukuda/efshape',
     author='SojiroFukuda',
```


# Comparing `tmp/QTNOME_P-Y-R-O-B-O-T-1.0.4.tar.gz` & `tmp/QTNOME_P-Y-R-O-B-O-T-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QTNOME_P-Y-R-O-B-O-T-1.0.4.tar", last modified: Thu Apr 27 04:09:41 2023, max compression
+gzip compressed data, was "QTNOME_P-Y-R-O-B-O-T-1.0.5.tar", last modified: Thu Apr 27 04:14:20 2023, max compression
```

## Comparing `QTNOME_P-Y-R-O-B-O-T-1.0.4.tar` & `QTNOME_P-Y-R-O-B-O-T-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-04-27 04:09:41.341461 QTNOME_P-Y-R-O-B-O-T-1.0.4/
--rw-rw-r--   0 kushal    (1000) kushal    (1000)    35156 2023-03-18 12:52:16.000000 QTNOME_P-Y-R-O-B-O-T-1.0.4/LICENSE
--rw-rw-r--   0 kushal    (1000) kushal    (1000)    45643 2023-04-27 04:09:41.341461 QTNOME_P-Y-R-O-B-O-T-1.0.4/PKG-INFO
-drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-04-27 04:09:41.341461 QTNOME_P-Y-R-O-B-O-T-1.0.4/QTNOME/
--rw-rw-r--   0 kushal    (1000) kushal    (1000)    14740 2023-04-27 04:03:48.000000 QTNOME_P-Y-R-O-B-O-T-1.0.4/QTNOME/QTNOME.py
-drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-04-27 04:09:41.341461 QTNOME_P-Y-R-O-B-O-T-1.0.4/QTNOME_P_Y_R_O_B_O_T.egg-info/
--rw-rw-r--   0 kushal    (1000) kushal    (1000)    45643 2023-04-27 04:09:41.000000 QTNOME_P-Y-R-O-B-O-T-1.0.4/QTNOME_P_Y_R_O_B_O_T.egg-info/PKG-INFO
--rw-rw-r--   0 kushal    (1000) kushal    (1000)      268 2023-04-27 04:09:41.000000 QTNOME_P-Y-R-O-B-O-T-1.0.4/QTNOME_P_Y_R_O_B_O_T.egg-info/SOURCES.txt
--rw-rw-r--   0 kushal    (1000) kushal    (1000)        1 2023-04-27 04:09:41.000000 QTNOME_P-Y-R-O-B-O-T-1.0.4/QTNOME_P_Y_R_O_B_O_T.egg-info/dependency_links.txt
--rw-rw-r--   0 kushal    (1000) kushal    (1000)        6 2023-04-27 04:09:41.000000 QTNOME_P-Y-R-O-B-O-T-1.0.4/QTNOME_P_Y_R_O_B_O_T.egg-info/requires.txt
--rw-rw-r--   0 kushal    (1000) kushal    (1000)        7 2023-04-27 04:09:41.000000 QTNOME_P-Y-R-O-B-O-T-1.0.4/QTNOME_P_Y_R_O_B_O_T.egg-info/top_level.txt
--rw-rw-r--   0 kushal    (1000) kushal    (1000)     4706 2023-04-27 04:05:21.000000 QTNOME_P-Y-R-O-B-O-T-1.0.4/README.md
--rw-rw-r--   0 kushal    (1000) kushal    (1000)      549 2023-04-27 04:05:51.000000 QTNOME_P-Y-R-O-B-O-T-1.0.4/pyproject.toml
--rw-rw-r--   0 kushal    (1000) kushal    (1000)       38 2023-04-27 04:09:41.341461 QTNOME_P-Y-R-O-B-O-T-1.0.4/setup.cfg
+drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-04-27 04:14:20.544287 QTNOME_P-Y-R-O-B-O-T-1.0.5/
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)    35156 2023-03-18 12:52:16.000000 QTNOME_P-Y-R-O-B-O-T-1.0.5/LICENSE
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)    45649 2023-04-27 04:14:20.544287 QTNOME_P-Y-R-O-B-O-T-1.0.5/PKG-INFO
+drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-04-27 04:14:20.544287 QTNOME_P-Y-R-O-B-O-T-1.0.5/QTNOME/
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)    14740 2023-04-27 04:03:48.000000 QTNOME_P-Y-R-O-B-O-T-1.0.5/QTNOME/QTNOME.py
+drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-04-27 04:14:20.544287 QTNOME_P-Y-R-O-B-O-T-1.0.5/QTNOME_P_Y_R_O_B_O_T.egg-info/
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)    45649 2023-04-27 04:14:20.000000 QTNOME_P-Y-R-O-B-O-T-1.0.5/QTNOME_P_Y_R_O_B_O_T.egg-info/PKG-INFO
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)      268 2023-04-27 04:14:20.000000 QTNOME_P-Y-R-O-B-O-T-1.0.5/QTNOME_P_Y_R_O_B_O_T.egg-info/SOURCES.txt
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)        1 2023-04-27 04:14:20.000000 QTNOME_P-Y-R-O-B-O-T-1.0.5/QTNOME_P_Y_R_O_B_O_T.egg-info/dependency_links.txt
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)        6 2023-04-27 04:14:20.000000 QTNOME_P-Y-R-O-B-O-T-1.0.5/QTNOME_P_Y_R_O_B_O_T.egg-info/requires.txt
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)        7 2023-04-27 04:14:20.000000 QTNOME_P-Y-R-O-B-O-T-1.0.5/QTNOME_P_Y_R_O_B_O_T.egg-info/top_level.txt
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)     4712 2023-04-27 04:12:02.000000 QTNOME_P-Y-R-O-B-O-T-1.0.5/README.md
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)      549 2023-04-27 04:13:10.000000 QTNOME_P-Y-R-O-B-O-T-1.0.5/pyproject.toml
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)       38 2023-04-27 04:14:20.544287 QTNOME_P-Y-R-O-B-O-T-1.0.5/setup.cfg
```

### Comparing `QTNOME_P-Y-R-O-B-O-T-1.0.4/LICENSE` & `QTNOME_P-Y-R-O-B-O-T-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `QTNOME_P-Y-R-O-B-O-T-1.0.4/PKG-INFO` & `QTNOME_P-Y-R-O-B-O-T-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QTNOME_P-Y-R-O-B-O-T
-Version: 1.0.4
+Version: 1.0.5
 Summary: An multiwindowed application envirement made in PyQt
 Author-email: KUSHAL <NONE@NONE.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -768,21 +768,21 @@
 
 class WIN(QTNOME.WINDOW) :
     def __init__(self, parent, xi, yi, width, height) :
         super().__init__(parent)
         self.setGeometry(xi, yi, width, height)
 
 def on_exit() :
-	print("[ # ] Exiting the application...")
+    print("[ # ] Exiting the application...")
 
 if __name__ == "__main__" :
     from random import randint
 
     QTNOME.INIT_UI()
-	QTNOME.INTERFACE_ENVIREMENT.add_on_exit(on_exit)
+    QTNOME.INTERFACE_ENVIREMENT.add_on_exit(on_exit)
 
     for _ in range(10) :
         randcolors = [randint(0, 255), randint(0, 255), randint(0, 255)]
         WI = QTNOME.CREATE_WINDOW([WIN, {"xi": randint(0, QtWidgets.QDesktopWidget().screenGeometry(-1).width() - 500),
                                   "yi": randint(0, QtWidgets.QDesktopWidget().screenGeometry(-1).height() - 300),
                                   "width": randint(0, 400), "height": randint(0, 250)}],
                                   name = str(_),
```

### Comparing `QTNOME_P-Y-R-O-B-O-T-1.0.4/QTNOME/QTNOME.py` & `QTNOME_P-Y-R-O-B-O-T-1.0.5/QTNOME/QTNOME.py`

 * *Files identical despite different names*

### Comparing `QTNOME_P-Y-R-O-B-O-T-1.0.4/QTNOME_P_Y_R_O_B_O_T.egg-info/PKG-INFO` & `QTNOME_P-Y-R-O-B-O-T-1.0.5/QTNOME_P_Y_R_O_B_O_T.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QTNOME-P-Y-R-O-B-O-T
-Version: 1.0.4
+Version: 1.0.5
 Summary: An multiwindowed application envirement made in PyQt
 Author-email: KUSHAL <NONE@NONE.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -768,21 +768,21 @@
 
 class WIN(QTNOME.WINDOW) :
     def __init__(self, parent, xi, yi, width, height) :
         super().__init__(parent)
         self.setGeometry(xi, yi, width, height)
 
 def on_exit() :
-	print("[ # ] Exiting the application...")
+    print("[ # ] Exiting the application...")
 
 if __name__ == "__main__" :
     from random import randint
 
     QTNOME.INIT_UI()
-	QTNOME.INTERFACE_ENVIREMENT.add_on_exit(on_exit)
+    QTNOME.INTERFACE_ENVIREMENT.add_on_exit(on_exit)
 
     for _ in range(10) :
         randcolors = [randint(0, 255), randint(0, 255), randint(0, 255)]
         WI = QTNOME.CREATE_WINDOW([WIN, {"xi": randint(0, QtWidgets.QDesktopWidget().screenGeometry(-1).width() - 500),
                                   "yi": randint(0, QtWidgets.QDesktopWidget().screenGeometry(-1).height() - 300),
                                   "width": randint(0, 400), "height": randint(0, 250)}],
                                   name = str(_),
```

### Comparing `QTNOME_P-Y-R-O-B-O-T-1.0.4/README.md` & `QTNOME_P-Y-R-O-B-O-T-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -82,21 +82,21 @@
 
 class WIN(QTNOME.WINDOW) :
     def __init__(self, parent, xi, yi, width, height) :
         super().__init__(parent)
         self.setGeometry(xi, yi, width, height)
 
 def on_exit() :
-	print("[ # ] Exiting the application...")
+    print("[ # ] Exiting the application...")
 
 if __name__ == "__main__" :
     from random import randint
 
     QTNOME.INIT_UI()
-	QTNOME.INTERFACE_ENVIREMENT.add_on_exit(on_exit)
+    QTNOME.INTERFACE_ENVIREMENT.add_on_exit(on_exit)
 
     for _ in range(10) :
         randcolors = [randint(0, 255), randint(0, 255), randint(0, 255)]
         WI = QTNOME.CREATE_WINDOW([WIN, {"xi": randint(0, QtWidgets.QDesktopWidget().screenGeometry(-1).width() - 500),
                                   "yi": randint(0, QtWidgets.QDesktopWidget().screenGeometry(-1).height() - 300),
                                   "width": randint(0, 400), "height": randint(0, 250)}],
                                   name = str(_),
```

### Comparing `QTNOME_P-Y-R-O-B-O-T-1.0.4/pyproject.toml` & `QTNOME_P-Y-R-O-B-O-T-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<=64.0.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "QTNOME_P-Y-R-O-B-O-T"
-version = "1.0.4"
+version = "1.0.5"
 description = "An multiwindowed application envirement made in PyQt"
 readme = "README.md"
 authors = [{name =  "KUSHAL", email = "NONE@NONE.com"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 keywords = ["UI", "Envirement", "QT",
 			"PyQt", "UI Envirement",
```


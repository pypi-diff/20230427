# Comparing `tmp/hexapterygon-1.0.1.tar.gz` & `tmp/hexapterygon-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexapterygon-1.0.1.tar", last modified: Wed Apr 26 18:54:19 2023, max compression
+gzip compressed data, was "hexapterygon-1.0.2.tar", last modified: Thu Apr 27 19:59:50 2023, max compression
```

## Comparing `hexapterygon-1.0.1.tar` & `hexapterygon-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-26 18:54:19.057233 hexapterygon-1.0.1/
--rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-04-26 16:34:05.000000 hexapterygon-1.0.1/LICENSE
--rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-04-26 18:54:19.057233 hexapterygon-1.0.1/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)     6338 2023-04-26 18:32:42.000000 hexapterygon-1.0.1/README.md
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-26 18:54:19.057233 hexapterygon-1.0.1/hexapterygon/
--rw-r--r--   0 xou       (1000) xou       (1000)     1442 2023-04-04 21:25:43.000000 hexapterygon-1.0.1/hexapterygon/DeviceEvents.py
--rw-r--r--   0 xou       (1000) xou       (1000)    10731 2023-04-26 18:51:30.000000 hexapterygon-1.0.1/hexapterygon/DeviceOverlay.py
--rw-r--r--   0 xou       (1000) xou       (1000)      691 2023-04-26 17:13:52.000000 hexapterygon-1.0.1/hexapterygon/HexaGlobals.py
--rw-r--r--   0 xou       (1000) xou       (1000)    14230 2023-04-26 18:52:35.000000 hexapterygon-1.0.1/hexapterygon/HexaTUI.py
--rw-r--r--   0 xou       (1000) xou       (1000)     1506 2023-04-19 11:46:33.000000 hexapterygon-1.0.1/hexapterygon/InsortForOldPython.py
--rw-r--r--   0 xou       (1000) xou       (1000)      324 2023-04-15 09:36:08.000000 hexapterygon-1.0.1/hexapterygon/StateEnums.py
--rw-r--r--   0 xou       (1000) xou       (1000)    17981 2023-04-14 03:20:33.000000 hexapterygon-1.0.1/hexapterygon/TUItilities.py
--rw-r--r--   0 xou       (1000) xou       (1000)     4209 2023-04-26 18:51:34.000000 hexapterygon-1.0.1/hexapterygon/__init__.py
--rw-r--r--   0 xou       (1000) xou       (1000)     2260 2023-04-26 18:36:02.000000 hexapterygon-1.0.1/hexapterygon/__main__.py
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-26 18:54:19.057233 hexapterygon-1.0.1/hexapterygon.egg-info/
--rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-04-26 18:54:18.000000 hexapterygon-1.0.1/hexapterygon.egg-info/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)      495 2023-04-26 18:54:19.000000 hexapterygon-1.0.1/hexapterygon.egg-info/SOURCES.txt
--rw-r--r--   0 xou       (1000) xou       (1000)        1 2023-04-26 18:54:18.000000 hexapterygon-1.0.1/hexapterygon.egg-info/dependency_links.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       60 2023-04-26 18:54:18.000000 hexapterygon-1.0.1/hexapterygon.egg-info/entry_points.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       36 2023-04-26 18:54:18.000000 hexapterygon-1.0.1/hexapterygon.egg-info/requires.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       13 2023-04-26 18:54:18.000000 hexapterygon-1.0.1/hexapterygon.egg-info/top_level.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       38 2023-04-26 18:54:19.057233 hexapterygon-1.0.1/setup.cfg
--rw-r--r--   0 xou       (1000) xou       (1000)      962 2023-04-26 18:44:39.000000 hexapterygon-1.0.1/setup.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-27 19:59:50.397792 hexapterygon-1.0.2/
+-rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-04-26 16:34:05.000000 hexapterygon-1.0.2/LICENSE
+-rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-04-27 19:59:50.397792 hexapterygon-1.0.2/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)     6338 2023-04-26 18:32:42.000000 hexapterygon-1.0.2/README.md
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-27 19:59:50.397792 hexapterygon-1.0.2/hexapterygon/
+-rw-r--r--   0 xou       (1000) xou       (1000)     1442 2023-04-04 21:25:43.000000 hexapterygon-1.0.2/hexapterygon/DeviceEvents.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    10725 2023-04-27 19:56:14.000000 hexapterygon-1.0.2/hexapterygon/DeviceOverlay.py
+-rw-r--r--   0 xou       (1000) xou       (1000)      691 2023-04-26 17:13:52.000000 hexapterygon-1.0.2/hexapterygon/HexaGlobals.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    14230 2023-04-26 18:52:35.000000 hexapterygon-1.0.2/hexapterygon/HexaTUI.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     1506 2023-04-19 11:46:33.000000 hexapterygon-1.0.2/hexapterygon/InsortForOldPython.py
+-rw-r--r--   0 xou       (1000) xou       (1000)      324 2023-04-15 09:36:08.000000 hexapterygon-1.0.2/hexapterygon/StateEnums.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    17981 2023-04-14 03:20:33.000000 hexapterygon-1.0.2/hexapterygon/TUItilities.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     4209 2023-04-27 19:57:26.000000 hexapterygon-1.0.2/hexapterygon/__init__.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     2260 2023-04-26 18:36:02.000000 hexapterygon-1.0.2/hexapterygon/__main__.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-04-27 19:59:50.397792 hexapterygon-1.0.2/hexapterygon.egg-info/
+-rw-r--r--   0 xou       (1000) xou       (1000)      391 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)      495 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/SOURCES.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)        1 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/dependency_links.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       60 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/entry_points.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       36 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/requires.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       13 2023-04-27 19:59:50.000000 hexapterygon-1.0.2/hexapterygon.egg-info/top_level.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       38 2023-04-27 19:59:50.397792 hexapterygon-1.0.2/setup.cfg
+-rw-r--r--   0 xou       (1000) xou       (1000)      962 2023-04-27 19:57:34.000000 hexapterygon-1.0.2/setup.py
```

### Comparing `hexapterygon-1.0.1/LICENSE` & `hexapterygon-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.1/README.md` & `hexapterygon-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.1/hexapterygon/DeviceEvents.py` & `hexapterygon-1.0.2/hexapterygon/DeviceEvents.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.1/hexapterygon/DeviceOverlay.py` & `hexapterygon-1.0.2/hexapterygon/DeviceOverlay.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         version = version if version else response
         return (self.__download(package, version), version)
 
 
     def install(self, package, *args): # TODO split (| version)
         if not self.install_allowed: return False
         tmp_pkg_splt = package.split('|')
-        version = None if len(tmp_pkg_splt) == 1 else int(tmp_pkg_splt[1].split('#')(0))
+        version = None if len(tmp_pkg_splt) == 1 else int(tmp_pkg_splt[1])
         package = tmp_pkg_splt[0]
         if isfile(package) and package.endswith('.apk'):
             package = package
             # TODO: check if is_installed
         else: 
             if self.is_installed(package):
                 self.event_install(package, InstallState.ALREADY_INSTALLED) # '"{package}" Package is already installed'
@@ -196,15 +196,15 @@
         if not instruction                 : return 
         elif   instruction == '[UNINSTALL]': self.__temp_instriction_call = self.uninstall
         elif   instruction == '[INSTALL]'  : self.__temp_instriction_call = self.install
         elif   instruction == '[SHELL]'    : self.__temp_instriction_call = self.__shell 
         else: # TODO: Add extra instruction called EXTERNAL (or something) for external shell commands if user allows so by arg
             tmp_split   = instruction.split('#')
             comment     = tmp_split[len(tmp_split)-1].strip()
-            instruction = tmp_split[0]
+            instruction = tmp_split[0].strip()
             self.event_debloat(instruction, comment)
             self.__temp_instriction_call(instruction)
 
 
     def debloat(self):
         instructions = self.get_config_instructions()
         if not instructions: return False
```

### Comparing `hexapterygon-1.0.1/hexapterygon/HexaGlobals.py` & `hexapterygon-1.0.2/hexapterygon/HexaGlobals.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.1/hexapterygon/HexaTUI.py` & `hexapterygon-1.0.2/hexapterygon/HexaTUI.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.1/hexapterygon/InsortForOldPython.py` & `hexapterygon-1.0.2/hexapterygon/InsortForOldPython.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.1/hexapterygon/TUItilities.py` & `hexapterygon-1.0.2/hexapterygon/TUItilities.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.1/hexapterygon/__init__.py` & `hexapterygon-1.0.2/hexapterygon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .DeviceOverlay import DeviceOverlay
 from github         import Github
 import hexapterygon.HexaGlobals as g
 from shutil import rmtree
 
 
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 def get_global_server_repo(): return g.SERVER_REPO
 def set_global_server_repo(value): g.SERVER_REPO = value
 def set_github_token      (value): g.GIT         = Github(login_or_token=value)
 
 
 
 class Hexapterygon(DeviceEvents): # TODO: restore via cmd package install-existing <package>
```

### Comparing `hexapterygon-1.0.1/hexapterygon/__main__.py` & `hexapterygon-1.0.2/hexapterygon/__main__.py`

 * *Files identical despite different names*

### Comparing `hexapterygon-1.0.1/setup.py` & `hexapterygon-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #def readfile(filename):
 #    with open(filename, 'r+') as f:
 #        return f.read()
 
 
 setup(
     name="hexapterygon",
-    version="1.0.1",
+    version="1.0.2",
     description="A user-friendly all-in-one cross-platform, (uni-curses compatible component, module and uitility) software for orchestrating and debloating your Android devices from unwanted pre-installed crap.",
     #long_description=readfile('README.md'),
     author="George Chousos",
     author_email="gxousos@gmail.com",
     url="https://github.com/GiorgosXou/hexapterygon",
     packages=['hexapterygon'],
     install_requires=['uni-curses', 'pure-python-adb', 'PyGithub'],
```


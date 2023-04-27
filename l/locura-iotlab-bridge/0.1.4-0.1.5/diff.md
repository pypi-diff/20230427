# Comparing `tmp/locura_iotlab_bridge-0.1.4.tar.gz` & `tmp/locura_iotlab_bridge-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/locura_iotlab_bridge-0.1.4.tar", last modified: Thu Apr 27 14:47:16 2023, max compression
+gzip compressed data, was "dist/locura_iotlab_bridge-0.1.5.tar", last modified: Thu Apr 27 14:50:10 2023, max compression
```

## Comparing `locura_iotlab_bridge-0.1.4.tar` & `locura_iotlab_bridge-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 14:47:16.000000 locura_iotlab_bridge-0.1.4/
--rw-r--r--   0 quentin   (1000) quentin   (1000)      503 2023-04-27 14:47:16.000000 locura_iotlab_bridge-0.1.4/PKG-INFO
--rw-r--r--   0 quentin   (1000) quentin   (1000)      718 2023-04-27 14:47:09.000000 locura_iotlab_bridge-0.1.4/setup.py
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 14:47:16.000000 locura_iotlab_bridge-0.1.4/locura_iotlab_bridge/
--rwxr-xr-x   0 quentin   (1000) quentin   (1000)     6564 2023-04-27 14:46:33.000000 locura_iotlab_bridge-0.1.4/locura_iotlab_bridge/locura_iotlab_bridge.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)     1099 2022-12-12 13:04:38.000000 locura_iotlab_bridge-0.1.4/locura_iotlab_bridge/helpers.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)       49 2022-12-12 15:29:01.000000 locura_iotlab_bridge-0.1.4/locura_iotlab_bridge/__init__.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2023-04-27 14:47:16.000000 locura_iotlab_bridge-0.1.4/setup.cfg
--rw-r--r--   0 quentin   (1000) quentin   (1000)    21783 2022-12-12 13:41:17.000000 locura_iotlab_bridge-0.1.4/LICENSE
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 14:47:16.000000 locura_iotlab_bridge-0.1.4/locura_iotlab_bridge.egg-info/
--rw-r--r--   0 quentin   (1000) quentin   (1000)      503 2023-04-27 14:47:16.000000 locura_iotlab_bridge-0.1.4/locura_iotlab_bridge.egg-info/PKG-INFO
--rw-r--r--   0 quentin   (1000) quentin   (1000)      345 2023-04-27 14:47:16.000000 locura_iotlab_bridge-0.1.4/locura_iotlab_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       21 2023-04-27 14:47:16.000000 locura_iotlab_bridge-0.1.4/locura_iotlab_bridge.egg-info/top_level.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2023-04-27 14:47:16.000000 locura_iotlab_bridge-0.1.4/locura_iotlab_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       27 2023-04-27 14:47:16.000000 locura_iotlab_bridge-0.1.4/locura_iotlab_bridge.egg-info/requires.txt
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 14:50:10.000000 locura_iotlab_bridge-0.1.5/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      503 2023-04-27 14:50:10.000000 locura_iotlab_bridge-0.1.5/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      718 2023-04-27 14:50:02.000000 locura_iotlab_bridge-0.1.5/setup.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 14:50:10.000000 locura_iotlab_bridge-0.1.5/locura_iotlab_bridge/
+-rwxr-xr-x   0 quentin   (1000) quentin   (1000)     6564 2023-04-27 14:46:33.000000 locura_iotlab_bridge-0.1.5/locura_iotlab_bridge/locura_iotlab_bridge.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     1156 2023-04-27 14:49:52.000000 locura_iotlab_bridge-0.1.5/locura_iotlab_bridge/helpers.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       49 2022-12-12 15:29:01.000000 locura_iotlab_bridge-0.1.5/locura_iotlab_bridge/__init__.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2023-04-27 14:50:10.000000 locura_iotlab_bridge-0.1.5/setup.cfg
+-rw-r--r--   0 quentin   (1000) quentin   (1000)    21783 2022-12-12 13:41:17.000000 locura_iotlab_bridge-0.1.5/LICENSE
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 14:50:10.000000 locura_iotlab_bridge-0.1.5/locura_iotlab_bridge.egg-info/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      503 2023-04-27 14:50:10.000000 locura_iotlab_bridge-0.1.5/locura_iotlab_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      345 2023-04-27 14:50:10.000000 locura_iotlab_bridge-0.1.5/locura_iotlab_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       21 2023-04-27 14:50:10.000000 locura_iotlab_bridge-0.1.5/locura_iotlab_bridge.egg-info/top_level.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2023-04-27 14:50:10.000000 locura_iotlab_bridge-0.1.5/locura_iotlab_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       27 2023-04-27 14:50:10.000000 locura_iotlab_bridge-0.1.5/locura_iotlab_bridge.egg-info/requires.txt
```

### Comparing `locura_iotlab_bridge-0.1.4/setup.py` & `locura_iotlab_bridge-0.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='locura_iotlab_bridge',
-    version='0.1.4',    
+    version='0.1.5',    
     description='Bridge to connect LocURa MQTT ecosystem to IOT-LAB',
     url='https://gitlab.irit.fr/rmess/locura/infra/locura_iotlab_bridge',
     author='Quentin Vey',
     author_email='quentin.vey@irit.fr',
     license='CeCILL 2.1',
     packages=['locura_iotlab_bridge'],
     install_requires=['iotlabcli>=3.3.0',
```

### Comparing `locura_iotlab_bridge-0.1.4/locura_iotlab_bridge/locura_iotlab_bridge.py` & `locura_iotlab_bridge-0.1.5/locura_iotlab_bridge/locura_iotlab_bridge.py`

 * *Files identical despite different names*

### Comparing `locura_iotlab_bridge-0.1.4/locura_iotlab_bridge/helpers.py` & `locura_iotlab_bridge-0.1.5/locura_iotlab_bridge/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,27 +4,28 @@
     return os.path.dirname(os.path.abspath(__file__))+'/locura_iotlab_bridge.py'
     
     
 __hidden_file_list__ = []   # keep the files in memory so they are not deleted 
                             # util the end of the script.
     
     
-def makeScriptConfig(host, username, password, port=1883, verbose=0):
+def makeScriptConfig(host, username, password, topic, port=1883, verbose=0):
     """Generate a temporary scriptconfig file which contain the appropriate 
     environment variables. This file is deleted when the script ends.
     Returns the absolute path of this file."""
     f = tempfile.NamedTemporaryFile(mode='w', 
                                     prefix="locura_iotlab_bridge", 
                                     delete=True
                                     )
     f.write("LI_BRIDGE_HOST={}\n".format(host))
     f.write("LI_BRIDGE_PORT={}\n".format(port))
     f.write("LI_BRIDGE_VERBOSE={}\n".format(verbose))
     f.write("LI_BRIDGE_USER={}\n".format(username))
     f.write("LI_BRIDGE_PWD={}\n".format(password))
+    f.write("LI_BRIDGE_TOPIC={}\n".format(topic))
     f.flush()
     
     __hidden_file_list__.append(f)
         
         
     return f.name
```

### Comparing `locura_iotlab_bridge-0.1.4/LICENSE` & `locura_iotlab_bridge-0.1.5/LICENSE`

 * *Files identical despite different names*


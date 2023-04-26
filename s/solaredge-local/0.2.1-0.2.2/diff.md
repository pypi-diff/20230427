# Comparing `tmp/solaredge_local-0.2.1.tar.gz` & `tmp/solaredge_local-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solaredge_local-0.2.1.tar", last modified: Wed Apr 26 15:08:52 2023, max compression
+gzip compressed data, was "solaredge_local-0.2.2.tar", last modified: Wed Apr 26 22:36:05 2023, max compression
```

## Comparing `solaredge_local-0.2.1.tar` & `solaredge_local-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 15:08:52.768911 solaredge_local-0.2.1/
--rw-rw-r--   0 drob      (1000) drob      (1000)     8972 2023-04-26 15:08:52.768911 solaredge_local-0.2.1/PKG-INFO
--rw-rw-r--   0 drob      (1000) drob      (1000)     8375 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/README.md
--rw-rw-r--   0 drob      (1000) drob      (1000)       38 2023-04-26 15:08:52.768911 solaredge_local-0.2.1/setup.cfg
--rw-rw-r--   0 drob      (1000) drob      (1000)     1357 2023-04-26 14:33:57.000000 solaredge_local-0.2.1/setup.py
-drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 15:08:52.768911 solaredge_local-0.2.1/solaredge_local/
--rw-rw-r--   0 drob      (1000) drob      (1000)       49 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/__init__.py
--rw-rw-r--   0 drob      (1000) drob      (1000)     2240 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/information_pb2.py
--rw-rw-r--   0 drob      (1000) drob      (1000)     5145 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/maintenance_pb2.py
--rw-rw-r--   0 drob      (1000) drob      (1000)    12142 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/powercontrol_pb2.py
--rw-rw-r--   0 drob      (1000) drob      (1000)      664 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/solaredge.py
--rw-rw-r--   0 drob      (1000) drob      (1000)     6161 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/status_pb2.py
-drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 15:08:52.768911 solaredge_local-0.2.1/solaredge_local.egg-info/
--rw-rw-r--   0 drob      (1000) drob      (1000)     8972 2023-04-26 15:08:52.000000 solaredge_local-0.2.1/solaredge_local.egg-info/PKG-INFO
--rw-rw-r--   0 drob      (1000) drob      (1000)      405 2023-04-26 15:08:52.000000 solaredge_local-0.2.1/solaredge_local.egg-info/SOURCES.txt
--rw-rw-r--   0 drob      (1000) drob      (1000)        1 2023-04-26 15:08:52.000000 solaredge_local-0.2.1/solaredge_local.egg-info/dependency_links.txt
--rw-rw-r--   0 drob      (1000) drob      (1000)       23 2023-04-26 15:08:52.000000 solaredge_local-0.2.1/solaredge_local.egg-info/requires.txt
--rw-rw-r--   0 drob      (1000) drob      (1000)       16 2023-04-26 15:08:52.000000 solaredge_local-0.2.1/solaredge_local.egg-info/top_level.txt
+drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 22:36:05.649291 solaredge_local-0.2.2/
+-rw-rw-r--   0 drob      (1000) drob      (1000)     8972 2023-04-26 22:36:05.649291 solaredge_local-0.2.2/PKG-INFO
+-rw-rw-r--   0 drob      (1000) drob      (1000)     8375 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/README.md
+-rw-rw-r--   0 drob      (1000) drob      (1000)       38 2023-04-26 22:36:05.649291 solaredge_local-0.2.2/setup.cfg
+-rw-rw-r--   0 drob      (1000) drob      (1000)     1371 2023-04-26 22:33:58.000000 solaredge_local-0.2.2/setup.py
+drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 22:36:05.649291 solaredge_local-0.2.2/solaredge_local/
+-rw-rw-r--   0 drob      (1000) drob      (1000)       49 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/__init__.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)     2240 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/information_pb2.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)     5145 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/maintenance_pb2.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)    12142 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/powercontrol_pb2.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)      664 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/solaredge.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)     6161 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/status_pb2.py
+drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 22:36:05.649291 solaredge_local-0.2.2/solaredge_local.egg-info/
+-rw-rw-r--   0 drob      (1000) drob      (1000)     8972 2023-04-26 22:36:05.000000 solaredge_local-0.2.2/solaredge_local.egg-info/PKG-INFO
+-rw-rw-r--   0 drob      (1000) drob      (1000)      405 2023-04-26 22:36:05.000000 solaredge_local-0.2.2/solaredge_local.egg-info/SOURCES.txt
+-rw-rw-r--   0 drob      (1000) drob      (1000)        1 2023-04-26 22:36:05.000000 solaredge_local-0.2.2/solaredge_local.egg-info/dependency_links.txt
+-rw-rw-r--   0 drob      (1000) drob      (1000)       37 2023-04-26 22:36:05.000000 solaredge_local-0.2.2/solaredge_local.egg-info/requires.txt
+-rw-rw-r--   0 drob      (1000) drob      (1000)       16 2023-04-26 22:36:05.000000 solaredge_local-0.2.2/solaredge_local.egg-info/top_level.txt
```

### Comparing `solaredge_local-0.2.1/PKG-INFO` & `solaredge_local-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaredge_local
-Version: 0.2.1
+Version: 0.2.2
 Summary: API wrapper to communicate locally with SolarEdge Inverters
 Home-page: https://github.com/drobtravels/solaredge-local
 Author: David Roberts
 Author-email: 
 License: MIT License
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `solaredge_local-0.2.1/README.md` & `solaredge_local-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.1/setup.py` & `solaredge_local-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,29 +18,29 @@
             buf.append(f.read())
     return sep.join(buf)
 
 long_description = read('README.md')
 
 setup(
     name='solaredge_local',
-    version="0.2.1",
+    version="0.2.2",
     url='https://github.com/drobtravels/solaredge-local',
     license='MIT License',
     author='David Roberts',
     author_email="",
     description='API wrapper to communicate locally with SolarEdge Inverters',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['solaredge_local'],
     include_package_data=True,
     platforms='any',
     python_requires='>=3.0',
     install_requires=[
-        'uplink',
-        'uplink-protobuf'
+        'uplink>=0.9.7',
+        'uplink-protobuf>=0.1.0'
     ],
     classifiers = [
         'Programming Language :: Python :: 3',
         'Development Status :: 4 - Beta',
         'Natural Language :: English',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

### Comparing `solaredge_local-0.2.1/solaredge_local/information_pb2.py` & `solaredge_local-0.2.2/solaredge_local/information_pb2.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.1/solaredge_local/maintenance_pb2.py` & `solaredge_local-0.2.2/solaredge_local/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.1/solaredge_local/powercontrol_pb2.py` & `solaredge_local-0.2.2/solaredge_local/powercontrol_pb2.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.1/solaredge_local/solaredge.py` & `solaredge_local-0.2.2/solaredge_local/solaredge.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.1/solaredge_local/status_pb2.py` & `solaredge_local-0.2.2/solaredge_local/status_pb2.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.1/solaredge_local.egg-info/PKG-INFO` & `solaredge_local-0.2.2/solaredge_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaredge-local
-Version: 0.2.1
+Version: 0.2.2
 Summary: API wrapper to communicate locally with SolarEdge Inverters
 Home-page: https://github.com/drobtravels/solaredge-local
 Author: David Roberts
 Author-email: 
 License: MIT License
 Platform: any
 Classifier: Programming Language :: Python :: 3
```


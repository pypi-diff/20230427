# Comparing `tmp/spotinst-agent-beta-2.2.267.tar.gz` & `tmp/spotinst-agent-beta-2.2.268.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.267.tar", last modified: Thu Apr 27 13:02:10 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.268.tar", last modified: Thu Apr 27 14:40:06 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.267.tar` & `spotinst-agent-beta-2.2.268.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.898686 spotinst-agent-beta-2.2.267/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.267/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.267/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 13:02:10.898517 spotinst-agent-beta-2.2.267/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.267/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-27 13:02:10.898739 spotinst-agent-beta-2.2.267/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-27 13:02:08.000000 spotinst-agent-beta-2.2.267/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.891925 spotinst-agent-beta-2.2.267/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.267/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.883037 spotinst-agent-beta-2.2.267/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.894160 spotinst-agent-beta-2.2.267/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.267/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.267/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.896093 spotinst-agent-beta-2.2.267/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    10851 2023-04-27 13:02:08.000000 spotinst-agent-beta-2.2.267/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.898237 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       56 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 14:40:06.463283 spotinst-agent-beta-2.2.268/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.268/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.268/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 14:40:06.462540 spotinst-agent-beta-2.2.268/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.268/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-27 14:40:06.463336 spotinst-agent-beta-2.2.268/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-27 14:40:02.000000 spotinst-agent-beta-2.2.268/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 14:40:06.448774 spotinst-agent-beta-2.2.268/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.268/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.268/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.268/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.268/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 14:40:06.439429 spotinst-agent-beta-2.2.268/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 14:40:06.451717 spotinst-agent-beta-2.2.268/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.268/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.268/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 14:40:06.453203 spotinst-agent-beta-2.2.268/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.268/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.268/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    10984 2023-04-27 14:40:02.000000 spotinst-agent-beta-2.2.268/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.268/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 14:40:06.461467 spotinst-agent-beta-2.2.268/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 14:40:06.000000 spotinst-agent-beta-2.2.268/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-27 14:40:06.000000 spotinst-agent-beta-2.2.268/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-27 14:40:06.000000 spotinst-agent-beta-2.2.268/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       56 2023-04-27 14:40:06.000000 spotinst-agent-beta-2.2.268/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-27 14:40:06.000000 spotinst-agent-beta-2.2.268/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-27 14:40:06.000000 spotinst-agent-beta-2.2.268/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.267/LICENSE` & `spotinst-agent-beta-2.2.268/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.267/PKG-INFO` & `spotinst-agent-beta-2.2.268/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.267
+Version: 2.2.268
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
```

### Comparing `spotinst-agent-beta-2.2.267/README.rst` & `spotinst-agent-beta-2.2.268/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.267/setup.py` & `spotinst-agent-beta-2.2.268/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.267",
+    version="2.2.268",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.268/spotinst_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.268/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.268/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.268/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.268/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.268/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.268/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.268/spotinst_agent/taskmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,30 +142,34 @@
                     continue
 
                 # import module only if it exists for more than 1 second (had enough time to write the entire content)
                 # now = time.time()
                 # if now - mod_modification_time < 1:
                 #     self.log.info("Not loading file since it was created too recently: modified at %s, now is %s" % (mod_modification_time, now))
                 #     continue
-                time.sleep(10)
+                time.sleep(30)
                 try:
                     # Import the module
                     self.log.info("Importing %s" % modname)
                     mod = __import__(modname, globals(), locals(), ['*'])
                 except Exception as e:
                     # Log error
                     self.log.error("Failed to import module: %s. %s" % (modname, traceback.format_exc()))
                     continue
 
                 # Find all classes defined in the module
                 self.log.info("Finding classes defined in module " + str(modname))
+
+                print(str(dir(mod)))
+
                 for attrname in dir(mod):
                     attr = getattr(mod, attrname)
                     # Only attempt to load classes that are infact classes but not the base Module class
                     self.log.debug("Checking " + str(modname) + " Attribute " + str(attrname))
+                    self.log.info("Checking " + str(modname) + " Attribute " + str(attrname))
 
                     if inspect.isclass(attr) and isModule(attr) and attr != basemodule.Module:
                         # Get class name
                         fqcn = '.'.join([modname, attrname])
                         self.log.info("Module loaded : " + fqcn)
                         try:
                             # Load Module class
```

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.268/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.268/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.267
+Version: 2.2.268
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
```

### Comparing `spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.268/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/spotinst-agent-beta-2.2.266.tar.gz` & `tmp/spotinst-agent-beta-2.2.267.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.266.tar", last modified: Thu Apr 27 12:19:01 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.267.tar", last modified: Thu Apr 27 13:02:10 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.266.tar` & `spotinst-agent-beta-2.2.267.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 12:19:01.483318 spotinst-agent-beta-2.2.266/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.266/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.266/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 12:19:01.482951 spotinst-agent-beta-2.2.266/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.266/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-27 12:19:01.483369 spotinst-agent-beta-2.2.266/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-27 12:18:59.000000 spotinst-agent-beta-2.2.266/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 12:19:01.469304 spotinst-agent-beta-2.2.266/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.266/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.266/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.266/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.266/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 12:19:01.457887 spotinst-agent-beta-2.2.266/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 12:19:01.473703 spotinst-agent-beta-2.2.266/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.266/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.266/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 12:19:01.476307 spotinst-agent-beta-2.2.266/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.266/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.266/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    10840 2023-04-27 11:07:26.000000 spotinst-agent-beta-2.2.266/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.266/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 12:19:01.482682 spotinst-agent-beta-2.2.266/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 12:19:01.000000 spotinst-agent-beta-2.2.266/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-27 12:19:01.000000 spotinst-agent-beta-2.2.266/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-27 12:19:01.000000 spotinst-agent-beta-2.2.266/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       56 2023-04-27 12:19:01.000000 spotinst-agent-beta-2.2.266/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-27 12:19:01.000000 spotinst-agent-beta-2.2.266/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-27 12:19:01.000000 spotinst-agent-beta-2.2.266/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.898686 spotinst-agent-beta-2.2.267/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.267/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.267/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 13:02:10.898517 spotinst-agent-beta-2.2.267/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.267/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-27 13:02:10.898739 spotinst-agent-beta-2.2.267/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-27 13:02:08.000000 spotinst-agent-beta-2.2.267/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.891925 spotinst-agent-beta-2.2.267/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.267/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.883037 spotinst-agent-beta-2.2.267/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.894160 spotinst-agent-beta-2.2.267/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.267/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.267/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.896093 spotinst-agent-beta-2.2.267/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    10851 2023-04-27 13:02:08.000000 spotinst-agent-beta-2.2.267/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.267/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 13:02:10.898237 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       56 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-27 13:02:10.000000 spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.266/LICENSE` & `spotinst-agent-beta-2.2.267/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.266/PKG-INFO` & `spotinst-agent-beta-2.2.267/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.266
+Version: 2.2.267
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
```

### Comparing `spotinst-agent-beta-2.2.266/README.rst` & `spotinst-agent-beta-2.2.267/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.266/setup.py` & `spotinst-agent-beta-2.2.267/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.266",
+    version="2.2.267",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.267/spotinst_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.267/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.267/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.267/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.267/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.267/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.267/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.267/spotinst_agent/taskmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,28 +129,28 @@
 
                 modname = f[:-3]
                 mod_modification_time = os.path.getmtime(os.path.join(path, f))
                 mod_modification_time_str = str(mod_modification_time)
                 self.log.info("Py file found: %s" % modname)
 
                 modules_list = [x.lower() for x in self.tasks.keys()]
-                if modname in modules_list:
-                    if self.tasks[modname]['modification_time'] == mod_modification_time_str:
-                        self.log.info("Module '{0}' already loaded".format(modname))
-                        continue
+                # if modname in modules_list:
+                #     if self.tasks[modname]['modification_time'] == mod_modification_time_str:
+                #         self.log.info("Module '{0}' already loaded".format(modname))
+                #         continue
 
                 if modname == "utils" or modname == "basemodule":
                     continue
 
                 # import module only if it exists for more than 1 second (had enough time to write the entire content)
-                now = time.time()
+                # now = time.time()
                 # if now - mod_modification_time < 1:
                 #     self.log.info("Not loading file since it was created too recently: modified at %s, now is %s" % (mod_modification_time, now))
                 #     continue
-                time.sleep(1)
+                time.sleep(10)
                 try:
                     # Import the module
                     self.log.info("Importing %s" % modname)
                     mod = __import__(modname, globals(), locals(), ['*'])
                 except Exception as e:
                     # Log error
                     self.log.error("Failed to import module: %s. %s" % (modname, traceback.format_exc()))
```

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.267/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.266
+Version: 2.2.267
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
```

### Comparing `spotinst-agent-beta-2.2.266/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.267/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*


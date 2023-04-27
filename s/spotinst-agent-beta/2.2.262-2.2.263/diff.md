# Comparing `tmp/spotinst-agent-beta-2.2.262.tar.gz` & `tmp/spotinst-agent-beta-2.2.263.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.262.tar", last modified: Thu Apr 27 10:18:36 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.263.tar", last modified: Thu Apr 27 10:37:39 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.262.tar` & `spotinst-agent-beta-2.2.263.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:18:36.456484 spotinst-agent-beta-2.2.262/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.262/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.262/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 10:18:36.456297 spotinst-agent-beta-2.2.262/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.262/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-27 10:18:36.456548 spotinst-agent-beta-2.2.262/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-27 10:18:33.000000 spotinst-agent-beta-2.2.262/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:18:36.452153 spotinst-agent-beta-2.2.262/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    12856 2023-04-27 10:14:26.000000 spotinst-agent-beta-2.2.262/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.262/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.262/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.262/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:18:36.442373 spotinst-agent-beta-2.2.262/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:18:36.454326 spotinst-agent-beta-2.2.262/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.262/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.262/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:18:36.454633 spotinst-agent-beta-2.2.262/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.262/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.262/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    10805 2023-04-27 09:36:09.000000 spotinst-agent-beta-2.2.262/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.262/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:18:36.456020 spotinst-agent-beta-2.2.262/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 10:18:36.000000 spotinst-agent-beta-2.2.262/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-27 10:18:36.000000 spotinst-agent-beta-2.2.262/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-27 10:18:36.000000 spotinst-agent-beta-2.2.262/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       56 2023-04-27 10:18:36.000000 spotinst-agent-beta-2.2.262/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-27 10:18:36.000000 spotinst-agent-beta-2.2.262/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-27 10:18:36.000000 spotinst-agent-beta-2.2.262/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:37:39.281026 spotinst-agent-beta-2.2.263/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.263/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.263/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 10:37:39.280837 spotinst-agent-beta-2.2.263/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.263/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-27 10:37:39.281085 spotinst-agent-beta-2.2.263/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-27 10:37:36.000000 spotinst-agent-beta-2.2.263/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:37:39.269836 spotinst-agent-beta-2.2.263/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13079 2023-04-27 10:37:20.000000 spotinst-agent-beta-2.2.263/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.263/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.263/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.263/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:37:39.259300 spotinst-agent-beta-2.2.263/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:37:39.273524 spotinst-agent-beta-2.2.263/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.263/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.263/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:37:39.274698 spotinst-agent-beta-2.2.263/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.263/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.263/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    10805 2023-04-27 09:36:09.000000 spotinst-agent-beta-2.2.263/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.263/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 10:37:39.280135 spotinst-agent-beta-2.2.263/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 10:37:39.000000 spotinst-agent-beta-2.2.263/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-27 10:37:39.000000 spotinst-agent-beta-2.2.263/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-27 10:37:39.000000 spotinst-agent-beta-2.2.263/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       56 2023-04-27 10:37:39.000000 spotinst-agent-beta-2.2.263/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-27 10:37:39.000000 spotinst-agent-beta-2.2.263/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-27 10:37:39.000000 spotinst-agent-beta-2.2.263/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.262/LICENSE` & `spotinst-agent-beta-2.2.263/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.262/PKG-INFO` & `spotinst-agent-beta-2.2.263/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.262
+Version: 2.2.263
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
```

### Comparing `spotinst-agent-beta-2.2.262/README.rst` & `spotinst-agent-beta-2.2.263/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.262/setup.py` & `spotinst-agent-beta-2.2.263/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.262",
+    version="2.2.263",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.263/spotinst_agent/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,17 @@
 def handle_base_modules(dirname, modules_path, initiator_modules_path):
     basemodule_yml_path = os.path.join(dirname, 'data/configuration/basemodule.yml')
     utils_path = os.path.join(dirname, 'utils.py')
     basemodule_template_path = os.path.join(dirname, 'basemodule.py')
 
     if not os.path.exists(initiator_modules_path):
         os.makedirs(initiator_modules_path)
+    copyfile(basemodule_template_path, initiator_modules_path + '/basemodule.py')
+    copyfile(basemodule_yml_path, initiator_modules_path + '/basemodule.yml')
+    copyfile(utils_path, initiator_modules_path + '/utils.py')
     if not os.path.exists(modules_path):
         os.makedirs(modules_path)
     copyfile(basemodule_template_path, modules_path + '/basemodule.py')
     copyfile(basemodule_yml_path, modules_path + '/basemodule.yml')
     copyfile(utils_path, modules_path + '/utils.py')
```

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.263/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.263/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.263/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.263/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.263/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.263/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.263/spotinst_agent/taskmanager.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.263/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.263/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.262
+Version: 2.2.263
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
```

### Comparing `spotinst-agent-beta-2.2.262/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.263/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*


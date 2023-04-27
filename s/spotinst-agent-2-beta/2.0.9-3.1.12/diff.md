# Comparing `tmp/spotinst-agent-2-beta-2.0.9.tar.gz` & `tmp/spotinst-agent-2-beta-3.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-2-beta-2.0.9.tar", last modified: Sun Mar 26 08:22:42 2023, max compression
+gzip compressed data, was "spotinst-agent-2-beta-3.1.12.tar", last modified: Thu Apr 27 08:02:47 2023, max compression
```

## Comparing `spotinst-agent-2-beta-2.0.9.tar` & `spotinst-agent-2-beta-3.1.12.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yarden     (502) staff       (20)        0 2023-03-26 08:22:42.252200 spotinst-agent-2-beta-2.0.9/
--rw-r--r--   0 yarden     (502) staff       (20)     1065 2023-03-23 06:31:33.000000 spotinst-agent-2-beta-2.0.9/LICENSE
--rw-r--r--   0 yarden     (502) staff       (20)      181 2023-03-23 06:31:33.000000 spotinst-agent-2-beta-2.0.9/MANIFEST.in
--rw-r--r--   0 yarden     (502) staff       (20)     1981 2023-03-26 08:22:42.251846 spotinst-agent-2-beta-2.0.9/PKG-INFO
--rw-r--r--   0 yarden     (502) staff       (20)     1287 2023-03-23 06:31:33.000000 spotinst-agent-2-beta-2.0.9/README.rst
--rw-r--r--   0 yarden     (502) staff       (20)       38 2023-03-26 08:22:42.252252 spotinst-agent-2-beta-2.0.9/setup.cfg
--rw-r--r--   0 yarden     (502) staff       (20)     1441 2023-03-26 08:22:39.000000 spotinst-agent-2-beta-2.0.9/setup.py
-drwxr-xr-x   0 yarden     (502) staff       (20)        0 2023-03-26 08:22:42.244826 spotinst-agent-2-beta-2.0.9/spotinst_agent/
--rw-r--r--   0 yarden     (502) staff       (20)    11603 2023-03-23 15:01:44.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent/__init__.py
--rw-r--r--   0 yarden     (502) staff       (20)     3383 2023-03-23 15:01:44.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent/agent.py
--rw-r--r--   0 yarden     (502) staff       (20)     9645 2023-03-23 15:01:44.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent/agentinit.py
--rw-r--r--   0 yarden     (502) staff       (20)     1157 2023-03-23 15:01:44.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent/basemodule.py
-drwxr-xr-x   0 yarden     (502) staff       (20)        0 2023-03-26 08:22:42.233132 spotinst-agent-2-beta-2.0.9/spotinst_agent/data/
-drwxr-xr-x   0 yarden     (502) staff       (20)        0 2023-03-26 08:22:42.246424 spotinst-agent-2-beta-2.0.9/spotinst_agent/data/configuration/
--rw-r--r--   0 yarden     (502) staff       (20)      180 2023-03-23 06:31:33.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 yarden     (502) staff       (20)      727 2023-03-23 15:01:44.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 yarden     (502) staff       (20)        0 2023-03-26 08:22:42.247154 spotinst-agent-2-beta-2.0.9/spotinst_agent/data/installation/
--rwxr-xr-x   0 yarden     (502) staff       (20)     6701 2023-03-23 15:01:44.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 yarden     (502) staff       (20)    21721 2023-03-23 15:01:44.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent/scheduler.py
--rw-r--r--   0 yarden     (502) staff       (20)     9252 2023-03-23 15:01:44.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent/taskmanager.py
--rw-r--r--   0 yarden     (502) staff       (20)     9662 2023-03-23 15:01:44.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent/utils.py
-drwxr-xr-x   0 yarden     (502) staff       (20)        0 2023-03-26 08:22:42.251418 spotinst-agent-2-beta-2.0.9/spotinst_agent_2_beta.egg-info/
--rw-r--r--   0 yarden     (502) staff       (20)     1981 2023-03-26 08:22:42.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent_2_beta.egg-info/PKG-INFO
--rw-r--r--   0 yarden     (502) staff       (20)      650 2023-03-26 08:22:42.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent_2_beta.egg-info/SOURCES.txt
--rw-r--r--   0 yarden     (502) staff       (20)        1 2023-03-26 08:22:42.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent_2_beta.egg-info/dependency_links.txt
--rw-r--r--   0 yarden     (502) staff       (20)       56 2023-03-26 08:22:42.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent_2_beta.egg-info/entry_points.txt
--rw-r--r--   0 yarden     (502) staff       (20)       23 2023-03-26 08:22:42.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent_2_beta.egg-info/requires.txt
--rw-r--r--   0 yarden     (502) staff       (20)       15 2023-03-26 08:22:42.000000 spotinst-agent-2-beta-2.0.9/spotinst_agent_2_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.528722 spotinst-agent-2-beta-3.1.12/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-2-beta-3.1.12/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-2-beta-3.1.12/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1982 2023-04-27 08:02:47.528530 spotinst-agent-2-beta-3.1.12/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-2-beta-3.1.12/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-27 08:02:47.528780 spotinst-agent-2-beta-3.1.12/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1442 2023-04-27 08:02:44.000000 spotinst-agent-2-beta-3.1.12/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.526051 spotinst-agent-2-beta-3.1.12/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    12950 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3383 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9645 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1157 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.520011 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.526571 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-03-12 08:32:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.526835 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6701 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21721 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    11165 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9662 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.528255 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1982 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      650 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       56 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       23 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-2-beta-2.0.9/LICENSE` & `spotinst-agent-2-beta-3.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-2.0.9/PKG-INFO` & `spotinst-agent-2-beta-3.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-2-beta
-Version: 2.0.9
+Version: 3.1.12
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
```

### Comparing `spotinst-agent-2-beta-2.0.9/README.rst` & `spotinst-agent-2-beta-3.1.12/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-2.0.9/setup.py` & `spotinst-agent-2-beta-3.1.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-2-beta',
 
-    version="2.0.9",
+    version="3.1.12",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent/__init__.py` & `spotinst-agent-2-beta-3.1.12/spotinst_agent/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 from time import sleep
 
 
 def main():
     s3_base_link = 'https://s3.amazonaws.com/spotinst-public/services/spotinst-agent-2'
     s3_base_workers_link = s3_base_link + "/workers"
     s3_base_collectors_link = s3_base_link + "/collectors"
+    s3_base_initiator_link = s3_base_link + "/initiators"
     modules_path = '/etc/spotinst/agent/modules'
+    initiator_modules_path = '/etc/spotinst/agent/initiators/modules'
     instance_details_path = '/etc/spotinst'
 
     results = parse_arguments()
     action = results.action
     argument = results.argument
     second_argument = results.second_argument
     third_argument  = results.third_argument
@@ -43,15 +45,21 @@
         else:
             print ("Please enter the name of the worker which you want to add.")
 
     elif action == "add-collector":
         if argument is not None:
             install_collector(argument, modules_path, s3_base_collectors_link)
         else:
-            print ("Please enter the name of the collector which you want to add.")
+            print("Please enter the name of the collector which you want to add.")
+
+    elif action == "add-initiator":
+        if argument is not None:
+            install_initiator(argument, initiator_modules_path, s3_base_initiator_link)
+        else:
+            print("Please enter the name of the initiator which you want to add.")
 
     elif action == "run":
         run_agent(debug, verbose, cloud_provider)
 
     elif action == "configure":
         if argument is not None:
             print ("configuring " + argument)
@@ -238,15 +246,24 @@
 def install_collector(collector_name, modules_path, s3_base_collectors_link):
     print ("adding collector " + collector_name)
     try:
         handle_prerequisites(s3_base_collectors_link, collector_name)
         get_collector_files(collector_name, modules_path, s3_base_collectors_link)
 
     except Exception as e:
-        print ("Could not get collector " + collector_name + " Exception : " + str(e))
+        print("Could not get collector " + collector_name + " Exception : " + str(e))
+
+
+def install_initiator(initiator_name, initiator_modules_path, s3_base_initiator_link):
+    print("adding initiator " + initiator_name)
+    try:
+        get_initiator_files(initiator_name, initiator_modules_path, s3_base_initiator_link)
+
+    except Exception as e:
+        print("Could not get initiator " + initiator_name + " Exception : " + str(e))
 
 
 def get_worker_files(modules_path, s3_base_workers_link, worker_name):
     py_response = urllib.request.urlopen(s3_base_workers_link + '/' + worker_name + '/' + worker_name + '.py')
     yml_response = urllib.request.urlopen(s3_base_workers_link + '/' + worker_name + '/' + worker_name + '.yml')
 
     with open(modules_path + '/' + worker_name + '.py', 'wb') as worker:
@@ -260,14 +277,24 @@
         response = urllib.request.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.py')
         collector.write(response.read())
     with open(modules_path + '/' + collector_name + '.yml', 'wb') as collector_cfg:
         response = urllib.request.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.yml')
         collector_cfg.write(response.read())
 
 
+def get_initiator_files(initiator_name, initiator_modules_path, s3_base_initiator_link):
+    with open(initiator_modules_path + '/' + initiator_name + '.py', 'wb') as initiator:
+        response = urllib.request.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.py')
+        initiator.write(response.read())
+    with open(initiator_modules_path + '/' + initiator_name + '.yml', 'wb') as initiator_cfg:
+        response = urllib.request.urlopen(
+            s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.yml')
+        initiator_cfg.write(response.read())
+
+
 def handle_prerequisites(s3_base_module_link, module_name):
     try:
         response = urllib.request.urlopen(s3_base_module_link + '/' + module_name + '/' + module_name + '.req')
         requirements_file = response.read().decode('utf-8')
         requirements_names = requirements_file.split("\n")
         print ("This module requires the following packages to be installed:")
         for requirement in requirements_names:
```

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent/agent.py` & `spotinst-agent-2-beta-3.1.12/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent/agentinit.py` & `spotinst-agent-2-beta-3.1.12/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent/basemodule.py` & `spotinst-agent-2-beta-3.1.12/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-2-beta-3.1.12/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 enable: True
 # interval in seconds
 reload_interval: 120
 aws_instance_id_locator_url: 'http://169.254.169.254/latest/meta-data/instance-id'
 aws_metadata_service_token_url: 'http://169.254.169.254/latest/api/token'
 gcp_instance_metadata_url: 'http://metadata.google.internal/computeMetadata/v1'
 azure_instance_id_locator_url: 'http://169.254.169.254/metadata/instance/compute/vmId?api-version=2017-08-01&format=text'
-azure_spot_instance_id_locator_url: 'http://169.254.169.254/metadata/instance/compute/vmId?api-version=2021-02-01&format=text'
+azure_spot_instance_id_locator_url: 'http://169.254.169.254/metadata/instance/compute/name?api-version=2017-08-01&format=text'
 gcp_instance_name: '/instance/name'
 azure_node_id_path: '/etc/spotinst/nodeId.txt'
 azure_pool_id_path: '/etc/spotinst/poolId.txt'
 cloud_provider_path: '/etc/spotinst/cloud_provider.txt'
```

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-2-beta-3.1.12/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent/scheduler.py` & `spotinst-agent-2-beta-3.1.12/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent/taskmanager.py` & `spotinst-agent-2-beta-3.1.12/spotinst_agent/taskmanager.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,25 @@
         self.reload_interval = reload_interval
         self.scheduler = ThreadedScheduler()
         self.running = True
         self.tasks = {}
         self.instance_details = instance_details
 
     def start(self):
+        initiators_folder = '/etc/spotinst/agent/initiators/modules'
+        self.log.debug("service is %s" % self.enable)
+
+        # Search for initiators in folder
+        initiators = self.load_modules(initiators_folder)
+
+        # Setup Modules
+        for initiator in initiators.values():
+            c = self.init_module(initiator['cls'])
+            self.schedule_initiator_module(c, initiator)
+
         modules_folder = '/etc/spotinst/agent/modules'
         self.log.debug("service is %s" % self.enable)
 
         # Search for modules in folder
         modules = self.load_modules(modules_folder)
 
         # Setup Modules
@@ -224,14 +235,49 @@
             task = self.scheduler.add_interval_task(func, name, splay, interval, method.sequential,
                                                     args, None, True)
 
             self.log.debug("Scheduled task: %s" % name)
             # Add task to list
             self.tasks[module['file_name']] = {'task': task, 'modification_time': module['modification_time']}
 
+    def schedule_initiator_module(self, c, module):
+        """
+        Schedule module
+        """
+        if c is None:
+            self.log.warning("Skipped loading invalid Module: %s" % c.__class__.__name__)
+            return
+
+        if not c.get_enable():
+            self.log.info("Skipped loading Module '%s' since it is disabled" % c.__class__.__name__)
+            return
+
+        # Get Module schedule
+        for name, schedule in c.get_schedule().items():
+            # Get scheduler args
+            func, args, splay, interval = schedule
+
+            # Check if a module with same name has already been scheduled
+            if module['file_name'] in self.tasks:
+                try:
+                    self.scheduler.cancel(self.tasks[module['file_name']]['task'])
+                    # Log
+                    self.log.info("Canceled task: %s" % name)
+                except ValueError as e:
+                    self.log.error("Unable to cancel task '{0}' - {1}".format(self.tasks[name], e))
+
+            # Schedule Collector
+            self.log.info("Scheduled task {0} to run every {1}s (delayed of {2}s)".format(name, interval, splay))
+            task = self.scheduler.add_single_task(func, name, splay, method.sequential,
+                                                  args, None)
+
+            self.log.debug("Scheduled task: %s" % name)
+            # Add task to list
+            self.tasks[module['file_name']] = {'task': task, 'modification_time': module['modification_time']}
+
     def stop(self):
         """
         Close and stop all tasks.
         """
         # Set Running Flag
         self.running = False
```

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent/utils.py` & `spotinst-agent-2-beta-3.1.12/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent_2_beta.egg-info/PKG-INFO` & `spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-2-beta
-Version: 2.0.9
+Version: 3.1.12
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
```

### Comparing `spotinst-agent-2-beta-2.0.9/spotinst_agent_2_beta.egg-info/SOURCES.txt` & `spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/spotinst-agent-beta-1.1.2582.tar.gz` & `tmp/spotinst-agent-beta-2.2.261.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spotinst-agent-beta-1.1.2582.tar", last modified: Mon Aug 16 13:44:31 2021, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.261.tar", last modified: Thu Apr 27 09:37:35 2023, max compression
```

## Comparing `spotinst-agent-beta-1.1.2582.tar` & `spotinst-agent-beta-2.2.261.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     2278 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/PKG-INFO
--rw-r--r--   0 cadurikatzav   (502) staff       (20)      181 2021-01-17 21:53:39.000000 spotinst-agent-beta-1.1.2582/MANIFEST.in
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     1393 2021-08-16 13:42:54.000000 spotinst-agent-beta-1.1.2582/setup.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent_beta.egg-info/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     2278 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 cadurikatzav   (502) staff       (20)      630 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 cadurikatzav   (502) staff       (20)       56 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 cadurikatzav   (502) staff       (20)       16 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 cadurikatzav   (502) staff       (20)       15 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent_beta.egg-info/top_level.txt
--rw-r--r--   0 cadurikatzav   (502) staff       (20)        1 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 cadurikatzav   (502) staff       (20)       38 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/setup.cfg
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     1287 2021-01-17 21:53:39.000000 spotinst-agent-beta-1.1.2582/README.rst
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     9604 2021-08-16 13:41:46.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/agentinit.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     1129 2021-08-16 13:41:46.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/basemodule.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)    11328 2021-08-16 13:41:46.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/__init__.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     8892 2021-08-16 13:41:46.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/taskmanager.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     9420 2021-08-16 13:41:46.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/utils.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)     3116 2021-08-16 13:41:46.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/agent.py
--rw-r--r--   0 cadurikatzav   (502) staff       (20)    21605 2021-08-16 13:41:46.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/scheduler.py
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/data/
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/data/configuration/
--rw-r--r--   0 cadurikatzav   (502) staff       (20)      180 2021-01-17 21:53:39.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 cadurikatzav   (502) staff       (20)      727 2021-08-16 13:41:33.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 cadurikatzav   (502) staff       (20)        0 2021-08-16 13:44:31.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/data/installation/
--rwxr-xr-x   0 cadurikatzav   (502) staff       (20)     6630 2021-08-16 13:41:46.000000 spotinst-agent-beta-1.1.2582/spotinst_agent/data/installation/agent-init.sh
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 09:37:35.693750 spotinst-agent-beta-2.2.261/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.261/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.261/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 09:37:35.693342 spotinst-agent-beta-2.2.261/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.261/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-27 09:37:35.693807 spotinst-agent-beta-2.2.261/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-27 09:36:56.000000 spotinst-agent-beta-2.2.261/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 09:37:35.678577 spotinst-agent-beta-2.2.261/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    12634 2023-04-27 09:36:09.000000 spotinst-agent-beta-2.2.261/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.261/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.261/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.261/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 09:37:35.665914 spotinst-agent-beta-2.2.261/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 09:37:35.685046 spotinst-agent-beta-2.2.261/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.261/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.261/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 09:37:35.686410 spotinst-agent-beta-2.2.261/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.261/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.261/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    10805 2023-04-27 09:36:09.000000 spotinst-agent-beta-2.2.261/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.261/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 09:37:35.692700 spotinst-agent-beta-2.2.261/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 09:37:35.000000 spotinst-agent-beta-2.2.261/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-27 09:37:35.000000 spotinst-agent-beta-2.2.261/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-27 09:37:35.000000 spotinst-agent-beta-2.2.261/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       56 2023-04-27 09:37:35.000000 spotinst-agent-beta-2.2.261/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-27 09:37:35.000000 spotinst-agent-beta-2.2.261/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-27 09:37:35.000000 spotinst-agent-beta-2.2.261/spotinst_agent_beta.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spotinst-agent-beta-1.1.2582/PKG-INFO` & `spotinst-agent-beta-2.2.261/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,60 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 1.1.2582
+Version: 2.2.261
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
-Description: Agent
-        =======
-        
-        Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
-        
-        Note:
-        The agent must have token to communicate with spotinst API.
-        The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
-        
-        Application
-        ===========
-        
-        Manual Executing
-        ~~~~~~~~~~~~~~~~
-        The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
-        
-        Otherwise, you can use the following options:
-        
-        Usage:  ./agent [options]
-        
-        -c --config            Use alternate configuration yml file.
-        -l --log               Use alternate Log file for output.
-        -t --test              Test run.  Do not run remote script.
-        -v --verbose           verbose log
-        --stdout               redirect output to stdout
-        --debug                run with dummy credentials for debug purposes
-        
-        Configuration
-        ~~~~~~~~~~~~~
-        There are two levels of configuration representing in yml files.
-        The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
-        The worker configuration, located at the workers folder is responsible of the specific workers parameters.
-        
-        
-        MAKEFILE
-        ~~~~~~~~~~~~~
-        run 'make release'
-        output file is located in the /dist folder
-        
-        Documentation
-        =============
-        
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
+License-File: LICENSE
+
+Agent
+=======
+
+Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
+
+Note:
+The agent must have token to communicate with spotinst API.
+The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
+
+Application
+===========
+
+Manual Executing
+~~~~~~~~~~~~~~~~
+The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
+
+Otherwise, you can use the following options:
+
+Usage:  ./agent [options]
+
+-c --config            Use alternate configuration yml file.
+-l --log               Use alternate Log file for output.
+-t --test              Test run.  Do not run remote script.
+-v --verbose           verbose log
+--stdout               redirect output to stdout
+--debug                run with dummy credentials for debug purposes
+
+Configuration
+~~~~~~~~~~~~~
+There are two levels of configuration representing in yml files.
+The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
+The worker configuration, located at the workers folder is responsible of the specific workers parameters.
+
+
+MAKEFILE
+~~~~~~~~~~~~~
+run 'make release'
+output file is located in the /dist folder
+
+Documentation
+=============
+
+
```

### Comparing `spotinst-agent-beta-1.1.2582/setup.py` & `spotinst-agent-beta-2.2.261/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="1.1.2582",
+    version="2.2.261",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.261/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,60 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 1.1.2582
+Version: 2.2.261
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
-Description: Agent
-        =======
-        
-        Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
-        
-        Note:
-        The agent must have token to communicate with spotinst API.
-        The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
-        
-        Application
-        ===========
-        
-        Manual Executing
-        ~~~~~~~~~~~~~~~~
-        The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
-        
-        Otherwise, you can use the following options:
-        
-        Usage:  ./agent [options]
-        
-        -c --config            Use alternate configuration yml file.
-        -l --log               Use alternate Log file for output.
-        -t --test              Test run.  Do not run remote script.
-        -v --verbose           verbose log
-        --stdout               redirect output to stdout
-        --debug                run with dummy credentials for debug purposes
-        
-        Configuration
-        ~~~~~~~~~~~~~
-        There are two levels of configuration representing in yml files.
-        The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
-        The worker configuration, located at the workers folder is responsible of the specific workers parameters.
-        
-        
-        MAKEFILE
-        ~~~~~~~~~~~~~
-        run 'make release'
-        output file is located in the /dist folder
-        
-        Documentation
-        =============
-        
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
+License-File: LICENSE
+
+Agent
+=======
+
+Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
+
+Note:
+The agent must have token to communicate with spotinst API.
+The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
+
+Application
+===========
+
+Manual Executing
+~~~~~~~~~~~~~~~~
+The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
+
+Otherwise, you can use the following options:
+
+Usage:  ./agent [options]
+
+-c --config            Use alternate configuration yml file.
+-l --log               Use alternate Log file for output.
+-t --test              Test run.  Do not run remote script.
+-v --verbose           verbose log
+--stdout               redirect output to stdout
+--debug                run with dummy credentials for debug purposes
+
+Configuration
+~~~~~~~~~~~~~
+There are two levels of configuration representing in yml files.
+The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
+The worker configuration, located at the workers folder is responsible of the specific workers parameters.
+
+
+MAKEFILE
+~~~~~~~~~~~~~
+run 'make release'
+output file is located in the /dist folder
+
+Documentation
+=============
+
+
```

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.261/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 setup.py
 spotinst_agent/__init__.py
 spotinst_agent/agent.py
 spotinst_agent/agentinit.py
 spotinst_agent/basemodule.py
```

### Comparing `spotinst-agent-beta-1.1.2582/README.rst` & `spotinst-agent-beta-2.2.261/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.261/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.261/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.261/spotinst_agent/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 from time import sleep
 
 
 def main():
     s3_base_link = 'https://s3.amazonaws.com/spotinst-public/services/spotinst-agent'
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
-    third_argument  = results.third_argument
+    third_argument = results.third_argument
     cloud_provider = results.cloud_provider
     args = vars(results)
     verbose = False
     debug = False
 
     if args['verbose']:
         verbose = True
@@ -32,51 +34,57 @@
     if args['debug']:
         debug = True
 
     if action == "add-worker":
         if argument is not None:
             install_worker(modules_path, s3_base_workers_link, argument)
         else:
-            print ("Please enter the name of the worker which you want to add.")
+            print("Please enter the name of the worker which you want to add.")
 
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
-            print ("configuring " + argument)
+            print("configuring " + argument)
         else:
-            print ("Spotinst agent configuration")
+            print("Spotinst agent configuration")
 
     elif action == "init":
 
         try_num = 1
         install_succeed = False
         while (not install_succeed) and (try_num <= 3):
             if try_num > 1:
                 sleep(20)
                 print("trying to Initializing agent again (retry %s/3)" % (format(try_num)))
             try_num += 1
-            print ("Initializing agent")
+            print("Initializing agent")
             install_succeed = handle_cloud_provider(cloud_provider, instance_details_path) and install_and_init_agent(
                 argument, second_argument, third_argument, modules_path)
 
         if not install_succeed:
             print("init failed")
             exit(1)
         else:
             print("Spotinst agent installed successfully")
     else:
-        print ("Unrecognized action. Please use one of the following : add-worker, add-collector, configure")
+        print("Unrecognized action. Please use one of the following : add-worker, add-collector, configure")
 
 
 def install_and_init_agent(token, account_id, custom_host, modules_path):
     # Paths
     runscript = None
     try:
         dirname, filename = os.path.split(os.path.abspath(__file__))
@@ -85,15 +93,15 @@
         create_agent_local_folders()
         handle_base_modules(dirname, modules_path)
         handle_yml_file(dirname)
         handle_credentials(account_id, script_full_path, spotinst_agent_path, token, custom_host)
         handle_agent_path(spotinst_agent_path)
         runscript = subprocess.Popen(script_full_path)
         runscript.wait()
-        print ('result : ' + str(runscript.communicate()))
+        print('result : ' + str(runscript.communicate()))
     except:
         if runscript is not None:
             runscript.kill()
         return False
     return True
 
 
@@ -105,15 +113,15 @@
         full_path = instance_details_path + "/cloud_provider.txt"
         cloud_provider_file = open(full_path, 'w')
         cloud_provider_file.write(cloud_provider)
         cloud_provider_file.close()
         os.chmod(full_path, 0o644)
         return True
     except IOError:
-        print "Unable to create /etc/spotinst/cloud_provider.txt"
+        print("Unable to create /etc/spotinst/cloud_provider.txt")
         if cloud_provider_file is not None:
             cloud_provider_file.close()
         return False
 
 
 def create_agent_local_folders():
     if not os.path.exists('/etc/spotinst'):
@@ -143,18 +151,18 @@
     default_yml_destination = '/etc/spotinst/agent/config/spotinst-agent.yml'
     if not os.path.exists('/etc/spotinst/agent/config/spotinst-agent.yml'):
         copyfile(default_agent_yml, default_yml_destination)
 
 
 def handle_credentials(account_id, script_full_path, spotinst_agent_path, token, host):
     if token is not None:
-        print ("Creating Spotinst credentials directory")
+        print("Creating Spotinst credentials directory")
 
         if host is None:
-            #if the customer didn't supply custom host set the default
+            # if the customer didn't supply custom host set the default
             host = 'api.spotinst.io'
         creds_file, creds_path = create_creds_file()
         write_creds_path(account_id, creds_file, token, host)
         os.chmod(creds_path, 0o777)
 
     else:
         # Credentials already exist - retrieve from file
@@ -164,14 +172,15 @@
         host = creds["host"]
     os.putenv("SPOTINST_TOKEN", token)
     os.putenv("SPOTINST_ACCOUNT_ID", account_id)
     os.putenv("CUSTOM_HOST", host)
     os.putenv("SPOTINST_AGENT_PATH", spotinst_agent_path)
     os.chmod(script_full_path, 0o777)
 
+
 def write_creds_path(account_id, creds_file, token, host):
     if account_id is not None:
         creds_file.write('token = ' + token + '\n' + 'account_id = ' + account_id + '\n' + 'host = ' + host)
     else:
         creds_file.write('token = ' + token + '\n' + 'host = ' + host)
 
 
@@ -183,15 +192,15 @@
     return creds_file, creds_path
 
 
 def handle_agent_path(spotinst_agent_path):
     try:
         os.symlink(spotinst_agent_path, '/usr/local/bin/spotinst-agent-service')
     except OSError:
-        print ('Symlink exists. Skipping symlink creation.')
+        print('Symlink exists. Skipping symlink creation.')
     os.chmod(spotinst_agent_path, 0o777)
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Spotinst Agent')
     parser.add_argument('action',
                         action="store",
@@ -217,31 +226,40 @@
                         default='AWS',
                         help='The cloud provider, supports: \'AWS\'(default), \'Azure\', \'Azure_Spot\', \'GCP\'')
     results = parser.parse_args()
     return results
 
 
 def install_worker(modules_path, s3_base_workers_link, worker_name):
-    print ("adding worker " + worker_name)
+    print("adding worker " + worker_name)
     try:
         handle_prerequisites(s3_base_workers_link, worker_name)
         get_worker_files(modules_path, s3_base_workers_link, worker_name)
 
     except Exception as e:
-        print ("Could not get worker " + str(worker_name) + " Exception : " + str(e))
+        print("Could not get worker " + str(worker_name) + " Exception : " + str(e))
 
 
 def install_collector(collector_name, modules_path, s3_base_collectors_link):
-    print ("adding collector " + collector_name)
+    print("adding collector " + collector_name)
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
     py_response = urllib2.urlopen(s3_base_workers_link + '/' + worker_name + '/' + worker_name + '.py')
     yml_response = urllib2.urlopen(s3_base_workers_link + '/' + worker_name + '/' + worker_name + '.yml')
 
     with open(modules_path + '/' + worker_name + '.py', 'wb') as worker:
@@ -255,35 +273,44 @@
         response = urllib2.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.py')
         collector.write(response.read())
     with open(modules_path + '/' + collector_name + '.yml', 'wb') as collector_cfg:
         response = urllib2.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.yml')
         collector_cfg.write(response.read())
 
 
+def get_initiator_files(initiator_name, initiator_modules_path, s3_base_initiator_link):
+    with open(initiator_modules_path + '/' + initiator_name + '.py', 'wb') as initiator:
+        response = urllib2.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.py')
+        initiator.write(response.read())
+    with open(initiator_modules_path + '/' + initiator_name + '.yml', 'wb') as initiator_cfg:
+        response = urllib2.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.yml')
+        initiator_cfg.write(response.read())
+
+
 def handle_prerequisites(s3_base_module_link, module_name):
     try:
         response = urllib2.urlopen(s3_base_module_link + '/' + module_name + '/' + module_name + '.req')
         requirements_file = response.read()
         requirements_names = requirements_file.split("\n")
-        print ("This module requires the following packages to be installed:")
+        print("This module requires the following packages to be installed:")
         for requirement in requirements_names:
-            print (requirement)
+            print(requirement)
 
         if len(requirements_names) > 0:
             import pip
             installed_packages = pip.get_installed_distributions()
             flat_installed_packages = [package.project_name for package in installed_packages]
 
             missing_packages = []
             for requirement in requirements_names:
                 if requirement not in flat_installed_packages:
                     missing_packages.append(requirement)
 
             if len(missing_packages) <= 0:
-                print ("All prerequisites have been met.")
+                print("All prerequisites have been met.")
                 pass
             else:
-                print ("Some prerequisites for this module have not been met. " \
-                       "Please install the following before proceeding: " + str(missing_packages))
+                print("Some prerequisites for this module have not been met. " \
+                      "Please install the following before proceeding: " + str(missing_packages))
                 sys.exit(1)
     except Exception:
         pass
```

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.261/spotinst_agent/taskmanager.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,25 @@
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
@@ -220,14 +231,49 @@
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

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.261/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.261/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.261/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.261/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-1.1.2582/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.261/spotinst_agent/data/installation/agent-init.sh`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,23 @@
 
 	# perform some very rudimentary platform detection
 	if command_exists lsb_release; then
 		os=`cat /etc/system-release | awk -F ' ' {'print $1'}`
 
 		if [ "$os" = "CentOS" ]; then
 			lsb_dist='centos'
-		else
-			vrsn=`cat /etc/debian_version`
+		elif [ -r /etc/debian_version ]; then
+          vrsn=`cat /etc/debian_version`
 
-		    if [ "$vrsn" = "jessie/sid" ]; then
-		    	lsb_dist='ubuntu14'
-		    else
-			    lsb_dist='debian'
-		    fi
+          if [ "$vrsn" = "jessie/sid" ]; then
+            lsb_dist='ubuntu14'
+          else
+            lsb_dist='debian'
+          fi
 		fi
-
 	fi
 	if [ -z "$lsb_dist" ] && [ -r /etc/lsb-release ]; then
 		lsb_dist="$(. /etc/lsb-release && echo "$DISTRIB_ID")"
 	fi
 	if [ -z "$lsb_dist" ] && [ -r /etc/debian_version ]; then
 		vrsn=`cat /etc/debian_version`
```


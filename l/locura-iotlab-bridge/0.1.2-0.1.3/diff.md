# Comparing `tmp/locura_iotlab_bridge-0.1.2.tar.gz` & `tmp/locura_iotlab_bridge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locura_iotlab_bridge-0.1.2.tar", last modified: Mon Dec 12 15:29:12 2022, max compression
+gzip compressed data, was "dist/locura_iotlab_bridge-0.1.3.tar", last modified: Thu Apr 27 14:42:14 2023, max compression
```

## Comparing `locura_iotlab_bridge-0.1.2.tar` & `locura_iotlab_bridge-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2022-12-12 15:29:12.556822 locura_iotlab_bridge-0.1.2/
--rw-r--r--   0 quentin   (1000) quentin   (1000)    21783 2022-12-12 13:41:17.000000 locura_iotlab_bridge-0.1.2/LICENSE
--rw-r--r--   0 quentin   (1000) quentin   (1000)      514 2022-12-12 15:29:12.556822 locura_iotlab_bridge-0.1.2/PKG-INFO
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2022-12-12 15:29:12.556822 locura_iotlab_bridge-0.1.2/locura_iotlab_bridge/
--rw-r--r--   0 quentin   (1000) quentin   (1000)       49 2022-12-12 15:29:01.000000 locura_iotlab_bridge-0.1.2/locura_iotlab_bridge/__init__.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)     1099 2022-12-12 13:04:38.000000 locura_iotlab_bridge-0.1.2/locura_iotlab_bridge/helpers.py
--rwxr-xr-x   0 quentin   (1000) quentin   (1000)     6236 2022-12-12 15:28:34.000000 locura_iotlab_bridge-0.1.2/locura_iotlab_bridge/locura_iotlab_bridge.py
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2022-12-12 15:29:12.556822 locura_iotlab_bridge-0.1.2/locura_iotlab_bridge.egg-info/
--rw-r--r--   0 quentin   (1000) quentin   (1000)      514 2022-12-12 15:29:12.000000 locura_iotlab_bridge-0.1.2/locura_iotlab_bridge.egg-info/PKG-INFO
--rw-r--r--   0 quentin   (1000) quentin   (1000)      345 2022-12-12 15:29:12.000000 locura_iotlab_bridge-0.1.2/locura_iotlab_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2022-12-12 15:29:12.000000 locura_iotlab_bridge-0.1.2/locura_iotlab_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       27 2022-12-12 15:29:12.000000 locura_iotlab_bridge-0.1.2/locura_iotlab_bridge.egg-info/requires.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       21 2022-12-12 15:29:12.000000 locura_iotlab_bridge-0.1.2/locura_iotlab_bridge.egg-info/top_level.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2022-12-12 15:29:12.556822 locura_iotlab_bridge-0.1.2/setup.cfg
--rw-r--r--   0 quentin   (1000) quentin   (1000)      718 2022-12-12 15:29:06.000000 locura_iotlab_bridge-0.1.2/setup.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 14:42:14.000000 locura_iotlab_bridge-0.1.3/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      503 2023-04-27 14:42:14.000000 locura_iotlab_bridge-0.1.3/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      718 2023-04-27 14:38:45.000000 locura_iotlab_bridge-0.1.3/setup.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 14:42:14.000000 locura_iotlab_bridge-0.1.3/locura_iotlab_bridge/
+-rwxr-xr-x   0 quentin   (1000) quentin   (1000)     6550 2023-04-27 14:38:07.000000 locura_iotlab_bridge-0.1.3/locura_iotlab_bridge/locura_iotlab_bridge.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     1099 2022-12-12 13:04:38.000000 locura_iotlab_bridge-0.1.3/locura_iotlab_bridge/helpers.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       49 2022-12-12 15:29:01.000000 locura_iotlab_bridge-0.1.3/locura_iotlab_bridge/__init__.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2023-04-27 14:42:14.000000 locura_iotlab_bridge-0.1.3/setup.cfg
+-rw-r--r--   0 quentin   (1000) quentin   (1000)    21783 2022-12-12 13:41:17.000000 locura_iotlab_bridge-0.1.3/LICENSE
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 14:42:14.000000 locura_iotlab_bridge-0.1.3/locura_iotlab_bridge.egg-info/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      503 2023-04-27 14:42:14.000000 locura_iotlab_bridge-0.1.3/locura_iotlab_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      345 2023-04-27 14:42:14.000000 locura_iotlab_bridge-0.1.3/locura_iotlab_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       21 2023-04-27 14:42:14.000000 locura_iotlab_bridge-0.1.3/locura_iotlab_bridge.egg-info/top_level.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2023-04-27 14:42:14.000000 locura_iotlab_bridge-0.1.3/locura_iotlab_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       27 2023-04-27 14:42:14.000000 locura_iotlab_bridge-0.1.3/locura_iotlab_bridge.egg-info/requires.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `locura_iotlab_bridge-0.1.2/LICENSE` & `locura_iotlab_bridge-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `locura_iotlab_bridge-0.1.2/locura_iotlab_bridge/helpers.py` & `locura_iotlab_bridge-0.1.3/locura_iotlab_bridge/helpers.py`

 * *Files identical despite different names*

### Comparing `locura_iotlab_bridge-0.1.2/locura_iotlab_bridge/locura_iotlab_bridge.py` & `locura_iotlab_bridge-0.1.3/locura_iotlab_bridge/locura_iotlab_bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import paho.mqtt.client as mqtt
 import time
 import json
 import argparse
 import os, sys
 
 class mqttSerialBridge(mqtt.Client) :
-    def __init__(self, nodeList, brokerAddress, username=None, password=None, verbose = None, IDMap=None, port=1883, experimentID = None, clean_session=True, userdata=None, protocol=mqtt.MQTTv311, transport="tcp") :
+    def __init__(self, nodeList, brokerAddress, username=None, password=None, verbose = None, IDMap=None, topicRoot = '',port=1883, experimentID = None, clean_session=True, userdata=None, protocol=mqtt.MQTTv311, transport="tcp") :
         super().__init__(client_id="mqttSerialBridge", clean_session=True, userdata=None, protocol=mqtt.MQTTv311, transport="tcp")
         self.brokerAddress = brokerAddress
         self.port = port
         self.nodeList = nodeList
         self.serialAggregator = SerialAggregator(nodeList, line_handler=self.line_handler)
         if username is not None :
             self.username_pw_set(username, password)
         self.IDMap  = IDMap
         self.rIDMap = {v:k for k,v in IDMap.items()} if not IDMap is None else None
         self.looping = False
         self.verbose = verbose if verbose else 0
+        self.topicRoot = topicRoot if topicRoot[-1] != '/' else topicRoot[:-1]
         
     def start(self):
         # MQTT connect
         self.connect_async(self.brokerAddress, self.port)
         # MQTT loop start
         self.loop_start()
         # serial aggregator start
@@ -52,15 +53,15 @@
             print("Error return code",rc,"on MQTT connect", file=sys.stderr)
             if rc == 5 :
                 print("Check MQTT credentials", file=sys.stderr)
             self.looping = False
             
         # subscribe on specific node topic
         for node in self.nodeList :
-            topic = 'testbed/node/{}/in'.format(node)
+            topic = '{}/{}/in'.format(self.topicRoot, node)
             self.subscribe(topic)
             if self.verbose >= 1 : 
                 print("subscribed to", topic, file=sys.stderr)
         
     def on_message(self, client, userdata, msg) :
         # parse/convert node id from topic and create node identifier
         node = msg.topic.split('/')[2]
@@ -111,14 +112,16 @@
                     help='Verbosity. Specify multiple times for more noise. LI_BRIDGE_VERBOSE environment variable can be used with the same effect.')
     parser.add_argument('-P','--port', action='store', default=int(os.environ['LI_BRIDGE_PORT']),
                     help='Broker port')
     parser.add_argument('-u','--username', action='store', default=os.environ['LI_BRIDGE_USER'],
                     help='username on the broker. Notice : LI_BRIDGE_USER environment variable has the same effect. This argument will override the environment variable')
     parser.add_argument('-p','--password', action='store', default=os.environ['LI_BRIDGE_PWD'],
                     help='password on the broker. Advice : use LI_BRIDGE_PWD environment variable instead. This argument will override the environment variable')
+    parser.add_argument('-t','--topic_root', action='store', default='testbed/node/',
+                    help='root of the topics. Topics used will be <topic_root>/node-id/out[_json] and <topic_root>/node-id/in')
     args = parser.parse_args()
 
     if args.idFile is not None :
         d = ''
         with open(args.idFile,'r') as f :
             for l in f.readlines() :
                 d += l
```

### Comparing `locura_iotlab_bridge-0.1.2/setup.py` & `locura_iotlab_bridge-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='locura_iotlab_bridge',
-    version='0.1.2',    
+    version='0.1.3',    
     description='Bridge to connect LocURa MQTT ecosystem to IOT-LAB',
     url='https://gitlab.irit.fr/rmess/locura/infra/locura_iotlab_bridge',
     author='Quentin Vey',
     author_email='quentin.vey@irit.fr',
     license='CeCILL 2.1',
     packages=['locura_iotlab_bridge'],
     install_requires=['iotlabcli>=3.3.0',
```


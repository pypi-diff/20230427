# Comparing `tmp/alibabacloud_chatbot20220408_py2-1.0.8.tar.gz` & `tmp/alibabacloud_chatbot20220408_py2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_chatbot20220408_py2-1.0.8.tar", last modified: Tue Apr 18 13:01:55 2023, max compression
+gzip compressed data, was "dist/alibabacloud_chatbot20220408_py2-1.0.9.tar", last modified: Thu Apr 27 12:52:42 2023, max compression
```

## Comparing `alibabacloud_chatbot20220408_py2-1.0.8.tar` & `alibabacloud_chatbot20220408_py2-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97927 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/client.py
--rw-r--r--   0 root         (0) root         (0)   399408 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2923 2023-04-18 13:01:55.000000 alibabacloud_chatbot20220408_py2-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      570 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98029 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408/client.py
+-rw-r--r--   0 root         (0) root         (0)   399889 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-04-27 12:52:42.000000 alibabacloud_chatbot20220408_py2-1.0.9/setup.py
```

### Comparing `alibabacloud_chatbot20220408_py2-1.0.8/LICENSE` & `alibabacloud_chatbot20220408_py2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408_py2-1.0.8/PKG-INFO` & `alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_chatbot20220408_py2
-Version: 1.0.8
+Name: alibabacloud-chatbot20220408-py2
+Version: 1.0.9
 Summary: Alibaba Cloud Chatbot (20220408) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_chatbot20220408_py2-1.0.8/README-CN.md` & `alibabacloud_chatbot20220408_py2-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408_py2-1.0.8/README.md` & `alibabacloud_chatbot20220408_py2-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/client.py` & `alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,16 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.intent_name):
             query['IntentName'] = request.intent_name
         if not UtilClient.is_unset(request.knowledge_id):
             query['KnowledgeId'] = request.knowledge_id
         if not UtilClient.is_unset(request.perspective_shrink):
             query['Perspective'] = request.perspective_shrink
+        if not UtilClient.is_unset(request.sand_box):
+            query['SandBox'] = request.sand_box
         if not UtilClient.is_unset(request.sender_id):
             query['SenderId'] = request.sender_id
         if not UtilClient.is_unset(request.sender_nick):
             query['SenderNick'] = request.sender_nick
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
         if not UtilClient.is_unset(request.utterance):
```

### Comparing `alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408/models.py` & `alibabacloud_chatbot20220408_py2-1.0.9/alibabacloud_chatbot20220408/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,20 +579,21 @@
             temp_model = CancelPublishTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ChatRequest(TeaModel):
     def __init__(self, agent_key=None, instance_id=None, intent_name=None, knowledge_id=None, perspective=None,
-                 sender_id=None, sender_nick=None, session_id=None, utterance=None, vendor_param=None):
+                 sand_box=None, sender_id=None, sender_nick=None, session_id=None, utterance=None, vendor_param=None):
         self.agent_key = agent_key  # type: str
         self.instance_id = instance_id  # type: str
         self.intent_name = intent_name  # type: str
         self.knowledge_id = knowledge_id  # type: str
         self.perspective = perspective  # type: list[str]
+        self.sand_box = sand_box  # type: bool
         self.sender_id = sender_id  # type: str
         self.sender_nick = sender_nick  # type: str
         self.session_id = session_id  # type: str
         self.utterance = utterance  # type: str
         self.vendor_param = vendor_param  # type: str
 
     def validate(self):
@@ -610,14 +611,16 @@
             result['InstanceId'] = self.instance_id
         if self.intent_name is not None:
             result['IntentName'] = self.intent_name
         if self.knowledge_id is not None:
             result['KnowledgeId'] = self.knowledge_id
         if self.perspective is not None:
             result['Perspective'] = self.perspective
+        if self.sand_box is not None:
+            result['SandBox'] = self.sand_box
         if self.sender_id is not None:
             result['SenderId'] = self.sender_id
         if self.sender_nick is not None:
             result['SenderNick'] = self.sender_nick
         if self.session_id is not None:
             result['SessionId'] = self.session_id
         if self.utterance is not None:
@@ -634,14 +637,16 @@
             self.instance_id = m.get('InstanceId')
         if m.get('IntentName') is not None:
             self.intent_name = m.get('IntentName')
         if m.get('KnowledgeId') is not None:
             self.knowledge_id = m.get('KnowledgeId')
         if m.get('Perspective') is not None:
             self.perspective = m.get('Perspective')
+        if m.get('SandBox') is not None:
+            self.sand_box = m.get('SandBox')
         if m.get('SenderId') is not None:
             self.sender_id = m.get('SenderId')
         if m.get('SenderNick') is not None:
             self.sender_nick = m.get('SenderNick')
         if m.get('SessionId') is not None:
             self.session_id = m.get('SessionId')
         if m.get('Utterance') is not None:
@@ -649,20 +654,22 @@
         if m.get('VendorParam') is not None:
             self.vendor_param = m.get('VendorParam')
         return self
 
 
 class ChatShrinkRequest(TeaModel):
     def __init__(self, agent_key=None, instance_id=None, intent_name=None, knowledge_id=None,
-                 perspective_shrink=None, sender_id=None, sender_nick=None, session_id=None, utterance=None, vendor_param=None):
+                 perspective_shrink=None, sand_box=None, sender_id=None, sender_nick=None, session_id=None, utterance=None,
+                 vendor_param=None):
         self.agent_key = agent_key  # type: str
         self.instance_id = instance_id  # type: str
         self.intent_name = intent_name  # type: str
         self.knowledge_id = knowledge_id  # type: str
         self.perspective_shrink = perspective_shrink  # type: str
+        self.sand_box = sand_box  # type: bool
         self.sender_id = sender_id  # type: str
         self.sender_nick = sender_nick  # type: str
         self.session_id = session_id  # type: str
         self.utterance = utterance  # type: str
         self.vendor_param = vendor_param  # type: str
 
     def validate(self):
@@ -680,14 +687,16 @@
             result['InstanceId'] = self.instance_id
         if self.intent_name is not None:
             result['IntentName'] = self.intent_name
         if self.knowledge_id is not None:
             result['KnowledgeId'] = self.knowledge_id
         if self.perspective_shrink is not None:
             result['Perspective'] = self.perspective_shrink
+        if self.sand_box is not None:
+            result['SandBox'] = self.sand_box
         if self.sender_id is not None:
             result['SenderId'] = self.sender_id
         if self.sender_nick is not None:
             result['SenderNick'] = self.sender_nick
         if self.session_id is not None:
             result['SessionId'] = self.session_id
         if self.utterance is not None:
@@ -704,14 +713,16 @@
             self.instance_id = m.get('InstanceId')
         if m.get('IntentName') is not None:
             self.intent_name = m.get('IntentName')
         if m.get('KnowledgeId') is not None:
             self.knowledge_id = m.get('KnowledgeId')
         if m.get('Perspective') is not None:
             self.perspective_shrink = m.get('Perspective')
+        if m.get('SandBox') is not None:
+            self.sand_box = m.get('SandBox')
         if m.get('SenderId') is not None:
             self.sender_id = m.get('SenderId')
         if m.get('SenderNick') is not None:
             self.sender_nick = m.get('SenderNick')
         if m.get('SessionId') is not None:
             self.session_id = m.get('SessionId')
         if m.get('Utterance') is not None:
```

### Comparing `alibabacloud_chatbot20220408_py2-1.0.8/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO` & `alibabacloud_chatbot20220408_py2-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-chatbot20220408-py2
-Version: 1.0.8
+Name: alibabacloud_chatbot20220408_py2
+Version: 1.0.9
 Summary: Alibaba Cloud Chatbot (20220408) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_chatbot20220408_py2-1.0.8/setup.py` & `alibabacloud_chatbot20220408_py2-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_chatbot20220408_py2.
 
-Created on 18/04/2023
+Created on 27/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_chatbot20220408"
 NAME = "alibabacloud_chatbot20220408_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Chatbot (20220408) SDK Library for Python2"
```


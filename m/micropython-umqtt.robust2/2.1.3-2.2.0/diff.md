# Comparing `tmp/micropython-umqtt.robust2-2.1.3.tar.gz` & `tmp/micropython-umqtt.robust2-2.2.0.tar.gz`

## Comparing `micropython-umqtt.robust2-2.1.3.tar` & `micropython-umqtt.robust2-2.2.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-rw-r--   0 wojciech  (1000) wojciech  (1000)    10286 2023-04-26 10:25:29.000000 micropython-umqtt.robust2-2.1.3/micropython_umqtt.robust2.egg-info/PKG-INFO
--rw-rw-r--   0 wojciech  (1000) wojciech  (1000)     4492 2023-04-26 10:25:29.000000 micropython-umqtt.robust2-2.1.3/umqtt/robust2.py
--rw-rw-r--   0 wojciech  (1000) wojciech  (1000)        0 2023-04-26 10:25:29.000000 micropython-umqtt.robust2-2.1.3/umqtt/__init__.py
+-rw-rw-r--   0 wojciech  (1000) wojciech  (1000)    10286 2023-04-27 10:23:21.000000 micropython-umqtt.robust2-2.2.0/micropython_umqtt.robust2.egg-info/PKG-INFO
+-rw-rw-r--   0 wojciech  (1000) wojciech  (1000)     4654 2023-04-27 10:23:21.000000 micropython-umqtt.robust2-2.2.0/umqtt/robust2.py
+-rw-rw-r--   0 wojciech  (1000) wojciech  (1000)        0 2023-04-27 10:23:21.000000 micropython-umqtt.robust2-2.2.0/umqtt/__init__.py
```

### Comparing `micropython-umqtt.robust2-2.1.3/micropython_umqtt.robust2.egg-info/PKG-INFO` & `micropython-umqtt.robust2-2.2.0/micropython_umqtt.robust2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: micropython-umqtt.robust2
-Version: 2.1.3
+Version: 2.2.0
 Summary: MQTT client for MicroPython ("robust" version).
 Home-page: https://github.com/fizista/micropython-umqtt.robust2
 Author: Wojciech Banaś
 Author-email: fizista+umqtt.robust2@gmail.com
 License: MIT
 Description: .. role:: bash(code)
            :language: bash
```

### Comparing `micropython-umqtt.robust2-2.1.3/umqtt/robust2.py` & `micropython-umqtt.robust2-2.2.0/umqtt/robust2.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 			D='?','connect','publish','subscribe','reconnect','sendqueue','disconnect','ping','wait_msg','keepalive','check_msg';print('MQTT (%s): %r'%(D[C],B))
 	def reconnect(A):
 		B=A.connect(False)
 		if A.conn_issue:super().disconnect()
 		return B
 	def resubscribe(A):
 		for (B,C) in A.subs:A.subscribe(B,C,False)
+	def things_to_do(A):return len(A.msg_to_send)+len(A.sub_to_send)+sum([len(B)for B in A.msg_to_confirm.values()])+sum([len(B)for B in A.sub_to_confirm.values()])
 	def add_msg_to_send(A,data):
 		C=len(A.msg_to_send);C+=sum(map(len,A.msg_to_confirm.values()))
 		while C>=A.MSG_QUEUE_MAX:
 			E=min(map(lambda x:x[0]if x else 65535,A.msg_to_confirm.values()),default=0)
 			if 0<E<65535:
 				B=None
 				for (F,D) in A.msg_to_confirm.items():
```


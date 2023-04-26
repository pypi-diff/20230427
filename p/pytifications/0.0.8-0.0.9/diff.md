# Comparing `tmp/pytifications-0.0.8.tar.gz` & `tmp/pytifications-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytifications-0.0.8.tar", last modified: Sat Nov 26 00:58:37 2022, max compression
+gzip compressed data, was "pytifications-0.0.9.tar", last modified: Sat Nov 26 20:59:13 2022, max compression
```

## Comparing `pytifications-0.0.8.tar` & `pytifications-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 otaviomaya   (501) staff       (20)        0 2022-11-26 00:58:37.589606 pytifications-0.0.8/
--rw-r--r--   0 otaviomaya   (501) staff       (20)     1068 2022-11-22 17:41:22.000000 pytifications-0.0.8/LICENSE
--rw-r--r--   0 otaviomaya   (501) staff       (20)     2114 2022-11-26 00:58:37.589319 pytifications-0.0.8/PKG-INFO
--rw-r--r--   0 otaviomaya   (501) staff       (20)     1587 2022-11-23 22:35:18.000000 pytifications-0.0.8/README.md
--rw-r--r--   0 otaviomaya   (501) staff       (20)      610 2022-11-26 00:35:53.000000 pytifications-0.0.8/pyproject.toml
--rw-r--r--   0 otaviomaya   (501) staff       (20)       38 2022-11-26 00:58:37.590440 pytifications-0.0.8/setup.cfg
-drwxr-xr-x   0 otaviomaya   (501) staff       (20)        0 2022-11-26 00:58:37.586477 pytifications-0.0.8/src/
-drwxr-xr-x   0 otaviomaya   (501) staff       (20)        0 2022-11-26 00:58:37.588991 pytifications-0.0.8/src/pytifications.egg-info/
--rw-r--r--   0 otaviomaya   (501) staff       (20)     2114 2022-11-26 00:58:37.000000 pytifications-0.0.8/src/pytifications.egg-info/PKG-INFO
--rw-r--r--   0 otaviomaya   (501) staff       (20)      217 2022-11-26 00:58:37.000000 pytifications-0.0.8/src/pytifications.egg-info/SOURCES.txt
--rw-r--r--   0 otaviomaya   (501) staff       (20)        1 2022-11-26 00:58:37.000000 pytifications-0.0.8/src/pytifications.egg-info/dependency_links.txt
--rw-r--r--   0 otaviomaya   (501) staff       (20)       14 2022-11-26 00:58:37.000000 pytifications-0.0.8/src/pytifications.egg-info/top_level.txt
--rw-r--r--   0 otaviomaya   (501) staff       (20)     5893 2022-11-26 00:56:15.000000 pytifications-0.0.8/src/pytifications.py
+drwxr-xr-x   0 otaviomaya   (501) staff       (20)        0 2022-11-26 20:59:13.957926 pytifications-0.0.9/
+-rw-r--r--   0 otaviomaya   (501) staff       (20)     1068 2022-11-22 17:41:22.000000 pytifications-0.0.9/LICENSE
+-rw-r--r--   0 otaviomaya   (501) staff       (20)     2564 2022-11-26 20:59:13.957800 pytifications-0.0.9/PKG-INFO
+-rw-r--r--   0 otaviomaya   (501) staff       (20)     2037 2022-11-26 20:58:28.000000 pytifications-0.0.9/README.md
+-rw-r--r--   0 otaviomaya   (501) staff       (20)      610 2022-11-26 20:59:02.000000 pytifications-0.0.9/pyproject.toml
+-rw-r--r--   0 otaviomaya   (501) staff       (20)       38 2022-11-26 20:59:13.957965 pytifications-0.0.9/setup.cfg
+drwxr-xr-x   0 otaviomaya   (501) staff       (20)        0 2022-11-26 20:59:13.956914 pytifications-0.0.9/src/
+drwxr-xr-x   0 otaviomaya   (501) staff       (20)        0 2022-11-26 20:59:13.957636 pytifications-0.0.9/src/pytifications.egg-info/
+-rw-r--r--   0 otaviomaya   (501) staff       (20)     2564 2022-11-26 20:59:13.000000 pytifications-0.0.9/src/pytifications.egg-info/PKG-INFO
+-rw-r--r--   0 otaviomaya   (501) staff       (20)      217 2022-11-26 20:59:13.000000 pytifications-0.0.9/src/pytifications.egg-info/SOURCES.txt
+-rw-r--r--   0 otaviomaya   (501) staff       (20)        1 2022-11-26 20:59:13.000000 pytifications-0.0.9/src/pytifications.egg-info/dependency_links.txt
+-rw-r--r--   0 otaviomaya   (501) staff       (20)       14 2022-11-26 20:59:13.000000 pytifications-0.0.9/src/pytifications.egg-info/top_level.txt
+-rw-r--r--   0 otaviomaya   (501) staff       (20)     7869 2022-11-26 20:54:22.000000 pytifications-0.0.9/src/pytifications.py
```

### Comparing `pytifications-0.0.8/LICENSE` & `pytifications-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytifications-0.0.8/PKG-INFO` & `pytifications-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: pytifications
-Version: 0.0.8
-Summary: A python package to send notifications via telegram
-Author-email: Knz13 <otaviomaya@gmail.com>
-Project-URL: Homepage, https://github.com/knz13/pytifications
-Project-URL: Bug Tracker, https://github.com/knz13/pytifications/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Pytifications
 
 This is a python package to send messages to your telegram from python code
 
 # Installation
 
 We are on PyPi! just paste this code on terminal
@@ -61,23 +47,47 @@
         PytificationButton(
             text="I'm a button!",
             callback=my_callback_func
         )
     ]
 ])
 ```
+* Editting messages
+```
+message = Pytifications.send_message('message sent from Pytifications!')
+
+#you can simply edit the text
+message.edit(text="Edited text")
+
+#or add buttons (if only the buttons are passed, the message will be kept the same)!
+def some_callback():
+    pass
+
+message.edit(buttons=[
+    [
+        PytificationsButton(
+            text="some callback :D",
+            callback=some_callback
+        )
+    ]
+])
+
+
+```
+
+
 * Edit last message
 ```
 from pytifications import Pytifications
 
 #login and etc...
 
 Pytifications.send_message("hi, i'm not edited!")
 
-#simply edit the last message
+#simply edit the last message from anywhere!
 Pytifications.edit_last_message("now i am!")
 
 #you can also change the buttons on the message!
 
 def do_something():
     print('something done!')
```

### Comparing `pytifications-0.0.8/README.md` & `pytifications-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: pytifications
+Version: 0.0.9
+Summary: A python package to send notifications via telegram
+Author-email: Knz13 <otaviomaya@gmail.com>
+Project-URL: Homepage, https://github.com/knz13/pytifications
+Project-URL: Bug Tracker, https://github.com/knz13/pytifications/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Pytifications
 
 This is a python package to send messages to your telegram from python code
 
 # Installation
 
 We are on PyPi! just paste this code on terminal
@@ -47,23 +61,47 @@
         PytificationButton(
             text="I'm a button!",
             callback=my_callback_func
         )
     ]
 ])
 ```
+* Editting messages
+```
+message = Pytifications.send_message('message sent from Pytifications!')
+
+#you can simply edit the text
+message.edit(text="Edited text")
+
+#or add buttons (if only the buttons are passed, the message will be kept the same)!
+def some_callback():
+    pass
+
+message.edit(buttons=[
+    [
+        PytificationsButton(
+            text="some callback :D",
+            callback=some_callback
+        )
+    ]
+])
+
+
+```
+
+
 * Edit last message
 ```
 from pytifications import Pytifications
 
 #login and etc...
 
 Pytifications.send_message("hi, i'm not edited!")
 
-#simply edit the last message
+#simply edit the last message from anywhere!
 Pytifications.edit_last_message("now i am!")
 
 #you can also change the buttons on the message!
 
 def do_something():
     print('something done!')
```

### Comparing `pytifications-0.0.8/pyproject.toml` & `pytifications-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0","requests"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pytifications"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Knz13", email="otaviomaya@gmail.com" },
 ]
 description = "A python package to send notifications via telegram"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pytifications-0.0.8/src/pytifications.egg-info/PKG-INFO` & `pytifications-0.0.9/src/pytifications.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytifications
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package to send notifications via telegram
 Author-email: Knz13 <otaviomaya@gmail.com>
 Project-URL: Homepage, https://github.com/knz13/pytifications
 Project-URL: Bug Tracker, https://github.com/knz13/pytifications/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -61,23 +61,47 @@
         PytificationButton(
             text="I'm a button!",
             callback=my_callback_func
         )
     ]
 ])
 ```
+* Editting messages
+```
+message = Pytifications.send_message('message sent from Pytifications!')
+
+#you can simply edit the text
+message.edit(text="Edited text")
+
+#or add buttons (if only the buttons are passed, the message will be kept the same)!
+def some_callback():
+    pass
+
+message.edit(buttons=[
+    [
+        PytificationsButton(
+            text="some callback :D",
+            callback=some_callback
+        )
+    ]
+])
+
+
+```
+
+
 * Edit last message
 ```
 from pytifications import Pytifications
 
 #login and etc...
 
 Pytifications.send_message("hi, i'm not edited!")
 
-#simply edit the last message
+#simply edit the last message from anywhere!
 Pytifications.edit_last_message("now i am!")
 
 #you can also change the buttons on the message!
 
 def do_something():
     print('something done!')
```

### Comparing `pytifications-0.0.8/src/pytifications.py` & `pytifications-0.0.9/src/pytifications.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,14 +11,62 @@
 
 @dataclass
 class PytificationButton:
     text: str
     callback: Callable
 
 
+class PytificationsMessage:
+    def __init__(self,message_id):
+
+        self._message_id = message_id
+
+    def edit(self,text: str = "",buttons: List[List[PytificationButton]] =[]): 
+        """
+        Method to edit this message in Telegram
+
+        if only the buttons are passed, the text will be kept the same
+
+        Args:
+            text: (:obj:`str`) message to send instead
+            buttons: (:obj:`List[List[PytificationButton]]`) a list of rows each with a list of columns in that row to be used to align the buttons
+        Returns:
+            :obj:`True` on success and :obj:`False` if no message was sent before
+        """
+
+        if not Pytifications._check_login():
+            return False
+
+        requestedButtons = []
+        for row in buttons:
+            rowButtons = []
+            for column in row:
+                Pytifications._registered_callbacks[column.callback.__name__] = column.callback
+                rowButtons.append({
+                    "callback_name":column.callback.__name__,
+                    "text":column.text
+                })
+             
+            requestedButtons.append(rowButtons)
+
+        request_data = {
+            "username":Pytifications._login,
+            "password_hash":hashlib.sha256(Pytifications._password.encode('utf-8')).hexdigest(),
+            "message_id":self._message_id,
+            "buttons":requestedButtons,
+            "script_id":Pytifications._script_id
+        }
+
+        if text != "":
+            request_data["message"] = text
+        
+        requests.patch('https://pytifications.herokuapp.com/edit_message',json=request_data)
+
+        return True
+
 
 class Pytifications:
     _login = None
     _logged_in = False
     _password = None
     _loop = None
     _registered_callbacks = {}
@@ -86,17 +134,19 @@
 
         make sure to have called Pytifications.login() before,
 
 
         Args:
             message: (:obj:`str`) message to be sent
             buttons: (:obj:`List[List[PytificationButton]]`) a list of rows each with a list of columns in that row to be used to align the buttons
+        Return:
+            False if any errors ocurred or :obj:`PytificationsMessage` if successful
         """
         if not Pytifications._check_login():
-            return
+            return False
 
         requestedButtons = []
         for row in buttons:
             rowButtons = []
             for column in row:
                 Pytifications._registered_callbacks[column.callback.__name__] = column.callback
                 rowButtons.append({
@@ -111,24 +161,28 @@
             "message":message,
             "buttons":requestedButtons,
             "script_id":Pytifications._script_id
         })
 
         if res.status_code != 200:
             print(f'could not send message. reason: {res.reason}')
-            return 
+            return False
 
         Pytifications._last_message_id = int(res.text)
 
         print(f'sent message: "{message}"')
 
-    def edit_last_message(message:str,buttons: List[List[PytificationButton]] = []):
+        return PytificationsMessage(int(res.text))
+
+    def edit_last_message(message:str = "",buttons: List[List[PytificationButton]] = []):
         """
         Use this method to edit the last sent message from this script
 
+        if only the buttons are passed, the text will be kept the same
+
         Args:
             message: (:obj:`str`) message to be sent
             buttons: (:obj:`List[List[PytificationButton]]`) a list of rows each with a list of columns in that row to be used to align the buttons
         Returns:
             :obj:`True` on success and :obj:`False` if no message was sent before
         """
         if not Pytifications._check_login() or Pytifications._last_message_id == None:
@@ -142,22 +196,26 @@
                 rowButtons.append({
                     "callback_name":column.callback.__name__,
                     "text":column.text
                 })
              
             requestedButtons.append(rowButtons)
         
-        requests.patch('https://pytifications.herokuapp.com/edit_message',json={
+        request_data = {
             "username":Pytifications._login,
             "password_hash":hashlib.sha256(Pytifications._password.encode('utf-8')).hexdigest(),
-            "message":message,
             "message_id":Pytifications._last_message_id,
             "buttons":requestedButtons,
             "script_id":Pytifications._script_id
-        })
+        }
+
+        if message != "":
+            request_data["message"] = message
+        
+        requests.patch('https://pytifications.herokuapp.com/edit_message',json=request_data)
 
         return True
         
 
     def _check_login():
         if not Pytifications._logged_in:
             print('could not send pynotification, make sure you have called Pytifications.login("username","password")')
```


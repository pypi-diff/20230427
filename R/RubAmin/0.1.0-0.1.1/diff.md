# Comparing `tmp/RubAmin-0.1.0.tar.gz` & `tmp/RubAmin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RubAmin-0.1.0.tar", last modified: Sun Mar  5 20:36:08 2023, max compression
+gzip compressed data, was "RubAmin-0.1.1.tar", last modified: Thu Apr 27 13:11:50 2023, max compression
```

## Comparing `RubAmin-0.1.0.tar` & `RubAmin-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-05 20:36:08.426002 RubAmin-0.1.0/
--rw-rw-rw-   0        0        0     1089 2023-01-30 20:21:09.000000 RubAmin-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      209 2023-03-05 20:36:08.426002 RubAmin-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-05 20:34:42.000000 RubAmin-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-05 20:36:08.414008 RubAmin-0.1.0/RubAmin/
--rw-rw-rw-   0        0        0      886 2023-03-04 22:12:51.000000 RubAmin-0.1.0/RubAmin/Socket.py
--rw-rw-rw-   0        0        0      117 2023-03-05 20:31:43.000000 RubAmin-0.1.0/RubAmin/__init__.py
--rw-rw-rw-   0        0        0      536 2023-03-04 21:53:09.000000 RubAmin-0.1.0/RubAmin/connections.py
--rw-rw-rw-   0        0        0     1434 2023-03-04 22:12:37.000000 RubAmin-0.1.0/RubAmin/createMethod.py
--rw-rw-rw-   0        0        0     1184 2022-08-26 10:37:26.000000 RubAmin-0.1.0/RubAmin/encryption.py
--rw-rw-rw-   0        0        0       54 2022-08-26 10:37:26.000000 RubAmin-0.1.0/RubAmin/login.py
--rw-rw-rw-   0        0        0      828 2022-08-26 10:37:26.000000 RubAmin-0.1.0/RubAmin/media.py
--rw-rw-rw-   0        0        0    25453 2023-03-05 20:32:35.000000 RubAmin-0.1.0/RubAmin/rubika.py
--rw-rw-rw-   0        0        0     1200 2023-03-05 01:51:38.000000 RubAmin-0.1.0/RubAmin/rubino.py
--rw-rw-rw-   0        0        0     1126 2023-03-04 22:16:41.000000 RubAmin-0.1.0/RubAmin/socket__init__.py
--rw-rw-rw-   0        0        0     1905 2022-08-26 10:37:26.000000 RubAmin-0.1.0/RubAmin/tools.py
-drwxrwxrwx   0        0        0        0 2023-03-05 20:36:08.424001 RubAmin-0.1.0/RubAmin.egg-info/
--rw-rw-rw-   0        0        0      209 2023-03-05 20:36:08.000000 RubAmin-0.1.0/RubAmin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-03-05 20:36:08.000000 RubAmin-0.1.0/RubAmin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-05 20:36:08.000000 RubAmin-0.1.0/RubAmin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-03-05 20:36:08.000000 RubAmin-0.1.0/RubAmin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-05 20:36:08.000000 RubAmin-0.1.0/RubAmin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-05 20:36:08.426002 RubAmin-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      438 2023-03-05 20:31:12.000000 RubAmin-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:11:50.441367 RubAmin-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-01-30 20:21:09.000000 RubAmin-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-04-27 13:11:50.440368 RubAmin-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-05 20:34:42.000000 RubAmin-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 13:11:50.427375 RubAmin-0.1.1/RubAmin/
+-rw-rw-rw-   0        0        0      886 2023-03-05 20:44:48.000000 RubAmin-0.1.1/RubAmin/Socket.py
+-rw-rw-rw-   0        0        0      140 2023-04-27 12:14:22.000000 RubAmin-0.1.1/RubAmin/__init__.py
+-rw-rw-rw-   0        0        0      536 2023-03-05 20:44:48.000000 RubAmin-0.1.1/RubAmin/connections.py
+-rw-rw-rw-   0        0        0     1434 2023-03-05 20:44:48.000000 RubAmin-0.1.1/RubAmin/createMethod.py
+-rw-rw-rw-   0        0        0     1184 2023-03-05 20:44:48.000000 RubAmin-0.1.1/RubAmin/encryption.py
+-rw-rw-rw-   0        0        0       54 2023-03-05 20:44:48.000000 RubAmin-0.1.1/RubAmin/login.py
+-rw-rw-rw-   0        0        0      828 2023-03-05 20:44:48.000000 RubAmin-0.1.1/RubAmin/media.py
+-rw-rw-rw-   0        0        0    29239 2023-04-27 12:22:13.000000 RubAmin-0.1.1/RubAmin/plus.py
+-rw-rw-rw-   0        0        0    25491 2023-04-27 12:28:59.000000 RubAmin-0.1.1/RubAmin/rubika.py
+-rw-rw-rw-   0        0        0     1200 2023-03-05 20:44:48.000000 RubAmin-0.1.1/RubAmin/rubino.py
+-rw-rw-rw-   0        0        0     1126 2023-03-05 20:44:48.000000 RubAmin-0.1.1/RubAmin/socket__init__.py
+-rw-rw-rw-   0        0        0     1905 2023-03-05 20:44:48.000000 RubAmin-0.1.1/RubAmin/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:11:50.438369 RubAmin-0.1.1/RubAmin.egg-info/
+-rw-rw-rw-   0        0        0      209 2023-04-27 13:11:50.000000 RubAmin-0.1.1/RubAmin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-04-27 13:11:50.000000 RubAmin-0.1.1/RubAmin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:11:50.000000 RubAmin-0.1.1/RubAmin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-27 13:11:50.000000 RubAmin-0.1.1/RubAmin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-27 13:11:50.000000 RubAmin-0.1.1/RubAmin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:11:50.441367 RubAmin-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      438 2023-04-27 12:32:32.000000 RubAmin-0.1.1/setup.py
```

### Comparing `RubAmin-0.1.0/LICENSE` & `RubAmin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RubAmin-0.1.0/RubAmin/Socket.py` & `RubAmin-0.1.1/RubAmin/Socket.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.1.0/RubAmin/connections.py` & `RubAmin-0.1.1/RubAmin/connections.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.1.0/RubAmin/createMethod.py` & `RubAmin-0.1.1/RubAmin/createMethod.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.1.0/RubAmin/encryption.py` & `RubAmin-0.1.1/RubAmin/encryption.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.1.0/RubAmin/media.py` & `RubAmin-0.1.1/RubAmin/media.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.1.0/RubAmin/rubika.py` & `RubAmin-0.1.1/RubAmin/rubika.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 		5 ,
 		'getGroupAdminMembers' , 
 		{
 			"group_guid" : group_guid
 		})
 		return loads(self.enc.decrypt(loads(await self.post(self.url , data)).get('data_enc'))).get('data').get('in_chat_members')
 
-	async def sendMessage(self : str , chat_id : str , text : str , metaData = None , message_id : bool = None) -> dict:
+	async def sendMessage(self : str , chat_id : str , text : str , metaData = None , replying_message_id : bool = None) -> dict:
 		'''Using this function, you can send
 		a text message to the desired
 		chat, in the first argument,
 		you must enter the chat ID where
 		the message is to be sent (GUID)
 		and in the second argument,
 		enter your message as a string
@@ -120,15 +120,15 @@
 		click on the message ID,
 		the message that is going
 		to be replied to (not required).'''
 		Input : dict = {
 			"object_guid" : chat_id,
 			"rnd" : f"{randint(100000,999999999)}",
 			"text" : text,
-			"reply_to_message_id" : message_id
+			"reply_to_message_id" : replying_message_id
 		}
 		if metaData != None:
 			Input['metadata'] = {'meta_data_parts' : metaData}
 		mode : list = ['**' , '__' , '``', '@@']
 		for check in mode:
 			if check in text:
 				metadata : list = self.Tool.textAnalysis(text)
@@ -276,20 +276,21 @@
 				"dc_id" : str(dc_id),
 				"file_id" : str(file_id),
 				"file_name" : file_name,
 				"mime" : mime,
 				"size" : size,
 				"type" : "File"
 		}}
-		mode : list = ['**' , '__' , '``']
-		for check in mode:
-			if check in caption:
-				metadata : list = self.Tool.textAnalysis(caption)
-				Input['metadata'] = {'meta_data_parts' : metadata[0]}
-				Input['text'] = metadata[1]
+		if caption:
+			mode : list = ['**' , '__' , '``']
+			for check in mode:
+				if check in caption:
+					metadata : list = self.Tool.textAnalysis(caption)
+					Input['metadata'] = {'meta_data_parts' : metadata[0]}
+					Input['text'] = metadata[1]
 		data : dict = await self.Method.createMethod(5 , 'sendMessage', Input)
 		return loads(self.enc.decrypt(loads(await self.post(self.url , data)).get('data_enc')))
 
 	async def editMessage(self , chat_id : str , message_id : str , text : str , metaData = None) -> dict:
 		'''This method is for editing messages and working with this method is very simple; Enter the chat ID in the first argument, the message ID in the second argument, and the new text in the third argument...'''
 		Input : dict = {
 			"message_id" : message_id,
```

### Comparing `RubAmin-0.1.0/RubAmin/rubino.py` & `RubAmin-0.1.1/RubAmin/rubino.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.1.0/RubAmin/socket__init__.py` & `RubAmin-0.1.1/RubAmin/socket__init__.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.1.0/RubAmin/tools.py` & `RubAmin-0.1.1/RubAmin/tools.py`

 * *Files identical despite different names*


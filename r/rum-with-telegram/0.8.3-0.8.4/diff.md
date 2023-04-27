# Comparing `tmp/rum_with_telegram-0.8.3.tar.gz` & `tmp/rum_with_telegram-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.8.3.tar", last modified: Thu Apr 27 12:06:18 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.8.4.tar", last modified: Thu Apr 27 13:41:29 2023, max compression
```

## Comparing `rum_with_telegram-0.8.3.tar` & `rum_with_telegram-0.8.4.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:06:18.026169 rum_with_telegram-0.8.3/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.3/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-04-27 12:06:18.024174 rum_with_telegram-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 12:06:18.000237 rum_with_telegram-0.8.3/local_test/
--rw-rw-rw-   0        0        0       27 2023-04-26 08:37:26.000000 rum_with_telegram-0.8.3/local_test/__init__.py
--rw-rw-rw-   0        0        0     1559 2023-04-26 08:37:39.000000 rum_with_telegram-0.8.3/local_test/config.py
--rw-rw-rw-   0        0        0      101 2023-04-26 08:37:24.000000 rum_with_telegram-0.8.3/local_test/local_test.py
--rw-rw-rw-   0        0        0      143 2023-04-26 08:37:24.000000 rum_with_telegram-0.8.3/local_test/local_test_rum.py
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-27 12:06:18.011206 rum_with_telegram-0.8.3/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-04-27 11:59:13.000000 rum_with_telegram-0.8.3/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1059 2023-04-27 12:02:26.000000 rum_with_telegram-0.8.3/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    23807 2023-04-27 12:02:26.000000 rum_with_telegram-0.8.3/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.8.3/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.3/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:06:18.022182 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-04-27 12:06:17.000000 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-04-27 12:06:17.000000 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:06:17.000000 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-27 12:06:17.000000 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-27 12:06:17.000000 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 12:06:18.026169 rum_with_telegram-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-04-27 11:59:13.000000 rum_with_telegram-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:41:29.477635 rum_with_telegram-0.8.4/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.4/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-04-27 13:41:29.475617 rum_with_telegram-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.4/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-27 13:41:29.462670 rum_with_telegram-0.8.4/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-04-27 13:41:13.000000 rum_with_telegram-0.8.4/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-04-27 12:59:31.000000 rum_with_telegram-0.8.4/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    23951 2023-04-27 13:40:24.000000 rum_with_telegram-0.8.4/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.8.4/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.4/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:41:29.473622 rum_with_telegram-0.8.4/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-04-27 13:41:29.000000 rum_with_telegram-0.8.4/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-04-27 13:41:29.000000 rum_with_telegram-0.8.4/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:41:29.000000 rum_with_telegram-0.8.4/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-27 13:41:29.000000 rum_with_telegram-0.8.4/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-27 13:41:29.000000 rum_with_telegram-0.8.4/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:41:29.477635 rum_with_telegram-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-04-27 13:41:13.000000 rum_with_telegram-0.8.4/setup.py
```

### Comparing `rum_with_telegram-0.8.3/LICENSE` & `rum_with_telegram-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.3/PKG-INFO` & `rum_with_telegram-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.8.3
+Version: 0.8.4
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.3/rum_with_telegram/config.py` & `rum_with_telegram-0.8.4/rum_with_telegram/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,27 +8,27 @@
     BLACK_LIST_PUBKEYS: list
     BLACK_LIST_TGIDS: list
     ADMIN_USERIDS: list
     RUM_SEED: str
     ETH_PVTKEY: str
     FEED_URL_BASE: str
     FEED_TITLE: str
-    TG_USER_ID: int
     TG_CHANNEL_NAME: str
     TG_CHANNEL_URL: str
-    TG_CHANNEL_ID: int
     TG_BOT_TOKEN: str
     TG_BOT_NAME: str
     TG_GROUP_NAME: str
-    TG_GROUP_ID: int
     DB_URL: str
     DB_ECHO: bool
     RUM_DELAY_HOURS: int
     RUM_POST_FOOTER: str
     TG_REPLY_POSTURL: bool
+    TG_USER_ID: int
+    TG_CHANNEL_ID: int = None
+    TG_GROUP_ID: int = None
 
 
 def read_json(json_file: str):
     with open(json_file, "r", encoding="utf-8") as f:
         data = json.load(f)
     return data
```

### Comparing `rum_with_telegram-0.8.3/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.8.4/rum_with_telegram/data_exchanger.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,16 @@
             )
             return
         _first_name = update.message.from_user.first_name
         _last_name = update.message.from_user.last_name
         _fullname = f"{_first_name} {_last_name}" if _last_name else _first_name
         _text = update.message.text or update.message.caption or ""
         if _text.startswith("/profile"):
-            return self.command_profile(update, context)
+            await self.command_profile(update, context)
+            return
         text = f"{_text}\n\nFrom {_fullname} through {self.config.TG_BOT_NAME}"
         _photo = update.message.photo
         if _photo:
             image = await context.bot.get_file(_photo[-1].file_id)
             image = bytes(await image.download_as_bytearray())
             resp = await context.bot.send_photo(
                 chat_id=self.config.TG_CHANNEL_NAME, photo=image, caption=text
@@ -449,15 +450,15 @@
         logger.info("start command_show_pvtkey")
         userid = update.message.from_user.id
         username = update.message.from_user.username
         chat_id = update.message.chat_id
         message_id = update.message.message_id
         user = self.db.init_user(userid, username)
         if user:
-            text = f"Your private key is: \n```\n{user.pvtkey}\n```\nPlease keep it safe."
+            text = f"Your private key (please keep it safe) is: \n```\n{user.pvtkey}\n```\nYour Address (can show to others) is:\n```\n{user.address}\n```"
         else:
             text = f"show_key error {userid}"
         await context.bot.send_message(
             chat_id=chat_id,
             text=text,
             reply_to_message_id=message_id,
             parse_mode="Markdown",
@@ -467,15 +468,15 @@
         logger.info("start command_new_pvtkey")
         userid = update.message.from_user.id
         username = update.message.from_user.username
         chat_id = update.message.chat_id
         message_id = update.message.message_id
         user = self.db.init_user(userid, username, is_cover=True)
         if user:
-            text = f"Your new private key is: \n```\n{ user.pvtkey}\n```\nPlease keep it safe."
+            text = f"Your private key (please keep it safe) is: \n```\n{user.pvtkey}\n```\nYour Address (can show to others) is:\n```\n{user.address}\n```"
         else:
             text = f"new_key error {userid}"
 
         await context.bot.send_message(
             chat_id=chat_id,
             text=text,
             reply_to_message_id=message_id,
```

### Comparing `rum_with_telegram-0.8.3/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.8.4/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.3/rum_with_telegram/module.py` & `rum_with_telegram-0.8.4/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.3/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.8.4/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.8.3
+Version: 0.8.4
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.3/setup.py` & `rum_with_telegram-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.8.3",
+    version="0.8.4",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```


# Comparing `tmp/rum_with_telegram-0.8.2.tar.gz` & `tmp/rum_with_telegram-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.8.2.tar", last modified: Wed Apr 26 09:35:07 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.8.3.tar", last modified: Thu Apr 27 12:06:18 2023, max compression
```

## Comparing `rum_with_telegram-0.8.2.tar` & `rum_with_telegram-0.8.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 09:35:07.946800 rum_with_telegram-0.8.2/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.2/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-04-26 09:35:07.944806 rum_with_telegram-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 09:35:07.917877 rum_with_telegram-0.8.2/local_test/
--rw-rw-rw-   0        0        0       27 2023-04-26 08:37:26.000000 rum_with_telegram-0.8.2/local_test/__init__.py
--rw-rw-rw-   0        0        0     1559 2023-04-26 08:37:39.000000 rum_with_telegram-0.8.2/local_test/config.py
--rw-rw-rw-   0        0        0      101 2023-04-26 08:37:24.000000 rum_with_telegram-0.8.2/local_test/local_test.py
--rw-rw-rw-   0        0        0      143 2023-04-26 08:37:24.000000 rum_with_telegram-0.8.2/local_test/local_test_rum.py
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-26 09:35:07.929846 rum_with_telegram-0.8.2/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-04-26 09:34:21.000000 rum_with_telegram-0.8.2/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1038 2023-04-26 09:33:02.000000 rum_with_telegram-0.8.2/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    23598 2023-04-26 09:33:06.000000 rum_with_telegram-0.8.2/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.8.2/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.2/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-04-26 09:35:07.942815 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-04-26 09:35:07.000000 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-04-26 09:35:07.000000 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 09:35:07.000000 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-26 09:35:07.000000 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-26 09:35:07.000000 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 09:35:07.946800 rum_with_telegram-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-04-26 09:34:33.000000 rum_with_telegram-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:06:18.026169 rum_with_telegram-0.8.3/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-04-27 12:06:18.024174 rum_with_telegram-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 12:06:18.000237 rum_with_telegram-0.8.3/local_test/
+-rw-rw-rw-   0        0        0       27 2023-04-26 08:37:26.000000 rum_with_telegram-0.8.3/local_test/__init__.py
+-rw-rw-rw-   0        0        0     1559 2023-04-26 08:37:39.000000 rum_with_telegram-0.8.3/local_test/config.py
+-rw-rw-rw-   0        0        0      101 2023-04-26 08:37:24.000000 rum_with_telegram-0.8.3/local_test/local_test.py
+-rw-rw-rw-   0        0        0      143 2023-04-26 08:37:24.000000 rum_with_telegram-0.8.3/local_test/local_test_rum.py
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-27 12:06:18.011206 rum_with_telegram-0.8.3/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-04-27 11:59:13.000000 rum_with_telegram-0.8.3/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1059 2023-04-27 12:02:26.000000 rum_with_telegram-0.8.3/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    23807 2023-04-27 12:02:26.000000 rum_with_telegram-0.8.3/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.8.3/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.3/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:06:18.022182 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-04-27 12:06:17.000000 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-04-27 12:06:17.000000 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 12:06:17.000000 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-27 12:06:17.000000 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-27 12:06:17.000000 rum_with_telegram-0.8.3/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 12:06:18.026169 rum_with_telegram-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-04-27 11:59:13.000000 rum_with_telegram-0.8.3/setup.py
```

### Comparing `rum_with_telegram-0.8.2/LICENSE` & `rum_with_telegram-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.2/PKG-INFO` & `rum_with_telegram-0.8.3/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rum_with_telegram
-Version: 0.8.2
+Name: rum-with-telegram
+Version: 0.8.3
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.2/local_test/config.py` & `rum_with_telegram-0.8.3/local_test/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.2/rum_with_telegram/config.py` & `rum_with_telegram-0.8.3/rum_with_telegram/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,25 +23,25 @@
     DB_URL: str
     DB_ECHO: bool
     RUM_DELAY_HOURS: int
     RUM_POST_FOOTER: str
     TG_REPLY_POSTURL: bool
 
 
-def read_json(json_file):
+def read_json(json_file: str):
     with open(json_file, "r", encoding="utf-8") as f:
         data = json.load(f)
     return data
 
 
-def write_json(json_file, data):
+def write_json(json_file: str, data: dict):
     with open(json_file, "w", encoding="utf-8") as f:
         json.dump(data, f, ensure_ascii=False, indent=4)
     return data
 
 
-def get_config(json_file):
+def get_config(json_file: str):
     if not os.path.exists(json_file):
         raise FileNotFoundError(f"Config file not found: {json_file}")
     data = read_json(json_file)
     config = Config(**data)
     return config
```

### Comparing `rum_with_telegram-0.8.2/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.8.3/rum_with_telegram/data_exchanger.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         userid,
         reply_to_message_id,
         rum_post_url,
     ):
         """reply to user with rum post url"""
         if not self.config.TG_REPLY_POSTURL:
             return
-        reply = f"⚜️ Success to blockchain.\n👉[{self.config.FEED_TITLE}]({rum_post_url})\n" + (
+        reply = f"⚜️ Success to blockchain.\n👉[{self.config.FEED_TITLE}]({rum_post_url})" + (
             extend_text or ""
         )
         await context.bot.send_message(
             chat_id=userid,
             text=reply,
             parse_mode="Markdown",
             disable_web_page_preview=True,
@@ -237,15 +237,15 @@
                 "chat_message_id": message_id,
                 "channel_message_id": resp.message_id,
             }
         )
         self.db.add_or_update(Relation, relation, "trx_id")
         await self._comment_with_feedurl(
             context,
-            f" and to channel {self.config.TG_CHANNEL_NAME}",
+            f" and to [{self.config.TG_CHANNEL_NAME}]({self.config.TG_CHANNEL_URL}/{resp.message_id})",
             userid,
             message_id,
             relation.get("rum_post_url"),
         )
 
     async def _handle_channel_post(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         """send message to rum group"""
@@ -275,21 +275,25 @@
             return
         logger.info("handle_channel_message %s", update.message.message_id)
         channel_message_id = update.message.forward_from_message_id
         chat_message_id = update.message.message_id
 
         # send reply to user in group chat
         for i in range(5):
-            rum_post_url = self.db.get_trx_sent(channel_message_id).rum_post_url
+            obj = self.db.get_trx_sent(channel_message_id)
+            if not obj:
+                await asyncio.sleep(0.5)
+                continue
+            rum_post_url = obj.rum_post_url
             if not rum_post_url:
-                logger.warning("%s not found channel_message_id %s", i, channel_message_id)
                 await asyncio.sleep(0.5)
             else:
                 break
         if not rum_post_url:
+            logger.warning("%s not found channel_message_id %s", i, channel_message_id)
             return
         logger.info("found rum_post_url %s", rum_post_url)
         await self._comment_with_feedurl(
             context, "", update.message.chat.id, chat_message_id, rum_post_url
         )
         payload = {
             "chat_message_id": chat_message_id,
@@ -303,22 +307,23 @@
         username = update.message.from_user.username
         userid = update.message.from_user.id
         reply_msg = update.message.reply_to_message
         channel_message_id = reply_msg.forward_from_message_id
         reply_chat_message_id = reply_msg.message_id
         reply_id = None
         if channel_message_id:
-            reply_id = self.db.get_trx_sent(channel_message_id).rum_post_id
+            obj = self.db.get_trx_sent(channel_message_id)
+            reply_id = obj.rum_post_id if obj else None
         elif reply_chat_message_id:
             obj = self.db.get_first(
                 Relation,
                 {"chat_message_id": reply_chat_message_id},
                 "chat_message_id",
             )
-            reply_id = obj.rum_post_id
+            reply_id = obj.rum_post_id if obj else None
             if obj and not channel_message_id:
                 channel_message_id = obj.channel_message_id
 
         if not channel_message_id and not reply_chat_message_id:
             bot = Bot(token=context.bot.token)
             _pinned = await bot.get_chat(self.config.TG_GROUP_ID)
             _pinned = _pinned.pinned_message
```

### Comparing `rum_with_telegram-0.8.2/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.8.3/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.2/rum_with_telegram/module.py` & `rum_with_telegram-0.8.3/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.2/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.8.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rum-with-telegram
-Version: 0.8.2
+Name: rum_with_telegram
+Version: 0.8.3
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.2/setup.py` & `rum_with_telegram-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.8.2",
+    version="0.8.3",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```


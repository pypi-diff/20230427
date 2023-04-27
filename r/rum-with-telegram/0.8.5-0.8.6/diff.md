# Comparing `tmp/rum_with_telegram-0.8.5.tar.gz` & `tmp/rum_with_telegram-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.8.5.tar", last modified: Thu Apr 27 15:23:37 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.8.6.tar", last modified: Thu Apr 27 15:26:21 2023, max compression
```

## Comparing `rum_with_telegram-0.8.5.tar` & `rum_with_telegram-0.8.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:23:37.748786 rum_with_telegram-0.8.5/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.5/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-04-27 15:23:37.747789 rum_with_telegram-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.5/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-27 15:23:37.731833 rum_with_telegram-0.8.5/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-04-27 15:23:10.000000 rum_with_telegram-0.8.5/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-04-27 12:59:31.000000 rum_with_telegram-0.8.5/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    23948 2023-04-27 15:22:59.000000 rum_with_telegram-0.8.5/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.8.5/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.5/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:23:37.744797 rum_with_telegram-0.8.5/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-04-27 15:23:37.000000 rum_with_telegram-0.8.5/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-04-27 15:23:37.000000 rum_with_telegram-0.8.5/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:23:37.000000 rum_with_telegram-0.8.5/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-27 15:23:37.000000 rum_with_telegram-0.8.5/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-27 15:23:37.000000 rum_with_telegram-0.8.5/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 15:23:37.748786 rum_with_telegram-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-04-27 15:23:10.000000 rum_with_telegram-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:21.647324 rum_with_telegram-0.8.6/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.6/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-04-27 15:26:21.646350 rum_with_telegram-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.6/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:21.634358 rum_with_telegram-0.8.6/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-04-27 15:25:09.000000 rum_with_telegram-0.8.6/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-04-27 12:59:31.000000 rum_with_telegram-0.8.6/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    23983 2023-04-27 15:24:57.000000 rum_with_telegram-0.8.6/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.8.6/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.6/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:21.644356 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-04-27 15:26:21.000000 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-04-27 15:26:21.000000 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 15:26:21.000000 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-27 15:26:21.000000 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-27 15:26:21.000000 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 15:26:21.648321 rum_with_telegram-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-04-27 15:25:09.000000 rum_with_telegram-0.8.6/setup.py
```

### Comparing `rum_with_telegram-0.8.5/LICENSE` & `rum_with_telegram-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.5/PKG-INFO` & `rum_with_telegram-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.8.5
+Version: 0.8.6
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.5/rum_with_telegram/config.py` & `rum_with_telegram-0.8.6/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.5/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.8.6/rum_with_telegram/data_exchanger.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,13 +556,13 @@
                 self.handle_channel_message,
             )
         )
         # group message:
         # send to rum group as comment of the pinned post or the reply-to post
         self.app.add_handler(
             MessageHandler(
-                content_filter & filters.ChatType.SUPERGROUP,
+                content_filter & (filters.ChatType.SUPERGROUP | filters.SenderChat.SUPER_GROUP),
                 self.handle_group_message,
             )
         )
 
         self.app.run_polling()
```

### Comparing `rum_with_telegram-0.8.5/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.8.6/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.5/rum_with_telegram/module.py` & `rum_with_telegram-0.8.6/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.5/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.8.6/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.8.5
+Version: 0.8.6
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.5/setup.py` & `rum_with_telegram-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.8.5",
+    version="0.8.6",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```


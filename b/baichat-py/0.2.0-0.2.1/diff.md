# Comparing `tmp/baichat_py-0.2.0.tar.gz` & `tmp/baichat_py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baichat_py-0.2.0.tar", max compression
+gzip compressed data, was "baichat_py-0.2.1.tar", max compression
```

## Comparing `baichat_py-0.2.0.tar` & `baichat_py-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1062 2023-04-27 10:27:07.676039 baichat_py-0.2.0/README.md
--rw-r--r--   0        0        0     5711 2023-04-27 10:26:33.227998 baichat_py-0.2.0/baichat_py/__init__.py
--rw-r--r--   0        0        0     1040 2023-04-27 10:27:17.408061 baichat_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 baichat_py-0.2.0/setup.py
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 baichat_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-27 10:27:07.676039 baichat_py-0.2.1/README.md
+-rw-r--r--   0        0        0     5807 2023-04-27 10:32:59.034118 baichat_py-0.2.1/baichat_py/__init__.py
+-rw-r--r--   0        0        0     1040 2023-04-27 10:33:03.116176 baichat_py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 baichat_py-0.2.1/setup.py
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 baichat_py-0.2.1/PKG-INFO
```

### Comparing `baichat_py-0.2.0/README.md` & `baichat_py-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `baichat_py-0.2.0/baichat_py/__init__.py` & `baichat_py-0.2.1/baichat_py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __version_tuple__ = tuple(map(int, __version__.split(".")))
 
 
 import os
 from pathlib import Path
 import json
 import random
@@ -70,19 +70,23 @@
 
     def __init__(
         self,
         url: str = None,
         config_file: Path = None,
         api_url: str = None,
         loop: asyncio.AbstractEventLoop = None,
+        sync: bool = False,
     ):
         self.url: str = self.URL if url is None else url
         self.api_url: str = self.API_URL if api_url is None else api_url
 
-        self.loop = asyncio.get_event_loop() if loop is None else loop
+        if not sync:
+            self.loop = asyncio.get_event_loop() if loop is None else loop
+        else:
+            self.loop = None
 
         self.config_file: Path = (
             self.CONFIG_FILE if config_file is None else config_file
         )
 
         self.create_config_dir_if_doesnt_exist()
```

### Comparing `baichat_py-0.2.0/pyproject.toml` & `baichat_py-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baichat-py"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["0xMRTT <0xMRTT@proton.me>"]
 maintainers = ["0xMRTT <0xMRTT@proton.me>"]
 readme = "README.md"
 packages = [{include = "baichat_py"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/Bavarder/baichat-py"
```

### Comparing `baichat_py-0.2.0/setup.py` & `baichat_py-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0']
 
 setup_kwargs = {
     'name': 'baichat-py',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': '',
     'long_description': '# BAIChat API Python\n\n## Installation\n\nYou can install it from PyPi\n\n``` shell\npip install baichat-py\n```\n\n## Usage\n\n### Async\n\n``` python\nimport asyncio\n\nloop = asyncio.get_event_loop() \nhello = loop.run_until_complete(chat.async_ask("Hi"))\n\nprint(hello.text)\n\n# => Hello! How can I assist you today?\n```\n\n### Context manager\n\n``` python\nwith BAIChat() as (loop, chat):\n    hello = chat.ask("Hi")\n\n    print(hello.text)\n\n# => Hello! How can I assist you today?\n```\n\n### Delta\n\n``` python\nwith BAIChat() as (loop, chat):\n    hello = chat.ask("Hi")\n\n    for delta in hello:\n        print(delta.text)\n    \n# => Hello\n# => Hello!\n# => Hello! How\n# => Hello! How may\n# => Hello! How may I\n# => Hello! How may I assist\n# => Hello! How may I assist you\n# => Hello! How may I assist you today\n# => Hello! How may I assist you today?\n```\n\n### Sync\n\n``` python\nchat = BAIChat()\nprint(chat.sync_ask("Hello, how are you?").text)\n\n# => Hello! As an AI language model, I don\'t have feelings, but I\'m functioning properly and ready to assist you. How may I help you today?\n```',
     'author': '0xMRTT',
     'author_email': '0xMRTT@proton.me',
     'maintainer': '0xMRTT',
     'maintainer_email': '0xMRTT@proton.me',
     'url': 'https://github.com/Bavarder/baichat-py',
```

### Comparing `baichat_py-0.2.0/PKG-INFO` & `baichat_py-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baichat-py
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Home-page: https://github.com/Bavarder/baichat-py
 License: GPL-3.0-or-later
 Keywords: openai,gpt3,baichat,chat
 Author: 0xMRTT
 Author-email: 0xMRTT@proton.me
 Maintainer: 0xMRTT
```


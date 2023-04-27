# Comparing `tmp/baichat_py-0.1.0.tar.gz` & `tmp/baichat_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baichat_py-0.1.0.tar", max compression
+gzip compressed data, was "baichat_py-0.2.0.tar", max compression
```

## Comparing `baichat_py-0.1.0.tar` & `baichat_py-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,5 @@
--rw-r--r--   0        0        0      831 2023-04-26 11:57:18.910560 baichat_py-0.1.0/README.md
--rw-r--r--   0        0        0        1 2023-04-26 11:59:45.478639 baichat_py-0.1.0/baichat_py/.ruff_cache/.gitignore
--rw-r--r--   0        0        0        8 2023-04-26 11:59:45.789644 baichat_py-0.1.0/baichat_py/.ruff_cache/.update-informer
--rw-r--r--   0        0        0       43 2023-04-26 11:59:45.478639 baichat_py-0.1.0/baichat_py/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      352 2023-04-26 12:01:11.011901 baichat_py-0.1.0/baichat_py/.ruff_cache/content/6b7098ae2beac324
--rw-r--r--   0        0        0      104 2023-04-26 12:02:12.543826 baichat_py-0.1.0/baichat_py/.ruff_cache/content/f84725b5df0f747c
--rw-r--r--   0        0        0     4580 2023-04-26 12:02:50.251400 baichat_py-0.1.0/baichat_py/__init__.py
--rw-r--r--   0        0        0     1040 2023-04-26 11:55:58.958479 baichat_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 baichat_py-0.1.0/setup.py
--rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 baichat_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-27 10:27:07.676039 baichat_py-0.2.0/README.md
+-rw-r--r--   0        0        0     5711 2023-04-27 10:26:33.227998 baichat_py-0.2.0/baichat_py/__init__.py
+-rw-r--r--   0        0        0     1040 2023-04-27 10:27:17.408061 baichat_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 baichat_py-0.2.0/setup.py
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 baichat_py-0.2.0/PKG-INFO
```

### Comparing `baichat_py-0.1.0/README.md` & `baichat_py-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BAIChat API Python
 
 ## Installation
 
 You can install it from PyPi
 
 ``` shell
-pip install baichat_py
+pip install baichat-py
 ```
 
 ## Usage
 
 ### Async
 
 ``` python
@@ -50,7 +50,15 @@
 # => Hello! How may I
 # => Hello! How may I assist
 # => Hello! How may I assist you
 # => Hello! How may I assist you today
 # => Hello! How may I assist you today?
 ```
 
+### Sync
+
+``` python
+chat = BAIChat()
+print(chat.sync_ask("Hello, how are you?").text)
+
+# => Hello! As an AI language model, I don't have feelings, but I'm functioning properly and ready to assist you. How may I help you today?
+```
```

### Comparing `baichat_py-0.1.0/baichat_py/__init__.py` & `baichat_py-0.2.0/baichat_py/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __version_tuple__ = tuple(map(int, __version__.split(".")))
 
 
 import os
 from pathlib import Path
 import json
 import random
 import string
 import aiohttp
 import asyncio
+import http.client
 
 
 class BAIChatDelta:
     def __init__(self, data: dict):
         self.data = data
 
     @property
@@ -144,22 +145,49 @@
             "Referer": "https://chatbot.theb.ai",
             "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/112.0",
             "Content-Type": "application/json",
         }
         async with aiohttp.ClientSession(headers=headers) as session:
             return await self.get_data_async(session, prompt)
 
+    def sync_ask(self, prompt: str) -> BAIChatResponse:
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Accept-Language": "en-US,en;q=0.5",
+            "Host": "chatbot.theb.ai",
+            "Origin": "https://chatbot.theb.ai",
+            "Referer": "https://chatbot.theb.ai",
+            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/112.0",
+            "Content-Type": "application/json",
+        }
+        conn = http.client.HTTPSConnection('chatbot.theb.ai') 
+        prompt = prompt.replace('"', "\n")
+
+        if self.chat_id == "":
+            self.chat_id = f"chatcmpl-{self.get_random_string()}"
+
+        payload = json.dumps(
+            {"prompt": prompt, "options": {"parentMessageId": self.chat_id}}
+        )
+        conn.request('POST', '/api/chat-process', payload,  headers=headers)
+
+        response = conn.getresponse()
+        result = response.read().decode('utf-8')
+        result = result.splitlines()
+        result = BAIChatResponse([json.loads(line) for line in result])
+
+        self.chat_id = result.id
+        return result
+
     def ask(self, prompt: str) -> BAIChatResponse:
         return self.loop.run_until_complete(self.async_ask(prompt))
 
     def __enter__(self):
         return (self.loop, self)
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         self.save_config()
 
 
 if __name__ == "__main__":
-    with BAIChat() as (loop, chat):
-        hello = chat.ask("Hi")
-
-        print(hello.text)
+    chat = BAIChat()
+    print(chat.sync_ask("Hello, how are you?").text)
```

### Comparing `baichat_py-0.1.0/pyproject.toml` & `baichat_py-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baichat-py"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["0xMRTT <0xMRTT@proton.me>"]
 maintainers = ["0xMRTT <0xMRTT@proton.me>"]
 readme = "README.md"
 packages = [{include = "baichat_py"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/Bavarder/baichat-py"
```

### Comparing `baichat_py-0.1.0/setup.py` & `baichat_py-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['baichat_py']
 
 package_data = \
-{'': ['*'], 'baichat_py': ['.ruff_cache/*', '.ruff_cache/content/*']}
+{'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0']
 
 setup_kwargs = {
     'name': 'baichat-py',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
-    'long_description': '# BAIChat API Python\n\n## Installation\n\nYou can install it from PyPi\n\n``` shell\npip install baichat_py\n```\n\n## Usage\n\n### Async\n\n``` python\nimport asyncio\n\nloop = asyncio.get_event_loop() \nhello = loop.run_until_complete(chat.async_ask("Hi"))\n\nprint(hello.text)\n\n# => Hello! How can I assist you today?\n```\n\n### Context manager\n\n``` python\nwith BAIChat() as (loop, chat):\n    hello = chat.ask("Hi")\n\n    print(hello.text)\n\n# => Hello! How can I assist you today?\n```\n\n### Delta\n\n``` python\nwith BAIChat() as (loop, chat):\n    hello = chat.ask("Hi")\n\n    for delta in hello:\n        print(delta.text)\n    \n# => Hello\n# => Hello!\n# => Hello! How\n# => Hello! How may\n# => Hello! How may I\n# => Hello! How may I assist\n# => Hello! How may I assist you\n# => Hello! How may I assist you today\n# => Hello! How may I assist you today?\n```\n\n',
+    'long_description': '# BAIChat API Python\n\n## Installation\n\nYou can install it from PyPi\n\n``` shell\npip install baichat-py\n```\n\n## Usage\n\n### Async\n\n``` python\nimport asyncio\n\nloop = asyncio.get_event_loop() \nhello = loop.run_until_complete(chat.async_ask("Hi"))\n\nprint(hello.text)\n\n# => Hello! How can I assist you today?\n```\n\n### Context manager\n\n``` python\nwith BAIChat() as (loop, chat):\n    hello = chat.ask("Hi")\n\n    print(hello.text)\n\n# => Hello! How can I assist you today?\n```\n\n### Delta\n\n``` python\nwith BAIChat() as (loop, chat):\n    hello = chat.ask("Hi")\n\n    for delta in hello:\n        print(delta.text)\n    \n# => Hello\n# => Hello!\n# => Hello! How\n# => Hello! How may\n# => Hello! How may I\n# => Hello! How may I assist\n# => Hello! How may I assist you\n# => Hello! How may I assist you today\n# => Hello! How may I assist you today?\n```\n\n### Sync\n\n``` python\nchat = BAIChat()\nprint(chat.sync_ask("Hello, how are you?").text)\n\n# => Hello! As an AI language model, I don\'t have feelings, but I\'m functioning properly and ready to assist you. How may I help you today?\n```',
     'author': '0xMRTT',
     'author_email': '0xMRTT@proton.me',
     'maintainer': '0xMRTT',
     'maintainer_email': '0xMRTT@proton.me',
     'url': 'https://github.com/Bavarder/baichat-py',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `baichat_py-0.1.0/PKG-INFO` & `baichat_py-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baichat-py
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/Bavarder/baichat-py
 License: GPL-3.0-or-later
 Keywords: openai,gpt3,baichat,chat
 Author: 0xMRTT
 Author-email: 0xMRTT@proton.me
 Maintainer: 0xMRTT
@@ -29,15 +29,15 @@
 # BAIChat API Python
 
 ## Installation
 
 You can install it from PyPi
 
 ``` shell
-pip install baichat_py
+pip install baichat-py
 ```
 
 ## Usage
 
 ### Async
 
 ``` python
@@ -78,8 +78,15 @@
 # => Hello! How may I
 # => Hello! How may I assist
 # => Hello! How may I assist you
 # => Hello! How may I assist you today
 # => Hello! How may I assist you today?
 ```
 
+### Sync
 
+``` python
+chat = BAIChat()
+print(chat.sync_ask("Hello, how are you?").text)
+
+# => Hello! As an AI language model, I don't have feelings, but I'm functioning properly and ready to assist you. How may I help you today?
+```
```


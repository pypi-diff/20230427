# Comparing `tmp/gpt-term-1.0.0.tar.gz` & `tmp/gpt-term-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-term-1.0.0.tar", last modified: Sun Apr 23 15:38:21 2023, max compression
+gzip compressed data, was "gpt-term-1.0.1.tar", last modified: Thu Apr 27 08:09:04 2023, max compression
```

## Comparing `gpt-term-1.0.0.tar` & `gpt-term-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:38:21.735917 gpt-term-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 15:38:10.000000 gpt-term-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-04-23 15:38:21.735917 gpt-term-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-23 15:38:10.000000 gpt-term-1.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-04-23 15:38:10.000000 gpt-term-1.0.0/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-23 15:38:10.000000 gpt-term-1.0.0/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:38:21.735917 gpt-term-1.0.0/gpt_term/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 15:38:10.000000 gpt-term-1.0.0/gpt_term/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43386 2023-04-23 15:38:10.000000 gpt-term-1.0.0/gpt_term/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:38:21.735917 gpt-term-1.0.0/gpt_term.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-04-23 15:38:21.000000 gpt-term-1.0.0/gpt_term.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-23 15:38:21.000000 gpt-term-1.0.0/gpt_term.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:38:21.000000 gpt-term-1.0.0/gpt_term.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 15:38:21.000000 gpt-term-1.0.0/gpt_term.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-23 15:38:21.000000 gpt-term-1.0.0/gpt_term.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 15:38:21.000000 gpt-term-1.0.0/gpt_term.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 15:38:21.735917 gpt-term-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-23 15:38:10.000000 gpt-term-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:09:04.922674 gpt-term-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-27 08:08:52.000000 gpt-term-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 08:08:52.000000 gpt-term-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-04-27 08:09:04.922674 gpt-term-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-27 08:08:52.000000 gpt-term-1.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-04-27 08:08:52.000000 gpt-term-1.0.1/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:09:04.918673 gpt-term-1.0.1/gpt_term/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 08:08:52.000000 gpt-term-1.0.1/gpt_term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-27 08:08:52.000000 gpt-term-1.0.1/gpt_term/config.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43634 2023-04-27 08:08:52.000000 gpt-term-1.0.1/gpt_term/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:09:04.922674 gpt-term-1.0.1/gpt_term.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 08:09:04.000000 gpt-term-1.0.1/gpt_term.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:09:04.922674 gpt-term-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-27 08:08:52.000000 gpt-term-1.0.1/setup.py
```

### Comparing `gpt-term-1.0.0/LICENSE` & `gpt-term-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.0/PKG-INFO` & `gpt-term-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.0.0
+Version: 1.0.1
 Summary: Use ChatGPT in terminal
 Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
 Author: xiaoxx970
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Chat with GPT in Terminal
 
-[![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](./README.md)
-[![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](./README.zh-CN.md)
+[![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.md)
+[![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.zh-CN.md)
 [![Platform badge](https://img.shields.io/badge/Platform-MacOS%7CWindows%7CLinux-green)]()
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
 This project enables chatting with ChatGPT in the terminal.
 
 Markdown content in answers is rendered as beautifully formatted rich text.
 
@@ -256,15 +256,15 @@
 
 Thanks to the following projects for providing strong support for this script:
 
 - [requests](https://github.com/psf/requests): For handling HTTP requests
 - [pyperclip](https://github.com/asweigart/pyperclip): A cross-platform clipboard operation library
 - [rich](https://github.com/willmcgugan/rich): For outputting rich text in the terminal
 - [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit): Command-line input processing library
-- [sseclient-py](https://github.com/btubbs/sseclient-py): For implementing streaming output of answers
+- [sseclient-py](https://github.com/mpetazzoni/sseclient): For implementing streaming output of answers
 - [tiktoken](https://github.com/OpenAI/tiktoken): A library for calculating and processing OpenAI API tokens
 
 ## Contributing
 
 Feel free to dive in! [Open an issue](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/new) or submit PRs.
 
 ### Contributors
```

### Comparing `gpt-term-1.0.0/README.md` & `gpt-term-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## Chat with GPT in Terminal
 
-[![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](./README.md)
-[![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](./README.zh-CN.md)
+[![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.md)
+[![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.zh-CN.md)
 [![Platform badge](https://img.shields.io/badge/Platform-MacOS%7CWindows%7CLinux-green)]()
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
 This project enables chatting with ChatGPT in the terminal.
 
 Markdown content in answers is rendered as beautifully formatted rich text.
 
@@ -242,15 +242,15 @@
 
 Thanks to the following projects for providing strong support for this script:
 
 - [requests](https://github.com/psf/requests): For handling HTTP requests
 - [pyperclip](https://github.com/asweigart/pyperclip): A cross-platform clipboard operation library
 - [rich](https://github.com/willmcgugan/rich): For outputting rich text in the terminal
 - [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit): Command-line input processing library
-- [sseclient-py](https://github.com/btubbs/sseclient-py): For implementing streaming output of answers
+- [sseclient-py](https://github.com/mpetazzoni/sseclient): For implementing streaming output of answers
 - [tiktoken](https://github.com/OpenAI/tiktoken): A library for calculating and processing OpenAI API tokens
 
 ## Contributing
 
 Feel free to dive in! [Open an issue](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/new) or submit PRs.
 
 ### Contributors
```

### Comparing `gpt-term-1.0.0/config.ini` & `gpt-term-1.0.1/gpt_term/config.ini`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.0/gpt_term/main.py` & `gpt-term-1.0.1/gpt_term/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import argparse
 import concurrent.futures
 import json
 import logging
 import os
 import platform
 import re
-import shutil
 import sys
 import threading
 import time
 from configparser import ConfigParser
 from datetime import date, datetime, timedelta
+from importlib.resources import read_text
+from pathlib import Path
 from queue import Queue
 from typing import Dict, List
 
 import pyperclip
 import requests
 import sseclient
 import tiktoken
@@ -32,18 +33,20 @@
 from rich.console import Console, Group
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 from . import __version__
 
-data_dir = os.path.expanduser("~") + "/.gpt-term"
-if not os.path.exists(data_dir):
-    os.makedirs(data_dir)
-    shutil.copy('config.ini', data_dir)
+data_dir = Path.home() / '.gpt-term'
+data_dir.mkdir(parents=True, exist_ok=True)
+config_path = data_dir / 'config.ini'
+if not config_path.exists():
+    with config_path.open('w') as f:
+        f.write(read_text('gpt_term', 'config.ini'))
 
 # 日志记录到 chat.log，注释下面这行可不记录日志
 logging.basicConfig(filename=f'{data_dir}/chat.log', format='%(asctime)s %(name)s: %(levelname)-6s %(message)s',
                     datefmt='[%Y-%m-%d %H:%M:%S]', level=logging.INFO)
 
 log = logging.getLogger("chat")
 
@@ -892,14 +895,15 @@
 
     write_config(config_ini)
     exit(0)
 
 
 def main():
     parser = argparse.ArgumentParser(description='Use ChatGPT in terminal')
+    parser.add_argument('--version', action='version', version=f'%(prog)s v{local_version}')
     parser.add_argument('--load', metavar='FILE', type=str, help='Load chat history from file')
     parser.add_argument('--key', type=str, help='Choose the API key to load')
     parser.add_argument('--model', type=str, help='Choose the AI model to use')
     parser.add_argument('-m', '--multi', action='store_true', help='Enable multi-line mode')
     parser.add_argument('-r', '--raw', action='store_true', help='Enable raw mode')
     # normal function args
 
@@ -928,15 +932,15 @@
     # log level set must be before debug logs, because default log level is INFO, and before new log level being set debug logs will not be written to log file
 
     log.info("GPT-Term start")
 
     log.debug(f"Local version: {str(local_version)}")
     # get local version from pkg resource
 
-    check_remote_update_thread = threading.Thread(target=get_remote_version)
+    check_remote_update_thread = threading.Thread(target=get_remote_version, daemon=True)
     check_remote_update_thread.start()
     log.debug("Remote version get thread started")
     # try to get remote version and check update
 
     # if 'key' arg triggered, load the api key from config.ini with the given key-name;
     # otherwise load the api key with the key-name "OPENAI_API_KEY"
     if args.key:
```

### Comparing `gpt-term-1.0.0/gpt_term.egg-info/PKG-INFO` & `gpt-term-1.0.1/gpt_term.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.0.0
+Version: 1.0.1
 Summary: Use ChatGPT in terminal
 Home-page: https://github.com/xiaoxx970/chatgpt-in-terminal
 Author: xiaoxx970
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Chat with GPT in Terminal
 
-[![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](./README.md)
-[![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](./README.zh-CN.md)
+[![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.md)
+[![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](https://github.com/xiaoxx970/chatgpt-in-terminal/blob/main/README.zh-CN.md)
 [![Platform badge](https://img.shields.io/badge/Platform-MacOS%7CWindows%7CLinux-green)]()
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
 This project enables chatting with ChatGPT in the terminal.
 
 Markdown content in answers is rendered as beautifully formatted rich text.
 
@@ -256,15 +256,15 @@
 
 Thanks to the following projects for providing strong support for this script:
 
 - [requests](https://github.com/psf/requests): For handling HTTP requests
 - [pyperclip](https://github.com/asweigart/pyperclip): A cross-platform clipboard operation library
 - [rich](https://github.com/willmcgugan/rich): For outputting rich text in the terminal
 - [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit): Command-line input processing library
-- [sseclient-py](https://github.com/btubbs/sseclient-py): For implementing streaming output of answers
+- [sseclient-py](https://github.com/mpetazzoni/sseclient): For implementing streaming output of answers
 - [tiktoken](https://github.com/OpenAI/tiktoken): A library for calculating and processing OpenAI API tokens
 
 ## Contributing
 
 Feel free to dive in! [Open an issue](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/new) or submit PRs.
 
 ### Contributors
```

### Comparing `gpt-term-1.0.0/setup.py` & `gpt-term-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     py_modules=["chat"],
     install_requires=install_requires,
     entry_points={
         "console_scripts": [
             "gpt-term=gpt_term.main:main"
         ]
     },
-    data_files=[('', ['config.ini'])],
+    include_package_data=True,
     python_requires=">=3.7",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ]
 )
```


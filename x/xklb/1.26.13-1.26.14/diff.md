# Comparing `tmp/xklb-1.26.13.tar.gz` & `tmp/xklb-1.26.14.tar.gz`

## Comparing `xklb-1.26.13.tar` & `xklb-1.26.14.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.13/.gitattributes
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 xklb-1.26.13/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.13/Windows.md
--rw-r--r--   0        0        0   418454 2020-02-02 00:00:00.000000 xklb-1.26.13/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.13/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.13/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.13/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.13/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 xklb-1.26.13/.github/workflows/push.yaml
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 xklb-1.26.13/sql/restore_listen_count.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/__init__.py
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/av.py
--rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/books.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/consts.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/db.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/dl_config.py
--rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/dl_extract.py
--rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/fs_extract.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/gui.py
--rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/hn_extract.py
--rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/lb.py
--rw-r--r--   0        0        0    35445 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/play_actions.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/playback.py
--rw-r--r--   0        0        0    26596 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/player.py
--rw-r--r--   0        0        0    14621 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/praw_extract.py
--rw-r--r--   0        0        0    16072 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/stats.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/subtitle.py
--rw-r--r--   0        0        0    12107 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/tube_backend.py
--rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/tube_extract.py
--rw-r--r--   0        0        0    28045 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/utils.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/christen.py
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/reddit_self.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.13/xklb/scripts/mining/words.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.13/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.13/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.13/LICENSE
--rw-r--r--   0        0        0    40448 2020-02-02 00:00:00.000000 xklb-1.26.13/README.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 xklb-1.26.13/pyproject.toml
--rw-r--r--   0        0        0    43985 2020-02-02 00:00:00.000000 xklb-1.26.13/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.14/.gitattributes
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 xklb-1.26.14/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.14/Windows.md
+-rw-r--r--   0        0        0   415271 2020-02-02 00:00:00.000000 xklb-1.26.14/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.14/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.14/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.14/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.14/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 xklb-1.26.14/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 xklb-1.26.14/sql/restore_listen_count.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/__init__.py
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/av.py
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/books.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/consts.py
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/db.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/dl_config.py
+-rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/gui.py
+-rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/lb.py
+-rw-r--r--   0        0        0    35700 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/play_actions.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/playback.py
+-rw-r--r--   0        0        0    26435 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/player.py
+-rw-r--r--   0        0        0    14621 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16072 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/stats.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/subtitle.py
+-rw-r--r--   0        0        0    12107 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28045 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/utils.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/nfb_ca.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/reddit_self.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/words.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.14/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.14/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.14/LICENSE
+-rw-r--r--   0        0        0    40448 2020-02-02 00:00:00.000000 xklb-1.26.14/README.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 xklb-1.26.14/pyproject.toml
+-rw-r--r--   0        0        0    43985 2020-02-02 00:00:00.000000 xklb-1.26.14/PKG-INFO
```

### Comparing `xklb-1.26.13/TODO` & `xklb-1.26.14/TODO`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/Windows.md` & `xklb-1.26.14/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/pdm.lock` & `xklb-1.26.14/pdm.lock`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 [[package]]
 name = "docx2txt"
 version = "0.8"
 summary = "A pure python-based utility to extract text and images from docx files."
 
 [[package]]
 name = "dogpile-cache"
-version = "1.1.8"
+version = "1.2.0"
 requires_python = ">=3.6"
 summary = "A caching front-end based on the Dogpile lock."
 dependencies = [
     "decorator>=4.0.0",
     "stevedore>=3.0.0",
 ]
 
@@ -596,15 +596,15 @@
 name = "pillow"
 version = "9.5.0"
 requires_python = ">=3.7"
 summary = "Python Imaging Library (Fork)"
 
 [[package]]
 name = "platformdirs"
-version = "3.2.0"
+version = "3.4.0"
 requires_python = ">=3.7"
 summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 requires_python = ">=3.6"
@@ -1040,16 +1040,16 @@
 name = "websockets"
 version = "11.0.2"
 requires_python = ">=3.7"
 summary = "An implementation of the WebSocket Protocol (RFC 6455 & 7692)"
 
 [[package]]
 name = "werkzeug"
-version = "2.2.3"
-requires_python = ">=3.7"
+version = "2.3.1"
+requires_python = ">=3.8"
 summary = "The comprehensive WSGI web application library."
 dependencies = [
     "MarkupSafe>=2.1.1",
 ]
 
 [[package]]
 name = "wheel"
@@ -1067,15 +1067,15 @@
 name = "xlsxwriter"
 version = "3.1.0"
 requires_python = ">=3.6"
 summary = "A Python module for creating Excel XLSX files."
 
 [[package]]
 name = "yarl"
-version = "1.9.1"
+version = "1.9.2"
 requires_python = ">=3.7"
 summary = "Yet another URL library"
 dependencies = [
     "idna>=2.0",
     "multidict>=4.0",
 ]
 
@@ -1091,15 +1091,15 @@
     "mutagen",
     "pycryptodomex",
     "websockets",
 ]
 
 [[package]]
 name = "zeroconf"
-version = "0.58.0"
+version = "0.58.2"
 requires_python = ">=3.7,<4.0"
 summary = "A pure python implementation of multicast DNS service discovery"
 dependencies = [
     "async-timeout>=3.0.0; python_version < \"3.11\"",
     "ifaddr>=0.1.7",
 ]
 
@@ -1633,17 +1633,17 @@
 "decorator 5.1.1" = [
     {url = "https://files.pythonhosted.org/packages/66/0c/8d907af351aa16b42caae42f9d6aa37b900c67308052d10fdce809f8d952/decorator-5.1.1.tar.gz", hash = "sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330"},
     {url = "https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl", hash = "sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186"},
 ]
 "docx2txt 0.8" = [
     {url = "https://files.pythonhosted.org/packages/7d/7d/60ee3f2b16d9bfdfa72e8599470a2c1a5b759cb113c6fe1006be28359327/docx2txt-0.8.tar.gz", hash = "sha256:2c06d98d7cfe2d3947e5760a57d924e3ff07745b379c8737723922e7009236e5"},
 ]
-"dogpile-cache 1.1.8" = [
-    {url = "https://files.pythonhosted.org/packages/66/62/c07222121b9032a1bc19865bee77cb8e4a9c36db75ec11a3fee780681c4c/dogpile.cache-1.1.8-py3-none-any.whl", hash = "sha256:3f0ca10b46b165e0b0e65e0e74b1a4b36187787b69db7c0f7073077adff2f05d"},
-    {url = "https://files.pythonhosted.org/packages/e4/11/c5c200e774fb6cca03288c25cdb600fb8c41f2ace38a7ebfedfd3de3c3e1/dogpile.cache-1.1.8.tar.gz", hash = "sha256:d844e8bb638cc4f544a4c89a834dfd36fe935400b71a16cbd744ebdfb720fd4e"},
+"dogpile-cache 1.2.0" = [
+    {url = "https://files.pythonhosted.org/packages/01/bc/c6ff56c73fb4d9859a0f3080ed5d454646d6849e8a9aede1f95cb2771de4/dogpile.cache-1.2.0.tar.gz", hash = "sha256:47554c860ceb484dd5aef9ff1f88fecb3d4aef6bb92119450f5bcbaa026bbfb1"},
+    {url = "https://files.pythonhosted.org/packages/08/4f/11c49c820186a436471d5c15075456621a0bcd710dac7bac5e7b62e3bbcb/dogpile.cache-1.2.0-py3-none-any.whl", hash = "sha256:d371f310bcdbe5d9c8e7e473348b75c5c97517ac8be16759b24dbaadef1c70a6"},
 ]
 "ebcdic 1.1.1" = [
     {url = "https://files.pythonhosted.org/packages/0d/2f/633031205333bee5f9f93761af8268746aa75f38754823aabb8570eb245b/ebcdic-1.1.1-py2.py3-none-any.whl", hash = "sha256:33b4cb729bc2d0bf46cc1847b0e5946897cb8d3f53520c5b9aa5fa98d7e735f1"},
 ]
 "enzyme 0.4.1" = [
     {url = "https://files.pythonhosted.org/packages/dd/99/e4eee822d9390ebf1f63a7a67e8351c09fb7cd75262e5bb1a5256898def9/enzyme-0.4.1.tar.gz", hash = "sha256:f2167fa97c24d1103a94d4bf4eb20f00ca76c38a37499821049253b2059c62bb"},
 ]
@@ -2259,17 +2259,17 @@
     {url = "https://files.pythonhosted.org/packages/d9/0e/7c6f054022235830dc2c37ec83e947d9ca09b0b0361e1e5e29983da92294/Pillow-9.5.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cb841572862f629b99725ebaec3287fc6d275be9b14443ea746c1dd325053cbd"},
     {url = "https://files.pythonhosted.org/packages/db/5c/ba9e291850f594f89436cdca93d36c6f8610d4fb7833a6c257f4481d4174/Pillow-9.5.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:662da1f3f89a302cc22faa9f14a262c2e3951f9dbc9617609a47521c69dd9f8f"},
     {url = "https://files.pythonhosted.org/packages/e7/2a/f3ed578595f8486ee2cc07434460097d89aedd406a3db849b890ca8ec416/Pillow-9.5.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:a127ae76092974abfbfa38ca2d12cbeddcdeac0fb71f9627cc1135bedaf9d51a"},
     {url = "https://files.pythonhosted.org/packages/ec/7d/01404982db598f271ac7c0d0207860f60ab9288cfacce9872eb567cfbfe3/Pillow-9.5.0-cp37-cp37m-macosx_10_10_x86_64.whl", hash = "sha256:5d4ebf8e1db4441a55c509c4baa7a0587a0210f7cd25fcfe74dbbce7a4bd1906"},
     {url = "https://files.pythonhosted.org/packages/f2/43/0892913d499c8df2c88dee69d59e77de19e0c51754a9be82023880641c09/Pillow-9.5.0-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:8aca1152d93dcc27dc55395604dcfc55bed5f25ef4c98716a928bacba90d33a3"},
     {url = "https://files.pythonhosted.org/packages/ff/fc/48a51c0fe2a00d5def57b9981a1e0f8339b516351da7a51500383d833bc8/Pillow-9.5.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:608488bdcbdb4ba7837461442b90ea6f3079397ddc968c31265c1e056964f1ef"},
 ]
-"platformdirs 3.2.0" = [
-    {url = "https://files.pythonhosted.org/packages/15/04/3f882b46b454ab374ea75425c6f931e499150ec1385a73e55b3f45af615a/platformdirs-3.2.0.tar.gz", hash = "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08"},
-    {url = "https://files.pythonhosted.org/packages/b2/f3/4fb5fae710fc9f22a42cd90dc0547da18ec83e2e139294ab94f04c449cf5/platformdirs-3.2.0-py3-none-any.whl", hash = "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"},
+"platformdirs 3.4.0" = [
+    {url = "https://files.pythonhosted.org/packages/5e/ac/26d3d2a99b5fc84852229fc8470ae612595900f7f52c78468fd3f3a15a27/platformdirs-3.4.0.tar.gz", hash = "sha256:a5e1536e5ea4b1c238a1364da17ff2993d5bd28e15600c2c8224008aff6bbcad"},
+    {url = "https://files.pythonhosted.org/packages/6c/fe/f6001fac1337528c14b353298d38748ee2387db0c262587ff4e7c68b5769/platformdirs-3.4.0-py3-none-any.whl", hash = "sha256:01437886022decaf285d8972f9526397bfae2ac55480ed372ed6d9eca048870a"},
 ]
 "pluggy 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/9e/01/f38e2ff29715251cf25532b9082a1589ab7e4f571ced434f98d0139336dc/pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
     {url = "https://files.pythonhosted.org/packages/a1/16/db2d7de3474b6e37cbb9c008965ee63835bba517e22cdb8c35b5116b5ce1/pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
 ]
 "praw 7.7.0" = [
     {url = "https://files.pythonhosted.org/packages/b3/93/55ae62910b94b46ecdd0ee8765289304f8df8deeaa1df7a96b0831c637ff/praw-7.7.0-py3-none-any.whl", hash = "sha256:22155c4b3006733a5ab0754136cf2226917747b61ec037ee335246fe0db5420e"},
@@ -2755,158 +2755,145 @@
     {url = "https://files.pythonhosted.org/packages/df/8f/064d879849112d09df9fd2a797668c011fbd33420d15e469435da903dc22/websockets-11.0.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e0eeeea3b01c97fd3b5049a46c908823f68b59bf0e18d79b231d8d6764bc81ee"},
     {url = "https://files.pythonhosted.org/packages/e7/55/883b3d2fb2435d4d80cbe39237d0a1ad7f6014f05de21926e3b410a1eae6/websockets-11.0.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:13bd5bebcd16a4b5e403061b8b9dcc5c77e7a71e3c57e072d8dff23e33f70fba"},
     {url = "https://files.pythonhosted.org/packages/ea/8a/32116db59137262378ba72a124e5ee28f78f8a3a621281cfbddb6a634b37/websockets-11.0.2-py3-none-any.whl", hash = "sha256:5004c087d17251938a52cce21b3dbdabeecbbe432ce3f5bbbf15d8692c36eac9"},
     {url = "https://files.pythonhosted.org/packages/f0/61/c1a45650b8526b19f2aeb9f3e03532e493e6470bd99c4f67c66f5e20915b/websockets-11.0.2-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b2a573c8d71b7af937852b61e7ccb37151d719974146b5dc734aad350ef55a02"},
     {url = "https://files.pythonhosted.org/packages/f8/cb/1178fe699508fc820eead75a8f1848dbc95acdd9fb2530b784db1e4a8f58/websockets-11.0.2-pp39-pypy39_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:518ed6782d9916c5721ebd61bb7651d244178b74399028302c8617d0620af291"},
     {url = "https://files.pythonhosted.org/packages/f8/e9/885a685ddf6a4f9033b6254cb742e4f2f47acee10e5d068f0a7ea8592e52/websockets-11.0.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:143782041e95b63083b02107f31cda999f392903ae331de1307441f3a4557d51"},
 ]
-"werkzeug 2.2.3" = [
-    {url = "https://files.pythonhosted.org/packages/02/3c/baaebf3235c87d61d6593467056d5a8fba7c75ac838b8d100a5e64eba7a0/Werkzeug-2.2.3.tar.gz", hash = "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe"},
-    {url = "https://files.pythonhosted.org/packages/f6/f8/9da63c1617ae2a1dec2fbf6412f3a0cfe9d4ce029eccbda6e1e4258ca45f/Werkzeug-2.2.3-py3-none-any.whl", hash = "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"},
+"werkzeug 2.3.1" = [
+    {url = "https://files.pythonhosted.org/packages/9b/5a/6259e936ce9b9043293dd8473943f5e6bba244c2cb6e3e5354406dfb0700/Werkzeug-2.3.1-py3-none-any.whl", hash = "sha256:69a4b8fcbb30a4c3fa81a5cebd961541273e4d222a4c08593b0b18312e14f64a"},
+    {url = "https://files.pythonhosted.org/packages/aa/70/3874542be48f8da37cecf59d931c56543a9b5704da26fad48ddf8bd024ae/Werkzeug-2.3.1.tar.gz", hash = "sha256:2d35a28a75ae03727eae14ea7d13627c0f77aed6b9998441e6dae0b387f697fc"},
 ]
 "wheel 0.40.0" = [
     {url = "https://files.pythonhosted.org/packages/61/86/cc8d1ff2ca31a312a25a708c891cf9facbad4eae493b3872638db6785eb5/wheel-0.40.0-py3-none-any.whl", hash = "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"},
     {url = "https://files.pythonhosted.org/packages/fc/ef/0335f7217dd1e8096a9e8383e1d472aa14717878ffe07c4772e68b6e8735/wheel-0.40.0.tar.gz", hash = "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873"},
 ]
 "xlrd 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/aa/05/ec9d4fcbbb74bbf4da9f622b3b61aec541e4eccf31d3c60c5422ec027ce2/xlrd-1.2.0.tar.gz", hash = "sha256:546eb36cee8db40c3eaa46c351e67ffee6eeb5fa2650b71bc4c758a29a1b29b2"},
     {url = "https://files.pythonhosted.org/packages/b0/16/63576a1a001752e34bf8ea62e367997530dc553b689356b9879339cf45a4/xlrd-1.2.0-py2.py3-none-any.whl", hash = "sha256:e551fb498759fa3a5384a94ccd4c3c02eb7c00ea424426e212ac0c57be9dfbde"},
 ]
 "xlsxwriter 3.1.0" = [
     {url = "https://files.pythonhosted.org/packages/17/00/b99c915fa2118b9a1dd061a5bf82094c843ab481c714c6d826668df834ad/XlsxWriter-3.1.0.tar.gz", hash = "sha256:02913b50b74c00f165933d5da3e3a02cab4204cb4932722a1b342c5c71034122"},
     {url = "https://files.pythonhosted.org/packages/bd/00/28d48d105fa914b460e9721b315af096937e2e82bf540932c68420ccd9e1/XlsxWriter-3.1.0-py3-none-any.whl", hash = "sha256:b70a147d36235d1ee835cfd037396f789db1f76740a0e5c917d54137169341de"},
 ]
-"yarl 1.9.1" = [
-    {url = "https://files.pythonhosted.org/packages/06/49/9c3b389037d1f50a81526ab9301f36d27b2589f39acf14ea40142e2a414f/yarl-1.9.1-cp37-cp37m-musllinux_1_1_ppc64le.whl", hash = "sha256:01cf88cb80411978a14aa49980968c1aeb7c18a90ac978c778250dd234d8e0ba"},
-    {url = "https://files.pythonhosted.org/packages/08/45/1822a28f2acee0eb0854bc31934971acd928ba88600cf826748a9edb3b7e/yarl-1.9.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a8b8d4b478a9862447daef4cafc89d87ea4ed958672f1d11db7732b77ead49cc"},
-    {url = "https://files.pythonhosted.org/packages/09/88/ca3857851d095b327f0d16d76c3063d97605b8657d82c96d4064dd9b586d/yarl-1.9.1-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:395ea180257a3742d09dcc5071739682a95f7874270ebe3982d6696caec75be0"},
-    {url = "https://files.pythonhosted.org/packages/0c/64/837e8fe0284a4330209d6412c4419fa0805eb9a991261feb4d5f5459336e/yarl-1.9.1-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:f206adb89424dca4a4d0b31981869700e44cd62742527e26d6b15a510dd410a2"},
-    {url = "https://files.pythonhosted.org/packages/0f/75/22897c5209185e3cf4f4ec074dbbbca2ee065d26c5b0405dd2300c16c685/yarl-1.9.1-cp37-cp37m-win32.whl", hash = "sha256:ecad20c3ef57c513dce22f58256361d10550a89e8eaa81d5082f36f8af305375"},
-    {url = "https://files.pythonhosted.org/packages/13/a9/704baa587a7334062335ce813a9f23e6cf5c49d540edfaeffeb8a4c0e47f/yarl-1.9.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:098bdc06ffb4db39c73883325b8c738610199f5f12e85339afedf07e912a39af"},
-    {url = "https://files.pythonhosted.org/packages/14/4c/27c98f3e23817bca2b69e60d533c5cf58c67ff53e1afcc11a3e21138747d/yarl-1.9.1-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:e7ddebeabf384099814353a2956ed3ab5dbaa6830cc7005f985fcb03b5338f05"},
-    {url = "https://files.pythonhosted.org/packages/14/7e/fd7c9ad7d309b0865a003082fe19842c96ea26ad9f55a8dcf6a61bacdbe9/yarl-1.9.1-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:8c72a1dc7e2ea882cd3df0417c808ad3b69e559acdc43f3b096d67f2fb801ada"},
-    {url = "https://files.pythonhosted.org/packages/15/6d/96de5c4765a1ee73d236766e1f7bbaabfa3c16c612407d92487f130b0da4/yarl-1.9.1-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:3abe37fd89a93ebe0010417ca671f422fa6fcffec54698f623b09f46b4d4a512"},
-    {url = "https://files.pythonhosted.org/packages/1a/8f/11d9de8535785ac4fb9bdae6d63c9ee03207a6a0f37e7421f0d59ff90b74/yarl-1.9.1-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:f76edb386178a54ea7ceffa798cb830c3c22ab50ea10dfb25dc952b04848295f"},
-    {url = "https://files.pythonhosted.org/packages/1e/2e/fc7b8b8adbd4017f1ef4ac214dcba81b973cf5b53a202ce410fdc3238803/yarl-1.9.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:5faf3ec98747318cb980aaf9addf769da68a66431fc203a373d95d7ee9c1fbb4"},
-    {url = "https://files.pythonhosted.org/packages/23/a0/f27e9d7210f1d5c1999cf5c16a43c0ad71aa50733559cbd172c05fbba9d0/yarl-1.9.1-cp310-cp310-win_amd64.whl", hash = "sha256:b63d41e0eecf3e3070d44f97456cf351fff7cb960e97ecb60a936b877ff0b4f6"},
-    {url = "https://files.pythonhosted.org/packages/26/ab/812fe43bb54f5bb31a201c3c0f099899ccb3ffd592eca64e8e384ffa5396/yarl-1.9.1-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:ac8e593df1fbea820da7676929f821a0c7c2cecb8477d010254ce8ed54328ea8"},
-    {url = "https://files.pythonhosted.org/packages/2a/2a/0db4373be43f5877ad4c9b87e8a0d562b35b7596411e51739151dbc1e010/yarl-1.9.1-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:92e37999e36f9f3ded78e9d839face6baa2abdf9344ea8ed2735f495736159de"},
-    {url = "https://files.pythonhosted.org/packages/2b/2d/ad085bf7f3d8a0bd35f590b47384b171d1abd27f18ed2f0822676fcde3e0/yarl-1.9.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:575975d28795a61e82c85f114c02333ca54cbd325fd4e4b27598c9832aa732e7"},
-    {url = "https://files.pythonhosted.org/packages/38/e4/dc17d4a2a2e4d88f908493ecf68495f6c3fa961f01ed67955dda45abc004/yarl-1.9.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:89099c887338608da935ba8bee027564a94f852ac40e472de15d8309517ad5fe"},
-    {url = "https://files.pythonhosted.org/packages/39/52/5a4d0569c642395c72862011558d3d3d1199af7132eb775ea13708d3340c/yarl-1.9.1-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:4d817593d345fefda2fae877accc8a0d9f47ada57086da6125fa02a62f6d1a94"},
-    {url = "https://files.pythonhosted.org/packages/3f/65/d0f6afbc4c553a798a7cd82131f5e2ed9fc350b18a4834fbc730a428f07f/yarl-1.9.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:56956b13ec275de31fe4fb991510b735c4fb3e1b01600528c952b9ac90464430"},
-    {url = "https://files.pythonhosted.org/packages/43/58/90de1fea8eb85138396ecb99669878e5c048f1c9b55ecbae317128ebcad4/yarl-1.9.1-cp39-cp39-win32.whl", hash = "sha256:518a92a34c741836a315150460b5c1c71ae782d569eabd7acf53372e437709f7"},
-    {url = "https://files.pythonhosted.org/packages/47/e5/c002eb8f463f8a99ec4a8f8aa05c68f75cba5af2c960b963e51484e74021/yarl-1.9.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9bb794882818fae20ff65348985fdf143ea6dfaf6413814db1848120db8be33e"},
-    {url = "https://files.pythonhosted.org/packages/48/94/1045a81f11b35e918b6c1c6b533c181ce0feebf337c58b5c5d6db589416a/yarl-1.9.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:b2b2382d59dec0f1fdca18ea429c4c4cee280d5e0dbc841180abb82e188cf6e9"},
-    {url = "https://files.pythonhosted.org/packages/4b/9c/e1e1b56bfa832e4a68fe22bac586492db228395b90bd68a700ed3801fe0e/yarl-1.9.1-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:90ebaf448b5f048352ec7c76cb8d452df30c27cb6b8627dfaa9cf742a14f141a"},
-    {url = "https://files.pythonhosted.org/packages/4d/b4/a9792d745d2ee769873a60e7011c4c41f5157619c622bac31befb77d37bd/yarl-1.9.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f878a78ed2ccfbd973cab46dd0933ecd704787724db23979e5731674d76eb36f"},
-    {url = "https://files.pythonhosted.org/packages/58/ea/fee20f5a45c05f89da121156e9e39bdcb1f11f06eac44fa2ec37f273c452/yarl-1.9.1-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:d5c407e530cf2979ea383885516ae79cc4f3c3530623acf5e42daf521f5c2564"},
-    {url = "https://files.pythonhosted.org/packages/5e/d6/d00d3717c36a01a37eced52ac76f77566dbbe95069fe024221de946484cf/yarl-1.9.1-cp38-cp38-win_amd64.whl", hash = "sha256:09c56a32c26e24ef98d5757c5064e252836f621f9a8b42737773aa92936b8e08"},
-    {url = "https://files.pythonhosted.org/packages/60/4c/804134e681cf5f0ce26ae76e44114ae69534a9bb0bd778244dd651995ea8/yarl-1.9.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:a21789bdf28549d4eb1de6910cabc762c9f6ae3eef85efc1958197c1c6ef853b"},
-    {url = "https://files.pythonhosted.org/packages/69/52/91919be6ea17ddd9f2432e733da409b13b070ab100f0e31213de76ccfef9/yarl-1.9.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:6cf47fe9df9b1ededc77e492581cdb6890a975ad96b4172e1834f1b8ba0fc3ba"},
-    {url = "https://files.pythonhosted.org/packages/6d/43/f342ae9852c75950db6f525f12d302c3515b429317b1292e5e910d6ff54e/yarl-1.9.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:85aa6fd779e194901386709e0eedd45710b68af2709f82a84839c44314b68c10"},
-    {url = "https://files.pythonhosted.org/packages/6d/b3/45d0f1588fa5928e8599a9af453e1e199a8397e3a5d92185e7d89e116e67/yarl-1.9.1-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:44fa6158e6b4b8ccfa2872c3900a226b29e8ce543ce3e48aadc99816afa8874d"},
-    {url = "https://files.pythonhosted.org/packages/74/04/17327e851489b0ba54137eae8c65fb5515a2f2770b92b8faf92c7b1af507/yarl-1.9.1-cp38-cp38-win32.whl", hash = "sha256:6b09cce412386ea9b4dda965d8e78d04ac5b5792b2fa9cced3258ec69c7d1c16"},
-    {url = "https://files.pythonhosted.org/packages/77/d7/15fa0e672750fab95e2d5ad01b49d6e66a1689d4a0e8bc8d9acd1c368b75/yarl-1.9.1-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:97d76a3128f48fa1c721ef8a50e2c2f549296b2402dc8a8cde12ff60ed922f53"},
-    {url = "https://files.pythonhosted.org/packages/7e/3f/d1538cacfc5a53c7e87e3a2592ca91ad7edd8bf8663b7ba8082fbc2a5365/yarl-1.9.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1baf8cdaaab65d9ccedbf8748d626ad648b74b0a4d033e356a2f3024709fb82f"},
-    {url = "https://files.pythonhosted.org/packages/81/66/0fc19e51ab945cb3e594698d2caa2b15e381df9ceaee76a8485d96ce43ff/yarl-1.9.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:08c8599d6aa8a24425f8635f6c06fa8726afe3be01c8e53e236f519bcfa5db5b"},
-    {url = "https://files.pythonhosted.org/packages/83/67/c0c49ee53f6de67f63a2353a93a0874a53d311eaea82dc227005eb77abcd/yarl-1.9.1-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:c3ca8d71b23bdf164b36d06df2298ec8a5bd3de42b17bf3e0e8e6a7489195f2c"},
-    {url = "https://files.pythonhosted.org/packages/83/8c/acbb9daafaf6c294b0fb2e169be6ff9b1919ab062d8f1822d626db862d9f/yarl-1.9.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:efec77851231410125cb5be04ec96fa4a075ca637f415a1f2d2c900b09032a8a"},
-    {url = "https://files.pythonhosted.org/packages/85/84/001652c238796c232c1e68344b505aed66afd80fbe7c5893b7b1b8b26276/yarl-1.9.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bab67d041c78e305ff3eef5e549304d843bd9b603c8855b68484ee663374ce15"},
-    {url = "https://files.pythonhosted.org/packages/86/49/c39527d02472fe1f596ddadbb15ca577ad54e31691af09ab4ef780a39419/yarl-1.9.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:df747104ef27ab1aa9a1145064fa9ea26ad8cf24bfcbdba7db7abf0f8b3676b9"},
-    {url = "https://files.pythonhosted.org/packages/8a/a1/043a206d0e9973c12cbf350a40329e4b055b16939a07c5f3666e86410579/yarl-1.9.1-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:74390c2318d066962500045aa145f5412169bce842e734b8c3e6e3750ad5b817"},
-    {url = "https://files.pythonhosted.org/packages/8d/0e/509bdca429daf36f29e392fd3f6a1217fee02f188044ef69140b77ca700e/yarl-1.9.1-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:6cdb47cbbacae8e1d7941b0d504d0235d686090eef5212ca2450525905e9cf02"},
-    {url = "https://files.pythonhosted.org/packages/90/18/69be0184dc369049a58d37c0b9be124edf8a934c906779ec464053970485/yarl-1.9.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:65d952e464df950eed32bb5dcbc1b4443c7c2de4d7abd7265b45b1b3b27f5fa2"},
-    {url = "https://files.pythonhosted.org/packages/95/f8/72360ff353741f6723eb6e1e0eb653409ed911ccd72930abb269d1010893/yarl-1.9.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ecaa5755a39f6f26079bf13f336c67af589c222d76b53cd3824d3b684b84d1f1"},
-    {url = "https://files.pythonhosted.org/packages/98/39/0508659c008173b6b42df9b8f4096fc01f30ab04d2c211e543caf8616a5c/yarl-1.9.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:13a1ad1f35839b3bb5226f59816b71e243d95d623f5b392efaf8820ddb2b3cd5"},
-    {url = "https://files.pythonhosted.org/packages/9b/4f/b5f0c6f3485ac0a7a1b98885aa67a411ee90af9b4c1929e5c0ca47033f3a/yarl-1.9.1-cp311-cp311-win_amd64.whl", hash = "sha256:b20a5ddc4e243cbaa54886bfe9af6ffc4ba4ef58f17f1bb691e973eb65bba84d"},
-    {url = "https://files.pythonhosted.org/packages/9d/c9/336c2fb5eb01ff8409f3d1180297493129278936f8cfdf205a1ceedca906/yarl-1.9.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:01a073c9175481dfed6b40704a1b67af5a9435fc4a58a27d35fd6b303469b0c7"},
-    {url = "https://files.pythonhosted.org/packages/a0/30/2ed8154bbaacdfee9cb47e1326f9c172f2fe7de74fedff9a6e90b9d5bbfb/yarl-1.9.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:d966cd59df9a4b218480562e8daab39e87e746b78a96add51a3ab01636fc4291"},
-    {url = "https://files.pythonhosted.org/packages/aa/8f/39e6c99091396816b8b92f6f4702b20dff13bfdaaa14317a24e1f689d46d/yarl-1.9.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1d7a0075a55380b19aa43b9e8056e128b058460d71d75018a4f9d60ace01e78c"},
-    {url = "https://files.pythonhosted.org/packages/ab/69/9e9119ea241fc96c1dddebc9fd2e31ade2e4d69e729f5e936e2e76f67533/yarl-1.9.1-cp310-cp310-win32.whl", hash = "sha256:39a7a9108e9fc633ae381562f8f0355bb4ba00355218b5fb19cf5263fcdbfa68"},
-    {url = "https://files.pythonhosted.org/packages/ab/e6/5495d2cfa603acb024b317fbbeada8e466966aef4b224615b556798102a8/yarl-1.9.1-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:f8e73f526140c1c32f5fca4cd0bc3b511a1abcd948f45b2a38a95e4edb76ca72"},
-    {url = "https://files.pythonhosted.org/packages/ac/44/aa6b863466903f7a4cec450a2a744f4ed1f9a03a2c633e2d649fffc49f4a/yarl-1.9.1-cp37-cp37m-win_amd64.whl", hash = "sha256:f5bcb80006efe9bf9f49ae89711253dd06df8053ff814622112a9219346566a7"},
-    {url = "https://files.pythonhosted.org/packages/b2/a8/bc0a30f46aadd5bc3320636263dfd281cac109f4400c75efe68538345119/yarl-1.9.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b3b5f8da07a21f2e57551f88a6709c2d340866146cf7351e5207623cfe8aad16"},
-    {url = "https://files.pythonhosted.org/packages/b5/cf/97eeb80f65592bfb548849eeb1c412eaff74a741898f764b5c81722d8702/yarl-1.9.1-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:73a4b46689f2d59c8ec6b71c9a0cdced4e7863dd6eb98a8c30ea610e191f9e1c"},
-    {url = "https://files.pythonhosted.org/packages/b9/98/06411f7b9ca9b32446d7fdb017cfbc9813657c63ca5178e4a047b517fecb/yarl-1.9.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:ca14b84091700ae7c1fcd3a6000bd4ec1a3035009b8bcb94f246741ca840bb22"},
-    {url = "https://files.pythonhosted.org/packages/bc/5c/8c487b8d28769859991c93ee3ab6c450153493025cfb0a5f539ccf6fec3b/yarl-1.9.1-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:46c4010de941e2e1365c07fb4418ddca10fcff56305a6067f5ae857f8c98f3a7"},
-    {url = "https://files.pythonhosted.org/packages/bc/ec/ed4b41242cfa6095be27e34d3f89ce7902e2b59fe69c20350a7ddcb9d2cd/yarl-1.9.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:92a101f6d5a9464e86092adc36cd40ef23d18a25bfb1eb32eaeb62edc22776bb"},
-    {url = "https://files.pythonhosted.org/packages/c3/1b/908ba0c887128013eca1135e143b346864c8c4fd41f9fdc9fd3926aa0943/yarl-1.9.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:75676110bce59944dd48fd18d0449bd37eaeb311b38a0c768f7670864b5f8b68"},
-    {url = "https://files.pythonhosted.org/packages/c7/b6/6173516ddfd71e5b681f05788c045167d58d4bcbb04b449dc649b1ad0fd7/yarl-1.9.1-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:307a782736ebf994e7600dcaeea3b3113083584da567272f2075f1540919d6b3"},
-    {url = "https://files.pythonhosted.org/packages/c9/68/f7ba1afe333c722a5d73d4d361c077adb3bdeadde8529b639e2db13f86e0/yarl-1.9.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:b5d5fb6c94b620a7066a3adb7c246c87970f453813979818e4707ac32ce4d7bd"},
-    {url = "https://files.pythonhosted.org/packages/c9/b9/9008308c81fff1345b68319e21bd6fd66cdbe5bbbc3884aae5a04c5215b8/yarl-1.9.1-cp39-cp39-win_amd64.whl", hash = "sha256:78755ce43b6e827e65ec0c68be832f86d059fcf05d4b33562745ebcfa91b26b1"},
-    {url = "https://files.pythonhosted.org/packages/c9/d5/a5ff51828497e9639cd910c8810f32ecad2c42d017eb627ef7eb1568be89/yarl-1.9.1-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:89da1fd6068553e3a333011cc17ad91c414b2100c32579ddb51517edc768b49c"},
-    {url = "https://files.pythonhosted.org/packages/ca/81/b8330100925ca799b0b5142f7bfb7ad845d6c9ebfc05745280fcd37d8f80/yarl-1.9.1-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:e124b283a04cc06d22443cae536f93d86cd55108fa369f22b8fe1f2288b2fe1c"},
-    {url = "https://files.pythonhosted.org/packages/cf/9b/3b9f29e3edc2ea2fb3494031fdc04f90768f975f582f8dfc3797e83041aa/yarl-1.9.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:27efc2e324f72df02818cd72d7674b1f28b80ab49f33a94f37c6473c8166ce49"},
-    {url = "https://files.pythonhosted.org/packages/d1/3b/14c196fa97a29523ade83e8a11eaed48f3e86d722a72203a0359e753a25c/yarl-1.9.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e2f01351b7809182822b21061d2a4728b7b9e08f4585ba90ee4c5c4d3faa0812"},
-    {url = "https://files.pythonhosted.org/packages/d2/b7/a65745167ecd74f41ffb3195b67ff1f6871f1716d913a7369fe59d8c8107/yarl-1.9.1-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:ef7e2f6c47c41e234600a02e1356b799761485834fe35d4706b0094cb3a587ee"},
-    {url = "https://files.pythonhosted.org/packages/d4/09/a9d45321fd2c63bfc8d9036f1cb3cb471c77fe61bb8566c838d263b24a28/yarl-1.9.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d21887cbcf6a3cc5951662d8222bc9c04e1b1d98eebe3bb659c3a04ed49b0eec"},
-    {url = "https://files.pythonhosted.org/packages/d4/23/0822c2042bf6523a697750e9703739e7c337fe8aa6ec12dc0f7953f734ff/yarl-1.9.1-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:4764114e261fe49d5df9b316b3221493d177247825c735b2aae77bc2e340d800"},
-    {url = "https://files.pythonhosted.org/packages/d5/ec/b79d97ac390e5f658839cfea6a7a55202c10fc0f7c4d570f5c150602bdb0/yarl-1.9.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e9fe3a1c073ab80a28a06f41d2b623723046709ed29faf2c56bea41848597d86"},
-    {url = "https://files.pythonhosted.org/packages/d6/85/4b742350008f5f90aef33545d759716909941fdd0685945c539cd6693901/yarl-1.9.1-cp311-cp311-win32.whl", hash = "sha256:9ba5a18c4fbd408fe49dc5da85478a76bc75c1ce912d7fd7b43ed5297c4403e1"},
-    {url = "https://files.pythonhosted.org/packages/dc/7c/8f94ffcec6cfa7ff4528aaf7e3a2e16dd289d1f4338136ab2829b0a1b2de/yarl-1.9.1-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:4295790981630c4dab9d6de7b0f555a4c8defe3ed7704a8e9e595a321e59a0f5"},
-    {url = "https://files.pythonhosted.org/packages/dd/1d/9a51fc00fa9fab28d9c9b61931ae64b1480f32e8a40985764e8573d32918/yarl-1.9.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f0cd87949d619157a0482c6c14e5011f8bf2bc0b91cb5087414d9331f4ef02dd"},
-    {url = "https://files.pythonhosted.org/packages/e9/e7/a0e5a64acd644d49268062d2c949828ab84bcd25dcbb1e554dc6535c4b53/yarl-1.9.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:eed9827033b7f67ad12cb70bd0cb59d36029144a7906694317c2dbf5c9eb5ddd"},
-    {url = "https://files.pythonhosted.org/packages/ed/02/695dd9ec40214fbad98ffc82e97bbe15d99cb798b837c5af38b5649a20cd/yarl-1.9.1.tar.gz", hash = "sha256:5ce0bcab7ec759062c818d73837644cde567ab8aa1e0d6c45db38dfb7c284441"},
-    {url = "https://files.pythonhosted.org/packages/ed/f2/c5fc02f07382bfef5ce1c0a24cf6c34cc5d0cf436532ac7a6b2c62083f41/yarl-1.9.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:88f6413ff5edfb9609e2769e32ce87a62353e66e75d264bf0eaad26fb9daa8f2"},
-    {url = "https://files.pythonhosted.org/packages/f2/c7/f948cce68feefe54b07a31e42f3fa832b59c758851f05cbc5028a28d6b32/yarl-1.9.1-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:b86e98c3021b7e2740d8719bf074301361bf2f51221ca2765b7a58afbfbd9042"},
-    {url = "https://files.pythonhosted.org/packages/f4/12/d5d7139fa844b66f2874a2b91b5152c2aee08d1b610ea0c13b9238518e98/yarl-1.9.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:791357d537a09a194f92b834f28c98d074e7297bac0a8f1d5b458a906cafa17c"},
+"yarl 1.9.2" = [
+    {url = "https://files.pythonhosted.org/packages/0e/b1/a65fcf0363ae8c08c0e586772a34cc15b4200bae163eed24258cc95cda90/yarl-1.9.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:566185e8ebc0898b11f8026447eacd02e46226716229cea8db37496c8cdd26e0"},
+    {url = "https://files.pythonhosted.org/packages/10/b1/13887c4fbf885d64f4b8c1bac403338f7c1c07a34e63d767af8d0972c28d/yarl-1.9.2-cp37-cp37m-win32.whl", hash = "sha256:f364d3480bffd3aa566e886587eaca7c8c04d74f6e8933f3f2c996b7f09bee1b"},
+    {url = "https://files.pythonhosted.org/packages/11/3d/785761e64dc90fda6feb9bd0459dc55ebe282a7d4564642a4a8ee277e0c0/yarl-1.9.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a74dcbfe780e62f4b5a062714576f16c2f3493a0394e555ab141bf0d746bb955"},
+    {url = "https://files.pythonhosted.org/packages/12/27/efe7476bdadb2564d7775e0895df56f3e3adf39495094750fb319599180e/yarl-1.9.2-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:13414591ff516e04fcdee8dc051c13fd3db13b673c7a4cb1350e6b2ad9639ad3"},
+    {url = "https://files.pythonhosted.org/packages/12/c0/18265b85980450b75641a32dd12635485241e295310c1b04e04ac0cc634e/yarl-1.9.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:38a3928ae37558bc1b559f67410df446d1fbfa87318b124bf5032c31e3447b74"},
+    {url = "https://files.pythonhosted.org/packages/14/5b/a0bf4a601ddf4073ae0dcd66a90708aaa944a4ad0addf777d9f1fcd6f4f0/yarl-1.9.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:f3b078dbe227f79be488ffcfc7a9edb3409d018e0952cf13f15fd6512847f3f7"},
+    {url = "https://files.pythonhosted.org/packages/15/5a/5435fe438874f03aa9f559c5173418fbac680b095ac394e88b0825d12ebd/yarl-1.9.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:56ff08ab5df8429901ebdc5d15941b59f6253393cb5da07b4170beefcf1b2528"},
+    {url = "https://files.pythonhosted.org/packages/16/dd/3ef5a4c74f9516f2193b0782046802d73c5475ef49678473a608194f3bf1/yarl-1.9.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:2c315df3293cd521033533d242d15eab26583360b58f7ee5d9565f15fee1bef4"},
+    {url = "https://files.pythonhosted.org/packages/19/41/97678e848ce963cd3e89c4dcc13900c9afedd42e5c7d9cfb019716f8bb2a/yarl-1.9.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:2b0738fb871812722a0ac2154be1f049c6223b9f6f22eec352996b69775b36d4"},
+    {url = "https://files.pythonhosted.org/packages/19/ed/deeec0a15bf1d9a3d2d2102ebb9dbd84dc312a00fbf88564b56b05f266a1/yarl-1.9.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:82aa6264b36c50acfb2424ad5ca537a2060ab6de158a5bd2a72a032cc75b9eb8"},
+    {url = "https://files.pythonhosted.org/packages/1d/78/a273c991086df02837676dc68ccf50d56b2fe624d75258d521c651a65d82/yarl-1.9.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:d4e2c6d555e77b37288eaf45b8f60f0737c9efa3452c6c44626a5455aeb250b9"},
+    {url = "https://files.pythonhosted.org/packages/25/68/b67d964bc7768f6462b51c05dd879b6c6f6e55168086b948e6e3e6f6928e/yarl-1.9.2-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:9b3152f2f5677b997ae6c804b73da05a39daa6a9e85a512e0e6823d81cdad7cc"},
+    {url = "https://files.pythonhosted.org/packages/2d/76/d9178fe8fe5823370b26bbd1bbb159c2cc3f7449cade1a50818bcfc98cae/yarl-1.9.2-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2a96c19c52ff442a808c105901d0bdfd2e28575b3d5f82e2f5fd67e20dc5f4ea"},
+    {url = "https://files.pythonhosted.org/packages/30/55/eda822473c6206470a89ca3550efa23202310a2e56317e55afb709008fd5/yarl-1.9.2-cp310-cp310-win32.whl", hash = "sha256:8ea48e0a2f931064469bdabca50c2f578b565fc446f302a79ba6cc0ee7f384d3"},
+    {url = "https://files.pythonhosted.org/packages/31/2c/e6af0f7710412e4ed49c1641f04ed1af334d448d51c55150235e3381f0a7/yarl-1.9.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:75df5ef94c3fdc393c6b19d80e6ef1ecc9ae2f4263c09cacb178d871c02a5ba9"},
+    {url = "https://files.pythonhosted.org/packages/34/1f/9a915044ec1e13f046e6d023e4dd1ea43316add36e199d46237d7d97cc88/yarl-1.9.2-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b03917871bf859a81ccb180c9a2e6c1e04d2f6a51d953e6a5cdd70c93d4e5a2a"},
+    {url = "https://files.pythonhosted.org/packages/35/0f/a68344daf90536755f4a890dbbab65dc6ca58c4a0268cf79bd7c5ddc1468/yarl-1.9.2-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8ec53a0ea2a80c5cd1ab397925f94bff59222aa3cf9c6da938ce05c9ec20428d"},
+    {url = "https://files.pythonhosted.org/packages/3b/b2/34e45989fa5fcf406dd471c517697a5bf483fb1bcaebcf2bedd2b86e0cbb/yarl-1.9.2-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:b8cc1863402472f16c600e3e93d542b7e7542a540f95c30afd472e8e549fc3f7"},
+    {url = "https://files.pythonhosted.org/packages/3b/b4/d20b0444fa0f0e7efdb328d16efd44d03a02427e090d02f936b990c9e9bc/yarl-1.9.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:59723a029760079b7d991a401386390c4be5bfec1e7dd83e25a6a0881859e716"},
+    {url = "https://files.pythonhosted.org/packages/3d/ea/041c270d8853572eec3e6ad26fe7a53eb85d68c052bfbc79b42ae5e63f8a/yarl-1.9.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:149ddea5abf329752ea5051b61bd6c1d979e13fbf122d3a1f9f0c8be6cb6f63c"},
+    {url = "https://files.pythonhosted.org/packages/40/2c/aa941cb37ed206f9f46158dcb6398f17a5bcb95124970fd43d017650b9b2/yarl-1.9.2-cp39-cp39-win32.whl", hash = "sha256:b124e2a6d223b65ba8768d5706d103280914d61f5cae3afbc50fc3dfcc016623"},
+    {url = "https://files.pythonhosted.org/packages/45/c6/c58e25159d2186247272595ffff1aaba319d10aab20b40429a6e80418328/yarl-1.9.2-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:53338749febd28935d55b41bf0bcc79d634881195a39f6b2f767870b72514caf"},
+    {url = "https://files.pythonhosted.org/packages/49/d7/3b21ce9742ded3e942bcf48b01ebe29fdcd8eb9dc3296ebfbb77660ee8bb/yarl-1.9.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bf74d08542c3a9ea97bb8f343d4fcbd4d8f91bba5ec9d5d7f792dbe727f88938"},
+    {url = "https://files.pythonhosted.org/packages/50/af/93f1b6d02e936d49e664a8eb4374877e5bacfef115c956939729ac9e2ca8/yarl-1.9.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:832b7e711027c114d79dffb92576acd1bd2decc467dec60e1cac96912602d0e6"},
+    {url = "https://files.pythonhosted.org/packages/53/87/f5588bdc6eba3ca4521bd37094563e8442ba2cff3d6b7e5a2cab48fdc96d/yarl-1.9.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b25322201585c69abc7b0e89e72790469f7dad90d26754717f3310bfe30331c2"},
+    {url = "https://files.pythonhosted.org/packages/54/90/8e7f57b0c83805652bd1c26663f9979d12fed8d22516c14c7f3021f97a19/yarl-1.9.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:b9a4e67ad7b646cd6f0938c7ebfd60e481b7410f574c560e455e938d2da8e0f4"},
+    {url = "https://files.pythonhosted.org/packages/58/c7/bad405a8b0b2366c3c21d650831d58fadca95af583c6dc1d2349512741cf/yarl-1.9.2-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:066c163aec9d3d073dc9ffe5dd3ad05069bcb03fcaab8d221290ba99f9f69ee3"},
+    {url = "https://files.pythonhosted.org/packages/5a/3e/53e50f6b492d73dab887428acff54d4ea1be7575bee2d846b932dff459d9/yarl-1.9.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5fcd436ea16fee7d4207c045b1e340020e58a2597301cfbcfdbe5abd2356c2fb"},
+    {url = "https://files.pythonhosted.org/packages/5d/6f/06e3e0b1935e8d65e7c52238b5e82b2afb3e067ff69b07a66b909f3b2432/yarl-1.9.2-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:674ca19cbee4a82c9f54e0d1eee28116e63bc6fd1e96c43031d11cbab8b2afd5"},
+    {url = "https://files.pythonhosted.org/packages/5f/3f/04b3c5e57844fb9c034b09c5cb6d2b43de5d64a093c30529fd233e16cf09/yarl-1.9.2.tar.gz", hash = "sha256:04ab9d4b9f587c06d801c2abfe9317b77cdf996c65a90d5e84ecc45010823571"},
+    {url = "https://files.pythonhosted.org/packages/62/c8/b8e048ba98a0f41d46a22060a57f913b4f9ed9c4f6862de36b8137bb67e2/yarl-1.9.2-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:783185c75c12a017cc345015ea359cc801c3b29a2966c2655cd12b233bf5a2be"},
+    {url = "https://files.pythonhosted.org/packages/63/80/95ae601d7b7f5f6b53174d91d94df865db9166895934d5065e924634dc76/yarl-1.9.2-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:9bf345c3a4f5ba7f766430f97f9cc1320786f19584acc7086491f45524a551ac"},
+    {url = "https://files.pythonhosted.org/packages/6a/67/1ea83dd287358d47adc49f2aeb9e4e8ae72bec8ae2604c3bcae1e7fd73de/yarl-1.9.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c0c77533b5ed4bcc38e943178ccae29b9bcf48ffd1063f5821192f23a1bd27b9"},
+    {url = "https://files.pythonhosted.org/packages/6b/83/e0cb0cbb37098475fca29b8c5000fed417b67fc2c6dc8d0fa7e32c000c80/yarl-1.9.2-cp311-cp311-win_amd64.whl", hash = "sha256:be6b3fdec5c62f2a67cb3f8c6dbf56bbf3f61c0f046f84645cd1ca73532ea051"},
+    {url = "https://files.pythonhosted.org/packages/75/4d/b86c4fd2c689eaeb078de274f6822b02872a5e19557af16257be3eda20ee/yarl-1.9.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:b7232f8dfbd225d57340e441d8caf8652a6acd06b389ea2d3222b8bc89cbfca6"},
+    {url = "https://files.pythonhosted.org/packages/78/1d/0554e6d4c8669ca707e93f188111e29cf8a3c97cf2e8e8448ad3b284ae84/yarl-1.9.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c3a53ba34a636a256d767c086ceb111358876e1fb6b50dfc4d3f4951d40133d5"},
+    {url = "https://files.pythonhosted.org/packages/7a/ff/b490d9995b23e8e6d773679b8f3c8347defe39570f63f3eb391ad208d853/yarl-1.9.2-cp37-cp37m-win_amd64.whl", hash = "sha256:6a5883464143ab3ae9ba68daae8e7c5c95b969462bbe42e2464d60e7e2698368"},
+    {url = "https://files.pythonhosted.org/packages/7e/8a/62334982016006a6820f2117990e1161d15fb05fb2d924b99d303ab2c8ab/yarl-1.9.2-cp37-cp37m-musllinux_1_1_ppc64le.whl", hash = "sha256:e65610c5792870d45d7b68c677681376fcf9cc1c289f23e8e8b39c1485384185"},
+    {url = "https://files.pythonhosted.org/packages/80/53/e0fcf51992fcce66863db5e3fef698a5235257c565a81a46fe3648abae39/yarl-1.9.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ac9bb4c5ce3975aeac288cfcb5061ce60e0d14d92209e780c93954076c7c4367"},
+    {url = "https://files.pythonhosted.org/packages/80/57/1dd9bc12ebaae2d08862c23a80662ecd9d63a61777f10e56f78ddb6ad48a/yarl-1.9.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:de119f56f3c5f0e2fb4dee508531a32b069a5f2c6e827b272d1e0ff5ac040333"},
+    {url = "https://files.pythonhosted.org/packages/84/c1/eaebee42cbcace2d5b5eb103cae668dec1c239f5c82b90da4b3b20f39419/yarl-1.9.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:646d663eb2232d7909e6601f1a9107e66f9791f290a1b3dc7057818fe44fc2b6"},
+    {url = "https://files.pythonhosted.org/packages/88/87/081c39d7b136820ca0a6d9c2bd160e91de01b1b4af2de2069bb51b52538c/yarl-1.9.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f4e2d08f07a3d7d3e12549052eb5ad3eab1c349c53ac51c209a0e5991bbada78"},
+    {url = "https://files.pythonhosted.org/packages/92/30/aceb4a4cacb850d2cd1841ec1746f42868886ae0523d0b1f3a7cfa31ef57/yarl-1.9.2-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3da8a678ca8b96c8606bbb8bfacd99a12ad5dd288bc6f7979baddd62f71c63ef"},
+    {url = "https://files.pythonhosted.org/packages/92/e4/4f8d1cada85dbf1aab7123125b0d2f997cd30457f3540c72c311ded740e6/yarl-1.9.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:494053246b119b041960ddcd20fd76224149cfea8ed8777b687358727911dd33"},
+    {url = "https://files.pythonhosted.org/packages/97/ae/7fba1ec8384192095731460dd2dd20ecdc19cbeade8996ef997bd989d5a2/yarl-1.9.2-cp38-cp38-win_amd64.whl", hash = "sha256:63c48f6cef34e6319a74c727376e95626f84ea091f92c0250a98e53e62c77c72"},
+    {url = "https://files.pythonhosted.org/packages/98/21/9ef4adf36cfac771518c3bf687bc9b92451bdaf01ec770879f19e7e5b3c7/yarl-1.9.2-cp310-cp310-win_amd64.whl", hash = "sha256:50f33040f3836e912ed16d212f6cc1efb3231a8a60526a407aeb66c1c1956dde"},
+    {url = "https://files.pythonhosted.org/packages/a6/a4/451ac414ebe15fd6b49a457c7e01f0a06f9b512c36e4388a9cfb26568fea/yarl-1.9.2-cp39-cp39-win_amd64.whl", hash = "sha256:61016e7d582bc46a5378ffdd02cd0314fb8ba52f40f9cf4d9a5e7dbef88dee18"},
+    {url = "https://files.pythonhosted.org/packages/a8/ce/95614d05af568504884e866d772c9f03235711f5a4d7fccfae54ce82d39d/yarl-1.9.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ee4afac41415d52d53a9833ebae7e32b344be72835bbb589018c9e938045a560"},
+    {url = "https://files.pythonhosted.org/packages/b3/81/fb394392ec748d8fce66212b29dc2fd9b2fd8e30d56d818a6a866708e534/yarl-1.9.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:a83503934c6273806aed765035716216cc9ab4e0364f7f066227e1aaea90b8d0"},
+    {url = "https://files.pythonhosted.org/packages/b7/aa/8b53bceea5454d0b5602ffc81aaf3b80cc2e9b793fe1e054f690beb82429/yarl-1.9.2-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:22a94666751778629f1ec4280b08eb11815783c63f52092a5953faf73be24191"},
+    {url = "https://files.pythonhosted.org/packages/b7/f6/4daab7a2c4b3b4bb9fe6496ab658171cddcfc3f1f24154b64002763fa763/yarl-1.9.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:5415d5a4b080dc9612b1b63cba008db84e908b95848369aa1da3686ae27b6d2b"},
+    {url = "https://files.pythonhosted.org/packages/ba/7e/dd4d8a9bd9343ecc7b45d80b134549c801dda119032a8af71d3699eaf070/yarl-1.9.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:6e7221580dc1db478464cfeef9b03b95c5852cc22894e418562997df0d074ccc"},
+    {url = "https://files.pythonhosted.org/packages/bb/98/9af77ac76f61ced2a4fb243c16cca6d941801927a332fb9d95da3899ed70/yarl-1.9.2-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:3458a24e4ea3fd8930e934c129b676c27452e4ebda80fbe47b56d8c6c7a63a9e"},
+    {url = "https://files.pythonhosted.org/packages/c4/0c/7898c35ca4945fdd416e1dadeda985cc391e4f9298ae5e71c3a5cd88e82d/yarl-1.9.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:838162460b3a08987546e881a2bfa573960bb559dfa739e7800ceeec92e64417"},
+    {url = "https://files.pythonhosted.org/packages/c9/d4/a5280faa1b8e9ad3a52ddc4c9aea94dd718f9c55f1e10cfb14580f5ebb45/yarl-1.9.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:891c0e3ec5ec881541f6c5113d8df0315ce5440e244a716b95f2525b7b9f3608"},
+    {url = "https://files.pythonhosted.org/packages/d0/17/875e45f3369af23ae6a299dab56140c4b5398b76757bc3b8388454277ba2/yarl-1.9.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:83fcc480d7549ccebe9415d96d9263e2d4226798c37ebd18c930fce43dfb9574"},
+    {url = "https://files.pythonhosted.org/packages/d5/8b/5a30baa12464d55b308c684a4a953df6b2190f7733c92719f194fcd42421/yarl-1.9.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:822b30a0f22e588b32d3120f6d41e4ed021806418b4c9f0bc3048b8c8cb3f92a"},
+    {url = "https://files.pythonhosted.org/packages/d9/cb/0bfa73fad2049b6315ace645df2bd0682e20f9eb2dac120c2e9183359aa1/yarl-1.9.2-cp311-cp311-win32.whl", hash = "sha256:a60347f234c2212a9f0361955007fcf4033a75bf600a33c88a0a8e91af77c0e8"},
+    {url = "https://files.pythonhosted.org/packages/d9/cf/bf402f68933fec675b608a941752b836bc25fa2ec7d6922a1b1f315214b5/yarl-1.9.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:8c56986609b057b4839968ba901944af91b8e92f1725d1a2d77cbac6972b9ed1"},
+    {url = "https://files.pythonhosted.org/packages/da/1a/94328f245b0f38913338cfa817826def45c193cfc75c76905392f6b484f8/yarl-1.9.2-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c1012fa63eb6c032f3ce5d2171c267992ae0c00b9e164efe4d73db818465fac3"},
+    {url = "https://files.pythonhosted.org/packages/de/3f/5a8fcff69c8628ce4dab00612981f4c0598fb9aabd90d01a1ebb037bb6f6/yarl-1.9.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:95d2ecefbcf4e744ea952d073c6922e72ee650ffc79028eb1e320e732898d7e8"},
+    {url = "https://files.pythonhosted.org/packages/e4/a7/6ffee644828e01c6d6ae177ac6cba56255bb793f79c4d32082a895bf8b91/yarl-1.9.2-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:e9fdc7ac0d42bc3ea78818557fab03af6181e076a2944f43c38684b4b6bed8e3"},
+    {url = "https://files.pythonhosted.org/packages/e5/12/4fd9a60b167b00a58552020babb638f9b43c514da0227df9fc6bdf16948f/yarl-1.9.2-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:32f1d071b3f362c80f1a7d322bfd7b2d11e33d2adf395cc1dd4df36c9c243095"},
+    {url = "https://files.pythonhosted.org/packages/e8/3b/38f2427f7ee497e169d7f8bd74c92a6ace98594c6a921b619ccc57703fe5/yarl-1.9.2-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:5610f80cf43b6202e2c33ba3ec2ee0a2884f8f423c8f4f62906731d876ef4fac"},
+    {url = "https://files.pythonhosted.org/packages/e9/12/f4989d778d8dd137fd58f55ab3a5501175896b8670239b4822ae44afd4ed/yarl-1.9.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:662e6016409828ee910f5d9602a2729a8a57d74b163c89a837de3fea050c7582"},
+    {url = "https://files.pythonhosted.org/packages/eb/cb/4970008c85810c7d0e154ac5d746451b04476ac1dd85dc538563a1c04698/yarl-1.9.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:8c2ad583743d16ddbdf6bb14b5cd76bf43b0d0006e918809d5d4ddf7bde8dd82"},
+    {url = "https://files.pythonhosted.org/packages/ee/8d/55467943a172b97c1b5d9569433c1a70f86f1f9b0f1c6574285f8ad02fc2/yarl-1.9.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:159d81f22d7a43e6eabc36d7194cb53f2f15f498dbbfa8edc8a3239350f59fe7"},
+    {url = "https://files.pythonhosted.org/packages/f0/39/e28eec982b1dfd7d6044e5af6f0ca0c1d5760c82f0667a72b0698237d61f/yarl-1.9.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:c027a6e96ef77d401d8d5a5c8d6bc478e8042f1e448272e8d9752cb0aff8b5c8"},
+    {url = "https://files.pythonhosted.org/packages/f0/cc/cf416dff5bd88899a567fea556a5f68ab94cdf525ebe122e0bdba478f2c4/yarl-1.9.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:52a25809fcbecfc63ac9ba0c0fb586f90837f5425edfd1ec9f3372b119585e45"},
+    {url = "https://files.pythonhosted.org/packages/f1/0c/c2e07b3a37c4363078a1c7d586b251eec191594a2d24d6e09dae33c1368f/yarl-1.9.2-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:1b1bba902cba32cdec51fca038fd53f8beee88b77efc373968d1ed021024cc04"},
+    {url = "https://files.pythonhosted.org/packages/f2/b1/9a6eeba1a3f35188eac6b7b535f20c06df0f48e78705405d86a0407e75f1/yarl-1.9.2-cp38-cp38-win32.whl", hash = "sha256:f7a3d8146575e08c29ed1cd287068e6d02f1c7bdff8970db96683b9591b86ee7"},
+    {url = "https://files.pythonhosted.org/packages/f2/ea/6fd350376ed2581d0cdb11018bad0215cf987817dba69ea9a4bf8adbac6e/yarl-1.9.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:8288d7cd28f8119b07dd49b7230d6b4562f9b61ee9a4ab02221060d21136be80"},
+    {url = "https://files.pythonhosted.org/packages/fb/2d/060ab740f64ea6ea2088e375c3046839faaf4bbba2b65a5364668bd765e7/yarl-1.9.2-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:84e0b1599334b1e1478db01b756e55937d4614f8654311eb26012091be109d59"},
+    {url = "https://files.pythonhosted.org/packages/fe/7d/9d85f658b6f7c041ca3ba371d133040c4dc41eb922aef0a6ba917291d187/yarl-1.9.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aff634b15beff8902d1f918012fc2a42e0dbae6f469fce134c8a0dc51ca423bb"},
 ]
 "yt-dlp 2023.3.4" = [
     {url = "https://files.pythonhosted.org/packages/a7/df/498c57f641e9993376cf52489047158e6d660e8bab06b72c470ad5cce2bd/yt_dlp-2023.3.4-py2.py3-none-any.whl", hash = "sha256:40ca421407ce07c8fd700854fd978d58526ec6fff3468caa34ff1c7333b8dc34"},
     {url = "https://files.pythonhosted.org/packages/e8/4a/1e01f24fcb49191626e2b17d00e13a093315d03a9da09fccb1c75913e420/yt-dlp-2023.3.4.tar.gz", hash = "sha256:265d5da97a76c15d7d9a4088a67b78acd5dcf6f8cfd8257c52f581ff996ff515"},
 ]
-"zeroconf 0.58.0" = [
-    {url = "https://files.pythonhosted.org/packages/07/92/c3c14cc65035785c1f738754b46b100f87da505f1f6d406c4167f42ba8df/zeroconf-0.58.0-pp37-pypy37_pp73-macosx_11_0_x86_64.whl", hash = "sha256:0b7a67d89ff9d89dd8359140f7da7ab04d1a300ef12544e79c90c6580477e700"},
-    {url = "https://files.pythonhosted.org/packages/17/8d/9e40a10d1427920a12225e2a2020f12ca294a76c57b546931e69ed9bf342/zeroconf-0.58.0-cp310-cp310-win32.whl", hash = "sha256:29350397f418e293e0027979c5c6f3896427e5c216e58b69a80a0f90e1403772"},
-    {url = "https://files.pythonhosted.org/packages/1c/36/a799d65270032f239902b811a67c45429d4e74693a4ca0d8aadc98332c5e/zeroconf-0.58.0-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:df88cd245f4ed6a0e70affec09fb39303ac2a5a46ee717bbaaeaca0a044d3980"},
-    {url = "https://files.pythonhosted.org/packages/20/cc/4933425464e991817fcceb5d95570bd3c007873e71ce4ce24dcb42338d48/zeroconf-0.58.0-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:240b34f92bbf669729161a1062ae54e1c9de6864fa7871f575b49e2597ddb27f"},
-    {url = "https://files.pythonhosted.org/packages/31/fb/ec30f85212f77f3b09a249062e6bfa095024cea47b2bfeabd349fc8fab2f/zeroconf-0.58.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:769a97230d5f957e776bf81105ee8a4997323574c4a24a515781293779515025"},
-    {url = "https://files.pythonhosted.org/packages/32/12/85e5d32ffea6f7a6ea852e4daa19c1dcdd72fbc336aaf99d722160738eb9/zeroconf-0.58.0-cp311-cp311-win_amd64.whl", hash = "sha256:aa1f3d47401f477d092eaa044e0b6378a7ad6715bb167c0c944d2c0b78acf635"},
-    {url = "https://files.pythonhosted.org/packages/3b/01/3a59b44db1fd917530f40266cb122bbb31ad2ecc6db60b9f9ea77d2f8e09/zeroconf-0.58.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:a0a13ca24065d89efe31762df3a7ab4f72a9b757609cc74699008266e613bb0c"},
-    {url = "https://files.pythonhosted.org/packages/41/dd/0aae3b1cd5bc49d3ece720fd79cbd3e429f59a5bd8a38f586f9dc093aaf6/zeroconf-0.58.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux_2_5_x86_64.manylinux1_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dc39d5f3f7ce0f22a29a087d3fabbda4dc11a9a493c1f34c651d199dad0e52b3"},
-    {url = "https://files.pythonhosted.org/packages/45/e7/2d4ed8455f414f7e91341d0f921b379322a32baab3d91ec2d1b557e11eea/zeroconf-0.58.0.tar.gz", hash = "sha256:391bc9fecb6a5e9b502eca7b0baf7001e648c2b4374b8e98e3e9387206926a4e"},
-    {url = "https://files.pythonhosted.org/packages/46/c6/f051af24eb840c90c6411dbbe8827443d77160f16e6ba5346a97b52cfe41/zeroconf-0.58.0-cp37-cp37m-win32.whl", hash = "sha256:9d031131d0a9db06fb14f99218e2f52a9784d799b843c514ed4aa164e97ef66a"},
-    {url = "https://files.pythonhosted.org/packages/50/55/08eefc5ec22ce56d97fcac2f9b2eac0117af274605c12fe0591ac815fb00/zeroconf-0.58.0-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:98cc5fece6d541bb6316e999cdd8b64c2ea3a40758ac8f90b965b5d17bb8cdcc"},
-    {url = "https://files.pythonhosted.org/packages/51/33/5d18cccf73a93b49cc1e34f61638389b65f4e1fc122f5399733bdea0db01/zeroconf-0.58.0-cp37-cp37m-win_amd64.whl", hash = "sha256:8b7e3bfa64e418753c5267c936679beff2a14b06710b7a9cff844aaf42159320"},
-    {url = "https://files.pythonhosted.org/packages/55/a3/8b486bd257ddef3e6ffc4fb3f1340639776f2c0b754e6576bde9626de00d/zeroconf-0.58.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:2bdcca252fb67176d5c7066915ee54710562d6600bf86c7f62387556b14d1937"},
-    {url = "https://files.pythonhosted.org/packages/58/25/b4c9bb30f393d434a913d9da6a4eb3c18c273009a09df646bf4480dc7f9c/zeroconf-0.58.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c30995918d6efcf510997b4010b8a93a8d6842937626df39285e93bc6ceaccb4"},
-    {url = "https://files.pythonhosted.org/packages/5b/7a/7368a856d2ee947eb4d1c240eb222b922d0a102e197637cb2a36435a735d/zeroconf-0.58.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:157e64b9cbf93c5d5d0338f7e178093367e2cd7cf9c64c79979f7b1e08c72b23"},
-    {url = "https://files.pythonhosted.org/packages/66/65/a282de824d3d2cfd7005f5878bee9f85cfad6d8ee4229590a19f7cb3be84/zeroconf-0.58.0-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:290e4f809898c0cb280d4acb7bc32159a498d3039f3b0c88632d4ba5d9cc7fac"},
-    {url = "https://files.pythonhosted.org/packages/6f/63/c5b3537991b7b42ef0a599f7b486c45d3e5e9c7bbe84bf74b59bd5c38466/zeroconf-0.58.0-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:c4e4b9cc2e0b83c9744b2aec55007b0953d903cbbc86b6c0f15f63de29951cb4"},
-    {url = "https://files.pythonhosted.org/packages/70/1f/80ddeed142db1f4439f9259903605a88bb71c246fbbc84e9126683e52e3f/zeroconf-0.58.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:69dce69a93a465a1b86086a54f2299c65cc42b793fa757328d2ee65e7d803333"},
-    {url = "https://files.pythonhosted.org/packages/70/f7/0854686465acfb5aae69a56d3c4d76a2d0ca4b2c602ecb88941f00963664/zeroconf-0.58.0-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:f29c52bc9494b1677cf9da760d4b4972909075cceca31aee3e17bcc52b17875f"},
-    {url = "https://files.pythonhosted.org/packages/72/6d/a124ec67b729411cee60cca1883770b03b63f5b40ac2e69fabe88396a6d6/zeroconf-0.58.0-cp39-cp39-win_amd64.whl", hash = "sha256:d394f720830d18ef5df8ac87ac7c9b41c9c160b659d7d87c707e1548dbfc0398"},
-    {url = "https://files.pythonhosted.org/packages/78/c6/7a19a4029a2b1597801856cada2b9c404acadb53aab7c0c954e78e7b5c4a/zeroconf-0.58.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bab4785e63e34a92118e42fed3308e60c8429443b7f2fcdb84a68ad3460669fb"},
-    {url = "https://files.pythonhosted.org/packages/7a/1e/1eee40ea648dab76808bb07a3ea7382dba7ae45a64b62035b42c2a9144f3/zeroconf-0.58.0-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:bbc820a4308ac6a81f4829df9959e19228fd262745e8de060be73a150fcc5abf"},
-    {url = "https://files.pythonhosted.org/packages/7d/d1/341c5118eb0722a60aec540652dd23c2e2cce0d18f0a007732a119485f44/zeroconf-0.58.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:34749a3c6e16e67eed4d78ca83561dcee93b95a7fe651b8ebe7d2a630c00c9af"},
-    {url = "https://files.pythonhosted.org/packages/7e/59/235dad814a6a356bfc2ee400779996297062cabb9f1d3468f66ab2274c65/zeroconf-0.58.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:262de8bbaa29833742a27a1adbe5c37a2157c6265993a9675640f53fd722ff63"},
-    {url = "https://files.pythonhosted.org/packages/87/0f/8824e8c3e69643e51410f814a0a5564af486ff860047bd395b8dd475ec62/zeroconf-0.58.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:72d55f8c41324271ecc756f39cf20f7980fb76783d79fdd7f4ec84c30648ac79"},
-    {url = "https://files.pythonhosted.org/packages/87/44/f0aee0c1c9485a80861e11595e6fc7cdf770b15a4a2c26410a74bce664a2/zeroconf-0.58.0-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:09b6dde642b84e10312190a9a1adac8222ccb3d1e8064b3acf1847f93043ce9c"},
-    {url = "https://files.pythonhosted.org/packages/8c/09/f8a84e24dedf70256c1cec55fe5be5d5f5c26c3a8ec74e6c304931d00251/zeroconf-0.58.0-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:76c677c4286338e79bc825d9becf7e303f9e51ff3225ff98b1c5226541f25b49"},
-    {url = "https://files.pythonhosted.org/packages/94/83/be4921d9e19eac676d8fd8302c913f83d2bd9a215a80ba3fd2a3d7184d7c/zeroconf-0.58.0-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:002ff2e5f61d4d3c1828e577c05368a383118770208d39ccec4499656953b3a9"},
-    {url = "https://files.pythonhosted.org/packages/95/8d/97480c7bd0e20a0910e5aec90d04edb751253f3a84c01b3e92067703d8ae/zeroconf-0.58.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:640fd8ce7b54b2ebfe04916b5f92bcb0920803c4c64eaee2de4ffb990d5b1a58"},
-    {url = "https://files.pythonhosted.org/packages/99/24/cb76535580d4f93f6889330fa3842711d6fbd1055c260a3ac92c912354f9/zeroconf-0.58.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:d4e56cfa6d4776273aad3af2679ce213e83b02987c05e63c30221185837e36b8"},
-    {url = "https://files.pythonhosted.org/packages/9e/0a/a7a1c6a7b147b4b6cb9f473228a0413396e2ce6e2d2cb88e3c334f518d09/zeroconf-0.58.0-cp38-cp38-win_amd64.whl", hash = "sha256:707bc1a76188145fe2573581e5d2e440ad576312d7be993be005f1a5a8d79673"},
-    {url = "https://files.pythonhosted.org/packages/a4/f4/3cce4290f95ce02069a9e0398db7b8912b4088bf7b70234f7fb8ab62f51a/zeroconf-0.58.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux_2_5_x86_64.manylinux1_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6fd516e5847c03c4f3a599cc6cc6b04d9cd3bed3c5e3a738714dd0d7b6f640f3"},
-    {url = "https://files.pythonhosted.org/packages/a7/ea/f9bff79a34675b9390913c0d7f38393dd052f7ccd8bb4cdb5b98acde4988/zeroconf-0.58.0-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:bda4415761dde9a5b32fbf06d2a0715fa60e89b5fe4165ee703fa70993a5d1db"},
-    {url = "https://files.pythonhosted.org/packages/a9/b7/26304980095c4b712591492846a9fb1778782be3aa14f94c6e669d77ee19/zeroconf-0.58.0-cp38-cp38-win32.whl", hash = "sha256:dca9da700a3703a30904bd607b686e83af5b68040f189e390c3c14027dc62f85"},
-    {url = "https://files.pythonhosted.org/packages/ad/c4/08c95648ef772f9845c951e47087429fbac707829ff35158c1017ca4d6d2/zeroconf-0.58.0-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:82cea9c88ed505d126eb439f03f3cb884d43a8d40c1a344047ef8a90e1a6b578"},
-    {url = "https://files.pythonhosted.org/packages/b2/3c/a2fa186934ac46e795d54cf324499f8707054b1a764bf12e3b8b6d0c8f18/zeroconf-0.58.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:52a64f24bc6dc710c75b864292f487303264dee369c804c219afd6fb0c6941d7"},
-    {url = "https://files.pythonhosted.org/packages/b4/67/31530df0fa6597653a442d70bb2fd07cb8b02b7e346f4545833583293b12/zeroconf-0.58.0-cp37-cp37m-macosx_11_0_x86_64.whl", hash = "sha256:22aae0465492376383da5be213dcdab1943d3d7b4156cc9ccb37a8893b61305a"},
-    {url = "https://files.pythonhosted.org/packages/b6/ed/40d452d8fdf625e810426e2ed64f6af1d471fc217fed2437cec76f4fc6d9/zeroconf-0.58.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2e60d5517d3027861a4c02ab8b6173a9768fbf0a13c881de8619336a18c2ac4d"},
-    {url = "https://files.pythonhosted.org/packages/b9/5d/7297bfce7fc41de28182e46a2a5e5a1bb5cf0fff0ae8edd5db88d6ae17f8/zeroconf-0.58.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:1cb248f8b60e2f2c6008115001e00ac1dfd4eee2b65240a9c8e1f69bbe793bef"},
-    {url = "https://files.pythonhosted.org/packages/be/a2/2a2fece44a41d95e7bd6eae2d0542ed0716280dde14b1000b62a5c6136b3/zeroconf-0.58.0-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux_2_5_x86_64.manylinux1_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b5afd42e3d3be046799c27ac1df3a15f939f06c8fa5fe61686650da003bb1ffb"},
-    {url = "https://files.pythonhosted.org/packages/c7/69/f326ec4200240a6b424135a13ff7a63e38376a2a0abe93f8b1495ef7d9b9/zeroconf-0.58.0-cp38-cp38-macosx_11_0_x86_64.whl", hash = "sha256:63dab853ec07d14795346ad8c86fd41d328c630036480d83cb904d65c43d8d03"},
-    {url = "https://files.pythonhosted.org/packages/cb/6b/45156039dc31b65e1f1f8fc113641ce0f1e2a15567bd8657e97f11b87c5b/zeroconf-0.58.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:86c74be41c7128b0b74096661b810cbf78582137f8c028590fc1136eea2a10bb"},
-    {url = "https://files.pythonhosted.org/packages/ce/c7/9f6375d7159e2d0e08eb7f6aeeaa3cee47230ca1eded9430e6b5bc7e4492/zeroconf-0.58.0-cp38-cp38-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:95e11e9720cf288e8478c2835640d56f655f7854bf074f54d7b0ee6aebaa7774"},
-    {url = "https://files.pythonhosted.org/packages/df/b3/e23933eaf489ece15d80b1b9974eae17c355ad35b3a8419bb3ac4d9cde6c/zeroconf-0.58.0-cp310-cp310-win_amd64.whl", hash = "sha256:1a9523f60f36388ff61c17b48e8d7218c190b15a0066af263bc58847253e7bb1"},
-    {url = "https://files.pythonhosted.org/packages/eb/56/c7e796f470c1c3cf8be1ea5d1a00dd479e856d7103036e81f9c9df5828b5/zeroconf-0.58.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:c8c4ef7748507307cc21ecc25c69c634cd4476d87961a0f8c1ad404c0a6fca30"},
-    {url = "https://files.pythonhosted.org/packages/ee/07/8eec42ae536cf656ffa2cf9b3287c09835b878d7d86a02e2849fdc60a406/zeroconf-0.58.0-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:5e1fe87e06dba5ba006ffb624706e81daef1f83d2320c5bd7e1a7a463af439ca"},
-    {url = "https://files.pythonhosted.org/packages/fb/37/d80b2141ea859deda2e0cbea5a159bb861b6ab45f7e7d266067887265e8c/zeroconf-0.58.0-cp311-cp311-win32.whl", hash = "sha256:8961e94d4345599651030f08bee5cbea6c66da4856595354f323f902da027a09"},
-    {url = "https://files.pythonhosted.org/packages/fe/70/997f85644cad510f09cdc88aeb6c7f62e36436252d030ce0ef6ac9cb55a8/zeroconf-0.58.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:4f1189715dfd466348763cf436eec28879a3251546844dd48445d3ec90057bbd"},
-    {url = "https://files.pythonhosted.org/packages/fe/a7/4b2eecaac3ef5e42d9b68a6bf1438e199a5d695202be66eb1089e729bed5/zeroconf-0.58.0-cp39-cp39-win32.whl", hash = "sha256:f1e909cc7942e32aec6d62ccc1d35bd0713e86ceddebec0914ea955610c0e560"},
+"zeroconf 0.58.2" = [
+    {url = "https://files.pythonhosted.org/packages/02/1e/3061b8d2da4b0b03e8dd7e6785573566278252c691be8e2088f8edc6ed7d/zeroconf-0.58.2.tar.gz", hash = "sha256:879067cec1d01b5c819df456b6f8fa8e88500fe0da1a40019bff9627bb9f3b58"},
+    {url = "https://files.pythonhosted.org/packages/05/8d/92240c2c79fab200d845f5ca1928772681eceac541b6b759ea94a797f08b/zeroconf-0.58.2-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:a717559f62385bf2be17f314fb7a0a01ed865f0336b0ea0e546deb18b4ea06cb"},
+    {url = "https://files.pythonhosted.org/packages/06/7e/34bfc646cbdbb8a6ffeb4f8fb34161894803438fceb80aceb6f2417c0a43/zeroconf-0.58.2-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:77a21858eef1a2a17996bfe33e5beac7e92a37ce95fdb65f18b5376da940dcf5"},
+    {url = "https://files.pythonhosted.org/packages/0d/85/d28dc222bd30e404a0b8b993619a3c5b125f504f04056bc9bd1ae8c70d82/zeroconf-0.58.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8d078a9dedc29d6924f342e9b50b4cd77adea10785b6026d48c422a42d2f83ac"},
+    {url = "https://files.pythonhosted.org/packages/13/89/2dda922840c1d4b308463d87a00eef6d2d275b577ab9dc7e5c4246f13df6/zeroconf-0.58.2-cp38-cp38-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:2485467ac159fc0c85a71df213b88890e7dcc0bc7bd147859c781b1897d544f8"},
+    {url = "https://files.pythonhosted.org/packages/17/ff/ca19993987699c9c38de4c024689b900bbc3713ad8087fea15d8b40a9859/zeroconf-0.58.2-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux_2_5_x86_64.manylinux1_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1b6d08c6171625ce674e11d7aedf49bc8e887cfa6e40b8afa904d65701288c23"},
+    {url = "https://files.pythonhosted.org/packages/1e/c6/8dad500f9b21c6e0b122f93b709b1cafde727bdc0b780487f542a7bdc9b2/zeroconf-0.58.2-cp37-cp37m-macosx_11_0_x86_64.whl", hash = "sha256:2838a6a5a26985f5ab92c470d40e66094f9fb966864da9eb863c5b4c502bd3f5"},
+    {url = "https://files.pythonhosted.org/packages/1f/bf/5dc41b9f5e73b6f24acd743334dce6b295f03030e3b8659e4f9b5483d2e6/zeroconf-0.58.2-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:e8ff7e8232750711e7190166e12f21120a6aa483b8394675346f467e3f2e89c2"},
+    {url = "https://files.pythonhosted.org/packages/20/2b/5d03d15ad4325bea92799309b748125b07075c776d0b30c149b4869d349c/zeroconf-0.58.2-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:f2d74f268b1a101db89991e9ea6fb2ad2df294b4d74c9862b0e8d065cd4eea5f"},
+    {url = "https://files.pythonhosted.org/packages/2c/fb/a6e5f554e8f495b231e38f0e5eabd7ff40765a90b1c214c9554988748152/zeroconf-0.58.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6a232ea50730d0549d983d30d29e094cb275b2335fe0b8d73359076a1dfcf3f7"},
+    {url = "https://files.pythonhosted.org/packages/31/79/ab0346c262c276aa58e7c7cbcc8a64deb75c23bf5ca893937254612df0f2/zeroconf-0.58.2-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:85c0214be21d389f6118f59b154a4520918e732ed343d7a005910707e2daffad"},
+    {url = "https://files.pythonhosted.org/packages/3e/b3/b44c1950ceffd161b15d41f07d3d07dac5cd6f82d2281dda7cf1b0a50b0a/zeroconf-0.58.2-pp37-pypy37_pp73-macosx_11_0_x86_64.whl", hash = "sha256:08cf1026800751a92a1aee66c71b356855c896d876349e463ef694790c40bbdd"},
+    {url = "https://files.pythonhosted.org/packages/43/22/14e39343504d5fc9c936351233a0866a35c4fd28181bf4ccede96b3f853b/zeroconf-0.58.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:abb44440d1dd23a3bd26d7ef17478968d429231f4879757e5e03ac2f24186fc3"},
+    {url = "https://files.pythonhosted.org/packages/46/17/3eb2f75dd921805a4a7078ad043f556b28ace938a55aea9d9afa35248f79/zeroconf-0.58.2-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:e13ecac3553c19298b9fbd70e093984f97df6dd39c9515a61912e13dbf0b7100"},
+    {url = "https://files.pythonhosted.org/packages/47/4e/d185278c92fdd35daa7cd682abe7528ebf59d7c7ccf665fb2f25283a7794/zeroconf-0.58.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:b6f33d7edef14422464be6512345078046fcb6e6de081c1a46dcf63769123f81"},
+    {url = "https://files.pythonhosted.org/packages/4a/54/3f9e0cb47f9c4f0402fe944a781996c9cecb8b2e735771b966fa5e4c5bfb/zeroconf-0.58.2-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux_2_5_x86_64.manylinux1_x86_64.manylinux2014_x86_64.whl", hash = "sha256:585de611c993593fd9bb8b62ca136d3429cac429327b3822a7b556573163a8ae"},
+    {url = "https://files.pythonhosted.org/packages/5f/f3/3a8dc92f01bded38aaac872e20bf6779a085377facec82844fa9cf2e80a7/zeroconf-0.58.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:83b538bbe2a3f4cdea50f9d6920923493e871a5b74dc61f7624f53836270b142"},
+    {url = "https://files.pythonhosted.org/packages/81/e4/e9f00849d19c0f1a759cf9f2599cbd0dbaef6c5ac53128d9b08360e91695/zeroconf-0.58.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:331eadee65f5c20996a69554adacdda9071e5251ce7cb143cd98fdb0ba4ca94b"},
+    {url = "https://files.pythonhosted.org/packages/8f/a3/e721d32db27168b8a59263f39f99ff0964124e29205548e83dc858a55bab/zeroconf-0.58.2-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux_2_5_x86_64.manylinux1_x86_64.manylinux2014_x86_64.whl", hash = "sha256:54e8f722f3a879ecbee0197b917b874ac17a87e1ec8c17b6fc33cb83ebf41038"},
+    {url = "https://files.pythonhosted.org/packages/93/99/924ce6a2f035b2c2211690c59912e4d9c9e6fc75437a1dd2187f5be4b770/zeroconf-0.58.2-cp38-cp38-macosx_11_0_x86_64.whl", hash = "sha256:56264b936421d9cffc2bd487c6b929861ebad7e4f11a22d9ace737f42c77a150"},
+    {url = "https://files.pythonhosted.org/packages/95/c3/19d7f57c4f3a5323e5dd3651803878ff724014c9917ed35bf999b8ec1b40/zeroconf-0.58.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:454cc6cb497f2c92999de9673f87b30f1dd6d09066614b7d99d4e5429de9a3ac"},
+    {url = "https://files.pythonhosted.org/packages/96/1b/afe9710c1506091a7b128e0514a8a9783bf80b6d7a0795a5a8c1387a1388/zeroconf-0.58.2-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:963e2d8b786b9be0960d6d2aa3787d93329f481a244b572c5d903402e197ec72"},
+    {url = "https://files.pythonhosted.org/packages/a3/f9/404ff15dd73da93b6fba568ad11224751d74f349d4749a9471c23b74779d/zeroconf-0.58.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:059ab32bb31b254677f74248ab705a0f58b05f5b421c9bf65e66e16cf6ac1dbb"},
+    {url = "https://files.pythonhosted.org/packages/a5/e0/a7451114308a466608e78276e0c53d6a9ece88dc9b3429111c93bcb8511e/zeroconf-0.58.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:9608e8e1d182e2367d7822efd03c7e7e97df845e1b635ad2493c337966cb3f24"},
+    {url = "https://files.pythonhosted.org/packages/ab/18/92e96b31debd368cd2f2106206e97dfc2482fef496eef69a334bdd7a2da1/zeroconf-0.58.2-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:30b6c8d568127cf0232ec24f8651a383b2742b5a950cbde1d349cfbcb18dfc2e"},
+    {url = "https://files.pythonhosted.org/packages/ae/df/bc9f667bd8d21dcf2645d672ad49d28245ce29bcf3ea3d2de0c7c4dac070/zeroconf-0.58.2-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:ca378b48991f57b2fc90b44407f3220fd47214dedfb2721cbafbb986a4038fc4"},
+    {url = "https://files.pythonhosted.org/packages/b2/a2/5b1dd1842f70af0cbca9a5f6a6e0bd612098b95a4721d4f21de25a31a37d/zeroconf-0.58.2-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:37bbc193a5efc8ac177ff4ba9efedff5174aa6dbec81de03e64d33cad699becd"},
+    {url = "https://files.pythonhosted.org/packages/b2/cd/dcd80ee94306a1143c300ada083c3d81866a41be27b951fa1862c7b84281/zeroconf-0.58.2-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:cbb2caf116cc68039e0cc0b05e15ba805a8bc06c37d0a5af3c07e0e893e95bad"},
+    {url = "https://files.pythonhosted.org/packages/bb/64/1a44c0e93f159cecc2c9cc508c259316eea1b1655bd4e03e5e64b141466f/zeroconf-0.58.2-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:35b589aeaf8f130debc8db2b20a1bf0eebafe5bb962fbbb793feb38a6fe15c1e"},
+    {url = "https://files.pythonhosted.org/packages/c1/a3/5b5e71c30e15a2581d6c31297b8365938c1ac872f4552e82ac3b63eec928/zeroconf-0.58.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:afe0e14aa38421463c77dd449416ff59cb9059bd23000b7d60a93817788ae21a"},
+    {url = "https://files.pythonhosted.org/packages/ce/ca/f93f443e10dccfa34a33e9fc87918f90a4bef33c4c019a4f5a6be1f648e3/zeroconf-0.58.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:0a3ed0bdae1efb7e3689339f8483e9f6857ec08b5d45dcf045ff553919a822ab"},
+    {url = "https://files.pythonhosted.org/packages/d1/4a/6f61f8895663b2edb1e77a677da71e56db4ad952200e544baa1cfbd6b440/zeroconf-0.58.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:bd5adb33f2a17c78123bf723a412c43cb8ce59337e36901b3d6246e0b49a0e29"},
+    {url = "https://files.pythonhosted.org/packages/dc/6e/0d6d7b8ba0163f4ab61d2e45bb6bbb75207ec6679b7a763c646dd35bcc62/zeroconf-0.58.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:a12e26b3b1bdb70d0d218d1f266ce6f095fade355ebe89cb7bc2bfaa45383818"},
+    {url = "https://files.pythonhosted.org/packages/ef/84/792f4cfa88b1364920880402d05ac05faa500def799cef459bf590f74941/zeroconf-0.58.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:4d943ef75d0ac66188e8953b06c25bdb610dbe56d1ed17485903ddf5881d007b"},
+    {url = "https://files.pythonhosted.org/packages/ef/88/457a942ab186ea16ea00b65363653b100e4aa2b0a84b5f3d2bccbec4b9e9/zeroconf-0.58.2-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:99b2c7e0a5330555cb5f85299de1990da0353b31bb628331626140ff3e997308"},
+    {url = "https://files.pythonhosted.org/packages/f0/08/ac916991a2a157d5a516ec72c0449a59752dcd6a25c6b8f81ba95596f5c2/zeroconf-0.58.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:701c45c1d5565d60a3d9ff3d4b7078fda350676cfe23b45a38eef6be609cd07a"},
 ]
 "zipp 3.15.0" = [
     {url = "https://files.pythonhosted.org/packages/00/27/f0ac6b846684cecce1ee93d32450c45ab607f65c2e0255f0092032d91f07/zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
     {url = "https://files.pythonhosted.org/packages/5b/fa/c9e82bbe1af6266adf08afb563905eb87cab83fde00a0a08963510621047/zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
 ]
```

### Comparing `xklb-1.26.13/readme.py` & `xklb-1.26.14/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.26.14/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.26.14/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/.github/workflows/push.yaml` & `xklb-1.26.14/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/av.py` & `xklb-1.26.14/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/books.py` & `xklb-1.26.14/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/consts.py` & `xklb-1.26.14/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/db.py` & `xklb-1.26.14/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/dl_config.py` & `xklb-1.26.14/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/dl_extract.py` & `xklb-1.26.14/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/fs_extract.py` & `xklb-1.26.14/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/gui.py` & `xklb-1.26.14/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/hn_extract.py` & `xklb-1.26.14/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/lb.py` & `xklb-1.26.14/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/play_actions.py` & `xklb-1.26.14/xklb/play_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,21 +714,14 @@
     )
     Path(path).unlink()
     shutil.move(temp_video, transcode_dest)
     return transcode_dest
 
 
 def play(args, m: Dict) -> None:
-    if args.safe and not tube_backend.is_supported(m["path"]):
-        log.info("[%s]: Skipping unsupported URL (safe_mode)", m["path"])
-        return
-
-    if is_play_in_order_lvl2(args, m["path"]):
-        m = get_ordinal_media(args, m)
-
     original_path = m["path"]
     if args.action in (SC.watch, SC.listen) and not m["path"].startswith("http"):
         media_path = Path(args.prefix + m["path"]).resolve() if args.prefix else Path(m["path"])
         m["path"] = str(media_path)
 
         if not media_path.exists():
             log.warning("[%s]: Does not exist. Skipping...", m["path"])
@@ -778,15 +771,15 @@
             player.set_playhead(args, original_path, playhead)
     player.post_act(args, original_path)
 
 
 def process_playqueue(args) -> None:
     query, bindings = construct_query(args)
 
-    if args.print:
+    if args.print and not any([args.partial, args.lower, args.upper, args.safe, args.play_in_order > 0]):
         player.printer(args, query, bindings)
         return
 
     media = list(args.db.query(query, bindings))
 
     if args.partial and Path(args.watch_later_directory).exists():
         media = utils.mpv_enrich2(args, media)
@@ -804,20 +797,29 @@
             "sort" in args.defaults,
             not args.partial,
             not args.random,
         ],
     ):
         media = utils.mpv_enrich(args, media)
 
-    if args.multiple_playback:
+    if args.safe:
+        media = [d for d in media if tube_backend.is_supported(d["path"]) or Path(d["path"]).exists()]
+
+    if args.print:
+        if args.play_in_order >= consts.SIMILAR:
+            media = [get_ordinal_media(args, d) for d in media]
+        player.media_printer(args, media)
+    elif args.multiple_playback:
         args.gui = True
         player.multiple_player(args, media)
     else:
         try:
             for m in media:
+                if is_play_in_order_lvl2(args, m["path"]):
+                    m = get_ordinal_media(args, m)
                 play(args, m)
         finally:
             if args.interdimensional_cable:
                 args.sock.send(b"raw quit \n")
             Path(args.mpv_socket).unlink(missing_ok=True)
             if args.chromecast:
                 Path(consts.CAST_NOW_PLAYING).unlink(missing_ok=True)
```

### Comparing `xklb-1.26.13/xklb/playback.py` & `xklb-1.26.14/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/player.py` & `xklb-1.26.14/xklb/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -673,24 +673,17 @@
         else:
             delay = 10  # TODO: idk
         sleep(delay)
 
     return r
 
 
-def printer(args, query, bindings) -> None:
-    media = list(args.db.query(query, bindings))
-
-    if hasattr(args, "partial") and args.partial and Path(args.watch_later_directory).exists():
-        media = utils.mpv_enrich2(args, media)
-
+def media_printer(args, media) -> None:
     if "b" in args.print:
         media = process_bigdirs(args, media)
-    elif any([hasattr(args, "lower") and args.lower, hasattr(args, "upper") and args.upper]):
-        media = utils.filter_episodic(args, media)
 
     if args.verbose >= consts.LOG_DEBUG and args.cols and "*" in args.cols:
         breakpoint()
 
     if not media:
         utils.no_media_found()
 
@@ -724,15 +717,15 @@
             print(f"Marked {marked} metadata records as watched", file=sys.stderr)
 
     if "f" in args.print:
         if args.limit == 1:
             f = media[0]["path"]
             if not Path(f).exists():
                 mark_media_deleted(args, f)
-                return printer(args, query, bindings)  # try again to find a valid file
+                raise FileNotFoundError
             utils.pipe_print(quote(f))
             return None
         else:
             if not args.cols:
                 args.cols = ["path"]
 
             selected_cols = [{k: d.get(k, None) for k in args.cols} for d in media]
@@ -762,18 +755,26 @@
         utils.col_duration(tbl, "avg_duration")
 
         for t in consts.TIME_COLUMNS:
             utils.col_naturaldate(tbl, t)
 
         print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
-        if "duration" in query:
-            if len(media) > 1:
-                print(f"{len(media)} media" + (f" (limited to {args.limit})" if args.limit else ""))
+        if len(media) > 1:
+            print(f"{len(media)} media" + (f" (limited to {args.limit})" if args.limit else ""))
 
-            duration = sum(m.get("duration") or 0 for m in media)
+        duration = sum(m.get("duration") or 0 for m in media)
+        if duration > 0:
             duration = human_time(duration)
             if "a" not in args.print:
                 print("Total duration:", duration)
                 return None
             return None
         return None
+
+
+def printer(args, query, bindings) -> None:
+    media = list(args.db.query(query, bindings))
+    try:
+        media_printer(args, media)
+    except FileNotFoundError:
+        return printer(args, query, bindings)  # try again to find a valid file
```

### Comparing `xklb-1.26.13/xklb/praw_extract.py` & `xklb-1.26.14/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/stats.py` & `xklb-1.26.14/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/subtitle.py` & `xklb-1.26.14/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/tabs_actions.py` & `xklb-1.26.14/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/tabs_extract.py` & `xklb-1.26.14/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/tube_backend.py` & `xklb-1.26.14/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/tube_extract.py` & `xklb-1.26.14/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/utils.py` & `xklb-1.26.14/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/__init__.py` & `xklb-1.26.14/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/bigdirs.py` & `xklb-1.26.14/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/christen.py` & `xklb-1.26.14/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/dedupe.py` & `xklb-1.26.14/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/merge_dbs.py` & `xklb-1.26.14/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/merge_online_local.py` & `xklb-1.26.14/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/move_list.py` & `xklb-1.26.14/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/optimize_db.py` & `xklb-1.26.14/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/redownload.py` & `xklb-1.26.14/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/relmv.py` & `xklb-1.26.14/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/scatter.py` & `xklb-1.26.14/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/streaming_tab_loader.py` & `xklb-1.26.14/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/mining/nfb_ca.py` & `xklb-1.26.14/xklb/scripts/mining/nfb_ca.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/mining/nouns.py` & `xklb-1.26.14/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/mining/pushshift.py` & `xklb-1.26.14/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/mining/reddit_self.py` & `xklb-1.26.14/xklb/scripts/mining/reddit_self.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/xklb/scripts/mining/words.py` & `xklb-1.26.14/xklb/scripts/mining/words.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/assets/kotobago.png` & `xklb-1.26.14/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/.gitignore` & `xklb-1.26.14/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/LICENSE` & `xklb-1.26.14/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/README.md` & `xklb-1.26.14/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.013)
+    xk media library subcommands (v1.26.014)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.26.13/pyproject.toml` & `xklb-1.26.14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.13/PKG-INFO` & `xklb-1.26.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.26.13
+Version: 1.26.14
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -100,15 +100,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.013)
+    xk media library subcommands (v1.26.014)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```


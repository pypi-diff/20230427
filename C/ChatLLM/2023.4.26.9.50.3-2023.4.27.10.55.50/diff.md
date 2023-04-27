# Comparing `tmp/ChatLLM-2023.4.26.9.50.3.tar.gz` & `tmp/ChatLLM-2023.4.27.10.55.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.26.9.50.3.tar", last modified: Wed Apr 26 01:50:03 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.27.10.55.50.tar", last modified: Thu Apr 27 02:55:51 2023, max compression
```

## Comparing `ChatLLM-2023.4.26.9.50.3.tar` & `ChatLLM-2023.4.27.10.55.50.tar`

### file list

```diff
@@ -1,89 +1,95 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.726815 ChatLLM-2023.4.26.9.50.3/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.26.9.50.3/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.696066 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1789 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1604 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1789 2023-04-26 01:50:03.726660 ChatLLM-2023.4.26.9.50.3/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      974 2023-04-26 01:32:56.000000 ChatLLM-2023.4.26.9.50.3/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/README.rst
--rw-r--r--   0 betterme   (501) staff       (20)       97 2023-04-25 11:54:57.000000 ChatLLM-2023.4.26.9.50.3/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.696487 ChatLLM-2023.4.26.9.50.3/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.698805 ChatLLM-2023.4.26.9.50.3/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      775 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3307 2023-04-26 01:49:42.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)      542 2023-04-25 08:23:38.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/pipeline.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.699767 ChatLLM-2023.4.26.9.50.3/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      571 2023-04-25 02:29:53.000000 ChatLLM-2023.4.26.9.50.3/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1429 2023-04-25 08:29:49.000000 ChatLLM-2023.4.26.9.50.3/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.701014 ChatLLM-2023.4.26.9.50.3/chatllm/his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.26.9.50.3/chatllm/his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      285 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.50.3/chatllm/his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.50.3/chatllm/his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2492 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.50.3/chatllm/his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.701713 ChatLLM-2023.4.26.9.50.3/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.26.9.50.3/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.26.9.50.3/chatllm/parse_utils/doc_parse.py
--rw-r--r--   0 betterme   (501) staff       (20)     3326 2023-04-26 00:57:53.000000 ChatLLM-2023.4.26.9.50.3/chatllm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.703247 ChatLLM-2023.4.26.9.50.3/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1446 2023-04-25 10:54:31.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      221 2023-04-25 11:01:07.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.706999 ChatLLM-2023.4.26.9.50.3/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.710586 ChatLLM-2023.4.26.9.50.3/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.26.9.50.3/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.26.9.50.3/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.50.3/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.50.3/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.50.3/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.26.9.50.3/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.50.3/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.726076 ChatLLM-2023.4.26.9.50.3/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1342 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.50.3/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.26.9.50.3/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 ChatLLM-2023.4.26.9.50.3/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 ChatLLM-2023.4.26.9.50.3/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.26.9.50.3/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-26 01:50:03.726864 ChatLLM-2023.4.26.9.50.3/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1554 2023-04-25 02:27:49.000000 ChatLLM-2023.4.26.9.50.3/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.726406 ChatLLM-2023.4.26.9.50.3/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.159094 ChatLLM-2023.4.27.10.55.50/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.27.10.55.50/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.122110 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     4130 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1744 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4130 2023-04-27 02:55:51.158928 ChatLLM-2023.4.27.10.55.50/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.10.55.50/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     3313 2023-04-27 02:50:29.000000 ChatLLM-2023.4.27.10.55.50/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.122727 ChatLLM-2023.4.27.10.55.50/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.125426 ChatLLM-2023.4.27.10.55.50/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 02:55:16.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3328 2023-04-27 02:46:24.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1335 2023-04-27 02:53:02.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1879 2023-04-26 12:42:49.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/pipeline.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.126104 ChatLLM-2023.4.27.10.55.50/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.10.55.50/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.27.10.55.50/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.127254 ChatLLM-2023.4.27.10.55.50/chatllm/his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.27.10.55.50/chatllm/his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      285 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.10.55.50/chatllm/his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.10.55.50/chatllm/his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2492 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.10.55.50/chatllm/his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.127870 ChatLLM-2023.4.27.10.55.50/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.27.10.55.50/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.27.10.55.50/chatllm/parse_utils/doc_parse.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3413 2023-04-26 05:56:00.000000 ChatLLM-2023.4.27.10.55.50/chatllm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.129699 ChatLLM-2023.4.27.10.55.50/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.132745 ChatLLM-2023.4.27.10.55.50/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.137017 ChatLLM-2023.4.27.10.55.50/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.27.10.55.50/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.27.10.55.50/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.27.10.55.50/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.27.10.55.50/data/imgs/chatpdf_ann_df.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.143759 ChatLLM-2023.4.27.10.55.50/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.27.10.55.50/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.27.10.55.50/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.10.55.50/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.10.55.50/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.10.55.50/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.27.10.55.50/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.10.55.50/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.158354 ChatLLM-2023.4.27.10.55.50/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.10.55.50/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     3260 2023-04-26 08:57:26.000000 ChatLLM-2023.4.27.10.55.50/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.27.10.55.50/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      254 2023-04-26 12:45:59.000000 ChatLLM-2023.4.27.10.55.50/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.27.10.55.50/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.27.10.55.50/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-27 02:55:51.159147 ChatLLM-2023.4.27.10.55.50/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.10.55.50/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.158665 ChatLLM-2023.4.27.10.55.50/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/tox.ini
```

### Comparing `ChatLLM-2023.4.26.9.50.3/.gitignore` & `ChatLLM-2023.4.27.10.55.50/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/.travis.yml` & `ChatLLM-2023.4.27.10.55.50/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/CONTRIBUTING.rst` & `ChatLLM-2023.4.27.10.55.50/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 .travis.yml
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 Makefile
+README.bak.md
 README.md
-README.rst
-TODO.md
 git_init.sh
 pypi.sh
 requirements.txt
 requirements_pdf.txt
 setup.py
 tox.ini
 ChatLLM.egg-info/PKG-INFO
@@ -31,14 +30,15 @@
 chatllm/applications/chatann.py
 chatllm/applications/chatbase.py
 chatllm/applications/chatcrawler.py
 chatllm/applications/chatdoc.py
 chatllm/applications/chatpdf.py
 chatllm/applications/chatsearch.py
 chatllm/applications/chatweb.py
+chatllm/applications/chatwhoosh.py
 chatllm/applications/pipeline.py
 chatllm/clis/README.md
 chatllm/clis/__init__.py
 chatllm/clis/cli.py
 chatllm/his/FaissANN.py
 chatllm/his/__init__.py
 chatllm/his/_chatllm.py
@@ -52,16 +52,21 @@
 chatllm/webui/nice_ui.py
 chatllm/webui/run.sh
 data/姚明.txt
 data/王治郅.txt
 data/科比.txt
 data/财报.pdf
 data/马保国.txt
+data/imgs/LLM.drawio.png
+data/imgs/LLM.png
+data/imgs/chatpdf.gif
+data/imgs/chatpdf_ann_df.png
 data/医/500种中药现代研究.txt
 data/医/古今医统大全.txt
+docs/INSTALL.md
 docs/Makefile
 docs/README.md
 docs/_config.yml
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
```

### Comparing `ChatLLM-2023.4.26.9.50.3/LICENSE` & `ChatLLM-2023.4.27.10.55.50/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/Makefile` & `ChatLLM-2023.4.27.10.55.50/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 from meutils.decorators import clear_cuda_cache
 
 from chatllm.utils import DEVICE, load_llm4chat
 
 
 class ChatBase(object):
 
-    def __init__(self, chat_func=None, prompt_template=None, role='你扮演的角色是ChatLLM项目助理，由Betterme开发'):
+    def __init__(self, chat_func=None, prompt_template=None, role='你扮演的角色是ChatLLM项目助理，由Betterme二次开发'):
         self.chat_func = chat_func
         self.prompt_template = prompt_template if prompt_template else self.default_document_prompt
         self.role = role
 
         #
         self.history = []
         self.knowledge_base = None
 
     def __call__(self, **kwargs):
         return self.qa(**kwargs)
 
-    def qa(self, query, knowledge_base='', **kwargs):
+    def qa(self, query, knowledge_base='请自由回答', **kwargs):
         """可重写"""
         return self._qa(query, knowledge_base, **kwargs)
 
     def set_chat_kwargs(self, **kwargs):
         self.chat_func = partial(self.chat_func, **kwargs)
 
     @clear_cuda_cache
```

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/embedding.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/embedding.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 from sentence_transformers import SentenceTransformer
 from meutils.docarray_ import Document, DocumentArray
 
 
 # 增加 docarray v2
 # 增加 ann后端
 class SentenceEmbedding(object):
-    def __init__(self, model_name_or_path="shibing624/text2vec-base-chinese", device=None):
+    def __init__(self, model_name_or_path="shibing624/text2vec-base-chinese", **st_kwargs):
         """
-            disk_cache()(DocEmbedding().encode)
+            disk_cache()(SentenceEmbedding().encode)
         :param model_name_or_path:
         :param device:
         """
-        self.st = SentenceTransformer(model_name_or_path, device)
+        self.st = SentenceTransformer(model_name_or_path, **st_kwargs)
 
     def __call__(self, *args, **kwargs):
         return self.encode(*args, **kwargs)
 
     def encode(self, sentences, batch_size=32, show_progress_bar=False, normalize_embeddings=False,
                return_document=False):
```

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/his/FaissANN.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/his/_chatllm.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/his/_qa.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/utils.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 DEVICE = (
     os.environ['DEVICE']
     if 'DEVICE' in os.environ else "cuda"
     if torch.cuda.is_available() else "mps"
     if torch.backends.mps.is_available() else "cpu"
 )
 
+# todo 多卡 https://github.com/THUDM/ChatGLM-6B#%E5%A4%9A%E5%8D%A1%E9%83%A8%E7%BD%B2
 
 def textsplitter(text, chunk_size=512, overlap_rate=0.2, sep=''):  # 简单粗暴
     return text.lower().split() | xjoin(sep) | xgroup(chunk_size, overlap_rate)
 
 
 def load_llm4chat(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, stream=True, **kwargs):
     model, tokenizer = load_llm(model_name_or_path, device, **kwargs)
```

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.27.10.55.50/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.27.10.55.50/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/data/医/古今医统大全.txt` & `ChatLLM-2023.4.27.10.55.50/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/data/姚明.txt` & `ChatLLM-2023.4.27.10.55.50/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/data/王治郅.txt` & `ChatLLM-2023.4.27.10.55.50/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/data/科比.txt` & `ChatLLM-2023.4.27.10.55.50/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/data/财报.pdf` & `ChatLLM-2023.4.27.10.55.50/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/docs/Makefile` & `ChatLLM-2023.4.27.10.55.50/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/docs/conf.py` & `ChatLLM-2023.4.27.10.55.50/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/docs/img.png` & `ChatLLM-2023.4.27.10.55.50/docs/img.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/docs/installation.rst` & `ChatLLM-2023.4.27.10.55.50/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/docs/make.bat` & `ChatLLM-2023.4.27.10.55.50/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.50.3/setup.py` & `ChatLLM-2023.4.27.10.55.50/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 
 """The setup script."""
 import time
 from setuptools import setup, find_packages
-# from llm4chat import __version__
 
 version = time.strftime("%Y.%m.%d.%H.%M.%S", time.localtime())
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
@@ -15,41 +14,41 @@
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().split('\n')
 
 setup(
     author="yuanjie",
     author_email='313303303@qq.com',
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     description="Create a Python package.",
     entry_points={
         'console_scripts': [
-            'llm4gpt=llm4gpt.clis.cli:cli'
+            'chatllm-run=chatllm.clis.cli:cli'
         ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords='chatllm',
     name='ChatLLM',
     # name='ChatSearch', # 抢占包
 
-    packages=find_packages(include=['chatllm', 'llm.*']),
+    packages=find_packages(include=['chatllm', 'chatllm.*']),
 
     test_suite='tests',
-    url='https://github.com/yuanjie-ai/llm4gpt',
+    url='https://github.com/yuanjie-ai/ChatLLM',
     version=version, # '0.0.0',
     zip_safe=False,
 )
```

### Comparing `ChatLLM-2023.4.26.9.50.3/tests/test_llm4gpt.py` & `ChatLLM-2023.4.27.10.55.50/tests/test_llm4gpt.py`

 * *Files identical despite different names*


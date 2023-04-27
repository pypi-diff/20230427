# Comparing `tmp/ChatLLM-2023.4.27.10.55.50.tar.gz` & `tmp/ChatLLM-2023.4.27.13.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.27.10.55.50.tar", last modified: Thu Apr 27 02:55:51 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.27.13.0.53.tar", last modified: Thu Apr 27 05:00:53 2023, max compression
```

## Comparing `ChatLLM-2023.4.27.10.55.50.tar` & `ChatLLM-2023.4.27.13.0.53.tar`

### file list

```diff
@@ -1,95 +1,99 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.159094 ChatLLM-2023.4.27.10.55.50/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.27.10.55.50/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.122110 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     4130 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1744 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-27 02:55:51.000000 ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4130 2023-04-27 02:55:51.158928 ChatLLM-2023.4.27.10.55.50/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.10.55.50/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     3313 2023-04-27 02:50:29.000000 ChatLLM-2023.4.27.10.55.50/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.122727 ChatLLM-2023.4.27.10.55.50/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.125426 ChatLLM-2023.4.27.10.55.50/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 02:55:16.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3328 2023-04-27 02:46:24.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1335 2023-04-27 02:53:02.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1879 2023-04-26 12:42:49.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.27.10.55.50/chatllm/applications/pipeline.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.126104 ChatLLM-2023.4.27.10.55.50/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.10.55.50/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.27.10.55.50/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.127254 ChatLLM-2023.4.27.10.55.50/chatllm/his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.27.10.55.50/chatllm/his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      285 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.10.55.50/chatllm/his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.10.55.50/chatllm/his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2492 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.10.55.50/chatllm/his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.127870 ChatLLM-2023.4.27.10.55.50/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.27.10.55.50/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.27.10.55.50/chatllm/parse_utils/doc_parse.py
--rw-r--r--   0 betterme   (501) staff       (20)     3413 2023-04-26 05:56:00.000000 ChatLLM-2023.4.27.10.55.50/chatllm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.129699 ChatLLM-2023.4.27.10.55.50/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.27.10.55.50/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.132745 ChatLLM-2023.4.27.10.55.50/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.137017 ChatLLM-2023.4.27.10.55.50/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.27.10.55.50/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.27.10.55.50/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.27.10.55.50/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.27.10.55.50/data/imgs/chatpdf_ann_df.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.143759 ChatLLM-2023.4.27.10.55.50/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.27.10.55.50/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.27.10.55.50/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.10.55.50/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.10.55.50/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.10.55.50/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.27.10.55.50/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.10.55.50/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.158354 ChatLLM-2023.4.27.10.55.50/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.10.55.50/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     3260 2023-04-26 08:57:26.000000 ChatLLM-2023.4.27.10.55.50/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.27.10.55.50/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      254 2023-04-26 12:45:59.000000 ChatLLM-2023.4.27.10.55.50/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.27.10.55.50/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.27.10.55.50/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-27 02:55:51.159147 ChatLLM-2023.4.27.10.55.50/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.10.55.50/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:55:51.158665 ChatLLM-2023.4.27.10.55.50/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.10.55.50/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.912993 ChatLLM-2023.4.27.13.0.53/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.27.13.0.53/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.875247 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     4148 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1899 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4148 2023-04-27 05:00:53.912790 ChatLLM-2023.4.27.13.0.53/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.13.0.53/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     3332 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.13.0.53/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.875792 ChatLLM-2023.4.27.13.0.53/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.878412 ChatLLM-2023.4.27.13.0.53/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3356 2023-04-27 05:00:51.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/pipeline.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.879084 ChatLLM-2023.4.27.13.0.53/chatllm/applications/whoosh_index/
+-rwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:57:33.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/whoosh_index/MAIN_WRITELOCK
+-rw-r--r--   0 betterme   (501) staff       (20)     4784 2023-04-27 02:58:02.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/whoosh_index/MAIN_h83t1id481a6v0bp.seg
+-rw-r--r--   0 betterme   (501) staff       (20)     1716 2023-04-27 02:58:02.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/whoosh_index/_MAIN_1.toc
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.879578 ChatLLM-2023.4.27.13.0.53/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.13.0.53/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.27.13.0.53/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.880678 ChatLLM-2023.4.27.13.0.53/chatllm/his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.27.13.0.53/chatllm/his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      285 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.0.53/chatllm/his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.0.53/chatllm/his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2492 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.0.53/chatllm/his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.881246 ChatLLM-2023.4.27.13.0.53/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.27.13.0.53/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.27.13.0.53/chatllm/parse_utils/doc_parse.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3533 2023-04-27 04:23:17.000000 ChatLLM-2023.4.27.13.0.53/chatllm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.883046 ChatLLM-2023.4.27.13.0.53/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.886890 ChatLLM-2023.4.27.13.0.53/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.891184 ChatLLM-2023.4.27.13.0.53/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.27.13.0.53/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.27.13.0.53/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.27.13.0.53/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.27.13.0.53/data/imgs/chatpdf_ann_df.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.898537 ChatLLM-2023.4.27.13.0.53/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.27.13.0.53/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.27.13.0.53/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.0.53/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.0.53/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.0.53/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.27.13.0.53/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.0.53/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.912090 ChatLLM-2023.4.27.13.0.53/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.13.0.53/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     3260 2023-04-26 08:57:26.000000 ChatLLM-2023.4.27.13.0.53/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.27.13.0.53/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.13.0.53/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.27.13.0.53/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.27.13.0.53/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-27 05:00:53.913056 ChatLLM-2023.4.27.13.0.53/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.13.0.53/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.912471 ChatLLM-2023.4.27.13.0.53/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/tox.ini
```

### Comparing `ChatLLM-2023.4.27.10.55.50/.gitignore` & `ChatLLM-2023.4.27.13.0.53/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/.travis.yml` & `ChatLLM-2023.4.27.13.0.53/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/CONTRIBUTING.rst` & `ChatLLM-2023.4.27.13.0.53/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.27.10.55.50
+Version: 2023.4.27.13.0.53
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -54,15 +54,15 @@
   <summary>Click to ChatPDF</summary>
 
 ```python
 from chatllm.applications.chatpdf import ChatPDF
 
 qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
-qa.create_index('财报.pdf')
+qa.create_index('财报.pdf')  # 构建知识库
 
 for i, _ in qa(query='东北证券主营业务'):
     pass
 # 根据已知信息，东北证券的主营业务为证券业务。公司作为证券公司，主要从事证券经纪、证券投资咨询、与证券交易、
 # 证券投资活动有关的财务顾问、证券承销与保荐、证券自营、融资融券、证券投资基金代销和代销金融产品待业务。
 ```
 一键启动 webui `chatllm-run webui --name chatpdf`
```

### Comparing `ChatLLM-2023.4.27.10.55.50/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 chatllm/applications/chatcrawler.py
 chatllm/applications/chatdoc.py
 chatllm/applications/chatpdf.py
 chatllm/applications/chatsearch.py
 chatllm/applications/chatweb.py
 chatllm/applications/chatwhoosh.py
 chatllm/applications/pipeline.py
+chatllm/applications/whoosh_index/MAIN_WRITELOCK
+chatllm/applications/whoosh_index/MAIN_h83t1id481a6v0bp.seg
+chatllm/applications/whoosh_index/_MAIN_1.toc
 chatllm/clis/README.md
 chatllm/clis/__init__.py
 chatllm/clis/cli.py
 chatllm/his/FaissANN.py
 chatllm/his/__init__.py
 chatllm/his/_chatllm.py
 chatllm/his/_qa.py
```

### Comparing `ChatLLM-2023.4.27.10.55.50/LICENSE` & `ChatLLM-2023.4.27.13.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/Makefile` & `ChatLLM-2023.4.27.13.0.53/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/PKG-INFO` & `ChatLLM-2023.4.27.13.0.53/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.27.10.55.50
+Version: 2023.4.27.13.0.53
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -54,15 +54,15 @@
   <summary>Click to ChatPDF</summary>
 
 ```python
 from chatllm.applications.chatpdf import ChatPDF
 
 qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
-qa.create_index('财报.pdf')
+qa.create_index('财报.pdf')  # 构建知识库
 
 for i, _ in qa(query='东北证券主营业务'):
     pass
 # 根据已知信息，东北证券的主营业务为证券业务。公司作为证券公司，主要从事证券经纪、证券投资咨询、与证券交易、
 # 证券投资活动有关的财务顾问、证券承销与保荐、证券自营、融资融券、证券投资基金代销和代销金融产品待业务。
 ```
 一键启动 webui `chatllm-run webui --name chatpdf`
```

### Comparing `ChatLLM-2023.4.27.10.55.50/README.md` & `ChatLLM-2023.4.27.13.0.53/docs/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,14 @@
   <summary>Click to ChatPDF</summary>
 
 ```python
 from chatllm.applications.chatpdf import ChatPDF
 
 qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
-qa.create_index('财报.pdf')
 
 for i, _ in qa(query='东北证券主营业务'):
     pass
 # 根据已知信息，东北证券的主营业务为证券业务。公司作为证券公司，主要从事证券经纪、证券投资咨询、与证券交易、
 # 证券投资活动有关的财务顾问、证券承销与保荐、证券自营、融资融券、证券投资基金代销和代销金融产品待业务。
 ```
 一键启动 webui `chatllm-run webui --name chatpdf`
@@ -86,16 +85,14 @@
   <summary>Click to TODO</summary>
 
 - [x] 增加一键启动 webui
   - `chatllm-run webui --name chatpdf`
 
 - [x] 增加ChatPDF
 
-- [x] 增加ChatWoosh
-
 - [x] 增加本地知识库组件
 
 - [ ] 增加互联网搜索组件
 
 - [ ] 增加知识图谱组件
 
 - [ ] 增加微调模块
```

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatann.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatann.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         # 召回结果df
         self.recall = pd.DataFrame({'id': [], 'text': [], 'score': []})
 
     def qa(self, query, topk=3, threshold=0.66, **kwargs):
         df = self.find(query, topk, threshold)
         if len(df) == 0:
             logger.warning('召回内容为空!!!')
-        knowledge_base = '\n'.join(df.text)
 
+        knowledge_base = '\n'.join(df.text)
         return self._qa(query, knowledge_base, **kwargs)
 
     def find(self, query, topk=5, threshold=0.66):  # 返回df
         v = self.encode(query)  # np
 
         if self.backend == 'in_memory':
             r = self.index.find(TorchTensor(v), topk)
```

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from meutils.decorators import clear_cuda_cache
 
 from chatllm.utils import DEVICE, load_llm4chat
 
 
 class ChatBase(object):
 
-    def __init__(self, chat_func=None, prompt_template=None, role='你扮演的角色是ChatLLM项目助理，由Betterme二次开发'):
+    def __init__(self, chat_func=None, prompt_template=None,
+                 role='你扮演的角色是ChatLLM智能机器人🤖，由Betterme二次开发'):
         self.chat_func = chat_func
         self.prompt_template = prompt_template if prompt_template else self.default_document_prompt
         self.role = role
 
         #
         self.history = []
         self.knowledge_base = None
@@ -32,19 +33,18 @@
         """可重写"""
         return self._qa(query, knowledge_base, **kwargs)
 
     def set_chat_kwargs(self, **kwargs):
         self.chat_func = partial(self.chat_func, **kwargs)
 
     @clear_cuda_cache
-    def _qa(self, query, knowledge_base='请自由回答', max_turns=1):
+    def _qa(self, query, knowledge_base='', max_turns=1):
+        self.knowledge_base = knowledge_base if knowledge_base.strip() else '请自由回答'
 
-        if knowledge_base:
-            self.knowledge_base = knowledge_base
-            query = self.prompt_template.format(context=knowledge_base, question=query, role=self.role)
+        query = self.prompt_template.format(context=self.knowledge_base, question=query, role=self.role)
 
         _history = self.history[-(max_turns - 1):] if max_turns > 1 else []
         result = self.chat_func(query=query, history=_history)
 
         if isinstance(result, types.GeneratorType):
             return self._stream(result)
         else:  # list(self._stream(result)) 想办法合并
```

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatpdf.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatpdf.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,30 +16,31 @@
 
 
 class ChatPDF(ChatANN):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
-    def create_index(self, file, textsplitter=textsplitter):  # todo 多篇 增加parser
-        texts = extract_text(file)
+    def create_index(self, file_or_text, textsplitter=textsplitter):  # todo 多篇 增加 parser loader
+
+        texts = extract_text(file_or_text)
         texts = textsplitter(texts)
         return super().create_index(texts)
 
 
 if __name__ == '__main__':
     # filename = '../../data/财报.pdf'
     # bytes_array = Path(filename).read_bytes()
     # texts = extract_text(bytes_array)
     # texts = textsplitter(texts)
     # print(texts)
     from chatllm.applications.chatpdf import ChatPDF
 
     qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')  # 自动建索引
-    qa.load_llm4chat(model_name_or_path='/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm')
+    qa.load_llm4chat(model_name_or_path='/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm', device='cpu')
     qa.create_index('../../data/财报.pdf')
 
     for i, _ in qa(query='东北证券主营业务', topk=1, threshold=0.8):
         pass
 
     # 召回结果
-    print(qa._df)
+    print(qa.recall)
```

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatwhoosh.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 
 class ChatWhoosh(ChatBase, EasySearch):
 
     def __init__(self, indexdir='whoosh_index', indexname='MAIN', **kwargs):
         ChatBase.__init__(self, **kwargs)
         EasySearch.__init__(self, indexdir, indexname)
-        self._df = pd.DataFrame({'id': [], 'text': [], 'score': []})
+        self.recall = pd.DataFrame({'id': [], 'text': [], 'score': []})
 
     def qa(self, query, topk=3, threshold=0.66, **kwargs):
         df = self.find(query, topk, threshold)
         if len(df) == 0:
             logger.warning('召回内容为空!!!')
         knowledge_base = '\n'.join(df.text)
 
         return self._qa(query, knowledge_base, **kwargs)
 
     def find(self, query, topk=3, threshold=0.66, **kwargs):
         df = super().find(defaultfield='text', querystring=query, limit=topk, **kwargs)
         if len(df):
-            self._df = df.query(f'score > {threshold}')
-        return self._df
+            self.recall = df.query(f'score > {threshold}')
+        return self.recall
 
     def create_index(self, texts, id_mapping=md5, **kwargs):
         ids = map(id_mapping, texts)
         df = pd.DataFrame({'id': ids, 'text': texts})
         schema = Schema(
             id=ID(stored=True),
             text=TEXT(stored=True, analyzer=ChineseAnalyzer(cachesize=-1))  # 无界缓存加速
@@ -51,8 +51,8 @@
 
 
 if __name__ == '__main__':
     from chatllm.applications.chatwhoosh import ChatWhoosh
 
     cw = ChatWhoosh(indexdir='whoosh_index')
     cw.create_index(texts=['周杰伦'] * 10)
-    cw.find('周杰伦')
+    print(cw.find('周杰伦'))
```

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/clis/cli.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/embedding.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/his/FaissANN.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/his/_chatllm.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/his/_qa.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/utils.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 DEVICE = (
     os.environ['DEVICE']
     if 'DEVICE' in os.environ else "cuda"
     if torch.cuda.is_available() else "mps"
     if torch.backends.mps.is_available() else "cpu"
 )
 
+
 # todo 多卡 https://github.com/THUDM/ChatGLM-6B#%E5%A4%9A%E5%8D%A1%E9%83%A8%E7%BD%B2
 
 def textsplitter(text, chunk_size=512, overlap_rate=0.2, sep=''):  # 简单粗暴
     return text.lower().split() | xjoin(sep) | xgroup(chunk_size, overlap_rate)
 
 
 def load_llm4chat(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, stream=True, **kwargs):
     model, tokenizer = load_llm(model_name_or_path, device, **kwargs)
-    if stream:
+    if stream and hasattr(model, 'stream_chat'):
         return partial(model.stream_chat, tokenizer=tokenizer)
     else:
         return partial(model.chat, tokenizer=tokenizer)
 
 
 def load_llm(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, device_map: Optional[Dict[str, int]] = None,
              **kwargs):
@@ -39,14 +40,16 @@
     model = AutoModel.from_pretrained(model_name_or_path, trust_remote_code=True, **kwargs)
 
     if torch.cuda.is_available() and device.lower().startswith("cuda"):
         # 根据当前设备GPU数量决定是否进行多卡部署
         num_gpus = torch.cuda.device_count()
         if num_gpus < 2 and device_map is None:
             model = model.half().cuda()
+            # model.transformer.prefix_encoder.float()
+
         else:
             from accelerate import dispatch_model
             # 可传入device_map自定义每张卡的部署情况
             if device_map is None:
                 device_map = auto_configure_device_map(num_gpus)
 
             model = dispatch_model(model, device_map=device_map).half().cuda()
@@ -84,8 +87,8 @@
         device_map[f'transformer.layers.{i}'] = gpu_target
         used += 1
 
     return device_map
 
 
 if __name__ == '__main__':
-    a = llm_load("/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
+    model, tokenizer = load_llm("/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm", device='cpu')
```

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/webui/chatpdf.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.27.13.0.53/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/data/imgs/LLM.drawio.png` & `ChatLLM-2023.4.27.13.0.53/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/data/imgs/LLM.png` & `ChatLLM-2023.4.27.13.0.53/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/data/imgs/chatpdf.gif` & `ChatLLM-2023.4.27.13.0.53/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.4.27.13.0.53/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.27.13.0.53/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/data/医/古今医统大全.txt` & `ChatLLM-2023.4.27.13.0.53/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/data/姚明.txt` & `ChatLLM-2023.4.27.13.0.53/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/data/王治郅.txt` & `ChatLLM-2023.4.27.13.0.53/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/data/科比.txt` & `ChatLLM-2023.4.27.13.0.53/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/data/财报.pdf` & `ChatLLM-2023.4.27.13.0.53/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/docs/INSTALL.md` & `ChatLLM-2023.4.27.13.0.53/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/docs/Makefile` & `ChatLLM-2023.4.27.13.0.53/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/docs/README.md` & `ChatLLM-2023.4.27.13.0.53/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,15 @@
   <summary>Click to ChatPDF</summary>
 
 ```python
 from chatllm.applications.chatpdf import ChatPDF
 
 qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
+qa.create_index('财报.pdf')  # 构建知识库
 
 for i, _ in qa(query='东北证券主营业务'):
     pass
 # 根据已知信息，东北证券的主营业务为证券业务。公司作为证券公司，主要从事证券经纪、证券投资咨询、与证券交易、
 # 证券投资活动有关的财务顾问、证券承销与保荐、证券自营、融资融券、证券投资基金代销和代销金融产品待业务。
 ```
 一键启动 webui `chatllm-run webui --name chatpdf`
@@ -85,14 +86,16 @@
   <summary>Click to TODO</summary>
 
 - [x] 增加一键启动 webui
   - `chatllm-run webui --name chatpdf`
 
 - [x] 增加ChatPDF
 
+- [x] 增加ChatWoosh
+
 - [x] 增加本地知识库组件
 
 - [ ] 增加互联网搜索组件
 
 - [ ] 增加知识图谱组件
 
 - [ ] 增加微调模块
```

### Comparing `ChatLLM-2023.4.27.10.55.50/docs/conf.py` & `ChatLLM-2023.4.27.13.0.53/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/docs/img.png` & `ChatLLM-2023.4.27.13.0.53/docs/img.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/docs/installation.rst` & `ChatLLM-2023.4.27.13.0.53/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/docs/make.bat` & `ChatLLM-2023.4.27.13.0.53/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/setup.py` & `ChatLLM-2023.4.27.13.0.53/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.10.55.50/tests/test_llm4gpt.py` & `ChatLLM-2023.4.27.13.0.53/tests/test_llm4gpt.py`

 * *Files identical despite different names*


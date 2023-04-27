# Comparing `tmp/ChatLLM-2023.4.27.18.17.54.tar.gz` & `tmp/ChatLLM-2023.4.27.18.6.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.27.18.17.54.tar", last modified: Thu Apr 27 10:17:55 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.27.18.6.56.tar", last modified: Thu Apr 27 10:06:57 2023, max compression
```

## Comparing `ChatLLM-2023.4.27.18.17.54.tar` & `ChatLLM-2023.4.27.18.6.56.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.163016 ChatLLM-2023.4.27.18.17.54/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.27.18.17.54/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.125082 ChatLLM-2023.4.27.18.17.54/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     4121 2023-04-27 10:17:55.000000 ChatLLM-2023.4.27.18.17.54/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1768 2023-04-27 10:17:55.000000 ChatLLM-2023.4.27.18.17.54/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 10:17:55.000000 ChatLLM-2023.4.27.18.17.54/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-27 10:17:55.000000 ChatLLM-2023.4.27.18.17.54/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 10:17:55.000000 ChatLLM-2023.4.27.18.17.54/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-27 10:17:55.000000 ChatLLM-2023.4.27.18.17.54/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-27 10:17:55.000000 ChatLLM-2023.4.27.18.17.54/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4121 2023-04-27 10:17:55.162838 ChatLLM-2023.4.27.18.17.54/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.18.17.54/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     3304 2023-04-27 06:03:48.000000 ChatLLM-2023.4.27.18.17.54/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.125963 ChatLLM-2023.4.27.18.17.54/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.126982 ChatLLM-2023.4.27.18.17.54/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.27.18.17.54/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.27.18.17.54/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.18.17.54/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.27.18.17.54/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.129689 ChatLLM-2023.4.27.18.17.54/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3413 2023-04-27 10:17:53.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.27.18.17.54/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.27.18.17.54/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.130297 ChatLLM-2023.4.27.18.17.54/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.18.17.54/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.27.18.17.54/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.130785 ChatLLM-2023.4.27.18.17.54/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.27.18.17.54/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.27.18.17.54/chatllm/parse_utils/doc_parse.py
--rw-r--r--   0 betterme   (501) staff       (20)     3533 2023-04-27 04:23:17.000000 ChatLLM-2023.4.27.18.17.54/chatllm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.132406 ChatLLM-2023.4.27.18.17.54/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.27.18.17.54/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.18.17.54/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.27.18.17.54/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.18.17.54/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.27.18.17.54/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.27.18.17.54/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.136346 ChatLLM-2023.4.27.18.17.54/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.142281 ChatLLM-2023.4.27.18.17.54/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.27.18.17.54/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.27.18.17.54/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.27.18.17.54/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.27.18.17.54/data/imgs/chatpdf_ann_df.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.146315 ChatLLM-2023.4.27.18.17.54/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.27.18.17.54/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.27.18.17.54/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.17.54/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.17.54/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.17.54/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.27.18.17.54/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.17.54/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.162158 ChatLLM-2023.4.27.18.17.54/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.18.17.54/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     3260 2023-04-26 08:57:26.000000 ChatLLM-2023.4.27.18.17.54/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.27.18.17.54/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.18.17.54/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.27.18.17.54/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.27.18.17.54/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-27 10:17:55.163066 ChatLLM-2023.4.27.18.17.54/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.18.17.54/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:17:55.162551 ChatLLM-2023.4.27.18.17.54/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.17.54/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:57.021376 ChatLLM-2023.4.27.18.6.56/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.27.18.6.56/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.984465 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     4120 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1768 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4120 2023-04-27 10:06:57.021227 ChatLLM-2023.4.27.18.6.56/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.18.6.56/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     3304 2023-04-27 06:03:48.000000 ChatLLM-2023.4.27.18.6.56/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.985271 ChatLLM-2023.4.27.18.6.56/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.985923 ChatLLM-2023.4.27.18.6.56/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.27.18.6.56/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.27.18.6.56/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.18.6.56/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.27.18.6.56/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.988523 ChatLLM-2023.4.27.18.6.56/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3400 2023-04-27 09:24:25.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.27.18.6.56/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.989082 ChatLLM-2023.4.27.18.6.56/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.18.6.56/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.27.18.6.56/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.989569 ChatLLM-2023.4.27.18.6.56/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.27.18.6.56/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.27.18.6.56/chatllm/parse_utils/doc_parse.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3533 2023-04-27 04:23:17.000000 ChatLLM-2023.4.27.18.6.56/chatllm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.991027 ChatLLM-2023.4.27.18.6.56/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.994925 ChatLLM-2023.4.27.18.6.56/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.998749 ChatLLM-2023.4.27.18.6.56/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.27.18.6.56/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.27.18.6.56/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.27.18.6.56/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.27.18.6.56/data/imgs/chatpdf_ann_df.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:57.005481 ChatLLM-2023.4.27.18.6.56/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.27.18.6.56/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.27.18.6.56/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.6.56/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.6.56/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.6.56/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.27.18.6.56/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.6.56/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:57.020622 ChatLLM-2023.4.27.18.6.56/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.18.6.56/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     3260 2023-04-26 08:57:26.000000 ChatLLM-2023.4.27.18.6.56/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.27.18.6.56/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.18.6.56/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.27.18.6.56/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.27.18.6.56/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-27 10:06:57.021421 ChatLLM-2023.4.27.18.6.56/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.18.6.56/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:57.020980 ChatLLM-2023.4.27.18.6.56/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/tox.ini
```

### Comparing `ChatLLM-2023.4.27.18.17.54/.gitignore` & `ChatLLM-2023.4.27.18.6.56/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/.travis.yml` & `ChatLLM-2023.4.27.18.6.56/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/CONTRIBUTING.rst` & `ChatLLM-2023.4.27.18.6.56/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.27.18.17.54
+Version: 2023.4.27.18.6.56
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.27.18.17.54/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/LICENSE` & `ChatLLM-2023.4.27.18.6.56/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/Makefile` & `ChatLLM-2023.4.27.18.6.56/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/PKG-INFO` & `ChatLLM-2023.4.27.18.6.56/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.27.18.17.54
+Version: 2023.4.27.18.6.56
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.27.18.17.54/README.md` & `ChatLLM-2023.4.27.18.6.56/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/_his/FaissANN.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/_his/_chatllm.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/_his/_qa.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatann.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,34 +14,33 @@
 from chatllm.utils import DEVICE, load_llm4chat
 
 
 class ChatBase(object):
 
     def __init__(self, chat_func=None, prompt_template=None, role=''):
         self.chat_func = chat_func
-        self.prompt_template = prompt_template or self.default_document_prompt
+        self.prompt_template = prompt_template if prompt_template else self.default_document_prompt
+        self.role = role or os.environ.get('LLM_ROLE', '')
 
         #
         self.history = []
         self.knowledge_base = None
-        self.role = None
 
     def __call__(self, **kwargs):
         return self.qa(**kwargs)
 
     def qa(self, query, knowledge_base='', **kwargs):
         """可重写"""
         return self._qa(query, knowledge_base, **kwargs)
 
     def set_chat_kwargs(self, **kwargs):
         self.chat_func = partial(self.chat_func, **kwargs)
 
     @clear_cuda_cache
-    def _qa(self, query, knowledge_base='', role='', max_turns=1):
-        self.role = role or os.environ.get('LLM_ROLE', '')
+    def _qa(self, query, knowledge_base='', max_turns=1):
         self.knowledge_base = knowledge_base if knowledge_base.strip() else '请自由回答'
 
         query = self.prompt_template.format(context=self.knowledge_base, question=query, role=self.role)
 
         _history = self.history[-(max_turns - 1):] if max_turns > 1 else []
         result = self.chat_func(query=query, history=_history)
```

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatpdf.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/chatyuan.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/clis/cli.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/embedding.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/utils.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/utils.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/webui/chatpdf.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/data/imgs/LLM.drawio.png` & `ChatLLM-2023.4.27.18.6.56/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/data/imgs/LLM.png` & `ChatLLM-2023.4.27.18.6.56/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/data/imgs/chatpdf.gif` & `ChatLLM-2023.4.27.18.6.56/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.4.27.18.6.56/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.27.18.6.56/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/data/医/古今医统大全.txt` & `ChatLLM-2023.4.27.18.6.56/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/data/姚明.txt` & `ChatLLM-2023.4.27.18.6.56/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/data/王治郅.txt` & `ChatLLM-2023.4.27.18.6.56/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/data/科比.txt` & `ChatLLM-2023.4.27.18.6.56/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/data/财报.pdf` & `ChatLLM-2023.4.27.18.6.56/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/docs/INSTALL.md` & `ChatLLM-2023.4.27.18.6.56/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/docs/Makefile` & `ChatLLM-2023.4.27.18.6.56/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/docs/README.md` & `ChatLLM-2023.4.27.18.6.56/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/docs/conf.py` & `ChatLLM-2023.4.27.18.6.56/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/docs/img.png` & `ChatLLM-2023.4.27.18.6.56/docs/img.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/docs/installation.rst` & `ChatLLM-2023.4.27.18.6.56/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/docs/make.bat` & `ChatLLM-2023.4.27.18.6.56/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/setup.py` & `ChatLLM-2023.4.27.18.6.56/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.17.54/tests/test_llm4gpt.py` & `ChatLLM-2023.4.27.18.6.56/tests/test_llm4gpt.py`

 * *Files identical despite different names*


# Comparing `tmp/ChatLLM-2023.4.27.13.20.47.tar.gz` & `tmp/ChatLLM-2023.4.27.18.6.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.27.13.20.47.tar", last modified: Thu Apr 27 05:20:47 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.27.18.6.56.tar", last modified: Thu Apr 27 10:06:57 2023, max compression
```

## Comparing `ChatLLM-2023.4.27.13.20.47.tar` & `ChatLLM-2023.4.27.18.6.56.tar`

### file list

```diff
@@ -1,99 +1,96 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.333242 ChatLLM-2023.4.27.13.20.47/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.27.13.20.47/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.293965 ChatLLM-2023.4.27.13.20.47/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     4149 2023-04-27 05:20:47.000000 ChatLLM-2023.4.27.13.20.47/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1899 2023-04-27 05:20:47.000000 ChatLLM-2023.4.27.13.20.47/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 05:20:47.000000 ChatLLM-2023.4.27.13.20.47/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-27 05:20:47.000000 ChatLLM-2023.4.27.13.20.47/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 05:20:47.000000 ChatLLM-2023.4.27.13.20.47/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-27 05:20:47.000000 ChatLLM-2023.4.27.13.20.47/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-27 05:20:47.000000 ChatLLM-2023.4.27.13.20.47/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4149 2023-04-27 05:20:47.333077 ChatLLM-2023.4.27.13.20.47/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.13.20.47/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     3332 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.13.20.47/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.294504 ChatLLM-2023.4.27.13.20.47/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.297124 ChatLLM-2023.4.27.13.20.47/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3331 2023-04-27 05:20:03.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/pipeline.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.297815 ChatLLM-2023.4.27.13.20.47/chatllm/applications/whoosh_index/
--rwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:57:33.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/whoosh_index/MAIN_WRITELOCK
--rw-r--r--   0 betterme   (501) staff       (20)     4784 2023-04-27 02:58:02.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/whoosh_index/MAIN_h83t1id481a6v0bp.seg
--rw-r--r--   0 betterme   (501) staff       (20)     1716 2023-04-27 02:58:02.000000 ChatLLM-2023.4.27.13.20.47/chatllm/applications/whoosh_index/_MAIN_1.toc
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.298488 ChatLLM-2023.4.27.13.20.47/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.13.20.47/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.27.13.20.47/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.299486 ChatLLM-2023.4.27.13.20.47/chatllm/his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.27.13.20.47/chatllm/his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      285 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.20.47/chatllm/his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.20.47/chatllm/his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2492 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.20.47/chatllm/his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.300042 ChatLLM-2023.4.27.13.20.47/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.27.13.20.47/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.27.13.20.47/chatllm/parse_utils/doc_parse.py
--rw-r--r--   0 betterme   (501) staff       (20)     3533 2023-04-27 04:23:17.000000 ChatLLM-2023.4.27.13.20.47/chatllm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.301926 ChatLLM-2023.4.27.13.20.47/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.27.13.20.47/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.20.47/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.27.13.20.47/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.20.47/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.27.13.20.47/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.27.13.20.47/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.305847 ChatLLM-2023.4.27.13.20.47/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.312950 ChatLLM-2023.4.27.13.20.47/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.27.13.20.47/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.27.13.20.47/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.27.13.20.47/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.27.13.20.47/data/imgs/chatpdf_ann_df.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.316855 ChatLLM-2023.4.27.13.20.47/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.27.13.20.47/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.27.13.20.47/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.20.47/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.20.47/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.20.47/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.27.13.20.47/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.20.47/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.332430 ChatLLM-2023.4.27.13.20.47/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.13.20.47/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     3260 2023-04-26 08:57:26.000000 ChatLLM-2023.4.27.13.20.47/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.27.13.20.47/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.13.20.47/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.27.13.20.47/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.27.13.20.47/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-27 05:20:47.333298 ChatLLM-2023.4.27.13.20.47/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.13.20.47/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:20:47.332783 ChatLLM-2023.4.27.13.20.47/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.20.47/tox.ini
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

### Comparing `ChatLLM-2023.4.27.13.20.47/.gitignore` & `ChatLLM-2023.4.27.18.6.56/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/.travis.yml` & `ChatLLM-2023.4.27.18.6.56/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/CONTRIBUTING.rst` & `ChatLLM-2023.4.27.18.6.56/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.27.13.20.47
+Version: 2023.4.27.18.6.56
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -40,32 +40,30 @@
 
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
 
-for i, _ in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
-    pass
+_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'))
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
 
 <details markdown="1">
   <summary>Click to ChatPDF</summary>
 
 ```python
 from chatllm.applications.chatpdf import ChatPDF
 
 qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
 qa.create_index('财报.pdf')  # 构建知识库
 
-for i, _ in qa(query='东北证券主营业务'):
-    pass
+list(qa(query='东北证券主营业务'))
 # 根据已知信息，东北证券的主营业务为证券业务。公司作为证券公司，主要从事证券经纪、证券投资咨询、与证券交易、
 # 证券投资活动有关的财务顾问、证券承销与保荐、证券自营、融资融券、证券投资基金代销和代销金融产品待业务。
 ```
 一键启动 webui `chatllm-run webui --name chatpdf`
 
 ![向量召回结果](data/imgs/chatpdf.gif)
```

### Comparing `ChatLLM-2023.4.27.13.20.47/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,37 +19,35 @@
 ChatLLM.egg-info/SOURCES.txt
 ChatLLM.egg-info/dependency_links.txt
 ChatLLM.egg-info/entry_points.txt
 ChatLLM.egg-info/not-zip-safe
 ChatLLM.egg-info/requires.txt
 ChatLLM.egg-info/top_level.txt
 chatllm/__init__.py
+chatllm/chatyuan.py
 chatllm/embedding.py
 chatllm/utils.py
+chatllm/_his/FaissANN.py
+chatllm/_his/__init__.py
+chatllm/_his/_chatllm.py
+chatllm/_his/_qa.py
 chatllm/applications/Question2Answer.py
 chatllm/applications/__init__.py
 chatllm/applications/chatann.py
 chatllm/applications/chatbase.py
 chatllm/applications/chatcrawler.py
 chatllm/applications/chatdoc.py
 chatllm/applications/chatpdf.py
 chatllm/applications/chatsearch.py
 chatllm/applications/chatweb.py
 chatllm/applications/chatwhoosh.py
 chatllm/applications/pipeline.py
-chatllm/applications/whoosh_index/MAIN_WRITELOCK
-chatllm/applications/whoosh_index/MAIN_h83t1id481a6v0bp.seg
-chatllm/applications/whoosh_index/_MAIN_1.toc
 chatllm/clis/README.md
 chatllm/clis/__init__.py
 chatllm/clis/cli.py
-chatllm/his/FaissANN.py
-chatllm/his/__init__.py
-chatllm/his/_chatllm.py
-chatllm/his/_qa.py
 chatllm/parse_utils/__init__.py
 chatllm/parse_utils/doc_parse.py
 chatllm/webui/__init__.py
 chatllm/webui/chatbase.py
 chatllm/webui/chatpdf.py
 chatllm/webui/gradio_ui.py
 chatllm/webui/nice_ui.py
```

### Comparing `ChatLLM-2023.4.27.13.20.47/LICENSE` & `ChatLLM-2023.4.27.18.6.56/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/Makefile` & `ChatLLM-2023.4.27.18.6.56/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/PKG-INFO` & `ChatLLM-2023.4.27.18.6.56/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.27.13.20.47
+Version: 2023.4.27.18.6.56
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -40,32 +40,30 @@
 
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
 
-for i, _ in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
-    pass
+_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'))
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
 
 <details markdown="1">
   <summary>Click to ChatPDF</summary>
 
 ```python
 from chatllm.applications.chatpdf import ChatPDF
 
 qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
 qa.create_index('财报.pdf')  # 构建知识库
 
-for i, _ in qa(query='东北证券主营业务'):
-    pass
+list(qa(query='东北证券主营业务'))
 # 根据已知信息，东北证券的主营业务为证券业务。公司作为证券公司，主要从事证券经纪、证券投资咨询、与证券交易、
 # 证券投资活动有关的财务顾问、证券承销与保荐、证券自营、融资融券、证券投资基金代销和代销金融产品待业务。
 ```
 一键启动 webui `chatllm-run webui --name chatpdf`
 
 ![向量召回结果](data/imgs/chatpdf.gif)
```

### Comparing `ChatLLM-2023.4.27.13.20.47/README.md` & `ChatLLM-2023.4.27.18.6.56/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,32 +18,30 @@
 
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
 
-for i, _ in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
-    pass
+_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'))
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
 
 <details markdown="1">
   <summary>Click to ChatPDF</summary>
 
 ```python
 from chatllm.applications.chatpdf import ChatPDF
 
 qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
 qa.create_index('财报.pdf')  # 构建知识库
 
-for i, _ in qa(query='东北证券主营业务'):
-    pass
+list(qa(query='东北证券主营业务'))
 # 根据已知信息，东北证券的主营业务为证券业务。公司作为证券公司，主要从事证券经纪、证券投资咨询、与证券交易、
 # 证券投资活动有关的财务顾问、证券承销与保荐、证券自营、融资融券、证券投资基金代销和代销金融产品待业务。
 ```
 一键启动 webui `chatllm-run webui --name chatpdf`
 
 ![向量召回结果](data/imgs/chatpdf.gif)
```

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatann.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 from meutils.decorators import clear_cuda_cache
 
 from chatllm.utils import DEVICE, load_llm4chat
 
 
 class ChatBase(object):
 
-    def __init__(self, chat_func=None, prompt_template=None,
-                 role='你扮演的角色是ChatLLM智能助理，是由Betterme开发'):
+    def __init__(self, chat_func=None, prompt_template=None, role=''):
         self.chat_func = chat_func
         self.prompt_template = prompt_template if prompt_template else self.default_document_prompt
-        self.role = role
+        self.role = role or os.environ.get('LLM_ROLE', '')
 
         #
         self.history = []
         self.knowledge_base = None
 
     def __call__(self, **kwargs):
         return self.qa(**kwargs)
@@ -63,15 +62,16 @@
         self.history += [[None, response]]  # 置空知识
 
     def load_llm4chat(self, model_name_or_path="THUDM/chatglm-6b", device=DEVICE, stream=True, **kwargs):
         assert not self.chat_func, "overwrite chat_func"
         self.chat_func = load_llm4chat(model_name_or_path, device, stream, **kwargs)
 
     @property
-    def default_document_prompt(self):
+    def default_document_prompt(
+        self):  # 重写 chat函数会更好 prompt += "[Round {}]\n问：{}\n答：{}\n".format(i, old_query, response)
         prompt_template = """
             {role}
             基于以下已知信息，简洁和专业的来回答问题。
             如果无法从中得到答案，请说 "根据已知信息无法回答该问题" 或 "没有提供足够的信息"，不允许在答案中添加编造成分，答案请使用中文。
             已知信息: {context}
             问题: {question}
             """.strip()
```

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatpdf.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/clis/cli.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/embedding.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/his/FaissANN.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/his/_chatllm.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/his/_qa.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/_his/_qa.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @Description  :
 
 from langchain.chains import RetrievalQA
 from langchain.prompts.prompt import PromptTemplate
 from langchain.vectorstores import FAISS
 
 # ME
-from chatllm.his._chatllm import ChatLLM
+from chatllm._his._chatllm import ChatLLM
 
 RetrievalQA.return_source_documents = True
 
 
 class QA(object):
     def __init__(self, chatllm: ChatLLM, faiss_ann: FAISS = None, document_prompt: PromptTemplate = None):
         """
```

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/utils.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/utils.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/webui/chatpdf.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.27.18.6.56/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/data/imgs/LLM.drawio.png` & `ChatLLM-2023.4.27.18.6.56/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/data/imgs/LLM.png` & `ChatLLM-2023.4.27.18.6.56/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/data/imgs/chatpdf.gif` & `ChatLLM-2023.4.27.18.6.56/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.4.27.18.6.56/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.27.18.6.56/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/data/医/古今医统大全.txt` & `ChatLLM-2023.4.27.18.6.56/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/data/姚明.txt` & `ChatLLM-2023.4.27.18.6.56/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/data/王治郅.txt` & `ChatLLM-2023.4.27.18.6.56/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/data/科比.txt` & `ChatLLM-2023.4.27.18.6.56/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/data/财报.pdf` & `ChatLLM-2023.4.27.18.6.56/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/docs/INSTALL.md` & `ChatLLM-2023.4.27.18.6.56/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/docs/Makefile` & `ChatLLM-2023.4.27.18.6.56/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/docs/README.md` & `ChatLLM-2023.4.27.18.6.56/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/docs/conf.py` & `ChatLLM-2023.4.27.18.6.56/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/docs/img.png` & `ChatLLM-2023.4.27.18.6.56/docs/img.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/docs/installation.rst` & `ChatLLM-2023.4.27.18.6.56/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/docs/make.bat` & `ChatLLM-2023.4.27.18.6.56/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/setup.py` & `ChatLLM-2023.4.27.18.6.56/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.20.47/tests/test_llm4gpt.py` & `ChatLLM-2023.4.27.18.6.56/tests/test_llm4gpt.py`

 * *Files identical despite different names*


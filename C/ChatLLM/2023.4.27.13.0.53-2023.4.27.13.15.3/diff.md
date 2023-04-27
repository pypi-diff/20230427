# Comparing `tmp/ChatLLM-2023.4.27.13.0.53.tar.gz` & `tmp/ChatLLM-2023.4.27.13.15.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.27.13.0.53.tar", last modified: Thu Apr 27 05:00:53 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.27.13.15.3.tar", last modified: Thu Apr 27 05:15:03 2023, max compression
```

## Comparing `ChatLLM-2023.4.27.13.0.53.tar` & `ChatLLM-2023.4.27.13.15.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.912993 ChatLLM-2023.4.27.13.0.53/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.27.13.0.53/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.875247 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     4148 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1899 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-27 05:00:53.000000 ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4148 2023-04-27 05:00:53.912790 ChatLLM-2023.4.27.13.0.53/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.13.0.53/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     3332 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.13.0.53/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.875792 ChatLLM-2023.4.27.13.0.53/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.878412 ChatLLM-2023.4.27.13.0.53/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3356 2023-04-27 05:00:51.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/pipeline.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.879084 ChatLLM-2023.4.27.13.0.53/chatllm/applications/whoosh_index/
--rwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:57:33.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/whoosh_index/MAIN_WRITELOCK
--rw-r--r--   0 betterme   (501) staff       (20)     4784 2023-04-27 02:58:02.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/whoosh_index/MAIN_h83t1id481a6v0bp.seg
--rw-r--r--   0 betterme   (501) staff       (20)     1716 2023-04-27 02:58:02.000000 ChatLLM-2023.4.27.13.0.53/chatllm/applications/whoosh_index/_MAIN_1.toc
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.879578 ChatLLM-2023.4.27.13.0.53/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.13.0.53/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.27.13.0.53/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.880678 ChatLLM-2023.4.27.13.0.53/chatllm/his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.27.13.0.53/chatllm/his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      285 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.0.53/chatllm/his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.0.53/chatllm/his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2492 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.0.53/chatllm/his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.881246 ChatLLM-2023.4.27.13.0.53/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.27.13.0.53/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.27.13.0.53/chatllm/parse_utils/doc_parse.py
--rw-r--r--   0 betterme   (501) staff       (20)     3533 2023-04-27 04:23:17.000000 ChatLLM-2023.4.27.13.0.53/chatllm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.883046 ChatLLM-2023.4.27.13.0.53/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.27.13.0.53/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.886890 ChatLLM-2023.4.27.13.0.53/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.891184 ChatLLM-2023.4.27.13.0.53/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.27.13.0.53/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.27.13.0.53/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.27.13.0.53/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.27.13.0.53/data/imgs/chatpdf_ann_df.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.898537 ChatLLM-2023.4.27.13.0.53/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.27.13.0.53/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.27.13.0.53/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.0.53/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.0.53/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.0.53/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.27.13.0.53/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.0.53/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.912090 ChatLLM-2023.4.27.13.0.53/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.13.0.53/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     3260 2023-04-26 08:57:26.000000 ChatLLM-2023.4.27.13.0.53/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.27.13.0.53/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.13.0.53/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.27.13.0.53/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.27.13.0.53/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-27 05:00:53.913056 ChatLLM-2023.4.27.13.0.53/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.13.0.53/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:00:53.912471 ChatLLM-2023.4.27.13.0.53/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.0.53/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.557615 ChatLLM-2023.4.27.13.15.3/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.27.13.15.3/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.469156 ChatLLM-2023.4.27.13.15.3/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     4148 2023-04-27 05:15:03.000000 ChatLLM-2023.4.27.13.15.3/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1899 2023-04-27 05:15:03.000000 ChatLLM-2023.4.27.13.15.3/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 05:15:03.000000 ChatLLM-2023.4.27.13.15.3/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-27 05:15:03.000000 ChatLLM-2023.4.27.13.15.3/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 05:15:03.000000 ChatLLM-2023.4.27.13.15.3/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-27 05:15:03.000000 ChatLLM-2023.4.27.13.15.3/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-27 05:15:03.000000 ChatLLM-2023.4.27.13.15.3/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4148 2023-04-27 05:15:03.557459 ChatLLM-2023.4.27.13.15.3/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.13.15.3/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     3332 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.13.15.3/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.471200 ChatLLM-2023.4.27.13.15.3/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.522730 ChatLLM-2023.4.27.13.15.3/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3334 2023-04-27 05:11:18.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/pipeline.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.523473 ChatLLM-2023.4.27.13.15.3/chatllm/applications/whoosh_index/
+-rwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 02:57:33.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/whoosh_index/MAIN_WRITELOCK
+-rw-r--r--   0 betterme   (501) staff       (20)     4784 2023-04-27 02:58:02.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/whoosh_index/MAIN_h83t1id481a6v0bp.seg
+-rw-r--r--   0 betterme   (501) staff       (20)     1716 2023-04-27 02:58:02.000000 ChatLLM-2023.4.27.13.15.3/chatllm/applications/whoosh_index/_MAIN_1.toc
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.524189 ChatLLM-2023.4.27.13.15.3/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.13.15.3/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.27.13.15.3/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.525231 ChatLLM-2023.4.27.13.15.3/chatllm/his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.27.13.15.3/chatllm/his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      285 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.15.3/chatllm/his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.15.3/chatllm/his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2492 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.13.15.3/chatllm/his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.525792 ChatLLM-2023.4.27.13.15.3/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.27.13.15.3/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.27.13.15.3/chatllm/parse_utils/doc_parse.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3533 2023-04-27 04:23:17.000000 ChatLLM-2023.4.27.13.15.3/chatllm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.527301 ChatLLM-2023.4.27.13.15.3/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.27.13.15.3/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.15.3/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.27.13.15.3/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.13.15.3/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.27.13.15.3/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.27.13.15.3/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.531229 ChatLLM-2023.4.27.13.15.3/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.535148 ChatLLM-2023.4.27.13.15.3/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.27.13.15.3/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.27.13.15.3/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.27.13.15.3/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.27.13.15.3/data/imgs/chatpdf_ann_df.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.542413 ChatLLM-2023.4.27.13.15.3/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.27.13.15.3/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.27.13.15.3/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.15.3/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.15.3/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.15.3/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.27.13.15.3/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.13.15.3/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.556861 ChatLLM-2023.4.27.13.15.3/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.13.15.3/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     3260 2023-04-26 08:57:26.000000 ChatLLM-2023.4.27.13.15.3/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.27.13.15.3/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.13.15.3/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.27.13.15.3/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.27.13.15.3/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-27 05:15:03.557663 ChatLLM-2023.4.27.13.15.3/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.13.15.3/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 05:15:03.557197 ChatLLM-2023.4.27.13.15.3/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.13.15.3/tox.ini
```

### Comparing `ChatLLM-2023.4.27.13.0.53/.gitignore` & `ChatLLM-2023.4.27.13.15.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/.travis.yml` & `ChatLLM-2023.4.27.13.15.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/CONTRIBUTING.rst` & `ChatLLM-2023.4.27.13.15.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.4.27.13.15.3/ChatLLM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.27.13.0.53
+Version: 2023.4.27.13.15.3
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.27.13.0.53/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.27.13.15.3/ChatLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/LICENSE` & `ChatLLM-2023.4.27.13.15.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/Makefile` & `ChatLLM-2023.4.27.13.15.3/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/PKG-INFO` & `ChatLLM-2023.4.27.13.15.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.27.13.0.53
+Version: 2023.4.27.13.15.3
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.27.13.0.53/README.md` & `ChatLLM-2023.4.27.13.15.3/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatann.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 
 from chatllm.utils import DEVICE, load_llm4chat
 
 
 class ChatBase(object):
 
     def __init__(self, chat_func=None, prompt_template=None,
-                 role='你扮演的角色是ChatLLM智能机器人🤖，由Betterme二次开发'):
+                 role='你扮演的角色是ChatLLM智能助理，由Betterme二次开发'):
         self.chat_func = chat_func
         self.prompt_template = prompt_template if prompt_template else self.default_document_prompt
         self.role = role
 
         #
         self.history = []
         self.knowledge_base = None
 
     def __call__(self, **kwargs):
         return self.qa(**kwargs)
 
-    def qa(self, query, knowledge_base='请自由回答', **kwargs):
+    def qa(self, query, knowledge_base='', **kwargs):
         """可重写"""
         return self._qa(query, knowledge_base, **kwargs)
 
     def set_chat_kwargs(self, **kwargs):
         self.chat_func = partial(self.chat_func, **kwargs)
 
     @clear_cuda_cache
@@ -65,15 +65,16 @@
     def load_llm4chat(self, model_name_or_path="THUDM/chatglm-6b", device=DEVICE, stream=True, **kwargs):
         assert not self.chat_func, "overwrite chat_func"
         self.chat_func = load_llm4chat(model_name_or_path, device, stream, **kwargs)
 
     @property
     def default_document_prompt(self):
         prompt_template = """
-            {role} 基于以下已知信息，简洁和专业的来回答问题。
+            {role}
+            基于以下已知信息，简洁和专业的来回答问题。
             如果无法从中得到答案，请说 "根据已知信息无法回答该问题" 或 "没有提供足够的信息"，不允许在答案中添加编造成分，答案请使用中文。
             已知信息: {context}
             问题: {question}
             """.strip()
 
         return prompt_template
 
@@ -83,9 +84,9 @@
 
     qa = ChatBase()
     qa.load_llm4chat(model_name_or_path="/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
 
     for i, _ in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
         pass
 
-    for i, _ in qa(query='你是谁', knowledge_base='自由回答'):
+    for i, _ in qa(query='你是谁', knowledge_base=''):
         pass
```

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatpdf.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/applications/whoosh_index/MAIN_h83t1id481a6v0bp.seg` & `ChatLLM-2023.4.27.13.15.3/chatllm/applications/whoosh_index/MAIN_h83t1id481a6v0bp.seg`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/applications/whoosh_index/_MAIN_1.toc` & `ChatLLM-2023.4.27.13.15.3/chatllm/applications/whoosh_index/_MAIN_1.toc`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/clis/cli.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/embedding.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/his/FaissANN.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/his/_chatllm.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/his/_qa.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/utils.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/utils.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/webui/chatpdf.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.27.13.15.3/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/data/imgs/LLM.drawio.png` & `ChatLLM-2023.4.27.13.15.3/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/data/imgs/LLM.png` & `ChatLLM-2023.4.27.13.15.3/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/data/imgs/chatpdf.gif` & `ChatLLM-2023.4.27.13.15.3/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.4.27.13.15.3/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.27.13.15.3/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/data/医/古今医统大全.txt` & `ChatLLM-2023.4.27.13.15.3/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/data/姚明.txt` & `ChatLLM-2023.4.27.13.15.3/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/data/王治郅.txt` & `ChatLLM-2023.4.27.13.15.3/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/data/科比.txt` & `ChatLLM-2023.4.27.13.15.3/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/data/财报.pdf` & `ChatLLM-2023.4.27.13.15.3/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/docs/INSTALL.md` & `ChatLLM-2023.4.27.13.15.3/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/docs/Makefile` & `ChatLLM-2023.4.27.13.15.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/docs/README.md` & `ChatLLM-2023.4.27.13.15.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/docs/conf.py` & `ChatLLM-2023.4.27.13.15.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/docs/img.png` & `ChatLLM-2023.4.27.13.15.3/docs/img.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/docs/installation.rst` & `ChatLLM-2023.4.27.13.15.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/docs/make.bat` & `ChatLLM-2023.4.27.13.15.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/setup.py` & `ChatLLM-2023.4.27.13.15.3/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.13.0.53/tests/test_llm4gpt.py` & `ChatLLM-2023.4.27.13.15.3/tests/test_llm4gpt.py`

 * *Files identical despite different names*


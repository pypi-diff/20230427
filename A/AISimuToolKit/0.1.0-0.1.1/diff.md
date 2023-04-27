# Comparing `tmp/AISimuToolKit-0.1.0.tar.gz` & `tmp/AISimuToolKit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AISimuToolKit-0.1.0.tar", last modified: Tue Apr 25 14:24:00 2023, max compression
+gzip compressed data, was "AISimuToolKit-0.1.1.tar", last modified: Thu Apr 27 09:34:25 2023, max compression
```

## Comparing `AISimuToolKit-0.1.0.tar` & `AISimuToolKit-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/exp/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      450 2023-04-24 16:38:46.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/base_action.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1512 2023-04-24 17:36:09.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/finetune_action.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1319 2023-04-22 12:03:37.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/instruct_action.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1965 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/probe_action.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     2524 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/reflect_action.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1866 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/register.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/exp/agents/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/agents/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)    13350 2023-04-25 11:27:15.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/agents/agent.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     9018 2023-04-25 10:46:01.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/agents/memory.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     5388 2023-04-25 11:38:16.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/experiment.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      158 2023-04-24 16:38:46.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/TimeStep.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      537 2023-04-22 12:03:37.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/register.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1309 2023-04-22 12:07:26.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/toolkit.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/model/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/model/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1469 2023-04-25 04:36:11.000000 AISimuToolKit-0.1.0/AISimuToolKit/model/embedding.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     9659 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.0/AISimuToolKit/model/model.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     2106 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.0/AISimuToolKit/model/register.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/store/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/store/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     6652 2023-04-22 11:34:15.000000 AISimuToolKit-0.1.0/AISimuToolKit/store/logger.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/utils/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/utils/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1559 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.0/AISimuToolKit/utils/utils.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      439 2023-04-25 14:24:00.000000 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/PKG-INFO
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1209 2023-04-25 14:24:00.000000 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/SOURCES.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        1 2023-04-25 14:24:00.000000 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/dependency_links.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      132 2023-04-25 14:24:00.000000 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/requires.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       19 2023-04-25 14:24:00.000000 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/top_level.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      439 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/PKG-INFO
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     8780 2023-04-23 03:13:54.000000 AISimuToolKit-0.1.0/README.md
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       38 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/setup.cfg
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1157 2023-04-25 14:23:34.000000 AISimuToolKit-0.1.0/setup.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/test/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-23 03:13:55.000000 AISimuToolKit-0.1.0/test/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/test/exp/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.1.0/test/exp/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/test/exp/agents/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.1.0/test/exp/agents/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      224 2023-04-24 18:44:21.000000 AISimuToolKit-0.1.0/test/exp/agents/test_agent.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1151 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.0/test/test_experiment.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.678927 AISimuToolKit-0.1.1/
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.518934 AISimuToolKit-0.1.1/AISimuToolKit/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.1/AISimuToolKit/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.518934 AISimuToolKit-0.1.1/AISimuToolKit/exp/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.530933 AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      450 2023-04-24 16:38:46.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/base_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1512 2023-04-24 17:36:09.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/finetune_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1319 2023-04-22 12:03:37.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/instruct_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1965 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/probe_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     2524 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/reflect_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1866 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/register.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.562932 AISimuToolKit-0.1.1/AISimuToolKit/exp/agents/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/agents/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)    14342 2023-04-27 09:23:51.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/agents/agent.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     9023 2023-04-27 08:40:40.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/agents/memory.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     5388 2023-04-25 11:38:16.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/experiment.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.626929 AISimuToolKit-0.1.1/AISimuToolKit/exp/toolkit/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      158 2023-04-24 16:38:46.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/toolkit/TimeStep.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/toolkit/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      537 2023-04-22 12:03:37.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/toolkit/register.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1309 2023-04-22 12:07:26.000000 AISimuToolKit-0.1.1/AISimuToolKit/exp/toolkit/toolkit.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.626929 AISimuToolKit-0.1.1/AISimuToolKit/model/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.1/AISimuToolKit/model/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1469 2023-04-25 04:36:11.000000 AISimuToolKit-0.1.1/AISimuToolKit/model/embedding.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     9662 2023-04-27 09:32:26.000000 AISimuToolKit-0.1.1/AISimuToolKit/model/model.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     2106 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.1/AISimuToolKit/model/register.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.626929 AISimuToolKit-0.1.1/AISimuToolKit/store/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.1/AISimuToolKit/store/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     6652 2023-04-22 11:34:15.000000 AISimuToolKit-0.1.1/AISimuToolKit/store/logger.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.626929 AISimuToolKit-0.1.1/AISimuToolKit/utils/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.1/AISimuToolKit/utils/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1559 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.1/AISimuToolKit/utils/utils.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.518934 AISimuToolKit-0.1.1/AISimuToolKit.egg-info/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      439 2023-04-27 09:34:24.000000 AISimuToolKit-0.1.1/AISimuToolKit.egg-info/PKG-INFO
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1209 2023-04-27 09:34:24.000000 AISimuToolKit-0.1.1/AISimuToolKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        1 2023-04-27 09:34:24.000000 AISimuToolKit-0.1.1/AISimuToolKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      132 2023-04-27 09:34:24.000000 AISimuToolKit-0.1.1/AISimuToolKit.egg-info/requires.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       19 2023-04-27 09:34:24.000000 AISimuToolKit-0.1.1/AISimuToolKit.egg-info/top_level.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      439 2023-04-27 09:34:25.678927 AISimuToolKit-0.1.1/PKG-INFO
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     8780 2023-04-23 03:13:54.000000 AISimuToolKit-0.1.1/README.md
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       38 2023-04-27 09:34:25.678927 AISimuToolKit-0.1.1/setup.cfg
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1157 2023-04-27 09:33:50.000000 AISimuToolKit-0.1.1/setup.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.626929 AISimuToolKit-0.1.1/test/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-23 03:13:55.000000 AISimuToolKit-0.1.1/test/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.662927 AISimuToolKit-0.1.1/test/exp/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.1.1/test/exp/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-27 09:34:25.662927 AISimuToolKit-0.1.1/test/exp/agents/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.1.1/test/exp/agents/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      224 2023-04-24 18:44:21.000000 AISimuToolKit-0.1.1/test/exp/agents/test_agent.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1151 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.1/test/test_experiment.py
```

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/finetune_action.py` & `AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/finetune_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/instruct_action.py` & `AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/instruct_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/probe_action.py` & `AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/probe_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/reflect_action.py` & `AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/reflect_action.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/register.py` & `AISimuToolKit-0.1.1/AISimuToolKit/exp/actions/register.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/exp/agents/agent.py` & `AISimuToolKit-0.1.1/AISimuToolKit/exp/agents/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 @author: Guo Shiguang
 @software: PyCharm
 @file: agent.py
 @time: 2023/4/19 9:22
 """
 import json
 import os.path
+import re
 from typing import List
 
 from AISimuToolKit.exp.agents.memory import Memory
 from AISimuToolKit.model.model import ApiBase
 from AISimuToolKit.store.logger import Logger
 
 
@@ -46,14 +47,15 @@
         self.reflect_nums = misc.get("reflect_nums", 10)
         self.summary_nums = misc.get("summary_nums", 10)
         self.importance_prompt = misc.get("importance_prompt",
                                           "On the scale of 1 to 10, where 1 is purely mundane (e.g., brushing teeth, making bed) and 10 is "
                                           "extremely poignant (e.g., a break up,college acceptance), rate the likely poignancy of the following "
                                           "piece of memory. \nMemory: {} \n Rating: <fill in>")
         self.summary = " ".join(profile)
+        self.get_num_pattern = r"\d+\.?\d*|\.\d+"
 
         for item in self.profile_list:
             self._save(experience=item, source="init")
 
     @classmethod
     def load(cls,
              format_num_len: int,
@@ -126,25 +128,40 @@
         """_summary_ 保存到记忆
         Args:
             experience (str): _description_ 经历
         """
         self.logger.history(
             f"agent_{self.agent_id} wrote in memory: {experience} because of {source}")
 
-        importance = self._chat(self.importance_prompt.format(experience))
-
-        try:
-            importance = float(importance)
-        except ValueError:
-            self.logger.error("cannot convert importance to float,set to 5 by default")
-            importance = 5.0
+        importance = self.get_importance(experience)
 
         self.memory.store(interactant='', experience=experience, source=source, importance=importance)
         return True
 
+    def get_importance(self, experience: str) -> float:
+        importance = self._chat(self.importance_prompt.format(experience))
+        self.logger.info(f"store into memory,and automatically get its importance: {importance}")
+        try:
+            importance = float(importance)
+            self.logger.info(f"convert importance to float: {importance}")
+        except Exception:
+            try:
+                num_list = re.findall(self.get_num_pattern, importance)
+                if len(num_list) > 1:
+                    importance = self._chat("find the most important number in the following sentences,it might be an "
+                                            "average number:\n" + importance)
+                    num_list = re.findall(self.get_num_pattern, importance)
+                importance = num_list[0]
+                importance = float(importance)
+                self.logger.info(f"convert importance to float: {importance}")
+            except Exception:
+                self.logger.error("cannot convert importance to float,set to 5.0 by default")
+                importance = 5.0
+        return importance
+
     def _finetune(self, num: int) -> bool:
         """_summary_ 让Agent在给定的语料上微调, 这里的语料是memory中的question和answer
         TODO 加个将经历转换成对话
         Args:
             num (_type_): _description_ 采用的memory数量
         """
         recent_memory = self.memory.retrieve_by_recentness(num)
```

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/exp/agents/memory.py` & `AISimuToolKit-0.1.1/AISimuToolKit/exp/agents/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,26 +184,26 @@
         :param num:
         :return:
         """
 
         def compute_score(row):
             score = 0
             for col in row.index:
-                if col in droped_weights.keys() and isinstance(row[col], (int, float)):
-                    score += row[col] * droped_weights.get(col, 0)
+                if col in dropped_weights.keys() and isinstance(row[col], (int, float)):
+                    score += row[col] * dropped_weights.get(col, 0)
             return score
 
-        droped_weights = weights.copy()
-        droped_weights.pop("similarity", None)
+        dropped_weights = weights.copy()
+        dropped_weights.pop("similarity", None)
         if "similarity" in weights.keys() and query is not None and query != "":
             query_embedding = self.bert.encode(query)
             cos_sim = 1 - pairwise_distances(query_embedding.reshape(1, -1), self.memory_df["embedding"].tolist(),
                                              metric="cosine")
             self.memory_df["similarity"] = cos_sim.reshape(-1)
-            droped_weights = weights
+            dropped_weights = weights
         self.memory_df['score'] = self.memory_df.apply(compute_score, axis=1)
 
         num = len(self.memory_df) if num == -1 else num
         return self.memory_df.sort_values(by="score", ascending=False).head(num).to_dict(orient="records")
 
     # TODO 一个公共的，用于改写对话/检索相关人员/。。。
     def get_model(self) -> PublicApiBase:
```

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/exp/experiment.py` & `AISimuToolKit-0.1.1/AISimuToolKit/exp/experiment.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/register.py` & `AISimuToolKit-0.1.1/AISimuToolKit/exp/toolkit/register.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/toolkit.py` & `AISimuToolKit-0.1.1/AISimuToolKit/exp/toolkit/toolkit.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/model/embedding.py` & `AISimuToolKit-0.1.1/AISimuToolKit/model/embedding.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/model/model.py` & `AISimuToolKit-0.1.1/AISimuToolKit/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                     },
                     "finish_reason": "stop",
                     "index": 0
                 }
             ]
         }
         """
-        self.logger.info("GPT-3.5-turbo: chat start")
+        self.logger.debug("GPT-3.5-turbo: chat start")
         agent_id = kwargs.get("agent_id", "")
         message = [
             {"role": "user", "content": query}
         ]
         completion = openai.ChatCompletion.create(
             model="gpt-3.5-turbo",
             messages=message,
@@ -102,25 +102,25 @@
             if completion["choices"][0]["finish_reason"] == "content_filter":
                 self.logger.warning("GPT-3.5-turbo: chat terminated by content filter")
                 if agent_id is not None:
                     self.logger.warning("GPT-3.5-turbo: agent_id triggers the problem is '{}'".format(agent_id))
                 self.logger.warning("GPT-3.5-turbo: message triggers the problem is '{}'".format(query))
                 break
             elif completion["choices"][0]["finish_reason"] == "length":
-                self.logger.info(
+                self.logger.debug(
                     "GPT-3.5-turbo: chat stop abnormally due to length limit,sending continue automatically")
                 message.append({"role": "assistant", "content": answer})
                 message.append({"role": "user", "content": "continue"})
                 completion = openai.ChatCompletion.create(
                     model="gpt-3.5-turbo",
                     messages=message,
                 )
                 answer = answer + " " + completion["choices"][0]["message"]["content"]
             elif completion["choices"][0]["finish_reason"] == "stop":
-                self.logger.info("GPT-3.5-turbo: chat stop normally")
+                self.logger.debug("GPT-3.5-turbo: chat stop normally")
                 break
             else:
                 self.logger.error("GPT-3.5-turbo: chat stop abnormally")
                 self.logger.error("GPT-3.5-turbo: message triggers the problem is '{}'".format(query))
                 break
         return answer
```

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/model/register.py` & `AISimuToolKit-0.1.1/AISimuToolKit/model/register.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/store/logger.py` & `AISimuToolKit-0.1.1/AISimuToolKit/store/logger.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit/utils/utils.py` & `AISimuToolKit-0.1.1/AISimuToolKit/utils/utils.py`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/AISimuToolKit.egg-info/SOURCES.txt` & `AISimuToolKit-0.1.1/AISimuToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/README.md` & `AISimuToolKit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.1.0/setup.py` & `AISimuToolKit-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages  # 这个包没有的可以pip一下
 
 setup(
     name="AISimuToolKit",  # 这里是pip项目发布的名称
-    version="0.1.0",  # 版本号，数值大的会优先被pip
+    version="0.1.1",  # 版本号，数值大的会优先被pip
     keywords=["pip", "AISimuToolKit"],  # 关键字
     description="ICIP's private utils.",  # 描述
     long_description="ICIP's private utils. The development version will be released when it is sufficiently refined",
     license="MIT Licence",  # 许可证
     url="http://git.cipsup.cn/aisimulationplatform/toolkit/aisimulation",  # 项目相关文件地址，一般是github项目地址即可
     author="Ren & Guo",  # 作者
     author_email="renmengjie22@mails.ucas.ac.cn,guoshiguang22@mails.ucas.edu.cn",
```

### Comparing `AISimuToolKit-0.1.0/test/test_experiment.py` & `AISimuToolKit-0.1.1/test/test_experiment.py`

 * *Files identical despite different names*


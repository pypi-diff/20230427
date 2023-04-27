# Comparing `tmp/sherlibs-27.4.2023.tar.gz` & `tmp/sherlibs-7.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherlibs-27.4.2023.tar", last modified: Wed Apr 26 20:27:23 2023, max compression
+gzip compressed data, was "sherlibs-7.4.4.tar", last modified: Wed Apr 26 20:45:40 2023, max compression
```

## Comparing `sherlibs-27.4.2023.tar` & `sherlibs-7.4.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:27:23.735823 sherlibs-27.4.2023/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:27:23.727823 sherlibs-27.4.2023/Ayra/
--rw-r--r--   0 root         (0) root         (0)     2984 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:27:23.727823 sherlibs-27.4.2023/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4692 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12383 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     1947 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:27:23.731823 sherlibs-27.4.2023/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     2002 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:27:23.735823 sherlibs-27.4.2023/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    19969 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17358 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    28733 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:27:23.735823 sherlibs-27.4.2023/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18537 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       50 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3453 2023-04-26 20:27:23.735823 sherlibs-27.4.2023/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2608 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 20:27:23.735823 sherlibs-27.4.2023/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1520 2023-04-26 20:26:53.000000 sherlibs-27.4.2023/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:27:23.735823 sherlibs-27.4.2023/sherlibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3453 2023-04-26 20:27:23.000000 sherlibs-27.4.2023/sherlibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1471 2023-04-26 20:27:23.000000 sherlibs-27.4.2023/sherlibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 20:27:23.000000 sherlibs-27.4.2023/sherlibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 20:27:23.000000 sherlibs-27.4.2023/sherlibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-26 20:27:23.000000 sherlibs-27.4.2023/sherlibs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.334969 sherlibs-7.4.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.326969 sherlibs-7.4.4/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-04-26 20:45:25.000000 sherlibs-7.4.4/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-04-26 20:45:25.000000 sherlibs-7.4.4/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.326969 sherlibs-7.4.4/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12383 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.330969 sherlibs-7.4.4/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.330969 sherlibs-7.4.4/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    19969 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17358 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28733 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-04-26 20:45:25.000000 sherlibs-7.4.4/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.334969 sherlibs-7.4.4/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18537 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-26 20:45:25.000000 sherlibs-7.4.4/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-04-26 20:26:53.000000 sherlibs-7.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-04-26 20:45:40.334969 sherlibs-7.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-04-26 20:26:53.000000 sherlibs-7.4.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 20:45:40.334969 sherlibs-7.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-04-26 20:26:53.000000 sherlibs-7.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.334969 sherlibs-7.4.4/sherlibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-04-26 20:45:40.000000 sherlibs-7.4.4/sherlibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-04-26 20:45:40.000000 sherlibs-7.4.4/sherlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 20:45:40.000000 sherlibs-7.4.4/sherlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 20:45:40.000000 sherlibs-7.4.4/sherlibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-26 20:45:40.000000 sherlibs-7.4.4/sherlibs.egg-info/top_level.txt
```

### Comparing `sherlibs-27.4.2023/Ayra/__init__.py` & `sherlibs-7.4.4/Ayra/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
             sys.exit()
     else:
         ayra_bot = AyraClient(
             validate_session(Var.SESSION, LOGS),
             udB=udB,
             app_version=ayra_version,
-            device_model="Ayra",
+            device_model="Sherlean",
         )
         ayra_bot.run_in_loop(autobot())
 
     asst = AyraClient(None, bot_token=udB.get_key("BOT_TOKEN"), udB=udB)
 
     if BOT_MODE:
         ayra_bot = asst
@@ -85,21 +85,19 @@
         ayra_bot.run_in_loop(enable_inline(ayra_bot, asst.me.username))
 
     vcClient = vc_connection(udB, ayra_bot)
 
     _version_changes(udB)
 
     HNDLR = udB.get_key("HNDLR") or "."
-    SUDOS = udB.get_key("SUDOS") or "1054295664"
-    VC_SUDOS = udB.get_key("VC_SUDOS") or "1054295664"
     DUAL_HNDLR = udB.get_key("DUAL_HNDLR") or "/"
-    SUDO_HNDLR = udB.get_key("SUDO_HNDLR") or "$"
+    SUDO_HNDLR = udB.get_key("SUDO_HNDLR") or "."
     INLINE_PM = udB.set_key("INLINE_PM", "True")
     PMLOG = udB.set_key("PMLOG", "True")
 else:
-    print("Ayra 2022 © senpai80")
+    print("Sherlean 2023 © shearlean10")
 
     from logging import getLogger
 
-    LOGS = getLogger("Ayra")
+    LOGS = getLogger("Sherlean")
 
     ayra_bot = asst = udB = vcClient = None
```

### Comparing `sherlibs-27.4.2023/Ayra/__main__.py` & `sherlibs-7.4.4/Ayra/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         _plugins = "autocorrect autopic audiotools compressor forcesubscribe fedutils gdrive glitch instagram nsfwfilter nightmode pdftools profanityfilter writer youtube"
         udB.set_key("EXCLUDE_OFFICIAL", _plugins)
 
     load_other_plugins(addons=addons, pmbot=pmbot, manager=manager, vcbot=vcbot)
 
     suc_msg = """
             ----------------------------------------------------------------------
-                                      ◈ ᴀʏʀᴀ ꭙ ᴜꜱᴇʀʙᴏᴛ​ ◈
+                                      sʜᴇᴀʀʟᴇᴀɴ ꭙ͢ ᴜsᴇʀʙᴏᴛ
             ----------------------------------------------------------------------
     """
 
     # for channel plugins
     plugin_channels = udB.get_key("PLUGIN_CHANNEL")
 
     # Customize ayra Assistant...
@@ -88,15 +88,15 @@
 
     try:
         cleanup_cache()
     except BaseException:
         pass
 
     LOGS.info(
-        f"Took {time_formatter((time.time() - start_time)*1000)} to start ◈ ᴀʏʀᴀ ꭙ ᴜꜱᴇʀʙᴏᴛ​ ◈"
+        f"Took {time_formatter((time.time() - start_time)*1000)} to start sʜᴇᴀʀʟᴇᴀɴ ꭙ͢ ᴜsᴇʀʙᴏᴛ"
     )
     LOGS.info(suc_msg)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sherlibs-27.4.2023/Ayra/_misc/__init__.py` & `sherlibs-7.4.4/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/_misc/_assistant.py` & `sherlibs-7.4.4/Ayra/_misc/_assistant.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/_misc/_decorators.py` & `sherlibs-7.4.4/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/_misc/_supporter.py` & `sherlibs-7.4.4/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/_misc/_wrappers.py` & `sherlibs-7.4.4/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/configs.py` & `sherlibs-7.4.4/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/__init__.py` & `sherlibs-7.4.4/Ayra/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/afk_db.py` & `sherlibs-7.4.4/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/antiflood_db.py` & `sherlibs-7.4.4/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/asst_fns.py` & `sherlibs-7.4.4/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/asstcmd_db.py` & `sherlibs-7.4.4/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/autoban_db.py` & `sherlibs-7.4.4/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/blacklist_db.py` & `sherlibs-7.4.4/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/botchat_db.py` & `sherlibs-7.4.4/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/broadcast_db.py` & `sherlibs-7.4.4/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/ch_db.py` & `sherlibs-7.4.4/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/dnd_db.py` & `sherlibs-7.4.4/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/echo_db.py` & `sherlibs-7.4.4/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/filestore_db.py` & `sherlibs-7.4.4/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/filter_db.py` & `sherlibs-7.4.4/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/forcesub_db.py` & `sherlibs-7.4.4/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/gban_mute_db.py` & `sherlibs-7.4.4/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/gcast_blacklist_db.py` & `sherlibs-7.4.4/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/greetings_db.py` & `sherlibs-7.4.4/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/logusers_db.py` & `sherlibs-7.4.4/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/mute_db.py` & `sherlibs-7.4.4/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/night_db.py` & `sherlibs-7.4.4/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/notes_db.py` & `sherlibs-7.4.4/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/nsfw_db.py` & `sherlibs-7.4.4/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/pmpermit_db.py` & `sherlibs-7.4.4/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/snips_db.py` & `sherlibs-7.4.4/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/vc_sudos.py` & `sherlibs-7.4.4/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/dB/warn_db.py` & `sherlibs-7.4.4/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/FastTelethon.py` & `sherlibs-7.4.4/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/__init__.py` & `sherlibs-7.4.4/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/admins.py` & `sherlibs-7.4.4/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/executor.py` & `sherlibs-7.4.4/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/gDrive.py` & `sherlibs-7.4.4/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/google_image.py` & `sherlibs-7.4.4/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/helper.py` & `sherlibs-7.4.4/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/info.py` & `sherlibs-7.4.4/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/misc.py` & `sherlibs-7.4.4/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/tools.py` & `sherlibs-7.4.4/Ayra/fns/tools.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/fns/ytdl.py` & `sherlibs-7.4.4/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/kynan.py` & `sherlibs-7.4.4/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/loader.py` & `sherlibs-7.4.4/Ayra/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             try:
                 modl = func(plugin)
             except ModuleNotFoundError as er:
                 modl = None
                 self._logger.error(f"{plugin}: '{er.name}' tidak terpasang!")
             except Exception as exc:
                 modl = None
-                self._logger.error(f"Ayra - {self.key} - ERROR - {plugin}")
+                self._logger.error(f"Sherlean - {self.key} - ERROR - {plugin}")
                 self._logger.exception(exc)
             if callable(after_load):
                 if func == import_module:
                     plugin = plugin.split(".")[-1]
                 after_load(self, modl, plugin_name=plugin)
 
     def load_single(self, log=False):
```

### Comparing `sherlibs-27.4.2023/Ayra/startup/BaseClient.py` & `sherlibs-7.4.4/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/startup/__init__.py` & `sherlibs-7.4.4/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/startup/_database.py` & `sherlibs-7.4.4/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/startup/_extra.py` & `sherlibs-7.4.4/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/startup/connections.py` & `sherlibs-7.4.4/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/startup/funcs.py` & `sherlibs-7.4.4/Ayra/startup/funcs.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/startup/loader.py` & `sherlibs-7.4.4/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/Ayra/startup/utils.py` & `sherlibs-7.4.4/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/LICENSE` & `sherlibs-7.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/PKG-INFO` & `sherlibs-7.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherlibs
-Version: 27.4.2023
+Version: 7.4.4
 Summary: A Secure and Powerful Python-Telethon Based Library For Shearlean Userbot.
 Home-page: https://github.com/shearlean10/sherlibs
 Author: shearlean10
 Author-email: shearleanshop@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/shearlean10/sherlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `sherlibs-27.4.2023/README.md` & `sherlibs-7.4.4/README.md`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/setup.py` & `sherlibs-7.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `sherlibs-27.4.2023/sherlibs.egg-info/PKG-INFO` & `sherlibs-7.4.4/sherlibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherlibs
-Version: 27.4.2023
+Version: 7.4.4
 Summary: A Secure and Powerful Python-Telethon Based Library For Shearlean Userbot.
 Home-page: https://github.com/shearlean10/sherlibs
 Author: shearlean10
 Author-email: shearleanshop@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/shearlean10/sherlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `sherlibs-27.4.2023/sherlibs.egg-info/SOURCES.txt` & `sherlibs-7.4.4/sherlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/sherlibs-7.4.4.tar.gz` & `tmp/sherlibs-7.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherlibs-7.4.4.tar", last modified: Wed Apr 26 20:45:40 2023, max compression
+gzip compressed data, was "sherlibs-7.4.5.tar", last modified: Thu Apr 27 06:52:16 2023, max compression
```

## Comparing `sherlibs-7.4.4.tar` & `sherlibs-7.4.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.334969 sherlibs-7.4.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.326969 sherlibs-7.4.4/Ayra/
--rw-r--r--   0 root         (0) root         (0)     2893 2023-04-26 20:45:25.000000 sherlibs-7.4.4/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-04-26 20:45:25.000000 sherlibs-7.4.4/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.326969 sherlibs-7.4.4/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4692 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12383 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     1947 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.330969 sherlibs-7.4.4/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     2002 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.330969 sherlibs-7.4.4/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    19969 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17358 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    28733 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-04-26 20:45:25.000000 sherlibs-7.4.4/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.334969 sherlibs-7.4.4/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18537 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-04-26 20:26:53.000000 sherlibs-7.4.4/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-26 20:45:25.000000 sherlibs-7.4.4/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-04-26 20:26:53.000000 sherlibs-7.4.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3449 2023-04-26 20:45:40.334969 sherlibs-7.4.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2608 2023-04-26 20:26:53.000000 sherlibs-7.4.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 20:45:40.334969 sherlibs-7.4.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1520 2023-04-26 20:26:53.000000 sherlibs-7.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:45:40.334969 sherlibs-7.4.4/sherlibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3449 2023-04-26 20:45:40.000000 sherlibs-7.4.4/sherlibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1471 2023-04-26 20:45:40.000000 sherlibs-7.4.4/sherlibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 20:45:40.000000 sherlibs-7.4.4/sherlibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 20:45:40.000000 sherlibs-7.4.4/sherlibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-26 20:45:40.000000 sherlibs-7.4.4/sherlibs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 06:52:16.771362 sherlibs-7.4.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 06:52:16.751363 sherlibs-7.4.5/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-04-26 20:45:25.000000 sherlibs-7.4.5/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-04-26 20:45:25.000000 sherlibs-7.4.5/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 06:52:16.751363 sherlibs-7.4.5/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-04-27 06:51:58.000000 sherlibs-7.4.5/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12383 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 06:52:16.763363 sherlibs-7.4.5/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 06:52:16.767362 sherlibs-7.4.5/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    19969 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17358 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28733 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-04-26 20:45:25.000000 sherlibs-7.4.5/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 06:52:16.771362 sherlibs-7.4.5/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18537 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-04-26 20:26:53.000000 sherlibs-7.4.5/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-27 06:51:58.000000 sherlibs-7.4.5/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-04-26 20:26:53.000000 sherlibs-7.4.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-04-27 06:52:16.771362 sherlibs-7.4.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-04-26 20:26:53.000000 sherlibs-7.4.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 06:52:16.771362 sherlibs-7.4.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-04-26 20:26:53.000000 sherlibs-7.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 06:52:16.771362 sherlibs-7.4.5/sherlibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-04-27 06:52:16.000000 sherlibs-7.4.5/sherlibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-04-27 06:52:16.000000 sherlibs-7.4.5/sherlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 06:52:16.000000 sherlibs-7.4.5/sherlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 06:52:16.000000 sherlibs-7.4.5/sherlibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-27 06:52:16.000000 sherlibs-7.4.5/sherlibs.egg-info/top_level.txt
```

### Comparing `sherlibs-7.4.4/Ayra/__init__.py` & `sherlibs-7.4.5/Ayra/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/__main__.py` & `sherlibs-7.4.5/Ayra/__main__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/_misc/__init__.py` & `sherlibs-7.4.5/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/_misc/_assistant.py` & `sherlibs-7.4.5/Ayra/_misc/_assistant.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         from_users.append(ayra_bot.uid)
 
     def ay(func):
         async def wrapper(event):
             if admins and not await admin_check(event):
                 return
             if from_users and event.sender_id not in from_users:
-                return await event.answer("Not for You!", alert=True)
+                return
             if owner and event.sender_id not in owner_and_sudos():
-                return await event.answer(f"This is {OWNER}'s bot!!")
+                return
             try:
                 await func(event)
             except Exception as er:
                 LOGS.exception(er)
 
         asst.add_event_handler(wrapper, CallbackQuery(data=data, **kwargs))
```

### Comparing `sherlibs-7.4.4/Ayra/_misc/_decorators.py` & `sherlibs-7.4.5/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/_misc/_supporter.py` & `sherlibs-7.4.5/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/_misc/_wrappers.py` & `sherlibs-7.4.5/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/configs.py` & `sherlibs-7.4.5/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/__init__.py` & `sherlibs-7.4.5/Ayra/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/afk_db.py` & `sherlibs-7.4.5/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/antiflood_db.py` & `sherlibs-7.4.5/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/asst_fns.py` & `sherlibs-7.4.5/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/asstcmd_db.py` & `sherlibs-7.4.5/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/autoban_db.py` & `sherlibs-7.4.5/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/blacklist_db.py` & `sherlibs-7.4.5/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/botchat_db.py` & `sherlibs-7.4.5/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/broadcast_db.py` & `sherlibs-7.4.5/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/ch_db.py` & `sherlibs-7.4.5/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/dnd_db.py` & `sherlibs-7.4.5/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/echo_db.py` & `sherlibs-7.4.5/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/filestore_db.py` & `sherlibs-7.4.5/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/filter_db.py` & `sherlibs-7.4.5/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/forcesub_db.py` & `sherlibs-7.4.5/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/gban_mute_db.py` & `sherlibs-7.4.5/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/gcast_blacklist_db.py` & `sherlibs-7.4.5/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/greetings_db.py` & `sherlibs-7.4.5/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/logusers_db.py` & `sherlibs-7.4.5/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/mute_db.py` & `sherlibs-7.4.5/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/night_db.py` & `sherlibs-7.4.5/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/notes_db.py` & `sherlibs-7.4.5/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/nsfw_db.py` & `sherlibs-7.4.5/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/pmpermit_db.py` & `sherlibs-7.4.5/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/snips_db.py` & `sherlibs-7.4.5/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/vc_sudos.py` & `sherlibs-7.4.5/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/dB/warn_db.py` & `sherlibs-7.4.5/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/FastTelethon.py` & `sherlibs-7.4.5/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/__init__.py` & `sherlibs-7.4.5/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/admins.py` & `sherlibs-7.4.5/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/executor.py` & `sherlibs-7.4.5/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/gDrive.py` & `sherlibs-7.4.5/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/google_image.py` & `sherlibs-7.4.5/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/helper.py` & `sherlibs-7.4.5/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/info.py` & `sherlibs-7.4.5/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/misc.py` & `sherlibs-7.4.5/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/tools.py` & `sherlibs-7.4.5/Ayra/fns/tools.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/fns/ytdl.py` & `sherlibs-7.4.5/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/kynan.py` & `sherlibs-7.4.5/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/loader.py` & `sherlibs-7.4.5/Ayra/loader.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/startup/BaseClient.py` & `sherlibs-7.4.5/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/startup/__init__.py` & `sherlibs-7.4.5/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/startup/_database.py` & `sherlibs-7.4.5/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/startup/_extra.py` & `sherlibs-7.4.5/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/startup/connections.py` & `sherlibs-7.4.5/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/startup/funcs.py` & `sherlibs-7.4.5/Ayra/startup/funcs.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/startup/loader.py` & `sherlibs-7.4.5/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/Ayra/startup/utils.py` & `sherlibs-7.4.5/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/LICENSE` & `sherlibs-7.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/PKG-INFO` & `sherlibs-7.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherlibs
-Version: 7.4.4
+Version: 7.4.5
 Summary: A Secure and Powerful Python-Telethon Based Library For Shearlean Userbot.
 Home-page: https://github.com/shearlean10/sherlibs
 Author: shearlean10
 Author-email: shearleanshop@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/shearlean10/sherlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `sherlibs-7.4.4/README.md` & `sherlibs-7.4.5/README.md`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/setup.py` & `sherlibs-7.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `sherlibs-7.4.4/sherlibs.egg-info/PKG-INFO` & `sherlibs-7.4.5/sherlibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherlibs
-Version: 7.4.4
+Version: 7.4.5
 Summary: A Secure and Powerful Python-Telethon Based Library For Shearlean Userbot.
 Home-page: https://github.com/shearlean10/sherlibs
 Author: shearlean10
 Author-email: shearleanshop@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/shearlean10/sherlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `sherlibs-7.4.4/sherlibs.egg-info/SOURCES.txt` & `sherlibs-7.4.5/sherlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


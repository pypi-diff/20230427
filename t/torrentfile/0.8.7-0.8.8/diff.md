# Comparing `tmp/torrentfile-0.8.7.tar.gz` & `tmp/torrentfile-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrentfile-0.8.7.tar", last modified: Sun Jan  8 18:01:17 2023, max compression
+gzip compressed data, was "torrentfile-0.8.8.tar", last modified: Thu Mar  2 10:43:51 2023, max compression
```

## Comparing `torrentfile-0.8.7.tar` & `torrentfile-0.8.8.tar`

### file list

```diff
@@ -1,44 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-01-08 18:01:17.407110 torrentfile-0.8.7/
--rw-rw-rw-   0        0        0     1879 2022-06-06 03:34:50.000000 torrentfile-0.8.7/.cbuild
--rw-rw-rw-   0        0        0     9602 2023-01-08 17:41:18.000000 torrentfile-0.8.7/CHANGELOG.md
--rw-rw-rw-   0        0        0    11560 2022-04-01 22:38:43.000000 torrentfile-0.8.7/LICENSE
--rw-rw-rw-   0        0        0      242 2022-08-07 23:54:01.000000 torrentfile-0.8.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2691 2022-12-09 04:15:09.000000 torrentfile-0.8.7/Makefile
--rw-rw-rw-   0        0        0    21745 2023-01-08 18:01:17.407110 torrentfile-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0     7118 2022-11-23 00:37:40.000000 torrentfile-0.8.7/README.md
-drwxrwxrwx   0        0        0        0 2023-01-08 18:01:17.386314 torrentfile-0.8.7/assets/
--rw-rw-rw-   0        0        0   999094 2022-10-21 07:26:02.000000 torrentfile-0.8.7/assets/Torrentfile.gif
--rw-rw-rw-   0        0        0    67244 2022-05-08 04:09:13.000000 torrentfile-0.8.7/assets/torrentfile-icon.ico
--rw-rw-rw-   0        0        0    31493 2022-05-08 04:09:13.000000 torrentfile-0.8.7/assets/torrentfile-icon.png
--rw-rw-rw-   0        0        0    25857 2022-02-13 04:29:03.000000 torrentfile-0.8.7/assets/torrentfile.png
-drwxrwxrwx   0        0        0        0 2023-01-08 18:01:17.388437 torrentfile-0.8.7/c/
--rw-rw-rw-   0        0        0    12601 2022-04-05 09:08:46.000000 torrentfile-0.8.7/c/hasher.c
--rw-rw-rw-   0        0        0     1396 2022-04-01 22:38:43.000000 torrentfile-0.8.7/c/hasher.h
--rw-rw-rw-   0        0        0    11387 2022-04-01 22:38:43.000000 torrentfile-0.8.7/c/sha.c
--rw-rw-rw-   0        0        0     1629 2022-04-01 22:38:43.000000 torrentfile-0.8.7/c/sha.h
--rw-rw-rw-   0        0        0     2599 2023-01-08 17:41:18.000000 torrentfile-0.8.7/pyproject.toml
--rw-rw-rw-   0        0        0       13 2022-06-05 02:35:20.000000 torrentfile-0.8.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-08 18:01:17.407110 torrentfile-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0      914 2022-08-07 23:54:01.000000 torrentfile-0.8.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-08 18:01:17.398373 torrentfile-0.8.7/torrentfile/
--rw-rw-rw-   0        0        0     1730 2023-01-08 18:01:11.000000 torrentfile-0.8.7/torrentfile/__init__.py
--rw-rw-rw-   0        0        0     1079 2023-01-08 18:01:11.000000 torrentfile-0.8.7/torrentfile/__main__.py
--rw-rw-rw-   0        0        0    17574 2023-01-08 18:01:12.000000 torrentfile-0.8.7/torrentfile/cli.py
--rw-rw-rw-   0        0        0     9087 2023-01-08 18:01:12.000000 torrentfile-0.8.7/torrentfile/commands.py
--rw-rw-rw-   0        0        0     3777 2023-01-08 18:01:11.000000 torrentfile-0.8.7/torrentfile/edit.py
--rw-rw-rw-   0        0        0    16936 2023-01-08 18:01:11.000000 torrentfile-0.8.7/torrentfile/hasher.py
--rw-rw-rw-   0        0        0    11745 2023-01-08 18:01:12.000000 torrentfile-0.8.7/torrentfile/interactive.py
--rw-rw-rw-   0        0        0     7952 2023-01-08 18:01:12.000000 torrentfile-0.8.7/torrentfile/mixins.py
--rw-rw-rw-   0        0        0    19468 2023-01-08 18:01:14.000000 torrentfile-0.8.7/torrentfile/rebuild.py
--rw-rw-rw-   0        0        0    20600 2023-01-08 18:01:12.000000 torrentfile-0.8.7/torrentfile/recheck.py
--rw-rw-rw-   0        0        0    24356 2023-01-08 18:01:13.000000 torrentfile-0.8.7/torrentfile/torrent.py
--rw-rw-rw-   0        0        0    10893 2023-01-08 18:01:12.000000 torrentfile-0.8.7/torrentfile/utils.py
--rw-rw-rw-   0        0        0      905 2023-01-08 18:01:11.000000 torrentfile-0.8.7/torrentfile/version.py
-drwxrwxrwx   0        0        0        0 2023-01-08 18:01:17.405188 torrentfile-0.8.7/torrentfile.egg-info/
--rw-rw-rw-   0        0        0    21745 2023-01-08 18:01:17.000000 torrentfile-0.8.7/torrentfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-01-08 18:01:17.000000 torrentfile-0.8.7/torrentfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-08 18:01:17.000000 torrentfile-0.8.7/torrentfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-01-08 18:01:17.000000 torrentfile-0.8.7/torrentfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-01-08 18:01:17.000000 torrentfile-0.8.7/torrentfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-01-08 18:01:17.000000 torrentfile-0.8.7/torrentfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1258 2023-01-08 17:41:18.000000 torrentfile-0.8.7/tox.ini
+drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.193834 torrentfile-0.8.8/
+-rw-rw-rw-   0        0        0     1879 2022-06-06 03:34:50.000000 torrentfile-0.8.8/.cbuild
+-rw-rw-rw-   0        0        0     9123 2023-03-02 05:11:02.000000 torrentfile-0.8.8/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11560 2022-04-01 22:38:43.000000 torrentfile-0.8.8/LICENSE
+-rw-rw-rw-   0        0        0      153 2023-01-14 00:36:54.000000 torrentfile-0.8.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2610 2023-03-02 04:35:28.000000 torrentfile-0.8.8/Makefile
+-rw-rw-rw-   0        0        0    22470 2023-03-02 10:43:51.193834 torrentfile-0.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7644 2023-03-02 05:53:52.000000 torrentfile-0.8.8/README.md
+drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.170080 torrentfile-0.8.8/assets/
+-rw-rw-rw-   0        0        0   999094 2022-10-21 07:26:02.000000 torrentfile-0.8.8/assets/Torrentfile.gif
+-rw-rw-rw-   0        0        0    67244 2022-05-08 04:09:13.000000 torrentfile-0.8.8/assets/torrentfile-icon.ico
+-rw-rw-rw-   0        0        0    31493 2022-05-08 04:09:13.000000 torrentfile-0.8.8/assets/torrentfile-icon.png
+-rw-rw-rw-   0        0        0    25857 2022-02-13 04:29:03.000000 torrentfile-0.8.8/assets/torrentfile.png
+drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.173109 torrentfile-0.8.8/c/
+-rw-rw-rw-   0        0        0    12601 2022-04-05 09:08:46.000000 torrentfile-0.8.8/c/hasher.c
+-rw-rw-rw-   0        0        0     1396 2022-04-01 22:38:43.000000 torrentfile-0.8.8/c/hasher.h
+-rw-rw-rw-   0        0        0    11387 2022-04-01 22:38:43.000000 torrentfile-0.8.8/c/sha.c
+-rw-rw-rw-   0        0        0     1629 2022-04-01 22:38:43.000000 torrentfile-0.8.8/c/sha.h
+-rw-rw-rw-   0        0        0     2511 2023-03-02 07:28:29.000000 torrentfile-0.8.8/pyproject.toml
+-rw-rw-rw-   0        0        0       13 2022-06-05 02:35:20.000000 torrentfile-0.8.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-03-02 10:43:51.194857 torrentfile-0.8.8/setup.cfg
+-rw-rw-rw-   0        0        0      914 2022-08-07 23:54:01.000000 torrentfile-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.179106 torrentfile-0.8.8/tests/
+-rw-rw-rw-   0        0        0    14895 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_cli.py
+-rw-rw-rw-   0        0        0     9288 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_commands.py
+-rw-rw-rw-   0        0        0     7214 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_edit.py
+-rw-rw-rw-   0        0        0     5171 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_interactive.py
+-rw-rw-rw-   0        0        0     5823 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_rebuild.py
+-rw-rw-rw-   0        0        0     8804 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_recheck.py
+-rw-rw-rw-   0        0        0     7030 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_torrent.py
+-rw-rw-rw-   0        0        0     6741 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.188175 torrentfile-0.8.8/torrentfile/
+-rw-rw-rw-   0        0        0     1810 2023-03-02 10:42:15.000000 torrentfile-0.8.8/torrentfile/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-03-02 10:42:15.000000 torrentfile-0.8.8/torrentfile/__main__.py
+-rw-rw-rw-   0        0        0    17505 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/cli.py
+-rw-rw-rw-   0        0        0    11276 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/commands.py
+-rw-rw-rw-   0        0        0     3647 2023-03-02 06:39:30.000000 torrentfile-0.8.8/torrentfile/edit.py
+-rw-rw-rw-   0        0        0    16402 2023-03-02 06:39:30.000000 torrentfile-0.8.8/torrentfile/hasher.py
+-rw-rw-rw-   0        0        0    11745 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/interactive.py
+-rw-rw-rw-   0        0        0     7695 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/mixins.py
+-rw-rw-rw-   0        0        0    18852 2023-03-02 10:42:19.000000 torrentfile-0.8.8/torrentfile/rebuild.py
+-rw-rw-rw-   0        0        0    20594 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/recheck.py
+-rw-rw-rw-   0        0        0    23628 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/torrent.py
+-rw-rw-rw-   0        0        0    11604 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/utils.py
+-rw-rw-rw-   0        0        0      882 2023-03-02 05:07:36.000000 torrentfile-0.8.8/torrentfile/version.py
+drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.193321 torrentfile-0.8.8/torrentfile.egg-info/
+-rw-rw-rw-   0        0        0    22470 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      927 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1893 2023-03-02 06:44:09.000000 torrentfile-0.8.8/tox.ini
```

### Comparing `torrentfile-0.8.7/.cbuild` & `torrentfile-0.8.8/.cbuild`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/LICENSE` & `torrentfile-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/PKG-INFO` & `torrentfile-0.8.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrentfile
-Version: 0.8.7
+Version: 0.8.8
 Summary: Terminal based command line tool for creating Bittorrent files.
 Author-email: alexpdev <alexpdev@pm.me>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -237,15 +237,15 @@
 ![torrentfile](https://github.com/alexpdev/torrentfile/blob/master/site/images/torrentfile.png?raw=true)
 
 * * *
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/alexpdev/torrentfile?color=orange)
 ![GitHub License](https://img.shields.io/github/license/alexpdev/torrentfile?color=red&logo=apache)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/torrentfile?color=brown)
-![GitHub Last Commit](https://badgen.net/github/last-commit/alexpdev/torrentfile?color=blue&icon=github)
+![GitHub Last Commit](https://badgen.net/github/last-commit/alexpdev/torrentfile?color=blue)
 [![CI](https://github.com/alexpdev/TorrentFile/actions/workflows/pyworkflow.yml/badge.svg?branch=master&event=push)](https://github.com/alexpdev/torrentfile/actions/workflows/pyworkflow.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/b67ff65b3d574025b65b6587266bbab7)](https://www.codacy.com/gh/alexpdev/torrentfile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=alexpdev/torrentfile&utm_campaign=Badge_Coverage)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b67ff65b3d574025b65b6587266bbab7)](https://www.codacy.com/gh/alexpdev/torrentfile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=alexpdev/torrentfile&utm_campaign=Badge_Grade)
 [![DeepSource](https://deepsource.io/gh/alexpdev/TorrentFile.svg/?label=active+issues&token=16Sl_dF7nTU8YgPilcqhvHm8)](https://deepsource.io/gh/alexpdev/torrentfile/)
 [![codecov](https://codecov.io/gh/alexpdev/torrentfile/branch/master/graph/badge.svg?token=EWF7NIL9SQ)](https://codecov.io/gh/alexpdev/torrentfile?color=navy&logo=codecov)
 
 ## 🌐 Overview
@@ -341,54 +341,63 @@
 torrentfile --quiet create /path/to/content
 ```
 
 ```bash
 torrentfile create /path/to/content --prog 0
 ```
 
-**`torrentfile`** automatically extracts the name of the file or directory  
-if the content and saves the file to the current working directory with the 
-extracted title.
+**`torrentfile`** extracts the name of the contents top level file or directory  
+and saves the torrent file to the current working directory with the extracted title.
 
 For example running the follwing command would create `./content.torrent`.
 
 ```bash
 torrentfile create /path/to/content
 ```
 
 To specify an alternative path or filename you may use the `-o`, `--out` flags  
 followed by the relative or absolute path to your preferred output location.
 
 ```bash
 torrentfile create /path/to/content -o /some/other/path/torrent.torrent
 ```
 
-If the path you specified with the `-o` flag already exists and is a directory,  
-then torrentfile will save the output to that directory with the default extracted title.
+If the path `--out` path specified is an existing directory, then the torrent file will be
+saved to that directory, with same filename as the default top level path name.
 
-For example the following command would create a Bittorrent file at `/some/other/path/content.torrent`.
+For example the following command would create a torrent file at `/some/other/path/content.torrent`.
 
 ```bash
 torrentfile create /path/to/content -o /some/other/path/
 ```
 
-Bittorrent V1 is still the most common version of torrent files and the most widely accepted,  
-therefore by default torrentfile uses the version 1 format.  However if you are using a modern 
-Bittorrent client and tracker then you may wish to use the newest version Bittorrent V2 or 
-a combination of the two.  To do this simply use the `--meta-version` flag with the appropriate  
-version.  Options include `1`(v1 default), `2`(v2), or `3`(v1 & v2).
+Bittorrent protocol V1 is still the most common version in use for torrent files, 
+therefore by default __`torrentfile`__ uses the version 1 format when creating the file.  
+However __`torrentfile`__ has full support for creating V2 format torrent files as well as 
+hybrid V1 & V2 format files. Use the `--meta-version` flag to specify which file format
+should be used during torrent file creation. Options include `1`(v1 default), `2`(v2), or `3`(v1 & v2).
 
 ```bash
 torrentfile create /path/to/content --meta-version 2
 ```
 
 ```bash
 torrentfile create /path/to/content --meta-version 3 
 ```
 
+__NEW FEATURE in v0.8.8__:
+
+>`torrentfile` now includes the option to command line flags for the `create` sub-command from an `ini` style
+configuration file, by using the `--config` and optional `--config-path` options to specify the path
+to the configuration file.  If `--config-path` is ommited, then `torrentfile` will look by default in the current
+working directory for a file named `torrentfile.ini`. If the file is not discovered in the current working directory, 
+it will move on to look `~/.torrentfile/torrentfile.ini` followed by `~/.config/torrentfile.ini`.  Please see the 
+[documentation](https://alexpdev.github.io/torrentfile/overview/) for more details on how the configuration file should be
+formatted.
+
 ### Check/Recheck Torrent
 
 The `recheck` subcommand allows you to scan a Bittorrent file and compare it's contents, 
 against a file or directory containing the contents the torrent file was created from.
 The output provided by this process gives a detailed perspective if any files are missing
 or have been corrupted in any way.  Supports any version of Bittorrent file.
 
@@ -404,15 +413,15 @@
 
 ```bash
 torrentfile edit /path/to/content --tracker https://new.tracker.url1.com  https://newtracker.url/2
 ```
 
 You can use the `-h` flag for a full list of available fields that can be edited.
 
-    torrentfile edit -h
+    __`torrentfile`__ edit -h
 
 ### Create Magnet
 
 To create a magnet URI for a pre-existing torrent meta file, use the sub-command  
 `magnet` or `m` with the path to the torrent file.
 
 ```bash
```

### Comparing `torrentfile-0.8.7/assets/Torrentfile.gif` & `torrentfile-0.8.8/assets/Torrentfile.gif`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/assets/torrentfile-icon.ico` & `torrentfile-0.8.8/assets/torrentfile-icon.ico`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/assets/torrentfile-icon.png` & `torrentfile-0.8.8/assets/torrentfile-icon.png`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/assets/torrentfile.png` & `torrentfile-0.8.8/assets/torrentfile.png`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/c/hasher.c` & `torrentfile-0.8.8/c/hasher.c`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/c/hasher.h` & `torrentfile-0.8.8/c/hasher.h`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/c/sha.c` & `torrentfile-0.8.8/c/sha.c`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/c/sha.h` & `torrentfile-0.8.8/c/sha.h`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/pyproject.toml` & `torrentfile-0.8.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,102 @@
-[build-system]
-requires = ["setuptools>=40.8.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "torrentfile"
-authors = [{name = "alexpdev", email = "alexpdev@pm.me"}]
-description = "Terminal based command line tool for creating Bittorrent files."
-license = {file = "LICENSE"}
-version = "0.8.7"
-readme = "README.md"
-requires-python = ">=3.6"
-keywords = ["Bittorrent", "torrent", "bittorrent-metafiles", "CLI"]
-classifiers = [
-    "Environment :: Console",
-    "Development Status :: 4 - Beta",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3 :: Only",
-    "Intended Audience :: End Users/Desktop",
-    "Intended Audience :: Developers",
-    "Topic :: Utilities",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: Apache Software License",
-]
-dependencies = ["pyben"]
-
-[project.scripts]
-torrentfile = "torrentfile:main"
-tfile = "torrentfile:main"
-
-[project.urls]
-homepage = "https://github.com/alexpdev/torrentfile"
-repository = "https://github.com"
-documentation = "https://alexpdev.github.io/torrentfile"
-changelog = "https://alexpdev.github.io/torrentfile/changelog/"
-issues = "https://github.com/alexpdev/torrentfile/issues"
-
-[tool.setuptools]
-packages = ["torrentfile"]
-
-[tool.bandit]
-skips = ["B101"]
-
-[tool.black]
-line-length = 79
-
-[tool.autopep8]
-max_line_length = 80
-ignore = "E266"
-in-place = true
-recursive = true
-aggressive = 3
-
-[tool.pytest.ini_options]
-testpaths = [
-    "tests",
-    "torrentfile",
-]
-console_output_style = "progress"
-addopts = "--maxfail=3"
-
-
-[tool.pylint. 'MESSAGES CONTROL']
-disable = [
-    "R1729",
-    "W0108",
-    "redefined-outer-name",
-    "attribute-defined-outside-init",
-    "invalid-name",
-    "not-callable",
-    "consider-using-with",
-    "implicit-str-concat"
-]
-
-[tool.pylint. 'VARIABLES']
-callbacks = ["cb_", "_cb", "hook_"]
-
-[tool.pylint. 'FORMAT']
-max-line-length = 80
-single-line-if-stmt = true
-
-[tool.pylint.'SIMILARITIES']
-ignore-comments = true
-ignore-docstrings=true
-ignore-imports=true
-
-[tool.pylint. 'DESIGN']
-max-args=15
-min-public-methods=0
-max-attributes=20
-max-statements=75
-max-branches=20
-min-similarity-lines=4
-max-locals=25
+[build-system]
+requires = ["setuptools>=40.8.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "torrentfile"
+authors = [{name = "alexpdev", email = "alexpdev@pm.me"}]
+description = "Terminal based command line tool for creating Bittorrent files."
+license = {file = "LICENSE"}
+version = "0.8.8"
+readme = "README.md"
+requires-python = ">=3.6"
+keywords = ["Bittorrent", "torrent", "bittorrent-metafiles", "CLI"]
+classifiers = [
+    "Environment :: Console",
+    "Development Status :: 4 - Beta",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3 :: Only",
+    "Intended Audience :: End Users/Desktop",
+    "Intended Audience :: Developers",
+    "Topic :: Utilities",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: Apache Software License",
+]
+dependencies = ["pyben"]
+
+[project.scripts]
+torrentfile = "torrentfile:main"
+tfile = "torrentfile:main"
+
+[project.urls]
+homepage = "https://github.com/alexpdev/torrentfile"
+repository = "https://github.com"
+documentation = "https://alexpdev.github.io/torrentfile"
+changelog = "https://alexpdev.github.io/torrentfile/changelog/"
+issues = "https://github.com/alexpdev/torrentfile/issues"
+
+[tool.setuptools]
+packages = ["torrentfile"]
+
+[tool.bandit]
+skips = ["B101"]
+
+[tool.black]
+line-length = 79
+
+[tool.autopep8]
+max_line_length = 80
+ignore = "E266"
+in-place = true
+recursive = true
+aggressive = 3
+
+[tool.pytest.ini_options]
+testpaths = [
+    "tests",
+    "torrentfile",
+]
+console_output_style = "progress"
+addopts = "--maxfail=3"
+
+
+[tool.pylint. 'MESSAGES CONTROL']
+disable = [
+    "R1729",
+    "W0108",
+    "W0106",
+    "redefined-outer-name",
+    "attribute-defined-outside-init",
+    "invalid-name",
+    "not-callable",
+    "consider-using-with",
+    "implicit-str-concat"
+]
+
+[tool.pylint. 'VARIABLES']
+callbacks = ["cb_", "_cb", "hook_"]
+
+[tool.pylint. 'FORMAT']
+max-line-length = 80
+single-line-if-stmt = true
+
+[tool.pylint.'SIMILARITIES']
+ignore-comments = true
+ignore-docstrings=true
+ignore-imports=true
+
+[tool.pylint. 'DESIGN']
+max-args=15
+min-public-methods=0
+max-attributes=20
+max-statements=75
+max-branches=20
+min-similarity-lines=4
+max-locals=25
```

### Comparing `torrentfile-0.8.7/setup.py` & `torrentfile-0.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/torrentfile/__init__.py` & `torrentfile-0.8.8/torrentfile/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,8 +33,19 @@
 from torrentfile.cli import execute, main
 from torrentfile.commands import create, edit, info, magnet, recheck
 from torrentfile.utils import toggle_debug_mode
 from torrentfile.version import __version__
 
 toggle_debug_mode(False)
 
-__all__ = ["execute", "create", "edit", "info", "magnet", "recheck", "main"]
+VERSION = __version__
+
+__all__ = [
+    "execute",
+    "create",
+    "edit",
+    "info",
+    "magnet",
+    "recheck",
+    "main",
+    "VERSION",
+]
```

### Comparing `torrentfile-0.8.7/torrentfile/__main__.py` & `torrentfile-0.8.8/torrentfile/__main__.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/torrentfile/cli.py` & `torrentfile-0.8.8/torrentfile/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,656 +1,664 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Command Line Interface for TorrentFile project.
-
-This module provides the primary command line argument parser for
-the torrentfile package. The main_script function is automatically
-invoked when called from command line, and parses accompanying arguments.
-
-Functions
----------
-main_script :
-    process command line arguments and run program.
-activate_logger :
-    turns on debug mode and logging facility.
-
-Classes
--------
-Config : class
-    controls logging configuration
-TorrentFileHelpFormatter : HelpFormatter
-    the command line help message formatter
-"""
-
-import io
-import logging
-import sys
-from argparse import ArgumentParser, HelpFormatter
-
-from torrentfile.commands import (
-    create,
-    edit,
-    info,
-    magnet,
-    rebuild,
-    recheck,
-    rename,
-)
-from torrentfile.interactive import select_action
-from torrentfile.utils import toggle_debug_mode
-from torrentfile.version import __version__ as version
-
-
-class Config:
-    """
-    Class the controls the logging configuration and output settings.
-
-    Controls the logging level, or whether to app should operate in quiet mode.
-    """
-
-    @staticmethod
-    def activate_quiet():
-        """
-        Activate quiet mode for the duration of the programs life.
-
-        When quiet mode is enabled, no logging, progress or state information
-        is output to the terminal
-        """
-        if sys.stdout or sys.stderr:
-            sys.stdout = io.StringIO()
-            sys.stderr = io.StringIO()
-
-    @staticmethod
-    def activate_logger():
-        """
-        Activate the builtin logging mechanism when passed debug flag from CLI.
-        """
-        logging.basicConfig(level=logging.WARNING)
-        logger = logging.getLogger()
-        console_handler = logging.StreamHandler(stream=sys.stderr)
-        stream_formatter = logging.Formatter(
-            "[%(asctime)s] [%(levelno)s] %(message)s",
-            datefmt="%H:%M:%S",
-            style="%",
-        )
-        console_handler.setFormatter(stream_formatter)
-        console_handler.setLevel(logging.DEBUG)
-        logger.setLevel(logging.DEBUG)
-        logger.addHandler(console_handler)
-        logger.debug("Debug: ON")
-        toggle_debug_mode(True)
-
-
-class TorrentFileHelpFormatter(HelpFormatter):
-    """
-    Formatting class for help tips provided by the CLI.
-
-    Subclasses Argparse.HelpFormatter.
-    """
-
-    def __init__(self, prog, width=45, max_help_positions=45):
-        """
-        Construct HelpFormat class for usage output.
-
-        Parameters
-        ----------
-        prog : str
-            Name of the program.
-        width : int
-            Max width of help message output.
-        max_help_positions : int
-            max length until line wrap.
-        """
-        super().__init__(
-            prog, width=width, max_help_position=max_help_positions
-        )
-
-    def _split_lines(self, text: str, _: int) -> list:
-        """
-        Split multiline help messages and remove indentation.
-
-        Parameters
-        ----------
-        text : str
-            text that needs to be split
-        _ : int
-            max width for line.
-
-        Returns
-        -------
-        list :
-            split into multiline text list
-        """
-        lines = text.split("\n")
-        return [line.strip() for line in lines if line]
-
-    def _format_text(self, text: str) -> str:
-        """
-        Format text for cli usage messages.
-
-        Parameters
-        ----------
-        text : str
-            Pre-formatted text.
-
-        Returns
-        -------
-        str
-            Formatted text from input.
-        """
-        text = text % dict(prog=self._prog) if "%(prog)" in text else text
-        text = self._whitespace_matcher.sub(" ", text).strip()
-        return text + "\n\n"
-
-    def _join_parts(self, part_strings: list) -> str:
-        """
-        Combine different sections of the help message.
-
-        Parameters
-        ----------
-        part_strings : list
-            List of argument help messages and headers.
-
-        Returns
-        -------
-        str
-            Fully formatted help message for CLI.
-        """
-        parts = self._format_headers(part_strings)
-        return super()._join_parts(parts)
-
-    @staticmethod
-    def _format_headers(parts: list) -> list:
-        """
-        Format help message section headers.
-
-        Parameters
-        ----------
-        parts : list
-            List of individual lines for help message.
-
-        Returns
-        -------
-        list
-            Input list with formatted section headers.
-        """
-        if parts and parts[0].startswith("usage:"):
-            parts[0] = "Usage\n=====\n  " + parts[0][6:]
-        headings = [i for i in range(len(parts)) if parts[i].endswith(":\n")]
-        for i in headings[::-1]:
-            parts[i] = parts[i][:-2].title()
-            underline = "".join(["\n", "-" * len(parts[i]), "\n"])
-            parts.insert(i + 1, underline)
-        return parts
-
-
-def execute(args: list = None) -> list:
-    """
-    Execute program with provided list of arguments.
-
-    If no arguments are given then it defaults to using
-    sys.argv.  This is the main entrypoint for the program
-    and command line interface.
-
-    Parameters
-    ----------
-    args : list
-        Commandline arguments. default=None
-
-    Returns
-    -------
-    list
-        Depends on what the command line args were.
-    """
-    toggle_debug_mode(False)
-    if not args:
-        if sys.argv[1:]:
-            args = sys.argv[1:]
-        else:
-            args = ["-h"]
-
-    parser = ArgumentParser(
-        "torrentfile",
-        usage="torrentfile <options>",
-        description=(
-            "Command line tools for creating, editing, checking, building "
-            "and interacting with Bittorrent metainfo files"
-        ),
-        prefix_chars="-",
-        formatter_class=TorrentFileHelpFormatter,
-        conflict_handler="resolve",
-    )
-
-    parser.add_argument(
-        "-i",
-        "--interactive",
-        action="store_true",
-        dest="interactive",
-        help="#Deprecated\t select program options interactively",
-    )
-
-    parser.add_argument(
-        "-q",
-        "--quiet",
-        help="Turn off all text output.",
-        dest="quiet",
-        action="store_true",
-    )
-
-    parser.add_argument(
-        "-V",
-        "--version",
-        action="version",
-        version=f"torrentfile v{version}",
-        help="show program version and exit",
-    )
-
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        dest="debug",
-        help="output debug information",
-    )
-
-    parser.set_defaults(func=parser.print_help)
-
-    subparsers = parser.add_subparsers(
-        title="Commands",
-        dest="command",
-        metavar="create, edit, info, magnet, recheck, rebuild, rename\n",
-    )
-
-    create_parser = subparsers.add_parser(
-        "create",
-        help="Create a new Bittorrent file.",
-        prefix_chars="-",
-        aliases=["c", "new"],
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    create_parser.add_argument(
-        "-a",
-        "-t",
-        "--announce",
-        "--tracker",
-        action="store",
-        dest="announce",
-        metavar="<url>",
-        nargs="+",
-        default=[],
-        help="One or more space-seperated torrent tracker url(s).",
-    )
-
-    create_parser.add_argument(
-        "-p",
-        "--private",
-        action="store_true",
-        dest="private",
-        help="Creates private torrent with multi-tracker and DHT turned off.",
-    )
-
-    create_parser.add_argument(
-        "-s",
-        "--source",
-        action="store",
-        dest="source",
-        metavar="<source>",
-        help="Add a source string. Useful for cross-seeding.",
-    )
-
-    create_parser.add_argument(
-        "-m",
-        "--magnet",
-        action="store_true",
-        dest="magnet",
-    )
-
-    create_parser.add_argument(
-        "-c",
-        "--comment",
-        action="store",
-        dest="comment",
-        metavar="<comment>",
-        help="Include a comment in file metadata",
-    )
-
-    create_parser.add_argument(
-        "-o",
-        "--out",
-        action="store",
-        dest="outfile",
-        metavar="<path>",
-        help="Explicitly specify the path to write the file.",
-    )
-
-    create_parser.add_argument(
-        "--cwd",
-        "--current",
-        action="store_true",
-        dest="cwd",
-        help="*deprecated* Saving to current directory is default behaviour",
-    )
-
-    create_parser.add_argument(
-        "--prog",
-        "--progress",
-        default="1",
-        action="store",
-        dest="progress",
-        help="""
-        Set the progress bar level.
-        Options = 0, 1
-        (0) = Do not display progress bar.
-        (1) = Display progress bar.(default)
-        """,
-    )
-
-    create_parser.add_argument(
-        "--meta-version",
-        default="1",
-        choices=["1", "2", "3"],
-        action="store",
-        dest="meta_version",
-        metavar="<int>",
-        help="""
-        Bittorrent metafile version.
-        Options = 1, 2, 3
-        (1) = Bittorrent v1 (Default)
-        (2) = Bittorrent v2
-        (3) = Bittorrent v1 & v2 hybrid
-        """,
-    )
-
-    create_parser.add_argument(
-        "--piece-length",
-        action="store",
-        dest="piece_length",
-        metavar="<int>",
-        help="""
-        (Default: <blank>) Number of bytes for per chunk of data transmitted
-        by Bittorrent client. Acceptable values include integers 14-26 which
-        will be interpreted as a perfect power of 2.  e.g. 14 = 16KiB pieces.
-        Examples:: [--piece-length 14] [--piece-length 20]
-        """,
-    )
-
-    create_parser.add_argument(
-        "-w",
-        "--web-seed",
-        action="store",
-        dest="url_list",
-        metavar="<url>",
-        nargs="+",
-        help="list of web addresses where torrent data exists (GetRight).",
-    )
-
-    create_parser.add_argument(
-        "--http-seed",
-        action="store",
-        dest="httpseeds",
-        metavar="<url>",
-        nargs="+",
-        help="list of URLs, addresses where content can be found (Hoffman).",
-    )
-
-    create_parser.add_argument(
-        "content",
-        action="store",
-        metavar="<content>",
-        nargs="?",
-        help="Path to content file or directory",
-    )
-
-    create_parser.set_defaults(func=create)
-
-    edit_parser = subparsers.add_parser(
-        "edit",
-        help="""Edit existing torrent meta file.""",
-        aliases=["e"],
-        prefix_chars="-",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    edit_parser.add_argument(
-        "metafile",
-        action="store",
-        help="path to *.torrent file",
-        metavar="<*.torrent>",
-    )
-
-    edit_parser.add_argument(
-        "--tracker",
-        action="store",
-        dest="announce",
-        metavar="<url>",
-        nargs="+",
-        help="""
-        Replace current list of tracker/announce urls with one or more space
-        seperated Bittorrent tracker announce url(s).
-        """,
-    )
-
-    edit_parser.add_argument(
-        "--web-seed",
-        action="store",
-        dest="url_list",
-        metavar="<url>",
-        nargs="+",
-        help="Replace current list of web-seed urls with one or more url(s)",
-    )
-
-    edit_parser.add_argument(
-        "--http-seed",
-        action="store",
-        dest="httpseeds",
-        metavar="<url>",
-        nargs="+",
-        help="replace all currently listed addresses with new list (Hoffman).",
-    )
-
-    edit_parser.add_argument(
-        "--private",
-        action="store_true",
-        help="Make torrent private.",
-        dest="private",
-    )
-
-    edit_parser.add_argument(
-        "--comment",
-        help="Replaces any existing comment with <comment>",
-        metavar="<comment>",
-        dest="comment",
-        action="store",
-    )
-
-    edit_parser.add_argument(
-        "--source",
-        action="store",
-        dest="source",
-        metavar="<source>",
-        help="Replaces current source with <source>",
-    )
-
-    edit_parser.set_defaults(func=edit)
-
-    info_parser = subparsers.add_parser(
-        "info",
-        help="Show detailed information about a torrent file.",
-        aliases=["i"],
-        prefix_chars="-",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    info_parser.add_argument(
-        "metafile",
-        action="store",
-        metavar="<*.torrent>",
-        help="path to pre-existing torrent file.",
-    )
-
-    info_parser.set_defaults(func=info)
-
-    magnet_parser = subparsers.add_parser(
-        "magnet",
-        help="Generate magnet url from an existing Bittorrent meta file.",
-        aliases=["m"],
-        prefix_chars="-",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    magnet_parser.add_argument(
-        "metafile",
-        action="store",
-        help="Path to Bittorrent meta file.",
-        metavar="<*.torrent>",
-    )
-
-    magnet_parser.set_defaults(func=magnet)
-
-    check_parser = subparsers.add_parser(
-        "recheck",
-        help="Gives a detailed look at how much of the torrent is available.",
-        aliases=["check", "r"],
-        prefix_chars="-",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    check_parser.add_argument(
-        "metafile",
-        action="store",
-        metavar="<*.torrent>",
-        help="path to .torrent file.",
-    )
-
-    check_parser.add_argument(
-        "content",
-        action="store",
-        metavar="<content>",
-        help="path to content file or directory",
-    )
-
-    check_parser.set_defaults(func=recheck)
-
-    rebuild_parser = subparsers.add_parser(
-        "rebuild",
-        help="""Re-assemble files obtained from a bittorrent file into the
-                appropriate file structure for re-seeding.  Read documentation
-                for more information, or use cases.""",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    rebuild_parser.add_argument(
-        "-m",
-        "--metafiles",
-        action="store",
-        metavar="<*.torrent>",
-        nargs="+",
-        dest="metafiles",
-        required=True,
-        help="path(s) to .torrent file(s)/folder(s) containing .torrent files",
-    )
-
-    rebuild_parser.add_argument(
-        "-c" "--contents",
-        action="store",
-        dest="contents",
-        nargs="+",
-        required=True,
-        metavar="<contents>",
-        help="folders that might contain the source contents needed to rebuld",
-    )
-
-    rebuild_parser.add_argument(
-        "-d",
-        "--destination",
-        action="store",
-        dest="destination",
-        required=True,
-        metavar="<destination>",
-        help="path to where torrents will be re-assembled",
-    )
-
-    rebuild_parser.set_defaults(func=rebuild)
-
-    rename_parser = subparsers.add_parser(
-        "rename",
-        help="""Rename a torrent file to it's original name provided in the
-                metadata/the same name you see in your torrent client.""",
-        formatter_class=TorrentFileHelpFormatter,
-    )
-
-    rename_parser.add_argument(
-        "target",
-        action="store",
-        metavar="<target>",
-        help="path to file that needs renaming.",
-    )
-
-    rename_parser.set_defaults(func=rename)
-
-    all_commands = [
-        "create",
-        "new",
-        "c",
-        "edit",
-        "e",
-        "info",
-        "i",
-        "magnet",
-        "m",
-        "recheck",
-        "check",
-        "r",
-        "rename",
-        "rebuild",
-        "-i",
-        "-h",
-        "-V",
-    ]
-    if not any(i for i in all_commands if i in args):
-        start = 0
-        while args[start] in ["-v", "-q"]:
-            start += 1
-        args.insert(start, "create")
-
-    args = parser.parse_args(args)
-
-    if args.quiet:
-        Config.activate_quiet()
-
-    elif args.debug:
-        Config.activate_logger()
-
-    if args.interactive:
-        return select_action()
-
-    if hasattr(args, "func"):
-        return args.func(args)
-    return args  # pragma: nocover
-
-
-main_script = execute
-
-
-def main():
-    """
-    Initiate main function for CLI script.
-    """
-    execute()
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Command Line Interface for TorrentFile project.
+
+This module provides the primary command line argument parser for
+the torrentfile package. The main_script function is automatically
+invoked when called from command line, and parses accompanying arguments.
+
+Functions
+---------
+main_script :
+    process command line arguments and run program.
+activate_logger :
+    turns on debug mode and logging facility.
+
+Classes
+-------
+Config : class
+    controls logging configuration
+TorrentFileHelpFormatter : HelpFormatter
+    the command line help message formatter
+"""
+
+import io
+import logging
+import sys
+from argparse import ArgumentParser, HelpFormatter
+
+from torrentfile.commands import (create, edit, info, magnet, rebuild, recheck,
+                                  rename)
+from torrentfile.utils import toggle_debug_mode
+from torrentfile.version import __version__ as version
+
+
+class Config:
+    """
+    Class the controls the logging configuration and output settings.
+
+    Controls the logging level, or whether to app should operate in quiet mode.
+    """
+
+    @staticmethod
+    def activate_quiet():
+        """
+        Activate quiet mode for the duration of the programs life.
+
+        When quiet mode is enabled, no logging, progress or state information
+        is output to the terminal
+        """
+        if sys.stdout or sys.stderr:
+            sys.stdout = io.StringIO()
+            sys.stderr = io.StringIO()
+
+    @staticmethod
+    def activate_logger():
+        """
+        Activate the builtin logging mechanism when passed debug flag from CLI.
+        """
+        logging.basicConfig(level=logging.WARNING)
+        logger = logging.getLogger()
+        console_handler = logging.StreamHandler(stream=sys.stderr)
+        stream_formatter = logging.Formatter(
+            "[%(asctime)s] [%(levelno)s] %(message)s",
+            datefmt="%H:%M:%S",
+            style="%",
+        )
+        console_handler.setFormatter(stream_formatter)
+        console_handler.setLevel(logging.DEBUG)
+        logger.setLevel(logging.DEBUG)
+        logger.addHandler(console_handler)
+        logger.debug("Debug: ON")
+        toggle_debug_mode(True)
+
+
+class TorrentFileHelpFormatter(HelpFormatter):
+    """
+    Formatting class for help tips provided by the CLI.
+
+    Subclasses Argparse.HelpFormatter.
+    """
+
+    def __init__(self, prog, width=45, max_help_positions=45):
+        """
+        Construct HelpFormat class for usage output.
+
+        Parameters
+        ----------
+        prog : str
+            Name of the program.
+        width : int
+            Max width of help message output.
+        max_help_positions : int
+            max length until line wrap.
+        """
+        super().__init__(
+            prog, width=width, max_help_position=max_help_positions
+        )
+
+    def _split_lines(self, text: str, _: int) -> list:
+        """
+        Split multiline help messages and remove indentation.
+
+        Parameters
+        ----------
+        text : str
+            text that needs to be split
+        _ : int
+            max width for line.
+
+        Returns
+        -------
+        list :
+            split into multiline text list
+        """
+        lines = text.split("\n")
+        return [line.strip() for line in lines if line]
+
+    def _format_text(self, text: str) -> str:
+        """
+        Format text for cli usage messages.
+
+        Parameters
+        ----------
+        text : str
+            Pre-formatted text.
+
+        Returns
+        -------
+        str
+            Formatted text from input.
+        """
+        text = text % {"prog": self._prog} if "%(prog)" in text else text
+        text = self._whitespace_matcher.sub(" ", text).strip()
+        return text + "\n\n"
+
+    def _join_parts(self, part_strings: list) -> str:
+        """
+        Combine different sections of the help message.
+
+        Parameters
+        ----------
+        part_strings : list
+            List of argument help messages and headers.
+
+        Returns
+        -------
+        str
+            Fully formatted help message for CLI.
+        """
+        parts = self._format_headers(part_strings)
+        return super()._join_parts(parts)
+
+    @staticmethod
+    def _format_headers(parts: list) -> list:
+        """
+        Format help message section headers.
+
+        Parameters
+        ----------
+        parts : list
+            List of individual lines for help message.
+
+        Returns
+        -------
+        list
+            Input list with formatted section headers.
+        """
+        if parts and parts[0].startswith("usage:"):
+            parts[0] = "Usage\n=====\n  " + parts[0][6:]
+        headings = [i for i in range(len(parts)) if parts[i].endswith(":\n")]
+        for i in headings[::-1]:
+            parts[i] = parts[i][:-2].title()
+            underline = "".join(["\n", "-" * len(parts[i]), "\n"])
+            parts.insert(i + 1, underline)
+        return parts
+
+
+def execute(args: list = None) -> list:
+    """
+    Execute program with provided list of arguments.
+
+    If no arguments are given then it defaults to using
+    sys.argv.  This is the main entrypoint for the program
+    and command line interface.
+
+    Parameters
+    ----------
+    args : list
+        Commandline arguments. default=None
+
+    Returns
+    -------
+    list
+        Depends on what the command line args were.
+    """
+    toggle_debug_mode(False)
+    if not args:
+        if sys.argv[1:]:
+            args = sys.argv[1:]
+        else:
+            args = ["-h"]
+
+    parser = ArgumentParser(
+        "torrentfile",
+        usage="torrentfile <options>",
+        description=(
+            "Command line tools for creating, editing, checking, building "
+            "and interacting with Bittorrent metainfo files"
+        ),
+        prefix_chars="-",
+        formatter_class=TorrentFileHelpFormatter,
+        conflict_handler="resolve",
+    )
+
+    parser.add_argument(
+        "-q",
+        "--quiet",
+        help="Turn off all text output.",
+        dest="quiet",
+        action="store_true",
+    )
+
+    parser.add_argument(
+        "-V",
+        "--version",
+        action="version",
+        version=f"torrentfile v{version}",
+        help="show program version and exit",
+    )
+
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        dest="debug",
+        help="output debug information",
+    )
+
+    parser.set_defaults(func=parser.print_help)
+
+    subparsers = parser.add_subparsers(
+        title="Commands",
+        dest="command",
+        metavar="create, edit, info, magnet, recheck, rebuild, rename\n",
+    )
+
+    create_parser = subparsers.add_parser(
+        "create",
+        help="Create a new Bittorrent file.",
+        prefix_chars="-",
+        aliases=["c", "new"],
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    create_parser.add_argument(
+        "-a",
+        "-t",
+        "--announce",
+        "--tracker",
+        action="store",
+        dest="announce",
+        metavar="<url>",
+        nargs="+",
+        default=[],
+        help="One or more space-seperated torrent tracker url(s).",
+    )
+
+    create_parser.add_argument(
+        "-p",
+        "--private",
+        action="store_true",
+        dest="private",
+        help="Creates private torrent with multi-tracker and DHT turned off.",
+    )
+
+    create_parser.add_argument(
+        "-s",
+        "--source",
+        action="store",
+        dest="source",
+        metavar="<source>",
+        help="Add a source string. Useful for cross-seeding.",
+    )
+
+    create_parser.add_argument(
+        "-f",
+        "--config",
+        action="store_true",
+        dest="config",
+        help="""
+        Parse torrent information from a config file. Looks in the current
+        working directory, or the directory named .torrentfile in the users
+        home directory for a torrentfile.ini file. You can also use this
+        option in combination with the --config-path to specify the path to
+        the config file. See documentation for details on properly formatting
+        config file.
+        """,
+    )
+
+    create_parser.add_argument(
+        "--config-path",
+        action="store",
+        metavar="<path>",
+        dest="config_path",
+        help="""
+        Use this option in combination with -f or --config
+        options to specify location of config file.
+        """,
+    )
+
+    create_parser.add_argument(
+        "-m",
+        "--magnet",
+        action="store_true",
+        dest="magnet",
+    )
+
+    create_parser.add_argument(
+        "-c",
+        "--comment",
+        action="store",
+        dest="comment",
+        metavar="<comment>",
+        help="Include a comment in file metadata",
+    )
+
+    create_parser.add_argument(
+        "-o",
+        "--out",
+        action="store",
+        dest="outfile",
+        metavar="<path>",
+        help="Explicitly specify the path to write the file.",
+    )
+
+    create_parser.add_argument(
+        "--cwd",
+        "--current",
+        action="store_true",
+        dest="cwd",
+        help="*deprecated* Saving to current directory is default behaviour",
+    )
+
+    create_parser.add_argument(
+        "--prog",
+        "--progress",
+        default="1",
+        action="store",
+        dest="progress",
+        help="""
+        Set the progress bar level.
+        Options = 0, 1
+        (0) = Do not display progress bar.
+        (1) = Display progress bar.(default)
+        """,
+    )
+
+    create_parser.add_argument(
+        "--meta-version",
+        default="1",
+        choices=["1", "2", "3"],
+        action="store",
+        dest="meta_version",
+        metavar="<int>",
+        help="""
+        Bittorrent metafile version.
+        Options = 1, 2, 3
+        (1) = Bittorrent v1 (Default)
+        (2) = Bittorrent v2
+        (3) = Bittorrent v1 & v2 hybrid
+        """,
+    )
+
+    create_parser.add_argument(
+        "--piece-length",
+        action="store",
+        dest="piece_length",
+        metavar="<int>",
+        help="""
+        (Default: auto calculated based on total size of content) Number of
+        bytes for per chunk of data transmitted by Bittorrent client.
+        Acceptable values include integers 14-26 which will be interpreted
+        as exponent for power of 2.  e.g. 14 = 16KiB pieces.
+        Examples:: [--piece-length 14] [--piece-length 20]
+        """,
+    )
+
+    create_parser.add_argument(
+        "-w",
+        "--web-seed",
+        action="store",
+        dest="url_list",
+        metavar="<url>",
+        nargs="+",
+        help="list of web addresses where torrent data exists (GetRight).",
+    )
+
+    create_parser.add_argument(
+        "--http-seed",
+        action="store",
+        dest="httpseeds",
+        metavar="<url>",
+        nargs="+",
+        help="list of URLs, addresses where content can be found (Hoffman).",
+    )
+
+    create_parser.add_argument(
+        "content",
+        action="store",
+        metavar="<content>",
+        nargs="?",
+        help="Path to content file or directory",
+    )
+
+    create_parser.set_defaults(func=create)
+
+    edit_parser = subparsers.add_parser(
+        "edit",
+        help="""Edit existing torrent meta file.""",
+        aliases=["e"],
+        prefix_chars="-",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    edit_parser.add_argument(
+        "metafile",
+        action="store",
+        help="path to *.torrent file",
+        metavar="<*.torrent>",
+    )
+
+    edit_parser.add_argument(
+        "--tracker",
+        action="store",
+        dest="announce",
+        metavar="<url>",
+        nargs="+",
+        help="""
+        Replace current list of tracker/announce urls with one or more space
+        seperated Bittorrent tracker announce url(s).
+        """,
+    )
+
+    edit_parser.add_argument(
+        "--web-seed",
+        action="store",
+        dest="url_list",
+        metavar="<url>",
+        nargs="+",
+        help="Replace current list of web-seed urls with one or more url(s)",
+    )
+
+    edit_parser.add_argument(
+        "--http-seed",
+        action="store",
+        dest="httpseeds",
+        metavar="<url>",
+        nargs="+",
+        help="replace all currently listed addresses with new list (Hoffman).",
+    )
+
+    edit_parser.add_argument(
+        "--private",
+        action="store_true",
+        help="Make torrent private.",
+        dest="private",
+    )
+
+    edit_parser.add_argument(
+        "--comment",
+        help="Replaces any existing comment with <comment>",
+        metavar="<comment>",
+        dest="comment",
+        action="store",
+    )
+
+    edit_parser.add_argument(
+        "--source",
+        action="store",
+        dest="source",
+        metavar="<source>",
+        help="Replaces current source with <source>",
+    )
+
+    edit_parser.set_defaults(func=edit)
+
+    info_parser = subparsers.add_parser(
+        "info",
+        help="Show detailed information about a torrent file.",
+        aliases=["i"],
+        prefix_chars="-",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    info_parser.add_argument(
+        "metafile",
+        action="store",
+        metavar="<*.torrent>",
+        help="path to pre-existing torrent file.",
+    )
+
+    info_parser.set_defaults(func=info)
+
+    magnet_parser = subparsers.add_parser(
+        "magnet",
+        help="Generate magnet url from an existing Bittorrent meta file.",
+        aliases=["m"],
+        prefix_chars="-",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    magnet_parser.add_argument(
+        "metafile",
+        action="store",
+        help="Path to Bittorrent meta file.",
+        metavar="<*.torrent>",
+    )
+
+    magnet_parser.set_defaults(func=magnet)
+
+    check_parser = subparsers.add_parser(
+        "recheck",
+        help="Gives a detailed look at how much of the torrent is available.",
+        aliases=["check", "r"],
+        prefix_chars="-",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    check_parser.add_argument(
+        "metafile",
+        action="store",
+        metavar="<*.torrent>",
+        help="path to .torrent file.",
+    )
+
+    check_parser.add_argument(
+        "content",
+        action="store",
+        metavar="<content>",
+        help="path to content file or directory",
+    )
+
+    check_parser.set_defaults(func=recheck)
+
+    rebuild_parser = subparsers.add_parser(
+        "rebuild",
+        help="""Re-assemble files obtained from a bittorrent file into the
+                appropriate file structure for re-seeding.  Read documentation
+                for more information, or use cases.""",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    rebuild_parser.add_argument(
+        "-m",
+        "--metafiles",
+        action="store",
+        metavar="<*.torrent>",
+        nargs="+",
+        dest="metafiles",
+        required=True,
+        help="path(s) to .torrent file(s)/folder(s) containing .torrent files",
+    )
+
+    rebuild_parser.add_argument(
+        "-c" "--contents",
+        action="store",
+        dest="contents",
+        nargs="+",
+        required=True,
+        metavar="<contents>",
+        help="folders that might contain the source contents needed to rebuld",
+    )
+
+    rebuild_parser.add_argument(
+        "-d",
+        "--destination",
+        action="store",
+        dest="destination",
+        required=True,
+        metavar="<destination>",
+        help="path to where torrents will be re-assembled",
+    )
+
+    rebuild_parser.set_defaults(func=rebuild)
+
+    rename_parser = subparsers.add_parser(
+        "rename",
+        help="""Rename a torrent file to it's original name provided in the
+                metadata/the same name you see in your torrent client.""",
+        formatter_class=TorrentFileHelpFormatter,
+    )
+
+    rename_parser.add_argument(
+        "target",
+        action="store",
+        metavar="<target>",
+        help="path to file that needs renaming.",
+    )
+
+    rename_parser.set_defaults(func=rename)
+
+    all_commands = [
+        "create",
+        "new",
+        "c",
+        "edit",
+        "e",
+        "info",
+        "i",
+        "magnet",
+        "m",
+        "recheck",
+        "check",
+        "r",
+        "rename",
+        "rebuild",
+        "-i",
+        "-h",
+        "-V",
+    ]
+    if not any(i for i in all_commands if i in args):
+        start = 0
+        while args[start] in ["-v", "-q"]:
+            start += 1
+        args.insert(start, "create")
+
+    args = parser.parse_args(args)
+
+    if args.quiet:
+        Config.activate_quiet()
+
+    elif args.debug:
+        Config.activate_logger()
+
+    if hasattr(args, "func"):
+        return args.func(args)
+    return args  # pragma: nocover
+
+
+main_script = execute
+
+
+def main():
+    """
+    Initiate main function for CLI script.
+    """
+    execute()
```

### Comparing `torrentfile-0.8.7/torrentfile/edit.py` & `torrentfile-0.8.8/torrentfile/edit.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Edit torrent module.
-
-Provides a facility by which certain properties of a torrent meta file can be
-edited by the user. The various command line arguments indicate which fields
-should be edited, and what the new value should be.  Depending on what fields
-are chosen to edit, this command can trigger a new info hash which means the
-torrent will no longer be able to participate in the same swarm as the original
-unedited torrent.
-
-Keywords
---------
-private
-comment
-source
-trackers
-web-seeds
-"""
-
-import logging
-import os
-
-import pyben
-
-logger = logging.getLogger(__name__)
-
-
-def filter_empty(args: dict, meta: dict, info: dict):
-    """
-    Remove the fields that were not used by the original file creator.
-
-    Parameters
-    ----------
-    args : dict
-        Editable metafile properties from user.
-    meta : dict
-        Metafile data dictionary.
-    info : dict
-        Metafile info dictionary.
-    """
-    for key, val in list(args.items()):
-        if val is None:
-            del args[key]
-            continue
-
-        if val == "":
-            if key in meta:
-                del meta[key]
-            elif key in info:
-                del info[key]
-            del args[key]
-            logger.debug("removeing empty fields %s", val)
-
-
-def edit_torrent(metafile: str, args: dict) -> dict:
-    """
-    Edit the properties and values in a torrent meta file.
-
-    Parameters
-    ----------
-    metafile : str
-        path to the torrent meta file.
-    args : dict
-        key value pairs of the properties to be edited.
-
-    Returns
-    -------
-    dict
-        The edited and nested Meta and info dictionaries.
-    """
-    logger.debug("editing torrent file %s", metafile)
-    meta = pyben.load(metafile)
-    info = meta["info"]
-    filter_empty(args, meta, info)
-
-    if "comment" in args:
-        info["comment"] = args["comment"]
-
-    if "source" in args:
-        info["source"] = args["source"]
-
-    if "private" in args:
-        info["private"] = 1
-
-    if "announce" in args:
-        val = args.get("announce", None)
-        if isinstance(val, str):
-            vallist = val.split()
-            meta["announce"] = vallist[0]
-            meta["announce-list"] = [vallist]
-        elif isinstance(val, list):
-            meta["announce"] = val[0]
-            meta["announce-list"] = [val]
-
-    if "url-list" in args:
-        val = args.get("url-list")
-        if isinstance(val, str):
-            meta["url-list"] = val.split()
-        elif isinstance(val, list):
-            meta["url-list"] = val
-
-    if "httpseeds" in args:
-        val = args.get("httpseeds")
-        if isinstance(val, str):
-            meta["httpseeds"] = val.split()
-        elif isinstance(val, list):
-            meta["httpseeds"] = val
-
-    meta["info"] = info
-    os.remove(metafile)
-    pyben.dump(meta, metafile)
-    return meta
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Edit torrent module.
+
+Provides a facility by which certain properties of a torrent meta file can be
+edited by the user. The various command line arguments indicate which fields
+should be edited, and what the new value should be.  Depending on what fields
+are chosen to edit, this command can trigger a new info hash which means the
+torrent will no longer be able to participate in the same swarm as the original
+unedited torrent.
+
+Keywords
+--------
+private
+comment
+source
+trackers
+web-seeds
+"""
+
+import logging
+import os
+
+import pyben
+
+logger = logging.getLogger(__name__)
+
+
+def filter_empty(args: dict, meta: dict, info: dict):
+    """
+    Remove the fields that were not used by the original file creator.
+
+    Parameters
+    ----------
+    args : dict
+        Editable metafile properties from user.
+    meta : dict
+        Metafile data dictionary.
+    info : dict
+        Metafile info dictionary.
+    """
+    for key, val in list(args.items()):
+        if val is None:
+            del args[key]
+            continue
+
+        if val == "":
+            if key in meta:
+                del meta[key]
+            elif key in info:
+                del info[key]
+            del args[key]
+            logger.debug("removeing empty fields %s", val)
+
+
+def edit_torrent(metafile: str, args: dict) -> dict:
+    """
+    Edit the properties and values in a torrent meta file.
+
+    Parameters
+    ----------
+    metafile : str
+        path to the torrent meta file.
+    args : dict
+        key value pairs of the properties to be edited.
+
+    Returns
+    -------
+    dict
+        The edited and nested Meta and info dictionaries.
+    """
+    logger.debug("editing torrent file %s", metafile)
+    meta = pyben.load(metafile)
+    info = meta["info"]
+    filter_empty(args, meta, info)
+
+    if "comment" in args:
+        info["comment"] = args["comment"]
+
+    if "source" in args:
+        info["source"] = args["source"]
+
+    if "private" in args:
+        info["private"] = 1
+
+    if "announce" in args:
+        val = args.get("announce", None)
+        if isinstance(val, str):
+            vallist = val.split()
+            meta["announce"] = vallist[0]
+            meta["announce-list"] = [vallist]
+        elif isinstance(val, list):
+            meta["announce"] = val[0]
+            meta["announce-list"] = [val]
+
+    if "url-list" in args:
+        val = args.get("url-list")
+        if isinstance(val, str):
+            meta["url-list"] = val.split()
+        elif isinstance(val, list):
+            meta["url-list"] = val
+
+    if "httpseeds" in args:
+        val = args.get("httpseeds")
+        if isinstance(val, str):
+            meta["httpseeds"] = val.split()
+        elif isinstance(val, list):
+            meta["httpseeds"] = val
+
+    meta["info"] = info
+    os.remove(metafile)
+    pyben.dump(meta, metafile)
+    return meta
```

### Comparing `torrentfile-0.8.7/torrentfile/hasher.py` & `torrentfile-0.8.8/torrentfile/hasher.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,534 +1,534 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Piece/File Hashers for Bittorrent meta file contents.
-"""
-
-import logging
-import os
-from hashlib import sha1, sha256  # nosec
-
-from torrentfile.mixins import CbMixin, ProgMixin
-from torrentfile.utils import next_power_2
-
-BLOCK_SIZE = 2**14  # 16KiB
-HASH_SIZE = 32
-
-logger = logging.getLogger(__name__)
-
-
-class Hasher(CbMixin, ProgMixin):
-    """
-    Piece hasher for Bittorrent V1 files.
-
-    Takes a sorted list of all file paths, calculates sha1 hash
-    for fixed size pieces of file data from each file
-    seemlessly until the last piece which may be smaller than others.
-
-    Parameters
-    ----------
-    paths : list
-        List of files.
-    piece_length : int
-        Size of chuncks to split the data into.
-    progress : int
-        default = None
-    """
-
-    def __init__(self, paths: list, piece_length: int, progress: bool = True):
-        """Generate hashes of piece length data from filelist contents."""
-        self.piece_length = piece_length
-        self.paths = paths
-        self.progress = progress
-        self.total = sum(os.path.getsize(i) for i in self.paths)
-        self.index = 0
-        self.current = open(self.paths[0], "rb")
-        if self.progress:
-            total = os.path.getsize(self.paths[0])
-            self.prog_start(total, self.paths[0], unit="bytes")
-        logger.debug("Hashing %s", str(self.paths[0]))
-
-    def __iter__(self):
-        """
-        Iterate through feed pieces.
-
-        Returns
-        -------
-        self : iterator
-            Iterator for leaves/hash pieces.
-        """
-        return self
-
-    def _handle_partial(self, arr: bytearray) -> bytearray:
-        """
-        Define the handling partial pieces that span 2 or more files.
-
-        Parameters
-        ----------
-        arr : bytearray
-            Incomplete piece containing partial data
-
-        Returns
-        -------
-        digest : bytearray
-            SHA1 digest of the complete piece.
-        """
-        while len(arr) < self.piece_length and self.next_file():
-            target = self.piece_length - len(arr)
-            temp = bytearray(target)
-            size = self.current.readinto(temp)
-            arr.extend(temp[:size])
-            self.prog_update(size)
-            if size == target:
-                break
-        return sha1(arr).digest()  # nosec
-
-    def next_file(self) -> bool:
-        """
-        Seemlessly transition to next file in file list.
-
-        Returns
-        -------
-        bool:
-            True if there is a next file otherwise False.
-        """
-        self.index += 1
-        self.prog_close()
-        if self.index < len(self.paths):
-            path = self.paths[self.index]
-            logger.debug("Hashing %s", str(path))
-            self.current.close()
-            if self.progress:
-                self.prog_start(os.path.getsize(path), path, unit="bytes")
-            self.current = open(path, "rb")
-            return True
-        return False
-
-    def __next__(self) -> bytes:
-        """
-        Generate piece-length pieces of data from input file list.
-
-        Returns
-        -------
-        bytes
-            SHA1 hash of the piece extracted.
-        """
-        while True:
-            piece = bytearray(self.piece_length)
-            size = self.current.readinto(piece)
-            if size == 0:
-                if not self.next_file():
-                    raise StopIteration
-            elif size < self.piece_length:
-                self.prog_update(size)
-                return self._handle_partial(piece[:size])
-            else:
-                self.prog_update(size)
-                return sha1(piece).digest()  # nosec
-
-
-def merkle_root(blocks: list) -> bytes:
-    """
-    Calculate the merkle root for a seq of sha256 hash digests.
-
-    Parameters
-    ----------
-    blocks : list
-        a sequence of sha256 layer hashes.
-
-    Returns
-    -------
-    bytes
-        the sha256 root hash of the merkle tree.
-    """
-    if blocks:
-        while len(blocks) > 1:
-            blocks = [
-                sha256(x + y).digest() for x, y in zip(*[iter(blocks)] * 2)
-            ]
-        return blocks[0]
-    return blocks
-
-
-class HasherV2(CbMixin, ProgMixin):
-    """
-    Calculate the root hash and piece layers for file contents.
-
-    **DEPRECATED**
-
-    Iterates over 16KiB blocks of data from given file, hashes the data,
-    then creates a hash tree from the individual block hashes until size of
-    hashed data equals the piece-length.  Then continues the hash tree until
-    root hash is calculated.
-
-    Parameters
-    ----------
-    path : str
-        Path to file.
-    piece_length : int
-        Size of layer hashes pieces.
-    progress : int
-        default = None
-    """
-
-    def __init__(self, path: str, piece_length: int, progress: bool = True):
-        """
-        Calculate and store hash information for specific file.
-
-        **DEPRECATED**
-        """
-        self.path = path
-        self.root = None
-        self.piece_layer = None
-        self.layer_hashes = []
-        self.piece_length = piece_length
-        self.num_blocks = piece_length // BLOCK_SIZE
-        if progress:
-            self.prog_start(os.path.getsize(path), path, unit="bytes")
-        with open(self.path, "rb") as fd:
-            self.process_file(fd)
-
-    def process_file(self, fd: str):
-        """
-        Calculate hashes over 16KiB chuncks of file content.
-
-        **DEPRECATED**
-
-        Parameters
-        ----------
-        fd : TextIOWrapper
-            Opened file in read mode.
-        """
-        while True:
-            blocks = []
-            leaf = bytearray(BLOCK_SIZE)
-            # generate leaves of merkle tree
-
-            for _ in range(self.num_blocks):
-                size = fd.readinto(leaf)
-                self.prog_update(size)
-                if not size:
-                    break
-                blocks.append(sha256(leaf[:size]).digest())
-
-            # blocks is empty mean eof
-            if not blocks:
-                break
-            if len(blocks) != self.num_blocks:
-                # when size of file doesn't fill the last block
-                # when the file contains multiple pieces
-                remaining = self.num_blocks - len(blocks)
-                if not self.layer_hashes:
-                    # when the there is only one block for file
-                    power2 = next_power_2(len(blocks))
-                    remaining = power2 - len(blocks)
-
-                # pad the the rest with zeroes to fill remaining space.
-                padding = [bytes(32) for _ in range(remaining)]
-                self.prog_update(HASH_SIZE * remaining)
-                blocks.extend(padding)
-            # calculate the root hash for the merkle tree up to piece-length
-
-            layer_hash = merkle_root(blocks)
-            self.cb(layer_hash)
-            self.layer_hashes.append(layer_hash)
-        self._calculate_root()
-        self.prog_close()
-
-    def _calculate_root(self):
-        """
-        Calculate root hash for the target file.
-
-        **DEPRECATED**
-        """
-        self.piece_layer = b"".join(self.layer_hashes)
-        hashes = len(self.layer_hashes)
-        if hashes > 1:
-            pow2 = next_power_2(hashes)
-            remainder = pow2 - hashes
-            pad_piece = [bytes(HASH_SIZE) for _ in range(self.num_blocks)]
-            for _ in range(remainder):
-                self.layer_hashes.append(merkle_root(pad_piece))
-        self.root = merkle_root(self.layer_hashes)
-
-
-class HasherHybrid(CbMixin, ProgMixin):
-    """
-    Calculate root and piece hashes for creating hybrid torrent file.
-
-    **DEPRECATED**
-
-    Create merkle tree layers from sha256 hashed 16KiB blocks of contents.
-    With a branching factor of 2, merge layer hashes until blocks equal
-    piece_length bytes for the piece layer, and then the root hash.
-
-    Parameters
-    ----------
-    path : str
-        path to target file.
-    piece_length : int
-        piece length for data chunks.
-    progress : int
-        default = None
-    """
-
-    def __init__(self, path: str, piece_length: int, progress: bool = True):
-        """
-        Construct Hasher class instances for each file in torrent.
-
-        **DEPRECATED**
-        """
-        self.path = path
-        self.piece_length = piece_length
-        self.pieces = []
-        self.layer_hashes = []
-        self.piece_layer = None
-        self.root = None
-        self.padding_piece = None
-        self.padding_file = None
-        if progress:
-            self.prog_start(os.path.getsize(path), path, unit="bytes")
-        self.amount = piece_length // BLOCK_SIZE
-        with open(path, "rb") as data:
-            self.process_file(data)
-
-    def _pad_remaining(self, block_count: int):
-        """
-        Generate Hash sized, 0 filled bytes for padding.
-
-        **DEPRECATED**
-
-        Parameters
-        ----------
-        block_count : int
-            current total number of blocks collected.
-
-        Returns
-        -------
-        padding : bytes
-            Padding to fill remaining portion of tree.
-        """
-        # when the there is only one block for file
-        remaining = self.amount - block_count
-        if not self.layer_hashes:
-            power2 = next_power_2(block_count)
-            remaining = power2 - block_count
-        self.prog_update(HASH_SIZE * remaining)
-        return [bytes(HASH_SIZE) for _ in range(remaining)]
-
-    def process_file(self, data: bytearray):
-        """
-        Calculate layer hashes for contents of file.
-
-        **DEPRECATED**
-
-        Parameters
-        ----------
-        data : BytesIO
-            File opened in read mode.
-        """
-        while True:
-            plength = self.piece_length
-            blocks = []
-            piece = sha1()  # nosec
-            total = 0
-            block = bytearray(BLOCK_SIZE)
-            for _ in range(self.amount):
-                size = data.readinto(block)
-                self.prog_update(size)
-                if not size:
-                    break
-                total += size
-                plength -= size
-                blocks.append(sha256(block[:size]).digest())
-                piece.update(block[:size])
-            if not blocks:
-                break
-            if len(blocks) != self.amount:
-                padding = self._pad_remaining(len(blocks))
-                blocks.extend(padding)
-            layer_hash = merkle_root(blocks)
-            self.cb(layer_hash)
-            self.layer_hashes.append(layer_hash)
-            if plength > 0:
-                self.padding_file = {
-                    "attr": "p",
-                    "length": plength,
-                    "path": [".pad", str(plength)],
-                }
-                piece.update(bytes(plength))
-            self.pieces.append(piece.digest())  # nosec
-        self._calculate_root()
-        self.prog_close()
-
-    def _calculate_root(self):
-        """
-        Calculate the root hash for opened file.
-
-        **DEPRECATED**
-        """
-        self.piece_layer = b"".join(self.layer_hashes)
-
-        if len(self.layer_hashes) > 1:
-            pad_piece = merkle_root([bytes(32) for _ in range(self.amount)])
-
-            pow2 = next_power_2(len(self.layer_hashes))
-            remainder = pow2 - len(self.layer_hashes)
-
-            self.layer_hashes += [pad_piece for _ in range(remainder)]
-        self.root = merkle_root(self.layer_hashes)
-
-
-class FileHasher(CbMixin, ProgMixin):
-    """
-    Calculate root and piece hashes for creating hybrid torrent file.
-
-    Create merkle tree layers from sha256 hashed 16KiB blocks of contents.
-    With a branching factor of 2, merge layer hashes until blocks equal
-    piece_length bytes for the piece layer, and then the root hash.
-
-    Parameters
-    ----------
-    path : str
-        path to target file.
-    piece_length : int
-        piece length for data chunks.
-    progress : int
-        default = None
-    """
-
-    def __init__(
-        self,
-        path: str,
-        piece_length: int,
-        progress: bool = True,
-        hybrid: bool = False,
-    ):
-        """
-        Construct Hasher class instances for each file in torrent.
-        """
-        self.path = path
-        self.piece_length = piece_length
-        self.pieces = []
-        self.layer_hashes = []
-        self.piece_layer = None
-        self.root = None
-        self.padding_piece = None
-        self.padding_file = None
-        self.amount = piece_length // BLOCK_SIZE
-        self.end = False
-        self.current = open(path, "rb")
-        self.hybrid = hybrid
-        if progress:
-            self.progressbar = True
-            self.prog_start(os.path.getsize(path), path, unit="bytes")
-
-    def __iter__(self):
-        """Return `self`: needed to implement iterator implementation."""
-        return self
-
-    def _pad_remaining(self, block_count: int):
-        """
-        Generate Hash sized, 0 filled bytes for padding.
-
-        Parameters
-        ----------
-        block_count : int
-            current total number of blocks collected.
-
-        Returns
-        -------
-        padding : bytes
-            Padding to fill remaining portion of tree.
-        """
-        # when the there is only one block for file
-        remaining = self.amount - block_count
-        if not self.layer_hashes:
-            power2 = next_power_2(block_count)
-            remaining = power2 - block_count
-        return [bytes(HASH_SIZE) for _ in range(remaining)]
-
-    def __next__(self) -> bytes:
-        """
-        Calculate layer hashes for contents of file.
-
-        Returns
-        -------
-        bytes
-            The layer merckle root hash.
-        """
-        if self.end:
-            self.end = False
-            raise StopIteration
-        plength = self.piece_length
-        blocks = []
-        piece = sha1()  # nosec
-        total = 0
-        block = bytearray(BLOCK_SIZE)
-        for _ in range(self.amount):
-            size = self.current.readinto(block)
-            if not size:
-                self.end = True
-                break
-            total += size
-            plength -= size
-            blocks.append(sha256(block[:size]).digest())
-            if self.hybrid:
-                piece.update(block[:size])
-        if not blocks:
-            self._calculate_root()
-            raise StopIteration
-        if len(blocks) != self.amount:
-            padding = self._pad_remaining(len(blocks))
-            blocks.extend(padding)
-        self.prog_update(total)
-        layer_hash = merkle_root(blocks)
-        self.layer_hashes.append(layer_hash)
-        self.cb(layer_hash)
-        if self.end:
-            self._calculate_root()
-            self.prog_close()
-        if self.hybrid:
-            if plength > 0:
-                self.padding_file = {
-                    "attr": "p",
-                    "length": plength,
-                    "path": [".pad", str(plength)],
-                }
-                piece.update(bytes(plength))
-            piece = piece.digest()
-            self.pieces.append(piece)
-            return layer_hash, piece
-        return layer_hash
-
-    def _calculate_root(self):
-        """
-        Calculate the root hash for opened file.
-        """
-        self.piece_layer = b"".join(self.layer_hashes)
-
-        if len(self.layer_hashes) > 1:
-            pad_piece = merkle_root([bytes(32) for _ in range(self.amount)])
-
-            pow2 = next_power_2(len(self.layer_hashes))
-            remainder = pow2 - len(self.layer_hashes)
-
-            self.layer_hashes += [pad_piece for _ in range(remainder)]
-        self.root = merkle_root(self.layer_hashes)
-        self.current.close()
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Piece/File Hashers for Bittorrent meta file contents.
+"""
+
+import logging
+import os
+from hashlib import sha1, sha256  # nosec
+
+from torrentfile.mixins import CbMixin, ProgMixin
+from torrentfile.utils import next_power_2
+
+BLOCK_SIZE = 2**14  # 16KiB
+HASH_SIZE = 32
+
+logger = logging.getLogger(__name__)
+
+
+class Hasher(CbMixin, ProgMixin):
+    """
+    Piece hasher for Bittorrent V1 files.
+
+    Takes a sorted list of all file paths, calculates sha1 hash
+    for fixed size pieces of file data from each file
+    seemlessly until the last piece which may be smaller than others.
+
+    Parameters
+    ----------
+    paths : list
+        List of files.
+    piece_length : int
+        Size of chuncks to split the data into.
+    progress : int
+        default = None
+    """
+
+    def __init__(self, paths: list, piece_length: int, progress: bool = True):
+        """Generate hashes of piece length data from filelist contents."""
+        self.piece_length = piece_length
+        self.paths = paths
+        self.progress = progress
+        self.total = sum(os.path.getsize(i) for i in self.paths)
+        self.index = 0
+        self.current = open(self.paths[0], "rb")
+        if self.progress:
+            total = os.path.getsize(self.paths[0])
+            self.prog_start(total, self.paths[0], unit="bytes")
+        logger.debug("Hashing %s", str(self.paths[0]))
+
+    def __iter__(self):
+        """
+        Iterate through feed pieces.
+
+        Returns
+        -------
+        self : iterator
+            Iterator for leaves/hash pieces.
+        """
+        return self
+
+    def _handle_partial(self, arr: bytearray) -> bytearray:
+        """
+        Define the handling partial pieces that span 2 or more files.
+
+        Parameters
+        ----------
+        arr : bytearray
+            Incomplete piece containing partial data
+
+        Returns
+        -------
+        digest : bytearray
+            SHA1 digest of the complete piece.
+        """
+        while len(arr) < self.piece_length and self.next_file():
+            target = self.piece_length - len(arr)
+            temp = bytearray(target)
+            size = self.current.readinto(temp)
+            arr.extend(temp[:size])
+            self.prog_update(size)
+            if size == target:
+                break
+        return sha1(arr).digest()  # nosec
+
+    def next_file(self) -> bool:
+        """
+        Seemlessly transition to next file in file list.
+
+        Returns
+        -------
+        bool:
+            True if there is a next file otherwise False.
+        """
+        self.index += 1
+        self.prog_close()
+        if self.index < len(self.paths):
+            path = self.paths[self.index]
+            logger.debug("Hashing %s", str(path))
+            self.current.close()
+            if self.progress:
+                self.prog_start(os.path.getsize(path), path, unit="bytes")
+            self.current = open(path, "rb")
+            return True
+        return False
+
+    def __next__(self) -> bytes:
+        """
+        Generate piece-length pieces of data from input file list.
+
+        Returns
+        -------
+        bytes
+            SHA1 hash of the piece extracted.
+        """
+        while True:
+            piece = bytearray(self.piece_length)
+            size = self.current.readinto(piece)
+            if size == 0:
+                if not self.next_file():
+                    raise StopIteration
+            elif size < self.piece_length:
+                self.prog_update(size)
+                return self._handle_partial(piece[:size])
+            else:
+                self.prog_update(size)
+                return sha1(piece).digest()  # nosec
+
+
+def merkle_root(blocks: list) -> bytes:
+    """
+    Calculate the merkle root for a seq of sha256 hash digests.
+
+    Parameters
+    ----------
+    blocks : list
+        a sequence of sha256 layer hashes.
+
+    Returns
+    -------
+    bytes
+        the sha256 root hash of the merkle tree.
+    """
+    if blocks:
+        while len(blocks) > 1:
+            blocks = [
+                sha256(x + y).digest() for x, y in zip(*[iter(blocks)] * 2)
+            ]
+        return blocks[0]
+    return blocks
+
+
+class HasherV2(CbMixin, ProgMixin):
+    """
+    Calculate the root hash and piece layers for file contents.
+
+    **DEPRECATED**
+
+    Iterates over 16KiB blocks of data from given file, hashes the data,
+    then creates a hash tree from the individual block hashes until size of
+    hashed data equals the piece-length.  Then continues the hash tree until
+    root hash is calculated.
+
+    Parameters
+    ----------
+    path : str
+        Path to file.
+    piece_length : int
+        Size of layer hashes pieces.
+    progress : int
+        default = None
+    """
+
+    def __init__(self, path: str, piece_length: int, progress: bool = True):
+        """
+        Calculate and store hash information for specific file.
+
+        **DEPRECATED**
+        """
+        self.path = path
+        self.root = None
+        self.piece_layer = None
+        self.layer_hashes = []
+        self.piece_length = piece_length
+        self.num_blocks = piece_length // BLOCK_SIZE
+        if progress:
+            self.prog_start(os.path.getsize(path), path, unit="bytes")
+        with open(self.path, "rb") as fd:
+            self.process_file(fd)
+
+    def process_file(self, fd: str):
+        """
+        Calculate hashes over 16KiB chuncks of file content.
+
+        **DEPRECATED**
+
+        Parameters
+        ----------
+        fd : TextIOWrapper
+            Opened file in read mode.
+        """
+        while True:
+            blocks = []
+            leaf = bytearray(BLOCK_SIZE)
+            # generate leaves of merkle tree
+
+            for _ in range(self.num_blocks):
+                size = fd.readinto(leaf)
+                self.prog_update(size)
+                if not size:
+                    break
+                blocks.append(sha256(leaf[:size]).digest())
+
+            # blocks is empty mean eof
+            if not blocks:
+                break
+            if len(blocks) != self.num_blocks:
+                # when size of file doesn't fill the last block
+                # when the file contains multiple pieces
+                remaining = self.num_blocks - len(blocks)
+                if not self.layer_hashes:
+                    # when the there is only one block for file
+                    power2 = next_power_2(len(blocks))
+                    remaining = power2 - len(blocks)
+
+                # pad the the rest with zeroes to fill remaining space.
+                padding = [bytes(32) for _ in range(remaining)]
+                self.prog_update(HASH_SIZE * remaining)
+                blocks.extend(padding)
+            # calculate the root hash for the merkle tree up to piece-length
+
+            layer_hash = merkle_root(blocks)
+            self.cb(layer_hash)
+            self.layer_hashes.append(layer_hash)
+        self._calculate_root()
+        self.prog_close()
+
+    def _calculate_root(self):
+        """
+        Calculate root hash for the target file.
+
+        **DEPRECATED**
+        """
+        self.piece_layer = b"".join(self.layer_hashes)
+        hashes = len(self.layer_hashes)
+        if hashes > 1:
+            pow2 = next_power_2(hashes)
+            remainder = pow2 - hashes
+            pad_piece = [bytes(HASH_SIZE) for _ in range(self.num_blocks)]
+            for _ in range(remainder):
+                self.layer_hashes.append(merkle_root(pad_piece))
+        self.root = merkle_root(self.layer_hashes)
+
+
+class HasherHybrid(CbMixin, ProgMixin):
+    """
+    Calculate root and piece hashes for creating hybrid torrent file.
+
+    **DEPRECATED**
+
+    Create merkle tree layers from sha256 hashed 16KiB blocks of contents.
+    With a branching factor of 2, merge layer hashes until blocks equal
+    piece_length bytes for the piece layer, and then the root hash.
+
+    Parameters
+    ----------
+    path : str
+        path to target file.
+    piece_length : int
+        piece length for data chunks.
+    progress : int
+        default = None
+    """
+
+    def __init__(self, path: str, piece_length: int, progress: bool = True):
+        """
+        Construct Hasher class instances for each file in torrent.
+
+        **DEPRECATED**
+        """
+        self.path = path
+        self.piece_length = piece_length
+        self.pieces = []
+        self.layer_hashes = []
+        self.piece_layer = None
+        self.root = None
+        self.padding_piece = None
+        self.padding_file = None
+        if progress:
+            self.prog_start(os.path.getsize(path), path, unit="bytes")
+        self.amount = piece_length // BLOCK_SIZE
+        with open(path, "rb") as data:
+            self.process_file(data)
+
+    def _pad_remaining(self, block_count: int):
+        """
+        Generate Hash sized, 0 filled bytes for padding.
+
+        **DEPRECATED**
+
+        Parameters
+        ----------
+        block_count : int
+            current total number of blocks collected.
+
+        Returns
+        -------
+        padding : bytes
+            Padding to fill remaining portion of tree.
+        """
+        # when the there is only one block for file
+        remaining = self.amount - block_count
+        if not self.layer_hashes:
+            power2 = next_power_2(block_count)
+            remaining = power2 - block_count
+        self.prog_update(HASH_SIZE * remaining)
+        return [bytes(HASH_SIZE) for _ in range(remaining)]
+
+    def process_file(self, data: bytearray):
+        """
+        Calculate layer hashes for contents of file.
+
+        **DEPRECATED**
+
+        Parameters
+        ----------
+        data : BytesIO
+            File opened in read mode.
+        """
+        while True:
+            plength = self.piece_length
+            blocks = []
+            piece = sha1()  # nosec
+            total = 0
+            block = bytearray(BLOCK_SIZE)
+            for _ in range(self.amount):
+                size = data.readinto(block)
+                self.prog_update(size)
+                if not size:
+                    break
+                total += size
+                plength -= size
+                blocks.append(sha256(block[:size]).digest())
+                piece.update(block[:size])
+            if not blocks:
+                break
+            if len(blocks) != self.amount:
+                padding = self._pad_remaining(len(blocks))
+                blocks.extend(padding)
+            layer_hash = merkle_root(blocks)
+            self.cb(layer_hash)
+            self.layer_hashes.append(layer_hash)
+            if plength > 0:
+                self.padding_file = {
+                    "attr": "p",
+                    "length": plength,
+                    "path": [".pad", str(plength)],
+                }
+                piece.update(bytes(plength))
+            self.pieces.append(piece.digest())  # nosec
+        self._calculate_root()
+        self.prog_close()
+
+    def _calculate_root(self):
+        """
+        Calculate the root hash for opened file.
+
+        **DEPRECATED**
+        """
+        self.piece_layer = b"".join(self.layer_hashes)
+
+        if len(self.layer_hashes) > 1:
+            pad_piece = merkle_root([bytes(32) for _ in range(self.amount)])
+
+            pow2 = next_power_2(len(self.layer_hashes))
+            remainder = pow2 - len(self.layer_hashes)
+
+            self.layer_hashes += [pad_piece for _ in range(remainder)]
+        self.root = merkle_root(self.layer_hashes)
+
+
+class FileHasher(CbMixin, ProgMixin):
+    """
+    Calculate root and piece hashes for creating hybrid torrent file.
+
+    Create merkle tree layers from sha256 hashed 16KiB blocks of contents.
+    With a branching factor of 2, merge layer hashes until blocks equal
+    piece_length bytes for the piece layer, and then the root hash.
+
+    Parameters
+    ----------
+    path : str
+        path to target file.
+    piece_length : int
+        piece length for data chunks.
+    progress : int
+        default = None
+    """
+
+    def __init__(
+        self,
+        path: str,
+        piece_length: int,
+        progress: bool = True,
+        hybrid: bool = False,
+    ):
+        """
+        Construct Hasher class instances for each file in torrent.
+        """
+        self.path = path
+        self.piece_length = piece_length
+        self.pieces = []
+        self.layer_hashes = []
+        self.piece_layer = None
+        self.root = None
+        self.padding_piece = None
+        self.padding_file = None
+        self.amount = piece_length // BLOCK_SIZE
+        self.end = False
+        self.current = open(path, "rb")
+        self.hybrid = hybrid
+        if progress:
+            self.progressbar = True
+            self.prog_start(os.path.getsize(path), path, unit="bytes")
+
+    def __iter__(self):
+        """Return `self`: needed to implement iterator implementation."""
+        return self
+
+    def _pad_remaining(self, block_count: int):
+        """
+        Generate Hash sized, 0 filled bytes for padding.
+
+        Parameters
+        ----------
+        block_count : int
+            current total number of blocks collected.
+
+        Returns
+        -------
+        padding : bytes
+            Padding to fill remaining portion of tree.
+        """
+        # when the there is only one block for file
+        remaining = self.amount - block_count
+        if not self.layer_hashes:
+            power2 = next_power_2(block_count)
+            remaining = power2 - block_count
+        return [bytes(HASH_SIZE) for _ in range(remaining)]
+
+    def __next__(self) -> bytes:
+        """
+        Calculate layer hashes for contents of file.
+
+        Returns
+        -------
+        bytes
+            The layer merckle root hash.
+        """
+        if self.end:
+            self.end = False
+            raise StopIteration
+        plength = self.piece_length
+        blocks = []
+        piece = sha1()  # nosec
+        total = 0
+        block = bytearray(BLOCK_SIZE)
+        for _ in range(self.amount):
+            size = self.current.readinto(block)
+            if not size:
+                self.end = True
+                break
+            total += size
+            plength -= size
+            blocks.append(sha256(block[:size]).digest())
+            if self.hybrid:
+                piece.update(block[:size])
+        if not blocks:
+            self._calculate_root()
+            raise StopIteration
+        if len(blocks) != self.amount:
+            padding = self._pad_remaining(len(blocks))
+            blocks.extend(padding)
+        self.prog_update(total)
+        layer_hash = merkle_root(blocks)
+        self.layer_hashes.append(layer_hash)
+        self.cb(layer_hash)
+        if self.end:
+            self._calculate_root()
+            self.prog_close()
+        if self.hybrid:
+            if plength > 0:
+                self.padding_file = {
+                    "attr": "p",
+                    "length": plength,
+                    "path": [".pad", str(plength)],
+                }
+                piece.update(bytes(plength))
+            piece = piece.digest()
+            self.pieces.append(piece)
+            return layer_hash, piece
+        return layer_hash
+
+    def _calculate_root(self):
+        """
+        Calculate the root hash for opened file.
+        """
+        self.piece_layer = b"".join(self.layer_hashes)
+
+        if len(self.layer_hashes) > 1:
+            pad_piece = merkle_root([bytes(32) for _ in range(self.amount)])
+
+            pow2 = next_power_2(len(self.layer_hashes))
+            remainder = pow2 - len(self.layer_hashes)
+
+            self.layer_hashes += [pad_piece for _ in range(remainder)]
+        self.root = merkle_root(self.layer_hashes)
+        self.current.close()
```

### Comparing `torrentfile-0.8.7/torrentfile/interactive.py` & `torrentfile-0.8.8/torrentfile/interactive.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.7/torrentfile/rebuild.py` & `torrentfile-0.8.8/torrentfile/recheck.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,604 +13,634 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 """
-Clases and functions for the rebuild or reassemble subcommand.
+Module container Checker Class.
 
-Re-assemble a torrent into the propper directory structure as indicated by a
-torrent meta file, and validate the contents of each file allong the
-way. Displays a progress bar for each torrent.
+The CheckerClass takes a torrentfile and tha path to it's contents.
+It will then iterate through every file and directory contained
+and compare their data to values contained within the torrent file.
+Completion percentages will be printed to screen for each file and
+at the end for the torrentfile as a whole.
 """
+
 import logging
-import math
 import os
-from hashlib import sha1
+from hashlib import sha1, sha256  # nosec
 from pathlib import Path
 
 import pyben
 
-from torrentfile.hasher import HasherV2
-from torrentfile.mixins import CbMixin, ProgMixin
-from torrentfile.utils import copypath
+from torrentfile.hasher import FileHasher
+from torrentfile.mixins import ProgMixin
+from torrentfile.utils import ArgumentError, MissingPathError
 
-logger = logging.getLogger(__name__)
 SHA1 = 20
+SHA256 = 32
+BLOCK_SIZE = 2**14  # 16KiB
 
+logger = logging.getLogger(__name__)
 
-class PathNode:
+
+class Checker:
     """
-    Base class representing information regarding a file included in torrent.
+    Check a given file or directory to see if it matches a torrentfile.
+
+    Public constructor for Checker class instance.
+
+    Parameters
+    ----------
+    metafile : str
+        Path to ".torrent" file.
+    path : str
+        Path where the content is located in filesystem.
+
+    Example
+    -------
+        >> metafile = "/path/to/torrentfile/content_file_or_dir.torrent"
+        >> location = "/path/to/location"
+        >> os.path.exists("/path/to/location/content_file_or_dir")
+        Out: True
+        >> checker = Checker(metafile, location)
     """
 
-    def __init__(
-        self,
-        start: int = None,
-        stop: int = None,
-        full: str = None,
-        filename: str = None,
-        path: str = None,
-        length: int = None,
-    ):
+    _hook = None
+
+    def __init__(self, metafile: str, path: str):
         """
-        Hold file information that contributes to the contents of torrent.
+        Validate data against hashes contained in .torrent file.
 
         Parameters
         ----------
-        start : int, optional
-            where the piece starts, by default None
-        stop : int, optional
-            where the piece ends, by default None
-        full : str, optional
-            full path, by default None
-        filename : str, optional
-            filename, by default None
-        path : str, optional
-            parent path, by default None
-        length : int, optional
-            size, by default None
-        """
-        self.path = path
-        self.start = start
-        self.stop = stop
-        self.length = length
-        self.filename = filename
-        self.full = full
+        metafile : str
+            path to .torrent file
+        path : str
+            path to content or contents parent directory.
+        """
+        if not os.path.exists(metafile):
+            raise FileNotFoundError
+        if os.path.isdir(metafile):
+            raise ArgumentError(
+                "The <metafile> must be a .torrent file. Not a directory"
+            )
+        self.last_log = None
+        self.log_msg("Checking: %s, %s", metafile, path)
+        self.metafile = metafile
+        self.total = 0
+        self.paths = []
+        self.fileinfo = {}
+        print("Extracting data from torrent file...")
+        self.meta = pyben.load(metafile)
+        self.info = self.meta["info"]
+        self.name = self.info["name"]
+        self.piece_length = self.info["piece length"]
+
+        if "meta version" in self.info:
+            if "pieces" in self.info:
+                self.meta_version = 3
+            else:
+                self.meta_version = 2
+        else:
+            self.meta_version = 1
 
-    def get_part(self, path: str) -> bytes:
+        self.root = self.find_root(path)
+        self.check_paths()
+
+    @classmethod
+    def register_callback(cls, hook):
         """
-        Extract the part of the file needed to complete the hash.
+        Register hooks from 3rd party programs to access generated info.
 
         Parameters
         ----------
-        path : str
-            filesystem path location of file.
-
-        Returns
-        -------
-        bytes
-            part of the file's contents
+        hook : function
+            callback function for the logging feature.
         """
-        with open(path, "rb") as fd:
-            if self.start:
-                fd.seek(self.start)
-            if self.stop != -1:
-                partial = fd.read(self.stop - self.start)
-            else:
-                partial = fd.read()
-        return partial
+        cls._hook = hook
 
-    def __len__(self) -> int:
+    def piece_checker(self):
         """
-        Return size of the file.
+        Check individual pieces of the torrent.
 
         Returns
         -------
-        int
-            total size
+        HashChecker | FeedChecker
+            Individual piece hasher.
         """
-        return self.length
+        if self.meta_version == 1:
+            return FeedChecker
+        return HashChecker
 
-
-class PieceNode:
-    """
-    Base class representing a single SHA1 hash block of data from a torrent.
-    """
-
-    def __init__(self, piece: bytes):
+    def results(self):
+        """
+        Generate result percentage and store for future calls.
         """
-        Store information about an individual SHA1 hash for a torrent file.
+        responses = []
+        for response in self.iter_hashes():
+            responses.append(response)
 
-        _extended_summary_
+        self.log_msg(
+            "Final result for %s recheck:  %s", self.metafile, self._result
+        )
 
-        Parameters
-        ----------
-        piece : bytes
-            SHA1 hash bytes
-        """
-        self.piece = piece
-        self.paths = []
-        self.result = None
-        self.dest = None
+        return self._result
 
-    def append(self, pathnode: PathNode):
+    def log_msg(self, *args, level: int = logging.INFO):
         """
-        Append the path argument to the paths list attribute.
+        Log message `msg` to logger and send `msg` to callback hook.
 
         Parameters
         ----------
-        pathnode : PathNode
-            the pathnode
+        *args : dict
+            formatting args for log message
+        level : int
+            Log level for this message; default=`logging.INFO`
         """
-        self.paths.append(pathnode)
+        message = args[0]
+        if len(args) >= 3:
+            message = message % tuple(args[1:])
+        elif len(args) == 2:
+            message = message % args[1]
 
-    def _find_matches(self, filemap: dict, paths: list, data: bytes) -> bool:
+        # Repeat log messages should be ignored.
+        if message != self.last_log:
+            self.last_log = message
+            logger.log(level, message)
+            if self._hook and level == logging.INFO:
+                self._hook(message)
+
+    def find_root(self, path: str) -> str:
         """
-        Gather relavent sections of the files in the list and check the hash.
+        Check path for torrent content.
+
+        The path can be a relative or absolute filesystem path.  In the case
+        where the content is a single file, the path may point directly to the
+        the file, or it may point to the parent directory.  If content points
+        to a directory.  The directory will be checked to see if it matches
+        the torrent's name, if not the directories contents will be searched.
+        The returned value will be the absolute path that matches the torrent's
+        name.
 
         Parameters
         ----------
-        filemap : dict
-            dictionary containing filename and path details
-        paths : list
-            list of pathnodes
-        data : bytes
-            raw file contents
+        path : str
+            root path to torrent content
 
         Returns
         -------
-        bool
-            success state
+        str
+            root path to content
         """
-        if not paths:
-            piece_hash = sha1(data).digest()  # nosec
-            return piece_hash == self.piece
-        pathnode = paths[0]
-        filename = pathnode.filename
-        if filename not in filemap:
-            return False  # pragma: nocover
-        for loc, size in filemap[filename]:
-            if size != len(pathnode):
-                continue
-            partial = pathnode.get_part(loc)
-            val = self._find_matches(filemap, paths[1:], data + partial)
-            if val:
-                dest_path = os.path.join(self.dest, pathnode.full)
-                copypath(loc, dest_path)
-            return val
-        return False
+        if not os.path.exists(path):
+            self.log_msg("Could not locate torrent content %s.", path)
+            raise FileNotFoundError(path)
 
-    def find_matches(self, filemap: dict, dest: str) -> bool:
-        """
-        Find the matching files for each path in the node.
+        root = Path(path)
+        if root.name == self.name:
+            self.log_msg("Content found: %s.", str(root))
+            return root
 
-        Parameters
-        ----------
-        filemap : dict
-            filename and details
-        dest : str
-            target destination path
+        if self.name in os.listdir(root):
+            return root / self.name
 
-        Returns
-        -------
-        bool
-            success status
+        self.log_msg("Could not locate torrent content in: %s", str(root))
+        raise FileNotFoundError(root)
+
+    def check_paths(self):
         """
-        self.dest = dest
-        self.result = self._find_matches(filemap, self.paths[:], bytes())
-        return self.result
+        Gather all file paths described in the torrent file.
+        """
+        finfo = self.fileinfo
 
+        if "length" in self.info:
+            self.log_msg("%s points to a single file", self.root)
+            self.total = self.info["length"]
+            self.paths.append(str(self.root))
 
-class Metadata(CbMixin, ProgMixin):
-    """
-    Class containing the metadata contents of a torrent file.
-    """
+            finfo[0] = {
+                "path": self.root,
+                "length": self.info["length"],
+            }
 
-    def __init__(self, path: str):
-        """
-        Construct metadata object for torrent info.
+            if self.meta_version > 1:
+                root = self.info["file tree"][self.name][""]["pieces root"]
+                finfo[0]["pieces root"] = root
 
-        Parameters
-        ----------
-        path : str
-            path to the .torrent file.
-        """
-        self.path = os.path.abspath(path)
-        self.name = None
-        self.piece_length = 1
-        self.meta_version = 1
-        self.pieces = b""
-        self.piece_nodes = []
-        self.length = 0
-        self.files = []
-        self.filenames = set()
-        self.extract()
-        if self.meta_version == 2:
-            self.num_pieces = len(self.filenames)
-        else:
-            self.num_pieces = math.ceil(len(self.pieces) / SHA1)
+            return
 
-    def extract(self):
-        """
-        Decode and extract information for the .torrent file.
-        """
-        meta = pyben.load(self.path)
-        info = meta["info"]
-        self.piece_length = info["piece length"]
-        self.name = info["name"]
-        self.meta_version = info.get("meta version", 1)
-        self.pieces = info.get("pieces", bytes())
-        if self.meta_version == 2:
-            self._parse_tree(info["file tree"], [self.name])
-        elif "length" in info:
-            self.length += info["length"]
-            self.is_file = True
-            self.filenames.add(info["name"])
-            self.files.append(
-                {
-                    "path": Path(self.name).parent,
-                    "filename": self.name,
-                    "full": self.name,
-                    "length": self.length,
+        # Otherwise Content is more than 1 file.
+        self.log_msg("%s points to a directory", self.root)
+        if self.meta_version == 1:
+            for i, item in enumerate(self.info["files"]):
+                self.total += item["length"]
+                base = os.path.join(*item["path"])
+
+                self.fileinfo[i] = {
+                    "path": str(self.root / base),
+                    "length": item["length"],
                 }
-            )
-        elif "files" in info:
-            for f in info["files"]:
-                path = f["path"]
-                full = os.path.join(self.name, *path)
-                self.files.append(
-                    {
-                        "path": Path(full).parent,
-                        "filename": path[-1],
-                        "full": full,
-                        "length": f["length"],
-                    }
-                )
-                self.length += f["length"]
-                self.filenames.add(path[-1])
-
-    def _map_pieces(self):
-        """
-        Create PathNode and PieceNode details for each piece in the torrent.
-        """
-        total_pieces = len(self.pieces) // SHA1
-        remainder = file_index = 0
-        current = {}
-        for i in range(total_pieces):
-            begin = SHA1 * i
-            piece = PieceNode(self.pieces[begin: begin + SHA1])
-            target = self.piece_length
-            if remainder:
-                start = current["length"] - remainder
-                if remainder < target:
-                    stop = -1
-                    target -= remainder
-                    remainder = 0
-                    file_index += 1
-                else:
-                    stop = start + target
-                    remainder -= target
-                    target -= target
-                pathnode = PathNode(start=start, stop=stop, **current)
-                piece.append(pathnode)
-            while target > 0 and file_index < len(self.files):
-                start = 0
-                current = self.files[file_index]
-                size = current["length"]
-                if size < target:
-                    stop = -1
-                    target -= size
-                    file_index += 1
-                else:
-                    stop = target
-                    remainder = size - target
-                    target = 0
-                pathnode = PathNode(start=start, stop=stop, **current)
-                piece.append(pathnode)
-            self.piece_nodes.append(piece)
 
-    def _parse_tree(self, tree: dict, partials: list):
+                self.paths.append(str(self.root / base))
+            return
+
+        self.walk_file_tree(self.info["file tree"], [])
+
+    def walk_file_tree(self, tree: dict, partials: list):
         """
-        Parse the file tree dictionary of the torrent metafile.
+        Traverse File Tree dictionary to get file details.
+
+        Extract full pathnames, length, root hash, and layer hashes
+        for each file included in the .torrent's file tree.
 
         Parameters
         ----------
         tree : dict
-            the dictionary representation of a file tree.
+            File Tree dict extracted from torrent file.
         partials : list
-            list of paths leading up to the current key value.
+            list of intermediate pathnames.
         """
         for key, val in tree.items():
+            # Empty string means the tree's leaf is value
             if "" in val:
-                self.filenames.add(key)
-                path = Path(os.path.join(*partials))
-                full = Path(os.path.join(path, key))
+                base = os.path.join(*partials, key)
+                roothash = None
                 length = val[""]["length"]
-                root = val[""]["pieces root"]
-                self.files.append(
-                    {
-                        "path": path,
-                        "full": full,
-                        "filename": key,
-                        "length": length,
-                        "root": root,
-                    }
-                )
-                self.length += length
+                roothash = None if not length else val[""]["pieces root"]
+                full = str(self.root / base)
+                self.fileinfo[len(self.paths)] = {
+                    "path": full,
+                    "length": length,
+                    "pieces root": roothash,
+                }
+                self.paths.append(full)
+                self.total += length
             else:
-                self._parse_tree(val, partials + [key])
+                self.walk_file_tree(val, partials + [key])
 
-    def _match_v1(self, filemap: dict, dest: str):
+    def iter_hashes(self) -> tuple:
         """
-        Check each of the nodes against the filemap dictionary for matches.
+        Produce results of comparing torrent contents piece by piece.
 
-        Parameters
-        ----------
-        filemap : dict
-            filenames and filesystem information
-        dest : str
-            target destination path
-        """
-        self._map_pieces()
-        copied = []
-        for piece_node in self.piece_nodes:
-            paths = piece_node.paths
-            if len(paths) == 1 and paths[0].path in copied:
-                self._update()
-                continue
-            if piece_node.find_matches(filemap, dest):
-                for pathnode in paths:
-                    if pathnode.path not in copied:
-                        copied.append(pathnode.path)
-                        dest_path = os.path.join(dest, pathnode.path)
-                        self._update()
-                        self.cb(pathnode.path, dest_path, self.num_pieces)
+        Yields
+        ------
+        chunck : bytes
+            hash of data found on disk
+        piece : bytes
+            hash of data when complete and correct
+        path : str
+            path to file being hashed
+        size : int
+            length of bytes hashed for piece
+        """
+        matched = consumed = 0
+        checker = self.piece_checker()
+        for chunk, piece, path, size in checker(self):
+            consumed += size
+            matching = 0
+            if chunk == piece:
+                matching += size
+                matched += size
+            yield chunk, piece, path, size
+            total_consumed = str(int(consumed / self.total * 100))
+            percent_matched = str(int(matched / consumed * 100))
+            self.log_msg(
+                "Processed: %s%%, Matched: %s%%",
+                total_consumed,
+                percent_matched,
+            )
+        self._result = (matched / consumed) * 100 if consumed > 0 else 0
 
-    def _match_v2(self, filemap: dict, dest: str):
-        """
-        Rebuild method for torrent v2 files.
 
-        Parameters
-        ----------
-        filemap : dict
-            filesystem information
-        dest : str
-            destiantion path
-        """
-        for entry in self.files:
-            filename = entry["filename"]
-            length = entry["length"]
-            if filename not in filemap:
-                continue  # pragma: nocover
-            paths = filemap[filename]
-            for path, size in paths:
-                if size == length:
-                    hasher = HasherV2(path, self.piece_length, True)
-                    if entry["root"] == hasher.root:
-                        dest_path = os.path.join(dest, entry["full"])
-                        copypath(entry["path"], dest_path)
-                        self._update()
-                        self.cb(path, dest_path, self.num_pieces)
-                        break
-
-    def rebuild(self, filemap: dict, dest: str):
-        """
-        Rebuild torrent file contents from filemap at dest.
-
-        Searches through the contents of the meta file and compares filenames
-        with those in the filemap dict, and if found checks their contents,
-        and copies them to the destination path.
+class FeedChecker(ProgMixin):
+    """
+    Validates torrent content.
 
-        Parameters
-        ----------
-        filemap : dict
-            filesystem information
-        dest : str
-            destiantion path
-        """
-        self._prog = None
-        if self.meta_version == 2:
-            self._match_v2(filemap, dest)
-        else:
-            self._match_v1(filemap, dest)
-        if self._prog is not None:
-            self.prog_close()
+    Seemlesly validate torrent file contents by comparing hashes in
+    metafile against data on disk.
 
-    def _update(self):
-        """Start and updating the progress bar."""
-        if self._prog is None:
-            self._prog = True
-            self.prog_start(self.num_pieces, self.name, unit="piece")
-        self.prog_update(1)
+    Parameters
+    ----------
+    checker : object
+        the checker class instance.
+    """
 
+    def __init__(self, checker: Checker):
+        """
+        Generate hashes of piece length data from filelist contents.
+        """
+        self.piece_length = checker.piece_length
+        self.paths = checker.paths
+        self.pieces = checker.info["pieces"]
+        self.fileinfo = checker.fileinfo
+        self.piece_map = {}
+        self.index = 0
+        self.piece_count = 0
+        self.it = None
 
-class Assembler(CbMixin):
-    """
-    Does most of the work in attempting the structure of torrentfiles.
+    def __iter__(self):
+        """
+        Assign iterator and return self.
+        """
+        self.it = self.iter_pieces()
+        return self
 
-    Requires three paths as arguments.
-    - torrent metafile or directory containing multiple meta files
-    - directory containing the contents of meta file
-    - directory where torrents will be re-assembled
-    """
+    def __next__(self):
+        """
+        Yield back result of comparison.
+        """
+        try:
+            partial = next(self.it)
+        except StopIteration as itererror:
+            raise StopIteration from itererror
+
+        chunck = sha1(partial).digest()  # nosec
+        start = self.piece_count * SHA1
+        end = start + SHA1
+        piece = self.pieces[start:end]
+        self.piece_count += 1
+        path = self.paths[self.index]
+        return chunck, piece, path, len(partial)
 
-    def __init__(self, metafiles: list, contents: list, dest: str):
+    def iter_pieces(self):
         """
-        Reassemble given torrent file from given cli arguments.
+        Iterate through, and hash pieces of torrent contents.
+
+        Yields
+        ------
+        piece : bytes
+            hash digest for block of torrent data.
+        """
+        partial = bytearray()
+        for i, path in enumerate(self.paths):
+            total = self.fileinfo[i]["length"]
+            self.prog_start(total, path, unit="bytes")
+            self.index = i
+            if os.path.exists(path):
+                for piece in self.extract(path, partial):
+                    if (len(piece) == self.piece_length) or (
+                        i + 1 == len(self.paths)
+                    ):
+                        yield piece
+                    else:
+                        partial = piece
+
+            else:
+                length = self.fileinfo[i]["length"]
+                for pad in self._gen_padding(partial, length):
+                    if len(pad) == self.piece_length:
+                        yield pad
+                    else:
+                        partial = pad
+            self.prog_close()
 
-        Rebuild metafiles and contents into their original directory
-        structure as much as possible in the destination directory.
-        Takes two paths as parameters,
-        - file or directory containing 1 or more torrent meta files
-        - path to where the contents are belived to be located.
+    def extract(self, path: str, partial: bytearray) -> bytearray:
+        """
+        Split file paths contents into blocks of data for hash pieces.
 
         Parameters
         ----------
-        metafiles : str
-            path to torrent metafile or directory containing torrent metafiles.
-        contents : str
-            path to content or directory containing content that belongs to
-            torrentfile.
-        dest: str
-            path to the directory where rebuild will take place.
-        """
-        self.counter = 0
-        self._lastlog = None
-        self.contents = contents
-        Metadata.set_callback(self._callback)
-        self.dest = dest
-        self.meta_paths = metafiles
-        self.metafiles = self._get_metafiles()
-        filenames = set()
-        for meta in self.metafiles:
-            filenames |= meta.filenames
-        self.filemap = _index_contents(self.contents, filenames)
+        path : str
+            path to content.
+        partial : bytes
+            any remaining content from last file.
 
-    def _callback(self, filename: str, dest: str, num_pieces: int):
+        Returns
+        -------
+        bytearray
+            Hash digest for block of .torrent contents.
         """
-        Run the callback functions associated with Mixin for copied files.
+        read = 0
+        length = self.fileinfo[self.index]["length"]
+        partial = bytearray() if len(partial) == self.piece_length else partial
+        if path not in self.paths:  # pragma: no cover
+            raise MissingPathError(path)
+        with open(path, "rb") as current:
+            while True:
+                bitlength = self.piece_length - len(partial)
+                part = bytearray(bitlength)
+                amount = current.readinto(part)
+                read += amount
+                partial.extend(part[:amount])
+                if amount < bitlength:
+                    if amount > 0 and read == length:
+                        self.prog_update(amount)
+                        yield partial
+                    break
+                self.prog_update(amount)
+                yield partial
+                partial = bytearray(0)
+        if length != read:
+            for pad in self._gen_padding(partial, length, read):
+                yield pad
+
+    def _gen_padding(self, partial: bytes, length: int, read=0) -> bytes:
+        """
+        Create padded pieces where file sizes do not match.
 
         Parameters
         ----------
-        filename : str
-            filename
-        dest : str
-            destination path
-        num_pieces : int
-            number of hash pieces
-        """
-        self.counter += 1
-        message = f"Matched:{num_pieces} {filename} -> {dest}"
-        if message != self._lastlog:
-            self._lastlog = message
-            logger.debug(message)
+        partial : bytes
+            any remaining data from last file processed.
+        length : int
+            size of space that needs padding
+        read : int
+            portion of length already padded
 
-    def assemble_torrents(self):
+        Yields
+        ------
+        bytes
+            A piece length sized block of zeros.
         """
-        Assemble collection of torrent files into original structure.
+        while read < length:
+            left = self.piece_length - len(partial)
+            if length - read > left:
+                padding = bytearray(left)
+                partial.extend(padding)
+                yield partial
+                read += left
+                partial = bytearray(0)
+            else:
+                partial.extend(bytearray(length - read))
+                read = length
+                yield partial
 
-        Returns
-        -------
-        int
-            number of files copied
+
+class HashChecker(ProgMixin):
+    """
+    Iterate through contents of meta data and verify with file contents.
+
+    Parameters
+    ----------
+    checker : Checker
+        the checker instance that maintains variables.
+    """
+
+    def __init__(self, checker: Checker):
         """
-        for metafile in self.metafiles:
-            logger.info(
-                "#%s Searching contents for %s", self.counter, metafile.name
-            )
-            self.rebuild(metafile)
-        return self.counter
+        Construct a HybridChecker instance.
+        """
+        self.checker = checker
+        self.paths = checker.paths
+        self.piece_length = checker.piece_length
+        self.fileinfo = checker.fileinfo
+        self.piece_layers = checker.meta["piece layers"]
+        self.current = None
+        self.index = -1
 
-    def rebuild(self, metafile: Metadata) -> None:
+    def __iter__(self):
+        """
+        Assign iterator and return self.
         """
-        Build the torrent file structure from contents of directory.
+        return self
 
-        Traverse contents dir and compare discovered files
-        with files listed in torrent metadata and copy
-        the matches to the destination directory respecting folder
-        structures along the way.
+    def __next__(self):
         """
-        metafile.rebuild(self.filemap, self.dest)
+        Provide the result of comparison.
+        """
+        if self.current is None:
+            self.next_file()
+        try:
+            return self.process_current()
+        except StopIteration as itererr:
+            if self.next_file():
+                return self.process_current()
+            raise StopIteration from itererr
 
-    def _iter_files(self, path: str) -> list:
+    class Padder:
         """
-        Iterate through metfiles directory createing Metafile objects.
+        Padding class to generate padding hashes wherever needed.
 
         Parameters
         ----------
-        path : str
-            fs path
-
-        Returns
-        -------
-        list
-            list of Metadata Object
+        length: int
+            the total size of the mock file generating padding for.
+        piece_length : int
+            the block size that each hash represents.
         """
-        metafiles = []
-        for filename in os.listdir(path):
-            if filename.lower().endswith(".torrent"):
-                try:
-                    meta = Metadata(os.path.join(path, filename))
-                    metafiles.append(meta)
-                except ValueError:  # pragma: nocover
-                    self.counter -= 1
-        return metafiles
 
-    def _get_metafiles(self) -> list:
+        def __init__(self, length, piece_length):
+            """
+            Construct padding class to Mock missing or incomplete files.
+
+            Parameters
+            ----------
+            length : int
+                size of the file
+            piece_length : int
+                the piece length for each iteration.
+            """
+            self.length = length
+            self.piece_length = piece_length
+            self.pad = sha256(bytearray(piece_length)).digest()
+
+        def __iter__(self):
+            """
+            Return self to correctly implement iterator type.
+            """
+            return self  # pragma: nocover
+
+        def __next__(self) -> bytes:
+            """
+            Iterate through seemingly endless sha256 hashes of zeros.
+
+            Returns
+            -------
+            tuple :
+                returns the padding
+
+            Raises
+            ------
+            StopIteration
+            """
+            if self.length >= self.piece_length:
+                self.length -= self.piece_length
+                return self.pad
+            if self.length > 0:
+                pad = sha256(bytearray(self.length)).digest()
+                self.length -= self.length
+                return pad
+            raise StopIteration
+
+    def next_file(self) -> bool:
         """
-        Collect all .torrent meta files from given directory or file.
+        Remove all references to  processed files and prepare for the next.
 
         Returns
         -------
-        list
-            metafile objects
+        bool
+            if there is a next file found
         """
-        metafiles = []
-        for path in self.meta_paths:
-            if os.path.exists(path):
-                if os.path.isdir(path):
-                    metafiles += self._iter_files(path)
-                elif path.lower().endswith(".torrent"):
-                    meta = Metadata(path)
-                    metafiles.append(meta)
-        return metafiles
-
-
-def _index_contents(contents: list, filenames: set) -> dict:
-    """
-    Collect all of the filenames and their respective paths.
-
-    Parameters
-    ----------
-    contents : list
-        paths to traverse looking for filenames
-    filenames : set
-        set of filenames to look for
+        self.index += 1
+        self.prog_close()
+        if self.current is None or self.index < len(self.paths):
+            self.current = self.paths[self.index]
+            self.length = self.fileinfo[self.index]["length"]
+            self.root_hash = self.fileinfo[self.index]["pieces root"]
+            if self.length > self.piece_length:
+                self.pieces = self.piece_layers[self.root_hash]
+            else:
+                self.pieces = self.root_hash
+            path = self.paths[self.index]
+            self.prog_start(self.length, path, unit="bytes")
+            self.count = 0
+            if os.path.exists(self.current):
+                self.hasher = FileHasher(path, self.piece_length, progress=0)
+            else:
+                self.hasher = self.Padder(self.length, self.piece_length)
+            return True
+        if self.index >= len(self.paths):
+            del self.current
+            del self.length
+            del self.root_hash
+            del self.pieces
+        return False
 
-    Returns
-    -------
-    dict
-        all filenames and their respective paths.
-    """
-    mapping = {}
-    for dirpath in contents:
-        mapped = _index_content(dirpath, filenames)
-        for key, value in mapped.items():
-            mapping.setdefault(key, [])
-            mapping[key].extend(value)
-    return mapping
+    def process_current(self) -> tuple:
+        """
+        Gather necessary information to compare to metafile details.
 
+        Returns
+        -------
+        tuple
+            a tuple containing the layer, piece, current path and size
 
-def _index_content(root: str, filenames: set) -> dict:
-    """
-    Collect filenames from directory or file.
+        Raises
+        ------
+        StopIteration
+        """
+        try:
+            layer = next(self.hasher)
+            piece, size = self.advance()
+            self.prog_update(size)
+            return layer, piece, self.current, size
+        except StopIteration as err:
+            if self.length > 0 and self.count * SHA256 < len(self.pieces):
+                self.hasher = self.Padder(self.length, self.piece_length)
+                piece, size = self.advance()
+                layer = next(self.hasher)
+                self.prog_update(0)
+                return layer, piece, self.current, size
+            raise StopIteration from err
 
-    Parameters
-    ----------
-    root : str
-        path to search for filenames
-    filenames : set
-        set of filenames to search for
+    def advance(self) -> tuple:
+        """
+        Increment the number of pieces processed for the current file.
 
-    Returns
-    -------
-    dict
-        filenames and their respective paths
-    """
-    filemap = {}
-    if os.path.isfile(root):
-        name = os.path.basename(root)
-        if name in filenames:
-            size = os.path.getsize(root)
-            filemap.setdefault(name, [])
-            filemap[name].append((root, size))
-        return filemap
-    if os.path.isdir(root):
-        for path in os.listdir(root):
-            fullpath = os.path.join(root, path)
-            resultmap = _index_content(fullpath, filenames)
-            for key, value in resultmap.items():
-                filemap.setdefault(key, [])
-                filemap[key].extend(value)
-    return filemap
+        Returns
+        -------
+        tuple
+            the piece and size
+        """
+        start = self.count * SHA256
+        end = start + SHA256
+        piece = self.pieces[start:end]
+        self.count += 1
+        if self.length >= self.piece_length:
+            self.length -= self.piece_length
+            size = self.piece_length
+        else:
+            size = self.length
+            self.length -= self.length
+        return piece, size
```

### Comparing `torrentfile-0.8.7/torrentfile/recheck.py` & `torrentfile-0.8.8/torrentfile/rebuild.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,649 +1,616 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Module container Checker Class.
-
-The CheckerClass takes a torrentfile and tha path to it's contents.
-It will then iterate through every file and directory contained
-and compare their data to values contained within the torrent file.
-Completion percentages will be printed to screen for each file and
-at the end for the torrentfile as a whole.
-"""
-
-import logging
-import os
-from hashlib import sha1, sha256  # nosec
-from pathlib import Path
-
-import pyben
-
-from torrentfile.hasher import FileHasher
-from torrentfile.mixins import ProgMixin
-from torrentfile.utils import ArgumentError, MissingPathError
-
-SHA1 = 20
-SHA256 = 32
-BLOCK_SIZE = 2**14  # 16KiB
-
-logger = logging.getLogger(__name__)
-
-
-class Checker:
-    """
-    Check a given file or directory to see if it matches a torrentfile.
-
-    Public constructor for Checker class instance.
-
-    Parameters
-    ----------
-    metafile : str
-        Path to ".torrent" file.
-    path : str
-        Path where the content is located in filesystem.
-
-    Example
-    -------
-        >> metafile = "/path/to/torrentfile/content_file_or_dir.torrent"
-        >> location = "/path/to/location"
-        >> os.path.exists("/path/to/location/content_file_or_dir")
-        Out: True
-        >> checker = Checker(metafile, location)
-    """
-
-    _hook = None
-
-    def __init__(self, metafile: str, path: str):
-        """
-        Validate data against hashes contained in .torrent file.
-
-        Parameters
-        ----------
-        metafile : str
-            path to .torrent file
-        path : str
-            path to content or contents parent directory.
-        """
-        if not os.path.exists(metafile):
-            raise FileNotFoundError
-        if os.path.isdir(metafile):
-            raise ArgumentError(
-                "The <metafile> must be a .torrent file. Not a directory"
-            )
-        self.last_log = None
-        self.log_msg("Checking: %s, %s", metafile, path)
-        self.metafile = metafile
-        self.total = 0
-        self.paths = []
-        self.fileinfo = {}
-        print("Extracting data from torrent file...")
-        self.meta = pyben.load(metafile)
-        self.info = self.meta["info"]
-        self.name = self.info["name"]
-        self.piece_length = self.info["piece length"]
-
-        if "meta version" in self.info:
-            if "pieces" in self.info:
-                self.meta_version = 3
-            else:
-                self.meta_version = 2
-        else:
-            self.meta_version = 1
-
-        self.root = self.find_root(path)
-        self.check_paths()
-
-    @classmethod
-    def register_callback(cls, hook):
-        """
-        Register hooks from 3rd party programs to access generated info.
-
-        Parameters
-        ----------
-        hook : function
-            callback function for the logging feature.
-        """
-        cls._hook = hook
-
-    def piece_checker(self):
-        """
-        Check individual pieces of the torrent.
-
-        Returns
-        -------
-        HashChecker | FeedChecker
-            Individual piece hasher.
-        """
-        if self.meta_version == 1:
-            return FeedChecker
-        return HashChecker
-
-    def results(self):
-        """
-        Generate result percentage and store for future calls.
-        """
-        responses = []
-        for response in self.iter_hashes():
-            responses.append(response)
-
-        self.log_msg(
-            "Final result for %s recheck:  %s", self.metafile, self._result
-        )
-
-        return self._result
-
-    def log_msg(self, *args, level: int = logging.INFO):
-        """
-        Log message `msg` to logger and send `msg` to callback hook.
-
-        Parameters
-        ----------
-        *args : dict
-            formatting args for log message
-        level : int
-            Log level for this message; default=`logging.INFO`
-        """
-        message = args[0]
-        if len(args) >= 3:
-            message = message % tuple(args[1:])
-        elif len(args) == 2:
-            message = message % args[1]
-
-        # Repeat log messages should be ignored.
-        if message != self.last_log:
-            self.last_log = message
-            logger.log(level, message)
-            if self._hook and level == logging.INFO:
-                self._hook(message)
-
-    def find_root(self, path: str) -> str:
-        """
-        Check path for torrent content.
-
-        The path can be a relative or absolute filesystem path.  In the case
-        where the content is a single file, the path may point directly to the
-        the file, or it may point to the parent directory.  If content points
-        to a directory.  The directory will be checked to see if it matches
-        the torrent's name, if not the directories contents will be searched.
-        The returned value will be the absolute path that matches the torrent's
-        name.
-
-        Parameters
-        ----------
-        path : str
-            root path to torrent content
-
-        Returns
-        -------
-        str
-            root path to content
-        """
-        if not os.path.exists(path):
-            self.log_msg("Could not locate torrent content %s.", path)
-            raise FileNotFoundError(path)
-
-        root = Path(path)
-        if root.name == self.name:
-            self.log_msg("Content found: %s.", str(root))
-            return root
-
-        if self.name in os.listdir(root):
-            return root / self.name
-
-        self.log_msg("Could not locate torrent content in: %s", str(root))
-        raise FileNotFoundError(root)
-
-    def check_paths(self):
-        """
-        Gather all file paths described in the torrent file.
-        """
-        finfo = self.fileinfo
-
-        if "length" in self.info:
-            self.log_msg("%s points to a single file", self.root)
-            self.total = self.info["length"]
-            self.paths.append(str(self.root))
-
-            finfo[0] = {
-                "path": self.root,
-                "length": self.info["length"],
-            }
-
-            if self.meta_version > 1:
-                root = self.info["file tree"][self.name][""]["pieces root"]
-                finfo[0]["pieces root"] = root
-
-            return
-
-        # Otherwise Content is more than 1 file.
-        self.log_msg("%s points to a directory", self.root)
-        if self.meta_version == 1:
-
-            for i, item in enumerate(self.info["files"]):
-                self.total += item["length"]
-                base = os.path.join(*item["path"])
-
-                self.fileinfo[i] = {
-                    "path": str(self.root / base),
-                    "length": item["length"],
-                }
-
-                self.paths.append(str(self.root / base))
-            return
-
-        self.walk_file_tree(self.info["file tree"], [])
-
-    def walk_file_tree(self, tree: dict, partials: list):
-        """
-        Traverse File Tree dictionary to get file details.
-
-        Extract full pathnames, length, root hash, and layer hashes
-        for each file included in the .torrent's file tree.
-
-        Parameters
-        ----------
-        tree : dict
-            File Tree dict extracted from torrent file.
-        partials : list
-            list of intermediate pathnames.
-        """
-        for key, val in tree.items():
-
-            # Empty string means the tree's leaf is value
-            if "" in val:
-
-                base = os.path.join(*partials, key)
-                roothash = None
-                length = val[""]["length"]
-                roothash = None if not length else val[""]["pieces root"]
-                full = str(self.root / base)
-                self.fileinfo[len(self.paths)] = {
-                    "path": full,
-                    "length": length,
-                    "pieces root": roothash,
-                }
-                self.paths.append(full)
-                self.total += length
-            else:
-                self.walk_file_tree(val, partials + [key])
-
-    def iter_hashes(self) -> tuple:
-        """
-        Produce results of comparing torrent contents piece by piece.
-
-        Yields
-        ------
-        chunck : bytes
-            hash of data found on disk
-        piece : bytes
-            hash of data when complete and correct
-        path : str
-            path to file being hashed
-        size : int
-            length of bytes hashed for piece
-        """
-        matched = consumed = 0
-        checker = self.piece_checker()
-        for chunk, piece, path, size in checker(self):
-            consumed += size
-            matching = 0
-            if chunk == piece:
-                matching += size
-                matched += size
-            yield chunk, piece, path, size
-            total_consumed = str(int(consumed / self.total * 100))
-            percent_matched = str(int(matched / consumed * 100))
-            self.log_msg(
-                "Processed: %s%%, Matched: %s%%",
-                total_consumed,
-                percent_matched,
-            )
-        self._result = (matched / consumed) * 100 if consumed > 0 else 0
-
-
-class FeedChecker(ProgMixin):
-    """
-    Validates torrent content.
-
-    Seemlesly validate torrent file contents by comparing hashes in
-    metafile against data on disk.
-
-    Parameters
-    ----------
-    checker : object
-        the checker class instance.
-    """
-
-    def __init__(self, checker: Checker):
-        """
-        Generate hashes of piece length data from filelist contents.
-        """
-        self.piece_length = checker.piece_length
-        self.paths = checker.paths
-        self.pieces = checker.info["pieces"]
-        self.fileinfo = checker.fileinfo
-        self.piece_map = {}
-        self.index = 0
-        self.piece_count = 0
-        self.it = None
-
-    def __iter__(self):
-        """
-        Assign iterator and return self.
-        """
-        self.it = self.iter_pieces()
-        return self
-
-    def __next__(self):
-        """
-        Yield back result of comparison.
-        """
-        try:
-            partial = next(self.it)
-        except StopIteration as itererror:
-            raise StopIteration from itererror
-
-        chunck = sha1(partial).digest()  # nosec
-        start = self.piece_count * SHA1
-        end = start + SHA1
-        piece = self.pieces[start:end]
-        self.piece_count += 1
-        path = self.paths[self.index]
-        return chunck, piece, path, len(partial)
-
-    def iter_pieces(self):
-        """
-        Iterate through, and hash pieces of torrent contents.
-
-        Yields
-        ------
-        piece : bytes
-            hash digest for block of torrent data.
-        """
-        partial = bytearray()
-        for i, path in enumerate(self.paths):
-            total = self.fileinfo[i]["length"]
-            self.prog_start(total, path, unit="bytes")
-            self.index = i
-            if os.path.exists(path):
-                for piece in self.extract(path, partial):
-                    if (len(piece) == self.piece_length) or (
-                        i + 1 == len(self.paths)
-                    ):
-                        yield piece
-                    else:
-                        partial = piece
-
-            else:
-                length = self.fileinfo[i]["length"]
-                for pad in self._gen_padding(partial, length):
-                    if len(pad) == self.piece_length:
-                        yield pad
-                    else:
-                        partial = pad
-            self.prog_close()
-
-    def extract(self, path: str, partial: bytearray) -> bytearray:
-        """
-        Split file paths contents into blocks of data for hash pieces.
-
-        Parameters
-        ----------
-        path : str
-            path to content.
-        partial : bytes
-            any remaining content from last file.
-
-        Returns
-        -------
-        bytearray
-            Hash digest for block of .torrent contents.
-        """
-        read = 0
-        length = self.fileinfo[self.index]["length"]
-        partial = bytearray() if len(partial) == self.piece_length else partial
-        if path not in self.paths:  # pragma: no cover
-            raise MissingPathError(path)
-        with open(path, "rb") as current:
-            while True:
-                bitlength = self.piece_length - len(partial)
-                part = bytearray(bitlength)
-                amount = current.readinto(part)
-                read += amount
-                partial.extend(part[:amount])
-                if amount < bitlength:
-                    if amount > 0 and read == length:
-                        self.prog_update(amount)
-                        yield partial
-                    break
-                self.prog_update(amount)
-                yield partial
-                partial = bytearray(0)
-        if length != read:
-            for pad in self._gen_padding(partial, length, read):
-                yield pad
-
-    def _gen_padding(self, partial: bytes, length: int, read=0) -> bytes:
-        """
-        Create padded pieces where file sizes do not match.
-
-        Parameters
-        ----------
-        partial : bytes
-            any remaining data from last file processed.
-        length : int
-            size of space that needs padding
-        read : int
-            portion of length already padded
-
-        Yields
-        ------
-        bytes
-            A piece length sized block of zeros.
-        """
-        while read < length:
-            left = self.piece_length - len(partial)
-            if length - read > left:
-                padding = bytearray(left)
-                partial.extend(padding)
-                yield partial
-                read += left
-                partial = bytearray(0)
-            else:
-                partial.extend(bytearray(length - read))
-                read = length
-                yield partial
-
-
-class HashChecker(ProgMixin):
-    """
-    Iterate through contents of meta data and verify with file contents.
-
-    Parameters
-    ----------
-    checker : Checker
-        the checker instance that maintains variables.
-    """
-
-    def __init__(self, checker: Checker):
-        """
-        Construct a HybridChecker instance.
-        """
-        self.checker = checker
-        self.paths = checker.paths
-        self.piece_length = checker.piece_length
-        self.fileinfo = checker.fileinfo
-        self.piece_layers = checker.meta["piece layers"]
-        self.current = None
-        self.index = -1
-
-    def __iter__(self):
-        """
-        Assign iterator and return self.
-        """
-        return self
-
-    def __next__(self):
-        """
-        Provide the result of comparison.
-        """
-        if self.current is None:
-            self.next_file()
-        try:
-            return self.process_current()
-        except StopIteration as itererr:
-            if self.next_file():
-                return self.process_current()
-            raise StopIteration from itererr
-
-    class Padder:
-        """
-        Padding class to generate padding hashes wherever needed.
-
-        Parameters
-        ----------
-        length: int
-            the total size of the mock file generating padding for.
-        piece_length : int
-            the block size that each hash represents.
-        """
-
-        def __init__(self, length, piece_length):
-            """
-            Construct padding class to Mock missing or incomplete files.
-
-            Parameters
-            ----------
-            length : int
-                size of the file
-            piece_length : int
-                the piece length for each iteration.
-            """
-            self.length = length
-            self.piece_length = piece_length
-            self.pad = sha256(bytearray(piece_length)).digest()
-
-        def __iter__(self):
-            """
-            Return self to correctly implement iterator type.
-            """
-            return self  # pragma: nocover
-
-        def __next__(self) -> bytes:
-            """
-            Iterate through seemingly endless sha256 hashes of zeros.
-
-            Returns
-            -------
-            tuple :
-                returns the padding
-
-            Raises
-            ------
-            StopIteration
-            """
-            if self.length >= self.piece_length:
-                self.length -= self.piece_length
-                return self.pad
-            if self.length > 0:
-                pad = sha256(bytearray(self.length)).digest()
-                self.length -= self.length
-                return pad
-            raise StopIteration
-
-    def next_file(self) -> bool:
-        """
-        Remove all references to  processed files and prepare for the next.
-
-        Returns
-        -------
-        bool
-            if there is a next file found
-        """
-        self.index += 1
-        self.prog_close()
-        if self.current is None or self.index < len(self.paths):
-            self.current = self.paths[self.index]
-            self.length = self.fileinfo[self.index]["length"]
-            self.root_hash = self.fileinfo[self.index]["pieces root"]
-            if self.length > self.piece_length:
-                self.pieces = self.piece_layers[self.root_hash]
-            else:
-                self.pieces = self.root_hash
-            path = self.paths[self.index]
-            self.prog_start(self.length, path, unit="bytes")
-            self.count = 0
-            if os.path.exists(self.current):
-                self.hasher = FileHasher(path, self.piece_length, progress=0)
-            else:
-                self.hasher = self.Padder(self.length, self.piece_length)
-            return True
-        if self.index >= len(self.paths):
-            del self.current
-            del self.length
-            del self.root_hash
-            del self.pieces
-        return False
-
-    def process_current(self) -> tuple:
-        """
-        Gather necessary information to compare to metafile details.
-
-        Returns
-        -------
-        tuple
-            a tuple containing the layer, piece, current path and size
-
-        Raises
-        ------
-        StopIteration
-        """
-        try:
-            layer = next(self.hasher)
-            piece, size = self.advance()
-            self.prog_update(size)
-            return layer, piece, self.current, size
-        except StopIteration as err:
-            if self.length > 0 and self.count * SHA256 < len(self.pieces):
-                self.hasher = self.Padder(self.length, self.piece_length)
-                piece, size = self.advance()
-                layer = next(self.hasher)
-                self.prog_update(0)
-                return layer, piece, self.current, size
-            raise StopIteration from err
-
-    def advance(self) -> tuple:
-        """
-        Increment the number of pieces processed for the current file.
-
-        Returns
-        -------
-        tuple
-            the piece and size
-        """
-        start = self.count * SHA256
-        end = start + SHA256
-        piece = self.pieces[start:end]
-        self.count += 1
-        if self.length >= self.piece_length:
-            self.length -= self.piece_length
-            size = self.piece_length
-        else:
-            size = self.length
-            self.length -= self.length
-        return piece, size
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Clases and functions for the rebuild or reassemble subcommand.
+
+Re-assemble a torrent into the propper directory structure as indicated by a
+torrent meta file, and validate the contents of each file allong the
+way. Displays a progress bar for each torrent.
+"""
+import logging
+import math
+import os
+from hashlib import sha1
+from pathlib import Path
+
+import pyben
+
+from torrentfile.hasher import HasherV2
+from torrentfile.mixins import CbMixin, ProgMixin
+from torrentfile.utils import copypath
+
+logger = logging.getLogger(__name__)
+SHA1 = 20
+
+
+class PathNode:
+    """
+    Base class representing information regarding a file included in torrent.
+    """
+
+    def __init__(
+        self,
+        start: int = None,
+        stop: int = None,
+        full: str = None,
+        filename: str = None,
+        path: str = None,
+        length: int = None,
+    ):
+        """
+        Hold file information that contributes to the contents of torrent.
+
+        Parameters
+        ----------
+        start : int, optional
+            where the piece starts, by default None
+        stop : int, optional
+            where the piece ends, by default None
+        full : str, optional
+            full path, by default None
+        filename : str, optional
+            filename, by default None
+        path : str, optional
+            parent path, by default None
+        length : int, optional
+            size, by default None
+        """
+        self.path = path
+        self.start = start
+        self.stop = stop
+        self.length = length
+        self.filename = filename
+        self.full = full
+
+    def get_part(self, path: str) -> bytes:
+        """
+        Extract the part of the file needed to complete the hash.
+
+        Parameters
+        ----------
+        path : str
+            filesystem path location of file.
+
+        Returns
+        -------
+        bytes
+            part of the file's contents
+        """
+        with open(path, "rb") as fd:
+            if self.start:
+                fd.seek(self.start)
+            if self.stop != -1:
+                partial = fd.read(self.stop - self.start)
+            else:
+                partial = fd.read()
+        return partial
+
+    def __len__(self) -> int:
+        """
+        Return size of the file.
+
+        Returns
+        -------
+        int
+            total size
+        """
+        return self.length
+
+
+class PieceNode:
+    """
+    Base class representing a single SHA1 hash block of data from a torrent.
+    """
+
+    def __init__(self, piece: bytes):
+        """
+        Store information about an individual SHA1 hash for a torrent file.
+
+        _extended_summary_
+
+        Parameters
+        ----------
+        piece : bytes
+            SHA1 hash bytes
+        """
+        self.piece = piece
+        self.paths = []
+        self.result = None
+        self.dest = None
+
+    def append(self, pathnode: PathNode):
+        """
+        Append the path argument to the paths list attribute.
+
+        Parameters
+        ----------
+        pathnode : PathNode
+            the pathnode
+        """
+        self.paths.append(pathnode)
+
+    def _find_matches(self, filemap: dict, paths: list, data: bytes) -> bool:
+        """
+        Gather relavent sections of the files in the list and check the hash.
+
+        Parameters
+        ----------
+        filemap : dict
+            dictionary containing filename and path details
+        paths : list
+            list of pathnodes
+        data : bytes
+            raw file contents
+
+        Returns
+        -------
+        bool
+            success state
+        """
+        if not paths:
+            piece_hash = sha1(data).digest()  # nosec
+            return piece_hash == self.piece
+        pathnode = paths[0]
+        filename = pathnode.filename
+        if filename not in filemap:
+            return False  # pragma: nocover
+        for loc, size in filemap[filename]:
+            if size != len(pathnode):
+                continue
+            partial = pathnode.get_part(loc)
+            val = self._find_matches(filemap, paths[1:], data + partial)
+            if val:
+                dest_path = os.path.join(self.dest, pathnode.full)
+                copypath(loc, dest_path)
+            return val
+        return False
+
+    def find_matches(self, filemap: dict, dest: str) -> bool:
+        """
+        Find the matching files for each path in the node.
+
+        Parameters
+        ----------
+        filemap : dict
+            filename and details
+        dest : str
+            target destination path
+
+        Returns
+        -------
+        bool
+            success status
+        """
+        self.dest = dest
+        self.result = self._find_matches(filemap, self.paths[:], bytes())
+        return self.result
+
+
+class Metadata(CbMixin, ProgMixin):
+    """
+    Class containing the metadata contents of a torrent file.
+    """
+
+    def __init__(self, path: str):
+        """
+        Construct metadata object for torrent info.
+
+        Parameters
+        ----------
+        path : str
+            path to the .torrent file.
+        """
+        self.path = os.path.abspath(path)
+        self.name = None
+        self.piece_length = 1
+        self.meta_version = 1
+        self.pieces = b""
+        self.piece_nodes = []
+        self.length = 0
+        self.files = []
+        self.filenames = set()
+        self.extract()
+        if self.meta_version == 2:
+            self.num_pieces = len(self.filenames)
+        else:
+            self.num_pieces = math.ceil(len(self.pieces) / SHA1)
+
+    def extract(self):
+        """
+        Decode and extract information for the .torrent file.
+        """
+        meta = pyben.load(self.path)
+        info = meta["info"]
+        self.piece_length = info["piece length"]
+        self.name = info["name"]
+        self.meta_version = info.get("meta version", 1)
+        self.pieces = info.get("pieces", bytes())
+        if self.meta_version == 2:
+            self._parse_tree(info["file tree"], [self.name])
+        elif "length" in info:
+            self.length += info["length"]
+            self.is_file = True
+            self.filenames.add(info["name"])
+            self.files.append(
+                {
+                    "path": Path(self.name).parent,
+                    "filename": self.name,
+                    "full": self.name,
+                    "length": self.length,
+                }
+            )
+        elif "files" in info:
+            for f in info["files"]:
+                path = f["path"]
+                full = os.path.join(self.name, *path)
+                self.files.append(
+                    {
+                        "path": Path(full).parent,
+                        "filename": path[-1],
+                        "full": full,
+                        "length": f["length"],
+                    }
+                )
+                self.length += f["length"]
+                self.filenames.add(path[-1])
+
+    def _map_pieces(self):
+        """
+        Create PathNode and PieceNode details for each piece in the torrent.
+        """
+        total_pieces = len(self.pieces) // SHA1
+        remainder = file_index = 0
+        current = {}
+        for i in range(total_pieces):
+            begin = SHA1 * i
+            piece = PieceNode(self.pieces[begin: begin + SHA1])
+            target = self.piece_length
+            if remainder:
+                start = current["length"] - remainder
+                if remainder < target:
+                    stop = -1
+                    target -= remainder
+                    remainder = 0
+                    file_index += 1
+                else:
+                    stop = start + target
+                    remainder -= target
+                    target -= target
+                pathnode = PathNode(start=start, stop=stop, **current)
+                piece.append(pathnode)
+            while target > 0 and file_index < len(self.files):
+                start = 0
+                current = self.files[file_index]
+                size = current["length"]
+                if size < target:
+                    stop = -1
+                    target -= size
+                    file_index += 1
+                else:
+                    stop = target
+                    remainder = size - target
+                    target = 0
+                pathnode = PathNode(start=start, stop=stop, **current)
+                piece.append(pathnode)
+            self.piece_nodes.append(piece)
+
+    def _parse_tree(self, tree: dict, partials: list):
+        """
+        Parse the file tree dictionary of the torrent metafile.
+
+        Parameters
+        ----------
+        tree : dict
+            the dictionary representation of a file tree.
+        partials : list
+            list of paths leading up to the current key value.
+        """
+        for key, val in tree.items():
+            if "" in val:
+                self.filenames.add(key)
+                path = Path(os.path.join(*partials))
+                full = Path(os.path.join(path, key))
+                length = val[""]["length"]
+                root = val[""]["pieces root"]
+                self.files.append(
+                    {
+                        "path": path,
+                        "full": full,
+                        "filename": key,
+                        "length": length,
+                        "root": root,
+                    }
+                )
+                self.length += length
+            else:
+                self._parse_tree(val, partials + [key])
+
+    def _match_v1(self, filemap: dict, dest: str):
+        """
+        Check each of the nodes against the filemap dictionary for matches.
+
+        Parameters
+        ----------
+        filemap : dict
+            filenames and filesystem information
+        dest : str
+            target destination path
+        """
+        self._map_pieces()
+        copied = []
+        for piece_node in self.piece_nodes:
+            paths = piece_node.paths
+            if len(paths) == 1 and paths[0].path in copied:
+                self._update()
+                continue
+            if piece_node.find_matches(filemap, dest):
+                for pathnode in paths:
+                    if pathnode.path not in copied:
+                        copied.append(pathnode.path)
+                        dest_path = os.path.join(dest, pathnode.path)
+                        self._update()
+                        self.cb(pathnode.path, dest_path, self.num_pieces)
+
+    def _match_v2(self, filemap: dict, dest: str):
+        """
+        Rebuild method for torrent v2 files.
+
+        Parameters
+        ----------
+        filemap : dict
+            filesystem information
+        dest : str
+            destiantion path
+        """
+        for entry in self.files:
+            filename = entry["filename"]
+            length = entry["length"]
+            if filename not in filemap:
+                continue  # pragma: nocover
+            paths = filemap[filename]
+            for path, size in paths:
+                if size == length:
+                    hasher = HasherV2(path, self.piece_length, True)
+                    if entry["root"] == hasher.root:
+                        dest_path = os.path.join(dest, entry["full"])
+                        copypath(entry["path"], dest_path)
+                        self._update()
+                        self.cb(path, dest_path, self.num_pieces)
+                        break
+
+    def rebuild(self, filemap: dict, dest: str):
+        """
+        Rebuild torrent file contents from filemap at dest.
+
+        Searches through the contents of the meta file and compares filenames
+        with those in the filemap dict, and if found checks their contents,
+        and copies them to the destination path.
+
+        Parameters
+        ----------
+        filemap : dict
+            filesystem information
+        dest : str
+            destiantion path
+        """
+        self._prog = None
+        if self.meta_version == 2:
+            self._match_v2(filemap, dest)
+        else:
+            self._match_v1(filemap, dest)
+        if self._prog is not None:
+            self.prog_close()
+
+    def _update(self):
+        """Start and updating the progress bar."""
+        if self._prog is None:
+            self._prog = True
+            self.prog_start(self.num_pieces, self.name, unit="piece")
+        self.prog_update(1)
+
+
+class Assembler(CbMixin):
+    """
+    Does most of the work in attempting the structure of torrentfiles.
+
+    Requires three paths as arguments.
+    - torrent metafile or directory containing multiple meta files
+    - directory containing the contents of meta file
+    - directory where torrents will be re-assembled
+    """
+
+    def __init__(self, metafiles: list, contents: list, dest: str):
+        """
+        Reassemble given torrent file from given cli arguments.
+
+        Rebuild metafiles and contents into their original directory
+        structure as much as possible in the destination directory.
+        Takes two paths as parameters,
+        - file or directory containing 1 or more torrent meta files
+        - path to where the contents are belived to be located.
+
+        Parameters
+        ----------
+        metafiles : str
+            path to torrent metafile or directory containing torrent metafiles.
+        contents : str
+            path to content or directory containing content that belongs to
+            torrentfile.
+        dest: str
+            path to the directory where rebuild will take place.
+        """
+        Metadata.set_callback(self._callback)
+        self.counter = 0
+        self._lastlog = None
+        self.contents = contents
+        self.dest = dest
+        self.meta_paths = metafiles
+        self.metafiles = self._get_metafiles()
+        filenames = set()
+        for meta in self.metafiles:
+            filenames |= meta.filenames
+        self.filemap = _index_contents(self.contents, filenames)
+
+    def _callback(self, filename: str, dest: str, num_pieces: int):
+        """
+        Run the callback functions associated with Mixin for copied files.
+
+        Parameters
+        ----------
+        filename : str
+            filename
+        dest : str
+            destination path
+        num_pieces : int
+            number of hash pieces
+        """
+        self.counter += 1
+        message = f"Matched:{num_pieces} {filename} -> {dest}"
+        if message != self._lastlog:
+            self._lastlog = message
+            logger.debug(message)
+
+    def assemble_torrents(self):
+        """
+        Assemble collection of torrent files into original structure.
+
+        Returns
+        -------
+        int
+            number of files copied
+        """
+        for metafile in self.metafiles:
+            logger.info(
+                "#%s Searching contents for %s", self.counter, metafile.name
+            )
+            self.rebuild(metafile)
+        return self.counter
+
+    def rebuild(self, metafile: Metadata) -> None:
+        """
+        Build the torrent file structure from contents of directory.
+
+        Traverse contents dir and compare discovered files
+        with files listed in torrent metadata and copy
+        the matches to the destination directory respecting folder
+        structures along the way.
+        """
+        metafile.rebuild(self.filemap, self.dest)
+
+    def _iter_files(self, path: str) -> list:
+        """
+        Iterate through metfiles directory createing Metafile objects.
+
+        Parameters
+        ----------
+        path : str
+            fs path
+
+        Returns
+        -------
+        list
+            list of Metadata Object
+        """
+        metafiles = []
+        for filename in os.listdir(path):
+            if filename.lower().endswith(".torrent"):
+                try:
+                    meta = Metadata(os.path.join(path, filename))
+                    metafiles.append(meta)
+                except ValueError:  # pragma: nocover
+                    self.counter -= 1
+        return metafiles
+
+    def _get_metafiles(self) -> list:
+        """
+        Collect all .torrent meta files from given directory or file.
+
+        Returns
+        -------
+        list
+            metafile objects
+        """
+        metafiles = []
+        for path in self.meta_paths:
+            if os.path.exists(path):
+                if os.path.isdir(path):
+                    metafiles += self._iter_files(path)
+                elif path.lower().endswith(".torrent"):
+                    meta = Metadata(path)
+                    metafiles.append(meta)
+        return metafiles
+
+
+def _index_contents(contents: list, filenames: set) -> dict:
+    """
+    Collect all of the filenames and their respective paths.
+
+    Parameters
+    ----------
+    contents : list
+        paths to traverse looking for filenames
+    filenames : set
+        set of filenames to look for
+
+    Returns
+    -------
+    dict
+        all filenames and their respective paths.
+    """
+    mapping = {}
+    for dirpath in contents:
+        mapped = _index_content(dirpath, filenames)
+        for key, value in mapped.items():
+            mapping.setdefault(key, [])
+            mapping[key].extend(value)
+    return mapping
+
+
+def _index_content(root: str, filenames: set) -> dict:
+    """
+    Collect filenames from directory or file.
+
+    Parameters
+    ----------
+    root : str
+        path to search for filenames
+    filenames : set
+        set of filenames to search for
+
+    Returns
+    -------
+    dict
+        filenames and their respective paths
+    """
+    filemap = {}
+    if os.path.isfile(root):
+        name = os.path.basename(root)
+        if name in filenames:
+            size = os.path.getsize(root)
+            filemap.setdefault(name, [])
+            filemap[name].append((root, size))
+        return filemap
+    if os.path.isdir(root):
+        for path in os.listdir(root):
+            fullpath = os.path.join(root, path)
+            resultmap = _index_content(fullpath, filenames)
+            for key, value in resultmap.items():
+                filemap.setdefault(key, [])
+                filemap[key].extend(value)
+    return filemap
```

### Comparing `torrentfile-0.8.7/torrentfile/torrent.py` & `torrentfile-0.8.8/torrentfile/torrent.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,728 +1,728 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Classes and procedures pertaining to the creation of torrent meta files.
-
-Classes
--------
-
-- `TorrentFile`
-    construct .torrent file.
-
-- `TorrentFileV2`
-    construct .torrent v2 files using provided data.
-
-- `MetaFile`
-    base class for all MetaFile classes.
-
-Constants
----------
-
-- BLOCK_SIZE : int
-    size of leaf hashes for merkle tree.
-
-- HASH_SIZE : int
-    Length of a sha256 hash.
-
-Bittorrent V2
--------------
-
-**From Bittorrent.org Documentation pages.**
-
-*Implementation details for Bittorrent Protocol v2.*
-
-!!!Note
-    All strings in a .torrent file that contain text must be UTF-8 encoded.
-
-### Meta Version 2 Dictionary:
-
-- "announce":
-    The URL of the tracker.
-
-- "info":
-    This maps to a dictionary, with keys described below.
-
-    - "name":
-        A display name for the torrent. It is purely advisory.
-
-    - "piece length":
-        The number of bytes that each logical piece in the peer
-        protocol refers to. I.e. it sets the granularity of piece, request,
-        bitfield and have messages. It must be a power of two and at least
-        6KiB.
-
-    - "meta version":
-        An integer value, set to 2 to indicate compatibility
-        with the current revision of this specification. Version 1 is not
-        assigned to avoid confusion with BEP3. Future revisions will only
-        increment this issue to indicate an incompatible change has been made,
-        for example that hash algorithms were changed due to newly discovered
-        vulnerabilities. Lementations must check this field first and indicate
-        that a torrent is of a newer version than they can handle before
-        performing other idations which may result in more general messages
-        about invalid files. Files are mapped into this piece address space so
-        that each non-empty
-
-    - "file tree":
-        A tree of dictionaries where dictionary keys represent UTF-8
-        encoded path elements. Entries with zero-length keys describe the
-        properties of the composed path at that point. 'UTF-8 encoded'
-        context only means that if the native encoding is known at creation
-        time it must be converted to UTF-8. Keys may contain invalid UTF-8
-        sequences or characters and names that are reserved on specific
-        filesystems. Implementations must be prepared to sanitize them. On
-        platforms path components exactly matching '.' and '..' must be
-        sanitized since they could lead to directory traversal attacks and
-        conflicting path descriptions. On platforms that require UTF-8
-        path components this sanitizing step must happen after normalizing
-        overlong UTF-8 encodings.
-        File is aligned to a piece boundary and occurs in same order as
-        the file tree. The last piece of each file may be shorter than the
-        specified piece length, resulting in an alignment gap.
-
-    - "length":
-        Length of the file in bytes. Presence of this field indicates
-        that the dictionary describes a file, not a directory. Which means
-        it must not have any sibling entries.
-
-    - "pieces root":
-        For non-empty files this is the the root hash of a merkle
-        tree with a branching factor of 2, constructed from 16KiB blocks
-        of the file. The last block may be shorter than 16KiB. The
-        remaining leaf hashes beyond the end of the file required to
-        construct upper layers of the merkle tree are set to zero. As of
-        meta version 2 SHA2-256 is used as digest function for the merkle
-        tree. The hash is stored in its binary form, not as human-readable
-        string.
-
-- "piece layers":
-    A dictionary of strings. For each file in the file tree that
-    is larger than the piece size it contains one string value.
-    The keys are the merkle roots while the values consist of concatenated
-    hashes of one layer within that merkle tree. The layer is chosen so
-    that one hash covers piece length bytes. For example if the piece
-    size is 16KiB then the leaf hashes are used. If a piece size of
-    128KiB is used then 3rd layer up from the leaf hashes is used. Layer
-    hashes which exclusively cover data beyond the end of file, i.e.
-    are only needed to balance the tree, are omitted. All hashes are
-    stored in their binary format. A torrent is not valid if this field is
-    absent, the contained hashes do not match the merkle roots or are
-    not from the correct layer.
-
-!!!important
-    The file tree root dictionary itself must not be a file,
-    i.e. it must not contain a zero-length key with a dictionary containing
-    a length key.
-
-Bittorrent V1
--------------
-
-### v1 meta-dictionary
-
-- announce:
-    The URL of the tracker.
-
-- info:
-    This maps to a dictionary, with keys described below.
-
-    - `name`:
-        maps to a UTF-8 encoded string which is the suggested name to
-        save the file (or directory) as. It is purely advisory.
-
-    - `piece length`:
-        maps to the number of bytes in each piece the file is split
-        into. For the purposes of transfer, files are split into
-        fixed-size pieces which are all the same length except for
-        possibly the last one which may be truncated.
-
-    - `piece length`:
-        is almost always a power of two, most commonly 2^18 = 256 K
-
-    - `pieces`:
-        maps to a string whose length is a multiple of 20. It is to be
-        subdivided into strings of length 20, each of which is the SHA1
-        hash of the piece at the corresponding index.
-
-    - `length`:
-        In the single file case, maps to the length of the file in bytes.
-
-    - `files`:
-        If present then the download represents a single file, otherwise it
-        represents a set of files which go in a directory structure.
-        For the purposes of the other keys, the multi-file case is treated
-        as only having a single file by concatenating the files in the order
-        they appear in the files list. The files list is the value `files`
-        maps to, and is a list of dictionaries containing the following keys:
-
-        - `path`:
-            A list of UTF-8 encoded strings corresponding to subdirectory
-            names, the last of which is the actual file name
-
-        - `length`:
-            Maps to the length of the file in bytes.
-
-    - `length`:
-        Only present if the content is a single file. Maps to the length
-        of the file in bytes.
-
-!!!Note
-    In the single file case, the name key is the name of a file,
-    in the muliple file case, it's the name of a directory.
-"""
-
-import logging
-import os
-from collections.abc import Sequence
-from datetime import datetime
-
-import pyben
-
-from torrentfile import utils
-from torrentfile.hasher import FileHasher, Hasher, HasherHybrid, HasherV2
-from torrentfile.mixins import ProgMixin
-from torrentfile.version import __version__ as version
-
-logger = logging.getLogger(__name__)
-
-
-class MetaFile:
-    """
-    Base Class for all TorrentFile classes.
-
-    Parameters
-    ----------
-    path : str
-        target path to torrent content.  Default: None
-    announce : str
-        One or more tracker URL's.  Default: None
-    comment : str
-        A comment.  Default: None
-    piece_length : int
-        Size of torrent pieces.  Default: None
-    private : bool
-        For private trackers.  Default: None
-    outfile : str
-        target path to write .torrent file. Default: None
-    source : str
-        Private tracker source. Default: None
-    progress : str
-        level of progress bar displayed  Default: "1"
-    cwd : bool
-        If True change default save location to current directory
-    httpseeds : list
-        one or more web addresses where torrent content can be found.
-    url_list : list
-        one or more web addressess where torrent content exists.
-    content : str
-        alias for 'path' arg.
-    meta_version : int
-        indicates which Bittorrent protocol to use for hashing content
-    """
-
-    hasher = None
-
-    @classmethod
-    def set_callback(cls, func):
-        """
-        Assign a callback function for the Hashing class to call for each hash.
-
-        Parameters
-        ----------
-        func : function
-            The callback function which accepts a single paramter.
-        """
-        if "hasher" in vars(cls) and vars(cls)["hasher"]:
-            cls.hasher.set_callback(func)
-
-    def __init__(
-        self,
-        path=None,
-        announce=None,
-        comment=None,
-        piece_length=None,
-        private=False,
-        outfile=None,
-        source=None,
-        progress=1,
-        cwd=False,
-        httpseeds=None,
-        url_list=None,
-        content=None,
-        meta_version=None,
-        **_,
-    ):
-        """
-        Construct MetaFile superclass and assign local attributes.
-        """
-        self.private = private
-        self.cwd = cwd
-        self.outfile = outfile
-        self.progress = int(progress)
-        self.comment = comment
-        self.source = source
-        self.meta_version = meta_version
-
-        if content:
-            path = content
-        if not path:
-            if announce and len(announce) > 1 and os.path.exists(announce[-1]):
-                path = announce[-1]
-                announce = announce[:-1]
-            elif url_list and os.path.exists(url_list[-1]):
-                path = url_list[-1]
-                url_list = url_list[:-1]
-            elif httpseeds and os.path.exists(httpseeds[-1]):
-                path = httpseeds[-1]
-                httpseeds = httpseeds[:-1]
-            else:
-                raise utils.MissingPathError("Path to content is required.")
-
-        # base path to torrent content.
-        self.path = path
-
-        logger.debug("path parameter found %s", path)
-
-        # Format piece_length attribute.
-        if piece_length:
-            self.piece_length = utils.normalize_piece_length(piece_length)
-            logger.debug("piece length parameter found %s", piece_length)
-        else:
-            self.piece_length = utils.path_piece_length(self.path)
-            logger.debug("piece length calculated %s", self.piece_length)
-
-        # Assign announce URL to empty string if none provided.
-        if not announce:
-            self.announce, self.announce_list = "", [[""]]
-
-        # Most torrent clients have editting trackers as a feature.
-        elif isinstance(announce, str):
-            self.announce, self.announce_list = announce, [[announce]]
-
-        elif isinstance(announce, Sequence):
-            self.announce, self.announce_list = announce[0], [announce]
-
-        self.meta = {
-            "announce": self.announce,
-            "announce-list": self.announce_list,
-            "created by": f"TorrentFile_v{version}",
-            "creation date": int(datetime.timestamp(datetime.now())),
-            "info": {},
-        }
-        if comment:
-            self.meta["info"]["comment"] = comment
-            logger.debug("comment parameter found %s", comment)
-        if private:
-            self.meta["info"]["private"] = 1
-            logger.debug("private parameter triggered")
-        if source:
-            self.meta["info"]["source"] = source
-            logger.debug("source parameter found %s", source)
-        if url_list:
-            self.meta["url-list"] = url_list
-            logger.debug("url list parameter found %s", str(url_list))
-        if httpseeds:
-            self.meta["httpseeds"] = httpseeds
-            logger.debug("httpseeds parameter found %s", str(httpseeds))
-        self.meta["info"]["piece length"] = self.piece_length
-
-        self.meta_version = meta_version
-        parent, self.name = os.path.split(self.path)
-        if not self.name:
-            self.name = os.path.basename(parent)
-        self.meta["info"]["name"] = self.name
-
-    def assemble(self):
-        """
-        Overload in subclasses.
-
-        Raises
-        ------
-        Exception
-            NotImplementedError
-        """
-        raise NotImplementedError
-
-    def sort_meta(self):
-        """Sort the info and meta dictionaries."""
-        logger.debug("sorting dictionary keys")
-        meta = self.meta
-        meta["info"] = dict(sorted(list(meta["info"].items())))
-        meta = dict(sorted(list(meta.items())))
-        return meta
-
-    def write(self, outfile=None) -> tuple:
-        """
-        Write meta information to .torrent file.
-
-        Final step in the torrent file creation process.
-        After hashing and sorting every piece of content
-        write the contents to file using the bencode encoding.
-
-        Parameters
-        ----------
-        outfile : str
-            Destination path for .torrent file. default=None
-
-        Returns
-        -------
-        outfile : str
-            Where the .torrent file was writen.
-        meta : dict
-            .torrent meta information.
-        """
-        if outfile:
-            self.outfile = outfile
-        elif self.outfile:
-            pass
-        else:
-            self.outfile = os.path.join(os.getcwd(), self.name) + ".torrent"
-        if str(self.outfile)[-1] in "\\/":
-            self.outfile = self.outfile + (self.name + ".torrent")
-        self.meta = self.sort_meta()
-        try:
-            pyben.dump(self.meta, self.outfile)
-        except PermissionError as excp:
-            logger.error(
-                "Permission Denied: Could not write to %s", self.outfile
-            )
-            raise PermissionError from excp
-        return self.outfile, self.meta
-
-
-class TorrentFile(MetaFile, ProgMixin):
-    """
-    Class for creating Bittorrent meta files.
-
-    Construct *Torrentfile* class instance object.
-
-    Parameters
-    ----------
-    **kwargs : dict
-        Dictionary containing torrent file options.
-    """
-
-    hasher = Hasher
-
-    def __init__(self, **kwargs):
-        """
-        Construct TorrentFile instance with given keyword args.
-
-        Parameters
-        ----------
-        **kwargs : dict
-            dictionary of keyword args passed to superclass.
-        """
-        super().__init__(**kwargs)
-        logger.debug("Assembling bittorrent v1 torrent file")
-        self.assemble()
-
-    def assemble(self):
-        """
-        Assemble components of torrent metafile.
-
-        Returns
-        -------
-        dict
-            metadata dictionary for torrent file
-        """
-        info = self.meta["info"]
-        size, filelist = utils.filelist_total(self.path)
-        if os.path.isfile(self.path):
-            info["length"] = size
-        else:
-            info["files"] = [
-                {
-                    "length": os.path.getsize(path),
-                    "path": os.path.relpath(path, self.path).split(os.sep),
-                }
-                for path in filelist
-            ]
-        pieces = bytearray()
-
-        feeder = Hasher(filelist, self.piece_length, self.progress)
-        for piece in feeder:
-            pieces.extend(piece)
-
-        info["pieces"] = pieces
-
-
-class TorrentFileV2(MetaFile, ProgMixin):
-    """
-    Class for creating Bittorrent meta v2 files.
-
-    Parameters
-    ----------
-    **kwargs : dict
-        Keyword arguments for torrent file options.
-    """
-
-    hasher = HasherV2
-
-    def __init__(self, **kwargs):
-        """
-        Construct `TorrentFileV2` Class instance from given parameters.
-
-        Parameters
-        ----------
-        **kwargs : dict
-            keywword arguments to pass to superclass.
-        """
-        super().__init__(**kwargs)
-        logger.debug("Assembling bittorrent v2 torrent file")
-        self.piece_layers = {}
-        self.hashes = []
-        self.total = len(utils.get_file_list(self.path))
-        self.assemble()
-
-    def assemble(self):
-        """
-        Assemble then return the meta dictionary for encoding.
-
-        Returns
-        -------
-        meta : dict
-            Metainformation about the torrent.
-        """
-        info = self.meta["info"]
-        if os.path.isfile(self.path):
-            info["file tree"] = {info["name"]: self._traverse(self.path)}
-            info["length"] = os.path.getsize(self.path)
-            self.prog_update(info["length"])
-        else:
-            info["file tree"] = self._traverse(self.path)
-
-        info["meta version"] = 2
-        self.meta["piece layers"] = self.piece_layers
-
-    def _traverse(self, path: str) -> dict:
-        """
-        Walk directory tree.
-
-        Parameters
-        ----------
-        path : str
-            Path to file or directory.
-        """
-        if os.path.isfile(path):
-            # Calculate Size and hashes for each file.
-            size = os.path.getsize(path)
-
-            if size == 0:
-                return {"": {"length": size}}
-
-            logger.debug("Hashing %s", str(path))
-            fhash = HasherV2(path, self.piece_length, self.progress)
-
-            if size > self.piece_length:
-                self.piece_layers[fhash.root] = fhash.piece_layer
-            return {"": {"length": size, "pieces root": fhash.root}}
-
-        file_tree = {}
-        if os.path.isdir(path):
-            for name in sorted(os.listdir(path)):
-                file_tree[name] = self._traverse(os.path.join(path, name))
-        return file_tree
-
-
-class TorrentFileHybrid(MetaFile, ProgMixin):
-    """
-    Construct the Hybrid torrent meta file with provided parameters.
-
-    Parameters
-    ----------
-    **kwargs : dict
-        Keyword arguments for torrent options.
-    """
-
-    hasher = HasherHybrid
-
-    def __init__(self, **kwargs):
-        """
-        Create Bittorrent v1 v2 hybrid metafiles.
-        """
-        super().__init__(**kwargs)
-        logger.debug("Assembling bittorrent Hybrid file")
-        self.name = os.path.basename(self.path)
-        self.hashes = []
-        self.piece_layers = {}
-        self.pieces = []
-        self.files = []
-        self.total = len(utils.get_file_list(self.path))
-        self.assemble()
-
-    def assemble(self):
-        """
-        Assemble the parts of the torrentfile into meta dictionary.
-        """
-        info = self.meta["info"]
-        info["meta version"] = 2
-
-        if os.path.isfile(self.path):
-            info["file tree"] = {self.name: self._traverse(self.path)}
-            info["length"] = os.path.getsize(self.path)
-
-        else:
-            info["file tree"] = self._traverse(self.path)
-            info["files"] = self.files
-
-        info["pieces"] = b"".join(self.pieces)
-        self.meta["piece layers"] = self.piece_layers
-        return info
-
-    def _traverse(self, path: str) -> dict:
-        """
-        Build meta dictionary while walking directory.
-
-        Parameters
-        ----------
-        path : str
-            Path to target file.
-        """
-        if os.path.isfile(path):
-            file_size = os.path.getsize(path)
-
-            self.files.append(
-                {
-                    "length": file_size,
-                    "path": os.path.relpath(path, self.path).split(os.sep),
-                }
-            )
-
-            if file_size == 0:
-                return {"": {"length": file_size}}
-
-            logger.debug("Hashing %s", str(path))
-            file_hash = HasherHybrid(path, self.piece_length, self.progress)
-            self.prog_update(file_size)
-
-            if file_size > self.piece_length:
-                self.piece_layers[file_hash.root] = file_hash.piece_layer
-
-            self.hashes.append(file_hash)
-            self.pieces.extend(file_hash.pieces)
-
-            if file_hash.padding_file:
-                self.files.append(file_hash.padding_file)
-
-            return {"": {"length": file_size, "pieces root": file_hash.root}}
-
-        tree = {}
-        if os.path.isdir(path):
-            for name in sorted(os.listdir(path)):
-                tree[name] = self._traverse(os.path.join(path, name))
-        return tree
-
-
-class TorrentAssembler(MetaFile):
-    """
-    Assembler class for Bittorrent version 2 and hybrid meta files.
-
-    This differs from the TorrentFileV2 and TorrentFileHybrid, because
-    it can be used as an iterator and works for both versions.
-
-    Parameters
-    ----------
-    **kwargs : dict
-        Keyword arguments for torrent options.
-    """
-
-    hasher = FileHasher
-
-    def __init__(self, **kwargs):
-        """
-        Create Bittorrent v1 v2 hybrid metafiles.
-        """
-        super().__init__(**kwargs)
-        logger.debug("Assembling bittorrent Hybrid file")
-        self.name = os.path.basename(self.path)
-        self.hashes = []
-        self.piece_layers = {}
-        self.pieces = bytearray()
-        self.files = []
-        self.hybrid = self.meta_version == "3"
-        self.total = len(utils.get_file_list(self.path))
-        self.assemble()
-
-    def assemble(self):
-        """
-        Assemble the parts of the torrentfile into meta dictionary.
-        """
-        info = self.meta["info"]
-        info["meta version"] = 2
-
-        if os.path.isfile(self.path):
-            info["file tree"] = {self.name: self._traverse(self.path)}
-            info["length"] = os.path.getsize(self.path)
-
-        else:
-            info["file tree"] = self._traverse(self.path)
-            if self.hybrid:
-                info["files"] = self.files
-
-        if self.hybrid:
-            info["pieces"] = self.pieces
-        self.meta["piece layers"] = self.piece_layers
-        return info
-
-    def _traverse(self, path: str) -> dict:
-        """
-        Build meta dictionary while walking directory.
-
-        Parameters
-        ----------
-        path : str
-            Path to target file.
-        """
-        if os.path.isfile(path):
-            file_size = os.path.getsize(path)
-            if self.hybrid:
-                self.files.append(
-                    {
-                        "length": file_size,
-                        "path": os.path.relpath(path, self.path).split(os.sep),
-                    }
-                )
-
-            if file_size == 0:
-                return {"": {"length": file_size}}
-
-            logger.debug("Hashing %s", str(path))
-            hasher = FileHasher(
-                path, self.piece_length, progress=True, hybrid=self.hybrid
-            )
-            layers = bytearray()
-            for result in hasher:
-                if self.hybrid:
-                    layer_hash, piece = result
-                    self.pieces.extend(piece)
-                else:
-                    layer_hash = result
-                layers.extend(layer_hash)
-            if file_size > self.piece_length:
-                self.piece_layers[hasher.root] = layers
-            if self.hybrid and hasher.padding_file:
-                self.files.append(hasher.padding_file)
-
-            return {"": {"length": file_size, "pieces root": hasher.root}}
-
-        tree = {}
-        if os.path.isdir(path):
-            for name in sorted(os.listdir(path)):
-                tree[name] = self._traverse(os.path.join(path, name))
-        return tree
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Classes and procedures pertaining to the creation of torrent meta files.
+
+Classes
+-------
+
+- `TorrentFile`
+    construct .torrent file.
+
+- `TorrentFileV2`
+    construct .torrent v2 files using provided data.
+
+- `MetaFile`
+    base class for all MetaFile classes.
+
+Constants
+---------
+
+- BLOCK_SIZE : int
+    size of leaf hashes for merkle tree.
+
+- HASH_SIZE : int
+    Length of a sha256 hash.
+
+Bittorrent V2
+-------------
+
+**From Bittorrent.org Documentation pages.**
+
+*Implementation details for Bittorrent Protocol v2.*
+
+!!!Note
+    All strings in a .torrent file that contain text must be UTF-8 encoded.
+
+### Meta Version 2 Dictionary:
+
+- "announce":
+    The URL of the tracker.
+
+- "info":
+    This maps to a dictionary, with keys described below.
+
+    - "name":
+        A display name for the torrent. It is purely advisory.
+
+    - "piece length":
+        The number of bytes that each logical piece in the peer
+        protocol refers to. I.e. it sets the granularity of piece, request,
+        bitfield and have messages. It must be a power of two and at least
+        6KiB.
+
+    - "meta version":
+        An integer value, set to 2 to indicate compatibility
+        with the current revision of this specification. Version 1 is not
+        assigned to avoid confusion with BEP3. Future revisions will only
+        increment this issue to indicate an incompatible change has been made,
+        for example that hash algorithms were changed due to newly discovered
+        vulnerabilities. Lementations must check this field first and indicate
+        that a torrent is of a newer version than they can handle before
+        performing other idations which may result in more general messages
+        about invalid files. Files are mapped into this piece address space so
+        that each non-empty
+
+    - "file tree":
+        A tree of dictionaries where dictionary keys represent UTF-8
+        encoded path elements. Entries with zero-length keys describe the
+        properties of the composed path at that point. 'UTF-8 encoded'
+        context only means that if the native encoding is known at creation
+        time it must be converted to UTF-8. Keys may contain invalid UTF-8
+        sequences or characters and names that are reserved on specific
+        filesystems. Implementations must be prepared to sanitize them. On
+        platforms path components exactly matching '.' and '..' must be
+        sanitized since they could lead to directory traversal attacks and
+        conflicting path descriptions. On platforms that require UTF-8
+        path components this sanitizing step must happen after normalizing
+        overlong UTF-8 encodings.
+        File is aligned to a piece boundary and occurs in same order as
+        the file tree. The last piece of each file may be shorter than the
+        specified piece length, resulting in an alignment gap.
+
+    - "length":
+        Length of the file in bytes. Presence of this field indicates
+        that the dictionary describes a file, not a directory. Which means
+        it must not have any sibling entries.
+
+    - "pieces root":
+        For non-empty files this is the the root hash of a merkle
+        tree with a branching factor of 2, constructed from 16KiB blocks
+        of the file. The last block may be shorter than 16KiB. The
+        remaining leaf hashes beyond the end of the file required to
+        construct upper layers of the merkle tree are set to zero. As of
+        meta version 2 SHA2-256 is used as digest function for the merkle
+        tree. The hash is stored in its binary form, not as human-readable
+        string.
+
+- "piece layers":
+    A dictionary of strings. For each file in the file tree that
+    is larger than the piece size it contains one string value.
+    The keys are the merkle roots while the values consist of concatenated
+    hashes of one layer within that merkle tree. The layer is chosen so
+    that one hash covers piece length bytes. For example if the piece
+    size is 16KiB then the leaf hashes are used. If a piece size of
+    128KiB is used then 3rd layer up from the leaf hashes is used. Layer
+    hashes which exclusively cover data beyond the end of file, i.e.
+    are only needed to balance the tree, are omitted. All hashes are
+    stored in their binary format. A torrent is not valid if this field is
+    absent, the contained hashes do not match the merkle roots or are
+    not from the correct layer.
+
+!!!important
+    The file tree root dictionary itself must not be a file,
+    i.e. it must not contain a zero-length key with a dictionary containing
+    a length key.
+
+Bittorrent V1
+-------------
+
+### v1 meta-dictionary
+
+- announce:
+    The URL of the tracker.
+
+- info:
+    This maps to a dictionary, with keys described below.
+
+    - `name`:
+        maps to a UTF-8 encoded string which is the suggested name to
+        save the file (or directory) as. It is purely advisory.
+
+    - `piece length`:
+        maps to the number of bytes in each piece the file is split
+        into. For the purposes of transfer, files are split into
+        fixed-size pieces which are all the same length except for
+        possibly the last one which may be truncated.
+
+    - `piece length`:
+        is almost always a power of two, most commonly 2^18 = 256 K
+
+    - `pieces`:
+        maps to a string whose length is a multiple of 20. It is to be
+        subdivided into strings of length 20, each of which is the SHA1
+        hash of the piece at the corresponding index.
+
+    - `length`:
+        In the single file case, maps to the length of the file in bytes.
+
+    - `files`:
+        If present then the download represents a single file, otherwise it
+        represents a set of files which go in a directory structure.
+        For the purposes of the other keys, the multi-file case is treated
+        as only having a single file by concatenating the files in the order
+        they appear in the files list. The files list is the value `files`
+        maps to, and is a list of dictionaries containing the following keys:
+
+        - `path`:
+            A list of UTF-8 encoded strings corresponding to subdirectory
+            names, the last of which is the actual file name
+
+        - `length`:
+            Maps to the length of the file in bytes.
+
+    - `length`:
+        Only present if the content is a single file. Maps to the length
+        of the file in bytes.
+
+!!!Note
+    In the single file case, the name key is the name of a file,
+    in the muliple file case, it's the name of a directory.
+"""
+
+import logging
+import os
+from collections.abc import Sequence
+from datetime import datetime
+
+import pyben
+
+from torrentfile import utils
+from torrentfile.hasher import FileHasher, Hasher, HasherHybrid, HasherV2
+from torrentfile.mixins import ProgMixin
+from torrentfile.version import __version__ as version
+
+logger = logging.getLogger(__name__)
+
+
+class MetaFile:
+    """
+    Base Class for all TorrentFile classes.
+
+    Parameters
+    ----------
+    path : str
+        target path to torrent content.  Default: None
+    announce : str
+        One or more tracker URL's.  Default: None
+    comment : str
+        A comment.  Default: None
+    piece_length : int
+        Size of torrent pieces.  Default: None
+    private : bool
+        For private trackers.  Default: None
+    outfile : str
+        target path to write .torrent file. Default: None
+    source : str
+        Private tracker source. Default: None
+    progress : str
+        level of progress bar displayed  Default: "1"
+    cwd : bool
+        If True change default save location to current directory
+    httpseeds : list
+        one or more web addresses where torrent content can be found.
+    url_list : list
+        one or more web addressess where torrent content exists.
+    content : str
+        alias for 'path' arg.
+    meta_version : int
+        indicates which Bittorrent protocol to use for hashing content
+    """
+
+    hasher = None
+
+    @classmethod
+    def set_callback(cls, func):
+        """
+        Assign a callback function for the Hashing class to call for each hash.
+
+        Parameters
+        ----------
+        func : function
+            The callback function which accepts a single paramter.
+        """
+        if "hasher" in vars(cls) and vars(cls)["hasher"]:
+            cls.hasher.set_callback(func)
+
+    def __init__(
+        self,
+        path=None,
+        announce=None,
+        comment=None,
+        piece_length=None,
+        private=False,
+        outfile=None,
+        source=None,
+        progress=1,
+        cwd=False,
+        httpseeds=None,
+        url_list=None,
+        content=None,
+        meta_version=None,
+        **_,
+    ):
+        """
+        Construct MetaFile superclass and assign local attributes.
+        """
+        self.private = private
+        self.cwd = cwd
+        self.outfile = outfile
+        self.progress = int(progress)
+        self.comment = comment
+        self.source = source
+        self.meta_version = meta_version
+
+        if content:
+            path = content
+        if not path:
+            if announce and len(announce) > 1 and os.path.exists(announce[-1]):
+                path = announce[-1]
+                announce = announce[:-1]
+            elif url_list and os.path.exists(url_list[-1]):
+                path = url_list[-1]
+                url_list = url_list[:-1]
+            elif httpseeds and os.path.exists(httpseeds[-1]):
+                path = httpseeds[-1]
+                httpseeds = httpseeds[:-1]
+            else:
+                raise utils.MissingPathError("Path to content is required.")
+
+        # base path to torrent content.
+        self.path = path
+
+        logger.debug("path parameter found %s", path)
+
+        # Format piece_length attribute.
+        if piece_length:
+            self.piece_length = utils.normalize_piece_length(piece_length)
+            logger.debug("piece length parameter found %s", piece_length)
+        else:
+            self.piece_length = utils.path_piece_length(self.path)
+            logger.debug("piece length calculated %s", self.piece_length)
+
+        # Assign announce URL to empty string if none provided.
+        if not announce:
+            self.announce, self.announce_list = "", [[""]]
+
+        # Most torrent clients have editting trackers as a feature.
+        elif isinstance(announce, str):
+            self.announce, self.announce_list = announce, [[announce]]
+
+        elif isinstance(announce, Sequence):
+            self.announce, self.announce_list = announce[0], [announce]
+
+        self.meta = {
+            "announce": self.announce,
+            "announce-list": self.announce_list,
+            "created by": f"TorrentFile_v{version}",
+            "creation date": int(datetime.timestamp(datetime.now())),
+            "info": {},
+        }
+        if comment:
+            self.meta["info"]["comment"] = comment
+            logger.debug("comment parameter found %s", comment)
+        if private:
+            self.meta["info"]["private"] = 1
+            logger.debug("private parameter triggered")
+        if source:
+            self.meta["info"]["source"] = source
+            logger.debug("source parameter found %s", source)
+        if url_list:
+            self.meta["url-list"] = url_list
+            logger.debug("url list parameter found %s", str(url_list))
+        if httpseeds:
+            self.meta["httpseeds"] = httpseeds
+            logger.debug("httpseeds parameter found %s", str(httpseeds))
+        self.meta["info"]["piece length"] = self.piece_length
+
+        self.meta_version = meta_version
+        parent, self.name = os.path.split(self.path)
+        if not self.name:
+            self.name = os.path.basename(parent)
+        self.meta["info"]["name"] = self.name
+
+    def assemble(self):
+        """
+        Overload in subclasses.
+
+        Raises
+        ------
+        Exception
+            NotImplementedError
+        """
+        raise NotImplementedError
+
+    def sort_meta(self):
+        """Sort the info and meta dictionaries."""
+        logger.debug("sorting dictionary keys")
+        meta = self.meta
+        meta["info"] = dict(sorted(list(meta["info"].items())))
+        meta = dict(sorted(list(meta.items())))
+        return meta
+
+    def write(self, outfile=None) -> tuple:
+        """
+        Write meta information to .torrent file.
+
+        Final step in the torrent file creation process.
+        After hashing and sorting every piece of content
+        write the contents to file using the bencode encoding.
+
+        Parameters
+        ----------
+        outfile : str
+            Destination path for .torrent file. default=None
+
+        Returns
+        -------
+        outfile : str
+            Where the .torrent file was writen.
+        meta : dict
+            .torrent meta information.
+        """
+        if outfile:
+            self.outfile = outfile
+        elif self.outfile:
+            pass
+        else:
+            self.outfile = os.path.join(os.getcwd(), self.name) + ".torrent"
+        if str(self.outfile)[-1] in "\\/":
+            self.outfile = self.outfile + (self.name + ".torrent")
+        self.meta = self.sort_meta()
+        try:
+            pyben.dump(self.meta, self.outfile)
+        except PermissionError as excp:
+            logger.error(
+                "Permission Denied: Could not write to %s", self.outfile
+            )
+            raise PermissionError from excp
+        return self.outfile, self.meta
+
+
+class TorrentFile(MetaFile, ProgMixin):
+    """
+    Class for creating Bittorrent meta files.
+
+    Construct *Torrentfile* class instance object.
+
+    Parameters
+    ----------
+    **kwargs : dict
+        Dictionary containing torrent file options.
+    """
+
+    hasher = Hasher
+
+    def __init__(self, **kwargs):
+        """
+        Construct TorrentFile instance with given keyword args.
+
+        Parameters
+        ----------
+        **kwargs : dict
+            dictionary of keyword args passed to superclass.
+        """
+        super().__init__(**kwargs)
+        logger.debug("Assembling bittorrent v1 torrent file")
+        self.assemble()
+
+    def assemble(self):
+        """
+        Assemble components of torrent metafile.
+
+        Returns
+        -------
+        dict
+            metadata dictionary for torrent file
+        """
+        info = self.meta["info"]
+        size, filelist = utils.filelist_total(self.path)
+        if os.path.isfile(self.path):
+            info["length"] = size
+        else:
+            info["files"] = [
+                {
+                    "length": os.path.getsize(path),
+                    "path": os.path.relpath(path, self.path).split(os.sep),
+                }
+                for path in filelist
+            ]
+        pieces = bytearray()
+
+        feeder = Hasher(filelist, self.piece_length, self.progress)
+        for piece in feeder:
+            pieces.extend(piece)
+
+        info["pieces"] = pieces
+
+
+class TorrentFileV2(MetaFile, ProgMixin):
+    """
+    Class for creating Bittorrent meta v2 files.
+
+    Parameters
+    ----------
+    **kwargs : dict
+        Keyword arguments for torrent file options.
+    """
+
+    hasher = HasherV2
+
+    def __init__(self, **kwargs):
+        """
+        Construct `TorrentFileV2` Class instance from given parameters.
+
+        Parameters
+        ----------
+        **kwargs : dict
+            keywword arguments to pass to superclass.
+        """
+        super().__init__(**kwargs)
+        logger.debug("Assembling bittorrent v2 torrent file")
+        self.piece_layers = {}
+        self.hashes = []
+        self.total = len(utils.get_file_list(self.path))
+        self.assemble()
+
+    def assemble(self):
+        """
+        Assemble then return the meta dictionary for encoding.
+
+        Returns
+        -------
+        meta : dict
+            Metainformation about the torrent.
+        """
+        info = self.meta["info"]
+        if os.path.isfile(self.path):
+            info["file tree"] = {info["name"]: self._traverse(self.path)}
+            info["length"] = os.path.getsize(self.path)
+            self.prog_update(info["length"])
+        else:
+            info["file tree"] = self._traverse(self.path)
+
+        info["meta version"] = 2
+        self.meta["piece layers"] = self.piece_layers
+
+    def _traverse(self, path: str) -> dict:
+        """
+        Walk directory tree.
+
+        Parameters
+        ----------
+        path : str
+            Path to file or directory.
+        """
+        if os.path.isfile(path):
+            # Calculate Size and hashes for each file.
+            size = os.path.getsize(path)
+
+            if size == 0:
+                return {"": {"length": size}}
+
+            logger.debug("Hashing %s", str(path))
+            fhash = HasherV2(path, self.piece_length, self.progress)
+
+            if size > self.piece_length:
+                self.piece_layers[fhash.root] = fhash.piece_layer
+            return {"": {"length": size, "pieces root": fhash.root}}
+
+        file_tree = {}
+        if os.path.isdir(path):
+            for name in sorted(os.listdir(path)):
+                file_tree[name] = self._traverse(os.path.join(path, name))
+        return file_tree
+
+
+class TorrentFileHybrid(MetaFile, ProgMixin):
+    """
+    Construct the Hybrid torrent meta file with provided parameters.
+
+    Parameters
+    ----------
+    **kwargs : dict
+        Keyword arguments for torrent options.
+    """
+
+    hasher = HasherHybrid
+
+    def __init__(self, **kwargs):
+        """
+        Create Bittorrent v1 v2 hybrid metafiles.
+        """
+        super().__init__(**kwargs)
+        logger.debug("Assembling bittorrent Hybrid file")
+        self.name = os.path.basename(self.path)
+        self.hashes = []
+        self.piece_layers = {}
+        self.pieces = []
+        self.files = []
+        self.total = len(utils.get_file_list(self.path))
+        self.assemble()
+
+    def assemble(self):
+        """
+        Assemble the parts of the torrentfile into meta dictionary.
+        """
+        info = self.meta["info"]
+        info["meta version"] = 2
+
+        if os.path.isfile(self.path):
+            info["file tree"] = {self.name: self._traverse(self.path)}
+            info["length"] = os.path.getsize(self.path)
+
+        else:
+            info["file tree"] = self._traverse(self.path)
+            info["files"] = self.files
+
+        info["pieces"] = b"".join(self.pieces)
+        self.meta["piece layers"] = self.piece_layers
+        return info
+
+    def _traverse(self, path: str) -> dict:
+        """
+        Build meta dictionary while walking directory.
+
+        Parameters
+        ----------
+        path : str
+            Path to target file.
+        """
+        if os.path.isfile(path):
+            file_size = os.path.getsize(path)
+
+            self.files.append(
+                {
+                    "length": file_size,
+                    "path": os.path.relpath(path, self.path).split(os.sep),
+                }
+            )
+
+            if file_size == 0:
+                return {"": {"length": file_size}}
+
+            logger.debug("Hashing %s", str(path))
+            file_hash = HasherHybrid(path, self.piece_length, self.progress)
+            self.prog_update(file_size)
+
+            if file_size > self.piece_length:
+                self.piece_layers[file_hash.root] = file_hash.piece_layer
+
+            self.hashes.append(file_hash)
+            self.pieces.extend(file_hash.pieces)
+
+            if file_hash.padding_file:
+                self.files.append(file_hash.padding_file)
+
+            return {"": {"length": file_size, "pieces root": file_hash.root}}
+
+        tree = {}
+        if os.path.isdir(path):
+            for name in sorted(os.listdir(path)):
+                tree[name] = self._traverse(os.path.join(path, name))
+        return tree
+
+
+class TorrentAssembler(MetaFile):
+    """
+    Assembler class for Bittorrent version 2 and hybrid meta files.
+
+    This differs from the TorrentFileV2 and TorrentFileHybrid, because
+    it can be used as an iterator and works for both versions.
+
+    Parameters
+    ----------
+    **kwargs : dict
+        Keyword arguments for torrent options.
+    """
+
+    hasher = FileHasher
+
+    def __init__(self, **kwargs):
+        """
+        Create Bittorrent v1 v2 hybrid metafiles.
+        """
+        super().__init__(**kwargs)
+        logger.debug("Assembling bittorrent Hybrid file")
+        self.name = os.path.basename(self.path)
+        self.hashes = []
+        self.piece_layers = {}
+        self.pieces = bytearray()
+        self.files = []
+        self.hybrid = self.meta_version == "3"
+        self.total = len(utils.get_file_list(self.path))
+        self.assemble()
+
+    def assemble(self):
+        """
+        Assemble the parts of the torrentfile into meta dictionary.
+        """
+        info = self.meta["info"]
+        info["meta version"] = 2
+
+        if os.path.isfile(self.path):
+            info["file tree"] = {self.name: self._traverse(self.path)}
+            info["length"] = os.path.getsize(self.path)
+
+        else:
+            info["file tree"] = self._traverse(self.path)
+            if self.hybrid:
+                info["files"] = self.files
+
+        if self.hybrid:
+            info["pieces"] = self.pieces
+        self.meta["piece layers"] = self.piece_layers
+        return info
+
+    def _traverse(self, path: str) -> dict:
+        """
+        Build meta dictionary while walking directory.
+
+        Parameters
+        ----------
+        path : str
+            Path to target file.
+        """
+        if os.path.isfile(path):
+            file_size = os.path.getsize(path)
+            if self.hybrid:
+                self.files.append(
+                    {
+                        "length": file_size,
+                        "path": os.path.relpath(path, self.path).split(os.sep),
+                    }
+                )
+
+            if file_size == 0:
+                return {"": {"length": file_size}}
+
+            logger.debug("Hashing %s", str(path))
+            hasher = FileHasher(
+                path, self.piece_length, progress=True, hybrid=self.hybrid
+            )
+            layers = bytearray()
+            for result in hasher:
+                if self.hybrid:
+                    layer_hash, piece = result
+                    self.pieces.extend(piece)
+                else:
+                    layer_hash = result
+                layers.extend(layer_hash)
+            if file_size > self.piece_length:
+                self.piece_layers[hasher.root] = layers
+            if self.hybrid and hasher.padding_file:
+                self.files.append(hasher.padding_file)
+
+            return {"": {"length": file_size, "pieces root": hasher.root}}
+
+        tree = {}
+        if os.path.isdir(path):
+            for name in sorted(os.listdir(path)):
+                tree[name] = self._traverse(os.path.join(path, name))
+        return tree
```

### Comparing `torrentfile-0.8.7/torrentfile/utils.py` & `torrentfile-0.8.8/torrentfile/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,7 +420,34 @@
 
     Returns
     -------
     bool
         is debug mode on
     """
     return os.environ["TORRENTFILE_DEBUG"] == "ON"
+
+
+def check_path_writable(path: str) -> bool:
+    """
+    Test if output path is writable.
+
+    Parameters
+    ----------
+    path : str
+        file system path string
+
+    Returns
+    -------
+    bool
+        True if writeable, otherwise raises PermissionError
+    """
+    try:
+        if path.endswith("\\") or path.endswith("/"):
+            path = os.path.join(path, ".torrent")
+        fd = open(path, "ab")
+        fd.close()
+        os.remove(path)
+    except PermissionError as err:  # pragma: nocover
+        directory = os.path.dirname(path)
+        message = f"Target directory is not writeable {directory}"
+        raise PermissionError(message) from err
+    return True
```

### Comparing `torrentfile-0.8.7/torrentfile/version.py` & `torrentfile-0.8.8/torrentfile/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Holds the release version number.
-"""
-
-__version__ = "0.8.7"
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Holds the release version number.
+"""
+
+__version__ = "0.8.8"
```

### Comparing `torrentfile-0.8.7/torrentfile.egg-info/PKG-INFO` & `torrentfile-0.8.8/torrentfile.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrentfile
-Version: 0.8.7
+Version: 0.8.8
 Summary: Terminal based command line tool for creating Bittorrent files.
 Author-email: alexpdev <alexpdev@pm.me>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -237,15 +237,15 @@
 ![torrentfile](https://github.com/alexpdev/torrentfile/blob/master/site/images/torrentfile.png?raw=true)
 
 * * *
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/alexpdev/torrentfile?color=orange)
 ![GitHub License](https://img.shields.io/github/license/alexpdev/torrentfile?color=red&logo=apache)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/torrentfile?color=brown)
-![GitHub Last Commit](https://badgen.net/github/last-commit/alexpdev/torrentfile?color=blue&icon=github)
+![GitHub Last Commit](https://badgen.net/github/last-commit/alexpdev/torrentfile?color=blue)
 [![CI](https://github.com/alexpdev/TorrentFile/actions/workflows/pyworkflow.yml/badge.svg?branch=master&event=push)](https://github.com/alexpdev/torrentfile/actions/workflows/pyworkflow.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/b67ff65b3d574025b65b6587266bbab7)](https://www.codacy.com/gh/alexpdev/torrentfile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=alexpdev/torrentfile&utm_campaign=Badge_Coverage)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b67ff65b3d574025b65b6587266bbab7)](https://www.codacy.com/gh/alexpdev/torrentfile/dashboard?utm_source=github.com&utm_medium=referral&utm_content=alexpdev/torrentfile&utm_campaign=Badge_Grade)
 [![DeepSource](https://deepsource.io/gh/alexpdev/TorrentFile.svg/?label=active+issues&token=16Sl_dF7nTU8YgPilcqhvHm8)](https://deepsource.io/gh/alexpdev/torrentfile/)
 [![codecov](https://codecov.io/gh/alexpdev/torrentfile/branch/master/graph/badge.svg?token=EWF7NIL9SQ)](https://codecov.io/gh/alexpdev/torrentfile?color=navy&logo=codecov)
 
 ## 🌐 Overview
@@ -341,54 +341,63 @@
 torrentfile --quiet create /path/to/content
 ```
 
 ```bash
 torrentfile create /path/to/content --prog 0
 ```
 
-**`torrentfile`** automatically extracts the name of the file or directory  
-if the content and saves the file to the current working directory with the 
-extracted title.
+**`torrentfile`** extracts the name of the contents top level file or directory  
+and saves the torrent file to the current working directory with the extracted title.
 
 For example running the follwing command would create `./content.torrent`.
 
 ```bash
 torrentfile create /path/to/content
 ```
 
 To specify an alternative path or filename you may use the `-o`, `--out` flags  
 followed by the relative or absolute path to your preferred output location.
 
 ```bash
 torrentfile create /path/to/content -o /some/other/path/torrent.torrent
 ```
 
-If the path you specified with the `-o` flag already exists and is a directory,  
-then torrentfile will save the output to that directory with the default extracted title.
+If the path `--out` path specified is an existing directory, then the torrent file will be
+saved to that directory, with same filename as the default top level path name.
 
-For example the following command would create a Bittorrent file at `/some/other/path/content.torrent`.
+For example the following command would create a torrent file at `/some/other/path/content.torrent`.
 
 ```bash
 torrentfile create /path/to/content -o /some/other/path/
 ```
 
-Bittorrent V1 is still the most common version of torrent files and the most widely accepted,  
-therefore by default torrentfile uses the version 1 format.  However if you are using a modern 
-Bittorrent client and tracker then you may wish to use the newest version Bittorrent V2 or 
-a combination of the two.  To do this simply use the `--meta-version` flag with the appropriate  
-version.  Options include `1`(v1 default), `2`(v2), or `3`(v1 & v2).
+Bittorrent protocol V1 is still the most common version in use for torrent files, 
+therefore by default __`torrentfile`__ uses the version 1 format when creating the file.  
+However __`torrentfile`__ has full support for creating V2 format torrent files as well as 
+hybrid V1 & V2 format files. Use the `--meta-version` flag to specify which file format
+should be used during torrent file creation. Options include `1`(v1 default), `2`(v2), or `3`(v1 & v2).
 
 ```bash
 torrentfile create /path/to/content --meta-version 2
 ```
 
 ```bash
 torrentfile create /path/to/content --meta-version 3 
 ```
 
+__NEW FEATURE in v0.8.8__:
+
+>`torrentfile` now includes the option to command line flags for the `create` sub-command from an `ini` style
+configuration file, by using the `--config` and optional `--config-path` options to specify the path
+to the configuration file.  If `--config-path` is ommited, then `torrentfile` will look by default in the current
+working directory for a file named `torrentfile.ini`. If the file is not discovered in the current working directory, 
+it will move on to look `~/.torrentfile/torrentfile.ini` followed by `~/.config/torrentfile.ini`.  Please see the 
+[documentation](https://alexpdev.github.io/torrentfile/overview/) for more details on how the configuration file should be
+formatted.
+
 ### Check/Recheck Torrent
 
 The `recheck` subcommand allows you to scan a Bittorrent file and compare it's contents, 
 against a file or directory containing the contents the torrent file was created from.
 The output provided by this process gives a detailed perspective if any files are missing
 or have been corrupted in any way.  Supports any version of Bittorrent file.
 
@@ -404,15 +413,15 @@
 
 ```bash
 torrentfile edit /path/to/content --tracker https://new.tracker.url1.com  https://newtracker.url/2
 ```
 
 You can use the `-h` flag for a full list of available fields that can be edited.
 
-    torrentfile edit -h
+    __`torrentfile`__ edit -h
 
 ### Create Magnet
 
 To create a magnet URI for a pre-existing torrent meta file, use the sub-command  
 `magnet` or `m` with the path to the torrent file.
 
 ```bash
```

### Comparing `torrentfile-0.8.7/torrentfile.egg-info/SOURCES.txt` & `torrentfile-0.8.8/torrentfile.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 assets/torrentfile-icon.ico
 assets/torrentfile-icon.png
 assets/torrentfile.png
 c/hasher.c
 c/hasher.h
 c/sha.c
 c/sha.h
+tests/test_cli.py
+tests/test_commands.py
+tests/test_edit.py
+tests/test_interactive.py
+tests/test_rebuild.py
+tests/test_recheck.py
+tests/test_torrent.py
+tests/test_utils.py
 torrentfile/__init__.py
 torrentfile/__main__.py
 torrentfile/cli.py
 torrentfile/commands.py
 torrentfile/edit.py
 torrentfile/hasher.py
 torrentfile/interactive.py
```


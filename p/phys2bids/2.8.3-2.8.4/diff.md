# Comparing `tmp/phys2bids-2.8.3.tar.gz` & `tmp/phys2bids-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phys2bids-2.8.3.tar", last modified: Tue Mar 14 16:24:16 2023, max compression
+gzip compressed data, was "dist/phys2bids-2.8.4.tar", last modified: Wed Apr 26 22:56:47 2023, max compression
```

## Comparing `phys2bids-2.8.3.tar` & `phys2bids-2.8.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 16:24:16.000000 phys2bids-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (116)    18540 2023-03-14 16:23:55.000000 phys2bids-2.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (116)    20733 2023-03-14 16:24:16.000000 phys2bids-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       71 2023-03-14 16:23:55.000000 phys2bids-2.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2189 2023-03-14 16:24:16.000000 phys2bids-2.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids/
--rw-r--r--   0 runner    (1001) docker     (116)     9043 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/viz.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     9595 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    26696 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/physio_obj.py
--rw-r--r--   0 runner    (1001) docker     (116)    20431 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/phys2bids.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids/cli/
--rw-r--r--   0 runner    (1001) docker     (116)       41 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7634 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (116)      131 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17563 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/io.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids/heuristics/
--rw-r--r--   0 runner    (1001) docker     (116)     2140 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/heuristics/heur_test_multifreq.py
--rw-r--r--   0 runner    (1001) docker     (116)     2141 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/heuristics/heur_test_acq.py
--rw-r--r--   0 runner    (1001) docker     (116)     2143 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/heuristics/heur_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (116)     2707 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/heuristics/heur_euskalibur.py
--rw-r--r--   0 runner    (1001) docker     (116)       89 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/heuristics/participant.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     4142 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    12153 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/test_physio_obj.py
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13924 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (116)     5294 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/test_bids.py
--rw-r--r--   0 runner    (1001) docker     (116)     4504 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     7733 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     2014 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/test_phys2bids.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids/tests/data/
--rw-r--r--   0 runner    (1001) docker     (116)      623 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/data/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      399 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/tests/data/tutorial_file_INFO.json
--rw-r--r--   0 runner    (1001) docker     (116)    10236 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/bids.py
--rw-r--r--   0 runner    (1001) docker     (116)     2123 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/due.py
--rw-r--r--   0 runner    (1001) docker     (116)     6880 2023-03-14 16:23:55.000000 phys2bids-2.8.3/phys2bids/slice4phys.py
--rw-r--r--   0 runner    (1001) docker     (116)      376 2023-03-14 16:23:55.000000 phys2bids-2.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    20733 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      634 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       57 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-14 16:24:16.000000 phys2bids-2.8.3/phys2bids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)    68611 2023-03-14 16:23:55.000000 phys2bids-2.8.3/versioneer.py
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2023-03-14 16:23:55.000000 phys2bids-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      231 2023-03-14 16:23:55.000000 phys2bids-2.8.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    68611 2023-04-26 22:56:31.000000 phys2bids-2.8.4/versioneer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20731 2023-04-26 22:56:47.000000 phys2bids-2.8.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13923 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_bids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4505 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7736 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12153 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_physio_obj.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/test_phys2bids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/tests/data/tutorial_file_INFO.json
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20501 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/phys2bids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/due.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26697 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/physio_obj.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17662 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/io.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/heuristics/
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/heuristics/heur_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/heuristics/heur_euskalibur.py
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/heuristics/participant.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/heuristics/heur_test_multifreq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/heuristics/heur_test_acq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9045 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/viz.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10235 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/bids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/slice4phys.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7634 2023-04-26 22:56:31.000000 phys2bids-2.8.4/phys2bids/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-26 22:56:31.000000 phys2bids-2.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-04-26 22:56:31.000000 phys2bids-2.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20731 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-26 22:56:47.000000 phys2bids-2.8.4/phys2bids.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-26 22:56:31.000000 phys2bids-2.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    18538 2023-04-26 22:56:31.000000 phys2bids-2.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-04-26 22:56:47.000000 phys2bids-2.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-04-26 22:56:31.000000 phys2bids-2.8.4/MANIFEST.in
```

### Comparing `phys2bids-2.8.3/README.md` & `phys2bids-2.8.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -50,26 +50,26 @@
 - [Developer calls calendar](https://calendar.google.com/calendar/u/0?cid=amoycDQ1MTdhMWdpaHNuNzlnOW1ucHJkMjRAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ)
 
 ## Tested OSs
 While all version until `2.6.2` were tested on Linux and Windows, starting from version `2.7` onward we had to **drop Windows testing**. The reason is related to the cost of running such tests: for each Windows test, we can run up to 8 tests on Linux instead. Partial Windows testing might be reintroduced in future releases.
 
 Hence, while **we cannot ensure that phys2bids will run on Windows**, however we don't see any reason it shouldn't. Besides, it will run on Linux Subsistems.
 
-We apologise for the discomfort. 
+We apologise for the discomfort.
 
 
 <!-- ## Hacktoberfest
 Hacktoberfest participants, welcome!
 We have some issues for you [here](https://github.com/physiopy/phys2bids/issues?q=is%3Aissue+is%3Aopen+label%3Ahacktoberfest)!
 However, feel free to tackle any issue you'd like. Depending on the issue and extent of contribution, Hacktoberfest related PRs might not count toward being listed as contributors and authors (unless there is the specific interest). You can ask about it in the issue itself!
 Feel free to ask help to the contributors over gitter, happy coding and (hopefully) enjoy hour tee (or tree)!
 
 ## The BrainWeb
 BrainWeb participants, welcome!
-We have a milestone [here](https://github.com/physiopy/phys2bids/milestone/5) as a collection of issues you could work on with our help. 
+We have a milestone [here](https://github.com/physiopy/phys2bids/milestone/5) as a collection of issues you could work on with our help.
 Check the issues with a `BrainWeb` label. Of course, they are only suggestions, so feel free to tackle any issue you want, even open new ones!
 You can also contact us on Gitter, in the BrainHack Mattermost (<a href="https://mattermost.brainhack.org/brainhack/channels/physiopy">#physiopy</a>), and don't hesitate to contact [Stefano](https://github.com/smoia) in other ways to jump in the development!
 -->
 
 **We're looking for code contributors,** but any suggestion/bug report is welcome! Feel free to open issues!
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

### Comparing `phys2bids-2.8.3/PKG-INFO` & `phys2bids-2.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phys2bids
-Version: 2.8.3
+Version: 2.8.4
 Summary: Python library to convert physiological data files into BIDS format
 Home-page: https://github.com/physiopy/phys2bids
 Author: phys2bids developers
 Maintainer: Stefano Moia
 Maintainer-email: s.moia@bcbl.eu
 License: Apache-2.0
 Download-URL: https://github.com/physiopy/phys2bids
@@ -60,26 +60,26 @@
         - [Developer calls calendar](https://calendar.google.com/calendar/u/0?cid=amoycDQ1MTdhMWdpaHNuNzlnOW1ucHJkMjRAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ)
         
         ## Tested OSs
         While all version until `2.6.2` were tested on Linux and Windows, starting from version `2.7` onward we had to **drop Windows testing**. The reason is related to the cost of running such tests: for each Windows test, we can run up to 8 tests on Linux instead. Partial Windows testing might be reintroduced in future releases.
         
         Hence, while **we cannot ensure that phys2bids will run on Windows**, however we don't see any reason it shouldn't. Besides, it will run on Linux Subsistems.
         
-        We apologise for the discomfort. 
+        We apologise for the discomfort.
         
         
         <!-- ## Hacktoberfest
         Hacktoberfest participants, welcome!
         We have some issues for you [here](https://github.com/physiopy/phys2bids/issues?q=is%3Aissue+is%3Aopen+label%3Ahacktoberfest)!
         However, feel free to tackle any issue you'd like. Depending on the issue and extent of contribution, Hacktoberfest related PRs might not count toward being listed as contributors and authors (unless there is the specific interest). You can ask about it in the issue itself!
         Feel free to ask help to the contributors over gitter, happy coding and (hopefully) enjoy hour tee (or tree)!
         
         ## The BrainWeb
         BrainWeb participants, welcome!
-        We have a milestone [here](https://github.com/physiopy/phys2bids/milestone/5) as a collection of issues you could work on with our help. 
+        We have a milestone [here](https://github.com/physiopy/phys2bids/milestone/5) as a collection of issues you could work on with our help.
         Check the issues with a `BrainWeb` label. Of course, they are only suggestions, so feel free to tackle any issue you want, even open new ones!
         You can also contact us on Gitter, in the BrainHack Mattermost (<a href="https://mattermost.brainhack.org/brainhack/channels/physiopy">#physiopy</a>), and don't hesitate to contact [Stefano](https://github.com/smoia) in other ways to jump in the development!
         -->
         
         **We're looking for code contributors,** but any suggestion/bug report is welcome! Feel free to open issues!
         
         This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
@@ -157,15 +157,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides: phys2bids
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: mat
 Provides-Extra: doc
-Provides-Extra: duecredit
 Provides-Extra: interfaces
-Provides-Extra: all
 Provides-Extra: acq
 Provides-Extra: test
+Provides-Extra: duecredit
 Provides-Extra: style
+Provides-Extra: mat
+Provides-Extra: all
```

### Comparing `phys2bids-2.8.3/setup.cfg` & `phys2bids-2.8.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 platforms = OS Independent
 provides = 
 	phys2bids
 
 [options]
 python_requires = >=3.6.1
 install_requires = 
-	numpy >=1.10, <1.24, !=*rc*
+	numpy >=1.10, <1.24
 	matplotlib >=3.1.1, !=3.3.0rc1
-	PyYAML >=5.1, !=*rc*
+	PyYAML >=5.1
 tests_require = 
 	pytest >=5.3
 test_suite = pytest
 zip_safe = False
 packages = find:
 include_package_data = True
 
@@ -45,14 +45,15 @@
 doc = 
 	sphinx >=2.0
 	sphinx-argparse
 	sphinx_rtd_theme
 style = 
 	flake8 >=3.7
 	flake8-docstrings >=1.5
+	codespell
 interfaces = 
 	%(acq)s
 	%(mat)s
 test = 
 	pytest >=5.3
 	pytest-cov
 	coverage
@@ -76,19 +77,35 @@
 	phys2bids=phys2bids.phys2bids:_main
 
 [flake8]
 exclude = 
 	*build/
 	heuristics
 	tests
-ignore = E126, E402, W503
+	_version.py
+	./phys2bids/cli/__init__.py
+	./phys2bids/tests/*
+	versioneer.py
+ignore = E126, E402, W503, E226
 max-line-length = 99
 per-file-ignores = 
 	*/__init__.py:F401
 
+[pydocstyle]
+convention = numpy
+match = 
+	nigsp/*.py
+match_dir = nigsp/[^tests,^heuristics]*
+
+[codespell]
+skip = venvs,.venv,versioneer.py,.git,build,./docs/_build
+write-changes = 
+count = 
+quiet-level = 3
+
 [tool:pytest]
 doctest_optionflags = NORMALIZE_WHITESPACE
 xfail_strict = true
 addopts = -rx
 
 [versioneer]
 vcs = git
```

### Comparing `phys2bids-2.8.3/phys2bids/viz.py` & `phys2bids-2.8.4/phys2bids/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
                  filename, figsize=FIGSIZE, dpi=SET_DPI):
     """
     Produce a figure with three plots.
 
     1. Plots the triggers in blue, a block in orange that indicates
     the time from the first trigger to the last, and a red line showing
     the threshold used for trigger detection
-    2. Same plot but showing only the intial trigger
-    3. Same plot but showing only the intial trigger
+    2. Same plot but showing only the initial trigger
+    3. Same plot but showing only the initial trigger
 
     Parameters
     ----------
     time: numpy ndarray
         time channel
     trigger: numpy ndarray
         trigger channel
```

### Comparing `phys2bids-2.8.3/phys2bids/utils.py` & `phys2bids-2.8.4/phys2bids/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             break
 
     if fftype_found:
         LGR.info(f'File extension is .{ftype}')
         LGR.warning('If both acq and txt files exist in the path, acq will be selected.')
         return fname, ftype
     else:
-        raise Exception(f'The file {filename} wasn\'t found in {indir}'
+        raise Exception(f'The file {filename} was not found in {indir}'
                         f' or {ftype} is not supported yet.\n'
                         f'phys2bids currently supports:'
                         f' {", ".join(SUPPORTED_FTYPES)}')
 
 
 def check_file_exists(filename):
     """
```

### Comparing `phys2bids-2.8.3/phys2bids/physio_obj.py` & `phys2bids-2.8.4/phys2bids/physio_obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
             raise IndexError(f'Slice ({idx.start}, {idx.stop}) is out of '
                              f'bounds for channel {self.trigger_idx} '
                              f'with size {trigger_length}')
 
         # Operate on each channel on its own
         for n, channel in enumerate(self.timeseries):
             idx_dict = {'start': idx.start, 'stop': idx.stop, 'step': idx.step}
-            # Adapt the slicing indexes to the right requency
+            # Adapt the slicing indexes to the right frequency
             for i in ['start', 'stop', 'step']:
                 if idx_dict[i]:
                     idx_dict[i] = int(np.floor(self.freq[n]
                                                / self.freq[self.trigger_idx]
                                                * idx_dict[i]))
 
             # Correct the slicing stop if necessary
```

### Comparing `phys2bids-2.8.3/phys2bids/phys2bids.py` & `phys2bids-2.8.4/phys2bids/phys2bids.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 LGR = logging.getLogger(__name__)
 LGR.setLevel(logging.INFO)
 
 
 def print_summary(filename, ntp_expected, ntp_found, samp_freq, time_offset, outfile):
     """
-    Print a summary onscreen and in file with informations on the files.
+    Print a summary onscreen and in file with information on the files.
 
     Parameters
     ----------
     filename: str
         Name of the input of phys2bids.
     ntp_expected: int
         Number of expected timepoints, as defined by user.
@@ -297,15 +297,16 @@
             # returns a dictionary in the form {take_idx: phys_in[startpoint, endpoint]}
 
             # save a figure for each take | give the right acquisition parameters for takes
             fileprefix = os.path.join(conversion_path,
                                       os.path.splitext(os.path.basename(filename))[0])
             for i, take in enumerate(phys_in.keys()):
                 plot_fileprefix = f'{fileprefix}_{take:02d}'
-                viz.export_trigger_plot(phys_in[take], phys_in[take].trigger_idx, plot_fileprefix, tr[i],
+                viz.export_trigger_plot(phys_in[take], phys_in[take].trigger_idx,
+                                        plot_fileprefix, tr[i],
                                         num_timepoints_expected[i], filename,
                                         sub, ses)
 
         # Single take acquisition type, or : nothing to split workflow
         else:
             # Run analysis on trigger channel to get first timepoint
             # and the time offset.
@@ -377,15 +378,15 @@
             # take the frequency
             for idx, i in enumerate(phys_in[take].freq):
                 # if that frequency is different than the frequency of the phys_obj entry
                 if i != uniq_freq:
                     # eliminate that channel from the dict since we only want channels
                     # with the same frequency
                     phys_out[key].delete_at_index(idx - count)
-                    # take into acount the elimination so in the next eliminated channel we
+                    # take into account the elimination so in the next eliminated channel we
                     # eliminate correctly
                     count += 1
             # Also create a BlueprintOutput object for each unique frequency found.
             # Populate it with the corresponding blueprint input and replace it
             # in the dictionary.
             # Add time channel in the proper frequency.
             if uniq_freq != phys_in[take].freq[0]:
@@ -394,17 +395,22 @@
                 phys_out[key].timeseries.insert(0, np.linspace(phys_in[take].timeseries[0][0],
                                                 phys_in[take].timeseries[0][-1],
                                                 num=phys_out[key].timeseries[0].shape[0]))
             # Add trigger channel in the proper frequency.
             if uniq_freq != phys_in[take].freq[phys_in[take].trigger_idx]:
                 phys_out[key].ch_name.insert(1, phys_in[take].ch_name[phys_in[take].trigger_idx])
                 phys_out[key].units.insert(1, phys_in[take].units[phys_in[take].trigger_idx])
-                phys_out[key].timeseries.insert(1, np.interp(phys_out[key].timeseries[0],
-                                                             phys_in[take].timeseries[0],
-                                                             phys_in[take].timeseries[phys_in[take].trigger_idx]))
+                phys_out[key].timeseries.insert(
+                    1,
+                    np.interp(
+                        phys_out[key].timeseries[0],
+                        phys_in[take].timeseries[0],
+                        phys_in[take].timeseries[phys_in[take].trigger_idx]
+                    )
+                )
             phys_out[key] = BlueprintOutput.init_from_blueprint(phys_out[key])
 
         # Preparing output parameters: name and folder.
         for uniq_freq in uniq_freq_list:
             key = f'{take}_{uniq_freq}'
             # If possible, prepare bids renaming.
             if heur_file is not None and sub is not None:
```

### Comparing `phys2bids-2.8.3/phys2bids/cli/run.py` & `phys2bids-2.8.4/phys2bids/cli/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                                'Default is to process all channels.',
                           default=None)
     optional.add_argument('-ntp', '--numtps',
                           dest='num_timepoints_expected',
                           nargs='*',
                           type=int,
                           help='Number of expected trigger timepoints (TRs). '
-                               'Default is None. Note: the estimation of beggining of '
+                               'Default is None. Note: the estimation of beginning of '
                                'neuroimaging acquisition cannot take place with this default. '
                                'If you\'re running phys2bids on a multi-run recording, '
                                'give a list of each expected ntp for each run.',
                           default=None)
     optional.add_argument('-tr', '--tr',
                           dest='tr',
                           nargs='*',
```

### Comparing `phys2bids-2.8.3/phys2bids/io.py` & `phys2bids-2.8.4/phys2bids/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Check if there are channels with different frequency than the maximum one.
 
     Parameters
     ----------
     timeseries : list of numpy.ndarrays
         list of numpy.ndarrays representing channels.
     freq : list of floats
-        list with the maximun frequency
+        list with the maximum frequency
     start : int, optional
         first sample of the channel to be considered
     endat : int or None, optional
         last sasmple to consider (None for last)
         Just in case the process takes too long
 
     Returns
@@ -63,15 +63,15 @@
     return multifreq_timeseries, multifreq_freq
 
 
 def generate_blueprint(timeseries, chtrig, interval, orig_units, orig_names):
     """
     Generate blueprint object from various information.
 
-    Standarize timeseries, chtrig interval orig_units and orig_names in the correct units and
+    Standardize timeseries, chtrig interval orig_units and orig_names in the correct units and
     format and generate a physio_obj.BlueprintInput object.
     This function is mainly thought to adapt txt files.
 
     Parameters
     ----------
     timeseries : list of numpy.ndarrays
         a list of numpy.ndarrays representing the channels
@@ -107,15 +107,15 @@
         raise AttributeError(f'Interval unit "{interval[-1]}" is not in a '
                              'valid frequency or time unit format, this probably '
                              'means your file is not in min, sec, msec, µsec, hr, min, s, ms, µs, '
                              'Mhz, KHz or Hz')
     # Check if the header is in frequency or sampling interval
     if 'Hz' in interval[-1]:
         LGR.info('Retrieving frequency from file header, calculating sample interval, '
-                 'and standarizing to Hz if needed')
+                 'and standardizing to Hz if needed')
         freq = float(interval[0])
         freq_unit = interval[-1]
         if freq_unit == 'MHz':
             freq = freq * (1000000)
         elif freq_unit == 'kHz':
             freq = freq * 1000
         interval[0] = 1 / freq
@@ -142,15 +142,15 @@
         else:
             interval[0] = float(interval[0])
         # get frequency
         freq = [1 / interval[0]] * len(timeseries)
     # reorder channels names
     names = ['time', ]
     names = names + orig_names
-    # reoder channels units
+    # reorder channels units
     units = ['s', ]
     units = units + orig_units
     # Check if the file has a time channel, otherwise create it.
     # As the "time" doesn't have a column header, if the number of header names
     # is less than the number of timeseries, then "time" is column 0...
     # ...otherwise, create the time channel
     if not (len(orig_names) < len(timeseries)):
@@ -225,15 +225,15 @@
     ----------
     header : list
         list that contains file header
 
     Returns
     -------
     interval : list of strings
-        maximun sampling frequency or interval value and unit for the recording
+        maximum sampling frequency or interval value and unit for the recording
     orig_units : list of strings
         contains original channels units
     orig_names : list of strings
         contains original channels name
 
     Raises
     ------
@@ -274,15 +274,15 @@
         orig_units = []
         orig_names = []
         # the for loop starts at index1 at 3 because that's the first line of the header
         # with channel name info and ends in 2 + twice the number of channels because
         # that should be the last channel name
         for index1 in range(3, 3 + len(header[-1]) * 2, 2):
             orig_names.append(header[index1][0])
-            # since units are in the line imediately after we get the units at the same time
+            # since units are in the line immediately after we get the units at the same time
             orig_units.append(header[index1 + 1][0])
     else:
         raise NotImplementedError(OPEN_ISSUE)
     return interval, orig_units, orig_names
 
 
 def load_txt(filename, chtrig=0):
@@ -424,14 +424,17 @@
 def load_gep(filename):
     """
     Populate object phys_input from GE physiological files.
 
     Uses the filename that the user provides to find any matching inputs
     from other recording types (PPG, RESP, or ECG).
 
+    **Note that the filename must not be altered from how it is output from
+    the scanner.**
+
     Populates physio_obj with all identified recording types (note that one
     or more of these may not be true recordings as the scanner outputs all
     possible types in all cases). The modality corresponding to the filename
     entered by the user is put first (after time and trigger).
 
     Parameters
     ----------
@@ -453,15 +456,15 @@
     --------
     physio_obj.BlueprintInput
     """
     import os
     from glob import glob
     from pathlib import Path
 
-    # Inititate lists of column names and units with time and trigger
+    # Initiate lists of column names and units with time and trigger
     names = ['time', 'trigger']
     units = ['s', 'mV']  # Assuming recording units are mV...
 
     # Add column for file given by user
     if 'PPGData' in filename:
         freq = [100, 100, 100]
         names.append('cardiac')
```

### Comparing `phys2bids-2.8.3/phys2bids/heuristics/heur_test_multifreq.py` & `phys2bids-2.8.4/phys2bids/heuristics/heur_test_multifreq.py`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/phys2bids/heuristics/heur_test_acq.py` & `phys2bids-2.8.4/phys2bids/heuristics/heur_test_acq.py`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/phys2bids/heuristics/heur_tutorial.py` & `phys2bids-2.8.4/phys2bids/heuristics/heur_tutorial.py`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/phys2bids/heuristics/heur_euskalibur.py` & `phys2bids-2.8.4/phys2bids/heuristics/heur_euskalibur.py`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/phys2bids/tests/test_utils.py` & `phys2bids-2.8.4/phys2bids/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 # Tests check_input_type
 def test_check_input_type(testpath, samefreq_full_acq_file):
     assert utils.check_input_type(samefreq_full_acq_file, testpath)
 
     with raises(Exception) as errorinfo:
         utils.check_input_type('nobel_prize.win', testpath)
-    assert "wasn't found" in str(errorinfo.value)
+    assert "was not found" in str(errorinfo.value)
 
 
 # Tests check_file_exists
 def test_check_file_exists(samefreq_full_acq_file):
     utils.check_file_exists(samefreq_full_acq_file)
 
     with raises(Exception) as errorinfo:
```

### Comparing `phys2bids-2.8.3/phys2bids/tests/test_physio_obj.py` & `phys2bids-2.8.4/phys2bids/tests/test_physio_obj.py`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/phys2bids/tests/test_viz.py` & `phys2bids-2.8.4/phys2bids/tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/phys2bids/tests/test_integration.py` & `phys2bids-2.8.4/phys2bids/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         logger_info = logger_info.readlines()
 
     # Get version info
     current_version = get_versions()
     assert check_string(logger_info, 'phys2bids version', current_version['version'], is_num=False)
 
     assert check_string(logger_info, '01. Trigger; sampled at', '1000.0')
-    # Should be 500.0 for sampling, but new faster multifreq version does not detect it. 
+    # Should be 500.0 for sampling, but new faster multifreq version does not detect it.
     assert check_string(logger_info, '04. Belt; sampled at', '1000.0')
 
     # Check that files are generated in conversion path
     # There should be a 500 too, but labchart export doesn't work well.
     for freq in ['40', '100', '1000']:
         assert isfile(join(conversion_path,
                            'sub-006_ses-01_task-test_rec-biopac_run-01_'
```

### Comparing `phys2bids-2.8.3/phys2bids/tests/test_bids.py` & `phys2bids-2.8.4/phys2bids/tests/test_bids.py`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/phys2bids/tests/conftest.py` & `phys2bids-2.8.4/phys2bids/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     Returns
     -------
     full_path : str
         Full path to downloaded `filename`
     """
     # This restores the same behavior as before.
-    # this three lines make tests dowloads work in windows
+    # this three lines make tests downloads work in windows
     if os.name == 'nt':
         orig_sslsocket_init = ssl.SSLSocket.__init__
         ssl.SSLSocket.__init__ = lambda *args, cert_reqs=ssl.CERT_NONE, **kwargs: orig_sslsocket_init(*args, cert_reqs=ssl.CERT_NONE, **kwargs)
         ssl._create_default_https_context = ssl._create_unverified_context
     url = 'https://osf.io/{}/download'.format(osf_id)
     full_path = os.path.join(path, filename)
     if not os.path.isfile(full_path):
```

### Comparing `phys2bids-2.8.3/phys2bids/tests/test_io.py` & `phys2bids-2.8.4/phys2bids/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 @pytest.fixture(scope='function')
 def loaded_acq_file(samefreq_short_txt_file):
     chtrig = 2
     header_acq, channels_acq = io.read_header_and_channels(samefreq_short_txt_file)
 
     # just a few quick checks to make sure the data loaded correctly
-    assert len(header_acq) == 9  # check proper header lenght
+    assert len(header_acq) == 9  # check proper header length
     assert len(channels_acq[0]) == 1048559  # check proper number of timepoints
     assert len(header_acq[-1]) == 2  # check extra line is deleted
     assert 'acq' in header_acq[0][0]
 
     return header_acq, channels_acq, chtrig
 
 
@@ -138,15 +138,15 @@
     # checks that the trigger is in the right channel
     assert phys_obj.ch_name[chtrig] == 'MR TRIGGER - Custom, HLT100C - A 5'
     assert phys_obj.freq[chtrig] == 10000.0
     assert phys_obj.units[chtrig] == 'Volts'
 
 
 def test_load_mat(matlab_file_labchart, matlab_file_acq):
-    # Read data to test labchart in mat exension
+    # Read data to test labchart in mat extension
     chtrig = 1
     phys_obj = io.load_mat(matlab_file_labchart, chtrig)
 
     # Check channel names are the same.
     orig_channels = ['time', 'Trigger', 'CO2', 'O2', 'Belt', 'Pulse']
     assert phys_obj.ch_name == orig_channels
 
@@ -154,15 +154,15 @@
     orig_freq = [1000.0, 1000.0, 100.0, 40.0, 400.0, 1000.0]
     assert phys_obj.freq == orig_freq
 
     # Check units are the same
     orig_units = ['s', 'V', 'mmHg', 'mmHg', 'V', 'V']
     assert phys_obj.units == orig_units
 
-    # Read data to test acq in mat exension
+    # Read data to test acq in mat extension
     chtrig = 3
     phys_obj = io.load_mat(matlab_file_acq, chtrig)
 
     # checks that the outputs make sense
     assert phys_obj.ch_name[0] == 'time'
     assert phys_obj.freq[0] == 10000.0
     assert phys_obj.units[0] == 's'
@@ -203,8 +203,8 @@
     phys_obj = io.load_gep(ge_two_gep_files_resp)
 
     # Check the channel data is as expected
     gep_data1 = np.loadtxt(ge_two_gep_files_resp)
     gep_data2 = np.loadtxt(os.path.join(testpath,
                                         'PPGData_epiRT_0000000000_00_00_000.gep'))
     assert np.array_equal(gep_data1, phys_obj.timeseries[2])
-    assert np.array_equal(gep_data2, phys_obj.timeseries[3])
+    assert np.array_equal(gep_data2, phys_obj.timeseries[3])
```

### Comparing `phys2bids-2.8.3/phys2bids/tests/test_phys2bids.py` & `phys2bids-2.8.4/phys2bids/tests/test_phys2bids.py`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/phys2bids/tests/data/README.md` & `phys2bids-2.8.4/phys2bids/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/phys2bids/bids.py` & `phys2bids-2.8.4/phys2bids/bids.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,18 @@
                 'pascal': 'Pa', 'pascals': 'Pa', 'pa': 'Pa',
                 # volt: voltage (electrical potential), emf
                 'volt': 'V', 'volts': 'V',
                 # degree Celsius: temperature relative to 273.15 K
                 '°c': '°C', '°celsius': '°C', 'celsius': '°C',
                 # ampere: electric current
                 'ampere': 'A', 'amp': 'A', 'amps': 'A',
-                # second: time and hertzs: frequency
+                # second: time and hertz: frequency
                 # siemens: electric conductance (e.g. EDA)
                 'siemens': 'S',
-                # second: time and hertzs
+                # second: time and hertz
                 '1/hz': 's', '1/hertz': 's', 'hz': 'Hz',
                 '1/s': 'Hz', '1/second': 'Hz', '1/seconds': 'Hz',
                 '1/sec': 'Hz', '1/secs': 'Hz', 'hertz': 'Hz',
                 'second': 's', 'seconds': 's', 'sec': 's',
                 'secs': 's',
                 # All the aliases with one letter (to avoid issues)
                 'k': 'K', 'n': 'N', 'v': 'V', 'c': '°C', 'a': 'A', 's': 's',
@@ -239,15 +239,15 @@
             tsvreader = reader(pf, delimiter="\t")
             for line in tsvreader:
                 if sub in line[p_id_idx]:
                     sub_exists = True
                     break
         # Only append to file if subject is not in the file
         if not sub_exists:
-            LGR.info(f'Appending subjet sub-{sub} to participants.tsv ...')
+            LGR.info(f'Appending subject sub-{sub} to participants.tsv ...')
             participants_data = ['n/a'] * header_length
             participants_data[p_id_idx] = f'sub-{sub}'
             utils.append_list_as_row(file_path, participants_data)
 
 
 def dataset_description_file(outdir):
     """
```

### Comparing `phys2bids-2.8.3/phys2bids/due.py` & `phys2bids-2.8.4/phys2bids/due.py`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/phys2bids/slice4phys.py` & `phys2bids-2.8.4/phys2bids/slice4phys.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         Default: 9
 
     Returns
     --------
     take_timestamps: dictionary
         Containing tuples of take start and end indexes for each take, based on
         trigger channels. It also contains take attributes: time offset from
-        session beggining, and nb of triggers in the form of
+        session beginning, and nb of triggers in the form of
         take_timestamps{1:(start, end, time offset, nb of triggers),
                        2:(...), ... }
     """
     # Initialize dictionaries to save  take timestamps and phys_in attributes
     take_timestamps = {}
 
     # Express the padding in samples equivalent
```

### Comparing `phys2bids-2.8.3/phys2bids.egg-info/PKG-INFO` & `phys2bids-2.8.4/phys2bids.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phys2bids
-Version: 2.8.3
+Version: 2.8.4
 Summary: Python library to convert physiological data files into BIDS format
 Home-page: https://github.com/physiopy/phys2bids
 Author: phys2bids developers
 Maintainer: Stefano Moia
 Maintainer-email: s.moia@bcbl.eu
 License: Apache-2.0
 Download-URL: https://github.com/physiopy/phys2bids
@@ -60,26 +60,26 @@
         - [Developer calls calendar](https://calendar.google.com/calendar/u/0?cid=amoycDQ1MTdhMWdpaHNuNzlnOW1ucHJkMjRAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ)
         
         ## Tested OSs
         While all version until `2.6.2` were tested on Linux and Windows, starting from version `2.7` onward we had to **drop Windows testing**. The reason is related to the cost of running such tests: for each Windows test, we can run up to 8 tests on Linux instead. Partial Windows testing might be reintroduced in future releases.
         
         Hence, while **we cannot ensure that phys2bids will run on Windows**, however we don't see any reason it shouldn't. Besides, it will run on Linux Subsistems.
         
-        We apologise for the discomfort. 
+        We apologise for the discomfort.
         
         
         <!-- ## Hacktoberfest
         Hacktoberfest participants, welcome!
         We have some issues for you [here](https://github.com/physiopy/phys2bids/issues?q=is%3Aissue+is%3Aopen+label%3Ahacktoberfest)!
         However, feel free to tackle any issue you'd like. Depending on the issue and extent of contribution, Hacktoberfest related PRs might not count toward being listed as contributors and authors (unless there is the specific interest). You can ask about it in the issue itself!
         Feel free to ask help to the contributors over gitter, happy coding and (hopefully) enjoy hour tee (or tree)!
         
         ## The BrainWeb
         BrainWeb participants, welcome!
-        We have a milestone [here](https://github.com/physiopy/phys2bids/milestone/5) as a collection of issues you could work on with our help. 
+        We have a milestone [here](https://github.com/physiopy/phys2bids/milestone/5) as a collection of issues you could work on with our help.
         Check the issues with a `BrainWeb` label. Of course, they are only suggestions, so feel free to tackle any issue you want, even open new ones!
         You can also contact us on Gitter, in the BrainHack Mattermost (<a href="https://mattermost.brainhack.org/brainhack/channels/physiopy">#physiopy</a>), and don't hesitate to contact [Stefano](https://github.com/smoia) in other ways to jump in the development!
         -->
         
         **We're looking for code contributors,** but any suggestion/bug report is welcome! Feel free to open issues!
         
         This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
@@ -157,15 +157,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides: phys2bids
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: mat
 Provides-Extra: doc
-Provides-Extra: duecredit
 Provides-Extra: interfaces
-Provides-Extra: all
 Provides-Extra: acq
 Provides-Extra: test
+Provides-Extra: duecredit
 Provides-Extra: style
+Provides-Extra: mat
+Provides-Extra: all
```

### Comparing `phys2bids-2.8.3/phys2bids.egg-info/requires.txt` & `phys2bids-2.8.4/phys2bids.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-numpy!=*rc*,<1.24,>=1.10
+numpy<1.24,>=1.10
 matplotlib!=3.3.0rc1,>=3.1.1
-PyYAML!=*rc*,>=5.1
+PyYAML>=5.1
 
 [acq]
 bioread>=1.0.5
 
 [all]
 sphinx>=2.0
 sphinx-argparse
 sphinx_rtd_theme
 duecredit
 bioread>=1.0.5
 pymatreader>=0.0.24
 flake8>=3.7
 flake8-docstrings>=1.5
+codespell
 pytest>=5.3
 pytest-cov
 coverage
 bioread>=1.0.5
 pymatreader>=0.0.24
 flake8>=3.7
 flake8-docstrings>=1.5
+codespell
 
 [doc]
 sphinx>=2.0
 sphinx-argparse
 sphinx_rtd_theme
 
 [duecredit]
@@ -36,16 +38,18 @@
 
 [mat]
 pymatreader>=0.0.24
 
 [style]
 flake8>=3.7
 flake8-docstrings>=1.5
+codespell
 
 [test]
 pytest>=5.3
 pytest-cov
 coverage
 bioread>=1.0.5
 pymatreader>=0.0.24
 flake8>=3.7
 flake8-docstrings>=1.5
+codespell
```

### Comparing `phys2bids-2.8.3/phys2bids.egg-info/SOURCES.txt` & `phys2bids-2.8.4/phys2bids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/versioneer.py` & `phys2bids-2.8.4/versioneer.py`

 * *Files identical despite different names*

### Comparing `phys2bids-2.8.3/LICENSE` & `phys2bids-2.8.4/LICENSE`

 * *Files identical despite different names*


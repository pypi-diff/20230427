# Comparing `tmp/optilibre-1.1.2.tar.gz` & `tmp/optilibre-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optilibre-1.1.2.tar", last modified: Tue Nov 16 17:40:12 2021, max compression
+gzip compressed data, was "optilibre-1.2.0.tar", last modified: Thu Apr 27 07:42:14 2023, max compression
```

## Comparing `optilibre-1.1.2.tar` & `optilibre-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,37 @@
-drwxrwx---   0 sydney    (1000) sydney    (1000)        0 2021-11-16 17:40:12.392889 optilibre-1.1.2/
--rw-rw----   0 sydney    (1000) sydney    (1000)    34454 2021-11-06 19:25:40.000000 optilibre-1.1.2/LICENSE
--rw-rw----   0 sydney    (1000) sydney    (1000)     2237 2021-11-16 17:40:12.392889 optilibre-1.1.2/PKG-INFO
--rw-r--r--   0 sydney    (1000) sydney    (1000)     1655 2021-11-16 17:14:54.000000 optilibre-1.1.2/README.md
--rw-rw----   0 sydney    (1000) sydney    (1000)      103 2021-11-16 16:02:51.000000 optilibre-1.1.2/pyproject.toml
--rw-rw----   0 sydney    (1000) sydney    (1000)      670 2021-11-16 17:40:12.392889 optilibre-1.1.2/setup.cfg
-drwxrwx---   0 sydney    (1000) sydney    (1000)        0 2021-11-16 17:40:12.392889 optilibre-1.1.2/src/
-drwxrwx---   0 sydney    (1000) sydney    (1000)        0 2021-11-16 17:40:12.392889 optilibre-1.1.2/src/optilibre/
--rw-rw----   0 sydney    (1000) sydney    (1000)      253 2021-11-16 17:02:58.000000 optilibre-1.1.2/src/optilibre/__init__.py
--rw-rw----   0 sydney    (1000) sydney    (1000)       70 2021-11-16 16:31:04.000000 optilibre-1.1.2/src/optilibre/__main__.py
--rw-rw----   0 sydney    (1000) sydney    (1000)     2133 2021-11-16 17:39:28.000000 optilibre-1.1.2/src/optilibre/cli.py
--rw-rw----   0 sydney    (1000) sydney    (1000)      313 2021-11-09 06:50:08.000000 optilibre-1.1.2/src/optilibre/enums.py
--rw-rw----   0 sydney    (1000) sydney    (1000)     2401 2021-11-06 08:26:22.000000 optilibre-1.1.2/src/optilibre/helpers.py
--rw-rw----   0 sydney    (1000) sydney    (1000)     7805 2021-11-16 17:38:53.000000 optilibre-1.1.2/src/optilibre/runner.py
-drwxrwx---   0 sydney    (1000) sydney    (1000)        0 2021-11-16 17:40:12.392889 optilibre-1.1.2/src/optilibre.egg-info/
--rw-rw----   0 sydney    (1000) sydney    (1000)     2237 2021-11-16 17:40:12.000000 optilibre-1.1.2/src/optilibre.egg-info/PKG-INFO
--rw-rw----   0 sydney    (1000) sydney    (1000)      335 2021-11-16 17:40:12.000000 optilibre-1.1.2/src/optilibre.egg-info/SOURCES.txt
--rw-rw----   0 sydney    (1000) sydney    (1000)        1 2021-11-16 17:40:12.000000 optilibre-1.1.2/src/optilibre.egg-info/dependency_links.txt
--rw-rw----   0 sydney    (1000) sydney    (1000)       10 2021-11-16 17:40:12.000000 optilibre-1.1.2/src/optilibre.egg-info/top_level.txt
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.911842 optilibre-1.2.0/
+-rw-r--r--   0 sydney     (501) staff       (20)      126 2023-04-26 14:48:40.000000 optilibre-1.2.0/.gitignore
+-rw-r--r--   0 sydney     (501) staff       (20)      159 2023-04-26 15:01:42.000000 optilibre-1.2.0/CHANGELOG.md
+-rw-r--r--   0 sydney     (501) staff       (20)    34454 2022-05-22 13:42:28.000000 optilibre-1.2.0/LICENSE
+-rw-r--r--   0 sydney     (501) staff       (20)      190 2023-04-26 14:46:30.000000 optilibre-1.2.0/Makefile
+-rw-r--r--   0 sydney     (501) staff       (20)     2200 2023-04-27 07:42:14.911950 optilibre-1.2.0/PKG-INFO
+-rw-r--r--   0 sydney     (501) staff       (20)     1655 2022-05-22 13:42:28.000000 optilibre-1.2.0/README.md
+-rw-r--r--   0 sydney     (501) staff       (20)      409 2022-05-30 08:28:22.000000 optilibre-1.2.0/optilibre.example.conf
+-rw-r--r--   0 sydney     (501) staff       (20)      908 2022-05-31 08:48:39.000000 optilibre-1.2.0/optilibre.example.toml
+-rw-r--r--   0 sydney     (501) staff       (20)      469 2023-04-26 15:06:54.000000 optilibre-1.2.0/pyproject.toml
+-rw-r--r--   0 sydney     (501) staff       (20)       31 2022-05-22 13:42:28.000000 optilibre-1.2.0/requirements.txt
+-rw-r--r--   0 sydney     (501) staff       (20)      654 2023-04-27 07:42:14.912266 optilibre-1.2.0/setup.cfg
+-rwxr-xr-x   0 sydney     (501) staff       (20)      497 2022-05-22 13:42:28.000000 optilibre-1.2.0/setup.sh
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.905139 optilibre-1.2.0/src/
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.910207 optilibre-1.2.0/src/optilibre/
+-rw-r--r--   0 sydney     (501) staff       (20)      489 2023-04-26 14:39:18.000000 optilibre-1.2.0/src/optilibre/__init__.py
+-rw-r--r--   0 sydney     (501) staff       (20)      200 2023-04-26 14:39:18.000000 optilibre-1.2.0/src/optilibre/__main__.py
+-rw-r--r--   0 sydney     (501) staff       (20)      160 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre/_version.py
+-rw-r--r--   0 sydney     (501) staff       (20)     2134 2022-05-22 14:24:54.000000 optilibre-1.2.0/src/optilibre/cli.py
+-rw-r--r--   0 sydney     (501) staff       (20)     4141 2023-04-26 08:18:28.000000 optilibre-1.2.0/src/optilibre/core.py
+-rw-r--r--   0 sydney     (501) staff       (20)      838 2023-04-25 12:43:08.000000 optilibre-1.2.0/src/optilibre/enums.py
+-rw-r--r--   0 sydney     (501) staff       (20)     5230 2023-04-26 08:19:48.000000 optilibre-1.2.0/src/optilibre/helpers.py
+-rw-r--r--   0 sydney     (501) staff       (20)     3178 2023-04-26 06:54:49.000000 optilibre-1.2.0/src/optilibre/models.py
+-rw-r--r--   0 sydney     (501) staff       (20)     7794 2023-04-26 13:25:59.000000 optilibre-1.2.0/src/optilibre/runner.py
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.911243 optilibre-1.2.0/src/optilibre/utils/
+-rw-r--r--   0 sydney     (501) staff       (20)        0 2022-05-27 11:05:59.000000 optilibre-1.2.0/src/optilibre/utils/__init__.py
+-rw-r--r--   0 sydney     (501) staff       (20)     2122 2022-07-20 14:11:59.000000 optilibre-1.2.0/src/optilibre/utils/parsers.py
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.911032 optilibre-1.2.0/src/optilibre.egg-info/
+-rw-r--r--   0 sydney     (501) staff       (20)     2200 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/PKG-INFO
+-rw-r--r--   0 sydney     (501) staff       (20)      703 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/SOURCES.txt
+-rw-r--r--   0 sydney     (501) staff       (20)        1 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/dependency_links.txt
+-rw-r--r--   0 sydney     (501) staff       (20)       54 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/entry_points.txt
+-rw-r--r--   0 sydney     (501) staff       (20)       32 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/requires.txt
+-rw-r--r--   0 sydney     (501) staff       (20)       10 2023-04-27 07:42:14.000000 optilibre-1.2.0/src/optilibre.egg-info/top_level.txt
+drwxr-xr-x   0 sydney     (501) staff       (20)        0 2023-04-27 07:42:14.911704 optilibre-1.2.0/systemd/
+-rw-r--r--   0 sydney     (501) staff       (20)      364 2022-05-22 13:42:28.000000 optilibre-1.2.0/systemd/opti_libre.service
+-rw-r--r--   0 sydney     (501) staff       (20)       90 2022-05-22 13:42:28.000000 optilibre-1.2.0/systemd/opti_libre.timer
```

### Comparing `optilibre-1.1.2/LICENSE` & `optilibre-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optilibre-1.1.2/PKG-INFO` & `optilibre-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: optilibre
-Version: 1.1.2
+Version: 1.2.0
 Summary: Video and Image optimizer
 Home-page: https://gitlab.com/daufinsyd/optilibre
 Author: Sydney Gems
 Author-email: sydney@gems.technology
-License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/daufinsyd/optilibre/-/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -65,9 +63,7 @@
  - any -> h265 (requires ffmpeg with libx265 encoder)
 
 ### Images
 
  - jpeg -> jpeg (requires jpegoptim)
  - any jpeg -> jpeg-xl (requires cjxl)
 
-
-
```

### Comparing `optilibre-1.1.2/README.md` & `optilibre-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `optilibre-1.1.2/setup.cfg` & `optilibre-1.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [metadata]
 name = optilibre
-version = 1.1.2
 author = Sydney Gems
 author_email = sydney@gems.technology
 description = Video and Image optimizer
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/daufinsyd/optilibre
 project_urls =
```

### Comparing `optilibre-1.1.2/src/optilibre/cli.py` & `optilibre-1.2.0/src/optilibre/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import optilibre
 import optilibre.helpers as helpers
 import optilibre.runner as runner
 
 import coloredlogs
 
+
 @click.group()
 @click.option('--debug/--no-debug', default=False)
 @click.version_option(optilibre.__version__)
 def cli(debug):
     if debug:
         coloredlogs.install(level=logging.DEBUG)
     else:
```

### Comparing `optilibre-1.1.2/src/optilibre.egg-info/PKG-INFO` & `optilibre-1.2.0/src/optilibre.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: optilibre
-Version: 1.1.2
+Version: 1.2.0
 Summary: Video and Image optimizer
 Home-page: https://gitlab.com/daufinsyd/optilibre
 Author: Sydney Gems
 Author-email: sydney@gems.technology
-License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/daufinsyd/optilibre/-/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -65,9 +63,7 @@
  - any -> h265 (requires ffmpeg with libx265 encoder)
 
 ### Images
 
  - jpeg -> jpeg (requires jpegoptim)
  - any jpeg -> jpeg-xl (requires cjxl)
 
-
-
```


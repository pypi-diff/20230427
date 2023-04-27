# Comparing `tmp/podcast_downloader-0.4.0.tar.gz` & `tmp/podcast_downloader-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_downloader-0.4.0.tar", last modified: Sun Jan 22 17:02:06 2023, max compression
+gzip compressed data, was "podcast_downloader-0.5.0.tar", last modified: Thu Apr 27 20:06:25 2023, max compression
```

## Comparing `podcast_downloader-0.4.0.tar` & `podcast_downloader-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:02:06.940698 podcast_downloader-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-22 17:01:58.000000 podcast_downloader-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-01-22 17:02:06.940698 podcast_downloader-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-01-22 17:01:58.000000 podcast_downloader-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:02:06.940698 podcast_downloader-0.4.0/podcast_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 17:01:58.000000 podcast_downloader-0.4.0/podcast_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-01-22 17:01:58.000000 podcast_downloader-0.4.0/podcast_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-01-22 17:01:58.000000 podcast_downloader-0.4.0/podcast_downloader/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-01-22 17:01:58.000000 podcast_downloader-0.4.0/podcast_downloader/downloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-22 17:01:58.000000 podcast_downloader-0.4.0/podcast_downloader/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-01-22 17:01:58.000000 podcast_downloader-0.4.0/podcast_downloader/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-01-22 17:01:58.000000 podcast_downloader-0.4.0/podcast_downloader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:02:06.940698 podcast_downloader-0.4.0/podcast_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-01-22 17:02:06.000000 podcast_downloader-0.4.0/podcast_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-01-22 17:02:06.000000 podcast_downloader-0.4.0/podcast_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 17:02:06.000000 podcast_downloader-0.4.0/podcast_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-22 17:02:06.000000 podcast_downloader-0.4.0/podcast_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-22 17:02:06.000000 podcast_downloader-0.4.0/podcast_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-22 17:02:06.940698 podcast_downloader-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-01-22 17:01:58.000000 podcast_downloader-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:06:25.317252 podcast_downloader-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-27 20:06:25.317252 podcast_downloader-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:06:25.317252 podcast_downloader-0.5.0/podcast_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/downloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:06:25.317252 podcast_downloader-0.5.0/podcast_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-27 20:06:25.000000 podcast_downloader-0.5.0/podcast_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 20:06:25.000000 podcast_downloader-0.5.0/podcast_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:06:25.000000 podcast_downloader-0.5.0/podcast_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 20:06:25.000000 podcast_downloader-0.5.0/podcast_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 20:06:25.000000 podcast_downloader-0.5.0/podcast_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:06:25.317252 podcast_downloader-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/setup.py
```

### Comparing `podcast_downloader-0.4.0/LICENSE` & `podcast_downloader-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.4.0/PKG-INFO` & `podcast_downloader-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast_downloader
-Version: 0.4.0
+Version: 0.5.0
 Summary: The script for downloading the recent mp3 from given RSS channels
 Home-page: https://github.com/dplocki/podcast-downloader
 Author: Dawid Plocki
 Author-email: dawid.plocki@gmail.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -12,14 +12,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Podcast Downloader
 
+![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
+![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
+![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
+
 The Python module for downloading files from given RSS feeds.
 It is not using database of any sort. It require configuration file.
 
 The script is analyzing the directory where it put the previously downloaded files.
 It is compering the last added file with the rss feed, finding the missing ones, and downloading them.
 
 As name suggested, the script is designed for podcasts. The files searched by default are mp3.
```

### Comparing `podcast_downloader-0.4.0/README.md` & `podcast_downloader-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Podcast Downloader
 
+![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
+![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
+![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
+
 The Python module for downloading files from given RSS feeds.
 It is not using database of any sort. It require configuration file.
 
 The script is analyzing the directory where it put the previously downloaded files.
 It is compering the last added file with the rss feed, finding the missing ones, and downloading them.
 
 As name suggested, the script is designed for podcasts. The files searched by default are mp3.
```

### Comparing `podcast_downloader-0.4.0/podcast_downloader/__main__.py` & `podcast_downloader-0.5.0/podcast_downloader/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 import os
 from typing import Callable, Dict, Iterable
 import urllib
 import argparse
 import re
 import time
+import sys
 
 from functools import partial
 from . import configuration
 
 from podcast_downloader.configuration import (
     configuration_verification,
     get_label_to_date,
     get_n_age_date,
     parse_day_label,
 )
-from .utils import log, compose, warning
-from .downloaded import get_extensions_checker, get_last_downloaded
+from .utils import log, compose, log_error, warning
+from .downloaded import get_downloaded_files, get_extensions_checker
 from .parameters import merge_parameters_collection, load_configuration_file, parse_argv
 from .rss import (
     RSSEntity,
     build_only_allowed_filter_for_link_data,
     build_only_new_entities,
     file_template_to_file_name,
     flatten_rss_links_data,
     get_raw_rss_entries_from_web,
+    limit_file_name,
     only_last_entity,
     only_entities_from_date,
 )
 
 
 def download_rss_entity_to_path(
     to_file_name_function: Callable[[RSSEntity], str], path: str, rss_entity: RSSEntity
 ):
-    return urllib.request.urlretrieve(
-        rss_entity.link, os.path.join(path, to_file_name_function(rss_entity))
-    )
+    path_to_file = os.path.join(path, to_file_name_function(rss_entity))
+
+    try:
+        return urllib.request.urlretrieve(rss_entity.link, path_to_file)
+    except Exception as exception:
+        log_error(
+            'The podcast file "{}" could not be saved to disk "{}" due to the following error:\n{}',
+            rss_entity.link,
+            path_to_file,
+            exception,
+        )
 
 
 def build_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "--downloads_limit",
@@ -78,14 +88,23 @@
         day_label = parse_day_label(from_nth_day_match[1])
 
         return only_entities_from_date(get_label_to_date(day_label)(local_time))
 
     raise Exception(f"The value the '{configuration_value}' is not recognizable")
 
 
+def is_windows_running():
+    return sys.platform == "win32"
+
+
+def get_system_file_name_limit(sub_configuration: Dict[str, str]) -> int:
+    # on Windows, the file name is limited to 260 characters including the path to it
+    return 255 if is_windows_running() else 260 - len(sub_configuration["path"]) - 1
+
+
 def configuration_to_function_rss_to_name(
     configuration_value: str, sub_configuration: Dict[str, str]
 ) -> Callable[[RSSEntity], str]:
     if (
         configuration.CONFIG_PODCASTS_REQUIRE_DATE in sub_configuration
         and configuration.CONFIG_FILE_NAME_TEMPLATE not in sub_configuration
     ):
@@ -131,16 +150,19 @@
         log("There is a problem with configuration file: {}", error)
         exit(1)
 
     RSS_SOURCES = CONFIGURATION[configuration.CONFIG_PODCASTS]
     DOWNLOADS_LIMITS = CONFIGURATION[configuration.CONFIG_DOWNLOADS_LIMIT]
 
     for rss_source in RSS_SOURCES:
+        file_length_limit = get_system_file_name_limit(rss_source)
         rss_source_name = rss_source[configuration.CONFIG_PODCASTS_NAME]
-        rss_source_path = rss_source[configuration.CONFIG_PODCASTS_PATH]
+        rss_source_path = os.path.expanduser(
+            rss_source[configuration.CONFIG_PODCASTS_PATH]
+        )
         rss_source_link = rss_source[configuration.CONFIG_PODCASTS_RSS_LINK]
         rss_disable = rss_source.get(configuration.CONFIG_PODCASTS_DISABLE, False)
         rss_file_name_template_value = rss_source.get(
             configuration.CONFIG_FILE_NAME_TEMPLATE,
             CONFIGURATION[configuration.CONFIG_FILE_NAME_TEMPLATE],
         )
         rss_if_directory_empty = rss_source.get(
@@ -160,17 +182,21 @@
 
         to_name_function = configuration_to_function_rss_to_name(
             rss_file_name_template_value, rss_source
         )
         on_directory_empty = configuration_to_function_on_empty_directory(
             rss_if_directory_empty
         )
-        last_downloaded_file = get_last_downloaded(
-            get_extensions_checker(rss_podcast_extensions), rss_source_path
+
+        downloaded_files = list(
+            get_downloaded_files(
+                get_extensions_checker(rss_podcast_extensions), rss_source_path
+            )
         )
+        last_downloaded_file = downloaded_files[0] if downloaded_files else None
 
         download_limiter_function = (
             partial(build_only_new_entities(to_name_function), last_downloaded_file)
             if last_downloaded_file
             else on_directory_empty
         )
 
@@ -182,28 +208,43 @@
             flatten_rss_links_data,
             get_raw_rss_entries_from_web,
         )(rss_source_link)
 
         log('Last downloaded file "{}"', last_downloaded_file or "<none>")
 
         if missing_files_links:
-            download_files = partial(download_rss_entity_to_path, to_name_function)
-
+            to_real_podcast_file_name = compose(
+                partial(limit_file_name, file_length_limit), to_name_function
+            )
+
+            download_podcast = partial(
+                download_rss_entity_to_path, to_real_podcast_file_name
+            )
             for rss_entry in reversed(missing_files_links):
+                wanted_podcast_file_name = to_name_function(rss_entry)
+                if wanted_podcast_file_name in downloaded_files:
+                    continue
+
                 if DOWNLOADS_LIMITS == 0:
                     continue
 
+                if len(wanted_podcast_file_name) > file_length_limit:
+                    warning(
+                        'Your system cannot support the full podcast file name "{}". The name will be shortened',
+                        wanted_podcast_file_name,
+                    )
+
                 log(
                     '{}: Downloading file: "{}" saved as "{}"',
                     rss_source_name,
                     rss_entry.link,
-                    to_name_function(rss_entry),
+                    to_real_podcast_file_name(rss_entry),
                 )
 
-                download_files(rss_source_path, rss_entry)
+                download_podcast(rss_source_path, rss_entry)
                 DOWNLOADS_LIMITS -= 1
         else:
             log("{}: Nothing new", rss_source_name)
 
         log("-" * 30)
 
     log("Finished")
```

### Comparing `podcast_downloader-0.4.0/podcast_downloader/configuration.py` & `podcast_downloader-0.5.0/podcast_downloader/configuration.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.4.0/podcast_downloader/downloaded.py` & `podcast_downloader-0.5.0/podcast_downloader/downloaded.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,13 +27,7 @@
     is_directory_file = partial(is_file, podcast_directory)
 
     return (
         file
         for file in get_files_from(podcast_directory)
         if podcast_files_filter(file) and is_directory_file(file)
     )
-
-
-def get_last_downloaded(
-    podcast_files_filter: Callable[[str], bool], podcast_directory: str
-) -> str:
-    return next(get_downloaded_files(podcast_files_filter, podcast_directory), None)
```

### Comparing `podcast_downloader-0.4.0/podcast_downloader/parameters.py` & `podcast_downloader-0.5.0/podcast_downloader/parameters.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.4.0/podcast_downloader/rss.py` & `podcast_downloader-0.5.0/podcast_downloader/rss.py`

 * *Files 23% similar despite different names*

```diff
@@ -43,23 +43,39 @@
     return ""
 
 
 def str_to_filename(value: str) -> str:
     value = unicodedata.normalize("NFKC", value)
     value = re.sub(r"[\u0000-\u001F\u007F\*/:<>\?\\\|]", " ", value)
 
-    return value.strip()[:FILE_NAME_CHARACTER_LIMIT]
+    return value.strip()
 
 
 def file_template_to_file_name(name_template: str, entity: RSSEntity) -> str:
     return (
         name_template.replace("%file_name%", link_to_file_name(entity.link))
         .replace("%publish_date%", time.strftime("%Y%m%d", entity.published_date))
         .replace("%file_extension%", link_to_extension(entity.link))
         .replace("%title%", str_to_filename(entity.title))
+        .strip()
+    )
+
+
+def limit_file_name(maximum_length: int, file_name: str) -> str:
+    last_dot_index = file_name.rfind(".")
+    if last_dot_index == -1:
+        return file_name[:maximum_length]
+
+    file_name_length = len(file_name)
+    if file_name_length <= maximum_length:
+        return file_name
+
+    return (
+        file_name[: maximum_length - file_name_length + last_dot_index]
+        + file_name[last_dot_index:]
     )
 
 
 def get_raw_rss_entries_from_web(
     rss_link: str,
 ) -> Generator[feedparser.FeedParserDict, None, None]:
     yield from feedparser.parse(rss_link).entries
```

### Comparing `podcast_downloader-0.4.0/podcast_downloader/utils.py` & `podcast_downloader-0.5.0/podcast_downloader/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,9 +18,15 @@
 
 def warning(message, *parameters):
     print(
         f"[\033[2m{datetime.now():%Y-%m-%d %H:%M:%S}\033[0m] \033[33mWarning:\033[0m {mark_parameters_in_message(message, *parameters)}"
     )
 
 
+def log_error(message, *parameters):
+    print(
+        f"[\033[2m{datetime.now():%Y-%m-%d %H:%M:%S}\033[0m] \033[31mError:\033[0m {mark_parameters_in_message(message, *parameters)}"
+    )
+
+
 def compose(*functions):
     return reduce(lambda f, g: lambda x: f(g(x)), functions)
```

### Comparing `podcast_downloader-0.4.0/podcast_downloader.egg-info/PKG-INFO` & `podcast_downloader-0.5.0/podcast_downloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast-downloader
-Version: 0.4.0
+Version: 0.5.0
 Summary: The script for downloading the recent mp3 from given RSS channels
 Home-page: https://github.com/dplocki/podcast-downloader
 Author: Dawid Plocki
 Author-email: dawid.plocki@gmail.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -12,14 +12,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Podcast Downloader
 
+![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
+![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
+![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
+
 The Python module for downloading files from given RSS feeds.
 It is not using database of any sort. It require configuration file.
 
 The script is analyzing the directory where it put the previously downloaded files.
 It is compering the last added file with the rss feed, finding the missing ones, and downloading them.
 
 As name suggested, the script is designed for podcasts. The files searched by default are mp3.
```

### Comparing `podcast_downloader-0.4.0/setup.py` & `podcast_downloader-0.5.0/setup.py`

 * *Files identical despite different names*


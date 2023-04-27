# Comparing `tmp/cyberdrop-dl-4.1.15.tar.gz` & `tmp/cyberdrop-dl-4.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.15.tar", last modified: Thu Apr 27 04:50:11 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.16.tar", last modified: Thu Apr 27 18:21:56 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.15.tar` & `cyberdrop-dl-4.1.16.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.429360 cyberdrop-dl-4.1.15/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.429360 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.429360 cyberdrop-dl-4.1.15/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17378 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.429360 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.152648 cyberdrop-dl-4.1.16/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-27 18:21:56.152648 cyberdrop-dl-4.1.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.144648 cyberdrop-dl-4.1.16/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.144648 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.148648 cyberdrop-dl-4.1.16/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.148648 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14912 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.148648 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17378 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.152648 cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19342 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.144648 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-27 18:21:56.152648 cyberdrop-dl-4.1.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/setup.py
```

### Comparing `cyberdrop-dl-4.1.15/LICENSE` & `cyberdrop-dl-4.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/PKG-INFO` & `cyberdrop-dl-4.1.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.15
+Version: 4.1.16
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.15 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.16 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.15/README.md` & `cyberdrop-dl-4.1.16/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 config_default = {
     "Apply_Config": False,
     "Configuration": {
         "Authentication": {
             "gofile_api_key": "",
             "pixeldrain_api_key": "",
+            "nudostar_username": "",
+            "nudostar_password": "",
             "simpcity_username": "",
             "simpcity_password": "",
             "socialmediagirls_username": "",
             "socialmediagirls_password": "",
             "xbunker_username": "",
             "xbunker_password": "",
         },
```

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,9 +235,9 @@
 class SkipData:
     """The allows optoins for domains to skip when scraping"""
     supported_hosts: ClassVar[Tuple[str]] = ("anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
                                              "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gofile",
                                              "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish",
                                              "gallery.deltaporno.com", "kemono.party",
                                              "lovefap", "nsfw.xxx", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
-                                             "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr")
+                                             "saint", "nudostar", "simpcity", "socialmediagirls", "xbunker", "xbunkr")
     sites: List[str]
```

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,37 +15,65 @@
     logger,
     make_title_safe,
 )
 from ..base_functions.data_classes import CascadeItem, MediaItem
 from ..base_functions.error_classes import FailedLoginFailure, NoExtensionFailure
 
 if TYPE_CHECKING:
-    from pathlib import Path
-
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
-async def write_last_post_file(file: Path, url: str):
-    """Writes the last post url from a thread to the specified file"""
-    async with aiofiles.open(file, mode='a') as f:
-        await f.write(url + '\n')
-
-
 @dataclass
 class ParseSpec:
     """Class for specific selectors of supported domains"""
     domain: str
-    title_clutter_tag: str = field(init=False)
+    title_block_element: str = "h1[class=p-title-value]"
+    title_clutter_element: str = field(init=False)
+
+    posts_block_element: str = "div[class*=message-main]"
+    posts_number_element: str = field(init=False)
+    posts_number_attribute: str = "href"
+
+    post_content_element: str = "div[class=bbWrapper]"
+    block_quote_element: str = "blockquote"
+
+    links_element: str = "a"
+    links_attribute: str = "href"
+
+    images_element: str = field(init=False)
+    images_attribute: str = field(init=False)
+
+    video_element: str = "video source"
+    video_attribute: str = "src"
+    saint_iframe_element: str = "iframe[class=saint-iframe]"
+    saint_iframe_attribute: str = "src"
+
+    embedded_content_element: str = "span[data-s9e-mediaembed-iframe]"
+    embedded_content_attribute: str = "data-s9e-mediaembed-iframe"
+
+    attachment_block_element: str = "section[class=message-attachments]"
+    attachment_element: str = "a"
+    attachment_attribute: str = "href"
+
+    next_page_element: str = 'a[class="pageNav-jump pageNav-jump--next"]'
+    next_page_attribute: str = "href"
 
     def __post_init__(self):
-        if self.domain in ("simpcity", "xbunker"):
-            self.title_clutter_tag = "a"
-        elif self.domain == "socialmediagirls":
-            self.title_clutter_tag = "span"
+        if self.domain in ("simpcity", "xbunker", "socialmediagirls"):
+            self.title_clutter_element = "a" if self.domain in ("simpcity", "xbunker") else "span"
+            self.posts_number_element = "li[class=u-concealed] a"
+            self.images_element = "div[class*=bbImage]"
+            self.images_attribute = "data-src"
+
+        elif self.domain == "nudostar":
+            self.title_clutter_element = "span"
+            self.posts_number_element = "a[class=u-concealed]"
+            self.images_element = "img[class*=bbImage]"
+            self.images_attribute = "src"
 
 
 class ForumLogin:
     def __init__(self, name: str, username: str, password: str):
         self.name = name
         self.logged_in = False
         self.username = username
@@ -60,15 +88,17 @@
         while True:
             try:
                 if self.logged_in:
                     return
                 if attempt == 5:
                     raise FailedLoginFailure()
 
-                domain = URL("https://" + url.host) / "login"
+                domain = URL("https://" + url.host) / "forum/login" if "nudostar" in url.host else \
+                    URL("https://" + url.host) / "login"
+
                 text = await session.get_text(domain)
                 await asyncio.sleep(5)
                 soup = BeautifulSoup(text, 'html.parser')
 
                 inputs = soup.select('form input')
                 data = {
                     elem['name']: elem['value']
@@ -89,23 +119,27 @@
                 self.logged_in = True
             except asyncio.exceptions.TimeoutError:
                 attempt += 1
                 continue
 
 
 class XenforoCrawler:
-    domains = ("simpcity", "socialmediagirls", "xbunker")
+    domains = ("nudostar", "simpcity", "socialmediagirls", "xbunker")
 
     def __init__(self, *, scraping_mapper, args: dict, SQL_Helper: SQLHelper, quiet: bool):
         self.include_id = args["Runtime"]["include_id"]
         self.quiet = quiet
         self.separate_posts = args["Forum_Options"]["separate_posts"]
         self.output_last = args["Forum_Options"]["output_last_forum_post"]
         self.output_last_file = args["Files"]["output_last_forum_post_file"]
 
+        self.nudostar = ForumLogin("NudoStar",
+                                   args["Authentication"]["nudostar_username"],
+                                   args["Authentication"]["nudostar_password"])
+
         self.simpcity = ForumLogin("SimpCity",
                                    args["Authentication"]["simpcity_username"],
                                    args["Authentication"]["simpcity_password"])
 
         self.socialmediagirls = ForumLogin("SocialMediaGirls",
                                            args["Authentication"]["socialmediagirls_username"],
                                            args["Authentication"]["socialmediagirls_password"])
@@ -127,14 +161,16 @@
         try:
             if "simpcity" in url.host:
                 await self.simpcity.login(session, url, self.quiet)
             elif "socialmediagirls" in url.host:
                 await self.socialmediagirls.login(session, url, self.quiet)
             elif "xbunker" in url.host:
                 await self.xbunker.login(session, url, self.quiet)
+            elif "nudostar" in url.host:
+                await self.nudostar.login(session, url, self.quiet)
 
             domain = next((domain for domain in self.domains if domain in url.host), None)
             if domain:
                 title = await self.parse_forum(session, scrape_url, ParseSpec(domain), cascade, "", post_num)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
@@ -167,15 +203,15 @@
             if link.startswith('//'):
                 link = "https:" + link
             elif link.startswith('/'):
                 link = domain / link[1:]
             found_links.append([URL(link), temp_title])
         return found_links
 
-    async def get_embedded(self, post_content, selector, attribute, domain, temp_title):
+    async def get_embedded(self, post_content, selector, attribute, temp_title):
         """Gets embedded media from post content based on selector and attribute provided"""
         found_links = []
         links = post_content.select(selector)
         for link in links:
             embed_data = link.get(attribute)
             embed_data = embed_data.replace("\/\/", "https://www.")
             embed_data = embed_data.replace("\\", "")
@@ -199,16 +235,15 @@
         """Splits given links into direct links and external links,
         returns external links, adds internal to the cascade"""
         forum_direct_urls = [x for x in content_links if x[0].host.replace(".st", ".su") in url.host]
         forum_direct_urls.extend([x for x in content_links if url.host in x[0].host.replace(".st", ".su")])
         forum_direct_urls.extend([x for x in content_links if "smgmedia" in x[0].host])
         content_links = [x for x in content_links if x not in forum_direct_urls]
         for link_title_bundle in forum_direct_urls:
-            link = link_title_bundle[0]
-            temp_title = link_title_bundle[1]
+            link, temp_title = link_title_bundle
             in_prog_title = temp_title + "/Attachments"
             if str(link).endswith("/"):
                 link = URL(str(link)[:-1])
             if 'attachments' in link.parts or 'content' in link.parts or 'data' in link.parts:
                 completed = await self.SQL_Helper.check_complete_singular(domain, link)
                 try:
                     filename, ext = await get_filename_and_ext(link.name, True)
@@ -233,69 +268,74 @@
         """Parses forum threads"""
         soup = await session.get_BS4(url)
 
         domain = URL("https://" + url.host)
         post_num_str = None
         content_links = []
 
-        title_block = soup.select_one("h1[class=p-title-value]")
-        for elem in title_block.find_all(spec.title_clutter_tag):
+        title_block = soup.select_one(spec.title_block_element)
+        for elem in title_block.find_all(spec.title_clutter_element):
             elem.decompose()
 
         if title:
             pass
         else:
             title = title_block.text
             title = await make_title_safe(title.replace("\n", "").strip())
 
-        posts = soup.select("div[class='message-main uix_messageContent js-quickEditTarget']")
+        posts = soup.select(spec.posts_block_element)
 
         for post in posts:
-            post_num_str = post.select_one("li[class=u-concealed] a").get('href').split('/')[-1]
+            post_num_str = post.select_one(spec.posts_number_element).get(spec.posts_number_attribute).split('/')[-1]
             post_num_int = int(post_num_str.split('post-')[-1])
             if post_number > post_num_int:
                 continue
 
             temp_title = title + "/" + post_num_str if self.separate_posts else title
 
-            for elem in post.find_all('blockquote'):
+            for elem in post.find_all(spec.block_quote_element):
                 elem.decompose()
-            post_content = post.select_one("div[class=bbWrapper]")
+            post_content = post.select_one(spec.post_content_element)
 
             # Get Links
-            content_links.extend(await self.get_links(post_content, "a", "href", domain, temp_title))
+            content_links.extend(await self.get_links(post_content, spec.links_element, spec.links_attribute, domain,
+                                                      temp_title))
 
             # Get Images
-            content_links.extend(await self.get_links(post_content, "div[class='bbImageWrapper js-lbImage']", "data-src", domain, temp_title))
-            content_links.extend(await self.get_links(post_content, "div[class='bbImageWrapper lazyload js-lbImage']", "data-src", domain, temp_title))
+            content_links.extend(await self.get_links(post_content, spec.images_element, spec.images_attribute, domain,
+                                                      temp_title))
 
             # Get Videos:
-            content_links.extend(await self.get_links(post_content, "video source", "src", domain, temp_title))
-            content_links.extend(await self.get_links(post_content, "iframe[class=saint-iframe]", "src", domain, temp_title))
+            content_links.extend(await self.get_links(post_content, spec.video_element, spec.video_attribute, domain,
+                                                      temp_title))
+            content_links.extend(await self.get_links(post_content, spec.saint_iframe_element,
+                                                      spec.saint_iframe_attribute, domain, temp_title))
 
             # Get Other Embedded Content
-            content_links.extend(await self.get_embedded(post_content, "span[data-s9e-mediaembed-iframe]", "data-s9e-mediaembed-iframe",
-                                 domain, temp_title))
+            content_links.extend(await self.get_embedded(post_content, spec.embedded_content_element,
+                                                         spec.embedded_content_attribute, temp_title))
 
             # Get Attachments
-            attachments_block = post.select_one("section[class=message-attachments]")
-            content_links.extend(await self.get_links(attachments_block, "a[class='file-preview js-lbImage']", "href", domain, temp_title))
+            attachments_block = post.select_one(spec.attachment_block_element)
+            content_links.extend(await self.get_links(attachments_block, spec.attachment_element,
+                                                      spec.attachment_attribute, domain, temp_title))
 
         # Handle links
         content_links = await self.filter_content_links(cascade, content_links, url, spec.domain)
         await self.handle_external_links(content_links, url)
 
-        next_page = soup.select_one('a[class="pageNav-jump pageNav-jump--next"]')
+        next_page = soup.select_one(spec.next_page_element)
         if next_page is not None:
-            next_page = next_page.get('href')
+            next_page = next_page.get(spec.next_page_attribute)
             if next_page is not None:
                 if next_page.startswith('/'):
                     next_page = domain / next_page[1:]
                 next_page = URL(next_page)
                 await self.parse_forum(session, next_page, spec, cascade, title, post_number)
         elif self.output_last:
             if 'page-' in url.raw_name or 'post-' in url.raw_name:
                 last_post_url = url.parent / post_num_str
             else:
                 last_post_url = url / post_num_str
-            await write_last_post_file(self.output_last_file, str(last_post_url))
+            async with aiofiles.open(self.output_last_file, mode='a') as f:
+                await f.write(f'{last_post_url}\n')
         return title
```

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,16 @@
     forum_opts.add_argument("--separate-posts", help="separates forum scraping into folders by post number", action="store_true")
 
     # Authentication details
     config_group = config_data["Authentication"]
     auth_opts = parser.add_argument_group("Authentication options")
     auth_opts.add_argument("--gofile-api-key", help="api key for premium gofile", default=config_group["gofile_api_key"])
     auth_opts.add_argument("--pixeldrain-api-key", help="api key for premium pixeldrain", default=config_group["pixeldrain_api_key"])
+    auth_opts.add_argument("--nudostar-username", help="username to login to nudostar", default=config_group["nudostar_username"])
+    auth_opts.add_argument("--nudostar-password", help="password to login to nudostar", default=config_group['nudostar_password'])
     auth_opts.add_argument("--simpcity-username", help="username to login to simpcity", default=config_group["simpcity_username"])
     auth_opts.add_argument("--simpcity-password", help="password to login to simpcity", default=config_group['simpcity_password'])
     auth_opts.add_argument("--socialmediagirls-username", help="username to login to socialmediagirls", default=config_group["socialmediagirls_username"])
     auth_opts.add_argument("--socialmediagirls-password", help="password to login to socialmediagirls", default=config_group["socialmediagirls_password"])
     auth_opts.add_argument("--xbunker-username", help="username to login to xbunker", default=config_group["xbunker_username"])
     auth_opts.add_argument("--xbunker-password", help="password to login to xbunker", default=config_group["xbunker_password"])
```

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/Scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,27 +85,28 @@
         self.bunkr_limiter = AsyncRateLimiter(15)
         self.coomeno_limiter = AsyncRateLimiter(6)
         self.gofile_limiter = AsyncRateLimiter(max_calls=1, period=2)
 
         self.gofile_semaphore = asyncio.Semaphore(1)
         self.jpgfish_semaphore = asyncio.Semaphore(5)
         self.cyberfile_semaphore = asyncio.Semaphore(2)
+        self.nudostar_semaphore = asyncio.Semaphore(1)
         self.simpcity_semaphore = asyncio.Semaphore(1)
         self.socialmediagirls_semaphore = asyncio.Semaphore(1)
         self.xbunker_semaphore = asyncio.Semaphore(1)
 
         self.mapping = {"anonfiles": self.Anonfiles, "bayfiles": self.Anonfiles, "xbunkr": self.XBunkr,
                         "bunkr": self.Bunkr, "cyberdrop": self.Cyberdrop, "cyberfile": self.CyberFile,
                         "erome": self.Erome, "fapello": self.Fapello, "gfycat": self.Gfycat, "gofile": self.GoFile,
                         "hgamecg": self.HGameCG, "imgbox": self.ImgBox, "pixeldrain": self.PixelDrain,
                         "postimg": self.PostImg, "saint": self.Saint, "img.kiwi": self.ShareX,
                         "jpg.church": self.ShareX, "jpg.fish": self.ShareX, "pixl.li": self.ShareX,
                         "nsfw.xxx": self.NSFW_XXX, "pimpandhost": self.PimpAndHost, "lovefap": self.LoveFap,
                         "e-hentai": self.EHentai, "gallery.deltaporno": self.ShareX, "vk.com": self.vk_redirect,
-                        "coomer.party": self.Coomeno, "kemono.party": self.Coomeno,
+                        "coomer.party": self.Coomeno, "kemono.party": self.Coomeno, "nudostar": self.Xenforo,
                         "simpcity": self.Xenforo, "socialmediagirls": self.Xenforo, "xbunker": self.Xenforo}
 
     async def _handle_album_additions(self, domain: str, album_obj: AlbumItem, title=None) -> None:
         if title:
             await album_obj.append_title(title)
             await self.Forums.add_album_to_thread(title, domain, album_obj)
         else:
@@ -322,20 +323,23 @@
                                                   quiet=self.quiet)
         title = None
         cascade = None
 
         if "simpcity" in url.host:
             async with self.simpcity_semaphore:
                 cascade, title = await self.xenforo_crawler.fetch(xenforo_session, url)
-        if "socialmediagirls" in url.host:
+        elif "socialmediagirls" in url.host:
             async with self.socialmediagirls_semaphore:
                 cascade, title = await self.xenforo_crawler.fetch(xenforo_session, url)
-        if "xbunker" in url.host:
+        elif "xbunker" in url.host:
             async with self.xbunker_semaphore:
                 cascade, title = await self.xenforo_crawler.fetch(xenforo_session, url)
+        elif "nudostar" in url.host:
+            async with self.nudostar_semaphore:
+                cascade, title = await self.xenforo_crawler.fetch(xenforo_session, url)
         if not title or await cascade.is_empty():
             await xenforo_session.exit_handler()
             return
         await self.Forums.add_thread(title, cascade)
         await xenforo_session.exit_handler()
 
     """URL to Function Mapper"""
```

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.15
+Version: 4.1.16
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.15 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.16 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.15/setup.cfg` & `cyberdrop-dl-4.1.16/setup.cfg`

 * *Files identical despite different names*


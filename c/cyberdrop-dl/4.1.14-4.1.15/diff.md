# Comparing `tmp/cyberdrop-dl-4.1.14.tar.gz` & `tmp/cyberdrop-dl-4.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.14.tar", last modified: Mon Apr 24 23:27:15 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.15.tar", last modified: Thu Apr 27 04:50:11 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.14.tar` & `cyberdrop-dl-4.1.15.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:14.999000 cyberdrop-dl-4.1.14/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-24 23:27:14.999000 cyberdrop-dl-4.1.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:14.987000 cyberdrop-dl-4.1.14/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:14.991000 cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:14.991000 cyberdrop-dl-4.1.14/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:14.995000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    19384 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:14.999000 cyberdrop-dl-4.1.14/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17378 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:14.999000 cyberdrop-dl-4.1.14/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:27:14.987000 cyberdrop-dl-4.1.14/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-24 23:27:14.000000 cyberdrop-dl-4.1.14/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-24 23:27:14.000000 cyberdrop-dl-4.1.14/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:27:14.000000 cyberdrop-dl-4.1.14/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 23:27:14.000000 cyberdrop-dl-4.1.14/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-24 23:27:14.000000 cyberdrop-dl-4.1.14/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 23:27:14.000000 cyberdrop-dl-4.1.14/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-24 23:27:14.999000 cyberdrop-dl-4.1.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:27:02.000000 cyberdrop-dl-4.1.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.429360 cyberdrop-dl-4.1.15/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.429360 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.429360 cyberdrop-dl-4.1.15/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17378 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:50:11.429360 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 04:50:11.000000 cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-27 04:50:11.433360 cyberdrop-dl-4.1.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 04:50:02.000000 cyberdrop-dl-4.1.15/setup.py
```

### Comparing `cyberdrop-dl-4.1.14/LICENSE` & `cyberdrop-dl-4.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/PKG-INFO` & `cyberdrop-dl-4.1.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.14
+Version: 4.1.15
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.14 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.15 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.14/README.md` & `cyberdrop-dl-4.1.15/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,156 +1,130 @@
 from __future__ import annotations
 
 import asyncio
+from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import CascadeItem
 
 if TYPE_CHECKING:
+    from bs4 import Tag
+
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
+@dataclass
+class ParseSpec:
+    """Class for specific selectors of supported domains"""
+    domain: str
+    posts_selectors: list[str] = field(init=False)
+    next_page_selector: str = field(init=False)
+
+    def __post_init__(self):
+        if self.domain == "coomer":
+            self.posts_selectors = ['h2[class=post-card__heading] a']
+            self.next_page_selector = 'a[title="Next page"]'
+        elif self.domain == "kemono":
+            self.posts_selectors = ['article[class="post-card post-card--preview"] a', 'article[class="post-card"] a']
+            self.next_page_selector = 'a[class=next]'
+
+
 class CoomenoCrawler:
     def __init__(self, *, include_id=False, scraping_mapper, separate_posts=False, quiet: bool, SQL_Helper: SQLHelper):
         self.include_id = include_id
         self.quiet = quiet
         self.scraping_mapper = scraping_mapper
         self.separate_posts = separate_posts
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL):
         """Director for Coomer/Kemono scraping"""
         await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         cascade = CascadeItem({})
         title = None
         try:
-            if "coomer" in url.host:
-                title = await self.handle_coomer(session, url, cascade)
-            elif "kemono" in url.host:
-                title = await self.handle_kemono(session, url, cascade)
+            domain = next((domain for domain in ("coomer", "kemono") if domain in url.host), None)
+            if domain:
+                title = await self.handle_coomeno(session, url, domain, cascade)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         await self.SQL_Helper.insert_cascade(cascade)
         await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return cascade, title
 
-    async def handle_coomer(self, session: ScrapeSession, url: URL, cascade: CascadeItem):
-        """Coomer director function"""
-        post_selectors = ['h2[class=post-card__heading] a']
-        next_page_selector = 'a[title="Next page"]'
-        images_selector = 'a[class="fileThumb"]'
-        downloads_selector = 'a[class=post__attachment-link]'
-        text_selector = 'div[class=post__content] a'
-
-        title = "Loose Coomer Files"
-        if "thumbnail" in url.parts:
-            parts = [x for x in url.parts if x not in ("thumbnail", "/")]
-            link = URL("https://coomer.party/" + "/".join(parts))
-
-            media_item = await create_media_item(link, url, self.SQL_Helper, "coomer")
-            await cascade.add_to_album("coomer", title, media_item)
-
-        elif "data" in url.parts:
-            media_item = await create_media_item(url, url, self.SQL_Helper, "coomer")
-            await cascade.add_to_album("coomer", title, media_item)
-
-        elif "post" in url.parts:
-            title = await self.parse_post(session, url, "coomer", cascade, images_selector, downloads_selector,
-                                          text_selector)
-
-        else:
-            title = await self.parse_profile(session, url, "coomer", cascade, post_selectors, next_page_selector,
-                                             images_selector, downloads_selector, text_selector)
-
-        return title
-
-    async def handle_kemono(self, session: ScrapeSession, url: URL, cascade: CascadeItem):
-        """Kemono director function"""
-        post_selectors = ['article[class="post-card post-card--preview"] a', 'article[class="post-card"] a']
-        next_page_selector = 'a[class=next]'
-        images_selector = 'a[class="fileThumb"]'
-        downloads_selector = 'a[class=post__attachment-link]'
-        text_selector = 'div[class=post__content] a'
-
-        title = "Loose Kemono Files"
+    async def handle_coomeno(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem) -> str:
+        """Coomer/Kemono director function"""
+        title = f"Loose {domain.capitalize()} Files"
         if "thumbnail" in url.parts:
             parts = [x for x in url.parts if x not in ("thumbnail", "/")]
-            link = URL("https://kemono.party/" + "/".join(parts))
+            link = URL(f"https://{domain}.party/{'/'.join(parts)}")
 
-            media_item = await create_media_item(link, url, self.SQL_Helper, "kemono")
-            await cascade.add_to_album("kemono", title, media_item)
+            media_item = await create_media_item(link, url, self.SQL_Helper, domain)
+            await cascade.add_to_album(domain, title, media_item)
 
         elif "data" in url.parts:
-            media_item = await create_media_item(url, url, self.SQL_Helper, "kemono")
-            await cascade.add_to_album("kemono", title, media_item)
+            media_item = await create_media_item(url, url, self.SQL_Helper, domain)
+            await cascade.add_to_album(domain, title, media_item)
 
         elif "post" in url.parts:
-            title = await self.parse_post(session, url, "kemono", cascade, images_selector, downloads_selector,
-                                          text_selector)
+            title = await self.parse_post(session, url, domain, cascade)
 
         else:
-            title = await self.parse_profile(session, url, "kemono", cascade, post_selectors, next_page_selector,
-                                             images_selector, downloads_selector, text_selector)
+            title = await self.parse_profile(session, url, ParseSpec(domain), cascade)
 
         return title
 
     async def map_links(self, text_content: list, title: str, referer: URL):
         """Maps external links to other scrapers"""
         tasks = []
         for content in text_content:
             link = URL(content.get('href'))
             tasks.append(asyncio.create_task(self.scraping_mapper.map_url(link, title, referer)))
         if tasks:
             await asyncio.wait(tasks)
 
-    async def parse_profile(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem,
-                            posts_selectors: list, next_page_selector: str, images_selector: str,
-                            downloads_selector: str, text_selector: str):
+    async def parse_profile(self, session: ScrapeSession, url: URL, spec: ParseSpec, cascade: CascadeItem) -> str:
         """Parses profiles with supplied selectors"""
         title = None
         try:
             soup = await session.get_BS4(url)
             title = await make_title_safe(soup.select_one("span[itemprop=name]").get_text())
             title = f"{title} ({url.host})"
 
             posts = []
-            for posts_selector in posts_selectors:
+            for posts_selector in spec.posts_selectors:
                 posts += soup.select(posts_selector)
             for post in posts:
                 path = post.get('href')
                 if path:
                     post_link = URL("https://" + url.host + path)
-                    await self.parse_post(session, post_link, domain, cascade, images_selector, downloads_selector,
-                                          text_selector, title)
+                    await self.parse_post(session, post_link, spec.domain, cascade, title)
 
-            next_page = soup.select_one(next_page_selector)
+            next_page = soup.select_one(spec.next_page_selector)
             if next_page:
                 next_page = next_page.get('href')
                 if next_page:
-                    await self.parse_profile(session, URL("https://" + url.host + next_page), domain, cascade,
-                                             posts_selectors, next_page_selector, images_selector, downloads_selector,
-                                             text_selector)
+                    await self.parse_profile(session, URL("https://" + url.host + next_page), spec, cascade)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return title
 
-    async def parse_post(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem,
-                         images_selector: str, downloads_selector: str, text_selector: str, title=None):
+    async def parse_post(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem, title: str = None) -> str:
         """Parses posts with supplied selectors"""
         try:
             text = await self.SQL_Helper.get_blob(url)
             if not text:
                 text = await session.get_text(url)
                 await self.SQL_Helper.insert_blob(text, url)
             soup = BeautifulSoup(text, 'html.parser')
@@ -162,35 +136,32 @@
                     title = title + '/' + await make_title_safe(prefix + post_title)
                 else:
                     title = await make_title_safe(prefix + post_title)
             elif not title:
                 post_title = soup.select_one("h1[class=post__title]").text.replace('\n', '').replace("..", "")
                 title = await make_title_safe(post_title)
 
-            images = soup.select(images_selector)
+            images = soup.select('a[class="fileThumb"]')
             for image in images:
-                href = image.get('href')
-                if href.startswith("/"):
-                    link = URL("https://" + url.host + href)
-                else:
-                    link = URL(href)
-                media_item = await create_media_item(link, url, self.SQL_Helper, domain)
-                await cascade.add_to_album(domain, title, media_item)
+                await self.parse_tag(image, url, domain, title, cascade)
 
-            downloads = soup.select(downloads_selector)
+            downloads = soup.select('a[class=post__attachment-link]')
             for download in downloads:
-                href = download.get('href')
-                if href.startswith("/"):
-                    link = URL("https://" + url.host + href)
-                else:
-                    link = URL(href)
-                media_item = await create_media_item(link, url, self.SQL_Helper, domain)
-                await cascade.add_to_album(domain, title, media_item)
+                await self.parse_tag(download, url, domain, title, cascade)
 
-            text_content = soup.select(text_selector)
+            text_content = soup.select('div[class=post__content] a')
             await self.map_links(text_content, title, url)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return title
+
+    async def parse_tag(self, tag: Tag, url: URL, domain: str, title: str, cascade: CascadeItem):
+        """Convert link from tag to MediaItem and add it to cascade"""
+        href = tag.get('href')
+        if href.startswith("/"):
+            href = "https://" + url.host + href
+        link = URL(href)
+        media_item = await create_media_item(link, url, self.SQL_Helper, domain)
+        await cascade.add_to_album(domain, title, media_item)
```

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,17 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> Optional[AlbumItem]:
         """Basic director for fapello"""
         await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
 
+        if not str(url).endswith("/"):
+            url = url / ""
+
         album_obj = await self.parse_profile(session, url)
 
         await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
     async def parse_profile(self, session: ScrapeSession, url: URL) -> Optional[AlbumItem]:
         """Profile parser, passes posts to parse_post"""
```

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.15/cyberdrop_dl/scraper/Scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.remove_bunkr_id = args['Runtime']['remove_bunkr_identifier']
         self.separate_posts = args["Forum_Options"]["separate_posts"]
         self.quiet = quiet
         self.jdownloader = JDownloader(args['JDownloader'], quiet)
 
         self.jpgfish_limiter = AsyncRateLimiter(10)
         self.bunkr_limiter = AsyncRateLimiter(15)
-        self.coomeno_limiter = AsyncRateLimiter(8)
+        self.coomeno_limiter = AsyncRateLimiter(6)
         self.gofile_limiter = AsyncRateLimiter(max_calls=1, period=2)
 
         self.gofile_semaphore = asyncio.Semaphore(1)
         self.jpgfish_semaphore = asyncio.Semaphore(5)
         self.cyberfile_semaphore = asyncio.Semaphore(2)
         self.simpcity_semaphore = asyncio.Semaphore(1)
         self.socialmediagirls_semaphore = asyncio.Semaphore(1)
```

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.14
+Version: 4.1.15
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.14 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.15 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.14/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.15/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.14/setup.cfg` & `cyberdrop-dl-4.1.15/setup.cfg`

 * *Files identical despite different names*


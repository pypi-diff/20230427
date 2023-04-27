# Comparing `tmp/browse-ocrd-0.5.4.tar.gz` & `tmp/browse-ocrd-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browse-ocrd-0.5.4.tar", last modified: Mon Feb 20 23:27:36 2023, max compression
+gzip compressed data, was "browse-ocrd-0.5.5.tar", last modified: Thu Apr 27 21:03:03 2023, max compression
```

## Comparing `browse-ocrd-0.5.4.tar` & `browse-ocrd-0.5.5.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-02-20 23:27:36.590905 browse-ocrd-0.5.4/
--rw-rw-r--   0 jk        (1000) jk        (1000)     1061 2020-07-21 10:23:15.000000 browse-ocrd-0.5.4/LICENSE
--rw-rw-r--   0 jk        (1000) jk        (1000)      104 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/MANIFEST.in
--rw-rw-r--   0 jk        (1000) jk        (1000)     6748 2023-02-20 23:27:36.590905 browse-ocrd-0.5.4/PKG-INFO
--rw-rw-r--   0 jk        (1000) jk        (1000)     5715 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/README.md
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-02-20 23:27:36.586905 browse-ocrd-0.5.4/browse_ocrd.egg-info/
--rw-rw-r--   0 jk        (1000) jk        (1000)     6748 2023-02-20 23:27:36.000000 browse-ocrd-0.5.4/browse_ocrd.egg-info/PKG-INFO
--rw-rw-r--   0 jk        (1000) jk        (1000)     1428 2023-02-20 23:27:36.000000 browse-ocrd-0.5.4/browse_ocrd.egg-info/SOURCES.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)        1 2023-02-20 23:27:36.000000 browse-ocrd-0.5.4/browse_ocrd.egg-info/dependency_links.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)      282 2023-02-20 23:27:36.000000 browse-ocrd-0.5.4/browse_ocrd.egg-info/entry_points.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)      196 2023-02-20 23:27:36.000000 browse-ocrd-0.5.4/browse_ocrd.egg-info/requires.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)       13 2023-02-20 23:27:36.000000 browse-ocrd-0.5.4/browse_ocrd.egg-info/top_level.txt
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-02-20 23:27:36.586905 browse-ocrd-0.5.4/ocrd_browser/
--rw-rw-r--   0 jk        (1000) jk        (1000)       22 2023-02-20 22:56:59.000000 browse-ocrd-0.5.4/ocrd_browser/__init__.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     4846 2022-10-22 10:12:29.000000 browse-ocrd-0.5.4/ocrd_browser/application.py
--rwxrwxr-x   0 jk        (1000) jk        (1000)     1813 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/main.py
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-02-20 23:27:36.586905 browse-ocrd-0.5.4/ocrd_browser/model/
--rw-rw-r--   0 jk        (1000) jk        (1000)      248 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/model/__init__.py
--rw-rw-r--   0 jk        (1000) jk        (1000)    19026 2023-02-20 22:01:29.000000 browse-ocrd-0.5.4/ocrd_browser/model/document.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     5917 2023-02-20 22:01:29.000000 browse-ocrd-0.5.4/ocrd_browser/model/page.py
--rw-rw-r--   0 jk        (1000) jk        (1000)    21734 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/model/page_xml_renderer.py
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-02-20 23:27:36.586905 browse-ocrd-0.5.4/ocrd_browser/resources/
--rw-rw-r--   0 jk        (1000) jk        (1000)        0 2020-07-27 18:20:55.000000 browse-ocrd-0.5.4/ocrd_browser/resources/__init__.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     2315 2020-08-12 08:30:42.000000 browse-ocrd-0.5.4/ocrd_browser/resources/about-dialog.ui
--rw-rw-r--   0 jk        (1000) jk        (1000)    20112 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/resources/main-window.ui
--rw-rw-r--   0 jk        (1000) jk        (1000)     4460 2020-08-12 08:31:07.000000 browse-ocrd-0.5.4/ocrd_browser/resources/open-dialog.ui
--rw-rw-r--   0 jk        (1000) jk        (1000)      852 2020-08-07 10:41:47.000000 browse-ocrd-0.5.4/ocrd_browser/resources/page-list.ui
--rw-rw-r--   0 jk        (1000) jk        (1000)     4751 2020-11-01 23:27:45.000000 browse-ocrd-0.5.4/ocrd_browser/resources/save-dialog.ui
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-02-20 23:27:36.590905 browse-ocrd-0.5.4/ocrd_browser/ui/
--rw-rw-r--   0 jk        (1000) jk        (1000)      324 2021-05-25 13:59:19.000000 browse-ocrd-0.5.4/ocrd_browser/ui/__init__.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     2928 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/ui/dialogs.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     3370 2021-11-08 13:00:43.000000 browse-ocrd-0.5.4/ocrd_browser/ui/icon_store.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     4539 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/ui/page_browser.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     7161 2022-10-23 21:47:29.000000 browse-ocrd-0.5.4/ocrd_browser/ui/page_store.py
--rw-rw-r--   0 jk        (1000) jk        (1000)    10137 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/ui/window.py
--rw-rw-r--   0 jk        (1000) jk        (1000)    26787 2023-02-20 22:52:19.000000 browse-ocrd-0.5.4/ocrd_browser/ui.gresource
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-02-20 23:27:36.590905 browse-ocrd-0.5.4/ocrd_browser/util/
--rw-rw-r--   0 jk        (1000) jk        (1000)       48 2021-07-22 11:30:21.000000 browse-ocrd-0.5.4/ocrd_browser/util/__init__.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     3607 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/util/config.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     2149 2023-02-20 22:01:29.000000 browse-ocrd-0.5.4/ocrd_browser/util/file_groups.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     3898 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/util/gtk.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     5149 2022-10-22 10:12:29.000000 browse-ocrd-0.5.4/ocrd_browser/util/image.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     2838 2022-10-23 12:10:49.000000 browse-ocrd-0.5.4/ocrd_browser/util/launcher.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     1855 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/util/streams.py
-drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-02-20 23:27:36.590905 browse-ocrd-0.5.4/ocrd_browser/view/
--rw-rw-r--   0 jk        (1000) jk        (1000)      374 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/view/__init__.py
--rw-rw-r--   0 jk        (1000) jk        (1000)    13739 2023-02-20 22:52:04.000000 browse-ocrd-0.5.4/ocrd_browser/view/base.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     7588 2023-02-20 22:01:29.000000 browse-ocrd-0.5.4/ocrd_browser/view/diff.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     1286 2020-11-11 15:29:57.000000 browse-ocrd-0.5.4/ocrd_browser/view/empty.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     1462 2023-02-20 22:01:29.000000 browse-ocrd-0.5.4/ocrd_browser/view/html.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     8689 2023-02-20 22:01:29.000000 browse-ocrd-0.5.4/ocrd_browser/view/images.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     4901 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/ocrd_browser/view/manager.py
--rw-rw-r--   0 jk        (1000) jk        (1000)    26906 2023-02-20 22:01:29.000000 browse-ocrd-0.5.4/ocrd_browser/view/page.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     1121 2022-10-25 17:58:38.000000 browse-ocrd-0.5.4/ocrd_browser/view/registry.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     4378 2023-02-20 22:01:29.000000 browse-ocrd-0.5.4/ocrd_browser/view/text.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     3899 2023-02-20 22:01:29.000000 browse-ocrd-0.5.4/ocrd_browser/view/xml.py
--rw-rw-r--   0 jk        (1000) jk        (1000)      195 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/pyproject.toml
--rw-rw-r--   0 jk        (1000) jk        (1000)      196 2023-02-20 22:01:29.000000 browse-ocrd-0.5.4/requirements.txt
--rw-rw-r--   0 jk        (1000) jk        (1000)     5135 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/serve.py
--rw-rw-r--   0 jk        (1000) jk        (1000)     2165 2023-02-20 23:27:36.590905 browse-ocrd-0.5.4/setup.cfg
--rw-rw-r--   0 jk        (1000) jk        (1000)      191 2022-08-01 12:08:36.000000 browse-ocrd-0.5.4/setup.py
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-04-27 21:03:03.068245 browse-ocrd-0.5.5/
+-rw-rw-r--   0 jk        (1000) jk        (1000)     1061 2020-07-21 10:23:15.000000 browse-ocrd-0.5.5/LICENSE
+-rw-rw-r--   0 jk        (1000) jk        (1000)      104 2022-08-01 12:08:36.000000 browse-ocrd-0.5.5/MANIFEST.in
+-rw-rw-r--   0 jk        (1000) jk        (1000)     7300 2023-04-27 21:03:03.068245 browse-ocrd-0.5.5/PKG-INFO
+-rw-rw-r--   0 jk        (1000) jk        (1000)     6267 2023-03-13 19:04:16.000000 browse-ocrd-0.5.5/README.md
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-04-27 21:03:03.060244 browse-ocrd-0.5.5/browse_ocrd.egg-info/
+-rw-rw-r--   0 jk        (1000) jk        (1000)     7300 2023-04-27 21:03:03.000000 browse-ocrd-0.5.5/browse_ocrd.egg-info/PKG-INFO
+-rw-rw-r--   0 jk        (1000) jk        (1000)     1441 2023-04-27 21:03:03.000000 browse-ocrd-0.5.5/browse_ocrd.egg-info/SOURCES.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)        1 2023-04-27 21:03:03.000000 browse-ocrd-0.5.5/browse_ocrd.egg-info/dependency_links.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)      282 2023-04-27 21:03:03.000000 browse-ocrd-0.5.5/browse_ocrd.egg-info/entry_points.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)      211 2023-04-27 21:03:03.000000 browse-ocrd-0.5.5/browse_ocrd.egg-info/requires.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)       13 2023-04-27 21:03:03.000000 browse-ocrd-0.5.5/browse_ocrd.egg-info/top_level.txt
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-04-27 21:03:03.060244 browse-ocrd-0.5.5/ocrd_browser/
+-rw-rw-r--   0 jk        (1000) jk        (1000)       22 2023-04-27 20:58:02.000000 browse-ocrd-0.5.5/ocrd_browser/__init__.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     6447 2023-04-05 12:40:25.000000 browse-ocrd-0.5.5/ocrd_browser/application.py
+-rwxrwxr-x   0 jk        (1000) jk        (1000)     1813 2022-08-01 12:08:36.000000 browse-ocrd-0.5.5/ocrd_browser/main.py
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-04-27 21:03:03.064244 browse-ocrd-0.5.5/ocrd_browser/model/
+-rw-rw-r--   0 jk        (1000) jk        (1000)      248 2022-08-01 12:08:36.000000 browse-ocrd-0.5.5/ocrd_browser/model/__init__.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)    19031 2023-03-13 16:00:35.000000 browse-ocrd-0.5.5/ocrd_browser/model/document.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     5917 2023-02-20 22:01:29.000000 browse-ocrd-0.5.5/ocrd_browser/model/page.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)    21734 2022-08-01 12:08:36.000000 browse-ocrd-0.5.5/ocrd_browser/model/page_xml_renderer.py
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-04-27 21:03:03.064244 browse-ocrd-0.5.5/ocrd_browser/resources/
+-rw-rw-r--   0 jk        (1000) jk        (1000)        0 2020-07-27 18:20:55.000000 browse-ocrd-0.5.5/ocrd_browser/resources/__init__.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     2315 2020-08-12 08:30:42.000000 browse-ocrd-0.5.5/ocrd_browser/resources/about-dialog.ui
+-rw-rw-r--   0 jk        (1000) jk        (1000)    20131 2023-04-03 16:27:05.000000 browse-ocrd-0.5.5/ocrd_browser/resources/main-window.ui
+-rw-rw-r--   0 jk        (1000) jk        (1000)     4460 2020-08-12 08:31:07.000000 browse-ocrd-0.5.5/ocrd_browser/resources/open-dialog.ui
+-rw-rw-r--   0 jk        (1000) jk        (1000)      852 2020-08-07 10:41:47.000000 browse-ocrd-0.5.5/ocrd_browser/resources/page-list.ui
+-rw-rw-r--   0 jk        (1000) jk        (1000)     4751 2020-11-01 23:27:45.000000 browse-ocrd-0.5.5/ocrd_browser/resources/save-dialog.ui
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-04-27 21:03:03.064244 browse-ocrd-0.5.5/ocrd_browser/ui/
+-rw-rw-r--   0 jk        (1000) jk        (1000)      352 2023-03-02 19:37:47.000000 browse-ocrd-0.5.5/ocrd_browser/ui/__init__.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     2928 2022-08-01 12:08:36.000000 browse-ocrd-0.5.5/ocrd_browser/ui/dialogs.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     3370 2023-03-02 19:43:13.000000 browse-ocrd-0.5.5/ocrd_browser/ui/icon_store.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     4539 2023-03-02 19:43:13.000000 browse-ocrd-0.5.5/ocrd_browser/ui/page_browser.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     7180 2023-03-13 15:39:17.000000 browse-ocrd-0.5.5/ocrd_browser/ui/page_store.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)    11630 2023-04-05 12:43:08.000000 browse-ocrd-0.5.5/ocrd_browser/ui/window.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)    26787 2023-04-03 16:44:02.000000 browse-ocrd-0.5.5/ocrd_browser/ui.gresource
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-04-27 21:03:03.064244 browse-ocrd-0.5.5/ocrd_browser/util/
+-rw-rw-r--   0 jk        (1000) jk        (1000)       48 2021-07-22 11:30:21.000000 browse-ocrd-0.5.5/ocrd_browser/util/__init__.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     5226 2023-03-13 17:53:38.000000 browse-ocrd-0.5.5/ocrd_browser/util/config.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     2233 2023-03-13 16:04:37.000000 browse-ocrd-0.5.5/ocrd_browser/util/file_groups.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     3910 2023-03-02 19:31:20.000000 browse-ocrd-0.5.5/ocrd_browser/util/gtk.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     5149 2022-10-22 10:12:29.000000 browse-ocrd-0.5.5/ocrd_browser/util/image.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     2889 2023-03-13 16:13:18.000000 browse-ocrd-0.5.5/ocrd_browser/util/launcher.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     1855 2022-08-01 12:08:36.000000 browse-ocrd-0.5.5/ocrd_browser/util/streams.py
+drwxrwxr-x   0 jk        (1000) jk        (1000)        0 2023-04-27 21:03:03.068245 browse-ocrd-0.5.5/ocrd_browser/view/
+-rw-rw-r--   0 jk        (1000) jk        (1000)      374 2022-08-01 12:08:36.000000 browse-ocrd-0.5.5/ocrd_browser/view/__init__.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)    13761 2023-03-13 15:41:48.000000 browse-ocrd-0.5.5/ocrd_browser/view/base.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     7588 2023-02-20 22:01:29.000000 browse-ocrd-0.5.5/ocrd_browser/view/diff.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     1286 2020-11-11 15:29:57.000000 browse-ocrd-0.5.5/ocrd_browser/view/empty.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     1462 2023-02-20 22:01:29.000000 browse-ocrd-0.5.5/ocrd_browser/view/html.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     8689 2023-02-20 22:01:29.000000 browse-ocrd-0.5.5/ocrd_browser/view/images.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     4901 2023-04-05 12:04:19.000000 browse-ocrd-0.5.5/ocrd_browser/view/manager.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)    26906 2023-02-20 22:01:29.000000 browse-ocrd-0.5.5/ocrd_browser/view/page.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     1121 2022-10-25 17:58:38.000000 browse-ocrd-0.5.5/ocrd_browser/view/registry.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     4378 2023-02-20 22:01:29.000000 browse-ocrd-0.5.5/ocrd_browser/view/text.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     3899 2023-03-13 17:46:19.000000 browse-ocrd-0.5.5/ocrd_browser/view/xml.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)      195 2022-08-01 12:08:36.000000 browse-ocrd-0.5.5/pyproject.toml
+-rw-rw-r--   0 jk        (1000) jk        (1000)      213 2023-03-13 15:37:44.000000 browse-ocrd-0.5.5/requirements.txt
+-rw-rw-r--   0 jk        (1000) jk        (1000)     5135 2022-08-01 12:08:36.000000 browse-ocrd-0.5.5/serve.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     2165 2023-04-27 21:03:03.068245 browse-ocrd-0.5.5/setup.cfg
+-rw-rw-r--   0 jk        (1000) jk        (1000)      191 2022-08-01 12:08:36.000000 browse-ocrd-0.5.5/setup.py
+-rw-rw-r--   0 jk        (1000) jk        (1000)     3792 2023-03-13 14:55:34.000000 browse-ocrd-0.5.5/test_conf.py
```

### Comparing `browse-ocrd-0.5.4/LICENSE` & `browse-ocrd-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/PKG-INFO` & `browse-ocrd-0.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browse-ocrd
-Version: 0.5.4
+Version: 0.5.5
 Summary: An extensible viewer for OCR-D workspaces
 Home-page: https://github.com/hnesk/browse-ocrd
 Author: Johannes Künsebeck
 Author-email: kuensebeck@googlemail.com
 License: MIT License
 Keywords: OCR,OCR-D,mets,PAGE Xml
 Classifier: Programming Language :: Python :: 3
@@ -141,27 +141,40 @@
 GLib.get_system_config_dirs()  # '/etc/xdg/xdg-ubuntu/ocrd-browser.conf', '/etc/xdg/ocrd-browser.conf'
 GLib.get_user_config_dir()     # '/home/jk/.config/ocrd-browser.conf'  
 os.getcwd()                    # './ocrd-browser.conf'
 ```
 
 ### Configuration file syntax
 
-The `ocrd-browser.conf` file is an ini-file with the following keys:
+The `ocrd-browser.conf` file is an ini-file with the following sections and keys:
 ```ini
 [FileGroups]
 # Preferred fileGrp names for thumbnail display in the Page Browser 
 # Comma separated list of regular expressions
 preferredImages = OCR-D-IMG, OCR-D-IMG.*, ORIGINAL
 
 # Each Tool has a section header [Tool XYZ]
 # At the moment the only defined tool is "PageViewer"  
 [Tool PageViewer]
 # shell commandline to execute with placeholders  
 commandline = /usr/bin/java -jar /home/jk/bin/JPageViewer/JPageViewer.jar --resolve-dir {workspace.directory} {file.path.absolute}
 ```
 
+> Note: You can get PRImA's PageViewer at [Github](https://github.com/PRImA-Research-Lab/prima-page-viewer/releases).
+
+
 The `commandline` string will be used as a python format string with the keyword arguments:
 
 * `workspace` : The current `ocrd.Workspace`, all properties get shell escaped (by `shlex.quote`) automatically.
 * `file` : The current `ocrd_models.OcrdFile`, all properties get shell escaped (by `shlex.quote`) automatically, also there is an additional property `path` with the properties `absolute` and `relative`, so `{file.path.absolute}` will be replaced by the shell quoted absolute path of the file. 
 
-> Note: You can get PRImA's PageViewer at [Github](https://github.com/PRImA-Research-Lab/prima-page-viewer/releases).
+### Configuration by environment variables
+
+It is possible to set or override values of the configuration through environment variables. The environment variables follow this structure :  `BROCRD__{SECTION}__{KEY}`, where `SECTION` and `KEY` are in upper snake case and divided by a double underscore (`__`). If the section title contains spaces, the single words are also divided by `__`.  
+
+Some examples:
+```shell
+BROCRD__FILE_GROUPS__PREFERRED_IMAGES='THUMB'  
+BROCRD__TOOL__PAGEVIEWER__COMMANDLINE='ls {file.path.absolute}'  
+
+```
+
```

### Comparing `browse-ocrd-0.5.4/README.md` & `browse-ocrd-0.5.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -115,27 +115,40 @@
 GLib.get_system_config_dirs()  # '/etc/xdg/xdg-ubuntu/ocrd-browser.conf', '/etc/xdg/ocrd-browser.conf'
 GLib.get_user_config_dir()     # '/home/jk/.config/ocrd-browser.conf'  
 os.getcwd()                    # './ocrd-browser.conf'
 ```
 
 ### Configuration file syntax
 
-The `ocrd-browser.conf` file is an ini-file with the following keys:
+The `ocrd-browser.conf` file is an ini-file with the following sections and keys:
 ```ini
 [FileGroups]
 # Preferred fileGrp names for thumbnail display in the Page Browser 
 # Comma separated list of regular expressions
 preferredImages = OCR-D-IMG, OCR-D-IMG.*, ORIGINAL
 
 # Each Tool has a section header [Tool XYZ]
 # At the moment the only defined tool is "PageViewer"  
 [Tool PageViewer]
 # shell commandline to execute with placeholders  
 commandline = /usr/bin/java -jar /home/jk/bin/JPageViewer/JPageViewer.jar --resolve-dir {workspace.directory} {file.path.absolute}
 ```
 
+> Note: You can get PRImA's PageViewer at [Github](https://github.com/PRImA-Research-Lab/prima-page-viewer/releases).
+
+
 The `commandline` string will be used as a python format string with the keyword arguments:
 
 * `workspace` : The current `ocrd.Workspace`, all properties get shell escaped (by `shlex.quote`) automatically.
 * `file` : The current `ocrd_models.OcrdFile`, all properties get shell escaped (by `shlex.quote`) automatically, also there is an additional property `path` with the properties `absolute` and `relative`, so `{file.path.absolute}` will be replaced by the shell quoted absolute path of the file. 
 
-> Note: You can get PRImA's PageViewer at [Github](https://github.com/PRImA-Research-Lab/prima-page-viewer/releases).
+### Configuration by environment variables
+
+It is possible to set or override values of the configuration through environment variables. The environment variables follow this structure :  `BROCRD__{SECTION}__{KEY}`, where `SECTION` and `KEY` are in upper snake case and divided by a double underscore (`__`). If the section title contains spaces, the single words are also divided by `__`.  
+
+Some examples:
+```shell
+BROCRD__FILE_GROUPS__PREFERRED_IMAGES='THUMB'  
+BROCRD__TOOL__PAGEVIEWER__COMMANDLINE='ls {file.path.absolute}'  
+
+```
+
```

### Comparing `browse-ocrd-0.5.4/browse_ocrd.egg-info/PKG-INFO` & `browse-ocrd-0.5.5/browse_ocrd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browse-ocrd
-Version: 0.5.4
+Version: 0.5.5
 Summary: An extensible viewer for OCR-D workspaces
 Home-page: https://github.com/hnesk/browse-ocrd
 Author: Johannes Künsebeck
 Author-email: kuensebeck@googlemail.com
 License: MIT License
 Keywords: OCR,OCR-D,mets,PAGE Xml
 Classifier: Programming Language :: Python :: 3
@@ -141,27 +141,40 @@
 GLib.get_system_config_dirs()  # '/etc/xdg/xdg-ubuntu/ocrd-browser.conf', '/etc/xdg/ocrd-browser.conf'
 GLib.get_user_config_dir()     # '/home/jk/.config/ocrd-browser.conf'  
 os.getcwd()                    # './ocrd-browser.conf'
 ```
 
 ### Configuration file syntax
 
-The `ocrd-browser.conf` file is an ini-file with the following keys:
+The `ocrd-browser.conf` file is an ini-file with the following sections and keys:
 ```ini
 [FileGroups]
 # Preferred fileGrp names for thumbnail display in the Page Browser 
 # Comma separated list of regular expressions
 preferredImages = OCR-D-IMG, OCR-D-IMG.*, ORIGINAL
 
 # Each Tool has a section header [Tool XYZ]
 # At the moment the only defined tool is "PageViewer"  
 [Tool PageViewer]
 # shell commandline to execute with placeholders  
 commandline = /usr/bin/java -jar /home/jk/bin/JPageViewer/JPageViewer.jar --resolve-dir {workspace.directory} {file.path.absolute}
 ```
 
+> Note: You can get PRImA's PageViewer at [Github](https://github.com/PRImA-Research-Lab/prima-page-viewer/releases).
+
+
 The `commandline` string will be used as a python format string with the keyword arguments:
 
 * `workspace` : The current `ocrd.Workspace`, all properties get shell escaped (by `shlex.quote`) automatically.
 * `file` : The current `ocrd_models.OcrdFile`, all properties get shell escaped (by `shlex.quote`) automatically, also there is an additional property `path` with the properties `absolute` and `relative`, so `{file.path.absolute}` will be replaced by the shell quoted absolute path of the file. 
 
-> Note: You can get PRImA's PageViewer at [Github](https://github.com/PRImA-Research-Lab/prima-page-viewer/releases).
+### Configuration by environment variables
+
+It is possible to set or override values of the configuration through environment variables. The environment variables follow this structure :  `BROCRD__{SECTION}__{KEY}`, where `SECTION` and `KEY` are in upper snake case and divided by a double underscore (`__`). If the section title contains spaces, the single words are also divided by `__`.  
+
+Some examples:
+```shell
+BROCRD__FILE_GROUPS__PREFERRED_IMAGES='THUMB'  
+BROCRD__TOOL__PAGEVIEWER__COMMANDLINE='ls {file.path.absolute}'  
+
+```
+
```

### Comparing `browse-ocrd-0.5.4/browse_ocrd.egg-info/SOURCES.txt` & `browse-ocrd-0.5.5/browse_ocrd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 serve.py
 setup.cfg
 setup.py
+test_conf.py
 browse_ocrd.egg-info/PKG-INFO
 browse_ocrd.egg-info/SOURCES.txt
 browse_ocrd.egg-info/dependency_links.txt
 browse_ocrd.egg-info/entry_points.txt
 browse_ocrd.egg-info/requires.txt
 browse_ocrd.egg-info/top_level.txt
 ocrd_browser/__init__.py
```

### Comparing `browse-ocrd-0.5.4/ocrd_browser/application.py` & `browse-ocrd-0.5.5/ocrd_browser/application.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from gi.repository import Gio, Gtk, GLib, Gdk
 
-from typing import List
+from typing import List, Dict, Any
 
+from ocrd_browser import __version__
 from ocrd_browser.util.gtk import ActionRegistry
-from ocrd_browser.ui import MainWindow, AboutDialog, OpenDialog
+from ocrd_browser.ui import MainWindow, WindowFlags, AboutDialog, OpenDialog
 from ocrd_browser.view import ViewRegistry
 
 from importlib_metadata import entry_points
 
 
 class OcrdBrowserApplication(Gtk.Application):
     # TODO: Parse arguments (with Gtk or click) to open certain views by mets+page_id+view(view_configuration_dict) and deep filename e.g.
@@ -20,26 +21,35 @@
     # TODO: Test application startup for all kinds of mets.xml (not necessarily OCR-D mets.xml) and views without crashes
     def __init__(self) -> None:
         Gtk.Application.__init__(self, application_id='org.readmachine.ocrd-browser',
                                  flags=Gio.ApplicationFlags.HANDLES_OPEN)
         self.actions = ActionRegistry(for_widget=self)
         self.view_registry = ViewRegistry.create_from_entry_points()
 
+        self.window_flags = WindowFlags.NONE
+        self.restricted = False
+
+        self.add_main_option("version", ord("v"), GLib.OptionFlags.NONE, GLib.OptionArg.NONE, "Show version and exit", None)
+        self.add_main_option("maximize", ord("m"), GLib.OptionFlags.NONE, GLib.OptionArg.NONE, "Open in maximized window", None)
+        self.add_main_option("fullscreen", ord("f"), GLib.OptionFlags.NONE, GLib.OptionArg.NONE, "Open in fullscreen window", None)
+        self.add_main_option("restricted", ord("r"), GLib.OptionFlags.NONE, GLib.OptionArg.NONE, "Open restricted (no edit/open functionality)", None)
+
     def do_startup(self) -> None:
         Gtk.Application.do_startup(self)
         self.actions.create('new')
         self.actions.create('open')
         self.actions.create('about')
         self.actions.create('quit')
 
         self.set_accels_for_action('view.zoom_by(1)', ['<Ctrl>plus'])
         self.set_accels_for_action('view.zoom_by(-1)', ['<Ctrl>minus'])
         self.set_accels_for_action('view.zoom_to::original', ['<Ctrl>0'])
         self.set_accels_for_action('view.zoom_to::width', ['<Ctrl>numbersign'])
         self.set_accels_for_action('view.zoom_to::page', ['<Ctrl><Alt>numbersign'])
+        self.set_accels_for_action("win.fullscreen", ['F11'])
 
         for entry_point in entry_points(group='ocrd_browser_ext'):
             (entry_point.load())(self)
 
         self.load_css()
 
     def load_css(self) -> None:
@@ -48,19 +58,15 @@
         # noinspection PyArgumentList
         Gtk.StyleContext().add_provider_for_screen(Gdk.Screen.get_default(), css, Gtk.STYLE_PROVIDER_PRIORITY_USER)
         # css = Gtk.CssProvider()
         # css.load_from_path('/home/jk/PycharmProjects/ocrd-browser/gresources/css/test.css')
         # Gtk.StyleContext().add_provider_for_screen(Gdk.Screen.get_default(), css, Gtk.STYLE_PROVIDER_PRIORITY_USER)
 
     def do_activate(self) -> None:
-
-        win = self.get_active_window()
-        if not win:
-            win = MainWindow(application=self)
-        win.present()
+        self._present_window(self.get_active_window())
 
     def on_about(self, _action: Gio.SimpleAction, _param: str = None) -> None:
         about_dialog = AboutDialog(application=self, transient_for=self.get_active_window(), modal=True)
         about_dialog.present()
 
     def on_quit(self, _action: Gio.SimpleAction, _param: str = None) -> None:
         open_windows: int = 0
@@ -77,20 +83,43 @@
         open_dialog = OpenDialog(application=self, transient_for=self.get_active_window(), modal=True)
         response = open_dialog.run()
         if response == Gtk.ResponseType.OK:
             self.open_in_window(open_dialog.get_uri(), window=open_dialog.get_transient_for())
         open_dialog.destroy()
 
     def on_new(self, _action: Gio.SimpleAction, _param: str = None) -> None:
-        win = MainWindow(application=self)
+        win = MainWindow(application=self, restricted=self.restricted)
         win.present()
 
     def do_open(self, files: List[Gio.File], file_count: int, hint: str) -> int:
         for file in files:
             self.open_in_window(file.get_uri(), window=None)
         return 0
 
+    def do_handle_local_options(self, goptions: GLib.VariantDict) -> int:
+        options: Dict[str, Any] = goptions.end().unpack()
+        if options.get('version', False):
+            print('browse-ocrd: {}'.format(__version__))
+            return 0
+        if options.get('maximize', False):
+            self.window_flags |= WindowFlags.MAXIMIZE
+        if options.get('fullscreen', False):
+            self.window_flags |= WindowFlags.FULLSCREEN
+        self.restricted = options.get('restricted', False)
+
+        return -1
+
     def open_in_window(self, uri: str, window: MainWindow = None) -> None:
         if not window or not window.document.empty:
-            window = MainWindow(application=self)
-        window.present()
+            window = MainWindow(application=self, restricted=self.restricted)
+        self._present_window(window)
         GLib.timeout_add(10, window.open, uri)
+
+    def _present_window(self, win: MainWindow) -> None:
+        if not win:
+            win = MainWindow(application=self, restricted=self.restricted)
+        if self.window_flags & WindowFlags.MAXIMIZE:
+            win.maximize()
+        if self.window_flags & WindowFlags.FULLSCREEN:
+            win.fullscreen()
+
+        win.present()
```

### Comparing `browse-ocrd-0.5.4/ocrd_browser/main.py` & `browse-ocrd-0.5.5/ocrd_browser/main.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/model/document.py` & `browse-ocrd-0.5.5/ocrd_browser/model/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 import shutil
 from functools import wraps
 
 from ocrd import Resolver
 from ocrd_browser.model.page import Page
-from ocrd_browser.util.file_groups import best_file_group, FileGroupHandle
+from ocrd_browser.util.file_groups import best_file_group, FileGroupHandle, PatternList
 from ocrd_browser.util.image import add_dpi_to_png_buffer
 from ocrd_browser.util.streams import SilencedStreams
 from ocrd_modelfactory import page_from_file
 from ocrd_models.constants import NAMESPACES as NS
 from ocrd_models import OcrdFile
 from ocrd_utils import pushd_popd
 from ocrd_utils.constants import MIME_TO_EXT
@@ -260,15 +260,15 @@
             if len(images) > 0:
                 image_paths[page_id] = self.directory.joinpath(images[0].local_filename)
             else:
                 log.warning('Found no images for PAGE %s and fileGrp %s', page_id, file_group)
                 image_paths[page_id] = None
         return image_paths
 
-    def get_default_image_group(self, preferred_image_file_groups: Optional[List[str]] = None) -> Optional[FileGroupHandle]:
+    def get_default_image_group(self, preferred_image_file_groups: PatternList = None) -> Optional[FileGroupHandle]:
         return best_file_group(self.file_groups, preferred_image_file_groups, [r'image/.*'], cutoff=0)
 
     def get_unused_page_id(self, template_page_id: str = 'PAGE_{page_nr}') -> Tuple[str, int]:
         """
         Finds a page_nr that yields an unused page_id for the workspace and returns page_id, page_nr
 
         @param template_page_id: str
```

### Comparing `browse-ocrd-0.5.4/ocrd_browser/model/page.py` & `browse-ocrd-0.5.5/ocrd_browser/model/page.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/model/page_xml_renderer.py` & `browse-ocrd-0.5.5/ocrd_browser/model/page_xml_renderer.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/resources/about-dialog.ui` & `browse-ocrd-0.5.5/ocrd_browser/resources/about-dialog.ui`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/resources/main-window.ui` & `browse-ocrd-0.5.5/ocrd_browser/resources/main-window.ui`

 * *Files 0% similar despite different names*

#### Comparing `browse-ocrd-0.5.4/ocrd_browser/resources/main-window.ui` & `browse-ocrd-0.5.5/ocrd_browser/resources/main-window.ui`

```diff
@@ -319,15 +319,15 @@
       </object>
     </child>
   </template>
   <object class="GtkPopoverMenu" id="main_menu">
     <property name="can_focus">False</property>
     <property name="relative_to">main_menu_button</property>
     <child>
-      <object class="GtkBox">
+      <object class="GtkBox" id="main_menu_box">
         <property name="visible">True</property>
         <property name="can_focus">False</property>
         <property name="border_width">4</property>
         <property name="orientation">vertical</property>
         <property name="spacing">2</property>
         <child>
           <object class="GtkModelButton">
```

### Comparing `browse-ocrd-0.5.4/ocrd_browser/resources/open-dialog.ui` & `browse-ocrd-0.5.5/ocrd_browser/resources/open-dialog.ui`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/resources/page-list.ui` & `browse-ocrd-0.5.5/ocrd_browser/resources/page-list.ui`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/resources/save-dialog.ui` & `browse-ocrd-0.5.5/ocrd_browser/resources/save-dialog.ui`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/ui/dialogs.py` & `browse-ocrd-0.5.5/ocrd_browser/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/ui/icon_store.py` & `browse-ocrd-0.5.5/ocrd_browser/ui/icon_store.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/ui/page_browser.py` & `browse-ocrd-0.5.5/ocrd_browser/ui/page_browser.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/ui/page_store.py` & `browse-ocrd-0.5.5/ocrd_browser/ui/page_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Tuple, Optional, Dict, List, Union, NewType, Callable, Any
 from itertools import count
 
 from ocrd_browser.util.image import cv_to_pixbuf, cv_scale
 from ocrd_browser.model import Document
 from .icon_store import LazyLoadingListStore
-from ..util.config import Settings
+from ..util.config import SettingsFactory
 
 import cv2
 import os
 
 RowResult = Tuple[Optional[int], Optional[Gtk.TreeModelRow]]
 ChangeList = Union[List[str], Dict[str, str]]
 Column = NewType('Column', int)
@@ -49,15 +49,15 @@
         self.pixbufs: Dict[str, GdkPixbuf.Pixbuf] = {
             icon_name: GdkPixbuf.Pixbuf.new_from_resource(
                 '/org/readmachine/ocrd-browser/icons/{}.png'.format(icon_name)
             ) for icon_name in ['page-loading', 'page-missing']
         }
 
         # TODO: make file_group selectable, see https://github.com/hnesk/browse-ocrd/issues/7#issuecomment-707851109
-        self.file_group = document.get_default_image_group(Settings.get().file_groups.preferred_images)
+        self.file_group = document.get_default_image_group(SettingsFactory.settings().file_groups.preferred_images)
         file_lookup = document.get_image_paths(self.file_group)
         order = count(start=1)
         for page_id in self.document.page_ids:
             file = file_lookup[page_id]
             self.append((page_id, '', str(file) if file else None, None, next(order)))
 
         GLib.timeout_add(10, self.start_loading)
```

### Comparing `browse-ocrd-0.5.4/ocrd_browser/ui/window.py` & `browse-ocrd-0.5.5/ocrd_browser/ui/window.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,105 @@
 from gi.repository import Gtk, GdkPixbuf, Gio, GObject, GLib, Gdk
+from enum import Flag, auto
+
 from ocrd_models import OcrdFile
 
 from ocrd_browser.model import Document
 from ocrd_browser.view import ViewRegistry, ViewPage
 from ocrd_browser.util.gtk import ActionRegistry, resource_string
 from .dialogs import SaveDialog, SaveChangesDialog
 from .page_browser import PagePreviewList
 from typing import List, cast, Any, Optional
 
 from ..view.manager import ViewManager
 
 
+EDIT_ACTIONS = ['app.new', 'win.toggle_edit_mode', 'win.page_remove', 'win.save_as', 'win.save']
+
+
+class WindowFlags(Flag):
+    NONE = 0
+    FULLSCREEN = auto()
+    MAXIMIZE = auto()
+
+
 @Gtk.Template(string=resource_string('main-window.ui'))
 class MainWindow(Gtk.ApplicationWindow):
     __gtype_name__ = "MainWindow"
 
     header_bar: Gtk.HeaderBar = Gtk.Template.Child()
     page_list_scroller: Gtk.ScrolledWindow = Gtk.Template.Child()
     current_page_label: Gtk.Label = Gtk.Template.Child()
     view_container: Gtk.Box = Gtk.Template.Child()
     view_menu_box: Gtk.Box = Gtk.Template.Child()
+    open_button_box: Gtk.ButtonBox = Gtk.Template.Child()
+    main_menu_box: Gtk.Box = Gtk.Template.Child()
 
-    def __init__(self, **kwargs: Any):
+    def __init__(self, restricted: bool = False, **kwargs: Any):
         Gtk.ApplicationWindow.__init__(self, **kwargs)
         # noinspection PyCallByClass,PyArgumentList
         self.set_icon(GdkPixbuf.Pixbuf.new_from_resource("/org/readmachine/ocrd-browser/icons/icon.png"))
         self.view_manager = ViewManager(self, self.view_container)
         self.current_page_id: Optional[str] = None
-        # noinspection PyTypeChecker
         self.document = Document.create(emitter=self.emit)
-
+        self._restricted = False
         self.actions = ActionRegistry(for_widget=self)
         self.actions.create('close')
         self.actions.create('goto_first')
         self.actions.create('go_back')
         self.actions.create('go_forward')
         self.actions.create('goto_last')
-        self.actions.create('page_remove')
         self.actions.create('page_properties')
         self.actions.create('close_view', param_type=GLib.VariantType("s"))
         self.actions.create('split_view', param_type=GLib.VariantType("(ssb)"))
         self.actions.create('create_view', param_type=GLib.VariantType("s"))
         self.actions.create('replace_view', param_type=GLib.VariantType("(ss)"))
-        self.actions.create('toggle_edit_mode', state=GLib.Variant('b', False))
+        self.actions.create('fullscreen', state=GLib.Variant.new_boolean(self.get_application().window_flags & WindowFlags.FULLSCREEN))
+        self.actions.create('toggle_edit_mode', state=GLib.Variant.new_boolean(False))
         self.actions.create('save')
         self.actions.create('save_as')
+        self.actions.create('page_remove')
 
         self.connect('delete-event', self.on_delete_event)
 
         self.page_list = PagePreviewList(self.document)
         self.page_list_scroller.add(self.page_list)
         self.page_list.connect('page_activated', self.on_page_activated)
         self.page_list.connect('pages_selected', self.on_pages_selected)
 
         for id_, view in self.view_registry.get_view_options().items():
             menu_item = Gtk.ModelButton(visible=True, centered=False, halign=Gtk.Align.FILL, label=view, hexpand=True)
             menu_item.set_detailed_action_name('win.create_view("{}")'.format(id_))
             self.view_menu_box.pack_start(menu_item, True, True, 0)
 
         self.view_manager.set_root_view(ViewPage)
-        # self.view_manager.split(None, ViewPage, False)
+        self.restricted = restricted
 
         self.update_ui()
 
+    @property
+    def restricted(self) -> bool:
+        return self._restricted
+
+    @restricted.setter
+    def restricted(self, restricted: bool) -> None:
+        for action in EDIT_ACTIONS:
+            if action.startswith('win.'):
+                self.actions[action[4:]].set_enabled(not restricted)
+            elif action.startswith('app.'):
+                self.get_application().actions[action[4:]].set_enabled(not restricted)
+
+        for item in self.main_menu_box.get_children():
+            if isinstance(item, Gtk.ModelButton):
+                if item.get_action_name() in EDIT_ACTIONS:
+                    item.set_visible(not restricted)
+
+        self.open_button_box.set_visible(not restricted)
+        self._restricted = restricted
+
     def on_page_remove(self, _a: Gio.SimpleAction, _p: None) -> None:
         for page_id in self.page_list.get_selected_ids():
             self.document.delete_page(page_id)
 
     def on_page_properties(self, _a: Gio.SimpleAction, _p: None) -> None:
         pass
 
@@ -144,18 +177,19 @@
             can_go_back = index > 0
             can_go_forward = index < last_page
 
         self.actions['goto_first'].set_enabled(can_go_back)
         self.actions['go_back'].set_enabled(can_go_back)
         self.actions['go_forward'].set_enabled(can_go_forward)
         self.actions['goto_last'].set_enabled(can_go_forward)
-        self.actions['page_remove'].set_enabled(self.document.editable)
-        # noinspection PyCallByClass,PyArgumentList
-        self.actions['toggle_edit_mode'].set_state(GLib.Variant.new_boolean(self.document.editable))
-        self.actions['save'].set_enabled(self.document.modified)
+        if not self.restricted:
+            self.actions['page_remove'].set_enabled(self.document.editable)
+            # noinspection PyCallByClass,PyArgumentList
+            self.actions['toggle_edit_mode'].set_state(GLib.Variant.new_boolean(self.document.editable))
+            self.actions['save'].set_enabled(self.document.modified)
         self.view_manager.update_ui()
 
     def close_confirm(self) -> bool:
         if self.document.modified:
             # Do you wanna save the changes?
             d = SaveChangesDialog(document=self.document, transient_for=self, modal=True)
             save_changes = d.run()
@@ -200,15 +234,15 @@
         self.view_manager.replace(replace_view, new_view_type)
 
     def on_close_view(self, _action: Gio.SimpleAction, view_name: GLib.Variant) -> None:
         try:
             self.view_manager.close(view_name.get_string())
         except ValueError:
             # Tried to remove last view
-            pass
+            self.on_close()
 
     def on_split_view(self, _action: Gio.SimpleAction, arguments: GLib.Variant) -> None:
         (split_view, new_view_name, horizontal) = arguments
         new_view_type = self.view_registry.get_view(new_view_name)
         self.view_manager.split(split_view, new_view_type, horizontal)
 
     def on_save(self, _a: Gio.SimpleAction = None, _p: None = None) -> bool:
@@ -238,7 +272,14 @@
         save_dialog.destroy()
         self.update_ui()
         return should_save
 
     def on_toggle_edit_mode(self, _a: Gio.SimpleAction = None, _p: None = None) -> None:
         self.document.editable = not self.document.editable
         self.update_ui()
+
+    def on_fullscreen(self, action: Gio.Action, value: GLib.Variant) -> None:
+        action.set_state(value)
+        if value.get_boolean():
+            self.fullscreen()
+        else:
+            self.unfullscreen()
```

### Comparing `browse-ocrd-0.5.4/ocrd_browser/ui.gresource` & `browse-ocrd-0.5.5/ocrd_browser/ui.gresource`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/util/file_groups.py` & `browse-ocrd-0.5.5/ocrd_browser/util/file_groups.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 import re
 from collections import Counter
-from typing import List, Optional, Counter as CounterType, NamedTuple, cast, Tuple, Union
+from typing import List, Optional, Counter as CounterType, NamedTuple, cast, Tuple, Union, Pattern, Sequence, Any
 
 from ocrd_models import OcrdFile
 
+AnyPattern = Union[Pattern[Any], str]
+PatternList = Optional[Sequence[AnyPattern]]
+
 
 class FileGroupHandle(NamedTuple):
     group: str
     mime: str
 
     @property
     def key(self) -> str:
@@ -24,30 +27,30 @@
     def cast(cls, tpl: Union[FileGroupHandle, Tuple[str, str]]) -> FileGroupHandle:
         if isinstance(tpl, cls):
             return tpl
         else:
             return cls._make(tpl)
 
 
-def weight_match(s: str, preferred: Optional[List[str]] = None) -> float:
+def weight_match(s: str, preferred: PatternList = None) -> float:
     """
     Weights how good a string matches a list of regular expressions
     """
     weight = 0.0
     if preferred:
         ln = float(len(preferred))
         for i, pref in enumerate(preferred):
             if re.fullmatch(pref, s):
                 # prefer matches earlier in the list
                 weight += (ln - i) / ln
                 # break or no break???
     return weight
 
 
-def best_file_group(file_group_handles: List[FileGroupHandle], preferred_groups: Optional[List[str]] = None, preferred_mimetypes: Optional[List[str]] = None, cutoff: float = -9999) -> Optional[FileGroupHandle]:
+def best_file_group(file_group_handles: List[FileGroupHandle], preferred_groups: PatternList = None, preferred_mimetypes: PatternList = None, cutoff: float = -9999) -> Optional[FileGroupHandle]:
     file_groups_counter: CounterType[FileGroupHandle] = Counter()
     for file_group_handle in file_group_handles:
         file_groups_counter[file_group_handle] += weight_match(file_group_handle.group, preferred_groups)  # type: ignore[assignment]
         file_groups_counter[file_group_handle] += weight_match(file_group_handle.mime, preferred_mimetypes)  # type: ignore[assignment]
         file_groups_counter[file_group_handle] -= len(file_group_handle.group) * 0.0001  # type: ignore[assignment]
     if file_groups_counter:
         [(file_group_handle, score)] = file_groups_counter.most_common(1)
```

### Comparing `browse-ocrd-0.5.4/ocrd_browser/util/gtk.py` & `browse-ocrd-0.5.5/ocrd_browser/util/gtk.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.for_widget = for_widget if for_widget else Gio.SimpleActionGroup()
         self.actions: Dict[str, Gio.SimpleAction] = {}
 
     def create(self, name: str, callback: ActionCallback = None,
                param_type: GLib.VariantType = None, state: GLib.Variant = None) -> Gio.SimpleAction:
         callback = callback if callback else getattr(self.for_widget, 'on_' + name)
         action = Gio.SimpleAction(name=name, parameter_type=param_type, state=state)
-        if state:
+        if state is not None:
             action.connect("change-state", callback)
         else:
             action.connect("activate", callback)
         self.for_widget.add_action(action)
         self.actions[name] = action
         return action
```

### Comparing `browse-ocrd-0.5.4/ocrd_browser/util/image.py` & `browse-ocrd-0.5.5/ocrd_browser/util/image.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/util/launcher.py` & `browse-ocrd-0.5.5/ocrd_browser/util/launcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from subprocess import Popen
 from typing import Dict, Optional, Any
 
 from ocrd_models import OcrdFile
 from ocrd_utils import getLogger
 
 from ocrd_browser.model import Document
-from ocrd_browser.util.config import _Tool, Settings
+from ocrd_browser.util.config import Tool, SettingsFactory
 
 
 class ResolvableFileName:
     def __init__(self, filename: str, in_doc: Document):
         self.filename = filename
         self.in_doc = in_doc
 
@@ -47,32 +47,33 @@
         return ResolvableFileName(self.object.local_filename, self.in_doc)
 
     # Recommended alias path, because local_filename sounds like a relative path
     path = local_filename
 
 
 class Launcher:
-    def __init__(self, tools: Optional[Dict[str, _Tool]] = None):
-        self.tools = tools if tools else Settings.get().tools
+    def __init__(self, tools: Optional[Dict[str, Tool]] = None):
+        self.tools = tools if tools else SettingsFactory.settings().tool
 
     def launch(self, toolname: str, doc: Document, file: OcrdFile) -> Optional[Popen]:  # type: ignore[type-arg]
         if toolname in self.tools:
-            return self.launch_tool(self.tools[toolname], doc, file)
+            return self.launch_tool(self.tools[toolname], doc, file, toolname)
         else:
             log = getLogger('ocrd_browser.util.launcher.Launcher.launch')
             log.error(
                 'Tool "%s" not found in your config, to fix place the following section in your ocrd-browser.conf',
                 toolname)
             log.error('[Tool %s]', toolname)
             log.error('commandline = /usr/bin/yourtool --base-dir {workspace.directory} {file.path.absolute}')
             return None
 
-    def launch_tool(self, tool: _Tool, doc: Document, file: OcrdFile, **kwargs: Any) -> Popen:  # type: ignore[type-arg]
+    def launch_tool(self, tool: Tool, doc: Document, file: OcrdFile, toolname: str, **kwargs: Any) -> Popen:  # type: ignore[type-arg]
         log = getLogger('ocrd_browser.util.launcher.Launcher.launch_tool')
         commandline = self._template(tool.commandline, doc, file)
-        log.debug('Calling tool "%s" with commandline: ', tool.name)
+        log.debug('Calling tool "%s" with commandline: ', toolname)
         log.debug('%s', commandline)
         process = Popen(args=commandline, shell=True, cwd=doc.directory, **kwargs)
         return process
 
-    def _template(self, arg: str, doc: Document, file: OcrdFile) -> str:
+    @staticmethod
+    def _template(arg: str, doc: Document, file: OcrdFile) -> str:
         return arg.format(file=FileProxy(file, doc), workspace=QuotingProxy(doc.workspace))
```

### Comparing `browse-ocrd-0.5.4/ocrd_browser/util/streams.py` & `browse-ocrd-0.5.5/ocrd_browser/util/streams.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/view/base.py` & `browse-ocrd-0.5.5/ocrd_browser/view/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
             phs = {'fileGrp': row[self.COLUMN_GROUP], 'ext': row[self.COLUMN_EXT], 'mime': row[self.COLUMN_MIME]}
             tooltip.set_text('fileGrp: {fileGrp} (Mime-Type: {mime})'.format(**phs))
             return True
         return False
 
     def set_document(self, document: 'Document') -> None:
         self.set_model(FileGroupModel.build(document, self.filter))
-        # self.set_active(0)
+        self.set_active(len(self.get_model()) - 1)
 
     def add_renderer(self, column: int, width: int = None) -> Gtk.CellRendererText:
         renderer = Gtk.CellRendererText(ellipsize=Pango.EllipsizeMode.MIDDLE)
         if width:
             renderer.props.width = width
         self.pack_start(renderer, False)
         self.add_attribute(renderer, "text", column)
```

### Comparing `browse-ocrd-0.5.4/ocrd_browser/view/diff.py` & `browse-ocrd-0.5.5/ocrd_browser/view/diff.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/view/empty.py` & `browse-ocrd-0.5.5/ocrd_browser/view/empty.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/view/html.py` & `browse-ocrd-0.5.5/ocrd_browser/view/html.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/view/images.py` & `browse-ocrd-0.5.5/ocrd_browser/view/images.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/view/manager.py` & `browse-ocrd-0.5.5/ocrd_browser/view/manager.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/view/page.py` & `browse-ocrd-0.5.5/ocrd_browser/view/page.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/view/registry.py` & `browse-ocrd-0.5.5/ocrd_browser/view/registry.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/view/text.py` & `browse-ocrd-0.5.5/ocrd_browser/view/text.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/ocrd_browser/view/xml.py` & `browse-ocrd-0.5.5/ocrd_browser/view/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     def config_changed(self, name: str, value: Any) -> None:
         super().config_changed(name, value)
         self.reload()
 
     def open_jpageviewer(self, _button: Gtk.Button) -> None:
         if self.current and self.current.page_file:
-            Launcher().launch('PageViewer', self.document, self.current.page_file)
+            Launcher().launch('pageviewer', self.document, self.current.page_file)
 
     def on_scroll(self, _widget: GtkSource.View, event: Gdk.EventScroll) -> bool:
         # Handles zoom in / zoom out on Ctrl+mouse wheel
         accel_mask = Gtk.accelerator_get_default_mod_mask()
         if event.state & accel_mask == Gdk.ModifierType.CONTROL_MASK:
             did_scroll, delta_x, delta_y = event.get_scroll_deltas()
             if did_scroll and abs(delta_y) > 0:
```

### Comparing `browse-ocrd-0.5.4/serve.py` & `browse-ocrd-0.5.5/serve.py`

 * *Files identical despite different names*

### Comparing `browse-ocrd-0.5.4/setup.cfg` & `browse-ocrd-0.5.5/setup.cfg`

 * *Files identical despite different names*


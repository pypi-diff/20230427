# Comparing `tmp/Bigsansar-0.9.9.tar.gz` & `tmp/Bigsansar-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-0.9.9.tar", last modified: Mon Nov 28 13:36:41 2022, max compression
+gzip compressed data, was "Bigsansar-1.0.0.tar", last modified: Thu Apr 27 13:56:34 2023, max compression
```

## Comparing `Bigsansar-0.9.9.tar` & `Bigsansar-1.0.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.428430 Bigsansar-0.9.9/
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.420430 Bigsansar-0.9.9/Bigsansar.egg-info/
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)     2834 2022-11-28 13:36:41.000000 Bigsansar-0.9.9/Bigsansar.egg-info/PKG-INFO
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)     2254 2022-11-28 13:36:41.000000 Bigsansar-0.9.9/Bigsansar.egg-info/SOURCES.txt
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)        1 2022-11-28 13:36:41.000000 Bigsansar-0.9.9/Bigsansar.egg-info/dependency_links.txt
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)       51 2022-11-28 13:36:41.000000 Bigsansar-0.9.9/Bigsansar.egg-info/entry_points.txt
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)       82 2022-11-28 13:36:41.000000 Bigsansar-0.9.9/Bigsansar.egg-info/requires.txt
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)       10 2022-11-28 13:36:41.000000 Bigsansar-0.9.9/Bigsansar.egg-info/top_level.txt
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     1073 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/LICENSE
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)     2834 2022-11-28 13:36:41.428430 Bigsansar-0.9.9/PKG-INFO
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     2125 2022-09-17 13:08:53.000000 Bigsansar-0.9.9/README.md
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.424430 Bigsansar-0.9.9/bigsansar/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/bigsansar/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)       63 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/bigsansar/admin.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      188 2022-07-24 05:40:08.000000 Bigsansar-0.9.9/bigsansar/apps.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.424430 Bigsansar-0.9.9/bigsansar/contrib/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-07-29 02:23:12.000000 Bigsansar-0.9.9/bigsansar/contrib/__init__.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.424430 Bigsansar-0.9.9/bigsansar/contrib/account/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-07-29 02:23:38.000000 Bigsansar-0.9.9/bigsansar/contrib/account/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      489 2022-07-29 02:39:27.000000 Bigsansar-0.9.9/bigsansar/contrib/account/admin.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      275 2022-07-29 02:42:59.000000 Bigsansar-0.9.9/bigsansar/contrib/account/apps.py
--rwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)     1155 2022-11-27 06:32:18.000000 Bigsansar-0.9.9/bigsansar/contrib/account/forms.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.424430 Bigsansar-0.9.9/bigsansar/contrib/account/migrations/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      969 2022-08-10 11:13:03.000000 Bigsansar-0.9.9/bigsansar/contrib/account/migrations/0001_initial.py
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)      400 2022-11-27 06:32:18.000000 Bigsansar-0.9.9/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-07-29 02:23:38.000000 Bigsansar-0.9.9/bigsansar/contrib/account/migrations/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      539 2022-07-31 04:08:52.000000 Bigsansar-0.9.9/bigsansar/contrib/account/models.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      340 2022-07-29 03:09:48.000000 Bigsansar-0.9.9/bigsansar/contrib/account/signals.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.424430 Bigsansar-0.9.9/bigsansar/contrib/account/templates/
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-27 06:32:18.000000 Bigsansar-0.9.9/bigsansar/contrib/account/templates/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)       60 2022-07-29 02:23:38.000000 Bigsansar-0.9.9/bigsansar/contrib/account/tests.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-07-29 02:54:05.000000 Bigsansar-0.9.9/bigsansar/contrib/account/urls.py
--rwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-27 07:04:21.000000 Bigsansar-0.9.9/bigsansar/contrib/account/views.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.424430 Bigsansar-0.9.9/bigsansar/contrib/blogs/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-09-11 00:46:48.000000 Bigsansar-0.9.9/bigsansar/contrib/blogs/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      520 2022-09-11 01:01:26.000000 Bigsansar-0.9.9/bigsansar/contrib/blogs/admin.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      188 2022-09-11 00:54:37.000000 Bigsansar-0.9.9/bigsansar/contrib/blogs/apps.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.424430 Bigsansar-0.9.9/bigsansar/contrib/blogs/migrations/
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)     2220 2022-09-11 05:01:12.000000 Bigsansar-0.9.9/bigsansar/contrib/blogs/migrations/0001_initial.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-09-11 00:46:48.000000 Bigsansar-0.9.9/bigsansar/contrib/blogs/migrations/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     1524 2022-09-11 04:47:35.000000 Bigsansar-0.9.9/bigsansar/contrib/blogs/models.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)       60 2022-09-11 00:46:48.000000 Bigsansar-0.9.9/bigsansar/contrib/blogs/tests.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)       63 2022-09-11 00:46:48.000000 Bigsansar-0.9.9/bigsansar/contrib/blogs/views.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.424430 Bigsansar-0.9.9/bigsansar/contrib/sites/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-08-02 03:24:55.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     1684 2022-11-27 07:01:04.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/admin.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      196 2022-08-02 03:28:58.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/apps.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     2936 2022-11-28 13:33:53.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/forms.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.424430 Bigsansar-0.9.9/bigsansar/contrib/sites/migrations/
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)     1769 2022-08-29 12:42:42.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/migrations/0001_initial.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-08-02 03:24:55.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/migrations/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     1760 2022-11-27 06:58:47.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/models.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.428430 Bigsansar-0.9.9/bigsansar/contrib/sites/templatetags/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-08-21 06:12:01.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/templatetags/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      394 2022-08-21 06:14:23.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/templatetags/pages.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)       60 2022-08-02 03:24:55.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/tests.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)       63 2022-08-02 03:24:55.000000 Bigsansar-0.9.9/bigsansar/contrib/sites/views.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.428430 Bigsansar-0.9.9/bigsansar/core/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      500 2022-07-24 05:40:08.000000 Bigsansar-0.9.9/bigsansar/core/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      402 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/bigsansar/core/host.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     7065 2022-11-27 06:51:45.000000 Bigsansar-0.9.9/bigsansar/core/init.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)       26 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/bigsansar/main.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.428430 Bigsansar-0.9.9/bigsansar/management/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/bigsansar/management/__init__.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.428430 Bigsansar-0.9.9/bigsansar/management/commands/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/bigsansar/management/commands/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     1076 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/bigsansar/management/commands/createuser.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.428430 Bigsansar-0.9.9/bigsansar/migrations/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/bigsansar/migrations/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)       57 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/bigsansar/models.py
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.428430 Bigsansar-0.9.9/bigsansar/static/
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-27 06:32:18.000000 Bigsansar-0.9.9/bigsansar/static/__init__.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     9230 2021-06-25 12:28:22.000000 Bigsansar-0.9.9/bigsansar/static/logo.png
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      478 2021-10-04 11:44:26.000000 Bigsansar-0.9.9/bigsansar/static/style.css
-drwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-28 13:36:41.428430 Bigsansar-0.9.9/bigsansar/templates/
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      947 2022-08-20 01:26:11.000000 Bigsansar-0.9.9/bigsansar/templates/404.html
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)        0 2022-11-27 06:32:18.000000 Bigsansar-0.9.9/bigsansar/templates/__init__.py
--rwxrwxr-x   0 pokhrelb9  (1000) pokhrelb9  (1000)      164 2022-11-27 06:32:18.000000 Bigsansar-0.9.9/bigsansar/templates/acc_active_email.html
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     1104 2022-05-17 12:22:34.000000 Bigsansar-0.9.9/bigsansar/templates/base.html
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     2207 2022-06-03 05:54:41.000000 Bigsansar-0.9.9/bigsansar/templates/default.html
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     2206 2022-08-20 01:25:43.000000 Bigsansar-0.9.9/bigsansar/templates/defaultpage.html
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     2109 2022-05-08 10:16:56.000000 Bigsansar-0.9.9/bigsansar/templates/nav.html
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      725 2022-05-21 13:13:59.000000 Bigsansar-0.9.9/bigsansar/templates/parking.html
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)       60 2022-07-17 12:32:17.000000 Bigsansar-0.9.9/bigsansar/tests.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)      796 2022-08-25 11:12:52.000000 Bigsansar-0.9.9/bigsansar/urls.py
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     1854 2022-09-04 04:19:55.000000 Bigsansar-0.9.9/bigsansar/views.py
--rw-rw-r--   0 pokhrelb9  (1000) pokhrelb9  (1000)       38 2022-11-28 13:36:41.428430 Bigsansar-0.9.9/setup.cfg
--rwxrwxrwx   0 pokhrelb9  (1000) pokhrelb9  (1000)     1257 2022-11-28 13:36:08.000000 Bigsansar-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.772078 Bigsansar-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.652717 Bigsansar-1.0.0/Bigsansar.egg-info/
+-rw-rw-rw-   0        0        0     2889 2023-04-27 13:56:34.000000 Bigsansar-1.0.0/Bigsansar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2244 2023-04-27 13:56:34.000000 Bigsansar-1.0.0/Bigsansar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:56:34.000000 Bigsansar-1.0.0/Bigsansar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-27 13:56:34.000000 Bigsansar-1.0.0/Bigsansar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2023-04-27 13:56:34.000000 Bigsansar-1.0.0/Bigsansar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-27 13:56:34.000000 Bigsansar-1.0.0/Bigsansar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2889 2023-04-27 13:56:34.770380 Bigsansar-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.671728 Bigsansar-1.0.0/bigsansar/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/admin.py
+-rw-rw-rw-   0        0        0      195 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.671728 Bigsansar-1.0.0/bigsansar/contrib/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.689424 Bigsansar-1.0.0/bigsansar/contrib/account/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/__init__.py
+-rw-rw-rw-   0        0        0      510 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/admin.py
+-rw-rw-rw-   0        0        0      284 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/apps.py
+-rw-rw-rw-   0        0        0     1176 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.691941 Bigsansar-1.0.0/bigsansar/contrib/account/migrations/
+-rw-rw-rw-   0        0        0      999 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      417 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/migrations/__init__.py
+-rw-rw-rw-   0        0        0      556 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/models.py
+-rw-rw-rw-   0        0        0      351 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/signals.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.699230 Bigsansar-1.0.0/bigsansar/contrib/account/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/templates/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/tests.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/urls.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/account/views.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.710255 Bigsansar-1.0.0/bigsansar/contrib/blogs/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/blogs/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/blogs/admin.py
+-rw-rw-rw-   0        0        0      195 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/blogs/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.712356 Bigsansar-1.0.0/bigsansar/contrib/blogs/migrations/
+-rw-rw-rw-   0        0        0     2272 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1572 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/blogs/models.py
+-rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/blogs/tests.py
+-rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/blogs/views.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.726092 Bigsansar-1.0.0/bigsansar/contrib/sites/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/admin.py
+-rw-rw-rw-   0        0        0      203 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/apps.py
+-rw-rw-rw-   0        0        0     3018 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.732594 Bigsansar-1.0.0/bigsansar/contrib/sites/migrations/
+-rw-rw-rw-   0        0        0     1816 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1826 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/models.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.735836 Bigsansar-1.0.0/bigsansar/contrib/sites/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      408 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/templatetags/pages.py
+-rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/tests.py
+-rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/contrib/sites/views.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.740327 Bigsansar-1.0.0/bigsansar/core/
+-rw-rw-rw-   0        0        0      524 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/core/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/core/host.py
+-rw-rw-rw-   0        0        0     7265 2023-04-27 12:43:38.000000 Bigsansar-1.0.0/bigsansar/core/init.py
+-rw-rw-rw-   0        0        0       27 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/main.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.740327 Bigsansar-1.0.0/bigsansar/management/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.744557 Bigsansar-1.0.0/bigsansar/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1122 2023-04-27 12:44:33.000000 Bigsansar-1.0.0/bigsansar/management/commands/createuser.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.747861 Bigsansar-1.0.0/bigsansar/migrations/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/models.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.753024 Bigsansar-1.0.0/bigsansar/static/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/static/__init__.py
+-rw-rw-rw-   0        0        0     9230 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/static/logo.png
+-rw-rw-rw-   0        0        0      525 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/static/style.css
+drwxrwxrwx   0        0        0        0 2023-04-27 13:56:34.768370 Bigsansar-1.0.0/bigsansar/templates/
+-rw-rw-rw-   0        0        0      977 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/templates/404.html
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/templates/__init__.py
+-rw-rw-rw-   0        0        0      168 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/templates/acc_active_email.html
+-rw-rw-rw-   0        0        0     1134 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/templates/base.html
+-rw-rw-rw-   0        0        0     2252 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/templates/default.html
+-rw-rw-rw-   0        0        0     2250 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/templates/defaultpage.html
+-rw-rw-rw-   0        0        0     2171 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/templates/nav.html
+-rw-rw-rw-   0        0        0      758 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/templates/parking.html
+-rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/tests.py
+-rw-rw-rw-   0        0        0      821 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/urls.py
+-rw-rw-rw-   0        0        0     1910 2023-04-27 12:27:15.000000 Bigsansar-1.0.0/bigsansar/views.py
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:56:34.772588 Bigsansar-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2023-04-27 13:55:59.000000 Bigsansar-1.0.0/setup.py
```

### Comparing `Bigsansar-0.9.9/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.0.0/Bigsansar.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,91 @@
-Metadata-Version: 2.1
-Name: Bigsansar
-Version: 0.9.9
-Summary: Build one in minutes with bigsansar - a visual site building tool!
-Home-page: https://bigsansar.com
-Author: Bikash Pokhrel
-Author-email: bigsansaroffice@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
-Project-URL: Documentations, https://docs.bigsansar.com/
-Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# How to get Bigsansar
-
-Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
-Bigsansar is Fully based on django.
-You can use
-[bigsansar](https://bigsansar.com)
-for install packaged.
-
-view our tutorials in 
-[youtube](https://youtube.com/bigsansar)
-
-for playlist:
-[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
-
-# Get the latest development version
-The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
-This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
-Get it using this shell command, which requires [Git](https://git-scm.com/):
-
-`git clone https://github.com/pokhrelb9/bigsansar.git`
-
-You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
-This archive is updated every time we commit code.
-
-# After you install bigsansar
-Type `bigsansar init` command for **automatically** setup server . 
-
-# For manually setup
-
-### After you get it
-
-go to `www` path and open `settings.py` file then add 
-`'bigsansar.apps.BigsansarConfig'`
-`'bigsansar.contrib.account.apps.AccountConfig'`
-in to 
-`INSTALLED_APPS = []` .
-
-### For Virtualhost middleware
-go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
-`MIDDLEWARE = []` .
-
-## Some usefull commands:
-
-`python3 manage.py createuser` - get unlimited users.
-
-
-
-## New update 
-* added virtual host in to admin pannel 
-* added pages system and working in this model 
-* making too easy to handel django with help of bigsansar in the future .
-* Removed signup systems prebuilded .
-
-
-## Load page in templates
-
-`{% load pages %}
-
-{% get_pages  as listpage %}
-{% for page in listpage %}
-<div>
-    < a href="{{ page.slug }}">{{ page.title }}</a>
-</div>
-{% endfor %}`
-
-#### More variable for **page**
-* page.id
-* page.domain
-* page.title
-* page.slug
-* page.body
-* page.visitor
-* page.publish_date
-
+Metadata-Version: 2.1
+Name: Bigsansar
+Version: 1.0.0
+Summary: Build one in minutes with bigsansar - a visual site building tool!
+Home-page: https://bigsansar.com
+Author: Bikash Pokhrel
+Author-email: bigsansaroffice@gmail.com
+Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
+Project-URL: Documentations, https://docs.bigsansar.com/
+Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# How to get Bigsansar
+
+Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
+Bigsansar is Fully based on django.
+You can use
+[bigsansar](https://bigsansar.com)
+for install packaged.
+
+view our tutorials in 
+[youtube](https://youtube.com/bigsansar)
+
+for playlist:
+[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
+
+# Get the latest development version
+The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
+This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
+Get it using this shell command, which requires [Git](https://git-scm.com/):
+
+`git clone https://github.com/pokhrelb9/bigsansar.git`
+
+You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
+This archive is updated every time we commit code.
+
+# After you install bigsansar
+Type `bigsansar init` command for **automatically** setup server . 
+
+# For manually setup
+
+### After you get it
+
+go to `www` path and open `settings.py` file then add 
+`'bigsansar.apps.BigsansarConfig'`
+`'bigsansar.contrib.account.apps.AccountConfig'`
+in to 
+`INSTALLED_APPS = []` .
+
+### For Virtualhost middleware
+go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
+`MIDDLEWARE = []` .
+
+## Some usefull commands:
+
+`python3 manage.py createuser` - get unlimited users.
+
+
+
+## New update 
+* added virtual host in to admin pannel 
+* added pages system and working in this model 
+* making too easy to handel django with help of bigsansar in the future .
+* Removed signup systems prebuilded .
+
+
+## Load page in templates
+
+`{% load pages %}
+
+{% get_pages  as listpage %}
+{% for page in listpage %}
+<div>
+    < a href="{{ page.slug }}">{{ page.title }}</a>
+</div>
+{% endfor %}`
+
+#### More variable for **page**
+* page.id
+* page.domain
+* page.title
+* page.slug
+* page.body
+* page.visitor
+* page.publish_date
```

### Comparing `Bigsansar-0.9.9/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.0.0/Bigsansar.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-setup.cfg
 setup.py
 Bigsansar.egg-info/PKG-INFO
 Bigsansar.egg-info/SOURCES.txt
 Bigsansar.egg-info/dependency_links.txt
 Bigsansar.egg-info/entry_points.txt
 Bigsansar.egg-info/requires.txt
 Bigsansar.egg-info/top_level.txt
```

### Comparing `Bigsansar-0.9.9/LICENSE` & `Bigsansar-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `Bigsansar-0.9.9/PKG-INFO` & `Bigsansar-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,91 @@
-Metadata-Version: 2.1
-Name: Bigsansar
-Version: 0.9.9
-Summary: Build one in minutes with bigsansar - a visual site building tool!
-Home-page: https://bigsansar.com
-Author: Bikash Pokhrel
-Author-email: bigsansaroffice@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
-Project-URL: Documentations, https://docs.bigsansar.com/
-Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# How to get Bigsansar
-
-Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
-Bigsansar is Fully based on django.
-You can use
-[bigsansar](https://bigsansar.com)
-for install packaged.
-
-view our tutorials in 
-[youtube](https://youtube.com/bigsansar)
-
-for playlist:
-[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
-
-# Get the latest development version
-The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
-This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
-Get it using this shell command, which requires [Git](https://git-scm.com/):
-
-`git clone https://github.com/pokhrelb9/bigsansar.git`
-
-You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
-This archive is updated every time we commit code.
-
-# After you install bigsansar
-Type `bigsansar init` command for **automatically** setup server . 
-
-# For manually setup
-
-### After you get it
-
-go to `www` path and open `settings.py` file then add 
-`'bigsansar.apps.BigsansarConfig'`
-`'bigsansar.contrib.account.apps.AccountConfig'`
-in to 
-`INSTALLED_APPS = []` .
-
-### For Virtualhost middleware
-go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
-`MIDDLEWARE = []` .
-
-## Some usefull commands:
-
-`python3 manage.py createuser` - get unlimited users.
-
-
-
-## New update 
-* added virtual host in to admin pannel 
-* added pages system and working in this model 
-* making too easy to handel django with help of bigsansar in the future .
-* Removed signup systems prebuilded .
-
-
-## Load page in templates
-
-`{% load pages %}
-
-{% get_pages  as listpage %}
-{% for page in listpage %}
-<div>
-    < a href="{{ page.slug }}">{{ page.title }}</a>
-</div>
-{% endfor %}`
-
-#### More variable for **page**
-* page.id
-* page.domain
-* page.title
-* page.slug
-* page.body
-* page.visitor
-* page.publish_date
-
+Metadata-Version: 2.1
+Name: Bigsansar
+Version: 1.0.0
+Summary: Build one in minutes with bigsansar - a visual site building tool!
+Home-page: https://bigsansar.com
+Author: Bikash Pokhrel
+Author-email: bigsansaroffice@gmail.com
+Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
+Project-URL: Documentations, https://docs.bigsansar.com/
+Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# How to get Bigsansar
+
+Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
+Bigsansar is Fully based on django.
+You can use
+[bigsansar](https://bigsansar.com)
+for install packaged.
+
+view our tutorials in 
+[youtube](https://youtube.com/bigsansar)
+
+for playlist:
+[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
+
+# Get the latest development version
+The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
+This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
+Get it using this shell command, which requires [Git](https://git-scm.com/):
+
+`git clone https://github.com/pokhrelb9/bigsansar.git`
+
+You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
+This archive is updated every time we commit code.
+
+# After you install bigsansar
+Type `bigsansar init` command for **automatically** setup server . 
+
+# For manually setup
+
+### After you get it
+
+go to `www` path and open `settings.py` file then add 
+`'bigsansar.apps.BigsansarConfig'`
+`'bigsansar.contrib.account.apps.AccountConfig'`
+in to 
+`INSTALLED_APPS = []` .
+
+### For Virtualhost middleware
+go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
+`MIDDLEWARE = []` .
+
+## Some usefull commands:
+
+`python3 manage.py createuser` - get unlimited users.
+
+
+
+## New update 
+* added virtual host in to admin pannel 
+* added pages system and working in this model 
+* making too easy to handel django with help of bigsansar in the future .
+* Removed signup systems prebuilded .
+
+
+## Load page in templates
+
+`{% load pages %}
+
+{% get_pages  as listpage %}
+{% for page in listpage %}
+<div>
+    < a href="{{ page.slug }}">{{ page.title }}</a>
+</div>
+{% endfor %}`
+
+#### More variable for **page**
+* page.id
+* page.domain
+* page.title
+* page.slug
+* page.body
+* page.visitor
+* page.publish_date
```

### Comparing `Bigsansar-0.9.9/README.md` & `Bigsansar-1.0.0/README.md`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-
-# How to get Bigsansar
-
-Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
-Bigsansar is Fully based on django.
-You can use
-[bigsansar](https://bigsansar.com)
-for install packaged.
-
-view our tutorials in 
-[youtube](https://youtube.com/bigsansar)
-
-for playlist:
-[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
-
-# Get the latest development version
-The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
-This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
-Get it using this shell command, which requires [Git](https://git-scm.com/):
-
-`git clone https://github.com/pokhrelb9/bigsansar.git`
-
-You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
-This archive is updated every time we commit code.
-
-# After you install bigsansar
-Type `bigsansar init` command for **automatically** setup server . 
-
-# For manually setup
-
-### After you get it
-
-go to `www` path and open `settings.py` file then add 
-`'bigsansar.apps.BigsansarConfig'`
-`'bigsansar.contrib.account.apps.AccountConfig'`
-in to 
-`INSTALLED_APPS = []` .
-
-### For Virtualhost middleware
-go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
-`MIDDLEWARE = []` .
-
-## Some usefull commands:
-
-`python3 manage.py createuser` - get unlimited users.
-
-
-
-## New update 
-* added virtual host in to admin pannel 
-* added pages system and working in this model 
-* making too easy to handel django with help of bigsansar in the future .
-* Removed signup systems prebuilded .
-
-
-## Load page in templates
-
-`{% load pages %}
-
-{% get_pages  as listpage %}
-{% for page in listpage %}
-<div>
-    < a href="{{ page.slug }}">{{ page.title }}</a>
-</div>
-{% endfor %}`
-
-#### More variable for **page**
-* page.id
-* page.domain
-* page.title
-* page.slug
-* page.body
-* page.visitor
+
+# How to get Bigsansar
+
+Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
+Bigsansar is Fully based on django.
+You can use
+[bigsansar](https://bigsansar.com)
+for install packaged.
+
+view our tutorials in 
+[youtube](https://youtube.com/bigsansar)
+
+for playlist:
+[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
+
+# Get the latest development version
+The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
+This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
+Get it using this shell command, which requires [Git](https://git-scm.com/):
+
+`git clone https://github.com/pokhrelb9/bigsansar.git`
+
+You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
+This archive is updated every time we commit code.
+
+# After you install bigsansar
+Type `bigsansar init` command for **automatically** setup server . 
+
+# For manually setup
+
+### After you get it
+
+go to `www` path and open `settings.py` file then add 
+`'bigsansar.apps.BigsansarConfig'`
+`'bigsansar.contrib.account.apps.AccountConfig'`
+in to 
+`INSTALLED_APPS = []` .
+
+### For Virtualhost middleware
+go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
+`MIDDLEWARE = []` .
+
+## Some usefull commands:
+
+`python3 manage.py createuser` - get unlimited users.
+
+
+
+## New update 
+* added virtual host in to admin pannel 
+* added pages system and working in this model 
+* making too easy to handel django with help of bigsansar in the future .
+* Removed signup systems prebuilded .
+
+
+## Load page in templates
+
+`{% load pages %}
+
+{% get_pages  as listpage %}
+{% for page in listpage %}
+<div>
+    < a href="{{ page.slug }}">{{ page.title }}</a>
+</div>
+{% endfor %}`
+
+#### More variable for **page**
+* page.id
+* page.domain
+* page.title
+* page.slug
+* page.body
+* page.visitor
 * page.publish_date
```

### Comparing `Bigsansar-0.9.9/bigsansar/contrib/account/forms.py` & `Bigsansar-1.0.0/bigsansar/contrib/account/forms.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from django import forms
-from django.contrib.auth.forms import UserCreationForm
-from django.contrib.auth.models import User
-from django.core.validators import RegexValidator
-
-
-class SignUpForm(UserCreationForm):
-    email = forms.EmailField(max_length=60, min_length=5, widget=forms.TextInput(attrs={'class': 'form-control',}))
-    username = forms.CharField(max_length=50, validators=[RegexValidator('^[a-z0-9]+$', message='use small Letters and digits with minimum of 3 character')], min_length=3, help_text='use Letters and digits with minimum of 3 character',widget=forms.TextInput(attrs={'class': 'form-control'}))
-    password1 = forms.CharField(label='Password', widget=forms.PasswordInput(attrs={'class': 'form-control'}))
-    password2 = forms.CharField(label='Password confirmation', widget=forms.PasswordInput(attrs={'class': 'form-control'}))
-
-    class Meta:
-        model = User
-        fields = ('username',  'email',)
-
-    def clean_email(self):
-        email = self.cleaned_data['email']
-        if User.objects.filter(email__iexact=email).exists():
-            raise forms.ValidationError('Email is Already Exists')
-        return email
+from django import forms
+from django.contrib.auth.forms import UserCreationForm
+from django.contrib.auth.models import User
+from django.core.validators import RegexValidator
+
+
+class SignUpForm(UserCreationForm):
+    email = forms.EmailField(max_length=60, min_length=5, widget=forms.TextInput(attrs={'class': 'form-control',}))
+    username = forms.CharField(max_length=50, validators=[RegexValidator('^[a-z0-9]+$', message='use small Letters and digits with minimum of 3 character')], min_length=3, help_text='use Letters and digits with minimum of 3 character',widget=forms.TextInput(attrs={'class': 'form-control'}))
+    password1 = forms.CharField(label='Password', widget=forms.PasswordInput(attrs={'class': 'form-control'}))
+    password2 = forms.CharField(label='Password confirmation', widget=forms.PasswordInput(attrs={'class': 'form-control'}))
+
+    class Meta:
+        model = User
+        fields = ('username',  'email',)
+
+    def clean_email(self):
+        email = self.cleaned_data['email']
+        if User.objects.filter(email__iexact=email).exists():
+            raise forms.ValidationError('Email is Already Exists')
+        return email
```

### Comparing `Bigsansar-0.9.9/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.0.0/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Generated by Django 4.0.6 on 2022-08-10 11:13
-
-from django.conf import settings
-from django.db import migrations, models
-import django.db.models.deletion
-import phonenumber_field.modelfields
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-        ('auth', '0012_alter_user_first_name_max_length'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='userinfo',
-            fields=[
-                ('user', models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, primary_key=True, serialize=False, to=settings.AUTH_USER_MODEL)),
-                ('phone', phonenumber_field.modelfields.PhoneNumberField(max_length=128, region=None)),
-                ('address', models.CharField(default='none', max_length=25)),
-            ],
-            options={
-                'verbose_name': 'User Advance Information',
-                'verbose_name_plural': 'Profile Details',
-            },
-        ),
-    ]
+# Generated by Django 4.0.6 on 2022-08-10 11:13
+
+from django.conf import settings
+from django.db import migrations, models
+import django.db.models.deletion
+import phonenumber_field.modelfields
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+        ('auth', '0012_alter_user_first_name_max_length'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='userinfo',
+            fields=[
+                ('user', models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, primary_key=True, serialize=False, to=settings.AUTH_USER_MODEL)),
+                ('phone', phonenumber_field.modelfields.PhoneNumberField(max_length=128, region=None)),
+                ('address', models.CharField(default='none', max_length=25)),
+            ],
+            options={
+                'verbose_name': 'User Advance Information',
+                'verbose_name_plural': 'Profile Details',
+            },
+        ),
+    ]
```

### Comparing `Bigsansar-0.9.9/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.0.0/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-# Generated by Django 4.0.6 on 2022-09-11 05:01
-
-import ckeditor.fields
-from django.conf import settings
-from django.db import migrations, models
-import django.db.models.deletion
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-        ('sites', '0001_initial'),
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='post',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('title', models.CharField(default='| Bigsansar', max_length=100)),
-                ('thumbnails', models.ImageField(blank=True, upload_to='%Y/%m/%d/')),
-                ('slug', models.SlugField(unique=True)),
-                ('body', ckeditor.fields.RichTextField()),
-                ('visitor', models.IntegerField(default=0)),
-                ('publish_date', models.DateField(auto_now_add=True)),
-                ('domain', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='sites.domains')),
-                ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
-            ],
-            options={
-                'verbose_name': 'Posts',
-                'verbose_name_plural': 'Posts',
-            },
-        ),
-        migrations.CreateModel(
-            name='comment',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('comments', models.TextField()),
-                ('publish_date', models.DateTimeField(auto_now=True)),
-                ('reply', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='blogs.comment')),
-                ('title', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='blogs.post')),
-                ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
-            ],
-            options={
-                'verbose_name': 'Comments',
-                'verbose_name_plural': 'Comments',
-            },
-        ),
-    ]
+# Generated by Django 4.0.6 on 2022-09-11 05:01
+
+import ckeditor.fields
+from django.conf import settings
+from django.db import migrations, models
+import django.db.models.deletion
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+        ('sites', '0001_initial'),
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='post',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('title', models.CharField(default='| Bigsansar', max_length=100)),
+                ('thumbnails', models.ImageField(blank=True, upload_to='%Y/%m/%d/')),
+                ('slug', models.SlugField(unique=True)),
+                ('body', ckeditor.fields.RichTextField()),
+                ('visitor', models.IntegerField(default=0)),
+                ('publish_date', models.DateField(auto_now_add=True)),
+                ('domain', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='sites.domains')),
+                ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
+            ],
+            options={
+                'verbose_name': 'Posts',
+                'verbose_name_plural': 'Posts',
+            },
+        ),
+        migrations.CreateModel(
+            name='comment',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('comments', models.TextField()),
+                ('publish_date', models.DateTimeField(auto_now=True)),
+                ('reply', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='blogs.comment')),
+                ('title', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='blogs.post')),
+                ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
+            ],
+            options={
+                'verbose_name': 'Comments',
+                'verbose_name_plural': 'Comments',
+            },
+        ),
+    ]
```

### Comparing `Bigsansar-0.9.9/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.0.0/bigsansar/contrib/sites/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,67 @@
-from ckeditor.fields import RichTextField
-from django.contrib.auth.models import User
-from django.db import models
-from django.urls import reverse
-
-from bigsansar.contrib.sites.models import domains
-
-
-# Create your models here.
-
-class post(models.Model):
-    domain = models.ForeignKey(domains, on_delete=models.CASCADE)
-    user = models.ForeignKey(User, on_delete=models.CASCADE)
-    title = models.CharField(max_length=100, default='| Bigsansar')
-    thumbnails = models.ImageField(upload_to='%Y/%m/%d/', blank=True)
-    slug = models.SlugField(unique=True)
-    body = RichTextField()
-    visitor = models.IntegerField(default=0)
-    publish_date = models.DateField(auto_now_add=True)
-
-    def delete(self, using=None, keep_parents=False):
-        self.thumbnails.storage.delete(self.thumbnails.name)
-        super().delete()
-
-    def __str__(self):
-        return self.title
-
-    class Meta:
-        verbose_name = 'Posts'
-        verbose_name_plural = 'Posts'
-
-    # def get_absolute_url(self):
-    #     return reverse("blog", kwargs={"slug": self.slug})
-
-
-class comment(models.Model):
-    user = models.ForeignKey(User, on_delete=models.CASCADE)
-    title = models.ForeignKey(post, on_delete=models.CASCADE)
-    comments = models.TextField()
-    reply = models.ForeignKey('self', on_delete=models.CASCADE, null=True)
-    publish_date = models.DateTimeField(auto_now=True)
-
-    def __str__(self):
-        return self.comments
-
-    class Meta:
-        verbose_name = 'Comments'
-        verbose_name_plural = 'Comments'
+import os
+import shutil
+
+from django.contrib.auth.models import User
+from django.db import models
+
+from www.settings import BASE_DIR
+
+
+# Create your models here.
+
+
+class domains(models.Model):
+    user = models.ForeignKey(User, on_delete=models.CASCADE)
+    domain = models.CharField(max_length=100, unique=True)
+    publish_date = models.DateField(auto_now_add=True)
+    visitor = models.IntegerField(default=1)
+
+    def __str__(self):
+        return self.domain
+
+    class Meta:
+        verbose_name = 'Domain'
+        verbose_name_plural = 'Custom Domain'
+
+    def get_absolute_url(self):
+        return "http://%s" % (self.domain,)
+
+    def delete(self, using=None, keep_parents=False):
+        filename = 'templates' + '/' + str(self.id)
+        try:
+            full_url = os.path.join(BASE_DIR, filename)
+            shutil.rmtree(full_url)
+
+        except:
+            pass
+
+        super().delete()
+
+
+class pages(models.Model):
+    domain = models.ForeignKey(domains, on_delete=models.CASCADE)
+    title = models.CharField(max_length=50)
+    slug = models.SlugField()
+    body = models.TextField()
+    visitor = models.IntegerField(default=0)
+    publish_date = models.DateField(auto_now_add=True)
+
+    class Meta:
+        verbose_name = 'Pages'
+        verbose_name_plural = 'Pages'
+
+    def __str__(self):
+        return self.domain.domain
+
+    def get_absolute_url(self):
+        return "http://%s/%s" % (self.domain, self.slug)
+
+    def delete(self, using=None, keep_parents=False):
+        filename = 'templates' + '/' + str(self.domain.id) + '/' + self.slug + '.html'
+        full_url = os.path.join(BASE_DIR, filename)
+        if os.path.exists(full_url):
+            os.remove(full_url)
+        else:
+            pass
+
+        super().delete()
```

### Comparing `Bigsansar-0.9.9/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.0.0/bigsansar/contrib/sites/admin.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from django.contrib import admin
-from django.contrib.admin import SimpleListFilter
-from django.utils.translation import gettext_lazy as _
-from bigsansar.contrib.sites.forms import create_domainform, customaddpageform, custompageform
-from bigsansar.contrib.sites.models import domains, pages
-
-
-# Register your models here.
-
-
-class domain_filter(SimpleListFilter):
-    title = _('Domains')  # a label for our filter
-    parameter_name = "domain"  # you can put anything here
-
-    def lookups(self, request, model_admin):
-        # This is where you create filter options; we have two:
-        qs = model_admin.get_queryset(request)
-        return qs.values_list('domain_id', 'domain__domain').order_by('domain').distinct()
-
-    def queryset(self, request, queryset):
-
-        # This is where you process parameters selected by use via filter options:
-        if self.value():
-            return queryset.filter(domain=self.value())
-
-
-class domainadmin(admin.ModelAdmin):
-    form = create_domainform
-    list_display = ['domain', 'publish_date', 'visitor']
-
-
-class pageadmin(admin.ModelAdmin):
-    add_form = customaddpageform
-    form = custompageform
-    prepopulated_fields = {"slug": ("title",)}
-    list_display = ['title', 'domain', 'publish_date', 'visitor']
-    list_filter = (domain_filter,)
-
-    def get_form(self, request, obj=None, **kwargs):
-        """
-        Use special form during foo creation
-        """
-        defaults = {}
-        if obj is None:
-            defaults['form'] = self.add_form
-        defaults.update(kwargs)
-        return super().get_form(request, obj, **defaults)
-
-
-admin.site.register(domains, domainadmin)
+from django.contrib import admin
+from django.contrib.admin import SimpleListFilter
+from django.utils.translation import gettext_lazy as _
+from bigsansar.contrib.sites.forms import create_domainform, customaddpageform, custompageform
+from bigsansar.contrib.sites.models import domains, pages
+
+
+# Register your models here.
+
+
+class domain_filter(SimpleListFilter):
+    title = _('Domains')  # a label for our filter
+    parameter_name = "domain"  # you can put anything here
+
+    def lookups(self, request, model_admin):
+        # This is where you create filter options; we have two:
+        qs = model_admin.get_queryset(request)
+        return qs.values_list('domain_id', 'domain__domain').order_by('domain').distinct()
+
+    def queryset(self, request, queryset):
+
+        # This is where you process parameters selected by use via filter options:
+        if self.value():
+            return queryset.filter(domain=self.value())
+
+
+class domainadmin(admin.ModelAdmin):
+    form = create_domainform
+    list_display = ['domain', 'publish_date', 'visitor']
+
+
+class pageadmin(admin.ModelAdmin):
+    add_form = customaddpageform
+    form = custompageform
+    prepopulated_fields = {"slug": ("title",)}
+    list_display = ['title', 'domain', 'publish_date', 'visitor']
+    list_filter = (domain_filter,)
+
+    def get_form(self, request, obj=None, **kwargs):
+        """
+        Use special form during foo creation
+        """
+        defaults = {}
+        if obj is None:
+            defaults['form'] = self.add_form
+        defaults.update(kwargs)
+        return super().get_form(request, obj, **defaults)
+
+
+admin.site.register(domains, domainadmin)
 admin.site.register(pages, pageadmin)
```

### Comparing `Bigsansar-0.9.9/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.0.0/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# Generated by Django 4.0.6 on 2022-08-29 12:42
-
-from django.conf import settings
-from django.db import migrations, models
-import django.db.models.deletion
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='domains',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('domain', models.CharField(max_length=100, unique=True)),
-                ('publish_date', models.DateField(auto_now_add=True)),
-                ('visitor', models.IntegerField(default=1)),
-                ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
-            ],
-            options={
-                'verbose_name': 'Domain',
-                'verbose_name_plural': 'Custom Domain',
-            },
-        ),
-        migrations.CreateModel(
-            name='pages',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('title', models.CharField(max_length=50)),
-                ('slug', models.SlugField()),
-                ('body', models.TextField()),
-                ('visitor', models.IntegerField(default=0)),
-                ('publish_date', models.DateField(auto_now_add=True)),
-                ('domain', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='sites.domains')),
-            ],
-            options={
-                'verbose_name': 'Pages',
-                'verbose_name_plural': 'Pages',
-            },
-        ),
-    ]
+# Generated by Django 4.0.6 on 2022-08-29 12:42
+
+from django.conf import settings
+from django.db import migrations, models
+import django.db.models.deletion
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='domains',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('domain', models.CharField(max_length=100, unique=True)),
+                ('publish_date', models.DateField(auto_now_add=True)),
+                ('visitor', models.IntegerField(default=1)),
+                ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
+            ],
+            options={
+                'verbose_name': 'Domain',
+                'verbose_name_plural': 'Custom Domain',
+            },
+        ),
+        migrations.CreateModel(
+            name='pages',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('title', models.CharField(max_length=50)),
+                ('slug', models.SlugField()),
+                ('body', models.TextField()),
+                ('visitor', models.IntegerField(default=0)),
+                ('publish_date', models.DateField(auto_now_add=True)),
+                ('domain', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='sites.domains')),
+            ],
+            options={
+                'verbose_name': 'Pages',
+                'verbose_name_plural': 'Pages',
+            },
+        ),
+    ]
```

### Comparing `Bigsansar-0.9.9/bigsansar/contrib/sites/models.py` & `Bigsansar-1.0.0/bigsansar/contrib/blogs/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,48 @@
-import os
-import shutil
-
-from django.contrib.auth.models import User
-from django.db import models
-
-from www.settings import BASE_DIR
-
-
-# Create your models here.
-
-
-class domains(models.Model):
-    user = models.ForeignKey(User, on_delete=models.CASCADE)
-    domain = models.CharField(max_length=100, unique=True)
-    publish_date = models.DateField(auto_now_add=True)
-    visitor = models.IntegerField(default=1)
-
-    def __str__(self):
-        return self.domain
-
-    class Meta:
-        verbose_name = 'Domain'
-        verbose_name_plural = 'Custom Domain'
-
-    def get_absolute_url(self):
-        return "http://%s" % (self.domain,)
-
-    def delete(self, using=None, keep_parents=False):
-        filename = 'templates' + '/' + str(self.id)
-        try:
-            full_url = os.path.join(BASE_DIR, filename)
-            shutil.rmtree(full_url)
-
-        except:
-            pass
-
-        super().delete()
-
-
-class pages(models.Model):
-    domain = models.ForeignKey(domains, on_delete=models.CASCADE)
-    title = models.CharField(max_length=50)
-    slug = models.SlugField()
-    body = models.TextField()
-    visitor = models.IntegerField(default=0)
-    publish_date = models.DateField(auto_now_add=True)
-
-    class Meta:
-        verbose_name = 'Pages'
-        verbose_name_plural = 'Pages'
-
-    def __str__(self):
-        return self.domain.domain
-
-    def get_absolute_url(self):
-        return "http://%s/%s" % (self.domain, self.slug)
-
-    def delete(self, using=None, keep_parents=False):
-        filename = 'templates' + '/' + str(self.domain.id) + '/' + self.slug + '.html'
-        full_url = os.path.join(BASE_DIR, filename)
-        if os.path.exists(full_url):
-            os.remove(full_url)
-        else:
-            pass
-
-        super().delete()
+from ckeditor.fields import RichTextField
+from django.contrib.auth.models import User
+from django.db import models
+from django.urls import reverse
+
+from bigsansar.contrib.sites.models import domains
+
+
+# Create your models here.
+
+class post(models.Model):
+    domain = models.ForeignKey(domains, on_delete=models.CASCADE)
+    user = models.ForeignKey(User, on_delete=models.CASCADE)
+    title = models.CharField(max_length=100, default='| Bigsansar')
+    thumbnails = models.ImageField(upload_to='%Y/%m/%d/', blank=True)
+    slug = models.SlugField(unique=True)
+    body = RichTextField()
+    visitor = models.IntegerField(default=0)
+    publish_date = models.DateField(auto_now_add=True)
+
+    def delete(self, using=None, keep_parents=False):
+        self.thumbnails.storage.delete(self.thumbnails.name)
+        super().delete()
+
+    def __str__(self):
+        return self.title
+
+    class Meta:
+        verbose_name = 'Posts'
+        verbose_name_plural = 'Posts'
+
+    # def get_absolute_url(self):
+    #     return reverse("blog", kwargs={"slug": self.slug})
+
+
+class comment(models.Model):
+    user = models.ForeignKey(User, on_delete=models.CASCADE)
+    title = models.ForeignKey(post, on_delete=models.CASCADE)
+    comments = models.TextField()
+    reply = models.ForeignKey('self', on_delete=models.CASCADE, null=True)
+    publish_date = models.DateTimeField(auto_now=True)
+
+    def __str__(self):
+        return self.comments
+
+    class Meta:
+        verbose_name = 'Comments'
+        verbose_name_plural = 'Comments'
```

### Comparing `Bigsansar-0.9.9/bigsansar/static/logo.png` & `Bigsansar-1.0.0/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-0.9.9/bigsansar/templates/default.html` & `Bigsansar-1.0.0/bigsansar/templates/defaultpage.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-<html>
-<head>
-    <title>Website created successfully - Hosted by bigsansar.com</title>
-    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <style type="text/css">
-    .clear {display:inline-block;}
-    .clear:after {content:" ";display:block;height:0;clear:both;overflow:hidden;visibility:hidden;}
-    .clear {display:block;}
-    body {background-color:#f9f9f9;font-family:Tahoma,Geneva,Kalimati,sans-serif;}
-    img {border:none;}
-    #content {width:963px; margin-left:auto;margin-right:auto;margin-top:90px;}
-    #logo {top:36px;left:55px;position:absolute;display:block;width:auto;height:auto;}
-    #content .content {background: #6b6b6b  repeat-y 7px top; margin:0;position:relative;float:left;width:961px;background-size:99%;height:300px;}
-    h1 {font-size:40px;text-align:center;font-weight:700;color:white;margin-top:130px;}
-    #content p {color:#ffffff;font-size:15px;padding:0 69px;}
-    #footer {clear:both;font-size:11px;color:#999999;width:961px;margin-left:auto;margin-right:auto;margin-top:25px;margin-bottom:20px;position:relative;}
-    #footer .links a {color:#999999;}
-    #footer .links {text-align:center;}
-    #footer .links .pipe {color:#cccccc;}
-    #footer .copyright {color:#6b6b6b;text-align:center;margin-top:6px;}
-	</style>
-</head>
-<body>
-<div id="main">
-    <div id="content">
-        <div class="content">
-            <h1>Your Site has been created!</h1>
-            <p>Your website has been successfully installed on the server! Please create the file <b>index</b> from the <b>pages</b> </p>
-            <div class="bottom"></div>
-            <div class="clear"></div></div>
-        <div class="clear"></div></div>
-    <div class="clear"></div></div>
-<div id="footer">
-    <div class="links">
-        <a href="https://bigsansar.com" target="_blank">Free Hosting</a>
-        <span class="pipe">|</span>
-        <a href="https://bigsansar.com/login" target="_blank">Login</a>
-        <span class="pipe">|</span>
-        <a href="http://www.facebook.com/bigsansar" target="_blank">Find on Facebook</a>
-    </div>
-    <div class="copyright">Copyright &copy; Bigsansar.com <?php echo date(Y);?>. All rights reserved</div>
-</div>
-</div>
-</body>
-</html>
+<html>
+<head>
+    <title>Website created successfully - Hosted by bigsansar.com</title>
+    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
+    <style type="text/css">
+    .clear {display:inline-block;}
+    .clear:after {content:" ";display:block;height:0;clear:both;overflow:hidden;visibility:hidden;}
+    .clear {display:block;}
+    body {background-color:#f9f9f9;font-family:Tahoma,Geneva,Kalimati,sans-serif;}
+    img {border:none;}
+    #content {width:963px; margin-left:auto;margin-right:auto;margin-top:90px;}
+    #logo {top:36px;left:55px;position:absolute;display:block;width:auto;height:auto;}
+    #content .content {background: #6b6b6b  repeat-y 7px top; margin:0;position:relative;float:left;width:961px;background-size:99%;height:300px;}
+    h1 {font-size:40px;text-align:center;font-weight:700;color:white;margin-top:130px;}
+    #content p {color:#ffffff;font-size:15px;padding:0 69px;}
+    #footer {clear:both;font-size:11px;color:#999999;width:961px;margin-left:auto;margin-right:auto;margin-top:25px;margin-bottom:20px;position:relative;}
+    #footer .links a {color:#999999;}
+    #footer .links {text-align:center;}
+    #footer .links .pipe {color:#cccccc;}
+    #footer .copyright {color:#6b6b6b;text-align:center;margin-top:6px;}
+	</style>
+</head>
+<body>
+<div id="main">
+    <div id="content">
+        <div class="content">
+            <h1>Your Page has been created!</h1>
+            <p>Your Page has been successfully installed on the server! Please Edit the file <b>{{ path }}</b> from the <b>pages</b> </p>
+            <div class="bottom"></div>
+            <div class="clear"></div></div>
+        <div class="clear"></div></div>
+    <div class="clear"></div></div>
+<div id="footer">
+    <div class="links">
+        <a href="https://bigsansar.com" target="_blank">Free Hosting</a>
+        <span class="pipe">|</span>
+        <a href="https://bigsansar.com/login" target="_blank">Login</a>
+        <span class="pipe">|</span>
+        <a href="http://www.facebook.com/bigsansar" target="_blank">Find on Facebook</a>
+    </div>
+    <div class="copyright">Copyright &copy; Bigsansar.com <?php echo date(Y);?>. All rights reserved</div>
+</div>
+</div>
+</body>
+</html>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
-****** Your Site has been created! ******
-Your website has been successfully installed on the server! Please create the
-file index from the pages
+****** Your Page has been created! ******
+Your Page has been successfully installed on the server! Please Edit the file {
+{ path }} from the pages
 Free_Hosting | Login | Find_on_Facebook
 Copyright © Bigsansar.com <?php echo date(Y);?>. All rights reserved
```

### Comparing `Bigsansar-0.9.9/bigsansar/templates/parking.html` & `Bigsansar-1.0.0/bigsansar/templates/parking.html`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-
-{% extends 'base.html' %}
-
-{% block head %}
-<style>
-body
-{
-  padding-top: 10%;
-  background: #eee;
-}
-</style>
-{% endblock %}
-
-{% block body %}
-
-<div class="container">
-  <div class="card text-center">
-  <div class="card-header">
-    Free Website and Hosting
-  </div>
-  <div class="card-body">
-    <h5 class="card-title">Welcome {{ domain }}</h5>
-    <p class="card-text">Build one in minutes with bigsansar - a visual site building tool!
-    <br/>This domain is Parked with Bigsansar. If this is your domain, please register first.
-</p>
-    <a href="https://bigsansar.com/login" class="btn btn-primary">Start With Free</a>
-  </div>
-  <div class="card-footer text-muted">
-    {{ time }}
-  </div>
-</div>
-</div>
-
+
+{% extends 'base.html' %}
+
+{% block head %}
+<style>
+body
+{
+  padding-top: 10%;
+  background: #eee;
+}
+</style>
+{% endblock %}
+
+{% block body %}
+
+<div class="container">
+  <div class="card text-center">
+  <div class="card-header">
+    Free Website and Hosting
+  </div>
+  <div class="card-body">
+    <h5 class="card-title">Welcome {{ domain }}</h5>
+    <p class="card-text">Build one in minutes with bigsansar - a visual site building tool!
+    <br/>This domain is Parked with Bigsansar. If this is your domain, please register first.
+</p>
+    <a href="https://bigsansar.com/login" class="btn btn-primary">Start With Free</a>
+  </div>
+  <div class="card-footer text-muted">
+    {{ time }}
+  </div>
+</div>
+</div>
+
 {% endblock %}
```

### Comparing `Bigsansar-0.9.9/bigsansar/urls.py` & `Bigsansar-1.0.0/bigsansar/urls.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""www URL Configuration
-
-The `urlpatterns` list routes URLs to views. For more information please see:
-    https://docs.djangoproject.com/en/4.0/topics/http/urls/
-Examples:
-Function views
-    1. Add an import:  from my_app import views
-    2. Add a URL to urlpatterns:  path('', views.home, name='home')
-Class-based views
-    1. Add an import:  from other_app.views import Home
-    2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
-Including another URLconf
-    1. Import the include() function: from django.urls import include, path
-    2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
-"""
-
-from django.urls import path
-
-from bigsansar import views
-
-urlpatterns = [
-    path('', views.index, name='index'),
-    path('<url>', views.pathviews, name='path'),
-
-]
+"""www URL Configuration
+
+The `urlpatterns` list routes URLs to views. For more information please see:
+    https://docs.djangoproject.com/en/4.0/topics/http/urls/
+Examples:
+Function views
+    1. Add an import:  from my_app import views
+    2. Add a URL to urlpatterns:  path('', views.home, name='home')
+Class-based views
+    1. Add an import:  from other_app.views import Home
+    2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
+Including another URLconf
+    1. Import the include() function: from django.urls import include, path
+    2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
+"""
+
+from django.urls import path
+
+from bigsansar import views
+
+urlpatterns = [
+    path('', views.index, name='index'),
+    path('<url>', views.pathviews, name='path'),
+
+]
```

### Comparing `Bigsansar-0.9.9/bigsansar/views.py` & `Bigsansar-1.0.0/bigsansar/views.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import datetime
-import os
-from www.settings import BASE_DIR
-from django.contrib.sites.shortcuts import get_current_site
-from django.http import HttpResponse
-from django.shortcuts import render
-from django.template import loader
-
-from bigsansar.contrib.sites.models import domains, pages
-
-DEFAULT_TEMPLATE = 'default.html'
-
-
-def index(request):
-    try:
-        current_site = get_current_site(request)
-        db = domains.objects.get(domain=current_site)
-        total = db.visitor + 1
-        domains.objects.filter(pk=db.id).update(visitor=total)
-
-
-    except:
-        current_site = get_current_site(request)
-        time = datetime.datetime.now()
-        return render(request, 'parking.html', {'domain': current_site, 'time': time})
-
-    else:
-        asp = 'home/' + str(db.user) + '/' + str(current_site) + '/' + 'index.html'
-        full_url = os.path.join(BASE_DIR, asp)
-        template = loader.select_template((full_url, DEFAULT_TEMPLATE))
-
-        return HttpResponse(template.render({}, request))
-
-
-def pathviews(request, url):
-    default_page = 'defaultpage.html'
-
-    try:
-        current_site = get_current_site(request)
-        db = domains.objects.get(domain=current_site)
-        get_pagename = url.strip('/')
-        page = pages.objects.get(domain=db, slug=get_pagename)
-        total = db.visitor + 1
-        pagetotal = page.visitor + 1
-        domains.objects.filter(pk=db.id).update(visitor=total)
-        pages.objects.filter(domain=db, slug=get_pagename).update(visitor=pagetotal)
-
-    except:
-
-        return render(request, '404.html')
-
-    else:
-        asp = 'home/' + str(db.user) + '/' + str(current_site) + '/' + page.slug + '.html'
-        full_url = os.path.join(BASE_DIR, asp)
-        template = loader.select_template((full_url, default_page))
-        return HttpResponse(template.render({'path': url}, request))
+import datetime
+import os
+from www.settings import BASE_DIR
+from django.contrib.sites.shortcuts import get_current_site
+from django.http import HttpResponse
+from django.shortcuts import render
+from django.template import loader
+
+from bigsansar.contrib.sites.models import domains, pages
+
+DEFAULT_TEMPLATE = 'default.html'
+
+
+def index(request):
+    try:
+        current_site = get_current_site(request)
+        db = domains.objects.get(domain=current_site)
+        total = db.visitor + 1
+        domains.objects.filter(pk=db.id).update(visitor=total)
+
+
+    except:
+        current_site = get_current_site(request)
+        time = datetime.datetime.now()
+        return render(request, 'parking.html', {'domain': current_site, 'time': time})
+
+    else:
+        asp = 'home/' + str(db.user) + '/' + str(current_site) + '/' + 'index.html'
+        full_url = os.path.join(BASE_DIR, asp)
+        template = loader.select_template((full_url, DEFAULT_TEMPLATE))
+
+        return HttpResponse(template.render({}, request))
+
+
+def pathviews(request, url):
+    default_page = 'defaultpage.html'
+
+    try:
+        current_site = get_current_site(request)
+        db = domains.objects.get(domain=current_site)
+        get_pagename = url.strip('/')
+        page = pages.objects.get(domain=db, slug=get_pagename)
+        total = db.visitor + 1
+        pagetotal = page.visitor + 1
+        domains.objects.filter(pk=db.id).update(visitor=total)
+        pages.objects.filter(domain=db, slug=get_pagename).update(visitor=pagetotal)
+
+    except:
+
+        return render(request, '404.html')
+
+    else:
+        asp = 'home/' + str(db.user) + '/' + str(current_site) + '/' + page.slug + '.html'
+        full_url = os.path.join(BASE_DIR, asp)
+        template = loader.select_template((full_url, default_page))
+        return HttpResponse(template.render({'path': url}, request))
```

### Comparing `Bigsansar-0.9.9/setup.py` & `Bigsansar-1.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="Bigsansar",
-    version="0.9.9",
-    author="Bikash Pokhrel",
-    author_email="bigsansaroffice@gmail.com",
-    description="Build one in minutes with bigsansar - a visual site building tool!",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://bigsansar.com",
-    project_urls={
-        "Bug Tracker": "https://github.com/pokhrelb9/bigsansar/issues",
-        "Documentations": "https://docs.bigsansar.com/"
-    },
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-
-    packages=setuptools.find_packages(),
-    package_data={'': ['templates/*', 'static/*']},
-
-    entry_points={
-        'console_scripts': [
-                    'bigsansar = bigsansar.core:main',
-                ],
-    },
-
-    python_requires=">=3.6",
-    install_requires=['django', 'django-phonenumber-field[phonenumberslite]', 'django-ckeditor', 'requests', 'pillow'],
-    keywords=['python', 'django host', 'bigsansar', 'django', 'django sites framework', 'django flatpages']
-)
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="Bigsansar",
+    version="1.0.0",
+    author="Bikash Pokhrel",
+    author_email="bigsansaroffice@gmail.com",
+    description="Build one in minutes with bigsansar - a visual site building tool!",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://bigsansar.com",
+    project_urls={
+        "Bug Tracker": "https://github.com/pokhrelb9/bigsansar/issues",
+        "Documentations": "https://docs.bigsansar.com/"
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+
+    packages=setuptools.find_packages(),
+    package_data={'': ['templates/*', 'static/*']},
+
+    entry_points={
+        'console_scripts': [
+                    'bigsansar = bigsansar.core:main',
+                ],
+    },
+
+    python_requires=">=3.6",
+    install_requires=['django', 'django-phonenumber-field[phonenumberslite]', 'django-ckeditor', 'requests', 'pillow'],
+    keywords=['python', 'django host', 'bigsansar', 'django', 'django sites framework', 'django flatpages']
+)
```


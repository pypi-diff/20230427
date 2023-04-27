# Comparing `tmp/django-cas-nge-4.3.2.tar.gz` & `tmp/django-cas-nge-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cas-nge-4.3.2.tar", last modified: Thu Apr 27 07:08:27 2023, max compression
+gzip compressed data, was "django-cas-nge-4.3.3.tar", last modified: Thu Apr 27 08:56:08 2023, max compression
```

## Comparing `django-cas-nge-4.3.2.tar` & `django-cas-nge-4.3.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.399348 django-cas-nge-4.3.2/
--rw-r--r--   0 huangjianglin   (501) staff       (20)     1050 2023-04-27 06:20:33.000000 django-cas-nge-4.3.2/LICENSE.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)       60 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/MANIFEST.in
--rw-r--r--   0 huangjianglin   (501) staff       (20)      470 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/Makefile
--rw-r--r--   0 huangjianglin   (501) staff       (20)     4034 2023-04-27 07:08:27.399499 django-cas-nge-4.3.2/PKG-INFO
--rw-r--r--   0 huangjianglin   (501) staff       (20)     2638 2023-04-27 06:58:20.000000 django-cas-nge-4.3.2/README.rst
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.386714 django-cas-nge-4.3.2/django_cas_ng/
--rw-r--r--   0 huangjianglin   (501) staff       (20)     1494 2023-04-26 09:49:54.000000 django-cas-nge-4.3.2/django_cas_ng/__init__.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)      145 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/apps.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)     8465 2023-04-26 09:48:03.000000 django-cas-nge-4.3.2/django_cas_ng/backends.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)     2070 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/decorators.py
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.373686 django-cas-nge-4.3.2/django_cas_ng/locale/
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.372122 django-cas-nge-4.3.2/django_cas_ng/locale/ca/
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.387103 django-cas-nge-4.3.2/django_cas_ng/locale/ca/LC_MESSAGES/
--rw-r--r--   0 huangjianglin   (501) staff       (20)     1106 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.372494 django-cas-nge-4.3.2/django_cas_ng/locale/de/
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.387468 django-cas-nge-4.3.2/django_cas_ng/locale/de/LC_MESSAGES/
--rw-r--r--   0 huangjianglin   (501) staff       (20)      871 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.372842 django-cas-nge-4.3.2/django_cas_ng/locale/es/
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.387851 django-cas-nge-4.3.2/django_cas_ng/locale/es/LC_MESSAGES/
--rw-r--r--   0 huangjianglin   (501) staff       (20)     1111 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.373202 django-cas-nge-4.3.2/django_cas_ng/locale/fr/
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.388233 django-cas-nge-4.3.2/django_cas_ng/locale/fr/LC_MESSAGES/
--rw-r--r--   0 huangjianglin   (501) staff       (20)      863 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.373507 django-cas-nge-4.3.2/django_cas_ng/locale/ru/
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.389702 django-cas-nge-4.3.2/django_cas_ng/locale/ru/LC_MESSAGES/
--rw-r--r--   0 huangjianglin   (501) staff       (20)     1192 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.373803 django-cas-nge-4.3.2/django_cas_ng/locale/ua/
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.390114 django-cas-nge-4.3.2/django_cas_ng/locale/ua/LC_MESSAGES/
--rw-r--r--   0 huangjianglin   (501) staff       (20)     1178 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/locale/ua/LC_MESSAGES/django.po
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.390667 django-cas-nge-4.3.2/django_cas_ng/management/
--rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/management/__init__.py
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.391164 django-cas-nge-4.3.2/django_cas_ng/management/commands/
--rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/management/commands/__init__.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)      359 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/management/commands/django_cas_ng_clean_sessions.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)     2509 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/middleware.py
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.392905 django-cas-nge-4.3.2/django_cas_ng/migrations/
--rw-r--r--   0 huangjianglin   (501) staff       (20)     1559 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/migrations/0001_initial.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)      590 2023-04-26 09:45:33.000000 django-cas-nge-4.3.2/django_cas_ng/migrations/0002_auto_20201023_1400.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)      401 2023-04-26 09:45:51.000000 django-cas-nge-4.3.2/django_cas_ng/migrations/0003_auto_20210813_1226.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/migrations/__init__.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)     2737 2023-04-26 09:47:10.000000 django-cas-nge-4.3.2/django_cas_ng/models.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/py.typed
--rw-r--r--   0 huangjianglin   (501) staff       (20)      218 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/signals.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)     4411 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/utils.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)    10856 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/django_cas_ng/views.py
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.396012 django-cas-nge-4.3.2/django_cas_nge.egg-info/
--rw-r--r--   0 huangjianglin   (501) staff       (20)     4034 2023-04-27 07:08:27.000000 django-cas-nge-4.3.2/django_cas_nge.egg-info/PKG-INFO
--rw-r--r--   0 huangjianglin   (501) staff       (20)     1333 2023-04-27 07:08:27.000000 django-cas-nge-4.3.2/django_cas_nge.egg-info/SOURCES.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)        1 2023-04-27 07:08:27.000000 django-cas-nge-4.3.2/django_cas_nge.egg-info/dependency_links.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)        1 2023-04-27 03:34:00.000000 django-cas-nge-4.3.2/django_cas_nge.egg-info/not-zip-safe
--rw-r--r--   0 huangjianglin   (501) staff       (20)       30 2023-04-27 07:08:27.000000 django-cas-nge-4.3.2/django_cas_nge.egg-info/requires.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)       14 2023-04-27 07:08:27.000000 django-cas-nge-4.3.2/django_cas_nge.egg-info/top_level.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)      110 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/requirements-dev.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)      176 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/requirements.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)      294 2023-04-27 07:08:27.400104 django-cas-nge-4.3.2/setup.cfg
--rwxr-xr-x   0 huangjianglin   (501) staff       (20)     2048 2023-04-27 07:08:21.000000 django-cas-nge-4.3.2/setup.py
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 07:08:27.399002 django-cas-nge-4.3.2/tests/
--rw-r--r--   0 huangjianglin   (501) staff       (20)    16858 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/tests/test_backend.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)     2299 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/tests/test_commands.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)     1220 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/tests/test_middleware.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)     6982 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/tests/test_signals.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)      336 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/tests/test_smoke.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)     5968 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/tests/test_utils.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)    17529 2023-04-26 03:13:09.000000 django-cas-nge-4.3.2/tests/test_views.py
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.318395 django-cas-nge-4.3.3/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     1050 2023-04-27 06:20:33.000000 django-cas-nge-4.3.3/LICENSE.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)       60 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/MANIFEST.in
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      470 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/Makefile
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     4029 2023-04-27 08:56:08.318542 django-cas-nge-4.3.3/PKG-INFO
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     2638 2023-04-27 06:58:20.000000 django-cas-nge-4.3.3/README.rst
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.305624 django-cas-nge-4.3.3/django_cas_ng/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     1494 2023-04-26 09:49:54.000000 django-cas-nge-4.3.3/django_cas_ng/__init__.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      145 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/apps.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     8465 2023-04-26 09:48:03.000000 django-cas-nge-4.3.3/django_cas_ng/backends.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     2070 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/decorators.py
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.297805 django-cas-nge-4.3.3/django_cas_ng/locale/
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.296251 django-cas-nge-4.3.3/django_cas_ng/locale/ca/
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.305967 django-cas-nge-4.3.3/django_cas_ng/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     1106 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.296603 django-cas-nge-4.3.3/django_cas_ng/locale/de/
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.306495 django-cas-nge-4.3.3/django_cas_ng/locale/de/LC_MESSAGES/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      871 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.296950 django-cas-nge-4.3.3/django_cas_ng/locale/es/
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.307354 django-cas-nge-4.3.3/django_cas_ng/locale/es/LC_MESSAGES/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     1111 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.297316 django-cas-nge-4.3.3/django_cas_ng/locale/fr/
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.308349 django-cas-nge-4.3.3/django_cas_ng/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      863 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.297629 django-cas-nge-4.3.3/django_cas_ng/locale/ru/
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.308845 django-cas-nge-4.3.3/django_cas_ng/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     1192 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.297922 django-cas-nge-4.3.3/django_cas_ng/locale/ua/
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.309202 django-cas-nge-4.3.3/django_cas_ng/locale/ua/LC_MESSAGES/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     1178 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/locale/ua/LC_MESSAGES/django.po
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.309618 django-cas-nge-4.3.3/django_cas_ng/management/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/management/__init__.py
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.310150 django-cas-nge-4.3.3/django_cas_ng/management/commands/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/management/commands/__init__.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      359 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/management/commands/django_cas_ng_clean_sessions.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     2509 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/middleware.py
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.312069 django-cas-nge-4.3.3/django_cas_ng/migrations/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     1559 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/migrations/0001_initial.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      590 2023-04-26 09:45:33.000000 django-cas-nge-4.3.3/django_cas_ng/migrations/0002_auto_20201023_1400.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      401 2023-04-26 09:45:51.000000 django-cas-nge-4.3.3/django_cas_ng/migrations/0003_auto_20210813_1226.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/migrations/__init__.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     2737 2023-04-26 09:47:10.000000 django-cas-nge-4.3.3/django_cas_ng/models.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/py.typed
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      218 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/signals.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     4411 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/utils.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)    10856 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/django_cas_ng/views.py
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.315553 django-cas-nge-4.3.3/django_cas_nge.egg-info/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     4029 2023-04-27 08:56:08.000000 django-cas-nge-4.3.3/django_cas_nge.egg-info/PKG-INFO
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     1333 2023-04-27 08:56:08.000000 django-cas-nge-4.3.3/django_cas_nge.egg-info/SOURCES.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)        1 2023-04-27 08:56:08.000000 django-cas-nge-4.3.3/django_cas_nge.egg-info/dependency_links.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)        1 2023-04-27 03:34:00.000000 django-cas-nge-4.3.3/django_cas_nge.egg-info/not-zip-safe
+-rw-r--r--   0 huangjianglin   (501) staff       (20)       30 2023-04-27 08:56:08.000000 django-cas-nge-4.3.3/django_cas_nge.egg-info/requires.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)       14 2023-04-27 08:56:08.000000 django-cas-nge-4.3.3/django_cas_nge.egg-info/top_level.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      110 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/requirements-dev.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      176 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/requirements.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      294 2023-04-27 08:56:08.319120 django-cas-nge-4.3.3/setup.cfg
+-rwxr-xr-x   0 huangjianglin   (501) staff       (20)     2043 2023-04-27 08:55:55.000000 django-cas-nge-4.3.3/setup.py
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-04-27 08:56:08.318085 django-cas-nge-4.3.3/tests/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)    16858 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/tests/test_backend.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     2299 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/tests/test_commands.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     1220 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/tests/test_middleware.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     6982 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/tests/test_signals.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      336 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/tests/test_smoke.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     5968 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/tests/test_utils.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)    17529 2023-04-26 03:13:09.000000 django-cas-nge-4.3.3/tests/test_views.py
```

### Comparing `django-cas-nge-4.3.2/LICENSE.txt` & `django-cas-nge-4.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/PKG-INFO` & `django-cas-nge-4.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-cas-nge
-Version: 4.3.2
+Version: 4.3.3
 Summary: Django CAS 1.0/2.0/3.0 client authentication library, support Django 2.2, 3.0, 3.1, 3.2, 4.0 and Python 3.7+
 Home-page: https://djangocas.dev
-Download-URL: https://github.com/django-cas-ng/django-cas-ng/releases
+Download-URL: https://github.com/tacnaci/django-cas-nge/releases
 Author: Joneai
 Author-email: mxjoneai@gmail.com
 License: BSD
 Keywords: django,cas,cas2,cas3,client,sso,single sign-on,Central Authentication Service,authentication,auth
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-cas-nge-4.3.2/README.rst` & `django-cas-nge-4.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/__init__.py` & `django-cas-nge-4.3.3/django_cas_ng/__init__.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/backends.py` & `django-cas-nge-4.3.3/django_cas_ng/backends.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/decorators.py` & `django-cas-nge-4.3.3/django_cas_ng/decorators.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/locale/ca/LC_MESSAGES/django.po` & `django-cas-nge-4.3.3/django_cas_ng/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/locale/de/LC_MESSAGES/django.po` & `django-cas-nge-4.3.3/django_cas_ng/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/locale/es/LC_MESSAGES/django.po` & `django-cas-nge-4.3.3/django_cas_ng/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/locale/fr/LC_MESSAGES/django.po` & `django-cas-nge-4.3.3/django_cas_ng/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/locale/ru/LC_MESSAGES/django.po` & `django-cas-nge-4.3.3/django_cas_ng/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/locale/ua/LC_MESSAGES/django.po` & `django-cas-nge-4.3.3/django_cas_ng/locale/ua/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/middleware.py` & `django-cas-nge-4.3.3/django_cas_ng/middleware.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/migrations/0001_initial.py` & `django-cas-nge-4.3.3/django_cas_ng/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/migrations/0002_auto_20201023_1400.py` & `django-cas-nge-4.3.3/django_cas_ng/migrations/0002_auto_20201023_1400.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/models.py` & `django-cas-nge-4.3.3/django_cas_ng/models.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/utils.py` & `django-cas-nge-4.3.3/django_cas_ng/utils.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_ng/views.py` & `django-cas-nge-4.3.3/django_cas_ng/views.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/django_cas_nge.egg-info/PKG-INFO` & `django-cas-nge-4.3.3/django_cas_nge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-cas-nge
-Version: 4.3.2
+Version: 4.3.3
 Summary: Django CAS 1.0/2.0/3.0 client authentication library, support Django 2.2, 3.0, 3.1, 3.2, 4.0 and Python 3.7+
 Home-page: https://djangocas.dev
-Download-URL: https://github.com/django-cas-ng/django-cas-ng/releases
+Download-URL: https://github.com/tacnaci/django-cas-nge/releases
 Author: Joneai
 Author-email: mxjoneai@gmail.com
 License: BSD
 Keywords: django,cas,cas2,cas3,client,sso,single sign-on,Central Authentication Service,authentication,auth
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-cas-nge-4.3.2/django_cas_nge.egg-info/SOURCES.txt` & `django-cas-nge-4.3.3/django_cas_nge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/setup.py` & `django-cas-nge-4.3.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     package_data={
         'django_cas_ng': [
             'locale/*/LC_MESSAGES/*',
             'py.typed',
         ],
     },
     url='https://djangocas.dev',
-    download_url='https://github.com/django-cas-ng/django-cas-ng/releases',
-    version='4.3.2',
+    download_url='https://github.com/tacnaci/django-cas-nge/releases',
+    version='4.3.3',
     python_requires=">=3.7",
     install_requires=[
         'Django>=2.2',
         'python-cas>=1.6.0',
     ],
     zip_safe=False,  # dot not package as egg or django will not found management commands
 )
```

### Comparing `django-cas-nge-4.3.2/tests/test_backend.py` & `django-cas-nge-4.3.3/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/tests/test_commands.py` & `django-cas-nge-4.3.3/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/tests/test_middleware.py` & `django-cas-nge-4.3.3/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/tests/test_signals.py` & `django-cas-nge-4.3.3/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/tests/test_utils.py` & `django-cas-nge-4.3.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-cas-nge-4.3.2/tests/test_views.py` & `django-cas-nge-4.3.3/tests/test_views.py`

 * *Files identical despite different names*


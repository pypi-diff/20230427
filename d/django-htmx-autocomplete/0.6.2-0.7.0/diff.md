# Comparing `tmp/django-htmx-autocomplete-0.6.2.tar.gz` & `tmp/django-htmx-autocomplete-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-autocomplete-0.6.2.tar", last modified: Tue Mar 14 18:32:29 2023, max compression
+gzip compressed data, was "django-htmx-autocomplete-0.7.0.tar", last modified: Thu Apr 27 16:43:18 2023, max compression
```

## Comparing `django-htmx-autocomplete-0.6.2.tar` & `django-htmx-autocomplete-0.7.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.798344 django-htmx-autocomplete-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-03-14 18:32:29.798344 django-htmx-autocomplete-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.794343 django-htmx-autocomplete-0.6.2/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    25175 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/autocomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.790343 django-htmx-autocomplete-0.6.2/autocomplete/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.790343 django-htmx-autocomplete-0.6.2/autocomplete/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.794343 django-htmx-autocomplete-0.6.2/autocomplete/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-14 18:32:29.000000 django-htmx-autocomplete-0.6.2/autocomplete/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.790343 django-htmx-autocomplete-0.6.2/autocomplete/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.794343 django-htmx-autocomplete-0.6.2/autocomplete/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-14 18:32:29.000000 django-htmx-autocomplete-0.6.2/autocomplete/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.790343 django-htmx-autocomplete-0.6.2/autocomplete/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.790343 django-htmx-autocomplete-0.6.2/autocomplete/static/autocomplete/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.794343 django-htmx-autocomplete-0.6.2/autocomplete/static/autocomplete/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/static/autocomplete/css/autocomplete.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.794343 django-htmx-autocomplete-0.6.2/autocomplete/static/autocomplete/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/static/autocomplete/js/autocomplete.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.790343 django-htmx-autocomplete-0.6.2/autocomplete/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.794343 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/ac_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/chip.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/chip_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/component.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/head.html
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/indicator-icon.html
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/item.html
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/item_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/scripts.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.798344 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/strings/available_results.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/strings/backspace_instruction.html
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/strings/item_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/strings/more_results.html
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/strings/multiselect.html
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/strings/no_results.html
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/strings/nothing_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/strings/selected.html
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/textinput.html
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/values.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.798344 django-htmx-autocomplete-0.6.2/autocomplete/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/templatetags/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/test_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/autocomplete/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:32:29.798344 django-htmx-autocomplete-0.6.2/django_htmx_autocomplete.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-03-14 18:32:29.000000 django-htmx-autocomplete-0.6.2/django_htmx_autocomplete.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-14 18:32:29.000000 django-htmx-autocomplete-0.6.2/django_htmx_autocomplete.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:32:29.000000 django-htmx-autocomplete-0.6.2/django_htmx_autocomplete.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-14 18:32:29.000000 django-htmx-autocomplete-0.6.2/django_htmx_autocomplete.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-14 18:32:29.000000 django-htmx-autocomplete-0.6.2/django_htmx_autocomplete.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-14 18:32:29.798344 django-htmx-autocomplete-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-14 18:32:01.000000 django-htmx-autocomplete-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.288826 django-htmx-autocomplete-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-27 16:43:18.288826 django-htmx-autocomplete-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.280826 django-htmx-autocomplete-0.7.0/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25303 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/autocomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.280826 django-htmx-autocomplete-0.7.0/autocomplete/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/autocomplete/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.280826 django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.280826 django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/css/autocomplete.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.280826 django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/js/autocomplete.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.284826 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/ac_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/chip.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/chip_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/component.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/indicator-icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/item_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/scripts.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.284826 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/available_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/backspace_instruction.html
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/item_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/more_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/multiselect.html
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/no_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/nothing_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/textinput.html
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/values.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.288826 django-htmx-autocomplete-0.7.0/autocomplete/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templatetags/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/test_autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.288826 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-27 16:43:18.288826 django-htmx-autocomplete-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/setup.py
```

### Comparing `django-htmx-autocomplete-0.6.2/LICENSE` & `django-htmx-autocomplete-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/PKG-INFO` & `django-htmx-autocomplete-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-autocomplete
-Version: 0.6.2
+Version: 0.7.0
 Summary: A Django autocomplete component powered by htmx
 Home-page: https://github.com/PHACDataHub/django-htmx-autocomplete
 Author: Luc Belliveau
 Author-email: luc.belliveau@canada.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.6.2 Summary: A
+Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.7.0 Summary: A
 Django autocomplete component powered by htmx Home-page: https://github.com/
 PHACDataHub/django-htmx-autocomplete Author: Luc Belliveau Author-email:
 luc.belliveau@canada.ca License: MIT Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `django-htmx-autocomplete-0.6.2/README.md` & `django-htmx-autocomplete-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/autocomplete.py` & `django-htmx-autocomplete-0.7.0/autocomplete/autocomplete.py`

 * *Files 2% similar despite different names*

```diff
@@ -473,14 +473,15 @@
                     update the selected style of the option if it is currently
                     in the dropdown list)
 
         """
         data = QueryDict(request.body)
         items_selected = data.getlist(self.name)
         override_component_id = data.get("component_id", "")
+        component_name = data.get("name", self.name)
 
         if items_selected == [""]:
             items_selected = []
 
         items_selected = [a for a in items_selected if a not in self.strip_values]
 
         if method == "toggle":
@@ -518,15 +519,15 @@
                         item["selected"] = False
 
 
             template = loader.get_template("autocomplete/item.html")
             return HttpResponse(
                 template.render(
                     {
-                        "name": self.name,
+                        "name": component_name,
                         "search": "",
                         "indicator": self.indicator,
                         "placeholder": self.placeholder,
                         "required": self.required,
                         "custom_strings": self.custom_strings,
                         "route_name": self.get_route_name(),
                         "component_id": self.get_component_id(override_component_id),
@@ -588,23 +589,24 @@
                     items (dict[]): List of items
         """
         items_selected = request.GET.getlist(self.name)
         if items_selected == [""]:
             items_selected = []
 
         override_component_id = request.GET.get("component_id", "")
+        component_name = request.GET.get("name", self.name)
 
         if method == "component":
             template = loader.get_template("autocomplete/component.html")
             selected_options = self.map_items(self.get_items(values=items_selected))
 
             return HttpResponse(
                 template.render(
                     {
-                        "name": self.name,
+                        "name": component_name,
                         "disabled": self.disabled,
                         "required": self.required,
                         "indicator": self.indicator,
                         "route_name": self.get_route_name(),
                         "component_id": self.get_component_id(override_component_id),
                         "label": self.label,
                         "placeholder": self.placeholder,
@@ -627,15 +629,15 @@
             total_results = len(items)
             if self.max_results is not None and len(items) > self.max_results:
                 items = items[: self.max_results]
 
             return HttpResponse(
                 template.render(
                     {
-                        "name": self.name,
+                        "name": component_name,
                         "required": self.required,
                         "placeholder": self.placeholder,
                         "indicator": self.indicator,
                         "custom_strings": self.custom_strings,
                         "multiselect": self.multiselect,
                         "route_name": self.get_route_name(),
                         "component_id": self.get_component_id(override_component_id),
```

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/locale/en/LC_MESSAGES/django.po` & `django-htmx-autocomplete-0.7.0/autocomplete/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/locale/fr/LC_MESSAGES/django.mo` & `django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/locale/fr/LC_MESSAGES/django.po` & `django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/static/autocomplete/css/autocomplete.css` & `django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/static/autocomplete/js/autocomplete.js` & `django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/ac_container.html` & `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/ac_container.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/chip.html` & `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/chip.html`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 {% endcomment %}
 
 <li class="chip" aria-hidden="true">
     <span>{{ item.label }}</span>
     {% if not disabled %}
     <a
         hx-put="{% url route_name method='toggle' %}"
-        hx-params="{{ name }},item,remove,component_id"
-        hx-vals='{"component_id": "{{ component_id|escapejs }}", "remove": true, "item": "{{ item.value|escapejs }}"}'
+        hx-params="{{ name }},name,item,remove,component_id"
+        hx-vals='{"name": "{{ name|escapejs }}", "component_id": "{{ component_id|escapejs }}", "remove": true, "item": "{{ item.value|escapejs }}"}'
         hx-include="#{{ component_id }}"
         hx-swap="delete"
         tabindex="-1"
         href="#"
     >
         <svg focusable="false" viewBox="0 0 24 24" width="0" height="0">
             <path
```

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/component.html` & `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/component.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/head.html` & `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/head.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/indicator-icon.html` & `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/indicator-icon.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/item.html` & `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/item.html`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,17 @@
     tabindex="-1"
     id="{{ component_id }}__item__{{ item.value|make_id }}"
     class="item {{ item.selected|yesno:'selected,' }}"
     aria-selected="{{ item.selected|yesno:'true,false' }}"
     onclick="return phac_aspc_autocomplete_item_click_handler(event)"
     href="#"
     hx-put="{% url route_name method='toggle' %}"
-    hx-params="{{ name }},item,component_id"
+    hx-params="{{ name }},name,item,component_id"
     hx-include="#{{ component_id }}"
-    hx-vals='{"component_id": "{{ component_id|escapejs }}", "item": "{{ item.value|escapejs }}"}'
+    hx-vals='{"name": "{{ name|escapejs }}", "component_id": "{{ component_id|escapejs }}", "item": "{{ item.value|escapejs }}"}'
     hx-swap="outerHTML"
     {% if swap_oob %}
     hx-swap-oob="outerHTML:#{{ component_id }}__item__{{ item.value|make_id }}"
     {% endif %}
 >
     {{ item.label|search_highlight:search }}
 </a>
```

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/item_list.html` & `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/item_list.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/scripts.html` & `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/scripts.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/templates/autocomplete/textinput.html` & `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/textinput.html`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     onblur="return phac_aspc_autocomplete_blur_handler(event, '{{ component_id|escapejs }}', {{ multiselect|yesno:'false,true' }})"
     onfocus="return phac_aspc_autocomplete_focus_handler(event)"
 
     hx-get="{% url route_name method='items' %}"
     hx-trigger="phac_aspc_autocomplete_trigger"
     hx-include="#{{ component_id }}"
     hx-target="#{{ component_id }}__items"
-    hx-vals="js:{component_id: '{{ component_id|escapejs }}', search: document.getElementById('{{ component_id|escapejs }}__textinput').value}"
+    hx-vals="js:{name: '{{ name|escapejs}}', component_id: '{{ component_id|escapejs }}', search: document.getElementById('{{ component_id|escapejs }}__textinput').value}"
     hx-swap="outerHTML"
     {% if indicator %}
     hx-indicator="#{{ component_id }}__container .htmx-indicator"
     {% endif %}
     {% if swap_oob %}
     hx-swap-oob="outerHTML:#{{ component_id }}__textinput"
     {% endif %}
```

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/templatetags/autocomplete.py` & `django-htmx-autocomplete-0.7.0/autocomplete/templatetags/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/test_autocomplete.py` & `django-htmx-autocomplete-0.7.0/autocomplete/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/autocomplete/widgets.py` & `django-htmx-autocomplete-0.7.0/autocomplete/widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This file enables the component to be used like other Django widgets
 """
 from django.forms import Widget
 
 from .autocomplete import HTMXAutoComplete
 
+
 class Autocomplete(Widget):
     """
     Django forms compatible autocomplete widget
 
     Parameters:
 
         name (str):     The name of the component (must be unique)
@@ -83,15 +84,25 @@
             self.a_c = use_ac
 
     def value_from_datadict(self, data, files, name):
         try:
             getter = data.getlist
         except AttributeError:
             getter = data.get
-        return getter(name)
+        buf = getter(name)
+
+        if not self.a_c.multiselect:
+            try:
+                return buf[0]
+            except IndexError:
+                return -1
+            except TypeError:
+                pass
+
+        return buf
 
     def value_omitted_from_data(self, data, files, name):
         # An unselected <select multiple> doesn't appear in POST data, so it's
         # never known if the value is actually omitted.
         return []
 
     def get_context(self, name, value, attrs):
@@ -101,15 +112,15 @@
             [] if value is None else [value] if not isinstance(value, list) else value
         )
         selected_options = self.a_c.map_items(
             self.a_c,
             self.a_c.get_items(self.a_c, values=[str(x) for x in items_selected]),
         )
 
-        context["name"] = self.a_c.name
+        context["name"] = attrs.get("name", self.attrs.get("name", self.a_c.name))
 
         context["disabled"] = attrs.get("disabled", self.attrs.get("disabled", False))
         context["required"] = attrs.get("required", self.attrs.get("required", False))
 
         context["indicator"] = self.a_c.indicator
         context["route_name"] = self.a_c.get_route_name()
         context["component_id"] = self.a_c.get_component_id(
```

### Comparing `django-htmx-autocomplete-0.6.2/django_htmx_autocomplete.egg-info/PKG-INFO` & `django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-autocomplete
-Version: 0.6.2
+Version: 0.7.0
 Summary: A Django autocomplete component powered by htmx
 Home-page: https://github.com/PHACDataHub/django-htmx-autocomplete
 Author: Luc Belliveau
 Author-email: luc.belliveau@canada.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.6.2 Summary: A
+Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.7.0 Summary: A
 Django autocomplete component powered by htmx Home-page: https://github.com/
 PHACDataHub/django-htmx-autocomplete Author: Luc Belliveau Author-email:
 luc.belliveau@canada.ca License: MIT Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `django-htmx-autocomplete-0.6.2/django_htmx_autocomplete.egg-info/SOURCES.txt` & `django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.6.2/setup.cfg` & `django-htmx-autocomplete-0.7.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-htmx-autocomplete
-version = 0.6.2
+version = 0.7.0
 description = A Django autocomplete component powered by htmx
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/PHACDataHub/django-htmx-autocomplete
 author = Luc Belliveau
 author_email = luc.belliveau@canada.ca
 license = MIT
```

### Comparing `django-htmx-autocomplete-0.6.2/setup.py` & `django-htmx-autocomplete-0.7.0/setup.py`

 * *Files identical despite different names*


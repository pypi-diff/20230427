# Comparing `tmp/pretix-sepadebit-2.4.0.tar.gz` & `tmp/pretix-sepadebit-2.4.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sepadebit-2.4.0.tar", last modified: Tue Mar 28 08:19:19 2023, max compression
+gzip compressed data, was "pretix-sepadebit-2.4.0.post1.tar", last modified: Thu Apr 27 16:32:58 2023, max compression
```

## Comparing `pretix-sepadebit-2.4.0.tar` & `pretix-sepadebit-2.4.0.post1.tar`

### file list

```diff
@@ -1,134 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.730853 pretix-sepadebit-2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1199 2023-03-28 08:19:19.730853 pretix-sepadebit-2.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/apps.py
--rw-rw-rw-   0 root         (0) root         (0)   109251 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/bicdata.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/exporters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15987 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16372 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/da/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16052 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    23666 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    23666 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    15738 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16269 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16075 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16034 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16032 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16132 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    24127 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15716 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    24357 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16508 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15722 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.714852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.718852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pt_BR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16025 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.718852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.718852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15963 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.718852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15950 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.718852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16039 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.718852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/uk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/uk/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16095 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.718852 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16063 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0002_auto_20170530_1527.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0004_sepaexport_testmode.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0005_auto_20190429_0811.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0006_sepaexport_currency.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0007_sepaduedate.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/models.py
--rw-rw-rw-   0 root         (0) root         (0)    19281 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     9441 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.718852 pretix-sepadebit-2.4.0/pretix_sepadebit/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/static/pretix_sepadebit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/static/pretix_sepadebit/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.718852 pretix-sepadebit-2.4.0/pretix_sepadebit/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.726853 pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     1551 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)     1476 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/control.html
--rw-rw-rw-   0 root         (0) root         (0)     5782 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/export.html
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/mail.txt
--rw-rw-rw-   0 root         (0) root         (0)     3400 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/orders.html
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/pending.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.730853 pretix-sepadebit-2.4.0/pretix_sepadebit/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10539 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/tests/test_payment.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    12651 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/pretix_sepadebit/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:19:19.722853 pretix-sepadebit-2.4.0/pretix_sepadebit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1199 2023-03-28 08:19:19.000000 pretix-sepadebit-2.4.0/pretix_sepadebit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3055 2023-03-28 08:19:19.000000 pretix-sepadebit-2.4.0/pretix_sepadebit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 08:19:19.000000 pretix-sepadebit-2.4.0/pretix_sepadebit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-03-28 08:19:19.000000 pretix-sepadebit-2.4.0/pretix_sepadebit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-03-28 08:19:19.000000 pretix-sepadebit-2.4.0/pretix_sepadebit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-28 08:19:19.000000 pretix-sepadebit-2.4.0/pretix_sepadebit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-03-28 08:19:19.730853 pretix-sepadebit-2.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-03-28 08:18:37.000000 pretix-sepadebit-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.757506 pretix-sepadebit-2.4.0.post1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-04-27 16:32:58.757506 pretix-sepadebit-2.4.0.post1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)   109251 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/bicdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/exporters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15987 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16372 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16052 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    23666 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    23666 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    15738 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16269 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16075 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16034 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16032 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16132 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    24127 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15716 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    24357 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16508 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15722 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt_BR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16025 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15963 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15950 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16039 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/uk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/uk/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16095 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16063 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0002_auto_20170530_1527.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0004_sepaexport_testmode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0005_auto_20190429_0811.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0006_sepaexport_currency.py
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0007_sepaduedate.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    19281 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     9441 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/static/pretix_sepadebit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/static/pretix_sepadebit/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.757506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/control.html
+-rw-rw-rw-   0 root         (0) root         (0)     5782 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/export.html
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/mail.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3400 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/orders.html
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/pending.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.757506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10539 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/tests/test_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    12651 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      137 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-04-27 16:32:58.757506 pretix-sepadebit-2.4.0.post1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/setup.py
```

### Comparing `pretix-sepadebit-2.4.0/LICENSE` & `pretix-sepadebit-2.4.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/README.rst` & `pretix-sepadebit-2.4.0.post1/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/apps.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/bicdata.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/bicdata.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/exporters.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/exporters.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/da/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/de/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/django.pot` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/el/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/es/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/it/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/si/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0001_initial.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0002_auto_20170530_1527.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0002_auto_20170530_1527.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0005_auto_20190429_0811.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0005_auto_20190429_0811.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0007_sepaduedate.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0007_sepaduedate.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/models.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/models.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/payment.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/signals.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/control.html` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/control.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/export.html` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/export.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/templates/pretix_sepadebit/orders.html` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/orders.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/tests/test_payment.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/tests/test_payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/urls.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit/views.py` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/views.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0/pretix_sepadebit.egg-info/SOURCES.txt` & `pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_sepadebit/__init__.py
 pretix_sepadebit/apps.py
 pretix_sepadebit/bicdata.py
 pretix_sepadebit/exporters.py
 pretix_sepadebit/models.py
```


# Comparing `tmp/musif-1.1.0.tar.gz` & `tmp/musif-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musif-1.1.0.tar", last modified: Wed Apr 26 15:09:24 2023, max compression
+gzip compressed data, was "musif-1.1.1.tar", last modified: Thu Apr 27 15:37:01 2023, max compression
```

## Comparing `musif-1.1.0.tar` & `musif-1.1.1.tar`

### file list

```diff
@@ -1,94 +1,103 @@
--rw-r--r--   0        0        0      971 2023-04-24 10:50:21.848481 musif-1.1.0/README.md
--rw-r--r--   0        0        0      258 2023-04-24 10:50:11.261815 musif-1.1.0/musif/__init__.py
--rw-r--r--   0        0        0     7344 2023-04-24 10:50:21.851815 musif-1.1.0/musif/__main__.py
--rw-r--r--   0        0        0      232 2023-04-24 10:50:11.261815 musif-1.1.0/musif/cache/__init__.py
--rw-r--r--   0        0        0    17854 2023-04-24 10:50:21.851815 musif-1.1.0/musif/cache/cache.py
--rw-r--r--   0        0        0     7606 2023-04-24 10:50:21.851815 musif-1.1.0/musif/cache/utils.py
--rw-r--r--   0        0        0        1 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/__init__.py
--rw-r--r--   0        0        0      202 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/_constants.py
--rw-r--r--   0        0        0     2402 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/_logs.py
--rw-r--r--   0        0        0     3067 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/_utils.py
--rw-r--r--   0        0        0      826 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/constants.py
--rw-r--r--   0        0        0     1700 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/didone_utils.py
--rw-r--r--   0        0        0     1175 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/exceptions.py
--rw-r--r--   0        0        0     4102 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/sort.py
--rw-r--r--   0        0        0     2103 2023-04-24 10:50:11.261815 musif-1.1.0/musif/common/translate.py
--rw-r--r--   0        0        0     7287 2023-04-24 10:50:21.851815 musif-1.1.0/musif/config.py
--rw-r--r--   0        0        0       52 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/file_name_generic/__init__.py
--rw-r--r--   0        0        0       34 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/file_name_generic/constants.py
--rw-r--r--   0        0        0      999 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/file_name_generic/handler.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/scoring/__init__.py
--rw-r--r--   0        0        0      646 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/scoring/constants.py
--rw-r--r--   0        0        0     5686 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/basic_modules/scoring/handler.py
--rw-r--r--   0        0        0     1600 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/common.py
--rw-r--r--   0        0        0     1178 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/constants.py
--rw-r--r--   0        0        0    28678 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/extract.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/__init__.py
--rw-r--r--   0        0        0       25 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/ambitus/__init__.py
--rw-r--r--   0        0        0      270 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/ambitus/constants.py
--rw-r--r--   0        0        0     2705 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/ambitus/handler.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/core/__init__.py
--rw-r--r--   0        0        0      465 2023-04-24 10:50:11.261815 musif-1.1.0/musif/extract/features/core/constants.py
--rw-r--r--   0        0        0     7246 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/core/handler.py
--rw-r--r--   0        0        0       55 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/density/__init__.py
--rw-r--r--   0        0        0       57 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/density/constants.py
--rw-r--r--   0        0        0     7668 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/density/handler.py
--rw-r--r--   0        0        0       25 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/dynamics/__init__.py
--rw-r--r--   0        0        0      821 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/dynamics/constants.py
--rw-r--r--   0        0        0     9029 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/dynamics/handler.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/harmony/__init__.py
--rw-r--r--   0        0        0      815 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/harmony/constants.py
--rw-r--r--   0        0        0     2741 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/harmony/handler.py
--rw-r--r--   0        0        0    26047 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/harmony/utils.py
--rw-r--r--   0        0        0       29 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/jsymbolic/__init__.py
--rw-r--r--   0        0        0      282 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/jsymbolic/__main__.py
--rw-r--r--   0        0        0     2345 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/jsymbolic/handler.py
--rw-r--r--   0        0        0     3381 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/jsymbolic/utils.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/key/__init__.py
--rw-r--r--   0        0        0      165 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/key/constants.py
--rw-r--r--   0        0        0     1044 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/key/handler.py
--rw-r--r--   0        0        0       25 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/lyrics/__init__.py
--rw-r--r--   0        0        0      113 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/lyrics/constants.py
--rw-r--r--   0        0        0     3669 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/lyrics/handler.py
--rw-r--r--   0        0        0       25 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/melody/__init__.py
--rw-r--r--   0        0        0    10534 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/melody/constants.py
--rw-r--r--   0        0        0    30504 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/melody/handler.py
--rw-r--r--   0        0        0       80 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/music21/__init__.py
--rw-r--r--   0        0        0      173 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/music21/constants.py
--rw-r--r--   0        0        0     2182 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/music21/handler.py
--rw-r--r--   0        0        0     3554 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/prefix.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/rhythm/__init__.py
--rw-r--r--   0        0        0      273 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/rhythm/constants.py
--rw-r--r--   0        0        0     5925 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/rhythm/handler.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale/__init__.py
--rw-r--r--   0        0        0      269 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/scale/constants.py
--rw-r--r--   0        0        0     3627 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale/handler.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale_relative/__init__.py
--rw-r--r--   0        0        0      102 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale_relative/constants.py
--rw-r--r--   0        0        0     2842 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale_relative/handler.py
--rw-r--r--   0        0        0     7321 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/scale_relative/utils.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/tempo/__init__.py
--rw-r--r--   0        0        0      306 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/tempo/constants.py
--rw-r--r--   0        0        0     5145 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/features/tempo/handler.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/texture/__init__.py
--rw-r--r--   0        0        0       45 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/texture/constants.py
--rw-r--r--   0        0        0     3077 2023-04-24 10:50:11.265148 musif-1.1.0/musif/extract/features/texture/handler.py
--rw-r--r--   0        0        0    21081 2023-04-24 10:50:21.851815 musif-1.1.0/musif/extract/utils.py
--rw-r--r--   0        0        0     2011 2023-04-24 10:50:11.265148 musif-1.1.0/musif/logs.py
--rw-r--r--   0        0        0       61 2023-04-24 10:50:11.265148 musif-1.1.0/musif/musescore/__init__.py
--rw-r--r--   0        0        0      948 2023-04-24 10:50:11.265148 musif-1.1.0/musif/musescore/common.py
--rw-r--r--   0        0        0       95 2023-04-24 10:50:11.265148 musif-1.1.0/musif/musescore/constants.py
--rw-r--r--   0        0        0       91 2023-04-24 10:50:11.265148 musif-1.1.0/musif/musicxml/__init__.py
--rw-r--r--   0        0        0     7532 2023-04-24 10:50:21.851815 musif-1.1.0/musif/musicxml/common.py
--rw-r--r--   0        0        0    15310 2023-04-24 10:50:21.851815 musif-1.1.0/musif/musicxml/constants.py
--rw-r--r--   0        0        0     2092 2023-04-24 10:50:11.265148 musif-1.1.0/musif/musicxml/key.py
--rw-r--r--   0        0        0    17541 2023-04-24 10:50:11.268481 musif-1.1.0/musif/musicxml/repeat.py
--rw-r--r--   0        0        0     4513 2023-04-24 10:50:21.851815 musif-1.1.0/musif/musicxml/scoring.py
--rw-r--r--   0        0        0     8151 2023-04-24 10:50:21.851815 musif-1.1.0/musif/musicxml/tempo.py
--rw-r--r--   0        0        0        0 2023-04-24 10:50:11.268481 musif-1.1.0/musif/process/__init__.py
--rw-r--r--   0        0        0      410 2023-04-24 10:50:11.268481 musif-1.1.0/musif/process/constants.py
--rw-r--r--   0        0        0    11327 2023-04-24 10:50:21.851815 musif-1.1.0/musif/process/processor.py
--rw-r--r--   0        0        0     7824 2023-04-24 10:50:21.855148 musif-1.1.0/musif/process/utils.py
--rw-r--r--   0        0        0      650 2023-04-24 10:50:21.855148 musif-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 musif-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      971 2023-04-27 15:28:52.916781 musif-1.1.1/README.md
+-rw-r--r--   0        0        0      258 2023-04-20 14:52:06.385051 musif-1.1.1/musif/__init__.py
+-rw-r--r--   0        0        0     7344 2023-04-27 15:28:46.353448 musif-1.1.1/musif/__main__.py
+-rw-r--r--   0        0        0      232 2023-04-20 14:52:06.385051 musif-1.1.1/musif/cache/__init__.py
+-rw-r--r--   0        0        0    17854 2023-04-27 15:28:46.353448 musif-1.1.1/musif/cache/cache.py
+-rw-r--r--   0        0        0     7606 2023-04-27 15:28:46.353448 musif-1.1.1/musif/cache/utils.py
+-rw-r--r--   0        0        0        1 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/__init__.py
+-rw-r--r--   0        0        0      202 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/_constants.py
+-rw-r--r--   0        0        0     2402 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/_logs.py
+-rw-r--r--   0        0        0     3067 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/_utils.py
+-rw-r--r--   0        0        0      826 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/constants.py
+-rw-r--r--   0        0        0     1700 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/didone_utils.py
+-rw-r--r--   0        0        0     1175 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/exceptions.py
+-rw-r--r--   0        0        0     4102 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/sort.py
+-rw-r--r--   0        0        0     2103 2023-04-20 14:52:06.388385 musif-1.1.1/musif/common/translate.py
+-rw-r--r--   0        0        0     7287 2023-04-27 15:28:52.916781 musif-1.1.1/musif/config.py
+-rw-r--r--   0        0        0     7225 2023-04-21 13:30:56.223307 musif-1.1.1/musif/config.py~
+-rw-r--r--   0        0        0       52 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/file_name_generic/__init__.py
+-rw-r--r--   0        0        0       34 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/file_name_generic/constants.py
+-rw-r--r--   0        0        0      999 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/file_name_generic/handler.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/scoring/__init__.py
+-rw-r--r--   0        0        0      646 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/scoring/constants.py
+-rw-r--r--   0        0        0     5686 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/basic_modules/scoring/handler.py
+-rw-r--r--   0        0        0     1600 2023-04-20 14:52:06.388385 musif-1.1.1/musif/extract/common.py
+-rw-r--r--   0        0        0     1178 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/constants.py
+-rw-r--r--   0        0        0    28678 2023-04-27 15:28:52.916781 musif-1.1.1/musif/extract/extract.py
+-rw-r--r--   0        0        0    28696 2023-04-21 14:59:05.660981 musif-1.1.1/musif/extract/extract.py~
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/ambitus/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/ambitus/constants.py
+-rw-r--r--   0        0        0     2705 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/ambitus/handler.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/core/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/core/constants.py
+-rw-r--r--   0        0        0     7246 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/core/handler.py
+-rw-r--r--   0        0        0       55 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/density/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/density/constants.py
+-rw-r--r--   0        0        0     7668 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/density/handler.py
+-rw-r--r--   0        0        0       25 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/dynamics/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/dynamics/constants.py
+-rw-r--r--   0        0        0     9029 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/dynamics/handler.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/harmony/__init__.py
+-rw-r--r--   0        0        0      815 2023-04-20 14:52:06.391718 musif-1.1.1/musif/extract/features/harmony/constants.py
+-rw-r--r--   0        0        0     2741 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/harmony/handler.py
+-rw-r--r--   0        0        0    26047 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/harmony/utils.py
+-rw-r--r--   0        0        0       29 2023-04-27 15:28:52.916781 musif-1.1.1/musif/extract/features/jsymbolic/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:03:56.233060 musif-1.1.1/musif/extract/features/jsymbolic/__init__.py~
+-rw-r--r--   0        0        0      282 2023-04-27 15:28:52.916781 musif-1.1.1/musif/extract/features/jsymbolic/__main__.py
+-rw-r--r--   0        0        0      282 2023-04-20 15:03:56.233060 musif-1.1.1/musif/extract/features/jsymbolic/__main__.py~
+-rw-r--r--   0        0        0     2827 2023-04-27 15:36:24.763452 musif-1.1.1/musif/extract/features/jsymbolic/handler.py
+-rw-r--r--   0        0        0     2827 2023-04-27 15:35:28.226785 musif-1.1.1/musif/extract/features/jsymbolic/handler.py~
+-rw-r--r--   0        0        0     3381 2023-04-27 15:28:52.920114 musif-1.1.1/musif/extract/features/jsymbolic/utils.py
+-rw-r--r--   0        0        0     3379 2023-04-21 13:22:20.964657 musif-1.1.1/musif/extract/features/jsymbolic/utils.py~
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/key/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/key/constants.py
+-rw-r--r--   0        0        0     1044 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/key/handler.py
+-rw-r--r--   0        0        0       25 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/lyrics/__init__.py
+-rw-r--r--   0        0        0      113 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/lyrics/constants.py
+-rw-r--r--   0        0        0     3669 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/lyrics/handler.py
+-rw-r--r--   0        0        0       25 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/melody/__init__.py
+-rw-r--r--   0        0        0    10534 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/melody/constants.py
+-rw-r--r--   0        0        0    30504 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/melody/handler.py
+-rw-r--r--   0        0        0       80 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/music21/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-27 15:28:52.920114 musif-1.1.1/musif/extract/features/music21/constants.py
+-rw-r--r--   0        0        0      174 2023-04-21 14:21:18.728272 musif-1.1.1/musif/extract/features/music21/constants.py~
+-rw-r--r--   0        0        0     2182 2023-04-27 15:28:52.920114 musif-1.1.1/musif/extract/features/music21/handler.py
+-rw-r--r--   0        0        0     2109 2023-04-21 14:26:52.742891 musif-1.1.1/musif/extract/features/music21/handler.py~
+-rw-r--r--   0        0        0     3554 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/prefix.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/rhythm/__init__.py
+-rw-r--r--   0        0        0      273 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/rhythm/constants.py
+-rw-r--r--   0        0        0     5925 2023-04-27 15:28:46.353448 musif-1.1.1/musif/extract/features/rhythm/handler.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.395051 musif-1.1.1/musif/extract/features/scale/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-27 15:28:46.356781 musif-1.1.1/musif/extract/features/scale/constants.py
+-rw-r--r--   0        0        0     3627 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/scale/handler.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/scale_relative/__init__.py
+-rw-r--r--   0        0        0      102 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/scale_relative/constants.py
+-rw-r--r--   0        0        0     2842 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/scale_relative/handler.py
+-rw-r--r--   0        0        0     7321 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/scale_relative/utils.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/tempo/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/tempo/constants.py
+-rw-r--r--   0        0        0     5145 2023-04-27 15:28:46.356781 musif-1.1.1/musif/extract/features/tempo/handler.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/texture/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/texture/constants.py
+-rw-r--r--   0        0        0     3077 2023-04-20 14:52:06.398385 musif-1.1.1/musif/extract/features/texture/handler.py
+-rw-r--r--   0        0        0    21081 2023-04-27 15:28:46.356781 musif-1.1.1/musif/extract/utils.py
+-rw-r--r--   0        0        0    21081 2023-04-20 15:03:44.999752 musif-1.1.1/musif/extract/utils.py~
+-rw-r--r--   0        0        0     2011 2023-04-20 14:52:06.398385 musif-1.1.1/musif/logs.py
+-rw-r--r--   0        0        0       61 2023-04-20 14:52:06.398385 musif-1.1.1/musif/musescore/__init__.py
+-rw-r--r--   0        0        0      948 2023-04-20 14:52:06.398385 musif-1.1.1/musif/musescore/common.py
+-rw-r--r--   0        0        0       95 2023-04-20 14:52:06.398385 musif-1.1.1/musif/musescore/constants.py
+-rw-r--r--   0        0        0       91 2023-04-20 14:52:06.398385 musif-1.1.1/musif/musicxml/__init__.py
+-rw-r--r--   0        0        0     7532 2023-04-27 15:28:46.356781 musif-1.1.1/musif/musicxml/common.py
+-rw-r--r--   0        0        0    15310 2023-04-27 15:28:46.356781 musif-1.1.1/musif/musicxml/constants.py
+-rw-r--r--   0        0        0     2092 2023-04-20 14:52:06.401718 musif-1.1.1/musif/musicxml/key.py
+-rw-r--r--   0        0        0    17541 2023-04-20 14:52:06.401718 musif-1.1.1/musif/musicxml/repeat.py
+-rw-r--r--   0        0        0     4513 2023-04-27 15:28:46.356781 musif-1.1.1/musif/musicxml/scoring.py
+-rw-r--r--   0        0        0     8151 2023-04-27 15:28:46.356781 musif-1.1.1/musif/musicxml/tempo.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:52:06.401718 musif-1.1.1/musif/process/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-20 14:52:06.401718 musif-1.1.1/musif/process/constants.py
+-rw-r--r--   0        0        0    11327 2023-04-27 15:28:46.356781 musif-1.1.1/musif/process/processor.py
+-rw-r--r--   0        0        0     7824 2023-04-27 15:28:46.356781 musif-1.1.1/musif/process/utils.py
+-rw-r--r--   0        0        0      650 2023-04-27 15:36:49.866786 musif-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 musif-1.1.1/PKG-INFO
```

### Comparing `musif-1.1.0/README.md` & `musif-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/__main__.py` & `musif-1.1.1/musif/__main__.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/cache/cache.py` & `musif-1.1.1/musif/cache/cache.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/cache/utils.py` & `musif-1.1.1/musif/cache/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/common/_logs.py` & `musif-1.1.1/musif/common/_logs.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/common/_utils.py` & `musif-1.1.1/musif/common/_utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/common/constants.py` & `musif-1.1.1/musif/common/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/common/didone_utils.py` & `musif-1.1.1/musif/common/didone_utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/common/exceptions.py` & `musif-1.1.1/musif/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/common/sort.py` & `musif-1.1.1/musif/common/sort.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/common/translate.py` & `musif-1.1.1/musif/common/translate.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/config.py` & `musif-1.1.1/musif/config.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/basic_modules/file_name_generic/handler.py` & `musif-1.1.1/musif/extract/basic_modules/file_name_generic/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/basic_modules/scoring/constants.py` & `musif-1.1.1/musif/extract/basic_modules/scoring/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/basic_modules/scoring/handler.py` & `musif-1.1.1/musif/extract/basic_modules/scoring/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/common.py` & `musif-1.1.1/musif/extract/common.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/constants.py` & `musif-1.1.1/musif/extract/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/extract.py` & `musif-1.1.1/musif/extract/extract.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/ambitus/handler.py` & `musif-1.1.1/musif/extract/features/ambitus/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/core/handler.py` & `musif-1.1.1/musif/extract/features/core/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/density/handler.py` & `musif-1.1.1/musif/extract/features/density/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/dynamics/constants.py` & `musif-1.1.1/musif/extract/features/dynamics/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/dynamics/handler.py` & `musif-1.1.1/musif/extract/features/dynamics/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/harmony/constants.py` & `musif-1.1.1/musif/extract/features/harmony/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/harmony/handler.py` & `musif-1.1.1/musif/extract/features/harmony/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/harmony/utils.py` & `musif-1.1.1/musif/extract/features/harmony/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/jsymbolic/handler.py` & `musif-1.1.1/musif/extract/features/jsymbolic/handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import contextlib
 import os
 import tempfile
 import subprocess
 import pandas as pd
 
+import musif.extract.constants as C
+from musif.logs import pwarn
 from musif.extract.features.jsymbolic.utils import get_java_path, _jsymbolic_path
 
 JSYMBOLIC_JAR = str(_jsymbolic_path())
 JAVA_PATH = get_java_path()
 
 
 def get_tmpdir():
@@ -28,37 +30,48 @@
     score_features: dict,
 ):
     # 1. create a temporary directory (if Linux, force RAM usig /dev/shm)
     with get_tmpdir() as tmpdirname:
         # 2. convert the score to MEI usiing music21
         # TODO: if music21 implements export to MEI, use it
         midi_path = os.path.abspath(os.path.join(tmpdirname, "score.midi"))
-        with open(os.devnull, 'w') as devnull:
-            with contextlib.redirect_stdout(devnull):
-                score_data['score'].write("MIDI", midi_path)
+        try:
+            with open(os.devnull, 'w') as devnull:
+                with contextlib.redirect_stdout(devnull):
+                    score_data['score'].write("MIDI", midi_path)
+        except Exception as e:
+            filename = score_data[C.DATA_FILE]
+            pwarn(f"jSymbolic: could not convert {filename} to MIDI: {e}")
+            return
+
         # 3. run the MEI file through the jSymbolic jar savign csv into the temporary
         # directory in RAM
         out_path = os.path.abspath(os.path.join(tmpdirname, "features"))
         cmd = [JAVA_PATH,
                f"-Xmx{cfg.jsymbolic_max_ram}",
                "-jar",
                JSYMBOLIC_JAR,
                "-csv",
                ]
         if cfg.jsymbolic_config_file is not None:
             cmd += ["-configrun", cfg.jsymbolic_config_file]
-        subprocess.run(
-            cmd + [
-                midi_path,
-                out_path + ".xml",
-                out_path + "_def.xml",
-            ],
-            check=True,
-            stdout=subprocess.DEVNULL,
-        )
+        try:
+            subprocess.run(
+                cmd + [
+                    midi_path,
+                    out_path + ".xml",
+                    out_path + "_def.xml",
+                ],
+                check=True,
+                stdout=subprocess.DEVNULL,
+            )
+        except Exception as e:
+            filename = score_data[C.DATA_FILE]
+            pwarn(f"jSymbolic: cannot run jSymbolic on {filename}: {e}")
+            return
         # 4. read the csv file into a pandas dataframe
         df = pd.read_csv(out_path + ".csv", na_values=["NaN", " NaN", "NaN ", " NaN "])
         df = df.drop(columns=df.columns[0])
         # 5. add `js_` prefix to the column names
         df.columns = ["js_" + c for c in df.columns]
         # 6. load the features into the score_features dictionary
         score_features.update(df.to_dict(orient='records')[0])
```

### Comparing `musif-1.1.0/musif/extract/features/jsymbolic/utils.py` & `musif-1.1.1/musif/extract/features/jsymbolic/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/key/handler.py` & `musif-1.1.1/musif/extract/features/key/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/lyrics/handler.py` & `musif-1.1.1/musif/extract/features/lyrics/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/melody/constants.py` & `musif-1.1.1/musif/extract/features/melody/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/melody/handler.py` & `musif-1.1.1/musif/extract/features/melody/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/music21/handler.py` & `musif-1.1.1/musif/extract/features/music21/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/prefix.py` & `musif-1.1.1/musif/extract/features/prefix.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/rhythm/handler.py` & `musif-1.1.1/musif/extract/features/rhythm/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/scale/handler.py` & `musif-1.1.1/musif/extract/features/scale/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/scale_relative/handler.py` & `musif-1.1.1/musif/extract/features/scale_relative/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/scale_relative/utils.py` & `musif-1.1.1/musif/extract/features/scale_relative/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/tempo/handler.py` & `musif-1.1.1/musif/extract/features/tempo/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/features/texture/handler.py` & `musif-1.1.1/musif/extract/features/texture/handler.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/extract/utils.py` & `musif-1.1.1/musif/extract/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/logs.py` & `musif-1.1.1/musif/logs.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/musescore/common.py` & `musif-1.1.1/musif/musescore/common.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/musicxml/common.py` & `musif-1.1.1/musif/musicxml/common.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/musicxml/constants.py` & `musif-1.1.1/musif/musicxml/constants.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/musicxml/key.py` & `musif-1.1.1/musif/musicxml/key.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/musicxml/repeat.py` & `musif-1.1.1/musif/musicxml/repeat.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/musicxml/scoring.py` & `musif-1.1.1/musif/musicxml/scoring.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/musicxml/tempo.py` & `musif-1.1.1/musif/musicxml/tempo.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/process/processor.py` & `musif-1.1.1/musif/process/processor.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/musif/process/utils.py` & `musif-1.1.1/musif/process/utils.py`

 * *Files identical despite different names*

### Comparing `musif-1.1.0/pyproject.toml` & `musif-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "roman>=3.3",
     "joblib>=1.0.0",
     "scipy>=1.6.0",
     "music21>=8,<9",
     "deepdiff>=6.2.1",
 ]
 name = "musif"
-version = "1.1.0"
+version = "1.1.1"
 description = "Music feature extraction library from the DIDONE project"
 authors = [
     { name = "Didone Project", email = "didone@iccmu.es" },
 ]
 requires-python = ">=3.10"
 readme = "README.md"
```

### Comparing `musif-1.1.0/PKG-INFO` & `musif-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musif
-Version: 1.1.0
+Version: 1.1.1
 Summary: Music feature extraction library from the DIDONE project
 License: MIT
 Author-email: Didone Project <didone@iccmu.es>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # musif
```


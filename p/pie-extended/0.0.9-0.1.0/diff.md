# Comparing `tmp/pie_extended-0.0.9.tar.gz` & `tmp/pie_extended-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pie_extended-0.0.9.tar", last modified: Fri Apr 24 12:13:10 2020, max compression
+gzip compressed data, was "pie_extended-0.1.0.tar", last modified: Thu Apr 27 09:47:41 2023, max compression
```

## Comparing `pie_extended-0.0.9.tar` & `pie_extended-0.1.0.tar`

### file list

```diff
@@ -1,70 +1,89 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/tests/
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/tests/test_models/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1888 2020-04-23 13:58:50.000000 pie_extended-0.0.9/tests/test_models/test_fro.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    14246 2020-04-23 13:58:50.000000 pie_extended-0.0.9/tests/test_models/test_lasla.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-20 08:44:57.000000 pie_extended-0.0.9/tests/test_models/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3558 2020-04-24 12:12:41.000000 pie_extended-0.0.9/tests/test_models/test_fr.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       59 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended.egg-info/entry_points.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       77 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       19 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1835 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     6448 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4827 2020-04-23 13:58:50.000000 pie_extended-0.0.9/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       67 2019-12-19 08:02:18.000000 pie_extended-0.0.9/pie_extended/__main__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/testing_utils/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3018 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/testing_utils/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/cli/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4148 2020-02-25 14:02:45.000000 pie_extended-0.0.9/pie_extended/cli/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3412 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/cli/sub.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/models/
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/models/fr/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1606 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/fr/processor.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5902 2020-04-24 12:12:41.000000 pie_extended-0.0.9/pie_extended/models/fr/tokenizer.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      716 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/fr/imports.py
--rwxrwxr-x   0 thibault  (1000) thibault  (1000)     1795 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/fr/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       47 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/models/lasla/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1390 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/lasla/processor.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3690 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/lasla/tokenizer.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1949 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/lasla/imports.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      788 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/lasla/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    21824 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/lasla/_params.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/models/fro/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1630 2020-02-25 14:02:45.000000 pie_extended-0.0.9/pie_extended/models/fro/processor.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3543 2020-02-25 14:02:45.000000 pie_extended-0.0.9/pie_extended/models/fro/tokenizer.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      920 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/fro/imports.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      687 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/models/fro/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/pipeline/
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/pipeline/disambiguators/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      283 2019-12-19 17:08:38.000000 pie_extended-0.0.9/pie_extended/pipeline/disambiguators/proto.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 17:07:25.000000 pie_extended-0.0.9/pie_extended/pipeline/disambiguators/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      820 2019-12-20 08:37:39.000000 pie_extended-0.0.9/pie_extended/pipeline/disambiguators/autocat.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/pipeline/formatters/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1407 2020-02-25 14:02:45.000000 pie_extended-0.0.9/pie_extended/pipeline/formatters/proto.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 15:11:48.000000 pie_extended-0.0.9/pie_extended/pipeline/formatters/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/pipeline/iterators/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4424 2020-04-23 13:58:50.000000 pie_extended-0.0.9/pie_extended/pipeline/iterators/proto.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        3 2019-12-19 17:13:20.000000 pie_extended-0.0.9/pie_extended/pipeline/iterators/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/pipeline/tokenizers/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1100 2020-02-25 14:02:45.000000 pie_extended-0.0.9/pie_extended/pipeline/tokenizers/simple_tokenizer.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 17:06:18.000000 pie_extended-0.0.9/pie_extended/pipeline/tokenizers/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1041 2020-02-25 14:02:45.000000 pie_extended-0.0.9/pie_extended/pipeline/tokenizers/memorizing.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-20 08:07:13.000000 pie_extended-0.0.9/pie_extended/pipeline/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/pipeline/postprocessor/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4401 2020-04-23 14:53:46.000000 pie_extended-0.0.9/pie_extended/pipeline/postprocessor/glue.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2300 2020-04-23 14:53:46.000000 pie_extended-0.0.9/pie_extended/pipeline/postprocessor/splitter.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5437 2020-04-23 14:53:46.000000 pie_extended-0.0.9/pie_extended/pipeline/postprocessor/proto.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3723 2020-04-23 14:53:46.000000 pie_extended-0.0.9/pie_extended/pipeline/postprocessor/memory.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2020-02-25 14:02:45.000000 pie_extended-0.0.9/pie_extended/pipeline/postprocessor/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1863 2020-04-23 14:53:46.000000 pie_extended-0.0.9/pie_extended/pipeline/postprocessor/rulebased.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2020-04-24 12:13:10.000000 pie_extended-0.0.9/pie_extended/utils/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      852 2019-12-19 17:13:48.000000 pie_extended-0.0.9/pie_extended/utils/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3968 2020-04-23 14:53:46.000000 pie_extended-0.0.9/pie_extended/tagger.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 07:58:23.000000 pie_extended-0.0.9/pie_extended/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     6448 2020-04-24 12:13:10.000000 pie_extended-0.0.9/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3792 2020-04-24 12:12:41.000000 pie_extended-0.0.9/setup.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2020-04-24 12:13:10.000000 pie_extended-0.0.9/setup.cfg
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.685574 pie_extended-0.1.0/
+-rw-r--r--   0 thibault  (1000) thibault  (1000)    16725 2019-12-19 07:41:47.000000 pie_extended-0.1.0/LICENSE
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6445 2023-04-27 09:47:41.685574 pie_extended-0.1.0/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5754 2021-02-11 08:38:42.000000 pie_extended-0.1.0/README.md
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.673574 pie_extended-0.1.0/pie_extended/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 07:58:23.000000 pie_extended-0.1.0/pie_extended/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       67 2019-12-19 08:02:18.000000 pie_extended-0.1.0/pie_extended/__main__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.673574 pie_extended-0.1.0/pie_extended/cli/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2020-08-20 16:54:07.000000 pie_extended-0.1.0/pie_extended/cli/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5212 2023-01-31 13:50:33.000000 pie_extended-0.1.0/pie_extended/cli/main.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4530 2022-05-10 08:25:45.000000 pie_extended-0.1.0/pie_extended/cli/utils.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.673574 pie_extended-0.1.0/pie_extended/models/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       82 2020-12-04 18:21:14.000000 pie_extended-0.1.0/pie_extended/models/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.673574 pie_extended-0.1.0/pie_extended/models/dum/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      616 2020-12-04 18:21:14.000000 pie_extended-0.1.0/pie_extended/models/dum/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      463 2021-01-13 15:28:06.000000 pie_extended-0.1.0/pie_extended/models/dum/imports.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.677574 pie_extended-0.1.0/pie_extended/models/fr/
+-rwxrwxr-x   0 thibault  (1000) thibault  (1000)     1795 2020-04-23 13:58:50.000000 pie_extended-0.1.0/pie_extended/models/fr/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5383 2021-04-12 07:59:41.000000 pie_extended-0.1.0/pie_extended/models/fr/excluders.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      761 2021-01-13 15:27:50.000000 pie_extended-0.1.0/pie_extended/models/fr/imports.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1606 2020-04-23 13:58:50.000000 pie_extended-0.1.0/pie_extended/models/fr/processor.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3637 2021-04-12 07:28:48.000000 pie_extended-0.1.0/pie_extended/models/fr/tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.677574 pie_extended-0.1.0/pie_extended/models/freem/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      810 2022-12-05 19:37:10.000000 pie_extended-0.1.0/pie_extended/models/freem/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      941 2021-04-12 08:03:09.000000 pie_extended-0.1.0/pie_extended/models/freem/imports.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.677574 pie_extended-0.1.0/pie_extended/models/fro/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1995 2022-12-05 19:37:10.000000 pie_extended-0.1.0/pie_extended/models/fro/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1114 2021-05-20 08:42:31.000000 pie_extended-0.1.0/pie_extended/models/fro/imports.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1998 2020-12-14 11:20:46.000000 pie_extended-0.1.0/pie_extended/models/fro/processor.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2755 2021-05-20 08:42:31.000000 pie_extended-0.1.0/pie_extended/models/fro/tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.677574 pie_extended-0.1.0/pie_extended/models/grc/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2023 2021-02-11 09:35:40.000000 pie_extended-0.1.0/pie_extended/models/grc/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      749 2021-03-22 13:34:04.000000 pie_extended-0.1.0/pie_extended/models/grc/imports.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1641 2021-02-11 09:35:40.000000 pie_extended-0.1.0/pie_extended/models/grc/processor.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2451 2021-03-22 13:31:46.000000 pie_extended-0.1.0/pie_extended/models/grc/tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.677574 pie_extended-0.1.0/pie_extended/models/lasla/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2495 2021-04-03 07:13:21.000000 pie_extended-0.1.0/pie_extended/models/lasla/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1375 2020-12-04 16:36:08.000000 pie_extended-0.1.0/pie_extended/models/lasla/_params.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2639 2021-01-13 15:25:15.000000 pie_extended-0.1.0/pie_extended/models/lasla/imports.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5596 2021-02-11 09:35:40.000000 pie_extended-0.1.0/pie_extended/models/lasla/processor.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4090 2021-02-03 12:42:25.000000 pie_extended-0.1.0/pie_extended/models/lasla/tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.677574 pie_extended-0.1.0/pie_extended/pipeline/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-20 08:07:13.000000 pie_extended-0.1.0/pie_extended/pipeline/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.677574 pie_extended-0.1.0/pie_extended/pipeline/disambiguators/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 17:07:25.000000 pie_extended-0.1.0/pie_extended/pipeline/disambiguators/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2134 2020-09-23 09:14:05.000000 pie_extended-0.1.0/pie_extended/pipeline/disambiguators/autocat.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      283 2019-12-19 17:08:38.000000 pie_extended-0.1.0/pie_extended/pipeline/disambiguators/proto.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.681574 pie_extended-0.1.0/pie_extended/pipeline/formatters/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 15:11:48.000000 pie_extended-0.1.0/pie_extended/pipeline/formatters/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1420 2020-06-22 12:18:04.000000 pie_extended-0.1.0/pie_extended/pipeline/formatters/proto.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.681574 pie_extended-0.1.0/pie_extended/pipeline/iterators/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        3 2019-12-19 17:13:20.000000 pie_extended-0.1.0/pie_extended/pipeline/iterators/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5461 2021-01-13 15:24:27.000000 pie_extended-0.1.0/pie_extended/pipeline/iterators/proto.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.681574 pie_extended-0.1.0/pie_extended/pipeline/postprocessor/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2020-02-25 14:02:45.000000 pie_extended-0.1.0/pie_extended/pipeline/postprocessor/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4614 2021-02-11 09:35:40.000000 pie_extended-0.1.0/pie_extended/pipeline/postprocessor/glue.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3723 2020-04-23 14:53:46.000000 pie_extended-0.1.0/pie_extended/pipeline/postprocessor/memory.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5455 2021-02-11 09:26:29.000000 pie_extended-0.1.0/pie_extended/pipeline/postprocessor/proto.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1863 2020-04-23 14:53:46.000000 pie_extended-0.1.0/pie_extended/pipeline/postprocessor/rulebased.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2887 2020-05-05 15:15:28.000000 pie_extended-0.1.0/pie_extended/pipeline/postprocessor/splitter.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.681574 pie_extended-0.1.0/pie_extended/pipeline/tokenizers/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 17:06:18.000000 pie_extended-0.1.0/pie_extended/pipeline/tokenizers/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2000 2020-08-20 16:54:07.000000 pie_extended-0.1.0/pie_extended/pipeline/tokenizers/memorizing.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2537 2020-12-04 18:21:14.000000 pie_extended-0.1.0/pie_extended/pipeline/tokenizers/simple_tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.681574 pie_extended-0.1.0/pie_extended/pipeline/tokenizers/utils/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2020-08-20 16:54:07.000000 pie_extended-0.1.0/pie_extended/pipeline/tokenizers/utils/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       86 2020-09-08 15:47:36.000000 pie_extended-0.1.0/pie_extended/pipeline/tokenizers/utils/chars.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    11438 2021-04-12 07:58:27.000000 pie_extended-0.1.0/pie_extended/pipeline/tokenizers/utils/excluder.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      601 2020-09-08 15:53:07.000000 pie_extended-0.1.0/pie_extended/pipeline/tokenizers/utils/regexps.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4979 2022-05-10 08:17:38.000000 pie_extended-0.1.0/pie_extended/tagger.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.681574 pie_extended-0.1.0/pie_extended/testing_utils/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3800 2020-08-20 16:54:07.000000 pie_extended-0.1.0/pie_extended/testing_utils/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.681574 pie_extended-0.1.0/pie_extended/utils/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1537 2020-05-05 15:15:28.000000 pie_extended-0.1.0/pie_extended/utils/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.673574 pie_extended-0.1.0/pie_extended.egg-info/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6445 2023-04-27 09:47:41.000000 pie_extended-0.1.0/pie_extended.egg-info/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2397 2023-04-27 09:47:41.000000 pie_extended-0.1.0/pie_extended.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-04-27 09:47:41.000000 pie_extended-0.1.0/pie_extended.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       64 2023-04-27 09:47:41.000000 pie_extended-0.1.0/pie_extended.egg-info/entry_points.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      130 2023-04-27 09:47:41.000000 pie_extended-0.1.0/pie_extended.egg-info/requires.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       19 2023-04-27 09:47:41.000000 pie_extended-0.1.0/pie_extended.egg-info/top_level.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-04-27 09:47:41.685574 pie_extended-0.1.0/setup.cfg
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3799 2023-04-27 09:47:25.000000 pie_extended-0.1.0/setup.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.673574 pie_extended-0.1.0/tests/
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:47:41.685574 pie_extended-0.1.0/tests/test_models/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-20 08:44:57.000000 pie_extended-0.1.0/tests/test_models/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4278 2020-04-28 14:13:57.000000 pie_extended-0.1.0/tests/test_models/test_fr.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1424 2020-08-20 16:54:07.000000 pie_extended-0.1.0/tests/test_models/test_fro.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     9770 2020-12-04 16:36:08.000000 pie_extended-0.1.0/tests/test_models/test_lasla.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pie_extended-0.0.9/tests/test_models/test_fr.py` & `pie_extended-0.1.0/tests/test_models/test_fr.py`

 * *Files 16% similar despite different names*

```diff
@@ -89,7 +89,23 @@
             list(
                 iterator.tokenizer.sentence_tokenizer("Va-t'en va-nu-pieds !")
             ),
             [
                 ["Va", "-t'", "en", "va", "-", "nu", "-", "pieds", "!"]
             ]
         )
+
+    def test_tokenization_abbreviations(self):
+        """ Check that abbreviation are recognized """
+        iterator, _ = get_iterator_and_processor()
+        self.assertEqual(
+            list(
+                iterator.tokenizer.sentence_tokenizer("La Zoo. montre des limites. cf. un truc. Et V. n.  est un neutre"
+                                                      ". Mais j'aime ma Lit. et mon lit.!")
+            ),
+            [
+                ['La', 'Zoo.', 'montre', 'des', 'limites', '.'],
+                ['cf.', 'un', 'truc', '.'],
+                ['Et', 'V.', 'n.', 'est', 'un', 'neutre', '.'],
+                ['Mais', "j'", 'aime', 'ma', 'Lit.', 'et', 'mon', 'lit', '.', '!']
+            ]
+        )
```

### Comparing `pie_extended-0.0.9/pie_extended.egg-info/SOURCES.txt` & `pie_extended-0.1.0/pie_extended.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,40 @@
+LICENSE
 README.md
 setup.py
 pie_extended/__init__.py
 pie_extended/__main__.py
 pie_extended/tagger.py
 pie_extended.egg-info/PKG-INFO
 pie_extended.egg-info/SOURCES.txt
 pie_extended.egg-info/dependency_links.txt
 pie_extended.egg-info/entry_points.txt
 pie_extended.egg-info/requires.txt
 pie_extended.egg-info/top_level.txt
 pie_extended/cli/__init__.py
-pie_extended/cli/sub.py
+pie_extended/cli/main.py
+pie_extended/cli/utils.py
 pie_extended/models/__init__.py
+pie_extended/models/dum/__init__.py
+pie_extended/models/dum/imports.py
 pie_extended/models/fr/__init__.py
+pie_extended/models/fr/excluders.py
 pie_extended/models/fr/imports.py
 pie_extended/models/fr/processor.py
 pie_extended/models/fr/tokenizer.py
+pie_extended/models/freem/__init__.py
+pie_extended/models/freem/imports.py
 pie_extended/models/fro/__init__.py
 pie_extended/models/fro/imports.py
 pie_extended/models/fro/processor.py
 pie_extended/models/fro/tokenizer.py
+pie_extended/models/grc/__init__.py
+pie_extended/models/grc/imports.py
+pie_extended/models/grc/processor.py
+pie_extended/models/grc/tokenizer.py
 pie_extended/models/lasla/__init__.py
 pie_extended/models/lasla/_params.py
 pie_extended/models/lasla/imports.py
 pie_extended/models/lasla/processor.py
 pie_extended/models/lasla/tokenizer.py
 pie_extended/pipeline/__init__.py
 pie_extended/pipeline/disambiguators/__init__.py
@@ -38,13 +49,17 @@
 pie_extended/pipeline/postprocessor/memory.py
 pie_extended/pipeline/postprocessor/proto.py
 pie_extended/pipeline/postprocessor/rulebased.py
 pie_extended/pipeline/postprocessor/splitter.py
 pie_extended/pipeline/tokenizers/__init__.py
 pie_extended/pipeline/tokenizers/memorizing.py
 pie_extended/pipeline/tokenizers/simple_tokenizer.py
+pie_extended/pipeline/tokenizers/utils/__init__.py
+pie_extended/pipeline/tokenizers/utils/chars.py
+pie_extended/pipeline/tokenizers/utils/excluder.py
+pie_extended/pipeline/tokenizers/utils/regexps.py
 pie_extended/testing_utils/__init__.py
 pie_extended/utils/__init__.py
 tests/test_models/__init__.py
 tests/test_models/test_fr.py
 tests/test_models/test_fro.py
 tests/test_models/test_lasla.py
```

### Comparing `pie_extended-0.0.9/pie_extended.egg-info/PKG-INFO` & `pie_extended-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,136 +1,176 @@
 Metadata-Version: 2.1
-Name: pie-extended
-Version: 0.0.9
+Name: pie_extended
+Version: 0.1.0
 Summary: Extension for nlp-pie package
-Home-page: https://github.com/ponteineptique/nlp-pie-taggers
+Home-page: https://github.com/hipster-philology/nlp-pie-taggers
 Author: Thibault Clérice
 License: MIT
-Description: 
-        # Pie Extended
-        
-        [![Build Status](https://travis-ci.org/hipster-philology/nlp-pie-taggers.svg?branch=master)](https://travis-ci.org/hipster-philology/nlp-pie-taggers)
-        [![Coverage Status](https://coveralls.io/repos/github/hipster-philology/nlp-pie-taggers/badge.svg?branch=master)](https://coveralls.io/github/hipster-philology/nlp-pie-taggers?branch=master)
-        ![PyPI](https://img.shields.io/pypi/v/pie-extended?style=flat-square)
-        
-        Extension for [`pie`](https://github.com/emanjavacas/pie) to include taggers with their models and pre/postprocessors.
-        
-        Pie is a wonderful tool to train models. And most of the time, it will be enough. What `pie_extended` is proposing here 
-        is to provide you with the necessary tools to share your models with customized pre- and post-processing.
-        
-        The current system provide an easier access to adding **customized**:
-        - normalization of your text,
-        - sentence tokenization,
-        - word tokenization,
-        - disambiguation,
-        - output formatting
-        
-        ## Install
-        
-        To install, simply do `pip install pie-extended`. Then, look at all available models.
-        
-        ## Run on terminal
-        
-        But on top of that, it provides a quick and easy way to use others models ! For example, in a shell :
-        
-        ```bash
-        pie-extended download lasla
-        pie-extended install-addons lasla
-        pie-extended tag laslsa your_file.txt
-        ```
-        
-        will give you access to all you need !
-        
-        ## Python API
-        
-        You can run the lemmatizer in your own scripts and retrieve token annotations as dictionaries:
-        
-        ```python
-        from typing import List
-        from pie_extended.cli.sub import get_tagger, get_model, download
-        
-        # In case you need to download
-        do_download = False
-        if do_download:
-            for dl in download("lasla"):
-                x = 1
-        
-        # model_path allows you to override the model loaded by another .tar
-        model_name = "lasla"
-        tagger = get_tagger(model_name, batch_size=256, device="cpu", model_path=None)
-        
-        sentences: List[str] = ["Lorem ipsum dolor sit amet, consectetur adipiscing elit. "]
-        # Get the main object from the model (: data iterator + postprocesor
-        from pie_extended.models.lasla.imports import get_iterator_and_processor
-        for sentence_group in sentences:
-            iterator, processor = get_iterator_and_processor()
-            print(tagger.tag_str(sentence_group, iterator=iterator, processor=processor) )
-        ```
-        
-        will result in
-        
-        ```python
-        [{'form': 'lorem', 'lemma': 'lor', 'POS': 'NOMcom', 'morph': 'Case=Acc|Numb=Sing', 'treated': 'lorem'},
-         {'form': 'ipsum', 'lemma': 'ipse', 'POS': 'PROdem', 'morph': 'Case=Acc|Numb=Sing', 'treated': 'ipsum'},
-         {'form': 'dolor', 'lemma': 'dolor', 'POS': 'NOMcom', 'morph': 'Case=Nom|Numb=Sing', 'treated': 'dolor'},
-         {'form': 'sit', 'lemma': 'sum1', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Act|Person=3',
-          'treated': 'sit'},
-         {'form': 'amet', 'lemma': 'amo', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Act|Person=3',
-          'treated': 'amet'}, {'form': ',', 'lemma': ',', 'pos': 'PUNC', 'morph': 'MORPH=empty', 'treated': ','},
-         {'form': 'consectetur', 'lemma': 'consector2', 'POS': 'VER',
-          'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Dep|Person=3', 'treated': 'consectetur'},
-         {'form': 'adipiscing', 'lemma': 'adipiscor', 'POS': 'VER', 'morph': 'Tense=Pres|Voice=Dep', 'treated': 'adipiscing'},
-         {'form': 'elit', 'lemma': 'elio', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Ind|Tense=Pres|Voice=Act|Person=3',
-          'treated': 'elit'}, {'form': '.', 'lemma': '.', 'pos': 'PUNC', 'morph': 'MORPH=empty', 'treated': '.'}]
-        ```
-        
-        ## Add a model
-        
-        - Create a package in `./pie_extended/models/`. Exemple: `foo`.
-        - Add the name of the package in `./pie_extended/models/__init__.py` in the variable `modules`.
-        - In the module `pie_extended.models.foo`, we should find the following variable:
-            - `Models` : a string with filenames and tasks for Pie.
-            - `DESC`: a METADATA object that bears information about the model
-            - `DOWNLOADS`: A list of file to download.
-            
-        ```python
-        from pie_extended.utils import Metadata, File, get_path
-        
-        DESC = Metadata(
-            "Foo"
-            "language",
-            ["Author 1", "Author 2"],
-            "A readable description",
-            "A link to more information"
-        )
-        
-        DOWNLOADS = [
-            File("/a/link/to/a/file", "local_name_of_the_file.tar")
-        ]
-        
-        
-        Models = "<{},task1,task2><{},lemma,pos>".format(
-            get_path("foo", "local_name_of_the_file.tar")
-        )
-        
-        ```
-        - In the module `pie_extended.models.foo.imports`, we should find the following content:
-            1. `get_iterator_and_processor`: a function that returns a `DataIterator` and a `Processor` 
-            2. (optionally) `addons`: a function that installs add-ons
-            3. (optionally) `Disambiguator`: a disambiguator instance (or an object creator that returns one)
-        
-        Check for a simple example in `pie_extended.models.fro.imports` and a more complex one 
-        in `pie_extended.models.lasla.imports`
-        
-        ## Warning
-        
-        This is an extremely early build, subject to change here and there. But it is functional !
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Pie Extended
+
+[![Build Status](https://travis-ci.org/hipster-philology/nlp-pie-taggers.svg?branch=master)](https://travis-ci.org/hipster-philology/nlp-pie-taggers)
+[![Coverage Status](https://coveralls.io/repos/github/hipster-philology/nlp-pie-taggers/badge.svg?branch=master)](https://coveralls.io/github/hipster-philology/nlp-pie-taggers?branch=master)
+![PyPI](https://img.shields.io/pypi/v/pie-extended?style=flat-square)
+
+**Warning**: This software is only compatible with up to Python 3.7 for the moment.
+
+Extension for [`pie`](https://github.com/emanjavacas/pie) to include taggers with their models and pre/postprocessors.
+
+Pie is a wonderful tool to train models. And most of the time, it will be enough. What `pie_extended` is proposing here 
+is to provide you with the necessary tools to share your models with customized pre- and post-processing.
+
+The current system provide an easier access to adding **customized**:
+- normalization of your text,
+- sentence tokenization,
+- word tokenization,
+- disambiguation,
+- output formatting
+
+## Cite as
+
+```
+@software{thibault_clerice_2020_3883590,
+  author       = {Clérice, Thibault},
+  title        = {Pie Extended, an extension for Pie with pre-processing and post-processing},
+  month        = jun,
+  year         = 2020,
+  publisher    = {Zenodo},
+  doi          = {10.5281/zenodo.3883589},
+  url          = {https://doi.org/10.5281/zenodo.3883589}
+}
+```
+
+## Current supported languages
+
+- Classical Latin (Model: `lasla`)
+- Ancient Greek (Model: `grc`)
+- Old French (Model: `fro`)
+- Early Modern French (Model: `freem`)
+- Classical French (Model: `fr`)
+- Old Dutch (Model: `dum`)
+
+If you trained models and want some help sharing them with Pie Extended, open an issue :)
+
+## Install
+
+To install, simply do `pip install pie-extended`. Then, look at all available models.
+
+## Run on terminal
+
+But on top of that, it provides a quick and easy way to use others models ! For example, in a shell :
+
+```bash
+pie-extended download lasla
+pie-extended install-addons lasla
+pie-extended tag lasla your_file.txt
+```
+
+will give you access to all you need !
+
+## Python API
+
+You can run the lemmatizer in your own scripts and retrieve token annotations as dictionaries:
+
+```python
+from typing import List
+from pie_extended.cli.utils import get_tagger, get_model, download
+
+# In case you need to download
+do_download = False
+if do_download:
+    for dl in download("lasla"):
+        x = 1
+
+# model_path allows you to override the model loaded by another .tar
+model_name = "lasla"
+tagger = get_tagger(model_name, batch_size=256, device="cpu", model_path=None)
+
+sentences: List[str] = ["Lorem ipsum dolor sit amet, consectetur adipiscing elit. "]
+# Get the main object from the model (: data iterator + postprocesor
+from pie_extended.models.lasla.imports import get_iterator_and_processor
+for sentence_group in sentences:
+    iterator, processor = get_iterator_and_processor()
+    print(tagger.tag_str(sentence_group, iterator=iterator, processor=processor) )
+```
+
+will result in
+
+```python
+[{'form': 'lorem', 'lemma': 'lor', 'POS': 'NOMcom', 'morph': 'Case=Acc|Numb=Sing', 'treated': 'lorem'},
+ {'form': 'ipsum', 'lemma': 'ipse', 'POS': 'PROdem', 'morph': 'Case=Acc|Numb=Sing', 'treated': 'ipsum'},
+ {'form': 'dolor', 'lemma': 'dolor', 'POS': 'NOMcom', 'morph': 'Case=Nom|Numb=Sing', 'treated': 'dolor'},
+ {'form': 'sit', 'lemma': 'sum1', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Act|Person=3',
+  'treated': 'sit'},
+ {'form': 'amet', 'lemma': 'amo', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Act|Person=3',
+  'treated': 'amet'}, {'form': ',', 'lemma': ',', 'pos': 'PUNC', 'morph': 'MORPH=empty', 'treated': ','},
+ {'form': 'consectetur', 'lemma': 'consector2', 'POS': 'VER',
+  'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Dep|Person=3', 'treated': 'consectetur'},
+ {'form': 'adipiscing', 'lemma': 'adipiscor', 'POS': 'VER', 'morph': 'Tense=Pres|Voice=Dep', 'treated': 'adipiscing'},
+ {'form': 'elit', 'lemma': 'elio', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Ind|Tense=Pres|Voice=Act|Person=3',
+  'treated': 'elit'}, {'form': '.', 'lemma': '.', 'pos': 'PUNC', 'morph': 'MORPH=empty', 'treated': '.'}]
+```
+
+## Add a model
+
+- Create a package in `./pie_extended/models/`. Exemple: `foo`.
+- Add the name of the package in `./pie_extended/models/__init__.py` in the variable `modules`.
+- In the module `pie_extended.models.foo`, we should find the following variable:
+    - `Models` : a string with filenames and tasks for Pie.
+    - `DESC`: a METADATA object that bears information about the model
+    - `DOWNLOADS`: A list of file to download.
+    
+```python
+from pie_extended.utils import Metadata, File, get_path
+
+DESC = Metadata(
+    "Foo"
+    "language",
+    ["Author 1", "Author 2"],
+    "A readable description",
+    "A link to more information"
+)
+
+DOWNLOADS = [
+    File("/a/link/to/a/file", "local_name_of_the_file.tar")
+]
+
+
+Models = "<{},task1,task2><{},lemma,pos>".format(
+    get_path("foo", "local_name_of_the_file.tar")
+)
+
+```
+- In the module `pie_extended.models.foo.imports`, we should find the following content:
+    1. `get_iterator_and_processor`: a function that returns a `DataIterator` and a `Processor` 
+    2. (optionally) `addons`: a function that installs add-ons
+    3. (optionally) `Disambiguator`: a disambiguator instance (or an object creator that returns one)
+
+Check for a simple example in `pie_extended.models.fro.imports` and a more complex one 
+in `pie_extended.models.lasla.imports`
+
+
+## Install development version (⚠ for development only)
+
+Clone the repository, create an environment, and then
+
+```bash
+python setup.py develop
+```
+
+## Warning
+
+This is an extremely early build, subject to change here and there. But it is functional !
+
+
```

### Comparing `pie_extended-0.0.9/README.md` & `pie_extended-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,75 @@
 # Pie Extended
 
 [![Build Status](https://travis-ci.org/hipster-philology/nlp-pie-taggers.svg?branch=master)](https://travis-ci.org/hipster-philology/nlp-pie-taggers)
 [![Coverage Status](https://coveralls.io/repos/github/hipster-philology/nlp-pie-taggers/badge.svg?branch=master)](https://coveralls.io/github/hipster-philology/nlp-pie-taggers?branch=master)
 ![PyPI](https://img.shields.io/pypi/v/pie-extended?style=flat-square)
 
+**Warning**: This software is only compatible with up to Python 3.7 for the moment.
+
 Extension for [`pie`](https://github.com/emanjavacas/pie) to include taggers with their models and pre/postprocessors.
 
 Pie is a wonderful tool to train models. And most of the time, it will be enough. What `pie_extended` is proposing here 
 is to provide you with the necessary tools to share your models with customized pre- and post-processing.
 
 The current system provide an easier access to adding **customized**:
 - normalization of your text,
 - sentence tokenization,
 - word tokenization,
 - disambiguation,
 - output formatting
 
+## Cite as
+
+```
+@software{thibault_clerice_2020_3883590,
+  author       = {Clérice, Thibault},
+  title        = {Pie Extended, an extension for Pie with pre-processing and post-processing},
+  month        = jun,
+  year         = 2020,
+  publisher    = {Zenodo},
+  doi          = {10.5281/zenodo.3883589},
+  url          = {https://doi.org/10.5281/zenodo.3883589}
+}
+```
+
+## Current supported languages
+
+- Classical Latin (Model: `lasla`)
+- Ancient Greek (Model: `grc`)
+- Old French (Model: `fro`)
+- Early Modern French (Model: `freem`)
+- Classical French (Model: `fr`)
+- Old Dutch (Model: `dum`)
+
+If you trained models and want some help sharing them with Pie Extended, open an issue :)
+
 ## Install
 
 To install, simply do `pip install pie-extended`. Then, look at all available models.
 
 ## Run on terminal
 
 But on top of that, it provides a quick and easy way to use others models ! For example, in a shell :
 
 ```bash
 pie-extended download lasla
 pie-extended install-addons lasla
-pie-extended tag laslsa your_file.txt
+pie-extended tag lasla your_file.txt
 ```
 
 will give you access to all you need !
 
 ## Python API
 
 You can run the lemmatizer in your own scripts and retrieve token annotations as dictionaries:
 
 ```python
 from typing import List
-from pie_extended.cli.sub import get_tagger, get_model, download
+from pie_extended.cli.utils import get_tagger, get_model, download
 
 # In case you need to download
 do_download = False
 if do_download:
     for dl in download("lasla"):
         x = 1
 
@@ -109,10 +136,19 @@
     1. `get_iterator_and_processor`: a function that returns a `DataIterator` and a `Processor` 
     2. (optionally) `addons`: a function that installs add-ons
     3. (optionally) `Disambiguator`: a disambiguator instance (or an object creator that returns one)
 
 Check for a simple example in `pie_extended.models.fro.imports` and a more complex one 
 in `pie_extended.models.lasla.imports`
 
+
+## Install development version (⚠ for development only)
+
+Clone the repository, create an environment, and then
+
+```bash
+python setup.py develop
+```
+
 ## Warning
 
-This is an extremely early build, subject to change here and there. But it is functional !
+This is an extremely early build, subject to change here and there. But it is functional !
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pie_extended-0.0.9/pie_extended/testing_utils/__init__.py` & `pie_extended-0.1.0/pie_extended/testing_utils/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 from pie_extended.pipeline.iterators.proto import DataIterator
 from pie_extended.pipeline.postprocessor.proto import ProcessorPrototype
 from pie_extended.tagger import ExtensibleTagger
 from pie.utils import model_spec
-from pie_extended.cli.sub import get_imports
+from pie_extended.cli.utils import get_imports
 
 
 class FakeTagger(ExtensibleTagger):
     def __init__(self, tokens, tasks):
         self.tokens = tokens
         self.tasks = tasks
         self.seen = []
@@ -23,18 +23,28 @@
 
 class FakeAutoTag(ExtensibleTagger):
     def __init__(self, tasks: List[str], **kwargs):
         self.tokens: List[str] = []
         self.lengths: List[int] = []
         self.tasks = tasks
         self.lower = False
+        self.glue_task: str = kwargs.get("glue_task", "_")
+        self.glue_value: str = kwargs.get("glue_value", "|")
         self.disambiguation = None
+        self.start_end: bool = False
         for key in kwargs:
             setattr(self, key, kwargs[key])
 
+    def toggle_start_end(self, status: Optional[bool] = None) -> bool:
+        if status is None:
+            self.start_end = not self.start_end
+        else:
+            self.start_end = status
+        return self.start_end
+
     def tag(self, sents: List[List[str]], lengths: List[int], *args, **kwargs):
         """ Fake tagging tokens by enumerating informations
 
         >>> tagger = FakeAutoTag(["pos", "lemma"])
         >>> tagger.tag([['a', 'b'], ['c']], lengths=[2, 1])
         ([[('a', ('pos0', 'lemma0')), ('b', ('pos1', 'lemma1'))], [('c', ('pos2', 'lemma2'))]], ['pos', 'lemma'])
 
@@ -46,21 +56,27 @@
             if len(t) != l:
                 raise ValueError("Tokens and lengths are inequal [len({}) != {}]".format(str(t), l))
 
         out = []
         total = 0
 
         def get_task(task, i):
+            if "_" in task:
+                return self.glue_value.join([tsk+str(i) for tsk in task.split(self.glue_task)])
             return task+str(i)
 
         for sent in sents:
             out.append([])
+            if self.start_end:
+                out[-1].append(("START", tuple(list(get_task(task, total) for task in self.tasks))))
             for tok in sent:
                 out[-1].append((tok, tuple(list(get_task(task, total) for task in self.tasks))))
                 total += 1
+            if self.start_end:
+                out[-1].append(("END", tuple(list(get_task(task, total) for task in self.tasks))))
         return out, self.tasks
 
     @staticmethod
     def from_model_string(model_string: str, **kwargs) -> "FakeAutoTag":
         """
 
         :param model_string:
```

### Comparing `pie_extended-0.0.9/pie_extended/cli/__init__.py` & `pie_extended-0.1.0/pie_extended/cli/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import click
 
-from . import sub
-from typing import Iterable
 
+from pie_extended.cli import utils
+from typing import Iterable
 
-MODELS = [name for name, *_ in sub.get_list()]
+MODELS = [name for name, *_ in utils.get_list()]
 
 
 @click.group("pie-ext")
 def pie_ext():
     """ Addon for Pie that allows you to download and install modules that you might be interested in """
 
 
 @pie_ext.command("list")
 @click.option("--full", is_flag=True, help="Display full information on models")
 def print_list(full):
     """ List available model to download and use """
     click.echo("Available Models:")
-    for module, desc in sub.get_list():
+    for module, desc in utils.get_list():
         click.echo("\t- {} ({}) : {}".format(
             click.style(module, bold=True),
             desc.lang,
             click.style(desc.title, underline=True)
         ))
         if full:
             click.echo("\t\tAuthor(s): {}".format(", ".join(desc.authors)))
@@ -30,60 +30,68 @@
 
 
 @pie_ext.command("download")
 @click.argument("model", type=click.Choice(MODELS, case_sensitive=False))
 def download(model):
     """ Download a [model] for future availability. Check list for available models"""
     click.echo(click.style("Starting downloading...", bold=True))
-    for index, file in enumerate(sub.download(model)):
+    for index, file in enumerate(utils.download(model)):
         if index == 0:
             click.echo("{} files to download".format(file))
         else:
             click.echo("- {} downloaded".format(file))
     click.echo(click.style("Finished !", bold=True))
 
 
 @pie_ext.command("tag")
 @click.argument("model", type=click.Choice(MODELS, case_sensitive=False))
 @click.argument("filepath", nargs=-1, type=click.Path(exists=True, dir_okay=False))
+@click.option("--no-tokenizer", "no_tokenizer", is_flag=True,
+              help="Do not apply advanced tokenizer: new line = one word, two new lines = one sentence")
 @click.option("--allow-n-failures", "allowed_failure", type=int, default=5,
               help="Number of failures before things crash")
 @click.option("--batch_size", type=int, default=16,
               help="Group of sentences tagged together")
 @click.option("--device", type=str, default="cpu",
               help="Use cpu or gpu for prediction")
 @click.option("--debug", is_flag=True,
               help="Raise error when a file is not tagged correctly")
 @click.option("--model_path", type=str, default=None,
               help="Provide this with your own model path if you want to test it")
 @click.option("--reset-exclude-patterns", "reset_patterns", is_flag=True, default=False,
               help="Reset exclude patterns")
 @click.option("--add-pattern", "add_pattern",
               help="Add new exclude patterns  for token (Regular expression)", multiple=True)
+@click.option("--max-tokens", "max_tokens",
+              help="Maximum length of sentence", type=int, default=64)
 def tag(model: str, filepath: str, allowed_failure: bool, batch_size: int, device: str, debug: bool,
         model_path: str,
-        reset_patterns: bool, add_pattern: Iterable[str]):
+        reset_patterns: bool, add_pattern: Iterable[str],
+        no_tokenizer: bool = False,
+        max_tokens: int = 64):
     """ Tag as many [filepath] as you want with [model] """
     from tqdm import tqdm
     click.echo(click.style("Getting the tagger", bold=True))
     try:
-        tagger = sub.get_tagger(model, batch_size=batch_size, device=device, model_path=model_path)
+        tagger = utils.get_tagger(model, batch_size=batch_size, device=device, model_path=model_path)
     except FileNotFoundError as e:
         click.echo("Model not found: please make sure you have downloaded the model files with "
                    "pie-extended download " + model)
         if debug:
             raise e
         return
     failures = []
     for file in tqdm(filepath):
         try:
-            sub.tag_file(model, tagger, file, reset_exclude_patterns=reset_patterns,
-                         exclude_patterns=add_pattern)
+            utils.tag_file(
+                model, tagger, file, reset_exclude_patterns=reset_patterns,
+                exclude_patterns=add_pattern, no_tokenizer=no_tokenizer,
+                max_tokens=max_tokens)
         except Exception as E:
-            failures.append(E)
+            failures.append((file, E))
             click.echo("{} could not be lemmatized".format(file))
             if debug:
                 raise E
             if len(failures) > allowed_failure:
                 click.echo(
                     click.style("Too many errors, stopping the process", fg="red")
                 )
@@ -93,9 +101,22 @@
 
 
 @pie_ext.command("install-addons")
 @click.argument("model", type=click.Choice(MODELS, case_sensitive=False))
 def install(model):
     """ Install addons for specific models"""
     click.echo(click.style("Installing add-ons", bold=True))
-    sub.get_addons(model)
+    utils.get_addons(model)
     click.echo(click.style("Done", bold=True))
+
+
+@pie_ext.command("details")
+@click.argument("model", type=click.Choice(MODELS, case_sensitive=False))
+@click.option("--model_path", type=str, default=None,
+              help="Provide this with your own model path if you want to test it")
+def details(model: str, model_path: str = None):
+    """ Get details about known characters by the [model] """
+    from tqdm import tqdm
+    click.echo(click.style("Getting the tagger", bold=True))
+    tagger = utils.get_tagger(model, model_path=model_path)
+    for model, tasks in tagger.models:
+        print(sorted(list(model.label_encoder.char.table.keys())))
```

### Comparing `pie_extended-0.0.9/pie_extended/cli/sub.py` & `pie_extended-0.1.0/pie_extended/cli/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,76 @@
 import os
+import sys
 from typing import Tuple, Iterable, List, Union
 from importlib import import_module
 
 import requests
 
 from .. import models
 from ..utils import Metadata, PATH, get_path
 from ..tagger import ExtensibleTagger
 from ..utils import ObjectCreator
 from pie.utils import model_spec
 
 
+def check(model: str, force: bool = False) -> bool:
+    """ Check if files are available for a given model """
+    module = get_model(model)
+    return False not in [
+        os.path.exists(
+            get_path(model, file.name)
+        )
+        for file in module.DOWNLOADS
+    ] or force
+
+
 def get_model(model: str):
     """ Retrieve a module given a string
 
     :param model: Module Name
     :return: Module
     """
     return import_module("{}.{}".format(models.__name__, model))
 
 
 def get_imports(module):
     return import_module("{}.{}".format(module.__name__, "imports"))
 
 
+def _download(url, filename):
+    with open(filename, 'wb') as f:
+        response = requests.get(url, stream=True)
+        total = response.headers.get('content-length')
+
+        if total is None:
+            f.write(response.content)
+        else:
+            downloaded = 0
+            total = int(total)
+            for data in response.iter_content(chunk_size=max(int(total/1000), 1024*1024)):
+                downloaded += len(data)
+                f.write(data)
+                done = int(50*downloaded/total)
+                sys.stdout.write('\r[{}{}]'.format('█' * done, '.' * (50-done)))
+                sys.stdout.flush()
+    sys.stdout.write('\n')
+
+
 def download(module: str) -> Iterable[Union[str, int]]:
     """ Download dependencies for the given module
 
     :param module: Module for which to download models and static files in general
     """
     lemmatizer = get_model(module)
     os.makedirs(os.path.join(PATH, module), exist_ok=True)
     yield len(lemmatizer.DOWNLOADS)
     for file in lemmatizer.DOWNLOADS:
 
-        data = requests.get(file.url)
         new_path = get_path(module, file.name)
-
-        with open(new_path, "wb") as f:
-            f.write(data.content)
+        _download(file.url, new_path)
         yield file.name
 
 
 def get_list() -> Iterable[Tuple[str, Metadata]]:
     """ Retrieve a list of available modules
     """
     for module in models.modules:
@@ -72,35 +100,38 @@
     return tagger
 
 
 def tag_file(
         model: str, tagger: ExtensibleTagger,
         fpath: str,
         reset_exclude_patterns: bool = False,
-        exclude_patterns: List[str] = None):
+        exclude_patterns: List[str] = None,
+        no_tokenizer: bool = False,
+        max_tokens: int = 256):
     """ Tag a file with a given model
 
     :param model: Module name of the model
     :param tagger: Tagger that should be used
     :param fpath: Path to the file to edit
     :param reset_exclude_patterns: Remove all pre-registered token exclusion regular expressions
     :param exclude_patterns: New exclude patterns to add to the data iterator (Does not require reset)
+    :param no_tokenizer: Does not use usual tokenizers (new line = word separator, two new lines = sentence_
     """
     module = get_model(model)
-    iterator, processor = getattr(get_imports(module), "get_iterator_and_processor")()
+    iterator, processor = getattr(get_imports(module), "get_iterator_and_processor")(max_tokens=max_tokens)
     # Remove first pattern
     if reset_exclude_patterns:
         iterator.reset_patterns()
 
     # Add new
     if exclude_patterns:
         for pattern in exclude_patterns:
             iterator.add_pattern(pattern)
 
-    tagger.tag_file(fpath, iterator=iterator, processor=processor)
+    tagger.tag_file(fpath, iterator=iterator, processor=processor, no_tokenizer=no_tokenizer)
     return True
 
 
 def get_addons(model: str):
     """ Runs the `addons` function from a module """
     module = get_model(model)
     addons = getattr(get_imports(module), "addons", lambda: print("No add-ons needed for " + model))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pie_extended-0.0.9/pie_extended/models/fr/processor.py` & `pie_extended-0.1.0/pie_extended/models/fr/processor.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.0.9/pie_extended/models/fr/imports.py` & `pie_extended-0.1.0/pie_extended/models/freem/imports.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-from .processor import FrGlueProcessor
-from pie_extended.pipeline.postprocessor.proto import RenamedTaskProcessor
-from .tokenizer import FrMemorizingTokenizer
+from ..fr.tokenizer import FrMemorizingTokenizer
 from pie_extended.pipeline.iterators.proto import DataIterator
+from pie_extended.pipeline.postprocessor.proto import ProcessorPrototype, RenamedTaskProcessor
 from pie_extended.pipeline.postprocessor.memory import MemoryzingProcessor
+from ..fr.processor import FrGlueProcessor
 
 
-def get_iterator_and_processor():
+def get_iterator_and_processor(max_tokens=256):
     tokenizer = FrMemorizingTokenizer()
+
     processor = MemoryzingProcessor(
             tokenizer_memory=tokenizer,
             head_processor=FrGlueProcessor(
                 head_processor=RenamedTaskProcessor({"pos": "POS", "NOMB": "NOMB.", "PERS": "PERS."})
             )
         )
 
     iterator = DataIterator(
-        tokenizer=tokenizer
+        tokenizer=tokenizer,
+        max_tokens=max_tokens,
+        exclude_patterns=[
+            excl.exclude_regexp
+            for excl in tokenizer.normalizers
+            if excl.exclude_regexp
+        ]
     )
     return iterator, processor
```

### Comparing `pie_extended-0.0.9/pie_extended/models/fr/__init__.py` & `pie_extended-0.1.0/pie_extended/models/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.0.9/pie_extended/models/lasla/processor.py` & `pie_extended-0.1.0/pie_extended/pipeline/postprocessor/rulebased.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-import regex as re
-from typing import Dict
+from pie_extended.pipeline.postprocessor.proto import ProcessorPrototype, ChainedProcessor
+from typing import Optional, Dict, List
+if "typing" == "nottyping":
+    from ..tokenizers.memorizing import MemorizingTokenizer
 
-from pie_extended.pipeline.postprocessor.glue import GlueProcessor
-from pie_extended.pipeline.postprocessor.rulebased import RuleBasedProcessor
 
-
-class LatinRulesProcessor(RuleBasedProcessor):
-    """ Lasla data has no punctuation, we tag it automatically.
-
-    "ne" token can be two different lemma, but I don't remember why I wrote this part. (ne/nec ?)
+class RuleBasedProcessor(ChainedProcessor):
+    """ Applies rules found in rules(token_annotation)
 
     """
-    PONCTU = re.compile(r"^\W+$")
 
-    def rules(self, annotation: Dict[str, str]) -> Dict[str, str]:
-        # If Else condition
-        token = annotation["form"]
+    def __init__(self, apply_on_reinsert: bool = False, head_processor: Optional[ProcessorPrototype] = None, **kwargs):
+        """ Apply rules on output of the taggers
 
-        if self.PONCTU.match(token):
-            return {"form": token, "lemma": token, "pos": "PUNC", "morph": "MORPH=empty",
-                    "treated": annotation['treated']}
-        elif token.startswith("-"):
-            if token == "-ne":
-                annotation["lemma"] = "ne2"
-            else:
-                annotation["lemma"] = "ne"
-        return annotation
+        :param apply_on_reinsert: Apply rules on reinsert task
+        :param head_processor: Processor to use before post-processing its results
 
-    def __init__(self, *args, **kwargs):
-        super(LatinRulesProcessor, self).__init__(*args, **kwargs)
+        >>> class ExampleRule(RuleBasedProcessor):
+        ...     def rules(self, annotation: Dict[str, str]) -> Dict[str, str]:
+        ...         if annotation["form"] == "need":
+        ...             annotation["1"] = "REPLACED"
+        ...         return annotation
+        >>> processor = ExampleRule()
+        >>> processor.set_tasks(["1", "2"])
+        ['1', '2']
+        >>> processor.get_dict("token", ["a", "b"]) == [{"form": "token", "1": "a", "2": "b"}]
+        True
+        >>> processor.get_dict("need", ["a", "b"]) == [{"form": "need", "1": "REPLACED", "2": "b"}]
+        True
+        """
+        super(RuleBasedProcessor, self).__init__(head_processor=head_processor, **kwargs)
+        self.apply_on_reinsert = apply_on_reinsert
 
+    def rules(self, annotation: Dict[str, str]) -> Dict[str, str]:
+        return annotation
 
-class LatinGlueProcessor(GlueProcessor):
-    OUTPUT_KEYS = ["form", "lemma", "pos", "morph"]
-    GLUE = {"morph": ["Case", "Numb", "Deg", "Mood", "Tense", "Voice", "Person"]}
-    WHEN_EMPTY = {"morph": "MORPH=empty"}
+    def reinsert(self, form: str) -> Dict[str, str]:
+        anno = super(RuleBasedProcessor, self).reinsert(form)
+        if self.apply_on_reinsert:
+            return self.rules(anno)
+        return anno
 
-    def __init__(self, *args, **kwargs):
-        super(LatinGlueProcessor, self).__init__(*args, **kwargs)
+    def get_dict(self, token: str, tags: List[str]) -> List[Dict[str, str]]:
+        return [self.rules(anno) for anno in self.head_processor.get_dict(token, tags)]
```

### Comparing `pie_extended-0.0.9/pie_extended/models/lasla/tokenizer.py` & `pie_extended-0.1.0/pie_extended/models/lasla/tokenizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,103 +1,115 @@
 import regex as re
-import click
-import sys
-from typing import List, Generator
+from typing import List, Generator, Tuple
+from unidecode import unidecode
 
-from pie_extended.models.fro.tokenizer import _Dots_except_apostrophe, _RomanNumber
+from pie_extended.models.fro.tokenizer import _Dots_except_apostrophe
 from pie_extended.pipeline.tokenizers.memorizing import MemorizingTokenizer
-from pie_extended.models.lasla._params import ne_and_n, latin_replacements, ve
-
-try:
-    import cltk
-    from cltk.tokenize.latin.word import WordTokenizer
-except ImportError as E:
-    click.echo(click.style("You need to install cltk and its Latin Data to runs this package", fg="red"))
-    click.echo("pip install https://github.com/PonteIneptique/cltk/archive/latin_clitics_exceptions.zip")
-    click.echo("pie-extended install-addons lasla")
-    sys.exit(0)
-
-
-ENCLITICS = ['que', 'n', 'ne', 'ue', 've', 'st']
-BASE_ENCLITICS_EXCEPTIONS = set(ENCLITICS + cltk.tokenize.latin.params.latin_exceptions + ne_and_n + ve)
-ENCLITIC_EXCEPTIONS = list([
-    token
-    for token in BASE_ENCLITICS_EXCEPTIONS
-])
-ENCLITIC_EXCEPTIONS += [
-    token.lower().replace("v", "u").replace("j", "i")
-    for token in BASE_ENCLITICS_EXCEPTIONS
-]
-ENCLITIC_EXCEPTIONS += [
-    token.lower().replace("v", "u")
-    for token in BASE_ENCLITICS_EXCEPTIONS
-]
-ENCLITIC_EXCEPTIONS += [
-    token.lower().replace("j", "i")
-    for token in BASE_ENCLITICS_EXCEPTIONS
-]
-ENCLITIC_EXCEPTIONS = set(ENCLITIC_EXCEPTIONS)
+from pie_extended.models.lasla._params import abbrs
+from pie_extended.pipeline.tokenizers.utils.excluder import (
+    ReferenceExcluder,
+    ExcluderPrototype,
+    RegexpExcluder,
+    AbbreviationsRemoverExcluder,
+    DEFAULT_CHAR_REGISTRY
+)
+from pie_extended.pipeline.tokenizers.utils import regexps
+from pie_extended.utils import roman_number
 
 
 class LatMemorizingTokenizer(MemorizingTokenizer):
     re_add_space_around_punct = re.compile(r"(\s*)([^\w\s])(\s*)")
+    re_words = re.compile("^\w+$")
     _sentence_boundaries = re.compile(
         r"([" + _Dots_except_apostrophe + r"]+\s*)+"
     )
-    roman_number_dot = re.compile(r"\.(" + _RomanNumber + r")\.")
+    re_roman_number = re.compile(r"^"+regexps.RomanNumbers+"$")
 
     def __init__(self):
         super(LatMemorizingTokenizer, self).__init__()
         self.tokens = []
-        self._word_tokenizer = WordTokenizer()
+        self.char_registry = DEFAULT_CHAR_REGISTRY
+        self.normalizers: Tuple[ExcluderPrototype, ...] = (
+            ReferenceExcluder(char_registry=self.char_registry),
+            ReferenceExcluder(regex_string=r"(\[IGN:[^\]]+\])", char_registry=self.char_registry),
+            RegexpExcluder(r"(\p{Greek}+)"),
+            RegexpExcluder(r"(\p{No})"),
+            AbbreviationsRemoverExcluder(abbrs=abbrs, char_registry=self.char_registry)
+        )
 
     @staticmethod
     def _sentence_tokenizer_merge_matches(match):
         """ Best way we found to deal with repeating groups"""
         start, end = match.span()
         return match.string[start:end] + "<SPLIT>"
 
-    @classmethod
-    def _real_sentence_tokenizer(cls, string: str) -> List[str]:
-        string = cls._sentence_boundaries.sub(cls._sentence_tokenizer_merge_matches, string)
-        string = string.replace("_DOT_", ".")
+    def _real_sentence_tokenizer(self, string: str) -> List[str]:
+        string = self._sentence_boundaries.sub(self._sentence_tokenizer_merge_matches, string)
+
+        for normalizer in self.normalizers:
+            string = normalizer.after_sentence_tokenizer(string)
+
         return string.split("<SPLIT>")
 
     def _real_word_tokenizer(self, text: str, lower: bool = False) -> List[str]:
-        tokenized = [tok for tok in self._word_tokenizer.tokenize(
-            text,
-            replacements=latin_replacements,
-            enclitics_exceptions=ENCLITIC_EXCEPTIONS
-        ) if tok]
-        if tokenized:
-            tokenized = [tok.lower() for tok in tokenized]
-        return tokenized
+        if lower is True:
+            text = text.lower()
+        return text.split()
 
     def sentence_tokenizer(self, text: str, lower: bool = False) -> Generator[List[str], None, None]:
         """
 
         >>> x = LatMemorizingTokenizer()
-        >>> list(x.sentence_tokenizer("Lasciva puella et lasciue Agamemnone whateverve."))
-        [['lasciua', 'puella', 'et', 'lasciue', 'agamemnone', 'whateuer', '-ue', '.']]
+        >>> list(x.sentence_tokenizer("XX Lasciva puella et lasciue C. Agamemnone whateverve."))
+        [['3', 'Lasciua', 'puella', 'et', 'lasciue', 'C', 'Agamemnone', 'whateuerue', '.']]
 
         """
         sentences = list()
         data = self.normalizer(text)
         for sent in self._real_sentence_tokenizer(data):
             sent = sent.strip()
             if sent:
                 sentences.append(self.word_tokenizer(sent))
         yield from sentences
 
     def normalizer(self, data: str) -> str:
+        for excluder in self.normalizers:
+            data = excluder.before_sentence_tokenizer(data)
+
         data = self.re_add_space_around_punct.sub(
-                    r" \g<2> ",
-                    self.roman_number_dot.sub(
-                        r"_DOT_\g<1>_DOT_",
-                        data
-                    )
-                )
+            r" \g<2> ",
+            data
+        )
         return data
 
+    def roman_to_number(self, inp: str) -> str:
+        out = roman_number(inp)
+        if out > 3:
+            out = 3
+        return str(out)
+
     def replacer(self, inp: str):
-        inp = inp.replace("V", "U").replace("v", "u").replace("J", "I").replace("j", "i")
+        """
+
+        :param inp:
+        :return:
+
+        """
+        for excluder in self.normalizers:
+            if not excluder.can_be_replaced and excluder.exclude_regexp.match(inp):
+                return inp
+        if self.re_roman_number.match(inp):
+            return self.roman_to_number(inp)
+        elif inp.isnumeric():
+            if inp.isdigit():  # avoid. ↀ
+                if int(inp) > 3:
+                    return "3"
+                else:
+                    return inp
+            return "3"
+        elif "." == inp:
+            return "."
+
+        if self.re_words.match(inp):  # Might check somehow else but for now... It's weird unidecode normalize into SS
+            inp = unidecode(inp)
+        inp = inp.replace("V", "U").replace("v", "u").replace("J", "I").replace("j", "i").replace(".", "")#.lower()
         return inp
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pie_extended-0.0.9/pie_extended/models/fro/processor.py` & `pie_extended-0.1.0/pie_extended/models/fro/processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,12 +32,20 @@
 
 class FroGlueProcessor(GlueProcessor):
     """ We glue morphological features into one column
 
     """
     OUTPUT_KEYS = ["form", "lemma", "POS", "morph"]
     GLUE = {"morph": ["MODE", "TEMPS", "PERS.", "NOMB.", "GENRE", "CAS", "DEGRE"]}
-    EMPTY_TAG: Dict[str, str] = {"CAS": "_", "NOMB.": "_", "DEGRE": "_", "MODE": "_", "TEMPS": "_", "GENRE": "_",
-                                 "PERS.": "_"}
+    EMPTY_TAG: Dict[str, str] = {"CAS": "CAS=x",
+                                 "NOMB.": "NOMB.=x",
+                                 "DEGRE": "DEGRE=x",
+                                 "MODE": "MODE=x",
+                                 "TEMPS": "TEMPS=x",
+                                 "GENRE": "GENRE=x",
+                                 "PERS.": "PERS.=x"}
 
     def __init__(self, *args, **kwargs):
-        super(FroGlueProcessor, self).__init__(*args, **kwargs)
+        super(FroGlueProcessor, self).__init__(*args, **kwargs)
+    
+    def _get_glued(self, glued_task: str, token_dict: Dict[str, str]):
+        return token_dict[glued_task]  # Tempfix because tasks contains their own name
```

### Comparing `pie_extended-0.0.9/pie_extended/models/fro/imports.py` & `pie_extended-0.1.0/pie_extended/models/fro/imports.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from .processor import FroRulesProcessor, FroGlueProcessor
 from pie_extended.pipeline.postprocessor.proto import RenamedTaskProcessor
 from .tokenizer import FroMemorizingTokenizer
 from pie_extended.pipeline.iterators.proto import DataIterator, GenericExcludePatterns
 from pie_extended.pipeline.postprocessor.memory import MemoryzingProcessor
 
 
-def get_iterator_and_processor():
+def get_iterator_and_processor(max_tokens=256):
     tokenizer = FroMemorizingTokenizer()
     processor = FroRulesProcessor(
         apply_on_reinsert=True,
         head_processor=MemoryzingProcessor(
             tokenizer_memory=tokenizer,
             head_processor=FroGlueProcessor(
                 head_processor=RenamedTaskProcessor({"pos": "POS", "NOMB": "NOMB.", "PERS": "PERS."})
             )
         )
     )
     iterator = DataIterator(
         tokenizer=tokenizer,
-        exclude_patterns=[GenericExcludePatterns.Punctuation_and_Underscore]
+        exclude_patterns=[
+            excl.exclude_regexp
+            for excl in tokenizer.normalizers
+            if excl.exclude_regexp
+        ] + [
+            GenericExcludePatterns.Punctuation_and_Underscore
+        ],
+        max_tokens=max_tokens
     )
     return iterator, processor
```

### Comparing `pie_extended-0.0.9/pie_extended/pipeline/formatters/proto.py` & `pie_extended-0.1.0/pie_extended/pipeline/formatters/proto.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
     """
     format_line: Callable[[Dict[str, str]], List[str]]
 
     def __init__(self, tasks: List[str]):
         self.tasks: List[str] = tasks
 
-        if sys.version_info.minor <= 6:
-            # Before 3.7, order of dictionary is not guaranteed
-            # Cf. https://mail.python.org/pipermail/python-dev/2017-December/151283.html
-            self.format_line = self.format_line_3_6
-        else:
-            self.format_line = self.format_line_3_7
+        # Before 3.7, order of dictionary is not guaranteed
+        # Cf. https://mail.python.org/pipermail/python-dev/2017-December/151283.html
+        self.format_line = self.format_line_3_6
+        # With post-processing, it's better to not trust order
+        #else:
+        #    self.format_line = self.format_line_3_7
 
     def format_line_3_6(self, annotation: Dict[str, str]) -> List[str]:
         """ Format the tags """
         return [annotation["form"]] + [annotation[task] for task in self.tasks]
 
     def format_line_3_7(self, annotation: Dict[str, str]) -> List[str]:
         """ Format the tags """
```

### Comparing `pie_extended-0.0.9/pie_extended/pipeline/iterators/proto.py` & `pie_extended-0.1.0/pie_extended/pipeline/iterators/proto.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,24 +12,26 @@
     """
     Punctuation_and_Underscore: Pattern = re.compile(r"^[_||[^\s\w]]+$", re.VERSION1)
     Punctuation: Pattern = re.compile(r"^[^\s\w]+$")
     PassageMarker: Pattern = re.compile(r"_Passage_[\w\d_]+")  # Use `_` as a joining character
 
 
 class DataIterator:
-    def __init__(self, tokenizer: SimpleTokenizer = None, exclude_patterns: List[Union[str, Pattern]] = None):
+    def __init__(self, tokenizer: SimpleTokenizer = None, exclude_patterns: List[Union[str, Pattern]] = None,
+                 max_tokens: int = 256):
         """ Iterator used to parse the text and returns bits to tag
 
         :param tokenizer: Tokenizer
         """
         self.tokenizer: SimpleTokenizer = tokenizer or SimpleTokenizer()
         self.exclude_patterns: List[Pattern] = []
         if exclude_patterns:
             for pattern in exclude_patterns:
                 self.add_pattern(pattern)
+        self.max_tokens = max_tokens
 
     def add_pattern(self, pattern: str):
         """ Add a pattern for removal
 
         :param pattern: Pattern for token removal
         """
         if isinstance(pattern, str):
@@ -89,18 +91,43 @@
                     match = True
                     break
             if not match:
                 clean.append(token)
 
         return clean, removed
 
-    def __call__(self, data: str, lower: bool = False) -> Iterable[Tuple[List[str], int, Dict[int, str]]]:
+    def _max_out(self, sentences):
+        for sentence in sentences:
+            if len(sentence) <= self.max_tokens:
+                yield sentence
+            else:
+                for n in range(0, len(sentence), self.max_tokens):
+                    yield sentence[n:n+self.max_tokens]
+
+    def __call__(self, data: str, lower: bool = False,
+                 no_tokenizer: bool = False) -> Iterable[Tuple[List[str], int, Dict[int, str]]]:
         """ Default iter data takes a text, an option to make lower
         and yield lists of words along with the length of the list
 
         :param data: A plain text
         :param lower: Whether or not to lower the text
         :yields: (Sentence as a list of word, Size of the sentence, Elements removed from the sentence)
         """
-        for sentence in self.tokenizer.sentence_tokenizer(data, lower=lower):
+        sentences = []
+
+        func = self.tokenizer.sentence_tokenizer
+        if no_tokenizer:
+            func = self.tokenizer.bypass_tokenizer
+
+        last_sentence_index = 0
+        for sentence in self._max_out(func(data, lower=lower)):
             clean_sentence, removed_from_input = self.exclude_tokens(sentence)
-            yield clean_sentence, len(clean_sentence), removed_from_input
+            if len(clean_sentence) == 0 and len(sentences):
+                sentences[-1][2].update({
+                    last_sentence_index + removed_index: removed_value
+                    for removed_index, removed_value in removed_from_input.items()
+                })
+                last_sentence_index += len(removed_from_input)
+            else:
+                sentences.append((clean_sentence, len(clean_sentence), removed_from_input))
+                last_sentence_index = len(sentence)
+        yield from sentences
```

### Comparing `pie_extended-0.0.9/pie_extended/pipeline/tokenizers/simple_tokenizer.py` & `pie_extended-0.1.0/pie_extended/pipeline/tokenizers/simple_tokenizer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Generator, List
 import regex as re
 import string
 from pie.tagger import regexsplitter, SECTION, FULLSTOP
 
 WORD = r'([{}])'.format(string.punctuation)
 
+RE_BYPASS_SENTENCE = re.compile(r"(?:\r?\n){2,}")
+RE_BYPASS_WORD = re.compile(r"(?:\r?\n)")
+
 
 class SimpleTokenizer(object):
     """ Tokenizer that memoryze what it tokenized.
 
     Mostly used to normalized input as input time and then reinserting normalized input
 
     """
@@ -27,7 +30,44 @@
         if lower:
             sentence = [w.lower() for w in sentence]
         return sentence
 
     def reset(self):
         """Can be used between documents for example """
         pass
+
+    def bypass_tokenizer(self, data: str, lower: bool = False) -> Generator[List[str], None, None]:
+        """ Function to enable pretokenized input while using replaces or the likes
+
+        :param data: The string (one new line = one word, two new lines = two words)
+        :param lower: Whether to lower the input
+
+
+        >>> tokenizer = SimpleTokenizer()
+        >>> list(tokenizer.bypass_tokenizer("one\\ntwo\\nthree\\n\\n.//.\\na\\nz"))
+        [['one', 'two', 'three'], ['.//.', 'a', 'z']]
+        """
+
+        for sentence in RE_BYPASS_SENTENCE.split(data):
+            if sentence:
+                yield [word for word in RE_BYPASS_WORD.split(sentence) if word]
+
+
+class LengthTokenizer(SimpleTokenizer):
+    def __init__(self, max_len=35):
+        super(LengthTokenizer, self).__init__()
+        self.max_len = max_len
+
+    def sentence_tokenizer(self, text: str, lower: bool = False) -> Generator[List[str], None, None]:
+        sentence = []
+        for token in text.split():
+            sentence.append(token)
+            if len(sentence) == self.max_len:
+                yield sentence
+                sentence = []
+        if sentence:
+            yield sentence
+
+    def word_tokenizer(self, text: str, lower: bool = False) -> List[str]:
+        if lower:
+            return text.lower().split()
+        return text.split()
```

### Comparing `pie_extended-0.0.9/pie_extended/pipeline/postprocessor/glue.py` & `pie_extended-0.1.0/pie_extended/pipeline/postprocessor/glue.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,44 +46,49 @@
     # Glue_char is what is used to glue things together -> Tense=Pres|Person=1
     GLUE_CHAR: str = "|"
     # Glue Empty are value to take when all things glued together are empty
     GLUE_EMPTY: Dict[str, str] = {"morph": "MORPH=empty"}
     # Value that means the current element is empty
     EMPTY_TAG: Dict[str, str] = {"Case": "_", "Numb": "_", "Deg": "_", "Mood": "_", "Tense": "_", "Voice": "_",
                                  "Person": "_"}
+    KEEP_EMPTY = False
 
     def __init__(self, *args, **kwargs):
         super(GlueProcessor, self).__init__(*args, **kwargs)
 
         # Sets-up some copy of the values
         self._out = self.OUTPUT_KEYS
         self._glue = self.GLUE
         self._glue_char = self.GLUE_CHAR
         self._glue_empty = self.GLUE_EMPTY
         self._empty_tags = self.EMPTY_TAG
+        self._keep_empty = self.KEEP_EMPTY
 
     def _yield_annotation(
             self, 
             token_dict: Dict[str, str]
         ) -> Generator[str, None, None]:
         # For each key we should return
         for head in self._out:
             if head not in self._glue:
                 yield head, token_dict[head]
             else:
                 # Otherwise, we glue together things that should be glued together
                 joined = self._glue_char.join([
-                    glued_task + "=" + token_dict[glued_task]
+                    self._get_glued(glued_task, token_dict)
                     for glued_task in self._glue[head]
-                    if token_dict[glued_task] != self._empty_tags.get(glued_task, None)
+                    if self._keep_empty or token_dict[glued_task] != self._empty_tags.get(glued_task, None)
                 ])
                 if not joined:
                     joined = self._glue_empty[head]
                 yield head, joined
 
+    def _get_glued(self, glued_task: str, token_dict: Dict[str, str]):
+        return glued_task + "=" + token_dict[glued_task]
+
     def reinsert(self, form: str) -> Dict[str, str]:
         return dict(form=form, **{key: self.empty_value for key in self._out if key != "form"})
 
     def get_dict(self, token: str, tags: List[str]) -> List[Dict[str, str]]:
         return [dict(self._yield_annotation(as_dict)) for as_dict in super(GlueProcessor, self).get_dict(token, tags)]
 
     @property
```

### Comparing `pie_extended-0.0.9/pie_extended/pipeline/postprocessor/splitter.py` & `pie_extended-0.1.0/pie_extended/pipeline/postprocessor/splitter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List, Dict, Optional
 from .proto import ChainedProcessor, ProcessorPrototype
+from copy import deepcopy
 
 
 class SplitterPostProcessor(ChainedProcessor):
     """ This processor aims to help in splitting enclitics and proclitics
 
 
     >>> proc = SplitterPostProcessor()
@@ -22,31 +23,41 @@
     >>> proc.set_tasks(["lemma", "POS", "Case"])
     ['lemma', 'POS', 'Case']
     >>> proc.get_dict("praedicatione", ["praedicatio界-ne", "NOMcom", "Nominatif"]) == [
     ...    {"form": "praedicatione", "lemma": "praedicatio界-ne", "POS": "NOMcom", "Case": "Nominatif"},
     ...    {"form": "praedicatione", "lemma": "praedicatio界-ne", "POS": "NOMcom", "Case": "Nominatif"}
     ... ]
     True
+    >>> proc = SplitterPostProcessor(keep=False, prefix="界")
+    >>> proc.set_tasks(["lemma", "POS", "Case"])
+    ['lemma', 'POS', 'Case']
+    >>> proc.get_dict("praedicatione", ["praedicatio界ne", "NOMcom", "Nominatif"]) ==  [
+    ...    {"form": "praedicatione", "lemma": "praedicatio", "POS": "NOMcom", "Case": "Nominatif"},
+    ...    {"form": "praedicatione", "lemma": "界ne", "POS": "NOMcom", "Case": "Nominatif"}
+    ... ]
+    True
     """
 
     def __init__(self, split_char: str = "界", column: str = "lemma", keep: bool = False,
-                 head_processor: Optional[ProcessorPrototype] = None, **kwargs):
+                 head_processor: Optional[ProcessorPrototype] = None, prefix: str = "", **kwargs):
         super(SplitterPostProcessor, self).__init__(head_processor, **kwargs)
-        self.split_char = split_char
-        self.column = column
-        self.keep = keep
+        self.split_char: str = split_char
+        self.column: str = column
+        self.keep: bool = keep
+        self.prefix: str = prefix
 
     def get_dict(self, token: str, tags: List[str]) -> List[Dict[str, str]]:
         out = []
         for anno in super(SplitterPostProcessor, self).get_dict(token=token, tags=tags):
             if self.split_char in anno[self.column]:
-                for new_val in anno[self.column].split(self.split_char):
+                for number, new_val in enumerate(anno[self.column].split(self.split_char)):
+                    if number > 0:
+                        new_val = self.prefix + new_val
                     if self.keep:
                         out.append(anno)
                     else:
-                        out.append({
-                            self.column: new_val,
-                            **{x: y for x, y in anno.items() if x != self.column}
-                        })
+                        new = deepcopy(anno)
+                        new[self.column] = new_val
+                        out.append(new)
             else:
                 out.append(anno)
         return out
```

### Comparing `pie_extended-0.0.9/pie_extended/pipeline/postprocessor/proto.py` & `pie_extended-0.1.0/pie_extended/pipeline/postprocessor/proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Optional, Type
+from typing import List, Dict, Optional, Type, Generator, Tuple
 
 DEFAULT_EMPTY = "_"
 
 
 class ProcessorPrototype:
     empty_value: str
```

### Comparing `pie_extended-0.0.9/pie_extended/pipeline/postprocessor/memory.py` & `pie_extended-0.1.0/pie_extended/pipeline/postprocessor/memory.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.0.9/pie_extended/tagger.py` & `pie_extended-0.1.0/pie_extended/tagger.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,44 +18,57 @@
         super(ExtensibleTagger, self).__init__(
             device=device,
             batch_size=batch_size,
             lower=lower
         )
         self.disambiguation: Optional[Disambiguator] = disambiguation
 
-    def tag_file(self, fpath: str, iterator: DataIterator, processor: ProcessorPrototype):
+    def tag_file(self, fpath: str, iterator: DataIterator, processor: ProcessorPrototype, no_tokenizer: bool = False):
         # Read content of the file
         with open(fpath) as f:
             data = f.read()
 
         _, ext = os.path.splitext(fpath)
 
         out_file = utils.ensure_ext(fpath, ext, 'pie')
         with open(out_file, 'w+') as f:
-            for line in self.iter_tag(data, iterator, processor=processor):
+            for line in self.iter_tag(data, iterator, processor=processor, no_tokenizer=no_tokenizer):
                 f.write(line)
 
         return out_file
 
-    def tag_str(self, data: str, iterator: DataIterator, processor: ProcessorPrototype) -> str:
-        return list(self.iter_tag_token(data, iterator, processor=processor))
-
-    def iter_tag_token(self, data: str, iterator: DataIterator, processor: ProcessorPrototype) \
-            -> Generator[Dict[str, str], None, None]:
+    def tag_str(self, data: str, iterator: DataIterator, processor: ProcessorPrototype,
+                no_tokenizer: bool = False) -> str:
+        return list(self.iter_tag_token(data, iterator, processor=processor, no_tokenizer=no_tokenizer))
+
+    def iter_tag_token(self,
+                       data: str,
+                       iterator: DataIterator,
+                       processor: ProcessorPrototype,
+                       no_tokenizer: bool = False,
+                       empty_token_on_sent_break: bool = False) -> Generator[Optional[Dict[str, str]], None, None]:
+        """ Reads the string in [DATA] with [ITERATOR] and [PROCESSOR], then returns each token as a dict
+
+        :param data: Textual
+        :param iterator: Iterator used to read data
+        :param processor: Processor used to post-process data
+        :param no_tokenizer: Disable the tokenizer inside the iterator
+        :param empty_token_on_sent_break: Returns a None token when going into a new sequence.
+        :yield: Token in the form of a dict or, if [empty_token...] is True, a None value when changing "sentences"
+        """
         # Reset at each document
         processor.reset()
         iterator.tokenizer.reset()
         # Iterate !
         for chunk in utils.chunks(
-                iterator(data, lower=self.lower),
+                iterator(data, lower=self.lower, no_tokenizer=no_tokenizer),
                 size=self.batch_size):
 
             # Unzip the batch into the sentences, their sizes and the dictionaries of things that needs
             #  to be reinserted
-
             sents, lengths, needs_reinsertion = zip(*chunk)
             is_empty = [not bool(sent) for sent in sents]
 
             tagged, tasks = self.tag(
                 sents=[sent for sent in sents if sent],
                 lengths=[l for l in lengths if l != 0]
             )
@@ -86,20 +99,22 @@
                         del sent_reinsertion[reinsertion_index + index]
                         reinsertion_index += 1
 
                     yield from processor.get_dict(token, tags)
 
                 for reinsertion in sorted(list(sent_reinsertion.keys())):
                     yield processor.reinsert(sent_reinsertion[reinsertion])
+                if empty_token_on_sent_break:
+                    yield None
 
     def iter_tag(self, data: str, iterator: DataIterator, processor: ProcessorPrototype,
-                 formatter_class: Type[Formatter] = Formatter):
+                 formatter_class: Type[Formatter] = Formatter, no_tokenizer: bool = False):
         formatter = None
 
-        for annotation in self.iter_tag_token(data, iterator, processor):
+        for annotation in self.iter_tag_token(data, iterator, processor, no_tokenizer = no_tokenizer):
             if not formatter:
                 formatter = formatter_class(processor.tasks)
                 yield formatter.write_headers()
             yield formatter.write_line(formatter.format_line(annotation))
 
         if formatter:
-            yield formatter.write_footer()
+            yield formatter.write_footer()
```

### Comparing `pie_extended-0.0.9/PKG-INFO` & `pie_extended-0.1.0/pie_extended.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,136 +1,176 @@
 Metadata-Version: 2.1
-Name: pie_extended
-Version: 0.0.9
+Name: pie-extended
+Version: 0.1.0
 Summary: Extension for nlp-pie package
-Home-page: https://github.com/ponteineptique/nlp-pie-taggers
+Home-page: https://github.com/hipster-philology/nlp-pie-taggers
 Author: Thibault Clérice
 License: MIT
-Description: 
-        # Pie Extended
-        
-        [![Build Status](https://travis-ci.org/hipster-philology/nlp-pie-taggers.svg?branch=master)](https://travis-ci.org/hipster-philology/nlp-pie-taggers)
-        [![Coverage Status](https://coveralls.io/repos/github/hipster-philology/nlp-pie-taggers/badge.svg?branch=master)](https://coveralls.io/github/hipster-philology/nlp-pie-taggers?branch=master)
-        ![PyPI](https://img.shields.io/pypi/v/pie-extended?style=flat-square)
-        
-        Extension for [`pie`](https://github.com/emanjavacas/pie) to include taggers with their models and pre/postprocessors.
-        
-        Pie is a wonderful tool to train models. And most of the time, it will be enough. What `pie_extended` is proposing here 
-        is to provide you with the necessary tools to share your models with customized pre- and post-processing.
-        
-        The current system provide an easier access to adding **customized**:
-        - normalization of your text,
-        - sentence tokenization,
-        - word tokenization,
-        - disambiguation,
-        - output formatting
-        
-        ## Install
-        
-        To install, simply do `pip install pie-extended`. Then, look at all available models.
-        
-        ## Run on terminal
-        
-        But on top of that, it provides a quick and easy way to use others models ! For example, in a shell :
-        
-        ```bash
-        pie-extended download lasla
-        pie-extended install-addons lasla
-        pie-extended tag laslsa your_file.txt
-        ```
-        
-        will give you access to all you need !
-        
-        ## Python API
-        
-        You can run the lemmatizer in your own scripts and retrieve token annotations as dictionaries:
-        
-        ```python
-        from typing import List
-        from pie_extended.cli.sub import get_tagger, get_model, download
-        
-        # In case you need to download
-        do_download = False
-        if do_download:
-            for dl in download("lasla"):
-                x = 1
-        
-        # model_path allows you to override the model loaded by another .tar
-        model_name = "lasla"
-        tagger = get_tagger(model_name, batch_size=256, device="cpu", model_path=None)
-        
-        sentences: List[str] = ["Lorem ipsum dolor sit amet, consectetur adipiscing elit. "]
-        # Get the main object from the model (: data iterator + postprocesor
-        from pie_extended.models.lasla.imports import get_iterator_and_processor
-        for sentence_group in sentences:
-            iterator, processor = get_iterator_and_processor()
-            print(tagger.tag_str(sentence_group, iterator=iterator, processor=processor) )
-        ```
-        
-        will result in
-        
-        ```python
-        [{'form': 'lorem', 'lemma': 'lor', 'POS': 'NOMcom', 'morph': 'Case=Acc|Numb=Sing', 'treated': 'lorem'},
-         {'form': 'ipsum', 'lemma': 'ipse', 'POS': 'PROdem', 'morph': 'Case=Acc|Numb=Sing', 'treated': 'ipsum'},
-         {'form': 'dolor', 'lemma': 'dolor', 'POS': 'NOMcom', 'morph': 'Case=Nom|Numb=Sing', 'treated': 'dolor'},
-         {'form': 'sit', 'lemma': 'sum1', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Act|Person=3',
-          'treated': 'sit'},
-         {'form': 'amet', 'lemma': 'amo', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Act|Person=3',
-          'treated': 'amet'}, {'form': ',', 'lemma': ',', 'pos': 'PUNC', 'morph': 'MORPH=empty', 'treated': ','},
-         {'form': 'consectetur', 'lemma': 'consector2', 'POS': 'VER',
-          'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Dep|Person=3', 'treated': 'consectetur'},
-         {'form': 'adipiscing', 'lemma': 'adipiscor', 'POS': 'VER', 'morph': 'Tense=Pres|Voice=Dep', 'treated': 'adipiscing'},
-         {'form': 'elit', 'lemma': 'elio', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Ind|Tense=Pres|Voice=Act|Person=3',
-          'treated': 'elit'}, {'form': '.', 'lemma': '.', 'pos': 'PUNC', 'morph': 'MORPH=empty', 'treated': '.'}]
-        ```
-        
-        ## Add a model
-        
-        - Create a package in `./pie_extended/models/`. Exemple: `foo`.
-        - Add the name of the package in `./pie_extended/models/__init__.py` in the variable `modules`.
-        - In the module `pie_extended.models.foo`, we should find the following variable:
-            - `Models` : a string with filenames and tasks for Pie.
-            - `DESC`: a METADATA object that bears information about the model
-            - `DOWNLOADS`: A list of file to download.
-            
-        ```python
-        from pie_extended.utils import Metadata, File, get_path
-        
-        DESC = Metadata(
-            "Foo"
-            "language",
-            ["Author 1", "Author 2"],
-            "A readable description",
-            "A link to more information"
-        )
-        
-        DOWNLOADS = [
-            File("/a/link/to/a/file", "local_name_of_the_file.tar")
-        ]
-        
-        
-        Models = "<{},task1,task2><{},lemma,pos>".format(
-            get_path("foo", "local_name_of_the_file.tar")
-        )
-        
-        ```
-        - In the module `pie_extended.models.foo.imports`, we should find the following content:
-            1. `get_iterator_and_processor`: a function that returns a `DataIterator` and a `Processor` 
-            2. (optionally) `addons`: a function that installs add-ons
-            3. (optionally) `Disambiguator`: a disambiguator instance (or an object creator that returns one)
-        
-        Check for a simple example in `pie_extended.models.fro.imports` and a more complex one 
-        in `pie_extended.models.lasla.imports`
-        
-        ## Warning
-        
-        This is an extremely early build, subject to change here and there. But it is functional !
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Pie Extended
+
+[![Build Status](https://travis-ci.org/hipster-philology/nlp-pie-taggers.svg?branch=master)](https://travis-ci.org/hipster-philology/nlp-pie-taggers)
+[![Coverage Status](https://coveralls.io/repos/github/hipster-philology/nlp-pie-taggers/badge.svg?branch=master)](https://coveralls.io/github/hipster-philology/nlp-pie-taggers?branch=master)
+![PyPI](https://img.shields.io/pypi/v/pie-extended?style=flat-square)
+
+**Warning**: This software is only compatible with up to Python 3.7 for the moment.
+
+Extension for [`pie`](https://github.com/emanjavacas/pie) to include taggers with their models and pre/postprocessors.
+
+Pie is a wonderful tool to train models. And most of the time, it will be enough. What `pie_extended` is proposing here 
+is to provide you with the necessary tools to share your models with customized pre- and post-processing.
+
+The current system provide an easier access to adding **customized**:
+- normalization of your text,
+- sentence tokenization,
+- word tokenization,
+- disambiguation,
+- output formatting
+
+## Cite as
+
+```
+@software{thibault_clerice_2020_3883590,
+  author       = {Clérice, Thibault},
+  title        = {Pie Extended, an extension for Pie with pre-processing and post-processing},
+  month        = jun,
+  year         = 2020,
+  publisher    = {Zenodo},
+  doi          = {10.5281/zenodo.3883589},
+  url          = {https://doi.org/10.5281/zenodo.3883589}
+}
+```
+
+## Current supported languages
+
+- Classical Latin (Model: `lasla`)
+- Ancient Greek (Model: `grc`)
+- Old French (Model: `fro`)
+- Early Modern French (Model: `freem`)
+- Classical French (Model: `fr`)
+- Old Dutch (Model: `dum`)
+
+If you trained models and want some help sharing them with Pie Extended, open an issue :)
+
+## Install
+
+To install, simply do `pip install pie-extended`. Then, look at all available models.
+
+## Run on terminal
+
+But on top of that, it provides a quick and easy way to use others models ! For example, in a shell :
+
+```bash
+pie-extended download lasla
+pie-extended install-addons lasla
+pie-extended tag lasla your_file.txt
+```
+
+will give you access to all you need !
+
+## Python API
+
+You can run the lemmatizer in your own scripts and retrieve token annotations as dictionaries:
+
+```python
+from typing import List
+from pie_extended.cli.utils import get_tagger, get_model, download
+
+# In case you need to download
+do_download = False
+if do_download:
+    for dl in download("lasla"):
+        x = 1
+
+# model_path allows you to override the model loaded by another .tar
+model_name = "lasla"
+tagger = get_tagger(model_name, batch_size=256, device="cpu", model_path=None)
+
+sentences: List[str] = ["Lorem ipsum dolor sit amet, consectetur adipiscing elit. "]
+# Get the main object from the model (: data iterator + postprocesor
+from pie_extended.models.lasla.imports import get_iterator_and_processor
+for sentence_group in sentences:
+    iterator, processor = get_iterator_and_processor()
+    print(tagger.tag_str(sentence_group, iterator=iterator, processor=processor) )
+```
+
+will result in
+
+```python
+[{'form': 'lorem', 'lemma': 'lor', 'POS': 'NOMcom', 'morph': 'Case=Acc|Numb=Sing', 'treated': 'lorem'},
+ {'form': 'ipsum', 'lemma': 'ipse', 'POS': 'PROdem', 'morph': 'Case=Acc|Numb=Sing', 'treated': 'ipsum'},
+ {'form': 'dolor', 'lemma': 'dolor', 'POS': 'NOMcom', 'morph': 'Case=Nom|Numb=Sing', 'treated': 'dolor'},
+ {'form': 'sit', 'lemma': 'sum1', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Act|Person=3',
+  'treated': 'sit'},
+ {'form': 'amet', 'lemma': 'amo', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Act|Person=3',
+  'treated': 'amet'}, {'form': ',', 'lemma': ',', 'pos': 'PUNC', 'morph': 'MORPH=empty', 'treated': ','},
+ {'form': 'consectetur', 'lemma': 'consector2', 'POS': 'VER',
+  'morph': 'Numb=Sing|Mood=Sub|Tense=Pres|Voice=Dep|Person=3', 'treated': 'consectetur'},
+ {'form': 'adipiscing', 'lemma': 'adipiscor', 'POS': 'VER', 'morph': 'Tense=Pres|Voice=Dep', 'treated': 'adipiscing'},
+ {'form': 'elit', 'lemma': 'elio', 'POS': 'VER', 'morph': 'Numb=Sing|Mood=Ind|Tense=Pres|Voice=Act|Person=3',
+  'treated': 'elit'}, {'form': '.', 'lemma': '.', 'pos': 'PUNC', 'morph': 'MORPH=empty', 'treated': '.'}]
+```
+
+## Add a model
+
+- Create a package in `./pie_extended/models/`. Exemple: `foo`.
+- Add the name of the package in `./pie_extended/models/__init__.py` in the variable `modules`.
+- In the module `pie_extended.models.foo`, we should find the following variable:
+    - `Models` : a string with filenames and tasks for Pie.
+    - `DESC`: a METADATA object that bears information about the model
+    - `DOWNLOADS`: A list of file to download.
+    
+```python
+from pie_extended.utils import Metadata, File, get_path
+
+DESC = Metadata(
+    "Foo"
+    "language",
+    ["Author 1", "Author 2"],
+    "A readable description",
+    "A link to more information"
+)
+
+DOWNLOADS = [
+    File("/a/link/to/a/file", "local_name_of_the_file.tar")
+]
+
+
+Models = "<{},task1,task2><{},lemma,pos>".format(
+    get_path("foo", "local_name_of_the_file.tar")
+)
+
+```
+- In the module `pie_extended.models.foo.imports`, we should find the following content:
+    1. `get_iterator_and_processor`: a function that returns a `DataIterator` and a `Processor` 
+    2. (optionally) `addons`: a function that installs add-ons
+    3. (optionally) `Disambiguator`: a disambiguator instance (or an object creator that returns one)
+
+Check for a simple example in `pie_extended.models.fro.imports` and a more complex one 
+in `pie_extended.models.lasla.imports`
+
+
+## Install development version (⚠ for development only)
+
+Clone the repository, create an environment, and then
+
+```bash
+python setup.py develop
+```
+
+## Warning
+
+This is an extremely early build, subject to change here and there. But it is functional !
+
+
```

### Comparing `pie_extended-0.0.9/setup.py` & `pie_extended-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from setuptools import find_packages, setup, Command
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Package meta-data.
 NAME = 'pie_extended'
 DESCRIPTION = "Extension for nlp-pie package"
-URL = 'https://github.com/ponteineptique/nlp-pie-taggers'
+URL = 'https://github.com/hipster-philology/nlp-pie-taggers'
 AUTHOR = 'Thibault Clérice'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = "0.0.9"
+VERSION = "0.1.0"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
@@ -101,15 +101,15 @@
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(exclude=('tests', 'env', 'venv',)),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
     entry_points={
-        'console_scripts': ['pie-extended=pie_extended.cli:pie_ext'],
+        'console_scripts': ['pie-extended=pie_extended.cli.main:pie_ext'],
     },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='MIT',
     classifiers=[
         # Trove classifiers
@@ -121,9 +121,9 @@
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Text Processing :: Linguistic'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
-    },
+    }
 )
```


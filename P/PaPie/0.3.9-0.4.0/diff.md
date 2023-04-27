# Comparing `tmp/PaPie-0.3.9.tar.gz` & `tmp/PaPie-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PaPie-0.3.9.tar", last modified: Thu May 20 06:19:58 2021, max compression
+gzip compressed data, was "PaPie-0.4.0.tar", last modified: Thu Apr 27 09:43:49 2023, max compression
```

## Comparing `PaPie-0.3.9.tar` & `PaPie-0.4.0.tar`

### file list

```diff
@@ -1,70 +1,68 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-20 06:19:58.093705 PaPie-0.3.9/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1075 2021-05-19 13:35:00.000000 PaPie-0.3.9/LICENSE
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       68 2021-05-19 13:35:00.000000 PaPie-0.3.9/MANIFEST.in
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    17941 2021-05-20 06:19:58.093705 PaPie-0.3.9/PKG-INFO
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-20 06:19:58.089705 PaPie-0.3.9/PaPie.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    17941 2021-05-20 06:19:57.000000 PaPie-0.3.9/PaPie.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1304 2021-05-20 06:19:58.000000 PaPie-0.3.9/PaPie.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2021-05-20 06:19:57.000000 PaPie-0.3.9/PaPie.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       51 2021-05-20 06:19:57.000000 PaPie-0.3.9/PaPie.egg-info/entry_points.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      210 2021-05-20 06:19:57.000000 PaPie-0.3.9/PaPie.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        9 2021-05-20 06:19:57.000000 PaPie-0.3.9/PaPie.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    14892 2021-05-19 13:35:00.000000 PaPie-0.3.9/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-20 06:19:58.093705 PaPie-0.3.9/pie/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      677 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       18 2021-05-20 06:19:57.000000 PaPie-0.3.9/pie/commit_build.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       92 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/constants.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-20 06:19:58.093705 PaPie-0.3.9/pie/data/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      181 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3316 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/base_reader.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4257 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/conll_reader.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    22359 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/dataset.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-20 06:19:58.093705 PaPie-0.3.9/pie/data/preprocessors/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       86 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/preprocessors/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      245 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/preprocessors/edit_tree_tuples.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4940 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/preprocessors/edit_trees.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4272 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/preprocessors/greedy_scripts.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3214 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/reader.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5414 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/tabreader.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2561 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/data/tei_reader.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     7711 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/default_settings.json
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2445 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/initialization.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-20 06:19:58.093705 PaPie-0.3.9/pie/models/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      378 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     6363 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/attention.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     7189 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/base_model.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4018 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/beam_search.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    20123 2021-05-20 06:19:06.000000 PaPie-0.3.9/pie/models/decoder.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     8320 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/embedding.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2356 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/encoder.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      970 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/highway.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1078 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/loaders.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5655 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/lstm.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    14659 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/model.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    13776 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/models/scorer.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4661 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/optimize.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    15014 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/pretrain_encoder.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-20 06:19:58.093705 PaPie-0.3.9/pie/scripts/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/scripts/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3726 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/scripts/evaluate.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4969 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/scripts/group.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      348 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/scripts/inspect_model.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1683 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/scripts/tag.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1782 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/scripts/tag_pipe.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     7233 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/scripts/train.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4318 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/settings.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5987 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/tagger.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     9686 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/torch_utils.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    12559 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/trainer.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     7136 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/utils.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-20 06:19:58.093705 PaPie-0.3.9/pie/webapp/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4644 2021-05-19 13:35:00.000000 PaPie-0.3.9/pie/webapp/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      210 2021-05-19 13:35:00.000000 PaPie-0.3.9/requirements.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2021-05-20 06:19:58.093705 PaPie-0.3.9/setup.cfg
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4634 2021-05-20 06:19:21.000000 PaPie-0.3.9/setup.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-20 06:19:58.093705 PaPie-0.3.9/test/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-19 13:35:00.000000 PaPie-0.3.9/test/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-20 06:19:58.093705 PaPie-0.3.9/test/data/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-19 13:35:00.000000 PaPie-0.3.9/test/data/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4876 2021-05-19 13:35:00.000000 PaPie-0.3.9/test/data/test_data.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5311 2021-05-19 13:35:00.000000 PaPie-0.3.9/test/data/test_tabreader.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:43:49.520457 PaPie-0.4.0/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1075 2021-05-20 08:00:23.000000 PaPie-0.4.0/LICENSE
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       68 2021-05-20 08:00:23.000000 PaPie-0.4.0/MANIFEST.in
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    15798 2023-04-27 09:43:49.520457 PaPie-0.4.0/PKG-INFO
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:43:49.508456 PaPie-0.4.0/PaPie.egg-info/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    15798 2023-04-27 09:43:49.000000 PaPie-0.4.0/PaPie.egg-info/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1259 2023-04-27 09:43:49.000000 PaPie-0.4.0/PaPie.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-04-27 09:43:49.000000 PaPie-0.4.0/PaPie.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       51 2023-04-27 09:43:49.000000 PaPie-0.4.0/PaPie.egg-info/entry_points.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      180 2023-04-27 09:43:49.000000 PaPie-0.4.0/PaPie.egg-info/requires.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        9 2023-04-27 09:43:49.000000 PaPie-0.4.0/PaPie.egg-info/top_level.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    15050 2021-05-20 08:00:23.000000 PaPie-0.4.0/README.md
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:43:49.512456 PaPie-0.4.0/pie/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       45 2023-04-27 09:43:29.000000 PaPie-0.4.0/pie/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       18 2023-04-27 09:43:49.000000 PaPie-0.4.0/pie/commit_build.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       92 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/constants.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:43:49.512456 PaPie-0.4.0/pie/data/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      181 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/data/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3316 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/data/base_reader.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4257 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/data/conll_reader.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    26303 2023-02-04 16:32:10.000000 PaPie-0.4.0/pie/data/dataset.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:43:49.516456 PaPie-0.4.0/pie/data/preprocessors/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       86 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/data/preprocessors/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      245 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/data/preprocessors/edit_tree_tuples.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4940 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/data/preprocessors/edit_trees.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4272 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/data/preprocessors/greedy_scripts.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3114 2023-04-27 09:43:29.000000 PaPie-0.4.0/pie/data/reader.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5414 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/data/tabreader.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     8278 2021-06-08 10:30:41.000000 PaPie-0.4.0/pie/default_settings.json
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2445 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/initialization.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:43:49.520457 PaPie-0.4.0/pie/models/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      378 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/models/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6377 2023-04-27 09:43:29.000000 PaPie-0.4.0/pie/models/attention.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     7189 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/models/base_model.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4018 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/models/beam_search.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    20129 2023-04-27 09:43:29.000000 PaPie-0.4.0/pie/models/decoder.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     8320 2021-06-08 10:30:37.000000 PaPie-0.4.0/pie/models/embedding.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2356 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/models/encoder.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      970 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/models/highway.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5655 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/models/lstm.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    14659 2023-02-04 16:32:10.000000 PaPie-0.4.0/pie/models/model.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    15725 2023-04-27 09:43:29.000000 PaPie-0.4.0/pie/models/scorer.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4661 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/optimize.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    15014 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/pretrain_encoder.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:43:49.520457 PaPie-0.4.0/pie/scripts/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/scripts/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4738 2021-05-20 09:05:41.000000 PaPie-0.4.0/pie/scripts/evaluate.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5604 2021-05-20 09:05:41.000000 PaPie-0.4.0/pie/scripts/group.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      348 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/scripts/inspect_model.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1683 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/scripts/tag.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1782 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/scripts/tag_pipe.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6978 2023-04-27 09:43:29.000000 PaPie-0.4.0/pie/scripts/train.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4554 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/settings.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5987 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/tagger.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     9686 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/torch_utils.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    14611 2023-04-27 09:43:29.000000 PaPie-0.4.0/pie/trainer.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     7136 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/utils.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:43:49.520457 PaPie-0.4.0/pie/webapp/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4644 2021-05-20 08:00:23.000000 PaPie-0.4.0/pie/webapp/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      179 2023-04-27 09:43:29.000000 PaPie-0.4.0/requirements.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-04-27 09:43:49.520457 PaPie-0.4.0/setup.cfg
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4634 2023-04-27 09:43:29.000000 PaPie-0.4.0/setup.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:43:49.520457 PaPie-0.4.0/test/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-20 08:00:23.000000 PaPie-0.4.0/test/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 09:43:49.520457 PaPie-0.4.0/test/data/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-20 08:00:23.000000 PaPie-0.4.0/test/data/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4876 2021-05-20 08:00:23.000000 PaPie-0.4.0/test/data/test_data.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5311 2021-05-20 08:00:23.000000 PaPie-0.4.0/test/data/test_tabreader.py
```

### Comparing `PaPie-0.3.9/LICENSE` & `PaPie-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/PKG-INFO` & `PaPie-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,307 +1,312 @@
 Metadata-Version: 2.1
 Name: PaPie
-Version: 0.3.9
+Version: 0.4.0
 Summary: A Framework for Joint Learning of Sequence Labeling Tasks, forked from Pie
 Home-page: https://github.com/lascivaroma/PaPie
 Author: Enrique Manjavacas; Mike Kestemont; Thibault Clerice
 License: MIT
-Description: 
-        
-        # PIE: A Framework for Joint Learning of Sequence Labeling Tasks
-        
-        [![DOI](https://zenodo.org/badge/131014015.svg)](https://zenodo.org/badge/latestdoi/131014015)
-        
-        ![Improving Lemmatization of Non-Standard Languages with Joint Learning (NAACL19 Paper)](https://www.aclweb.org/anthology/N19-1153/)
-        
-        PIE was primarily conceived to make experimentation on sequence labeling of variation-rich languages easy and user-friendly. PIE has been tested mostly for Lemmatization but other SoTA accuracies from other tasks like POS have been reproduced (cf. Plank et al ). PIE is *highly* configurable both in terms of input preprocessing and model definition, in principle not requiring users to write any code (instead experiments are defined with json files). It is highly modular and therefore easy to extend. It includes transductive lemmatization as an additional sequence labeling task and, finally, it is reasonably fast and memory efficient.
-        
-        Documentation is work in progress and it will improve over the following months. A good place to learn about its functionality is to check `pie/default_settings.json` which explains all input parameters and shows a full example of a config file (minus input data).
-        
-        If you find `pie` useful, please use the following reference:
-        
-        ```
-        @inproceedings{manjavacas-etal-2019-improving,
-            title = "Improving Lemmatization of Non-Standard Languages with Joint Learning",
-            author = "Manjavacas, Enrique  and
-              K{\'a}d{\'a}r, {\'A}kos  and
-              Kestemont, Mike",
-            booktitle = "Proceedings of the 2019 Conference of the North {A}merican Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers)",
-            month = jun,
-            year = "2019",
-            address = "Minneapolis, Minnesota",
-            publisher = "Association for Computational Linguistics",
-            url = "https://www.aclweb.org/anthology/N19-1153",
-            doi = "10.18653/v1/N19-1153",
-            pages = "1493--1503",
-            abstract = "Lemmatization of standard languages is concerned with (i) abstracting over morphological differences and (ii) resolving token-lemma ambiguities of inflected words in order to map them to a dictionary headword. In the present paper we aim to improve lemmatization performance on a set of non-standard historical languages in which the difficulty is increased by an additional aspect (iii): spelling variation due to lacking orthographic standards. We approach lemmatization as a string-transduction task with an Encoder-Decoder architecture which we enrich with sentence information using a hierarchical sentence encoder. We show significant improvements over the state-of-the-art by fine-tuning the sentence encodings to jointly optimize a bidirectional language model loss. Crucially, our architecture does not require POS or morphological annotations, which are not always available for historical corpora. Additionally, we also test the proposed model on a set of typologically diverse standard languages showing results on par or better than a model without fine-tuned sentence representations and previous state-of-the-art systems. Finally, to encourage future work on processing of non-standard varieties, we release the dataset of non-standard languages underlying the present study, which is based on openly accessible sources.",
-        }
-        ```
-        
-        ## 1. Installation
-        
-        PIE is available from pypi, which means that all you should need to do is:
-        
-        ```bash
-        pip install nlp-pie
-        ```
-        
-        ### For development
-        
-        If you are planning to develop on top of PIE, the easiest way is to get setup is to download the repository and install the dependencies (see `requirements.txt`). The only step needed to have `pie` available from any place in the file system is to add the path to `pie` to the `PYTHONPATH` environment variable. There are two ways to accomplish this:
-        
-        - From your bash init file (depending on your distro and configuration this could be `.bashrc`, `.bash_profile`, `.profile`, etc...):
-        
-        ```bash
-        export PYTHONPATH="$PYTHONPATH:/path/to/pie"
-        ```
-        
-        - From your python script, using `sys`:
-        
-        ```python
-        import sys
-        sys.path.append('/path/to/pie')
-        ```
-        
-        ## 2. Training
-        
-        Training models is done with `pie train path/to/config.json` (or script `python pie/scripts/train.py`. All non-nested parameters can be overwritten directly from the command line using environment variables like `PIE_DEVICE=cpu` (for input parameter `device`. Warning: bear in mind that due to the way bash parses environment variables `PIE_...=False` will be parsed into a boolean `True`, which might be counter-intuitive. If you wish to get `False` for a parameter from the command line you can use `PIE_...=""`).
-        
-        ## 3. Evaluation
-        
-        A given model can be evaluated with `pie evaluate` (or `python pie/scripts/evaluate.py`).
-        
-        ## 4. Tagging
-        
-        Given one or several trained models, two scripts are provided in order to tag given input: `pie tag` and `pie tag-pipe` (or `python pie/scripts/tag.py`, `python pie/scripts/tag_pipe.py`), the difference being that the first tags input files and the second can take input from a unix pipe.
-        
-        Common to both scripts is the *model specification* that allows to combine several models, where the output for a particular task is taken from a model that excels at that task.
-        For example, given models `good-pos-tagger.tar` and `good-lemma-tagger.tar`, we can define a tagger that uses `good-pos-tagger.tar` for POS-tagging and `good-lemma-tagger.tar` for lemmatization with the following specification: `<good-lemma-tagger.tar,lemma><good-pos-tagger.tar,pos>`.
-        
-        - If your input is in a file `test.txt` (with a sentence per line) you can use:
-        
-        `pie tag "<good-lemma-tagger.tar,lemma><good-pos-tagger.tar,pos>" test.txt`
-        
-        and the output will be written to `test.pie.txt`
-        
-        - If you want to pass input from the command line, you can use:
-        ```
-        $ echo "el gato duerme encima de la silla" | pie tag-pipe spanish-lemmatizer.rar
-        
-        token	lemma
-        el	el
-        gato	gato
-        duerme	dormir
-        encima	encima
-        de	de
-        la	el
-        silla	silla
-        ```
-        
-        ## 5. Model
-        
-        PIE underlying model comprises a set of hierarchical feature extractors from the character-level up to the sentence-level. For each input token a sentence-level feature vector is extracted and used for the prediction of any number of target tasks (e.g. POS-tagging, lemmatization, ...). A visualization of the underlying model using bidirectional RNNs to extract word-level and sentence-level features is shown below.
-        
-        ![PIE](./img/PIE.svg)
-        
-        Prediction is accomplished with decoder modules. We provide implementations of a `linear` decoder trained to maximize the probability assigned by the model to the corpus data via a softmax function (similar to a MaxEnt classifier). A `crf` decoder, particularly suited for tasks that imply a dependency between neighboring output tags and an `attentional` decoder, suited for tasks that can be solved by generating the token-level output character by characters in a string transduction manner (e.g. lemmatization, normalization).
-        
-        ## 6. Configuration files
-        
-        Training a model only requires a model specification and paths to training and dev datasets. Pie user interface employs a simple json file (in order to allow in-line comments, we make use of the package `JSON_minify`), an example of which can be seen below:
-        
-        ```json
-        {
-          "modelname": "lemmatization-latin",
-          "modelpath": "models",
-        
-          "input_path": "datasets/LLCT1/train.tsv",
-          "dev_path": "datasets/LLCT1/dev.tsv",
-          "sep": "\t",
-         
-          "tasks": [
-            {
-              "name": "lemma",
-              "target": true,
-              "context": "sentence",
-              "level": "char",
-              "decoder": "attentional",
-              "settings": {
-                "bos": true,
-                "eos": true,
-                "lower": true,
-                "target": "lemma"
-              },
-              "layer": -1
-            }
-          ],
-          "batch_size": 25,
-          "epochs": 100,
-          
-          "dropout": 0.25,
-          "optimizer": "Adam",
-          "patience": 3,
-          "lr": 0.001,
-          "lr_factor": 0.75,
-          "lr_patience": 2,
-          
-          "cell": "GRU",
-          "num_layers": 1,
-          "hidden_size": 150,
-          "wemb_dim": 0,
-          "cemb_dim": 300,
-          "cemb_type": "rnn",
-          "cemb_layers": 2
-        }
-        ```
-        
-        The very minimum set of options required to train a model includes `input_path` (path to files with training data), `dev_path` (path to files with development data), and `tasks`, which defines the model to be trained. Other parameters refer to model hyperparameters (`cell`, `num_layers`, `hidden_size`, `wemb_dim`, `cemb_dim`, `cemb_type`, `cemb_layers`), training (`batch_size`, `epochs`) and optimization (`dropout`, `optimizer`, `patience`, `lr`, `lr_factor`, `lr_patience).
-        
-        ### POS tagging using a CRF
-        
-        ```json
-        {
-          "tasks": [
-            {
-              "name": "pos", 
-              "target": true,
-              "decoder": "crf",
-              "layer": -1
-            }
-          ]
-        }
-        
-        ```
-        
-        ### POS tagging using a linear decoder and 2 auxiliary tasks
-        ```json
-        {
-          "tasks": [
-            {
-              "name": "pos",
-              "level": "token",
-              "target": true,
-              "decoder": "crf",
-              "layer": -1,
-              "schedule": {
-                "patience": 3
-              }
-            },
-            {
-              "name": "case",
-              "level": "token",
-              "target": false,
-              "decoder": "linear",
-              "layer": 0,
-              "schedule": {
-                "patience": 2,
-                "factor": 0.5
-              }
-            },
-            {
-              "name": "number",
-              "level": "token",
-              "target": false,
-              "decoder": "linear",
-              "layer": 0,
-              "schedule": {
-                "patience": 2,
-                "factor": 0.5
-              }
-            }
-          ]
-        }
-        ```
-        
-        By setting a schedule we can fine-tune the learning dynamics of auxiliary tasks in a multi-task settings (see below for more information on this). 
-        
-        To avoid verbosity, parameters invariant across auxiliary tasks can be specified only once using `task_defaults`. Similarly, learning schedule parameters invariant across tasks (`factor`, `patience`, `threshold`, `min_weight`) can be factored out of the task schedule definition. In summary, the previous configuration can be rewritten in the following form:
-        
-        ```json
-        {
-          "tasks": [
-            {
-              "name": "pos",
-              "level": "token",
-              "target": true,
-              "decoder": "crf",
-              "layer": -1,
-              "schedule": {
-                "patience": 3
-              }
-            },
-            {
-              "name": "case"
-            },
-            {
-              "name": "number"
-            }
-          ],
-          "task_defaults": {
-            "level": "token",
-            "decoder": "linear",
-            "layer": 0
-          },
-          "patience": 2,
-          "factor": 0.5
-        }
-        
-        ```
-        
-        ### Transduction-based lemmatization
-        
-        PIE has built-in support for lemmatization as a string transduction task using an Encoder-Decoder architecture as shown below (lemmatizing Latin token "esse" to its lemma "edo"):
-        
-        ![Encoder-Decoder for lemmatization](./img/seq2seq.png)
-        
-        PIE implements several state-of-the-art attention mechanisms to faciliate information flow between the encoder and the decoder. Additionally, the decoder can be conditioned on sentence-level features to help with disambiguating.
-        
-        A task configuration for lemmatization with an Encoder-Decoder model and integrated sentence-level features is shown below.
-        
-        ```json
-        {
-          "tasks": [
-            {
-              "name": "lemma",
-              "level": "char",
-              "target": true,
-              "decoder": "attentional",
-              "context": "sentence",
-              "layer": -1,
-              "schedule": {
-                "patience": 3
-              }
-            }
-          ]
-        }
-        ```
-        
-        ## 7. Improving feature extraction with a joint Language Model loss
-        
-        Pie has a built-in option to improve feature extraction by predicting neighboring words from the sentence-level feature vectors. The mechanism has been thoroughly tested for lemmatization in research currently submitted to review and it has been shown to be very effective for languages without a fixed writing standard (e.g. historical languages) and other languages with high token-lemma ambiguity. Besides, there is nothing in theory opposing the idea that it might help with other tasks such as POS-tagging, morphological analyses, etc...  The options affecting the joint LM-loss are: `include_lm` (switch on the option), `lm_shared_softmax` (whether to share parameters between forward and backward LMs, recommended value: `true`), `lm_schedule` (parameters to lower the weight assigned to the LM loss over training, once the LM loss starts overfitting it is a good idea to start reducing the loss and eventually set it to 0 to avoid affecting the learning of the target task).
-        
-        ## 8. Multi-task learning
-        
-        When more than one task is defined, at least and at most one task has to have the key-value pair `"target": true`, denoting that that's the task we ultimately care about. All the other tasks will be treated as auxiliary tasks with the goal of extracting better features for the target task. Note that in any case the model will still be able to predict output for auxiliary tasks, but in the spirit of multi-task learning, you will prefer to train a separate model for each of the tasks you care about, selecting each time the appropriate target task and letting all other tasks help the optimization. In the end, you have as many models as tasks you care about, each of which has been optimized for the respective task.
-        
-        ### More on auxiliary tasks
-        
-        An auxiliary task might help learning better features that the classifier for the target task can exploit to produce better (in terms of classification performance) and more robust output (less susceptible to spurious correlations). However, training dynamics in a multi-task setting are complex (even more so than in a normal setting), since different tasks usually results in different learning curves that have to be monitored. In particular, if an auxiliary task converges before the target task, further training might lead that auxiliary task towards overfitting, thereby undoing the potential work done so far. Moreover, losses from different tasks are usually in different scales and this might have the effect that an auxiliary task with a loss on a higher scale dominates training.
-        
-        In order to avoid it, the strategy chosen for PIE consists on set learning schedules for tasks (similar to early stopping) that decrease the weights given to particular tasks over time based on development performance. 
-        
-        Multi-task learning consists on jointly training a model for different tasks while sharing parts of the general architecture for all tasks. This can be accomplished by either computing the loss for all tasks every batch and aggregating it before the backward pass, or optimizing in each batch for a single task randomly sampled based on a particular distribution. PIE follows the latter setting, which is known to produce better results.
-        
-        Additionally, it is also important, in case of a multi-layer sentence-level feature extractor, to select at what layer a particular task can help the most (this can be controlled with the "layer" option).
-        
-        Finally, multi-task learning is far from being a silver bullet and it is an empirical question whether a multi-task learning setup will yield improvements. It is recommended to first train a single model, and then try different multi-task learning configuration to see if improvements can be achieved.
-        
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
+
+# (Pa)PIE: A Framework for Joint Learning of Sequence Labeling Tasks
+
+[![DOI](https://zenodo.org/badge/131014015.svg)](https://zenodo.org/badge/latestdoi/131014015)
+
+![Improving Lemmatization of Non-Standard Languages with Joint Learning (NAACL19 Paper)](https://www.aclweb.org/anthology/N19-1153/)
+
+**Warning:** This is a fork from [pie](https://github.com/emanjavacas/pie). It provides some sometime *unstable* improvement over the original software.
+
+PIE was primarily conceived to make experimentation on sequence labeling of variation-rich languages easy and user-friendly. PIE has been tested mostly for Lemmatization but other SoTA accuracies from other tasks like POS have been reproduced (cf. Plank et al ). PIE is *highly* configurable both in terms of input preprocessing and model definition, in principle not requiring users to write any code (instead experiments are defined with json files). It is highly modular and therefore easy to extend. It includes transductive lemmatization as an additional sequence labeling task and, finally, it is reasonably fast and memory efficient.
+
+Documentation is work in progress and it will improve over the following months. A good place to learn about its functionality is to check `pie/default_settings.json` which explains all input parameters and shows a full example of a config file (minus input data).
+
+If you find `pie` useful, please use the following reference:
+
+```
+@inproceedings{manjavacas-etal-2019-improving,
+    title = "Improving Lemmatization of Non-Standard Languages with Joint Learning",
+    author = "Manjavacas, Enrique  and
+      K{\'a}d{\'a}r, {\'A}kos  and
+      Kestemont, Mike",
+    booktitle = "Proceedings of the 2019 Conference of the North {A}merican Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers)",
+    month = jun,
+    year = "2019",
+    address = "Minneapolis, Minnesota",
+    publisher = "Association for Computational Linguistics",
+    url = "https://www.aclweb.org/anthology/N19-1153",
+    doi = "10.18653/v1/N19-1153",
+    pages = "1493--1503",
+    abstract = "Lemmatization of standard languages is concerned with (i) abstracting over morphological differences and (ii) resolving token-lemma ambiguities of inflected words in order to map them to a dictionary headword. In the present paper we aim to improve lemmatization performance on a set of non-standard historical languages in which the difficulty is increased by an additional aspect (iii): spelling variation due to lacking orthographic standards. We approach lemmatization as a string-transduction task with an Encoder-Decoder architecture which we enrich with sentence information using a hierarchical sentence encoder. We show significant improvements over the state-of-the-art by fine-tuning the sentence encodings to jointly optimize a bidirectional language model loss. Crucially, our architecture does not require POS or morphological annotations, which are not always available for historical corpora. Additionally, we also test the proposed model on a set of typologically diverse standard languages showing results on par or better than a model without fine-tuned sentence representations and previous state-of-the-art systems. Finally, to encourage future work on processing of non-standard varieties, we release the dataset of non-standard languages underlying the present study, which is based on openly accessible sources.",
+}
+```
+
+## 1. Installation
+
+PIE is available from pypi, which means that all you should need to do is:
+
+```bash
+pip install nlp-pie
+```
+
+### For development
+
+If you are planning to develop on top of PIE, the easiest way is to get setup is to download the repository and install the dependencies (see `requirements.txt`). The only step needed to have `pie` available from any place in the file system is to add the path to `pie` to the `PYTHONPATH` environment variable. There are two ways to accomplish this:
+
+- From your bash init file (depending on your distro and configuration this could be `.bashrc`, `.bash_profile`, `.profile`, etc...):
+
+```bash
+export PYTHONPATH="$PYTHONPATH:/path/to/pie"
+```
+
+- From your python script, using `sys`:
+
+```python
+import sys
+sys.path.append('/path/to/pie')
+```
+
+## 2. Training
+
+Training models is done with `pie train path/to/config.json` (or script `python pie/scripts/train.py`. All non-nested parameters can be overwritten directly from the command line using environment variables like `PIE_DEVICE=cpu` (for input parameter `device`. Warning: bear in mind that due to the way bash parses environment variables `PIE_...=False` will be parsed into a boolean `True`, which might be counter-intuitive. If you wish to get `False` for a parameter from the command line you can use `PIE_...=""`).
+
+## 3. Evaluation
+
+A given model can be evaluated with `pie evaluate` (or `python pie/scripts/evaluate.py`).
+
+## 4. Tagging
+
+Given one or several trained models, two scripts are provided in order to tag given input: `pie tag` and `pie tag-pipe` (or `python pie/scripts/tag.py`, `python pie/scripts/tag_pipe.py`), the difference being that the first tags input files and the second can take input from a unix pipe.
+
+Common to both scripts is the *model specification* that allows to combine several models, where the output for a particular task is taken from a model that excels at that task.
+For example, given models `good-pos-tagger.tar` and `good-lemma-tagger.tar`, we can define a tagger that uses `good-pos-tagger.tar` for POS-tagging and `good-lemma-tagger.tar` for lemmatization with the following specification: `<good-lemma-tagger.tar,lemma><good-pos-tagger.tar,pos>`.
+
+- If your input is in a file `test.txt` (with a sentence per line) you can use:
+
+`pie tag "<good-lemma-tagger.tar,lemma><good-pos-tagger.tar,pos>" test.txt`
+
+and the output will be written to `test.pie.txt`
+
+- If you want to pass input from the command line, you can use:
+```
+$ echo "el gato duerme encima de la silla" | pie tag-pipe spanish-lemmatizer.rar
+
+token	lemma
+el	el
+gato	gato
+duerme	dormir
+encima	encima
+de	de
+la	el
+silla	silla
+```
+
+## 5. Model
+
+PIE underlying model comprises a set of hierarchical feature extractors from the character-level up to the sentence-level. For each input token a sentence-level feature vector is extracted and used for the prediction of any number of target tasks (e.g. POS-tagging, lemmatization, ...). A visualization of the underlying model using bidirectional RNNs to extract word-level and sentence-level features is shown below.
+
+![PIE](./img/PIE.svg)
+
+Prediction is accomplished with decoder modules. We provide implementations of a `linear` decoder trained to maximize the probability assigned by the model to the corpus data via a softmax function (similar to a MaxEnt classifier). A `crf` decoder, particularly suited for tasks that imply a dependency between neighboring output tags and an `attentional` decoder, suited for tasks that can be solved by generating the token-level output character by characters in a string transduction manner (e.g. lemmatization, normalization).
+
+## 6. Configuration files
+
+Training a model only requires a model specification and paths to training and dev datasets. Pie user interface employs a simple json file (in order to allow in-line comments, we make use of the package `JSON_minify`), an example of which can be seen below:
+
+```json
+{
+  "modelname": "lemmatization-latin",
+  "modelpath": "models",
+
+  "input_path": "datasets/LLCT1/train.tsv",
+  "dev_path": "datasets/LLCT1/dev.tsv",
+  "sep": "\t",
+ 
+  "tasks": [
+    {
+      "name": "lemma",
+      "target": true,
+      "context": "sentence",
+      "level": "char",
+      "decoder": "attentional",
+      "settings": {
+        "bos": true,
+        "eos": true,
+        "lower": true,
+        "target": "lemma"
+      },
+      "layer": -1
+    }
+  ],
+  "batch_size": 25,
+  "epochs": 100,
+  
+  "dropout": 0.25,
+  "optimizer": "Adam",
+  "patience": 3,
+  "lr": 0.001,
+  "lr_factor": 0.75,
+  "lr_patience": 2,
+  
+  "cell": "GRU",
+  "num_layers": 1,
+  "hidden_size": 150,
+  "wemb_dim": 0,
+  "cemb_dim": 300,
+  "cemb_type": "rnn",
+  "cemb_layers": 2
+}
+```
+
+The very minimum set of options required to train a model includes `input_path` (path to files with training data), `dev_path` (path to files with development data), and `tasks`, which defines the model to be trained. Other parameters refer to model hyperparameters (`cell`, `num_layers`, `hidden_size`, `wemb_dim`, `cemb_dim`, `cemb_type`, `cemb_layers`), training (`batch_size`, `epochs`) and optimization (`dropout`, `optimizer`, `patience`, `lr`, `lr_factor`, `lr_patience).
+
+### POS tagging using a CRF
+
+```json
+{
+  "tasks": [
+    {
+      "name": "pos", 
+      "target": true,
+      "decoder": "crf",
+      "layer": -1
+    }
+  ]
+}
+
+```
+
+### POS tagging using a linear decoder and 2 auxiliary tasks
+```json
+{
+  "tasks": [
+    {
+      "name": "pos",
+      "level": "token",
+      "target": true,
+      "decoder": "crf",
+      "layer": -1,
+      "schedule": {
+        "patience": 3
+      }
+    },
+    {
+      "name": "case",
+      "level": "token",
+      "target": false,
+      "decoder": "linear",
+      "layer": 0,
+      "schedule": {
+        "patience": 2,
+        "factor": 0.5
+      }
+    },
+    {
+      "name": "number",
+      "level": "token",
+      "target": false,
+      "decoder": "linear",
+      "layer": 0,
+      "schedule": {
+        "patience": 2,
+        "factor": 0.5
+      }
+    }
+  ]
+}
+```
+
+By setting a schedule we can fine-tune the learning dynamics of auxiliary tasks in a multi-task settings (see below for more information on this). 
+
+To avoid verbosity, parameters invariant across auxiliary tasks can be specified only once using `task_defaults`. Similarly, learning schedule parameters invariant across tasks (`factor`, `patience`, `threshold`, `min_weight`) can be factored out of the task schedule definition. In summary, the previous configuration can be rewritten in the following form:
+
+```json
+{
+  "tasks": [
+    {
+      "name": "pos",
+      "level": "token",
+      "target": true,
+      "decoder": "crf",
+      "layer": -1,
+      "schedule": {
+        "patience": 3
+      }
+    },
+    {
+      "name": "case"
+    },
+    {
+      "name": "number"
+    }
+  ],
+  "task_defaults": {
+    "level": "token",
+    "decoder": "linear",
+    "layer": 0
+  },
+  "patience": 2,
+  "factor": 0.5
+}
+
+```
+
+### Transduction-based lemmatization
+
+PIE has built-in support for lemmatization as a string transduction task using an Encoder-Decoder architecture as shown below (lemmatizing Latin token "esse" to its lemma "edo"):
+
+![Encoder-Decoder for lemmatization](./img/seq2seq.png)
+
+PIE implements several state-of-the-art attention mechanisms to faciliate information flow between the encoder and the decoder. Additionally, the decoder can be conditioned on sentence-level features to help with disambiguating.
+
+A task configuration for lemmatization with an Encoder-Decoder model and integrated sentence-level features is shown below.
+
+```json
+{
+  "tasks": [
+    {
+      "name": "lemma",
+      "level": "char",
+      "target": true,
+      "decoder": "attentional",
+      "context": "sentence",
+      "layer": -1,
+      "schedule": {
+        "patience": 3
+      }
+    }
+  ]
+}
+```
+
+## 7. Improving feature extraction with a joint Language Model loss
+
+Pie has a built-in option to improve feature extraction by predicting neighboring words from the sentence-level feature vectors. The mechanism has been thoroughly tested for lemmatization in research currently submitted to review and it has been shown to be very effective for languages without a fixed writing standard (e.g. historical languages) and other languages with high token-lemma ambiguity. Besides, there is nothing in theory opposing the idea that it might help with other tasks such as POS-tagging, morphological analyses, etc...  The options affecting the joint LM-loss are: `include_lm` (switch on the option), `lm_shared_softmax` (whether to share parameters between forward and backward LMs, recommended value: `true`), `lm_schedule` (parameters to lower the weight assigned to the LM loss over training, once the LM loss starts overfitting it is a good idea to start reducing the loss and eventually set it to 0 to avoid affecting the learning of the target task).
+
+## 8. Multi-task learning
+
+When more than one task is defined, at least and at most one task has to have the key-value pair `"target": true`, denoting that that's the task we ultimately care about. All the other tasks will be treated as auxiliary tasks with the goal of extracting better features for the target task. Note that in any case the model will still be able to predict output for auxiliary tasks, but in the spirit of multi-task learning, you will prefer to train a separate model for each of the tasks you care about, selecting each time the appropriate target task and letting all other tasks help the optimization. In the end, you have as many models as tasks you care about, each of which has been optimized for the respective task.
+
+### More on auxiliary tasks
+
+An auxiliary task might help learning better features that the classifier for the target task can exploit to produce better (in terms of classification performance) and more robust output (less susceptible to spurious correlations). However, training dynamics in a multi-task setting are complex (even more so than in a normal setting), since different tasks usually results in different learning curves that have to be monitored. In particular, if an auxiliary task converges before the target task, further training might lead that auxiliary task towards overfitting, thereby undoing the potential work done so far. Moreover, losses from different tasks are usually in different scales and this might have the effect that an auxiliary task with a loss on a higher scale dominates training.
+
+In order to avoid it, the strategy chosen for PIE consists on set learning schedules for tasks (similar to early stopping) that decrease the weights given to particular tasks over time based on development performance. 
+
+Multi-task learning consists on jointly training a model for different tasks while sharing parts of the general architecture for all tasks. This can be accomplished by either computing the loss for all tasks every batch and aggregating it before the backward pass, or optimizing in each batch for a single task randomly sampled based on a particular distribution. PIE follows the latter setting, which is known to produce better results.
+
+Additionally, it is also important, in case of a multi-layer sentence-level feature extractor, to select at what layer a particular task can help the most (this can be controlled with the "layer" option).
+
+Finally, multi-task learning is far from being a silver bullet and it is an empirical question whether a multi-task learning setup will yield improvements. It is recommended to first train a single model, and then try different multi-task learning configuration to see if improvements can be achieved.
+
+
```

### Comparing `PaPie-0.3.9/PaPie.egg-info/PKG-INFO` & `PaPie-0.4.0/PaPie.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,307 +1,312 @@
 Metadata-Version: 2.1
 Name: PaPie
-Version: 0.3.9
+Version: 0.4.0
 Summary: A Framework for Joint Learning of Sequence Labeling Tasks, forked from Pie
 Home-page: https://github.com/lascivaroma/PaPie
 Author: Enrique Manjavacas; Mike Kestemont; Thibault Clerice
 License: MIT
-Description: 
-        
-        # PIE: A Framework for Joint Learning of Sequence Labeling Tasks
-        
-        [![DOI](https://zenodo.org/badge/131014015.svg)](https://zenodo.org/badge/latestdoi/131014015)
-        
-        ![Improving Lemmatization of Non-Standard Languages with Joint Learning (NAACL19 Paper)](https://www.aclweb.org/anthology/N19-1153/)
-        
-        PIE was primarily conceived to make experimentation on sequence labeling of variation-rich languages easy and user-friendly. PIE has been tested mostly for Lemmatization but other SoTA accuracies from other tasks like POS have been reproduced (cf. Plank et al ). PIE is *highly* configurable both in terms of input preprocessing and model definition, in principle not requiring users to write any code (instead experiments are defined with json files). It is highly modular and therefore easy to extend. It includes transductive lemmatization as an additional sequence labeling task and, finally, it is reasonably fast and memory efficient.
-        
-        Documentation is work in progress and it will improve over the following months. A good place to learn about its functionality is to check `pie/default_settings.json` which explains all input parameters and shows a full example of a config file (minus input data).
-        
-        If you find `pie` useful, please use the following reference:
-        
-        ```
-        @inproceedings{manjavacas-etal-2019-improving,
-            title = "Improving Lemmatization of Non-Standard Languages with Joint Learning",
-            author = "Manjavacas, Enrique  and
-              K{\'a}d{\'a}r, {\'A}kos  and
-              Kestemont, Mike",
-            booktitle = "Proceedings of the 2019 Conference of the North {A}merican Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers)",
-            month = jun,
-            year = "2019",
-            address = "Minneapolis, Minnesota",
-            publisher = "Association for Computational Linguistics",
-            url = "https://www.aclweb.org/anthology/N19-1153",
-            doi = "10.18653/v1/N19-1153",
-            pages = "1493--1503",
-            abstract = "Lemmatization of standard languages is concerned with (i) abstracting over morphological differences and (ii) resolving token-lemma ambiguities of inflected words in order to map them to a dictionary headword. In the present paper we aim to improve lemmatization performance on a set of non-standard historical languages in which the difficulty is increased by an additional aspect (iii): spelling variation due to lacking orthographic standards. We approach lemmatization as a string-transduction task with an Encoder-Decoder architecture which we enrich with sentence information using a hierarchical sentence encoder. We show significant improvements over the state-of-the-art by fine-tuning the sentence encodings to jointly optimize a bidirectional language model loss. Crucially, our architecture does not require POS or morphological annotations, which are not always available for historical corpora. Additionally, we also test the proposed model on a set of typologically diverse standard languages showing results on par or better than a model without fine-tuned sentence representations and previous state-of-the-art systems. Finally, to encourage future work on processing of non-standard varieties, we release the dataset of non-standard languages underlying the present study, which is based on openly accessible sources.",
-        }
-        ```
-        
-        ## 1. Installation
-        
-        PIE is available from pypi, which means that all you should need to do is:
-        
-        ```bash
-        pip install nlp-pie
-        ```
-        
-        ### For development
-        
-        If you are planning to develop on top of PIE, the easiest way is to get setup is to download the repository and install the dependencies (see `requirements.txt`). The only step needed to have `pie` available from any place in the file system is to add the path to `pie` to the `PYTHONPATH` environment variable. There are two ways to accomplish this:
-        
-        - From your bash init file (depending on your distro and configuration this could be `.bashrc`, `.bash_profile`, `.profile`, etc...):
-        
-        ```bash
-        export PYTHONPATH="$PYTHONPATH:/path/to/pie"
-        ```
-        
-        - From your python script, using `sys`:
-        
-        ```python
-        import sys
-        sys.path.append('/path/to/pie')
-        ```
-        
-        ## 2. Training
-        
-        Training models is done with `pie train path/to/config.json` (or script `python pie/scripts/train.py`. All non-nested parameters can be overwritten directly from the command line using environment variables like `PIE_DEVICE=cpu` (for input parameter `device`. Warning: bear in mind that due to the way bash parses environment variables `PIE_...=False` will be parsed into a boolean `True`, which might be counter-intuitive. If you wish to get `False` for a parameter from the command line you can use `PIE_...=""`).
-        
-        ## 3. Evaluation
-        
-        A given model can be evaluated with `pie evaluate` (or `python pie/scripts/evaluate.py`).
-        
-        ## 4. Tagging
-        
-        Given one or several trained models, two scripts are provided in order to tag given input: `pie tag` and `pie tag-pipe` (or `python pie/scripts/tag.py`, `python pie/scripts/tag_pipe.py`), the difference being that the first tags input files and the second can take input from a unix pipe.
-        
-        Common to both scripts is the *model specification* that allows to combine several models, where the output for a particular task is taken from a model that excels at that task.
-        For example, given models `good-pos-tagger.tar` and `good-lemma-tagger.tar`, we can define a tagger that uses `good-pos-tagger.tar` for POS-tagging and `good-lemma-tagger.tar` for lemmatization with the following specification: `<good-lemma-tagger.tar,lemma><good-pos-tagger.tar,pos>`.
-        
-        - If your input is in a file `test.txt` (with a sentence per line) you can use:
-        
-        `pie tag "<good-lemma-tagger.tar,lemma><good-pos-tagger.tar,pos>" test.txt`
-        
-        and the output will be written to `test.pie.txt`
-        
-        - If you want to pass input from the command line, you can use:
-        ```
-        $ echo "el gato duerme encima de la silla" | pie tag-pipe spanish-lemmatizer.rar
-        
-        token	lemma
-        el	el
-        gato	gato
-        duerme	dormir
-        encima	encima
-        de	de
-        la	el
-        silla	silla
-        ```
-        
-        ## 5. Model
-        
-        PIE underlying model comprises a set of hierarchical feature extractors from the character-level up to the sentence-level. For each input token a sentence-level feature vector is extracted and used for the prediction of any number of target tasks (e.g. POS-tagging, lemmatization, ...). A visualization of the underlying model using bidirectional RNNs to extract word-level and sentence-level features is shown below.
-        
-        ![PIE](./img/PIE.svg)
-        
-        Prediction is accomplished with decoder modules. We provide implementations of a `linear` decoder trained to maximize the probability assigned by the model to the corpus data via a softmax function (similar to a MaxEnt classifier). A `crf` decoder, particularly suited for tasks that imply a dependency between neighboring output tags and an `attentional` decoder, suited for tasks that can be solved by generating the token-level output character by characters in a string transduction manner (e.g. lemmatization, normalization).
-        
-        ## 6. Configuration files
-        
-        Training a model only requires a model specification and paths to training and dev datasets. Pie user interface employs a simple json file (in order to allow in-line comments, we make use of the package `JSON_minify`), an example of which can be seen below:
-        
-        ```json
-        {
-          "modelname": "lemmatization-latin",
-          "modelpath": "models",
-        
-          "input_path": "datasets/LLCT1/train.tsv",
-          "dev_path": "datasets/LLCT1/dev.tsv",
-          "sep": "\t",
-         
-          "tasks": [
-            {
-              "name": "lemma",
-              "target": true,
-              "context": "sentence",
-              "level": "char",
-              "decoder": "attentional",
-              "settings": {
-                "bos": true,
-                "eos": true,
-                "lower": true,
-                "target": "lemma"
-              },
-              "layer": -1
-            }
-          ],
-          "batch_size": 25,
-          "epochs": 100,
-          
-          "dropout": 0.25,
-          "optimizer": "Adam",
-          "patience": 3,
-          "lr": 0.001,
-          "lr_factor": 0.75,
-          "lr_patience": 2,
-          
-          "cell": "GRU",
-          "num_layers": 1,
-          "hidden_size": 150,
-          "wemb_dim": 0,
-          "cemb_dim": 300,
-          "cemb_type": "rnn",
-          "cemb_layers": 2
-        }
-        ```
-        
-        The very minimum set of options required to train a model includes `input_path` (path to files with training data), `dev_path` (path to files with development data), and `tasks`, which defines the model to be trained. Other parameters refer to model hyperparameters (`cell`, `num_layers`, `hidden_size`, `wemb_dim`, `cemb_dim`, `cemb_type`, `cemb_layers`), training (`batch_size`, `epochs`) and optimization (`dropout`, `optimizer`, `patience`, `lr`, `lr_factor`, `lr_patience).
-        
-        ### POS tagging using a CRF
-        
-        ```json
-        {
-          "tasks": [
-            {
-              "name": "pos", 
-              "target": true,
-              "decoder": "crf",
-              "layer": -1
-            }
-          ]
-        }
-        
-        ```
-        
-        ### POS tagging using a linear decoder and 2 auxiliary tasks
-        ```json
-        {
-          "tasks": [
-            {
-              "name": "pos",
-              "level": "token",
-              "target": true,
-              "decoder": "crf",
-              "layer": -1,
-              "schedule": {
-                "patience": 3
-              }
-            },
-            {
-              "name": "case",
-              "level": "token",
-              "target": false,
-              "decoder": "linear",
-              "layer": 0,
-              "schedule": {
-                "patience": 2,
-                "factor": 0.5
-              }
-            },
-            {
-              "name": "number",
-              "level": "token",
-              "target": false,
-              "decoder": "linear",
-              "layer": 0,
-              "schedule": {
-                "patience": 2,
-                "factor": 0.5
-              }
-            }
-          ]
-        }
-        ```
-        
-        By setting a schedule we can fine-tune the learning dynamics of auxiliary tasks in a multi-task settings (see below for more information on this). 
-        
-        To avoid verbosity, parameters invariant across auxiliary tasks can be specified only once using `task_defaults`. Similarly, learning schedule parameters invariant across tasks (`factor`, `patience`, `threshold`, `min_weight`) can be factored out of the task schedule definition. In summary, the previous configuration can be rewritten in the following form:
-        
-        ```json
-        {
-          "tasks": [
-            {
-              "name": "pos",
-              "level": "token",
-              "target": true,
-              "decoder": "crf",
-              "layer": -1,
-              "schedule": {
-                "patience": 3
-              }
-            },
-            {
-              "name": "case"
-            },
-            {
-              "name": "number"
-            }
-          ],
-          "task_defaults": {
-            "level": "token",
-            "decoder": "linear",
-            "layer": 0
-          },
-          "patience": 2,
-          "factor": 0.5
-        }
-        
-        ```
-        
-        ### Transduction-based lemmatization
-        
-        PIE has built-in support for lemmatization as a string transduction task using an Encoder-Decoder architecture as shown below (lemmatizing Latin token "esse" to its lemma "edo"):
-        
-        ![Encoder-Decoder for lemmatization](./img/seq2seq.png)
-        
-        PIE implements several state-of-the-art attention mechanisms to faciliate information flow between the encoder and the decoder. Additionally, the decoder can be conditioned on sentence-level features to help with disambiguating.
-        
-        A task configuration for lemmatization with an Encoder-Decoder model and integrated sentence-level features is shown below.
-        
-        ```json
-        {
-          "tasks": [
-            {
-              "name": "lemma",
-              "level": "char",
-              "target": true,
-              "decoder": "attentional",
-              "context": "sentence",
-              "layer": -1,
-              "schedule": {
-                "patience": 3
-              }
-            }
-          ]
-        }
-        ```
-        
-        ## 7. Improving feature extraction with a joint Language Model loss
-        
-        Pie has a built-in option to improve feature extraction by predicting neighboring words from the sentence-level feature vectors. The mechanism has been thoroughly tested for lemmatization in research currently submitted to review and it has been shown to be very effective for languages without a fixed writing standard (e.g. historical languages) and other languages with high token-lemma ambiguity. Besides, there is nothing in theory opposing the idea that it might help with other tasks such as POS-tagging, morphological analyses, etc...  The options affecting the joint LM-loss are: `include_lm` (switch on the option), `lm_shared_softmax` (whether to share parameters between forward and backward LMs, recommended value: `true`), `lm_schedule` (parameters to lower the weight assigned to the LM loss over training, once the LM loss starts overfitting it is a good idea to start reducing the loss and eventually set it to 0 to avoid affecting the learning of the target task).
-        
-        ## 8. Multi-task learning
-        
-        When more than one task is defined, at least and at most one task has to have the key-value pair `"target": true`, denoting that that's the task we ultimately care about. All the other tasks will be treated as auxiliary tasks with the goal of extracting better features for the target task. Note that in any case the model will still be able to predict output for auxiliary tasks, but in the spirit of multi-task learning, you will prefer to train a separate model for each of the tasks you care about, selecting each time the appropriate target task and letting all other tasks help the optimization. In the end, you have as many models as tasks you care about, each of which has been optimized for the respective task.
-        
-        ### More on auxiliary tasks
-        
-        An auxiliary task might help learning better features that the classifier for the target task can exploit to produce better (in terms of classification performance) and more robust output (less susceptible to spurious correlations). However, training dynamics in a multi-task setting are complex (even more so than in a normal setting), since different tasks usually results in different learning curves that have to be monitored. In particular, if an auxiliary task converges before the target task, further training might lead that auxiliary task towards overfitting, thereby undoing the potential work done so far. Moreover, losses from different tasks are usually in different scales and this might have the effect that an auxiliary task with a loss on a higher scale dominates training.
-        
-        In order to avoid it, the strategy chosen for PIE consists on set learning schedules for tasks (similar to early stopping) that decrease the weights given to particular tasks over time based on development performance. 
-        
-        Multi-task learning consists on jointly training a model for different tasks while sharing parts of the general architecture for all tasks. This can be accomplished by either computing the loss for all tasks every batch and aggregating it before the backward pass, or optimizing in each batch for a single task randomly sampled based on a particular distribution. PIE follows the latter setting, which is known to produce better results.
-        
-        Additionally, it is also important, in case of a multi-layer sentence-level feature extractor, to select at what layer a particular task can help the most (this can be controlled with the "layer" option).
-        
-        Finally, multi-task learning is far from being a silver bullet and it is an empirical question whether a multi-task learning setup will yield improvements. It is recommended to first train a single model, and then try different multi-task learning configuration to see if improvements can be achieved.
-        
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
+
+# (Pa)PIE: A Framework for Joint Learning of Sequence Labeling Tasks
+
+[![DOI](https://zenodo.org/badge/131014015.svg)](https://zenodo.org/badge/latestdoi/131014015)
+
+![Improving Lemmatization of Non-Standard Languages with Joint Learning (NAACL19 Paper)](https://www.aclweb.org/anthology/N19-1153/)
+
+**Warning:** This is a fork from [pie](https://github.com/emanjavacas/pie). It provides some sometime *unstable* improvement over the original software.
+
+PIE was primarily conceived to make experimentation on sequence labeling of variation-rich languages easy and user-friendly. PIE has been tested mostly for Lemmatization but other SoTA accuracies from other tasks like POS have been reproduced (cf. Plank et al ). PIE is *highly* configurable both in terms of input preprocessing and model definition, in principle not requiring users to write any code (instead experiments are defined with json files). It is highly modular and therefore easy to extend. It includes transductive lemmatization as an additional sequence labeling task and, finally, it is reasonably fast and memory efficient.
+
+Documentation is work in progress and it will improve over the following months. A good place to learn about its functionality is to check `pie/default_settings.json` which explains all input parameters and shows a full example of a config file (minus input data).
+
+If you find `pie` useful, please use the following reference:
+
+```
+@inproceedings{manjavacas-etal-2019-improving,
+    title = "Improving Lemmatization of Non-Standard Languages with Joint Learning",
+    author = "Manjavacas, Enrique  and
+      K{\'a}d{\'a}r, {\'A}kos  and
+      Kestemont, Mike",
+    booktitle = "Proceedings of the 2019 Conference of the North {A}merican Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers)",
+    month = jun,
+    year = "2019",
+    address = "Minneapolis, Minnesota",
+    publisher = "Association for Computational Linguistics",
+    url = "https://www.aclweb.org/anthology/N19-1153",
+    doi = "10.18653/v1/N19-1153",
+    pages = "1493--1503",
+    abstract = "Lemmatization of standard languages is concerned with (i) abstracting over morphological differences and (ii) resolving token-lemma ambiguities of inflected words in order to map them to a dictionary headword. In the present paper we aim to improve lemmatization performance on a set of non-standard historical languages in which the difficulty is increased by an additional aspect (iii): spelling variation due to lacking orthographic standards. We approach lemmatization as a string-transduction task with an Encoder-Decoder architecture which we enrich with sentence information using a hierarchical sentence encoder. We show significant improvements over the state-of-the-art by fine-tuning the sentence encodings to jointly optimize a bidirectional language model loss. Crucially, our architecture does not require POS or morphological annotations, which are not always available for historical corpora. Additionally, we also test the proposed model on a set of typologically diverse standard languages showing results on par or better than a model without fine-tuned sentence representations and previous state-of-the-art systems. Finally, to encourage future work on processing of non-standard varieties, we release the dataset of non-standard languages underlying the present study, which is based on openly accessible sources.",
+}
+```
+
+## 1. Installation
+
+PIE is available from pypi, which means that all you should need to do is:
+
+```bash
+pip install nlp-pie
+```
+
+### For development
+
+If you are planning to develop on top of PIE, the easiest way is to get setup is to download the repository and install the dependencies (see `requirements.txt`). The only step needed to have `pie` available from any place in the file system is to add the path to `pie` to the `PYTHONPATH` environment variable. There are two ways to accomplish this:
+
+- From your bash init file (depending on your distro and configuration this could be `.bashrc`, `.bash_profile`, `.profile`, etc...):
+
+```bash
+export PYTHONPATH="$PYTHONPATH:/path/to/pie"
+```
+
+- From your python script, using `sys`:
+
+```python
+import sys
+sys.path.append('/path/to/pie')
+```
+
+## 2. Training
+
+Training models is done with `pie train path/to/config.json` (or script `python pie/scripts/train.py`. All non-nested parameters can be overwritten directly from the command line using environment variables like `PIE_DEVICE=cpu` (for input parameter `device`. Warning: bear in mind that due to the way bash parses environment variables `PIE_...=False` will be parsed into a boolean `True`, which might be counter-intuitive. If you wish to get `False` for a parameter from the command line you can use `PIE_...=""`).
+
+## 3. Evaluation
+
+A given model can be evaluated with `pie evaluate` (or `python pie/scripts/evaluate.py`).
+
+## 4. Tagging
+
+Given one or several trained models, two scripts are provided in order to tag given input: `pie tag` and `pie tag-pipe` (or `python pie/scripts/tag.py`, `python pie/scripts/tag_pipe.py`), the difference being that the first tags input files and the second can take input from a unix pipe.
+
+Common to both scripts is the *model specification* that allows to combine several models, where the output for a particular task is taken from a model that excels at that task.
+For example, given models `good-pos-tagger.tar` and `good-lemma-tagger.tar`, we can define a tagger that uses `good-pos-tagger.tar` for POS-tagging and `good-lemma-tagger.tar` for lemmatization with the following specification: `<good-lemma-tagger.tar,lemma><good-pos-tagger.tar,pos>`.
+
+- If your input is in a file `test.txt` (with a sentence per line) you can use:
+
+`pie tag "<good-lemma-tagger.tar,lemma><good-pos-tagger.tar,pos>" test.txt`
+
+and the output will be written to `test.pie.txt`
+
+- If you want to pass input from the command line, you can use:
+```
+$ echo "el gato duerme encima de la silla" | pie tag-pipe spanish-lemmatizer.rar
+
+token	lemma
+el	el
+gato	gato
+duerme	dormir
+encima	encima
+de	de
+la	el
+silla	silla
+```
+
+## 5. Model
+
+PIE underlying model comprises a set of hierarchical feature extractors from the character-level up to the sentence-level. For each input token a sentence-level feature vector is extracted and used for the prediction of any number of target tasks (e.g. POS-tagging, lemmatization, ...). A visualization of the underlying model using bidirectional RNNs to extract word-level and sentence-level features is shown below.
+
+![PIE](./img/PIE.svg)
+
+Prediction is accomplished with decoder modules. We provide implementations of a `linear` decoder trained to maximize the probability assigned by the model to the corpus data via a softmax function (similar to a MaxEnt classifier). A `crf` decoder, particularly suited for tasks that imply a dependency between neighboring output tags and an `attentional` decoder, suited for tasks that can be solved by generating the token-level output character by characters in a string transduction manner (e.g. lemmatization, normalization).
+
+## 6. Configuration files
+
+Training a model only requires a model specification and paths to training and dev datasets. Pie user interface employs a simple json file (in order to allow in-line comments, we make use of the package `JSON_minify`), an example of which can be seen below:
+
+```json
+{
+  "modelname": "lemmatization-latin",
+  "modelpath": "models",
+
+  "input_path": "datasets/LLCT1/train.tsv",
+  "dev_path": "datasets/LLCT1/dev.tsv",
+  "sep": "\t",
+ 
+  "tasks": [
+    {
+      "name": "lemma",
+      "target": true,
+      "context": "sentence",
+      "level": "char",
+      "decoder": "attentional",
+      "settings": {
+        "bos": true,
+        "eos": true,
+        "lower": true,
+        "target": "lemma"
+      },
+      "layer": -1
+    }
+  ],
+  "batch_size": 25,
+  "epochs": 100,
+  
+  "dropout": 0.25,
+  "optimizer": "Adam",
+  "patience": 3,
+  "lr": 0.001,
+  "lr_factor": 0.75,
+  "lr_patience": 2,
+  
+  "cell": "GRU",
+  "num_layers": 1,
+  "hidden_size": 150,
+  "wemb_dim": 0,
+  "cemb_dim": 300,
+  "cemb_type": "rnn",
+  "cemb_layers": 2
+}
+```
+
+The very minimum set of options required to train a model includes `input_path` (path to files with training data), `dev_path` (path to files with development data), and `tasks`, which defines the model to be trained. Other parameters refer to model hyperparameters (`cell`, `num_layers`, `hidden_size`, `wemb_dim`, `cemb_dim`, `cemb_type`, `cemb_layers`), training (`batch_size`, `epochs`) and optimization (`dropout`, `optimizer`, `patience`, `lr`, `lr_factor`, `lr_patience).
+
+### POS tagging using a CRF
+
+```json
+{
+  "tasks": [
+    {
+      "name": "pos", 
+      "target": true,
+      "decoder": "crf",
+      "layer": -1
+    }
+  ]
+}
+
+```
+
+### POS tagging using a linear decoder and 2 auxiliary tasks
+```json
+{
+  "tasks": [
+    {
+      "name": "pos",
+      "level": "token",
+      "target": true,
+      "decoder": "crf",
+      "layer": -1,
+      "schedule": {
+        "patience": 3
+      }
+    },
+    {
+      "name": "case",
+      "level": "token",
+      "target": false,
+      "decoder": "linear",
+      "layer": 0,
+      "schedule": {
+        "patience": 2,
+        "factor": 0.5
+      }
+    },
+    {
+      "name": "number",
+      "level": "token",
+      "target": false,
+      "decoder": "linear",
+      "layer": 0,
+      "schedule": {
+        "patience": 2,
+        "factor": 0.5
+      }
+    }
+  ]
+}
+```
+
+By setting a schedule we can fine-tune the learning dynamics of auxiliary tasks in a multi-task settings (see below for more information on this). 
+
+To avoid verbosity, parameters invariant across auxiliary tasks can be specified only once using `task_defaults`. Similarly, learning schedule parameters invariant across tasks (`factor`, `patience`, `threshold`, `min_weight`) can be factored out of the task schedule definition. In summary, the previous configuration can be rewritten in the following form:
+
+```json
+{
+  "tasks": [
+    {
+      "name": "pos",
+      "level": "token",
+      "target": true,
+      "decoder": "crf",
+      "layer": -1,
+      "schedule": {
+        "patience": 3
+      }
+    },
+    {
+      "name": "case"
+    },
+    {
+      "name": "number"
+    }
+  ],
+  "task_defaults": {
+    "level": "token",
+    "decoder": "linear",
+    "layer": 0
+  },
+  "patience": 2,
+  "factor": 0.5
+}
+
+```
+
+### Transduction-based lemmatization
+
+PIE has built-in support for lemmatization as a string transduction task using an Encoder-Decoder architecture as shown below (lemmatizing Latin token "esse" to its lemma "edo"):
+
+![Encoder-Decoder for lemmatization](./img/seq2seq.png)
+
+PIE implements several state-of-the-art attention mechanisms to faciliate information flow between the encoder and the decoder. Additionally, the decoder can be conditioned on sentence-level features to help with disambiguating.
+
+A task configuration for lemmatization with an Encoder-Decoder model and integrated sentence-level features is shown below.
+
+```json
+{
+  "tasks": [
+    {
+      "name": "lemma",
+      "level": "char",
+      "target": true,
+      "decoder": "attentional",
+      "context": "sentence",
+      "layer": -1,
+      "schedule": {
+        "patience": 3
+      }
+    }
+  ]
+}
+```
+
+## 7. Improving feature extraction with a joint Language Model loss
+
+Pie has a built-in option to improve feature extraction by predicting neighboring words from the sentence-level feature vectors. The mechanism has been thoroughly tested for lemmatization in research currently submitted to review and it has been shown to be very effective for languages without a fixed writing standard (e.g. historical languages) and other languages with high token-lemma ambiguity. Besides, there is nothing in theory opposing the idea that it might help with other tasks such as POS-tagging, morphological analyses, etc...  The options affecting the joint LM-loss are: `include_lm` (switch on the option), `lm_shared_softmax` (whether to share parameters between forward and backward LMs, recommended value: `true`), `lm_schedule` (parameters to lower the weight assigned to the LM loss over training, once the LM loss starts overfitting it is a good idea to start reducing the loss and eventually set it to 0 to avoid affecting the learning of the target task).
+
+## 8. Multi-task learning
+
+When more than one task is defined, at least and at most one task has to have the key-value pair `"target": true`, denoting that that's the task we ultimately care about. All the other tasks will be treated as auxiliary tasks with the goal of extracting better features for the target task. Note that in any case the model will still be able to predict output for auxiliary tasks, but in the spirit of multi-task learning, you will prefer to train a separate model for each of the tasks you care about, selecting each time the appropriate target task and letting all other tasks help the optimization. In the end, you have as many models as tasks you care about, each of which has been optimized for the respective task.
+
+### More on auxiliary tasks
+
+An auxiliary task might help learning better features that the classifier for the target task can exploit to produce better (in terms of classification performance) and more robust output (less susceptible to spurious correlations). However, training dynamics in a multi-task setting are complex (even more so than in a normal setting), since different tasks usually results in different learning curves that have to be monitored. In particular, if an auxiliary task converges before the target task, further training might lead that auxiliary task towards overfitting, thereby undoing the potential work done so far. Moreover, losses from different tasks are usually in different scales and this might have the effect that an auxiliary task with a loss on a higher scale dominates training.
+
+In order to avoid it, the strategy chosen for PIE consists on set learning schedules for tasks (similar to early stopping) that decrease the weights given to particular tasks over time based on development performance. 
+
+Multi-task learning consists on jointly training a model for different tasks while sharing parts of the general architecture for all tasks. This can be accomplished by either computing the loss for all tasks every batch and aggregating it before the backward pass, or optimizing in each batch for a single task randomly sampled based on a particular distribution. PIE follows the latter setting, which is known to produce better results.
+
+Additionally, it is also important, in case of a multi-layer sentence-level feature extractor, to select at what layer a particular task can help the most (this can be controlled with the "layer" option).
+
+Finally, multi-task learning is far from being a silver bullet and it is an empirical question whether a multi-task learning setup will yield improvements. It is recommended to first train a single model, and then try different multi-task learning configuration to see if improvements can be achieved.
+
+
```

### Comparing `PaPie-0.3.9/PaPie.egg-info/SOURCES.txt` & `PaPie-0.4.0/PaPie.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,28 +23,26 @@
 pie/utils.py
 pie/data/__init__.py
 pie/data/base_reader.py
 pie/data/conll_reader.py
 pie/data/dataset.py
 pie/data/reader.py
 pie/data/tabreader.py
-pie/data/tei_reader.py
 pie/data/preprocessors/__init__.py
 pie/data/preprocessors/edit_tree_tuples.py
 pie/data/preprocessors/edit_trees.py
 pie/data/preprocessors/greedy_scripts.py
 pie/models/__init__.py
 pie/models/attention.py
 pie/models/base_model.py
 pie/models/beam_search.py
 pie/models/decoder.py
 pie/models/embedding.py
 pie/models/encoder.py
 pie/models/highway.py
-pie/models/loaders.py
 pie/models/lstm.py
 pie/models/model.py
 pie/models/scorer.py
 pie/scripts/__init__.py
 pie/scripts/evaluate.py
 pie/scripts/group.py
 pie/scripts/inspect_model.py
```

### Comparing `PaPie-0.3.9/README.md` & `PaPie-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
-# PIE: A Framework for Joint Learning of Sequence Labeling Tasks
+# (Pa)PIE: A Framework for Joint Learning of Sequence Labeling Tasks
 
 [![DOI](https://zenodo.org/badge/131014015.svg)](https://zenodo.org/badge/latestdoi/131014015)
 
 ![Improving Lemmatization of Non-Standard Languages with Joint Learning (NAACL19 Paper)](https://www.aclweb.org/anthology/N19-1153/)
 
+**Warning:** This is a fork from [pie](https://github.com/emanjavacas/pie). It provides some sometime *unstable* improvement over the original software.
+
 PIE was primarily conceived to make experimentation on sequence labeling of variation-rich languages easy and user-friendly. PIE has been tested mostly for Lemmatization but other SoTA accuracies from other tasks like POS have been reproduced (cf. Plank et al ). PIE is *highly* configurable both in terms of input preprocessing and model definition, in principle not requiring users to write any code (instead experiments are defined with json files). It is highly modular and therefore easy to extend. It includes transductive lemmatization as an additional sequence labeling task and, finally, it is reasonably fast and memory efficient.
 
 Documentation is work in progress and it will improve over the following months. A good place to learn about its functionality is to check `pie/default_settings.json` which explains all input parameters and shows a full example of a config file (minus input data).
 
 If you find `pie` useful, please use the following reference:
 
 ```
```

### Comparing `PaPie-0.3.9/pie/data/base_reader.py` & `PaPie-0.4.0/pie/data/base_reader.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/data/conll_reader.py` & `PaPie-0.4.0/pie/data/conll_reader.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/data/dataset.py` & `PaPie-0.4.0/pie/data/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-
 import warnings
 from functools import partial
 import tarfile
 import json
 import yaml
 try:
     from yaml import CLoader as Loader, CDumper as Dumper
 except ImportError:
     from yaml import Loader, Dumper
 import logging
 from collections import Counter, defaultdict
 import random
+from typing import Dict, List, Union, Tuple, Any
 
 import torch
 
 from pie import utils, torch_utils, constants
 from . import preprocessors
 
+# Typing utilities
+Sentence = List[str]
+TaskName = str
+Label = str
+DictGT = Dict[TaskName, List[Label]]
+
 
 class LabelEncoder(object):
     """
     Label encoder
     """
     def __init__(self, level='token', name=None, target=None,
                  lower=False, utfnorm=False, utfnorm_type='NFKD', drop_diacritics=False,
@@ -157,14 +163,37 @@
         else:
             most_common = self.freqs.most_common()
 
         self.inverse_table = list(self.reserved) + [sym for sym, _ in most_common]
         self.table = {sym: idx for idx, sym in enumerate(self.inverse_table)}
         self.fitted = True
 
+    def register_upper(self):
+        """ Params registers the same vocabulary but in full uppercase
+
+        Important when using the upper strategy
+        """
+        inp = self.inverse_table[len(self.reserved):]
+        new_chars = list(map(
+            lambda x: x.upper(),
+            filter(
+                lambda x: x.islower() and x.upper() not in inp,
+                inp
+            )
+        ))
+        if self.max_size:
+            t = len(self.inverse_table)
+            r = len(self.reserved)
+            if (self.max_size - t - r) > 0:
+                new_chars = new_chars[:min(len(new_chars), self.max_size-t-r)]
+            else:
+                return # We have too much in the vocab already
+        self.inverse_table.extend(new_chars)
+        self.table = {sym: idx for idx, sym in enumerate(self.inverse_table)}
+
     def preprocess_text(self, seq):
         """
         Apply surface level preprocessing such as lowering, unicode normalization
         """
         if self.text_preprocess_fn:
             seq = list(map(self.text_preprocess_fn, seq))
         return seq
@@ -305,25 +334,26 @@
 class MultiLabelEncoder(object):
     """
     Complex Label encoder for all tasks.
     """
     def __init__(self, word_max_size=None, word_min_freq=1, word_lower=False,
                  char_max_size=None, char_min_freq=None, char_lower=False,
                  char_eos=True, char_bos=True, utfnorm=False, utfnorm_type='NFKD',
-                 drop_diacritics=False):
+                 drop_diacritics=False, noise_strategies = None):
         self.word = LabelEncoder(max_size=word_max_size, min_freq=word_min_freq,
                                  lower=word_lower, utfnorm=utfnorm,
                                  utfnorm_type=utfnorm_type,
                                  drop_diacritics=drop_diacritics, name='word')
         self.char = LabelEncoder(max_size=char_max_size, min_freq=char_min_freq,
                                  level='char', lower=char_lower, name='char',
                                  eos=char_eos, bos=char_bos, utfnorm_type=utfnorm_type,
                                  utfnorm=utfnorm, drop_diacritics=drop_diacritics)
         self.tasks = {}
         self.nsents = None
+        self.noise_strategies = noise_strategies or {}
 
     def __repr__(self):
         return (
             '<MultiLabelEncoder>\n\t' +
             '\n\t'.join(map(str, [self.word, self.char] + list(self.tasks.values()))) +
             '\n</MultiLabelEncoder>')
 
@@ -360,15 +390,16 @@
                  char_max_size=settings.char_max_size,
                  char_min_freq=settings.char_min_freq,
                  char_lower=settings.char_lower,
                  char_eos=settings.char_eos,
                  char_bos=settings.char_bos,
                  utfnorm=settings.utfnorm,
                  utfnorm_type=settings.utfnorm_type,
-                 drop_diacritics=settings.drop_diacritics)
+                 drop_diacritics=settings.drop_diacritics,
+                 noise_strategies=settings.noise_strategies)
 
         for task in settings.tasks:
             if tasks is not None and task['settings']['target'] not in tasks:
                 raise ValueError("No available data for task [{}]".format(
                     task['settings']['target']))
             le.add_task(task['name'], level=task['level'], **task['settings'])
 
@@ -390,26 +421,31 @@
             self.char.add(inp)
 
             for le in self.tasks.values():
                 le.add(tasks[le.target], inp)
 
         self.word.compute_vocab()
         self.char.compute_vocab()
+
+        if self.noise_strategies["uppercase"]["apply"]:
+            self.word.register_upper()
+            self.char.register_upper()
+
         for le in self.tasks.values():
             le.compute_vocab()
 
         return self
 
     def fit_reader(self, reader):
         """
         fit reader in a non verbose way (to warn about parsing issues)
         """
         return self.fit(line for (_, line) in reader.readsents(silent=False))
 
-    def transform(self, sents):
+    def transform(self, sents: Union[List[Sentence], List[Tuple[Sentence, DictGT]]]):
         """
         Parameters
         ===========
         sents : list of Example's
 
         Returns
         ===========
@@ -562,15 +598,15 @@
             packed = self.pack_batch(batch, **kwargs)
             if return_raw:
                 inp, tasks = zip(*batch)
                 yield packed, (inp, tasks)
             else:
                 yield packed
 
-    def batch_generator(self, return_raw=False):
+    def _batch_generator_cached(self, return_raw=False):
         """
         Generator over dataset batches. Each batch is a tuple of (input, tasks):
             * (word, char)
                 - word : tensor(length, batch_size), padded lengths
                 - char : tensor(length, batch_size * words), padded lengths
             * (tasks) dictionary with tasks
         """
@@ -586,14 +622,71 @@
                 if return_raw:
                     yield batch, raw
                 else:
                     yield batch
         else:
             yield from self.batch_generator_(return_raw=return_raw)
 
+    def _get_noised_batch(self, raw_words, raw_targets, apply_noise: Dict[str, Dict[str, Any]]):
+        """
+
+        """
+        raw_words = list(raw_words)  # Was a Tuple before
+
+        # Run N strategies per N sentences rand on the range [0.00:1.00(
+        apply_strategies = torch.rand(len(apply_noise), len(raw_words))
+
+        # Iterate over strategies
+        for strat_id, (strat_name, strategy) in enumerate(apply_noise.items()):
+            targets = (apply_strategies[strat_id] < strategy.get("ratio", 0)).nonzero(as_tuple=True)
+
+            if not len(targets):
+                continue
+
+            changed_index = targets[0].tolist()
+
+            for index, sent, truth in zip(
+                    changed_index,
+                    map(raw_words.__getitem__, changed_index),
+                    map(raw_targets.__getitem__, changed_index)
+            ):
+                raw_words[index] = getattr(NoiseStrategies, strat_name)(
+                    sent,
+                    tasks=changed_index,
+                    **strategy.get("params", {})
+                )
+
+        # Recreate a batch
+        return self.pack_batch(list(zip(raw_words, raw_targets)), device=self.device)
+
+    def batch_generator(self, return_raw=False, apply_noise=None):
+        """
+        Generator over dataset batches. Each batch is a tuple of (input, tasks):
+            * (word, char)
+                - word : tensor(length, batch_size), padded lengths
+                - char : tensor(length, batch_size * words), padded lengths
+            * (tasks) dictionary with tasks
+        """
+        if apply_noise or return_raw:
+            for batch, raw in self._batch_generator_cached(return_raw=True):
+                if apply_noise:  # If we need to apply noise
+                    batch = self._get_noised_batch(*raw, apply_noise=apply_noise)
+                if return_raw:
+                    # Batch = ((word, wlen), (char, clen)), tasks
+                    # Raw Tuple[List[words], Tuple[Dict[task, List[gold]]...]]
+                    # For each strategy
+                        # Index = list(range(0, len(raw[0])+1), get N random
+                        # Then for each index, -> strategy(raw[0][1])
+                        # Batch[0] -> apply on word and char reusing index
+                    yield batch, raw
+                else:
+                    yield batch
+        else:
+            yield from self._batch_generator_cached(return_raw=False)
+
     def batch_generator_(self, return_raw=False):
         buf = []
         for (fpath, line_num), data in self.reader.readsents():
 
             # fill buffer
             buf.append(data)
 
@@ -647,7 +740,13 @@
         self.device = device
 
     def __getitem__(self, idx):
         return tuple(wrap_device(self.batches[idx], self.device))
 
     def __len__(self):
         return len(self.batches)
+
+
+class NoiseStrategies:
+    @staticmethod
+    def uppercase(inp: Sentence, tasks: DictGT = None, **kwargs) -> List[str]:
+        return list(map(str.upper, inp))
```

### Comparing `PaPie-0.3.9/pie/data/preprocessors/edit_trees.py` & `PaPie-0.4.0/pie/data/preprocessors/edit_trees.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/data/preprocessors/greedy_scripts.py` & `PaPie-0.4.0/pie/data/preprocessors/greedy_scripts.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/data/reader.py` & `PaPie-0.4.0/pie/data/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import random
 
 from pie.utils import get_filenames
 
 from .tabreader import TabReader
 from .conll_reader import CONLLReader, CONLLUReader
-from .tei_reader import TEIReader
 
 
 class Reader(object):
     """
     Dispatcher class
 
     Parameters
@@ -52,17 +51,14 @@
 
         elif fpath.endswith('conll'):
             return CONLLReader
 
         elif fpath.endswith('conllu'):
             return CONLLUReader
 
-        elif fpath.endswith('xml'):
-            return TEIReader
-
         else:
             raise ValueError("Unknown file format: {}".format(fpath))
 
     def reset(self):
         """
         Called after a full run over `readsents`
         """
```

### Comparing `PaPie-0.3.9/pie/data/tabreader.py` & `PaPie-0.4.0/pie/data/tabreader.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/default_settings.json` & `PaPie-0.4.0/pie/default_settings.json`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,19 @@
       // For target tasks, "patience", "threshold" control early stopping (how many steps
       // without improvement over the threshold we need before stopping learning).
       // For auxiliary tasks, they control how we decay the loss weight of that task
       // and extra parameters are available: "factor" (by how much), "min_weight"
       // (minimum weight) given to the loss, "weight" (initial weight) and "mode"
       // (whether the task dev score is being minimized "min" or maximized "max")
       "schedule": {
-	"patience": 2, "threshold": 0.001
+        "patience": 2,
+        "threshold": 0.001,
+        // Metric to fit on
+        // Can be "accuracy", "balanced-accuracy", "f1", "precision" or "recall"
+         "evaluation": "accuracy"
       },
 
       "default": "copy", // while processing the files if the field is missing predict
       // the input token or something else:
       // - "copy" for copy over the token form
       // - "UNK" predict "UNK"
       "read_only": false // encode task but don't model it
@@ -83,15 +87,20 @@
   ],
 
   // task defaults for any given auxiliary task (can be overwritten by a task definition)
   "task_defaults": {
     "level": "token",
     "layer": -1,
     "decoder": "linear",
-    "context": "sentence"
+    "context": "sentence",
+    "schedule": {
+      // Can be "accuracy", "balanced-accuracy", "f1", "precision",
+      //    and "recall"
+       "evaluation": "accuracy"
+    }
   },
 
   // general task schedule params (can be overwritten in the "settings" entry of each)
   "patience": 100, // task patience (global early stopping patience for target task)
   "factor": 1, // default task schedule factor
   "threshold": 0, // default task schedule thresholed
   "min_weight": 0, // default task schedule min_weight
@@ -118,29 +127,48 @@
   "load_pretrained_encoder": "", // path to file with pretrained sentence encoder
   "freeze_embeddings": false, // whether to freeze the word embeddings
 
   // * Optimization
   "dropout": 0.0, // dropout
   "word_dropout": 0.0, // input word dropout
   "optimizer": "Adam", // optimizer type
+  "optimizer_params": {
+    // Advance Optimizers params
+  },
   "clip_norm": 5.0, // clip norm of gradient up to this value
   "lr": 0.001,
-  "lr_factor": 0.75, // lr schedule (decrease lr by this factor after `lr_patience` epochs
-  // without improvement on dev-set data)
-  "min_lr": 0.000001, // minimum learning rate
-  "lr_patience": 2, // patience for lr schedule
+
+  "lr_scheduler": "ReduceLROnPlateau",
+  "lr_scheduler_delay": 0, // Number of steps without using the lr_scheduler
+  "lr_scheduler_params": {
+    // needs to be adapted if lr_scheduler is not ReduceLROnPlateau
+    "mode": "max",
+    "factor": 0.75,
+    "patience": 2,
+    "min_lr": 0.000001
+  },
+
   "checks_per_epoch": 1, // check model on dev-set so many times during epoch
 
   // * Model hyperparameters
   "wemb_dim": 0, // word-level embedding dimension (if 0 no word embeddings are use)
   "cemb_dim": 150, // input dimension for char-level embeddings
   "cemb_type": "rnn", // character embedding type (rnn or cnn)
   "custom_cemb_cell": false, // whether to use the custom lstm cell for word embeddings
   "cemb_layers": 1, // number of layers for the rnn-embeddings and the attentional decoder
   "merge_type": "concat", // how to merge word-level and char-level embs (mixer or concat)
   "scorer": "general", // attention type (one of "general", "dot" and "bahdanau")
   "linear_layers": 1, // number of layers for linear decoders
   "hidden_size": 300, // sentence encoding dimension
   "num_layers": 1, // num recurrent layers for the sentence encoder
   "cell": "LSTM", // cell type for rnns
-  "init_rnn": "default" // initializing RNNs (default, xavier_uniform, orthogonal)
+  "init_rnn": "default", // initializing RNNs (default, xavier_uniform, orthogonal)
+
+
+   "noise_strategies": {
+     "uppercase": {
+       "apply": false,
+       "ratio": 0.10,
+       "params": {}
+     }
+   }
 }
```

### Comparing `PaPie-0.3.9/pie/initialization.py` & `PaPie-0.4.0/pie/initialization.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/models/attention.py` & `PaPie-0.4.0/pie/models/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         self.W_a = nn.Linear(dim, dim, bias=False)
         self.init()
 
     def init(self):
         initialization.init_linear(self.W_a)
 
     def forward(self, dec_out, enc_outs, **kwargs):
-        return DotScorer(self.W_a(dec_out), enc_outs)
+        w = self.W_a(dec_out)
+        return DotScorer(w, enc_outs)
 
 
 class BahdanauScorer(nn.Module):
     """
     Projects both query decoder state and encoder states to an attention space.
     The scores are computed by a dot product with a learnable param v_a after
     transforming the sum of query decoder state and encoder state with a tanh.
```

### Comparing `PaPie-0.3.9/pie/models/base_model.py` & `PaPie-0.4.0/pie/models/base_model.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/models/beam_search.py` & `PaPie-0.4.0/pie/models/beam_search.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/models/decoder.py` & `PaPie-0.4.0/pie/models/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,15 @@
             # We replace the value at indexes *tensor_to_original_batch_indexes* by the prediction
             #   of current sequence output
             seq_output[tensor_to_original_batch_indexes] = inp
 
             # We set the score where we have EOS predictions as 0
             score[inp == eos] = 0
             # So that we can add the score to finale scores
-            final_scores[tensor_to_original_batch_indexes] += score.cpu()
+            final_scores[tensor_to_original_batch_indexes.cpu()] += score.cpu()
 
             # We add this new output to the final hypothesis
             hyps.append(seq_output.tolist())
 
             # If there nothing else than EOS, it's the end of the prediction time
             if non_eos.sum() == 0:
                 break
```

### Comparing `PaPie-0.3.9/pie/models/embedding.py` & `PaPie-0.4.0/pie/models/embedding.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/models/encoder.py` & `PaPie-0.4.0/pie/models/encoder.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/models/highway.py` & `PaPie-0.4.0/pie/models/highway.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/models/lstm.py` & `PaPie-0.4.0/pie/models/lstm.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/models/model.py` & `PaPie-0.4.0/pie/models/model.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/models/scorer.py` & `PaPie-0.4.0/pie/models/scorer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,86 @@
-
+from typing import Optional
 import yaml
 import difflib
 from termcolor import colored
 from terminaltables import github_table
 from collections import Counter, defaultdict
 
-from sklearn.metrics import accuracy_score, precision_recall_fscore_support
-from sklearn.utils.multiclass import unique_labels
+from torchmetrics.functional import accuracy, precision, recall, f1_score
 import numpy as np
-from pie import utils
+import torch
 from pie import constants
 
 
+def format_score(score):
+    return round(float(score), 4)
+
+
+class _LocalEncoder:
+    def __init__(self, *values):
+        self.toi = sorted(list(set(values)))
+
+    def encode(self, array):
+        return torch.tensor([
+            self.toi.index(v)
+            for v in array
+        ], device="cpu")
+
+    def decode(self, idx: int) -> str:
+        return self.toi[idx]
+
+def precision_recall_fscore_support(
+        preds: torch.Tensor,
+        trues: torch.Tensor,
+        average: Optional[str] = "micro",
+        num_classes: int = -1
+):
+    p = precision(preds, trues, task="multiclass", average=average, num_classes=num_classes)
+    r = recall(preds, trues, task="multiclass", average=average, num_classes=num_classes)
+    f1 = f1_score(preds, trues, task="multiclass", average=average, num_classes=num_classes)
+    if average == "micro":
+        s = len(trues)
+    else:
+        s = None
+    return p, r, f1, s
+
+
 def get_known_and_ambigous_tokens(trainset, label_encoders):
     """ Retrieve known and ambiguous token for all label encoders, for one dataset
 
     :param trainset: Trainset
     :param label_encoders: List of label encoders
     :return: Known set of tokens, ambiguous token par task (Dict[task, Set[str])
     """
     known = set()
     ambs = defaultdict(lambda: defaultdict(Counter))
-    targets = [le.target for le in label_encoders]
+    # targets = [le.target for le in label_encoders]
     for _, (inp, tasks) in trainset.reader.readsents():
         known.update(inp)
         for le in label_encoders:
             for tok, true in zip(inp, le.preprocess(tasks[le.target], inp)):
                 ambs[le.target][tok][true] += 1
     ambs = {t: set(tok for tok in ambs[t] if len(ambs[t][tok]) > 1) for t in ambs}
     return known, ambs
 
 
 def compute_scores(trues, preds):
 
-    def format_score(score):
-        return round(float(score), 4)
+    enc = _LocalEncoder(*trues, *preds)
+    preds_array = enc.encode(preds)
+    trues_array = enc.encode(trues)
+    num_classes = len(enc.toi)
+    p, r, f1, s = precision_recall_fscore_support(preds_array, trues_array, num_classes=num_classes)
+    b = format_score(recall(preds_array, trues_array, task="multiclass", average="macro", num_classes=num_classes))
+    p = format_score(p)
+    r = format_score(r)
+    a = format_score(accuracy(preds_array, trues_array, task="multiclass", average="micro", num_classes=num_classes))
 
-    with utils.shutup():
-        p, r, f1, _ = precision_recall_fscore_support(trues, preds, average="macro")
-        p = format_score(p)
-        r = format_score(r)
-        a = format_score(accuracy_score(trues, preds))
-
-    return {'accuracy': a, 'precision': p, 'recall': r, 'support': len(trues)}
+    return {'accuracy': a, 'precision': p, 'recall': r, 'support': s,
+            'balanced-accuracy': b, 'f1': format_score(f1)}
 
 
 class Scorer(object):
     """
     Accumulate predictions over batches and compute evaluation scores
     """
     def __init__(self, label_encoder):
@@ -126,14 +160,16 @@
         output['known-tokens'] = compute_scores(knw_trues, knw_preds)
         support = len(unk_trues)
         if support > 0:
             output['unknown-tokens'] = compute_scores(unk_trues, unk_preds)
         support = len(amb_trues)
         if support > 0:
             output['ambiguous-tokens'] = compute_scores(amb_trues, amb_preds)
+
+        # compute scores for unknown targets
         support = len(unk_trg_trues)
         if support > 0:
             output['unknown-targets'] = compute_scores(unk_trg_trues, unk_trg_preds)
 
         return output
 
     def get_most_common(self, errors, most_common):
@@ -319,50 +355,71 @@
     def get_classification_report(self):
         return classification_report(
             y_true=self.trues,
             y_pred=self.preds)
 
     @staticmethod
     def scores_in_markdown(scores):
-        measures = ["accuracy", "precision", "recall", "support"]
+        measures = ["accuracy", "precision", "recall",
+                    "f1", "balanced-accuracy", "support"]
         table = [[""] + measures]
         for key in scores:
             table.append([key, *[scores[key][meas] for meas in measures]])
 
         return (github_table.GithubFlavoredMarkdownTable(table)).table
 
+    @property
+    def dict(self):
+        return {
+            "known_tokens": self.known_tokens,
+            "amb_tokens": self.amb_tokens,
+            "preds": self.preds,
+            "trues": self.trues,
+            "tokens": self.tokens
+        }
+
 
 def classification_report(y_true, y_pred, digits=2):
     """ Generate a classification report similar to
     sklearn.metrics.classification_report but in markdown
 
     :param y_true: List of GT values
     :param y_pred: List of predictions
     :param digits: Number of float digits
     :return: Github Markdown Table
     """
     floatfmt = "{0:" + '.{:}f'.format(digits) + "}"
 
-    labels = unique_labels(y_true, y_pred)
+    labels = list(set(y_true).union(set(y_pred)))
     target_names = [str(key) for key in labels]
 
-    last_line_heading = 'avg / total'
+    last_line_heading = '[Macro-Average]'
     headers = ["target", "precision", "recall", "f1-score", "support"]
 
-    p, r, f1, s = precision_recall_fscore_support(y_true, y_pred, average=None)
-
-    formatted = []
-    for nb_list in [p, r, f1]:
-        formatted.append([floatfmt.format(x) for x in nb_list.tolist()])
-    support = [[str(x) for x in s.tolist()]]
-
-    tbl_rows = list(zip(target_names, *formatted, *support))
+    enc = _LocalEncoder(*y_true, *y_pred)
+    preds_array = enc.encode(y_pred)
+    trues_array = enc.encode(y_true)
+    num_classes = len(enc.toi)
+    p, r, f1, s = precision_recall_fscore_support(preds_array, trues_array, average=None, num_classes=num_classes)
+
+    tbl_rows = []
+    for idx, (pre, rec, f1s) in enumerate(zip(p.tolist(), r.tolist(), f1.tolist())):
+        label = enc.decode(idx)
+        if y_true.count(label) > 0:  # Only take into account truth classes
+            tbl_rows.append([
+                label,
+                floatfmt.format(pre),
+                floatfmt.format(rec),
+                floatfmt.format(f1s),
+                str(y_true.count(label)),
+            ])
 
     # compute averages
+    tbl_rows.append(["-"]*5)
     last_row = [last_line_heading,
                 floatfmt.format(np.average(p)),
                 floatfmt.format(np.average(r)),
                 floatfmt.format(np.average(f1)),
-                str(np.sum(s))]
+                str(len(y_true))]
     tbl_rows.append(last_row)
 
     return github_table.GithubFlavoredMarkdownTable([headers] + tbl_rows).table
```

### Comparing `PaPie-0.3.9/pie/optimize.py` & `PaPie-0.4.0/pie/optimize.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/pretrain_encoder.py` & `PaPie-0.4.0/pie/pretrain_encoder.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/scripts/group.py` & `PaPie-0.4.0/pie/scripts/group.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,26 +72,35 @@
 @click.option('--model_info', is_flag=True, default=False)
 @click.option('--full', is_flag=True, default=False)
 @click.option('--confusion', default=False, is_flag=True)
 @click.option('--report', default=False, is_flag=True)
 @click.option('--markdown', default=False, is_flag=True)
 @click.option('--use_beam', is_flag=True, default=False)
 @click.option('--beam_width', type=int, default=12)
+@click.option('--confusion', default=False, is_flag=True,
+              help="Show the confusion matrix for most common terms at least")
+@click.option('--report', default=False, is_flag=True, help="Show metrics for each label on top of the class results")
+@click.option('--markdown', default=False, is_flag=True, help="Display results in markdown")
+@click.option("--export", default=False, is_flag=True, help="Export the data from the evaluation")
+@click.option("--export-name", default="full_report.json", help="Name of the exported file")
 def evaluate(model_path, test_path, train_path, settings, batch_size,
              buffer_size, device, model_info, full, confusion, report,
-             markdown, use_beam, beam_width):
+             markdown, export, export_name,
+             use_beam, beam_width):
     """ Evaluate [MODEL_PATH] against [TEST_PATH] using [TRAIN_PATH] to compute
     unknown tokens"""
     import pie.scripts.evaluate
     pie.scripts.evaluate.run(
         model_path=model_path, test_path=test_path, train_path=train_path,
         settings=settings, batch_size=batch_size, buffer_size=buffer_size,
         device=device, model_info=model_info, full=full, confusion=confusion,
         report=report, markdown=markdown,
-        use_beam=use_beam, beam_width=beam_width)
+        use_beam=use_beam, beam_width=beam_width,
+        export_scorer=export, export_name=export_name
+    )
 
 
 @pie_cli.command("train")
 @click.argument('config_path')
 def train(config_path):
     """ Train a model using the file at [CONFIG_PATH]"""
     import pie.scripts.train
```

### Comparing `PaPie-0.3.9/pie/scripts/tag.py` & `PaPie-0.4.0/pie/scripts/tag.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/scripts/tag_pipe.py` & `PaPie-0.4.0/pie/scripts/tag_pipe.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/scripts/train.py` & `PaPie-0.4.0/pie/scripts/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 import logging
 
 import pie
 from pie.settings import settings_from_file
 from pie.trainer import Trainer
 from pie import initialization
 from pie.data import Dataset, Reader, MultiLabelEncoder
-from pie.models import SimpleModel, get_pretrained_embeddings
-from pie import optimize
+from pie.models import SimpleModel
 
 # set seeds
 import random
 import numpy
 import torch
 
 
@@ -103,26 +102,21 @@
         include_lm=settings.include_lm, lm_shared_softmax=settings.lm_shared_softmax,
         # decoder
         scorer=settings.scorer, linear_layers=settings.linear_layers)
 
     # pretrain(/load pretrained) embeddings
     if model.wemb is not None:
         if settings.pretrain_embeddings:
-            print("Pretraining word embeddings")
-            wemb_reader = Reader(
-                settings, settings.input_path, settings.dev_path, settings.test_path)
-            weight = get_pretrained_embeddings(
-                wemb_reader, label_encoder, size=settings.wemb_dim,
-                window=5, negative=5, min_count=1)
-            model.wemb.weight.data = torch.tensor(weight, dtype=torch.float32)
+            raise ValueError("Pretrained Gensim embedding is not supported in PaPie since 0.3.12. "
+                             "Check load_pretrained_embeddings as an alternative.")
 
         elif settings.load_pretrained_embeddings:
             print("Loading pretrained embeddings")
             if not os.path.isfile(settings.load_pretrained_embeddings):
-                print("Couldn't find pretrained eembeddings in: {}".format(
+                print("Couldn't find pretrained embeddings in: {}".format(
                     settings.load_pretrained_embeddings))
             initialization.init_pretrained_embeddings(
                 settings.load_pretrained_embeddings, label_encoder.word, model.wemb)
 
     # load pretrained weights
     if settings.load_pretrained_encoder:
         model.init_from_encoder(pie.Encoder.load(settings.load_pretrained_encoder))
@@ -197,12 +191,13 @@
     parser.add_argument('config_path', nargs='?', default='config.json')
     parser.add_argument('--opt_path', help='Path to optimization file (see opt.json)')
     parser.add_argument('--n_iter', type=int, default=20)
     args = parser.parse_args()
 
     settings = settings_from_file(args.config_path)
 
+    from pie import optimize
     if args.opt_path:
         opt = optimize.read_opt(args.opt_path)
         optimize.run_optimize(run, settings, opt, args.n_iter)
     else:
         run(settings)
```

### Comparing `PaPie-0.3.9/pie/settings.py` & `PaPie-0.4.0/pie/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,14 +102,20 @@
         if task.get('target', False):
             if has_target:
                 raise ValueError("Got more than one target task")
             has_target = True
     if not has_target:
         raise ValueError("Needs at least one target task")
 
+    # backward compatibility
+    if "lr_patience" in settings:
+        settings.lr_scheduler_params['patience'] = settings.lr_patience
+    if "lr_factor" in settings:
+        settings.lr_scheduler_params['factor'] = settings.lr_factor
+
     return settings
 
 
 def settings_from_file(config_path):
     """Loads and parses a parameter file.
 
     Parameters
```

### Comparing `PaPie-0.3.9/pie/tagger.py` & `PaPie-0.4.0/pie/tagger.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/torch_utils.py` & `PaPie-0.4.0/pie/torch_utils.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/trainer.py` & `PaPie-0.4.0/pie/trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-
+import inspect
 import os
 import uuid
 import logging
 import time
 import collections
 import random
 import tempfile
-
+from typing import ClassVar
 
 import tqdm
 
 import torch
 from torch import optim
+from torch.optim import Optimizer
 from torch.nn.utils import clip_grad_norm_
+import pytorch_optimizer as ext_optims
 
 logging.basicConfig(format='%(asctime)s : %(message)s', level=logging.INFO)
 
 
 def get_batch_task(tasks, **kwargs):
     tnames, target = [], None
     for task in tasks:
@@ -146,27 +148,51 @@
                     self.tasks[task]['weight'] = max(new_weight, min_weight)
 
     def get_weights(self):
         return {task: self.tasks[task]['weight'] for task in self.tasks}
 
 
 class LRScheduler(object):
-    def __init__(self, optimizer, threshold=0.0, **kwargs):
-        self.lr_scheduler = optim.lr_scheduler.ReduceLROnPlateau(
-            optimizer, mode='max', threshold=threshold, **kwargs)
+    def __init__(self, optimizer,
+                 lr_scheduler='ReduceLROnPlateau',
+                 delay=0, **kwargs):
+
+        self.nb_steps: int = 0
+        self.delay: int = delay
+        lr_scheduler_cls = getattr(optim.lr_scheduler, lr_scheduler)
+        params = inspect.signature(lr_scheduler_cls).parameters
+        self.lr_scheduler = lr_scheduler_cls(
+            optimizer,
+            # pick kwargs that fit the selected scheduler
+            **{kwarg: val for kwarg, val in kwargs.items() if kwarg in params})
 
     def step(self, score):
-        self.lr_scheduler.step(score)
+        self.nb_steps += 1
+
+        # apply the step() method of the lr_scheduler when delay is reached
+        if self.delay and self.nb_steps <= self.delay:
+            return
+
+        if isinstance(self.lr_scheduler, optim.lr_scheduler.ReduceLROnPlateau):
+            self.lr_scheduler.step(score)
+        else:
+            self.lr_scheduler.step()
 
     def __repr__(self):
-        return '<LrScheduler lr="{:g}" steps="{}" patience="{}" threshold="{}"/>' \
-            .format(self.lr_scheduler.optimizer.param_groups[0]['lr'],
-                    self.lr_scheduler.num_bad_epochs,
-                    self.lr_scheduler.patience,
-                    self.lr_scheduler.threshold)
+        res = '<LrScheduler="{}" lr="{:g}" delay="{}" steps="{}"'.format(
+            self.lr_scheduler.__class__.__name__,
+            self.lr_scheduler.optimizer.param_groups[0]['lr'],
+            self.delay,
+            self.nb_steps)
+        for key in dir(self.lr_scheduler):
+            val = getattr(self.lr_scheduler, key)
+            if (not key.startswith('__')) and isinstance(val, (str, float, int)):
+                res += ' {}="{}"'.format(key, val)
+        res += '/>'
+        return res
 
 
 class Trainer(object):
     """
     Trainer
 
     Settings
@@ -179,16 +205,16 @@
     checks_per_epoch
     """
     def __init__(self, settings, model, dataset, num_instances):
         self.target_task = get_target_task(settings)
         self.verbose = settings.verbose
         self.dataset = dataset
         self.model = model
-        self.optimizer = getattr(optim, settings.optimizer)(
-            model.parameters(), lr=settings.lr)
+        self.optimizer = self.get_optimizer(settings.optimizer)(
+            model.parameters(), lr=settings.lr, **settings.optimizer_params)
         self.clip_norm = settings.clip_norm
 
         self.report_freq = settings.report_freq
         self.num_batches = num_instances // dataset.batch_size
         if settings.checks_per_epoch == 1:
             self.check_freq = self.num_batches - 1  # check after last batch
         elif settings.checks_per_epoch > self.num_batches:
@@ -196,16 +222,25 @@
         elif settings.checks_per_epoch > 1:
             self.check_freq = self.num_batches // settings.checks_per_epoch  # check just
         else:
             self.check_freq = 0  # no checks
 
         self.task_scheduler = TaskScheduler(settings)
         self.lr_scheduler = LRScheduler(
-            self.optimizer, factor=settings.lr_factor,
-            patience=settings.lr_patience, min_lr=settings.min_lr)
+            self.optimizer,
+            lr_scheduler=settings.lr_scheduler,
+            delay=settings.lr_scheduler_delay,
+            **settings.lr_scheduler_params)
+
+        self.noise_strategies = settings.noise_strategies or {}
+        self.noise_strategies = {
+            strategy_name: strategy
+            for strategy_name, strategy in self.noise_strategies.items()
+            if isinstance(strategy, dict) and strategy.get("apply") is True
+        }
 
         if settings.verbose:
             print()
             print("Evaluation check every {}/{} batches".format(
                 self.check_freq, self.num_batches))
             print()
             print("::: Task schedules :::")
@@ -213,14 +248,28 @@
             print(self.task_scheduler)
             print()
             print("::: LR schedule :::")
             print()
             print(self.lr_scheduler)
             print()
 
+    @staticmethod
+    def get_optimizer(optimizer_name: str) -> ClassVar[Optimizer]:
+        """ Allows for getting new optimizers from the torch-optimizer library without
+        breaking previous behaviour
+        :param optimizer_name: Optimizer Name, eg. Adam, SGD, Ranger
+        :return: Optimizer class
+        """
+        if hasattr(optim, optimizer_name):
+            return getattr(optim, optimizer_name)
+        elif hasattr(ext_optims, optimizer_name):
+            return getattr(ext_optims, optimizer_name)
+        else:
+            raise ValueError("Unknown optimizer %s " % optimizer_name)
+
     def weight_loss(self, loss):
         """
         Apply weights to losses and return a single loss number
         """
         weights = self.task_scheduler.get_weights()
 
         return sum(weights.get(k, 1) * loss[k] for k in loss)
@@ -267,15 +316,18 @@
             for task_name, scorer in summary.items():
                 stored_scores[task_name] = scorer.get_scores()
                 scorer.print_summary(scores=stored_scores[task_name])
 
         self.model.train()
         dev_scores = {}
         for task, scored in stored_scores.items():
-            dev_scores[task] = scored['all']['accuracy']
+            dev_scores[task] = scored['all'][
+                self.task_scheduler.tasks[task].get("evaluation", "accuracy")
+            ]
+
         # add lm scores
         if 'lm_fwd' in dev_loss or 'lm_bwd' in dev_loss:
             dev_scores['lm_fwd'] = dev_loss['lm_fwd']
             dev_scores['lm_bwd'] = dev_loss['lm_bwd']
 
         self.task_scheduler.step(dev_scores, self.model)
         self.lr_scheduler.step(dev_scores[self.target_task])
@@ -290,15 +342,15 @@
 
     def train_epoch(self, devset, epoch):
         rep_loss = collections.defaultdict(float)
         rep_batches = collections.defaultdict(int)
         rep_items, rep_start = 0, time.time()
         scores = None
 
-        for b, batch in enumerate(self.dataset.batch_generator()):
+        for b, batch in enumerate(self.dataset.batch_generator(apply_noise=self.noise_strategies)):
             # get loss
             loss = self.model.loss(batch, get_batch_task(self.model.tasks.values()))
 
             if not loss:
                 raise ValueError("Got empty loss, no tasks defined?")
 
             # optimize
```

### Comparing `PaPie-0.3.9/pie/utils.py` & `PaPie-0.4.0/pie/utils.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/pie/webapp/__init__.py` & `PaPie-0.4.0/pie/webapp/__init__.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/setup.py` & `PaPie-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Package meta-data.
 NAME = 'PaPie'
 DESCRIPTION = 'A Framework for Joint Learning of Sequence Labeling Tasks, forked from Pie'
 URL = 'https://github.com/lascivaroma/PaPie'
 AUTHOR = 'Enrique Manjavacas; Mike Kestemont; Thibault Clerice'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = "0.3.9"
+VERSION = "0.4.0"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

### Comparing `PaPie-0.3.9/test/data/test_data.py` & `PaPie-0.4.0/test/data/test_data.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.3.9/test/data/test_tabreader.py` & `PaPie-0.4.0/test/data/test_tabreader.py`

 * *Files identical despite different names*


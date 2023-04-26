# Comparing `tmp/beginai-1.5.3.tar.gz` & `tmp/beginai-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beginai-1.5.3.tar", last modified: Fri Jan 20 20:03:16 2023, max compression
+gzip compressed data, was "beginai-2.0.0.tar", last modified: Wed Apr 26 22:08:40 2023, max compression
```

## Comparing `beginai-1.5.3.tar` & `beginai-2.0.0.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.697243 beginai-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-20 20:03:16.697243 beginai-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-20 20:03:07.000000 beginai-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.693243 beginai-1.5.3/beginai/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.693243 beginai-1.5.3/beginai/conn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/conn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/conn/mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.693243 beginai-1.5.3/beginai/exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.693243 beginai-1.5.3/beginai/exec/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.693243 beginai-1.5.3/beginai/exec/embeddings/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/category.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/date.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.693243 beginai-1.5.3/beginai/exec/embeddings/instructions/deep_text/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/deep_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/deep_text/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/parse_and_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/instructions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/master.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/embeddings/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/execute_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/exec/remote_compute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.693243 beginai-1.5.3/beginai/orchapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/orchapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/orchapi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.697243 beginai-1.5.3/beginai/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/storage/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/storage/sqllite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.697243 beginai-1.5.3/beginai/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.697243 beginai-1.5.3/beginai/tests/exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.697243 beginai-1.5.3/beginai/tests/exec/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.697243 beginai-1.5.3/beginai/tests/exec/embeddings/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/instructions/boolean_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/instructions/category_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/instructions/date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/instructions/interaction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/instructions/location_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/instructions/number_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/instructions/parse_and_execute_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/instructions/text_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/mock_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/tests/exec/embeddings/worker_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.697243 beginai-1.5.3/beginai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-01-20 20:03:07.000000 beginai-1.5.3/beginai/utils/syft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:03:16.693243 beginai-1.5.3/beginai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-20 20:03:16.000000 beginai-1.5.3/beginai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-01-20 20:03:16.000000 beginai-1.5.3/beginai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 20:03:16.000000 beginai-1.5.3/beginai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-20 20:03:16.000000 beginai-1.5.3/beginai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-20 20:03:16.000000 beginai-1.5.3/beginai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-20 20:03:16.697243 beginai-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-01-20 20:03:16.000000 beginai-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 22:08:40.980579 beginai-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-26 22:08:28.000000 beginai-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.976579 beginai-2.0.0/beginai/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.976579 beginai-2.0.0/beginai/conn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/conn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/conn/mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.976579 beginai-2.0.0/beginai/exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.976579 beginai-2.0.0/beginai/exec/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17506 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/exec/embeddings/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/date.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/exec/embeddings/instructions/deep_text/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/deep_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/deep_text/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/parse_and_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/instructions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/embeddings/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/execute_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/exec/remote_compute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/orchapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/orchapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/orchapi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/storage/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/storage/sqllite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/tests/exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/tests/exec/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/boolean_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/interaction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/location_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/parse_and_execute_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/instructions/text_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/mock_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/tests/exec/embeddings/worker_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.980579 beginai-2.0.0/beginai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-26 22:08:28.000000 beginai-2.0.0/beginai/utils/syft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:08:40.976579 beginai-2.0.0/beginai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 22:08:40.000000 beginai-2.0.0/beginai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-26 22:08:40.000000 beginai-2.0.0/beginai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:08:40.000000 beginai-2.0.0/beginai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 22:08:40.000000 beginai-2.0.0/beginai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 22:08:40.000000 beginai-2.0.0/beginai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 22:08:40.980579 beginai-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-26 22:08:39.000000 beginai-2.0.0/setup.py
```

### Comparing `beginai-1.5.3/PKG-INFO` & `beginai-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beginai
-Version: 1.5.3
+Version: 2.0.0
 Summary: A library to interact with Begin AI platform in order to build personalisation algorithms.
 Home-page: https://docs.begin.ai
 Author: Begin AI Research & Engineering
 Author-email: engineering@begin.ai
 License: Proprietary
 Description: 
                 This is Begin AI python SDK for both batch processing and application integration.
```

### Comparing `beginai-1.5.3/beginai/conn/mqtt.py` & `beginai-2.0.0/beginai/conn/mqtt.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/embeddings/apply.py` & `beginai-2.0.0/beginai/exec/embeddings/apply.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 import pandas as pd
 import datetime
 from beginai.exec.embeddings.instructions.utils import sort_instructions
 
 
 class AlgorithmsApplier(object):
 
-    host = "https://sdk.begin.ai"
+    host = "https://sdk-a1ummign.uc.gateway.dev"
 
     INTERACTIONS = 'interactions'
     CREATED_AT = 'beginai_created_at'
+    INTERVENTION_TIMESTAMP = 'intervention_timestamp'
     LABELS = 'labels'
     BATCH_SIZE = 20000
 
     def __init__(self, app_id, license_key, host=None):
         self.orchapi = OrchAPI()
         self.orchapi.configure_orch_connection(host or self.host)
         self.orchapi.set_app_id_and_license_key(
@@ -94,15 +95,15 @@
         print("Start time: ", datetime.datetime.now())
 
         instructions_id, current_embeddings_version, instructions = \
             self._get_instructions()
 
         self._generate_signatures(instructions)
 
-        self._submit(instructions_id, current_embeddings_version, update)
+        self._submit_embeddings(instructions_id, current_embeddings_version, update)
 
         print("End time: ", datetime.datetime.now())
         self.flush_memory()
 
     def flush_memory(self):
         self.embeddings = {}
         self.files = {}
@@ -230,16 +231,36 @@
                 user_interactions[uuid][target_object_name][target_uuid] = []
 
             for action_value in group.apply(lambda row: [{'value': row[interaction_column], 'created_at': row[self.CREATED_AT]}], axis=1):
                 user_interactions[uuid][target_object_name][target_uuid].append(
                     action_value[0])
 
         return user_interactions
+    
+    def _submit_intervention_dates(self, data, object_name):
+        if self._submission_in_progress:
+            return
+        
+        self._submission_in_progress = True
 
-    def _submit(self, instructions_id, current_version, update):
+        end_counter = self.BATCH_SIZE
+        start_counter = 0
+        all_ = len(data)
+
+        while(start_counter < all_):
+            slice = data[start_counter:end_counter]
+            self.orchapi.submit_intervention_dates_batch(slice, object_name)
+            print(
+                f"Submitted {len(slice)} at index {start_counter} out of {all_} interventions for object {object_name}")
+            start_counter += self.BATCH_SIZE
+            end_counter += self.BATCH_SIZE
+
+        self._submission_in_progress = False
+
+    def _submit_embeddings(self, instructions_id, current_version, update):
         if self._submission_in_progress or len(self.embeddings) == 0:
             return
 
         print("Working on submitting existing set. please wait.")
 
         self._submission_in_progress = True
 
@@ -320,14 +341,37 @@
 
     def classify(self, project_id, target_id):
         return self.orchapi.classify(project_id, target_id)
 
     def get_training_performance(self, project_id):
         return self.orchapi.training_results(project_id)
 
+    def record_intervention_dates(self, filename, object_name, unique_identifier_column, intervention_date, file_separator = ','):
+        if object_name == '' or object_name is None:
+            raise ValueError('The object name must be provided')
+
+        if unique_identifier_column == '' or unique_identifier_column is None:
+            raise ValueError('The unique indentifier column must be provided')
+
+        if intervention_date == '' or intervention_date is None:
+            raise ValueError('The intervention date must be provided')
+
+        if filename == '' or filename is None:
+            raise ValueError('The filename must be provided')
+
+        df = self._read_file(filename=filename, file_separator=file_separator)
+        df = df.rename(columns= {unique_identifier_column: 'internal_id', intervention_date: self.INTERVENTION_TIMESTAMP})
+
+        df[self.INTERVENTION_TIMESTAMP] = pd.to_datetime(df[self.INTERVENTION_TIMESTAMP], format="%d-%m-%Y")
+        df[self.INTERVENTION_TIMESTAMP] = df[self.INTERVENTION_TIMESTAMP].apply(lambda x:  x.timestamp())
+
+        dictionary = df.to_dict(orient='records')
+        
+        self._submit_intervention_dates(dictionary, object_name)
+
     def engagement_score(self, project_id, target_id, start_date, end_date):
         start_date = parse_date_to_format(start_date)
         end_date = parse_date_to_format(end_date)
 
         return self.orchapi.engagement_score(project_id, target_id, start_date, end_date)
 
     # maintenance end points
```

### Comparing `beginai-1.5.3/beginai/exec/embeddings/instructions/__init__.py` & `beginai-2.0.0/beginai/exec/embeddings/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/embeddings/instructions/date.py` & `beginai-2.0.0/beginai/exec/embeddings/instructions/date.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/embeddings/instructions/deep_text/bpe.py` & `beginai-2.0.0/beginai/exec/embeddings/instructions/deep_text/bpe.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/embeddings/instructions/interaction.py` & `beginai-2.0.0/beginai/exec/embeddings/instructions/interaction.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/embeddings/instructions/location.py` & `beginai-2.0.0/beginai/exec/embeddings/instructions/location.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/embeddings/instructions/number.py` & `beginai-2.0.0/beginai/exec/embeddings/instructions/number.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/embeddings/instructions/parse_and_execute.py` & `beginai-2.0.0/beginai/exec/embeddings/instructions/parse_and_execute.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/embeddings/instructions/text.py` & `beginai-2.0.0/beginai/exec/embeddings/instructions/text.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/embeddings/instructions/utils.py` & `beginai-2.0.0/beginai/exec/embeddings/instructions/utils.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/embeddings/worker.py` & `beginai-2.0.0/beginai/exec/embeddings/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ...orchapi.api import OrchAPI
 from . import ParseAndExecute
 import datetime
 
 
 class BeginWorker(object):
 
-    host = "https://sdk.begin.ai"
+    host = "https://sdk-a1ummign.uc.gateway.dev"
 
     def __init__(self, app_id, license_key, host=None):
         self.orchapi = OrchAPI()
         self.orchapi.configure_orch_connection(host or self.host)
         self.orchapi.set_app_id_and_license_key(
             app_id=app_id, license_key=license_key)
         self._reset_to_initial_state()
```

### Comparing `beginai-1.5.3/beginai/exec/execute_compute.py` & `beginai-2.0.0/beginai/exec/execute_compute.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/exec/remote_compute.py` & `beginai-2.0.0/beginai/exec/remote_compute.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/instructions/boolean_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/boolean_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/instructions/category_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/category_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/instructions/date_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/date_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/instructions/interaction_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/interaction_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/instructions/location_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/location_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/instructions/number_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/number_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/instructions/parse_and_execute_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/parse_and_execute_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/instructions/text_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/instructions/text_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/mock_service.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/mock_service.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/tests/exec/embeddings/worker_test.py` & `beginai-2.0.0/beginai/tests/exec/embeddings/worker_test.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai/utils/syft.py` & `beginai-2.0.0/beginai/utils/syft.py`

 * *Files identical despite different names*

### Comparing `beginai-1.5.3/beginai.egg-info/PKG-INFO` & `beginai-2.0.0/beginai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beginai
-Version: 1.5.3
+Version: 2.0.0
 Summary: A library to interact with Begin AI platform in order to build personalisation algorithms.
 Home-page: https://docs.begin.ai
 Author: Begin AI Research & Engineering
 Author-email: engineering@begin.ai
 License: Proprietary
 Description: 
                 This is Begin AI python SDK for both batch processing and application integration.
```

### Comparing `beginai-1.5.3/beginai.egg-info/SOURCES.txt` & `beginai-2.0.0/beginai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 beginai/conn/mqtt.py
 beginai/exec/__init__.py
 beginai/exec/execute_compute.py
 beginai/exec/remote_compute.py
 beginai/exec/embeddings/__init__.py
 beginai/exec/embeddings/apply.py
 beginai/exec/embeddings/master.py
-beginai/exec/embeddings/schema.py
 beginai/exec/embeddings/worker.py
 beginai/exec/embeddings/instructions/__init__.py
 beginai/exec/embeddings/instructions/boolean.py
 beginai/exec/embeddings/instructions/category.py
 beginai/exec/embeddings/instructions/date.py
 beginai/exec/embeddings/instructions/interaction.py
 beginai/exec/embeddings/instructions/location.py
```

### Comparing `beginai-1.5.3/setup.py` & `beginai-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 REQ_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "pip-dep")
 core_reqs, core_dependency_links = get_requirements(os.path.join(REQ_DIR, "requirements.txt"))
 
 
 if __name__ == "__main__":
     setup(
         name="beginai",
-        version="1.5.3",
+        version="2.0.0",
         author="Begin AI Research & Engineering",
         author_email="engineering@begin.ai",
         description="A library to interact with Begin AI platform in order to build personalisation algorithms.",
         long_description="""
         This is Begin AI python SDK for both batch processing and application integration. 
         It can be used to integrate applications with Begin.ai orchestration platform to deliver applications with
         personalisation algorithms to do:
```


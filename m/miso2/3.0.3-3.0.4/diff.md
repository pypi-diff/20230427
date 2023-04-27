# Comparing `tmp/miso2-3.0.3.tar.gz` & `tmp/miso2-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miso2-3.0.3.tar", last modified: Tue Apr 25 12:01:58 2023, max compression
+gzip compressed data, was "miso2-3.0.4.tar", last modified: Thu Apr 27 14:14:00 2023, max compression
```

## Comparing `miso2-3.0.3.tar` & `miso2-3.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.271395 miso2-3.0.3/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1054 2023-04-25 06:11:49.000000 miso2-3.0.3/LICENCE.txt
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      817 2023-04-25 12:01:58.271395 miso2-3.0.3/PKG-INFO
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      191 2023-04-25 06:11:49.000000 miso2-3.0.3/README.md
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.263395 miso2-3.0.3/miso/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2205 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/__main__.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.267395 miso2-3.0.3/miso/data/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2760 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/dataset.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1567 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/download.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     7328 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/filenames_dataset.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     3133 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/image_dataset.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2574 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/image_loader.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     3963 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/image_utils.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     7948 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/tf_generator.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5338 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/training_dataset.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     3473 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/utils.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.267395 miso2-3.0.3/miso/deploy/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/deploy/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5839 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/deploy/inference.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     6140 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/deploy/model_info.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     8173 2023-04-25 11:03:22.000000 miso2-3.0.3/miso/deploy/saving.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5139 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/deploy/server.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.267395 miso2-3.0.3/miso/layers/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     4315 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/_common_blocks.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2072 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/asoftmax.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2841 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/batch_instance_normalisation.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     3251 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/cyclic.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     7993 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/group_normalisation.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2479 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/msoftmax.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.267395 miso2-3.0.3/miso/models/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     4475 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/base_cyclic.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5671 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/factory.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)       50 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/model_zoo.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)    12979 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/resnet_cyclic.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     4772 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/transfer_learning.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.267395 miso2-3.0.3/miso/stats/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1452 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/accuracy.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)    13669 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/confusion_matrix.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     6150 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/embedding.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     4861 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/mislabelling.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      882 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/most_representative.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1454 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/projections.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      957 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/training.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.271395 miso2-3.0.3/miso/training/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/training/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     4918 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/training/adaptive_learning_rate.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     3154 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/training/parameters.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5238 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/training/tf_augmentation.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)    24759 2023-04-25 11:59:34.000000 miso2-3.0.3/miso/training/trainer.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1702 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/training/training_result.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.271395 miso2-3.0.3/miso/utils/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     9973 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/flowcam.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      726 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/lock.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      216 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/misc.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1407 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/rolling_buffer.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5155 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/singleton.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     9990 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/wave.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.271395 miso2-3.0.3/miso2.egg-info/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      817 2023-04-25 12:01:58.000000 miso2-3.0.3/miso2.egg-info/PKG-INFO
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1491 2023-04-25 12:01:58.000000 miso2-3.0.3/miso2.egg-info/SOURCES.txt
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        1 2023-04-25 12:01:58.000000 miso2-3.0.3/miso2.egg-info/dependency_links.txt
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      231 2023-04-25 12:01:58.000000 miso2-3.0.3/miso2.egg-info/requires.txt
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        5 2023-04-25 12:01:58.000000 miso2-3.0.3/miso2.egg-info/top_level.txt
--rw-rw-r--   0 chaos     (1000) chaos     (1000)       38 2023-04-25 12:01:58.271395 miso2-3.0.3/setup.cfg
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1794 2023-04-25 12:01:06.000000 miso2-3.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.790503 miso2-3.0.4/
+-rw-rw-rw-   0        0        0     1062 2023-04-17 11:49:46.000000 miso2-3.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0      838 2023-04-27 14:14:00.789497 miso2-3.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-04-17 11:49:46.000000 miso2-3.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.500793 miso2-3.0.4/miso/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/__init__.py
+-rw-rw-rw-   0        0        0     2257 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.577591 miso2-3.0.4/miso/data/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/__init__.py
+-rw-rw-rw-   0        0        0     2829 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/dataset.py
+-rw-rw-rw-   0        0        0     1610 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/download.py
+-rw-rw-rw-   0        0        0     7520 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/filenames_dataset.py
+-rw-rw-rw-   0        0        0     3213 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/image_dataset.py
+-rw-rw-rw-   0        0        0     2651 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/image_loader.py
+-rw-rw-rw-   0        0        0     4074 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/image_utils.py
+-rw-rw-rw-   0        0        0     8146 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/tf_generator.py
+-rw-rw-rw-   0        0        0     5646 2023-04-27 08:34:09.000000 miso2-3.0.4/miso/data/training_dataset.py
+-rw-rw-rw-   0        0        0     3565 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.601790 miso2-3.0.4/miso/deploy/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/deploy/__init__.py
+-rw-rw-rw-   0        0        0     5993 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/deploy/inference.py
+-rw-rw-rw-   0        0        0     6285 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/deploy/model_info.py
+-rw-rw-rw-   0        0        0     8394 2023-04-25 22:30:59.000000 miso2-3.0.4/miso/deploy/saving.py
+-rw-rw-rw-   0        0        0     5275 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/deploy/server.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.642604 miso2-3.0.4/miso/layers/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/__init__.py
+-rw-rw-rw-   0        0        0     4432 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/_common_blocks.py
+-rw-rw-rw-   0        0        0     2127 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/asoftmax.py
+-rw-rw-rw-   0        0        0     2904 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/batch_instance_normalisation.py
+-rw-rw-rw-   0        0        0     3386 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/cyclic.py
+-rw-rw-rw-   0        0        0     8188 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/group_normalisation.py
+-rw-rw-rw-   0        0        0     2546 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/msoftmax.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.676706 miso2-3.0.4/miso/models/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/models/__init__.py
+-rw-rw-rw-   0        0        0     4596 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/models/base_cyclic.py
+-rw-rw-rw-   0        0        0     5798 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/models/factory.py
+-rw-rw-rw-   0        0        0       56 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/models/model_zoo.py
+-rw-rw-rw-   0        0        0    13297 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/models/resnet_cyclic.py
+-rw-rw-rw-   0        0        0     4884 2023-04-27 12:22:14.000000 miso2-3.0.4/miso/models/transfer_learning.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.720827 miso2-3.0.4/miso/stats/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/__init__.py
+-rw-rw-rw-   0        0        0     1490 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/accuracy.py
+-rw-rw-rw-   0        0        0    14013 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/confusion_matrix.py
+-rw-rw-rw-   0        0        0     6294 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/embedding.py
+-rw-rw-rw-   0        0        0     4983 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/mislabelling.py
+-rw-rw-rw-   0        0        0      909 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/most_representative.py
+-rw-rw-rw-   0        0        0     1496 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/projections.py
+-rw-rw-rw-   0        0        0      993 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/training.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.746757 miso2-3.0.4/miso/training/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/training/__init__.py
+-rw-rw-rw-   0        0        0     5042 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/training/adaptive_learning_rate.py
+-rw-rw-rw-   0        0        0     3282 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/training/parameters.py
+-rw-rw-rw-   0        0        0     5374 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/training/tf_augmentation.py
+-rw-rw-rw-   0        0        0    25756 2023-04-27 10:48:06.000000 miso2-3.0.4/miso/training/trainer.py
+-rw-rw-rw-   0        0        0     1757 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/training/training_result.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.788502 miso2-3.0.4/miso/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/__init__.py
+-rw-rw-rw-   0        0        0    10218 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/flowcam.py
+-rw-rw-rw-   0        0        0      757 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/lock.py
+-rw-rw-rw-   0        0        0      227 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/misc.py
+-rw-rw-rw-   0        0        0     1455 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/rolling_buffer.py
+-rw-rw-rw-   0        0        0     5300 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/singleton.py
+-rw-rw-rw-   0        0        0    10056 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/wave.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.517763 miso2-3.0.4/miso2.egg-info/
+-rw-rw-rw-   0        0        0      838 2023-04-27 14:14:00.000000 miso2-3.0.4/miso2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2023-04-27 14:14:00.000000 miso2-3.0.4/miso2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 14:14:00.000000 miso2-3.0.4/miso2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      231 2023-04-27 14:14:00.000000 miso2-3.0.4/miso2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 14:14:00.000000 miso2-3.0.4/miso2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 14:14:00.790503 miso2-3.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2023-04-27 14:13:46.000000 miso2-3.0.4/setup.py
```

### Comparing `miso2-3.0.3/LICENCE.txt` & `miso2-3.0.4/LICENCE.txt`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2020 Ross Marchant
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
+Copyright 2020 Ross Marchant
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
```

### Comparing `miso2-3.0.3/PKG-INFO` & `miso2-3.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1
-Name: miso2
-Version: 3.0.3
-Summary: Python scripts for training CNNs for particle classification
-Home-page: https://github.com/microfossil/particle-classification
-Author: Ross Marchant
-Author-email: ross.g.marchant@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/microfossil/particle-classification
-Project-URL: Paper, https://jm.copernicus.org/articles/39/183/2020/
-Keywords: microfossil,cnn
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
-# particle-classification
-Python scripts for particle classification
-
-https://stackoverflow.com/questions/53779509/upload-failed-403-invalid-or-non-existent-authentication-information-python
+Metadata-Version: 2.1
+Name: miso2
+Version: 3.0.4
+Summary: Python scripts for training CNNs for particle classification
+Home-page: https://github.com/microfossil/particle-classification
+Author: Ross Marchant
+Author-email: ross.g.marchant@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/microfossil/particle-classification
+Project-URL: Paper, https://jm.copernicus.org/articles/39/183/2020/
+Keywords: microfossil,cnn
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
+# particle-classification
+Python scripts for particle classification
+
+https://stackoverflow.com/questions/53779509/upload-failed-403-invalid-or-non-existent-authentication-information-python
```

### Comparing `miso2-3.0.3/miso/__main__.py` & `miso2-3.0.4/miso/__main__.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import argparse
-from miso.training.trainer import train_image_classification_model
-from miso.training.parameters import MisoParameters
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="Train a CNN to classify images")
-    parser.add_argument("-i", "--input", required=True, help="Directory of images, URL link to zipped directory of images, or ParticleTrieur project file")
-    parser.add_argument("-o", "--output", required=True, help="Output directory to store training results")
-    parser.add_argument("-t", "--type", required=True, help="Type of CNN: resnet_tl, resnet_cyclic_tl, base_cyclic, resnet_cyclic, resnet18, resnet50, vgg16, vgg19")
-
-    parser.add_argument("-f", "--filters", type=int, default=4, help="Number of filters in the first convolutional block")
-
-    parser.add_argument("--min_count", type=int, default=10, help="Minimum number of images in a class for it to be included")
-    parser.add_argument("--map_others", action='store_true', help="Classes with not enough images will be put into 'others' class (so long as the total is also greater than min_count")
-    args = parser.parse_args()
-
-    tp = MisoParameters()
-    tp.source = args.input
-    tp.output_dir = args.output
-    tp.cnn_type = args.type
-    tp.filters = args.filters
-    tp.min_count = args.min_count
-    tp.map_others = args.map_others
-
-    train_image_classification_model(tp)
-    # print("This is the name of the script: ", sys.argv[0])
-    # print("Number of arguments: ", len(sys.argv))
-    # print("The arguments are: ", str(sys.argv))
-    #
-    # params = default_params()
-    # print(params)
-    # key = None
-    # for arg in sys.argv[1:]:
-    #     print(arg)
-    #     if arg.startswith('--'):
-    #         key = arg[2:]
-    #         print(key)
-    #     else:
-    #         try:
-    #             val = int(arg)
-    #             print("int")
-    #         except ValueError:
-    #             try:
-    #                 val = float(arg)
-    #                 print("float")
-    #             except:
-    #                 val = arg
-    #                 print("string")
-    #         params[key] = val
-    # print(params)
-    # train_image_classification_model(params)
-
+import argparse
+from miso.training.trainer import train_image_classification_model
+from miso.training.parameters import MisoParameters
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="Train a CNN to classify images")
+    parser.add_argument("-i", "--input", required=True, help="Directory of images, URL link to zipped directory of images, or ParticleTrieur project file")
+    parser.add_argument("-o", "--output", required=True, help="Output directory to store training results")
+    parser.add_argument("-t", "--type", required=True, help="Type of CNN: resnet_tl, resnet_cyclic_tl, base_cyclic, resnet_cyclic, resnet18, resnet50, vgg16, vgg19")
+
+    parser.add_argument("-f", "--filters", type=int, default=4, help="Number of filters in the first convolutional block")
+
+    parser.add_argument("--min_count", type=int, default=10, help="Minimum number of images in a class for it to be included")
+    parser.add_argument("--map_others", action='store_true', help="Classes with not enough images will be put into 'others' class (so long as the total is also greater than min_count")
+    args = parser.parse_args()
+
+    tp = MisoParameters()
+    tp.source = args.input
+    tp.output_dir = args.output
+    tp.cnn_type = args.type
+    tp.filters = args.filters
+    tp.min_count = args.min_count
+    tp.map_others = args.map_others
+
+    train_image_classification_model(tp)
+    # print("This is the name of the script: ", sys.argv[0])
+    # print("Number of arguments: ", len(sys.argv))
+    # print("The arguments are: ", str(sys.argv))
+    #
+    # params = default_params()
+    # print(params)
+    # key = None
+    # for arg in sys.argv[1:]:
+    #     print(arg)
+    #     if arg.startswith('--'):
+    #         key = arg[2:]
+    #         print(key)
+    #     else:
+    #         try:
+    #             val = int(arg)
+    #             print("int")
+    #         except ValueError:
+    #             try:
+    #                 val = float(arg)
+    #                 print("float")
+    #             except:
+    #                 val = arg
+    #                 print("string")
+    #         params[key] = val
+    # print(params)
+    # train_image_classification_model(params)
+
```

### Comparing `miso2-3.0.3/miso/data/dataset.py` & `miso2-3.0.4/miso/data/dataset.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import hashlib
-import os
-import numpy as np
-from numpy.lib.format import open_memmap
-import gc
-
-
-class DatasetBase:
-    def __init__(self, memmap_directory=None, overwrite_memmap=False, dtype=np.uint8):
-        self.memmap_directory = memmap_directory
-        self.overwrite_memmap = overwrite_memmap
-        self.memmap_file = None
-        self.hash_data = None
-        self.data = None
-        self.shape = None
-        self.dtype = dtype
-
-    def read_or_create_data(self, shape, dtype):
-        self.shape = shape
-        self.dtype = dtype
-
-        if isinstance(shape, list):
-            raise ValueError("Shape must be a tuple, e.g. (100,32,32,3) not a list, e.g. [100,32,32,3]")
-
-        if self.memmap_directory:
-            if self.hash_data is None:
-                raise ValueError("Please set the hash_data (as a numpy array) to use memory mapping")
-            self.memmap_file = os.path.join(self.memmap_directory, self.get_hash_id() + ".npy")
-            if self.overwrite_memmap is False and os.path.exists(self.memmap_file):
-                print("Existing data found at {}".format(self.memmap_file))
-                self.data = open_memmap(self.memmap_file, mode='r+', dtype=self.dtype, shape=self.shape)
-                # Check if not all zeros
-                # If all zeros, usually indication of an error creating the memmap file previously, therefore recreate
-                if np.count_nonzero(self.data[0]) > 0 and np.count_nonzero(self.data[-1]) > 0:
-                    return True
-                else:
-                    self.data._mmap.close()
-                    print("File was likely corrupted, recreating.")
-            print("Creating memmap file at {}".format(self.memmap_file))
-            os.makedirs(self.memmap_directory, exist_ok=True)
-            self.data = open_memmap(self.memmap_file, mode='w+', dtype=self.dtype, shape=self.shape)
-        else:
-            self.data = np.zeros(self.shape, dtype=self.dtype)
-
-        return False
-
-    def get_hash_id(self):
-        """
-        Creates a 16 character hash id based on the hash data. This is used to create a unique
-        filename for the numpy memmap array
-        :return: 16 character hash id
-        """
-        if self.hash_data is None:
-            raise ValueError("Please set the hash_data before getting the hash")
-        else:
-            return hashlib.sha256(repr(self.hash_data).encode('UTF-8')).hexdigest()[0:16]
-
-    def release(self):
-        if self.memmap_file is None:
-            del self.data
-        else:
-            if os.path.exists(self.memmap_file):
-                self.data._mmap.close()
-                del self.data
-                gc.collect()
-                os.remove(self.memmap_file)
-            self.memmap_file = None
-
-
+import hashlib
+import os
+import numpy as np
+from numpy.lib.format import open_memmap
+import gc
+
+
+class DatasetBase:
+    def __init__(self, memmap_directory=None, overwrite_memmap=False, dtype=np.uint8):
+        self.memmap_directory = memmap_directory
+        self.overwrite_memmap = overwrite_memmap
+        self.memmap_file = None
+        self.hash_data = None
+        self.data = None
+        self.shape = None
+        self.dtype = dtype
+
+    def read_or_create_data(self, shape, dtype):
+        self.shape = shape
+        self.dtype = dtype
+
+        if isinstance(shape, list):
+            raise ValueError("Shape must be a tuple, e.g. (100,32,32,3) not a list, e.g. [100,32,32,3]")
+
+        if self.memmap_directory:
+            if self.hash_data is None:
+                raise ValueError("Please set the hash_data (as a numpy array) to use memory mapping")
+            self.memmap_file = os.path.join(self.memmap_directory, self.get_hash_id() + ".npy")
+            if self.overwrite_memmap is False and os.path.exists(self.memmap_file):
+                print("Existing data found at {}".format(self.memmap_file))
+                self.data = open_memmap(self.memmap_file, mode='r+', dtype=self.dtype, shape=self.shape)
+                # Check if not all zeros
+                # If all zeros, usually indication of an error creating the memmap file previously, therefore recreate
+                if np.count_nonzero(self.data[0]) > 0 and np.count_nonzero(self.data[-1]) > 0:
+                    return True
+                else:
+                    self.data._mmap.close()
+                    print("File was likely corrupted, recreating.")
+            print("Creating memmap file at {}".format(self.memmap_file))
+            os.makedirs(self.memmap_directory, exist_ok=True)
+            self.data = open_memmap(self.memmap_file, mode='w+', dtype=self.dtype, shape=self.shape)
+        else:
+            self.data = np.zeros(self.shape, dtype=self.dtype)
+
+        return False
+
+    def get_hash_id(self):
+        """
+        Creates a 16 character hash id based on the hash data. This is used to create a unique
+        filename for the numpy memmap array
+        :return: 16 character hash id
+        """
+        if self.hash_data is None:
+            raise ValueError("Please set the hash_data before getting the hash")
+        else:
+            return hashlib.sha256(repr(self.hash_data).encode('UTF-8')).hexdigest()[0:16]
+
+    def release(self):
+        if self.memmap_file is None:
+            del self.data
+        else:
+            if os.path.exists(self.memmap_file):
+                self.data._mmap.close()
+                del self.data
+                gc.collect()
+                os.remove(self.memmap_file)
+            self.memmap_file = None
+
+
```

### Comparing `miso2-3.0.3/miso/data/download.py` & `miso2-3.0.4/miso/data/download.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import tensorflow as tf
-import os
-from zipfile import ZipFile
-import hashlib
-
-
-def download_images(origin, directory):
-    # Fix URLs
-    # - OneDrive
-    if origin.startswith("https://1drv.ms/"):
-        origin = origin.replace("https://1drv.ms/", "https://1drv.ws/")
-
-    hash = hashlib.md5(origin.encode()).hexdigest()[:10]
-    directory = os.path.join(directory, hash)
-    zip_path = os.path.join(directory, "download.zip")
-    if os.path.exists(directory) is False or os.path.exists(zip_path) is True:
-        os.makedirs(directory, exist_ok=True)
-        outp = tf.keras.utils.get_file(
-            "download.zip",
-            origin,
-            untar=False,
-            md5_hash=None,
-            file_hash=None,
-            cache_subdir=directory,
-            hash_algorithm='auto',
-            extract=True,
-            archive_format='auto',
-            cache_dir=None)
-        print(outp)
-        # Create a ZipFile Object and load sample.zip in it
-        with ZipFile(zip_path, 'r') as zip_obj:
-            # Get list of files names in zip
-            paths = [path for path in zip_obj.namelist() if not path.startswith("_")]
-            dir_name = paths[0].replace(',', '/').replace(',', '\\')
-            folder_path = os.path.join(directory, dir_name)
-        os.remove(os.path.join(directory, "download.zip"))
-    else:
-        paths = [path for path in os.listdir(directory) if not path.startswith("_")]
-        folder_path = os.path.join(directory, paths[0])
-        print("Already downloaded at: {}".format(folder_path))
-    return folder_path
-
-
+import tensorflow as tf
+import os
+from zipfile import ZipFile
+import hashlib
+
+
+def download_images(origin, directory):
+    # Fix URLs
+    # - OneDrive
+    if origin.startswith("https://1drv.ms/"):
+        origin = origin.replace("https://1drv.ms/", "https://1drv.ws/")
+
+    hash = hashlib.md5(origin.encode()).hexdigest()[:10]
+    directory = os.path.join(directory, hash)
+    zip_path = os.path.join(directory, "download.zip")
+    if os.path.exists(directory) is False or os.path.exists(zip_path) is True:
+        os.makedirs(directory, exist_ok=True)
+        outp = tf.keras.utils.get_file(
+            "download.zip",
+            origin,
+            untar=False,
+            md5_hash=None,
+            file_hash=None,
+            cache_subdir=directory,
+            hash_algorithm='auto',
+            extract=True,
+            archive_format='auto',
+            cache_dir=None)
+        print(outp)
+        # Create a ZipFile Object and load sample.zip in it
+        with ZipFile(zip_path, 'r') as zip_obj:
+            # Get list of files names in zip
+            paths = [path for path in zip_obj.namelist() if not path.startswith("_")]
+            dir_name = paths[0].replace(',', '/').replace(',', '\\')
+            folder_path = os.path.join(directory, dir_name)
+        os.remove(os.path.join(directory, "download.zip"))
+    else:
+        paths = [path for path in os.listdir(directory) if not path.startswith("_")]
+        folder_path = os.path.join(directory, paths[0])
+        print("Already downloaded at: {}".format(folder_path))
+    return folder_path
+
+
```

### Comparing `miso2-3.0.3/miso/data/filenames_dataset.py` & `miso2-3.0.4/miso/data/filenames_dataset.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-from typing import NamedTuple
-
-import numpy as np
-from glob import glob
-import os
-from collections import OrderedDict
-import platform
-import pandas as pd
-import xml.etree.ElementTree as ET
-
-from miso.data.download import download_images
-
-from pathlib import Path
-
-
-
-def ls(source_dir):
-    return sorted(glob(os.path.join(source_dir, "*")))
-
-
-def parse_directory(source_dir, skip='~', has_classes=True):
-    """
-    Parses a directory consisting of subdirectories named by class and stores the image filenames in a dictionary
-    :param source_dir: The directory to parse
-    :param verbose: Print out the progress
-    :param skip: If a subdirectory starts with this character it will be skipped ('_' and '.' are skipped always)
-    :param has_classes: The files are arranged in subdirectories by class name
-    :return: Dictionary with class names for the keys and lists of filenames for the values
-    """
-    if has_classes:
-        sub_dirs = sorted(glob(os.path.join(source_dir, "*")))
-    else:
-        sub_dirs = [source_dir]
-    filenames = OrderedDict()
-    for sub_dir in sub_dirs:
-        if os.path.isdir(sub_dir) is False:
-            continue
-        # Get the directory name
-        sub_name = os.path.basename(sub_dir)
-        # Skip directories starting with ~
-        if sub_name.startswith(skip) or \
-            sub_name.startswith('_') or \
-            sub_name.startswith('.'):
-            continue
-        files = []
-        for ext in ["*.jpg", "*.jpeg", "*.png", "*.tif", "*.tiff", "*.bmp"]:
-            sub_files1 = sorted(glob(os.path.join(sub_dir, ext)))
-            files.extend(sub_files1)
-            if platform.system() == 'Linux':
-                sub_files2 = sorted(glob(os.path.join(sub_dir, ext.upper())))
-                files.extend(sub_files2)
-        # Add to dictionary
-        if has_classes:
-            filenames[sub_name] = files
-        else:
-            filenames['null'] = files
-    return filenames
-
-
-def parse_csv(csv_file, source_dir, file_idx=0, cls_idx=1, cls_label_idx=2, verbose=True):
-    if verbose:
-        print("Parsing csv file {} for directory {}".format(csv_file, source_dir))
-    df = pd.read_csv(csv_file)
-    num_classes = np.max(df.iloc[:, cls_idx]) + 1
-    cls_labels = [df.loc[df.iloc[:, cls_idx] == i].iloc[0, cls_label_idx] for i in range(num_classes)]
-    filenames = OrderedDict()
-    for i in range(num_classes):
-        if verbose:
-            print("- {}".format(cls_labels[i]), end='')
-        names = df.loc[df.iloc[:, cls_idx] == i].iloc[:, file_idx]
-        paths = [os.path.join(source_dir, n) for n in names]
-        filenames[cls_labels[i]] = paths
-        if verbose:
-            print(" ({} files)".format(len(paths)))
-    return filenames
-
-
-def parse_xml(xml_filename):
-    project = ET.parse(xml_filename).getroot()
-
-    filenames = []
-    cls = []
-    cls_labels = []
-
-    filenames_dict = OrderedDict()
-
-    images_xml = project.find('images')
-    for i, image_xml in enumerate(images_xml.iter('image')):
-        relfile = image_xml.find('source').find('filename').text
-        if os.path.isabs(relfile):
-            absfile = relfile
-        else:
-            absfile = os.path.abspath(os.path.join(os.path.dirname(xml_filename), relfile))
-        if os.path.isfile(absfile) is False:
-            continue
-        filenames.append(absfile)
-
-        cls_names = []
-        cls_scores = []
-        cls_base = image_xml.find('classifications')
-        for cls_val in cls_base.iter('classification'):
-            cls_names.append(cls_val.find('code').text)
-            cls_scores.append(float(cls_val.find('value').text))
-        cls.append(cls_names[np.argmax(cls_scores)])
-
-    for taxon_xml in project.find('taxons').iter('taxon'):
-        if taxon_xml.find('isClass').text == 'true':
-            cls_labels.append(taxon_xml.find('code').text)
-    cls_labels = sorted(cls_labels)
-
-    df = pd.DataFrame({'filenames': filenames, 'cls': cls})
-    for label in cls_labels:
-        filenames_dict[label] = df.filenames[df.cls == label]
-    return filenames_dict
-
-
-class FilenamesDataset(object):
-    def __init__(self,
-                 source: str,
-                 csv_idxs=(0, 1, 2),
-                 has_classes=True):
-        self.source = source
-        self.csv_idxs = csv_idxs
-        self.has_classes = has_classes
-        self.cls_filenames = OrderedDict()
-        self.filenames = None
-        self.cls_labels = None
-        self.cls = None
-        self.cls_counts = None
-        self.num_classes = None
-
-    def load(self, min_count=0, map_others=False):
-        print('-' * 80)
-        print("Parsing source {}".format(self.source))
-        print()
-
-        # Load filenames
-        if self.source.endswith(".xml"):
-            self.cls_filenames = parse_xml(self.source)
-        elif self.source.endswith(".csv"):
-            self.cls_filenames = parse_csv(self.source, self.source, self.csv_idxs[0], self.csv_idxs[1], self.csv_idxs[2])
-        elif self.source.startswith("http"):
-            dir_for_download = os.path.join(str(Path.home()), 'miso_datasets')
-            os.makedirs(dir_for_download, exist_ok=True)
-            dir_path = download_images(self.source, dir_for_download)
-            self.cls_filenames = parse_directory(dir_path, has_classes=self.has_classes)
-        else:
-            self.cls_filenames = parse_directory(self.source, has_classes=self.has_classes)
-
-        # Check we found some images
-        filenames = [v for key, val in self.cls_filenames.items() for v in val]
-        if len(filenames) == 0:
-            raise ValueError("! Did not find any images")
-
-        # Display how many found
-        print("Classes:")
-        for k, v in self.cls_filenames.items():
-            print("- {}: {} images".format(k, len(v)))
-        print()
-
-        # Apply min count
-        if min_count > 0:
-            print("Removing classes with less than {} images:".format(min_count))
-            others = []
-            filtered_cls_filenames = OrderedDict()
-            was_min = False
-            for k, v in self.cls_filenames.items():
-                if len(v) < min_count:
-                    others.extend(v)
-                    print("- {}: {} images".format(k, len(v)))
-                    was_min = True
-                else:
-                    filtered_cls_filenames[k] = v
-            if was_min is False:
-                print("- none found")
-            # Put in others
-            if map_others is True and len(others) > min_count:
-                if 'others' in filtered_cls_filenames:
-                    filtered_cls_filenames['others'].extend(others)
-                else:
-                    filtered_cls_filenames['others'] = others
-                print("- these images have been places in the 'others' class, {} total".format(len(others)))
-            self.cls_filenames = filtered_cls_filenames
-            print()
-
-        # Flatten filename and class dictionary to a list
-        self.filenames = [v for key, val in self.cls_filenames.items() for v in val]
-        self.cls_labels = list(self.cls_filenames.keys())
-        self.cls = np.asarray([self.cls_labels.index(key) for key, val in self.cls_filenames.items() for v in val])
-        self.cls_counts = np.asarray([len(val) for key, val in self.cls_filenames.items()])
-        self.num_classes = len(self.cls_filenames.keys())
-
+from typing import NamedTuple
+
+import numpy as np
+from glob import glob
+import os
+from collections import OrderedDict
+import platform
+import pandas as pd
+import xml.etree.ElementTree as ET
+
+from miso.data.download import download_images
+
+from pathlib import Path
+
+
+
+def ls(source_dir):
+    return sorted(glob(os.path.join(source_dir, "*")))
+
+
+def parse_directory(source_dir, skip='~', has_classes=True):
+    """
+    Parses a directory consisting of subdirectories named by class and stores the image filenames in a dictionary
+    :param source_dir: The directory to parse
+    :param verbose: Print out the progress
+    :param skip: If a subdirectory starts with this character it will be skipped ('_' and '.' are skipped always)
+    :param has_classes: The files are arranged in subdirectories by class name
+    :return: Dictionary with class names for the keys and lists of filenames for the values
+    """
+    if has_classes:
+        sub_dirs = sorted(glob(os.path.join(source_dir, "*")))
+    else:
+        sub_dirs = [source_dir]
+    filenames = OrderedDict()
+    for sub_dir in sub_dirs:
+        if os.path.isdir(sub_dir) is False:
+            continue
+        # Get the directory name
+        sub_name = os.path.basename(sub_dir)
+        # Skip directories starting with ~
+        if sub_name.startswith(skip) or \
+            sub_name.startswith('_') or \
+            sub_name.startswith('.'):
+            continue
+        files = []
+        for ext in ["*.jpg", "*.jpeg", "*.png", "*.tif", "*.tiff", "*.bmp"]:
+            sub_files1 = sorted(glob(os.path.join(sub_dir, ext)))
+            files.extend(sub_files1)
+            if platform.system() == 'Linux':
+                sub_files2 = sorted(glob(os.path.join(sub_dir, ext.upper())))
+                files.extend(sub_files2)
+        # Add to dictionary
+        if has_classes:
+            filenames[sub_name] = files
+        else:
+            filenames['null'] = files
+    return filenames
+
+
+def parse_csv(csv_file, source_dir, file_idx=0, cls_idx=1, cls_label_idx=2, verbose=True):
+    if verbose:
+        print("Parsing csv file {} for directory {}".format(csv_file, source_dir))
+    df = pd.read_csv(csv_file)
+    num_classes = np.max(df.iloc[:, cls_idx]) + 1
+    cls_labels = [df.loc[df.iloc[:, cls_idx] == i].iloc[0, cls_label_idx] for i in range(num_classes)]
+    filenames = OrderedDict()
+    for i in range(num_classes):
+        if verbose:
+            print("- {}".format(cls_labels[i]), end='')
+        names = df.loc[df.iloc[:, cls_idx] == i].iloc[:, file_idx]
+        paths = [os.path.join(source_dir, n) for n in names]
+        filenames[cls_labels[i]] = paths
+        if verbose:
+            print(" ({} files)".format(len(paths)))
+    return filenames
+
+
+def parse_xml(xml_filename):
+    project = ET.parse(xml_filename).getroot()
+
+    filenames = []
+    cls = []
+    cls_labels = []
+
+    filenames_dict = OrderedDict()
+
+    images_xml = project.find('images')
+    for i, image_xml in enumerate(images_xml.iter('image')):
+        relfile = image_xml.find('source').find('filename').text
+        if os.path.isabs(relfile):
+            absfile = relfile
+        else:
+            absfile = os.path.abspath(os.path.join(os.path.dirname(xml_filename), relfile))
+        if os.path.isfile(absfile) is False:
+            continue
+        filenames.append(absfile)
+
+        cls_names = []
+        cls_scores = []
+        cls_base = image_xml.find('classifications')
+        for cls_val in cls_base.iter('classification'):
+            cls_names.append(cls_val.find('code').text)
+            cls_scores.append(float(cls_val.find('value').text))
+        cls.append(cls_names[np.argmax(cls_scores)])
+
+    for taxon_xml in project.find('taxons').iter('taxon'):
+        if taxon_xml.find('isClass').text == 'true':
+            cls_labels.append(taxon_xml.find('code').text)
+    cls_labels = sorted(cls_labels)
+
+    df = pd.DataFrame({'filenames': filenames, 'cls': cls})
+    for label in cls_labels:
+        filenames_dict[label] = df.filenames[df.cls == label]
+    return filenames_dict
+
+
+class FilenamesDataset(object):
+    def __init__(self,
+                 source: str,
+                 csv_idxs=(0, 1, 2),
+                 has_classes=True):
+        self.source = source
+        self.csv_idxs = csv_idxs
+        self.has_classes = has_classes
+        self.cls_filenames = OrderedDict()
+        self.filenames = None
+        self.cls_labels = None
+        self.cls = None
+        self.cls_counts = None
+        self.num_classes = None
+
+    def load(self, min_count=0, map_others=False):
+        print('-' * 80)
+        print("Parsing source {}".format(self.source))
+        print()
+
+        # Load filenames
+        if self.source.endswith(".xml"):
+            self.cls_filenames = parse_xml(self.source)
+        elif self.source.endswith(".csv"):
+            self.cls_filenames = parse_csv(self.source, self.source, self.csv_idxs[0], self.csv_idxs[1], self.csv_idxs[2])
+        elif self.source.startswith("http"):
+            dir_for_download = os.path.join(str(Path.home()), 'miso_datasets')
+            os.makedirs(dir_for_download, exist_ok=True)
+            dir_path = download_images(self.source, dir_for_download)
+            self.cls_filenames = parse_directory(dir_path, has_classes=self.has_classes)
+        else:
+            self.cls_filenames = parse_directory(self.source, has_classes=self.has_classes)
+
+        # Check we found some images
+        filenames = [v for key, val in self.cls_filenames.items() for v in val]
+        if len(filenames) == 0:
+            raise ValueError("! Did not find any images")
+
+        # Display how many found
+        print("Classes:")
+        for k, v in self.cls_filenames.items():
+            print("- {}: {} images".format(k, len(v)))
+        print()
+
+        # Apply min count
+        if min_count > 0:
+            print("Removing classes with less than {} images:".format(min_count))
+            others = []
+            filtered_cls_filenames = OrderedDict()
+            was_min = False
+            for k, v in self.cls_filenames.items():
+                if len(v) < min_count:
+                    others.extend(v)
+                    print("- {}: {} images".format(k, len(v)))
+                    was_min = True
+                else:
+                    filtered_cls_filenames[k] = v
+            if was_min is False:
+                print("- none found")
+            # Put in others
+            if map_others is True and len(others) > min_count:
+                if 'others' in filtered_cls_filenames:
+                    filtered_cls_filenames['others'].extend(others)
+                else:
+                    filtered_cls_filenames['others'] = others
+                print("- these images have been places in the 'others' class, {} total".format(len(others)))
+            self.cls_filenames = filtered_cls_filenames
+            print()
+
+        # Flatten filename and class dictionary to a list
+        self.filenames = [v for key, val in self.cls_filenames.items() for v in val]
+        self.cls_labels = list(self.cls_filenames.keys())
+        self.cls = np.asarray([self.cls_labels.index(key) for key, val in self.cls_filenames.items() for v in val])
+        self.cls_counts = np.asarray([len(val) for key, val in self.cls_filenames.items()])
+        self.num_classes = len(self.cls_filenames.keys())
+
```

### Comparing `miso2-3.0.3/miso/data/image_dataset.py` & `miso2-3.0.4/miso/data/image_dataset.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import numpy as np
-import skimage.io as skio
-
-from miso.data.dataset import DatasetBase
-from miso.data.image_loader import ParallelImageLoader
-from miso.data.image_utils import resize_transform, resize_with_pad_transform, null_transform
-from miso.data.tf_generator import TFGenerator
-
-
-class ImageDataset(DatasetBase):
-    def __init__(self,
-                 filenames,
-                 cls=None,
-                 transform_fn=None,
-                 transform_args=None,
-                 img_size=None,
-                 memmap_directory=None,
-                 overwrite_memmap=False,
-                 unique_id=None,
-                 dtype=np.uint8):
-        self.filenames = filenames
-        self.cls = cls
-        self.transform_fn = transform_fn
-        self.transform_args = transform_args
-        self.unique_id = unique_id
-
-        # Pre-made transforms
-        if self.transform_fn == 'resize':
-            self.transform_fn = resize_transform
-        elif self.transform_fn == 'resize_with_pad':
-            self.transform_fn = resize_with_pad_transform
-
-        if self.transform_fn is None:
-            self.transform_fn = null_transform
-            self.transform_args = [0]
-
-        # Get dataset unique identification hash
-        super().__init__(memmap_directory=memmap_directory, overwrite_memmap=overwrite_memmap, dtype=dtype)
-        self.hash_data = ["ImageDataset", self.filenames, str(self.dtype), self.unique_id]
-
-        print('-' * 80)
-        print("Loading images")
-        print("- id: {}".format(self.get_hash_id()))
-        if memmap_directory is None:
-            print("- stored in RAM")
-        else:
-            print("- stored on disk at {}".format(self.memmap_file))
-
-        if img_size is None:
-            # Read first image to see the size
-            im = skio.imread(self.filenames[0])
-            if self.transform_args is not None:
-                im = self.transform_fn(im, *self.transform_args)
-            else:
-                im = self.transform_fn(im)
-            self.img_size = im.shape
-        else:
-            self.img_size = img_size
-        self.arr_size = (len(self.filenames),) + self.img_size
-        print("Array size is {}".format(self.arr_size))
-
-    def load(self):
-        if self.read_or_create_data(self.arr_size, self.dtype) is not True:
-            loader = ParallelImageLoader(self.filenames,
-                                         self.data,
-                                         transform_fn=self.transform_fn,
-                                         transform_args=self.transform_args)
-            loader.load()
-
-    def create_generator(self, batch_size, idxs=None, map_fn=TFGenerator.map_fn_divide_255, shuffle=True, one_shot=False, undersample=False):
-        # Create generators for training
-        gen = TFGenerator(self.data,
-                          self.cls,
-                          idxs=idxs,
-                          batch_size=batch_size,
-                          map_fn=map_fn,
-                          shuffle=shuffle,
-                          one_shot=one_shot,
-                          undersample=undersample)
-        return gen
+import numpy as np
+import skimage.io as skio
+
+from miso.data.dataset import DatasetBase
+from miso.data.image_loader import ParallelImageLoader
+from miso.data.image_utils import resize_transform, resize_with_pad_transform, null_transform
+from miso.data.tf_generator import TFGenerator
+
+
+class ImageDataset(DatasetBase):
+    def __init__(self,
+                 filenames,
+                 cls=None,
+                 transform_fn=None,
+                 transform_args=None,
+                 img_size=None,
+                 memmap_directory=None,
+                 overwrite_memmap=False,
+                 unique_id=None,
+                 dtype=np.uint8):
+        self.filenames = filenames
+        self.cls = cls
+        self.transform_fn = transform_fn
+        self.transform_args = transform_args
+        self.unique_id = unique_id
+
+        # Pre-made transforms
+        if self.transform_fn == 'resize':
+            self.transform_fn = resize_transform
+        elif self.transform_fn == 'resize_with_pad':
+            self.transform_fn = resize_with_pad_transform
+
+        if self.transform_fn is None:
+            self.transform_fn = null_transform
+            self.transform_args = [0]
+
+        # Get dataset unique identification hash
+        super().__init__(memmap_directory=memmap_directory, overwrite_memmap=overwrite_memmap, dtype=dtype)
+        self.hash_data = ["ImageDataset", self.filenames, str(self.dtype), self.unique_id]
+
+        print('-' * 80)
+        print("Loading images")
+        print("- id: {}".format(self.get_hash_id()))
+        if memmap_directory is None:
+            print("- stored in RAM")
+        else:
+            print("- stored on disk at {}".format(self.memmap_file))
+
+        if img_size is None:
+            # Read first image to see the size
+            im = skio.imread(self.filenames[0])
+            if self.transform_args is not None:
+                im = self.transform_fn(im, *self.transform_args)
+            else:
+                im = self.transform_fn(im)
+            self.img_size = im.shape
+        else:
+            self.img_size = img_size
+        self.arr_size = (len(self.filenames),) + self.img_size
+        print("Array size is {}".format(self.arr_size))
+
+    def load(self):
+        if self.read_or_create_data(self.arr_size, self.dtype) is not True:
+            loader = ParallelImageLoader(self.filenames,
+                                         self.data,
+                                         transform_fn=self.transform_fn,
+                                         transform_args=self.transform_args)
+            loader.load()
+
+    def create_generator(self, batch_size, idxs=None, map_fn=TFGenerator.map_fn_divide_255, shuffle=True, one_shot=False, undersample=False):
+        # Create generators for training
+        gen = TFGenerator(self.data,
+                          self.cls,
+                          idxs=idxs,
+                          batch_size=batch_size,
+                          map_fn=map_fn,
+                          shuffle=shuffle,
+                          one_shot=one_shot,
+                          undersample=undersample)
+        return gen
```

### Comparing `miso2-3.0.3/miso/data/image_utils.py` & `miso2-3.0.4/miso/data/image_utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import numpy as np
-from skimage import io as skio, transform as skt, color as skc
-
-
-def load_image(filename, img_size=None, img_type='rgb'):
-    """
-    Loads an image, converting it if necessary
-    :param filename: Filename of image to load
-    :param img_size: Size of image, e.g. (224, 224). If None, the image dimensions are preserved
-    :param img_type: 'rgb' (colour) or 'k' (greyscale)
-    :return:
-    """
-    # Colour
-    if img_type == 'rgb':
-        im = skio.imread(filename)
-        # im = np.asarray(im, dtype=np.float)
-        # If it was a single channel image, make into 3-channel
-        if im.ndim == 2:
-            im = np.repeat(im[..., np.newaxis], repeats=3, axis=-1)
-    # Greyscale
-    elif img_type == 'k' or img_type == 'greyscale':
-        im = skio.imread(filename, as_gray=True)
-        im = im[..., np.newaxis]
-    else:
-        raise ValueError("img_type must be 'rgb' or 'k'")
-    # Resize and pad
-    if img_size is not None:
-        im = resize_and_pad_image(im, img_size)
-    return im
-
-
-def resize_and_pad_image(im, img_size):
-    # Add last dim if greyscale
-    if np.ndim(im) == 2:
-        im = im[..., np.newaxis]
-    # Get the ratio of width to height for each
-    current_whratio = im.shape[1] / im.shape[0]
-    desired_whratio = img_size[1] / img_size[0]
-    # Check if the image has roughly the same ratio, else pad it
-    if np.round(im.shape[0] * desired_whratio) != im.shape[1]:
-        height = im.shape[0]
-        width = im.shape[1]
-        # Desired shape is wider than current one
-        if desired_whratio > current_whratio:
-            half = np.round(height * desired_whratio)
-            height_pad_start = 0
-            height_pad_end = 0
-            width_pad_start = int(abs(np.floor((width - half) / 2)))
-            width_pad_end = int(abs(np.ceil((width - half) / 2)))
-        # Desired shape is taller than current
-        else:
-            half = np.round(width / desired_whratio)
-            height_pad_start = int(abs(np.floor((height - half) / 2)))
-            height_pad_end = int(abs(np.ceil((height - half) / 2)))
-            width_pad_start = 0
-            width_pad_end = 0
-        # Constant value to pad with
-        consts = [np.median(np.concatenate((im[0, :, i], im[-1, :, i], im[:, 0, i], im[:, -1, i]))) for i in range(im.shape[2])]
-        # Pad
-        im = np.stack(
-            [np.pad(im[:, :, c],
-                    ((height_pad_start, height_pad_end), (width_pad_start, width_pad_end)),
-                    mode='constant',
-                    constant_values=consts[c])
-             for c in range(im.shape[2])], axis=2)
-        # # Revert if was greyscale
-        # if im.shape[2] == 1:
-        #     im = im[..., 0]
-    # Resize
-    if im.dtype == np.uint8:
-        im = im / 255
-    if im.shape[0] != img_size[0] or im.shape[1] != img_size[1]:
-        im = skt.resize(im, img_size)
-    return im
-
-
-def to_channels(im, out_channels, to_greyscale=False):
-    # Number of channels in image
-    if np.ndim(im) == 3:
-        img_channels = im.shape[2]
-    else:
-        im = im[..., np.newaxis]
-        img_channels = 1
-    # Convert to greyscale if needed:
-    if img_channels == 3 and to_greyscale is True:
-        im = skc.rgb2gray(im)[..., np.newaxis]
-        img_channels = 1
-    # Repeat if needed
-    if img_channels == 1 and out_channels == 3:
-        im = np.repeat(im, 3, axis=-1)
-    return im
-
-
-def resize_transform(im, shape, to_greyscale=False):
-    im = to_channels(im, shape[2], to_greyscale)
-    if im.shape[0] == shape[0] and im.shape[1] == shape[1]:
-        return im
-    im = skt.resize(im, shape)
-    return (im * 255).astype(np.uint8)
-
-
-def resize_with_pad_transform(im, shape, to_greyscale=False):
-    im = to_channels(im, shape[2], to_greyscale)
-    if im.shape[0] == shape[0] and im.shape[1] == shape[1]:
-        return im
-    im = resize_and_pad_image(im, shape)
-    return (im * 255).astype(np.uint8)
-
-
-def null_transform(im, args):
-    return im
+import numpy as np
+from skimage import io as skio, transform as skt, color as skc
+
+
+def load_image(filename, img_size=None, img_type='rgb'):
+    """
+    Loads an image, converting it if necessary
+    :param filename: Filename of image to load
+    :param img_size: Size of image, e.g. (224, 224). If None, the image dimensions are preserved
+    :param img_type: 'rgb' (colour) or 'k' (greyscale)
+    :return:
+    """
+    # Colour
+    if img_type == 'rgb':
+        im = skio.imread(filename)
+        # im = np.asarray(im, dtype=np.float)
+        # If it was a single channel image, make into 3-channel
+        if im.ndim == 2:
+            im = np.repeat(im[..., np.newaxis], repeats=3, axis=-1)
+    # Greyscale
+    elif img_type == 'k' or img_type == 'greyscale':
+        im = skio.imread(filename, as_gray=True)
+        im = im[..., np.newaxis]
+    else:
+        raise ValueError("img_type must be 'rgb' or 'k'")
+    # Resize and pad
+    if img_size is not None:
+        im = resize_and_pad_image(im, img_size)
+    return im
+
+
+def resize_and_pad_image(im, img_size):
+    # Add last dim if greyscale
+    if np.ndim(im) == 2:
+        im = im[..., np.newaxis]
+    # Get the ratio of width to height for each
+    current_whratio = im.shape[1] / im.shape[0]
+    desired_whratio = img_size[1] / img_size[0]
+    # Check if the image has roughly the same ratio, else pad it
+    if np.round(im.shape[0] * desired_whratio) != im.shape[1]:
+        height = im.shape[0]
+        width = im.shape[1]
+        # Desired shape is wider than current one
+        if desired_whratio > current_whratio:
+            half = np.round(height * desired_whratio)
+            height_pad_start = 0
+            height_pad_end = 0
+            width_pad_start = int(abs(np.floor((width - half) / 2)))
+            width_pad_end = int(abs(np.ceil((width - half) / 2)))
+        # Desired shape is taller than current
+        else:
+            half = np.round(width / desired_whratio)
+            height_pad_start = int(abs(np.floor((height - half) / 2)))
+            height_pad_end = int(abs(np.ceil((height - half) / 2)))
+            width_pad_start = 0
+            width_pad_end = 0
+        # Constant value to pad with
+        consts = [np.median(np.concatenate((im[0, :, i], im[-1, :, i], im[:, 0, i], im[:, -1, i]))) for i in range(im.shape[2])]
+        # Pad
+        im = np.stack(
+            [np.pad(im[:, :, c],
+                    ((height_pad_start, height_pad_end), (width_pad_start, width_pad_end)),
+                    mode='constant',
+                    constant_values=consts[c])
+             for c in range(im.shape[2])], axis=2)
+        # # Revert if was greyscale
+        # if im.shape[2] == 1:
+        #     im = im[..., 0]
+    # Resize
+    if im.dtype == np.uint8:
+        im = im / 255
+    if im.shape[0] != img_size[0] or im.shape[1] != img_size[1]:
+        im = skt.resize(im, img_size)
+    return im
+
+
+def to_channels(im, out_channels, to_greyscale=False):
+    # Number of channels in image
+    if np.ndim(im) == 3:
+        img_channels = im.shape[2]
+    else:
+        im = im[..., np.newaxis]
+        img_channels = 1
+    # Convert to greyscale if needed:
+    if img_channels == 3 and to_greyscale is True:
+        im = skc.rgb2gray(im)[..., np.newaxis]
+        img_channels = 1
+    # Repeat if needed
+    if img_channels == 1 and out_channels == 3:
+        im = np.repeat(im, 3, axis=-1)
+    return im
+
+
+def resize_transform(im, shape, to_greyscale=False):
+    im = to_channels(im, shape[2], to_greyscale)
+    if im.shape[0] == shape[0] and im.shape[1] == shape[1]:
+        return im
+    im = skt.resize(im, shape)
+    return (im * 255).astype(np.uint8)
+
+
+def resize_with_pad_transform(im, shape, to_greyscale=False):
+    im = to_channels(im, shape[2], to_greyscale)
+    if im.shape[0] == shape[0] and im.shape[1] == shape[1]:
+        return im
+    im = resize_and_pad_image(im, shape)
+    return (im * 255).astype(np.uint8)
+
+
+def null_transform(im, args):
+    return im
```

### Comparing `miso2-3.0.3/miso/data/tf_generator.py` & `miso2-3.0.4/miso/data/tf_generator.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,198 +1,198 @@
-import numpy as np
-import tensorflow as tf
-import tensorflow.keras.backend as K
-from imblearn.under_sampling import RandomUnderSampler
-
-
-class TFGenerator(object):
-    def __init__(self,
-                 data,
-                 cls=None,
-                 idxs=None,
-                 batch_size=32,
-                 shuffle=True,
-                 prefetch=4,
-                 map_fn=None,
-                 one_shot=False,
-                 undersample=False,
-                 data_dtype=tf.float32,
-                 labels_dtype=tf.float32):
-        """
-        Class to create a tf.data.Dataset given a set of data and associated labels.
-        Use the create() function to return the dataset
-        :param data: Input data
-        :param cls: Input class data (e.g. onehot vector or index), can be none
-        :param idxs: Indices of the data to use, if None all data are used
-        :param batch_size: Batch size for training / inference
-        :param shuffle: Whether to shuffle the data each time
-        :param prefetch: How many batches to prefetch
-        :param map_fn: Function applied to the data when creating a batch. Must take a tensor as input
-        :param one_shot: If True, dataset will only iterate through the data once. (Use for validation / inference etc)
-        """
-        self.data = data
-        self.data_dtype = data_dtype
-        if isinstance(cls, list):
-            cls = np.asarray(cls)
-        self.labels = cls
-        self.labels_dtype = labels_dtype
-        self.batch_size = batch_size
-        self.shuffle = shuffle
-        self.prefetch = prefetch
-        self.map_fn = map_fn
-        self.one_shot = one_shot
-        self.undersample = undersample
-        if idxs is None:
-            self.idxs = np.arange(len(data))
-        else:
-            self.idxs = idxs.copy()
-        self.on_epoch_end()
-
-    def __len__(self):
-        if self.one_shot:
-            return int(np.ceil(len(self.idxs) / self.batch_size))
-        else:
-            return int(np.floor(len(self.idxs) / self.batch_size))
-
-    def on_epoch_end(self):
-        if self.undersample:
-            rus = RandomUnderSampler()
-            if isinstance(self.labels[0], np.ndarray):
-                c = np.argmax(self.labels, axis=-1)
-            else:
-                c = self.labels
-            x, y = rus.fit_sample(self.idxs.reshape(-1, 1), c[self.idxs])
-            x = x.flatten()
-            #y = y.flatten()
-            np.random.shuffle(x)
-            #print(len(x))
-            #print(np.unique(y, return_counts=True))
-            #np.random.shuffle(y)
-            #for i in range(100):
-            #    print(y[i], end="")
-            #print()
-            self.idxs = x
-        elif self.shuffle:
-            np.random.shuffle(self.idxs)
-
-    def generator(self):
-        """
-        Generates pairs of data and optionally, cls. After all data is processed, the index is randomised
-        :return: generator of (data[i], cls[i])
-        """
-        i = 0
-        while i < len(self.idxs):
-            idx = self.idxs[i]
-            if self.labels is None:
-                yield self.data[idx]
-            else:
-                yield (self.data[idx], self.labels[idx])
-            i += 1
-        self.on_epoch_end()
-
-    def to_tfdataset(self):
-        """
-        Creates the tf.data.Dataset
-        :return: A tf.data.Dataset that iterates through batches of (data, label) pairs
-        """
-        if isinstance(self.labels, list) or np.ndim(self.labels) <= 1:
-            label_shape = None
-        else:
-            label_shape = self.labels[0].shape
-        if self.labels is not None:
-            ds = tf.data.Dataset.from_generator(self.generator,
-                                                output_types=(self.data_dtype, self.labels_dtype),
-                                                output_shapes=(self.data[0].shape, label_shape))
-        else:
-            ds = tf.data.Dataset.from_generator(self.generator,
-                                                output_types=self.data_dtype,
-                                                output_shapes=self.data[0].shape)
-        """
-        From docs:
-        Performance can often be improved by setting num_parallel_calls so that map will use multiple threads to process elements. 
-        If deterministic order isn't required, it can also improve performance to set deterministic=False.
-
-        Note that the map function has to take a Tensor input
-        """
-        if self.map_fn is not None:
-            ds = ds.map(lambda x, y: (self.map_fn(x), y), num_parallel_calls=tf.data.experimental.AUTOTUNE)
-        if self.one_shot is False:
-            ds = ds.repeat()
-        ds = ds.batch(self.batch_size).prefetch(self.prefetch)
-        return ds
-
-    def tf1_compat_generator_error(self):
-        # Get shapes from input data
-        images = self.data
-        onehots = self.labels
-        shuffle_size = 1000
-        img_size = images.shape
-        img_size = (None, *img_size[1:])
-        onehot_size = onehots.shape
-        onehot_size = (None, onehot_size[1])
-        images_tensor = tf.placeholder(tf.float32, shape=img_size)
-        onehots_tensor = tf.placeholder(tf.float32, shape=onehot_size)
-        # Create dataset
-        dataset = tf.data.Dataset.from_tensor_slices((images_tensor, onehots_tensor))
-        if self.map_fn is not None:
-            dataset = dataset.map(lambda x, y: (self.map_fn(x), y), num_parallel_calls=tf.data.experimental.AUTOTUNE)
-        if self.one_shot:
-            dataset = dataset.repeat(1)
-        else:
-            dataset = dataset.shuffle(shuffle_size, reshuffle_each_iteration=True).repeat()
-        dataset = dataset.batch(self.batch_size)
-        dataset = dataset.prefetch(1)
-        iterator = dataset.make_initializable_iterator()
-        init_op = iterator.initializer
-        next_val = iterator.get_next()
-        with K.get_session().as_default() as sess:
-            sess.run(init_op, feed_dict={images_tensor: images, onehots_tensor: onehots})
-            while True:
-                inputs, labels = sess.run(next_val)
-                yield inputs, labels
-
-    def tf1_compat_generator(self):
-        if isinstance(self.labels, list) or np.ndim(self.labels) <= 1:
-            label_shape = None
-        else:
-            label_shape = self.labels[0].shape
-        if self.labels is not None:
-            ds = tf.data.Dataset.from_generator(self.generator,
-                                                output_types=(self.data_dtype, self.labels_dtype),
-                                                output_shapes=(self.data[0].shape, label_shape))
-        else:
-            ds = tf.data.Dataset.from_generator(self.generator,
-                                                output_types=self.data_dtype,
-                                                output_shapes=self.data[0].shape)
-        if self.map_fn is not None:
-            ds = ds.map(lambda x, y: (self.map_fn(x), y), num_parallel_calls=tf.data.experimental.AUTOTUNE)
-        if self.one_shot is False:
-            ds = ds.repeat()
-        ds = ds.batch(self.batch_size).prefetch(self.prefetch)
-        iterator = ds.make_initializable_iterator()
-        init_op = iterator.initializer
-        next_val = iterator.get_next()
-        with K.get_session().as_default() as sess:
-            sess.run(init_op)
-            while True:
-                inputs, labels = sess.run(next_val)
-                yield inputs, labels
-
-    def create(self):
-        if int(tf.__version__[0]) == 2:
-            return self.to_tfdataset()
-        else:
-            return self.tf1_compat_generator()
-
-    @staticmethod
-    def map_fn_divide_255(t):
-        t = tf.cast(t, tf.float32)
-        return tf.divide(t, 255.0)
-
-    @staticmethod
-    def map_fn_divide_255_and_rotate_fn(k):
-        def wrapper(t):
-            t = tf.cast(t, tf.float32)
-            t = tf.image.rot90(t, k)
-            return tf.divide(t, 255.0)
-        return wrapper
-
+import numpy as np
+import tensorflow as tf
+import tensorflow.keras.backend as K
+from imblearn.under_sampling import RandomUnderSampler
+
+
+class TFGenerator(object):
+    def __init__(self,
+                 data,
+                 cls=None,
+                 idxs=None,
+                 batch_size=32,
+                 shuffle=True,
+                 prefetch=4,
+                 map_fn=None,
+                 one_shot=False,
+                 undersample=False,
+                 data_dtype=tf.float32,
+                 labels_dtype=tf.float32):
+        """
+        Class to create a tf.data.Dataset given a set of data and associated labels.
+        Use the create() function to return the dataset
+        :param data: Input data
+        :param cls: Input class data (e.g. onehot vector or index), can be none
+        :param idxs: Indices of the data to use, if None all data are used
+        :param batch_size: Batch size for training / inference
+        :param shuffle: Whether to shuffle the data each time
+        :param prefetch: How many batches to prefetch
+        :param map_fn: Function applied to the data when creating a batch. Must take a tensor as input
+        :param one_shot: If True, dataset will only iterate through the data once. (Use for validation / inference etc)
+        """
+        self.data = data
+        self.data_dtype = data_dtype
+        if isinstance(cls, list):
+            cls = np.asarray(cls)
+        self.labels = cls
+        self.labels_dtype = labels_dtype
+        self.batch_size = batch_size
+        self.shuffle = shuffle
+        self.prefetch = prefetch
+        self.map_fn = map_fn
+        self.one_shot = one_shot
+        self.undersample = undersample
+        if idxs is None:
+            self.idxs = np.arange(len(data))
+        else:
+            self.idxs = idxs.copy()
+        self.on_epoch_end()
+
+    def __len__(self):
+        if self.one_shot:
+            return int(np.ceil(len(self.idxs) / self.batch_size))
+        else:
+            return int(np.floor(len(self.idxs) / self.batch_size))
+
+    def on_epoch_end(self):
+        if self.undersample:
+            rus = RandomUnderSampler()
+            if isinstance(self.labels[0], np.ndarray):
+                c = np.argmax(self.labels, axis=-1)
+            else:
+                c = self.labels
+            x, y = rus.fit_sample(self.idxs.reshape(-1, 1), c[self.idxs])
+            x = x.flatten()
+            #y = y.flatten()
+            np.random.shuffle(x)
+            #print(len(x))
+            #print(np.unique(y, return_counts=True))
+            #np.random.shuffle(y)
+            #for i in range(100):
+            #    print(y[i], end="")
+            #print()
+            self.idxs = x
+        elif self.shuffle:
+            np.random.shuffle(self.idxs)
+
+    def generator(self):
+        """
+        Generates pairs of data and optionally, cls. After all data is processed, the index is randomised
+        :return: generator of (data[i], cls[i])
+        """
+        i = 0
+        while i < len(self.idxs):
+            idx = self.idxs[i]
+            if self.labels is None:
+                yield self.data[idx]
+            else:
+                yield (self.data[idx], self.labels[idx])
+            i += 1
+        self.on_epoch_end()
+
+    def to_tfdataset(self):
+        """
+        Creates the tf.data.Dataset
+        :return: A tf.data.Dataset that iterates through batches of (data, label) pairs
+        """
+        if isinstance(self.labels, list) or np.ndim(self.labels) <= 1:
+            label_shape = None
+        else:
+            label_shape = self.labels[0].shape
+        if self.labels is not None:
+            ds = tf.data.Dataset.from_generator(self.generator,
+                                                output_types=(self.data_dtype, self.labels_dtype),
+                                                output_shapes=(self.data[0].shape, label_shape))
+        else:
+            ds = tf.data.Dataset.from_generator(self.generator,
+                                                output_types=self.data_dtype,
+                                                output_shapes=self.data[0].shape)
+        """
+        From docs:
+        Performance can often be improved by setting num_parallel_calls so that map will use multiple threads to process elements. 
+        If deterministic order isn't required, it can also improve performance to set deterministic=False.
+
+        Note that the map function has to take a Tensor input
+        """
+        if self.map_fn is not None:
+            ds = ds.map(lambda x, y: (self.map_fn(x), y), num_parallel_calls=tf.data.experimental.AUTOTUNE)
+        if self.one_shot is False:
+            ds = ds.repeat()
+        ds = ds.batch(self.batch_size).prefetch(self.prefetch)
+        return ds
+
+    def tf1_compat_generator_error(self):
+        # Get shapes from input data
+        images = self.data
+        onehots = self.labels
+        shuffle_size = 1000
+        img_size = images.shape
+        img_size = (None, *img_size[1:])
+        onehot_size = onehots.shape
+        onehot_size = (None, onehot_size[1])
+        images_tensor = tf.placeholder(tf.float32, shape=img_size)
+        onehots_tensor = tf.placeholder(tf.float32, shape=onehot_size)
+        # Create dataset
+        dataset = tf.data.Dataset.from_tensor_slices((images_tensor, onehots_tensor))
+        if self.map_fn is not None:
+            dataset = dataset.map(lambda x, y: (self.map_fn(x), y), num_parallel_calls=tf.data.experimental.AUTOTUNE)
+        if self.one_shot:
+            dataset = dataset.repeat(1)
+        else:
+            dataset = dataset.shuffle(shuffle_size, reshuffle_each_iteration=True).repeat()
+        dataset = dataset.batch(self.batch_size)
+        dataset = dataset.prefetch(1)
+        iterator = dataset.make_initializable_iterator()
+        init_op = iterator.initializer
+        next_val = iterator.get_next()
+        with K.get_session().as_default() as sess:
+            sess.run(init_op, feed_dict={images_tensor: images, onehots_tensor: onehots})
+            while True:
+                inputs, labels = sess.run(next_val)
+                yield inputs, labels
+
+    def tf1_compat_generator(self):
+        if isinstance(self.labels, list) or np.ndim(self.labels) <= 1:
+            label_shape = None
+        else:
+            label_shape = self.labels[0].shape
+        if self.labels is not None:
+            ds = tf.data.Dataset.from_generator(self.generator,
+                                                output_types=(self.data_dtype, self.labels_dtype),
+                                                output_shapes=(self.data[0].shape, label_shape))
+        else:
+            ds = tf.data.Dataset.from_generator(self.generator,
+                                                output_types=self.data_dtype,
+                                                output_shapes=self.data[0].shape)
+        if self.map_fn is not None:
+            ds = ds.map(lambda x, y: (self.map_fn(x), y), num_parallel_calls=tf.data.experimental.AUTOTUNE)
+        if self.one_shot is False:
+            ds = ds.repeat()
+        ds = ds.batch(self.batch_size).prefetch(self.prefetch)
+        iterator = ds.make_initializable_iterator()
+        init_op = iterator.initializer
+        next_val = iterator.get_next()
+        with K.get_session().as_default() as sess:
+            sess.run(init_op)
+            while True:
+                inputs, labels = sess.run(next_val)
+                yield inputs, labels
+
+    def create(self):
+        if int(tf.__version__[0]) == 2:
+            return self.to_tfdataset()
+        else:
+            return self.tf1_compat_generator()
+
+    @staticmethod
+    def map_fn_divide_255(t):
+        t = tf.cast(t, tf.float32)
+        return tf.divide(t, 255.0)
+
+    @staticmethod
+    def map_fn_divide_255_and_rotate_fn(k):
+        def wrapper(t):
+            t = tf.cast(t, tf.float32)
+            t = tf.image.rot90(t, k)
+            return tf.divide(t, 255.0)
+        return wrapper
+
```

### Comparing `miso2-3.0.3/miso/data/training_dataset.py` & `miso2-3.0.4/miso/data/training_dataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,145 @@
-from typing import NamedTuple
-
-from sklearn.model_selection import train_test_split
-from tensorflow.keras.utils import to_categorical
-import numpy as np
-from scipy.stats.mstats import gmean
-
-from miso.data.filenames_dataset import FilenamesDataset
-from miso.data.image_dataset import ImageDataset
-from miso.data.tf_generator import TFGenerator
-
-
-class TrainingDataset(object):
-    def __init__(self,
-                 source,
-                 img_size=(224, 224, 3),
-                 img_type='rgb',
-                 min_count=0,
-                 map_others=False,
-                 test_split=0.2,
-                 random_seed=0,
-                 memmap_directory=None):
-        if len(img_size) != 3:
-            raise ValueError("img_size must be in format [height, width, num_channels]")
-        self.source = source
-        self.img_size = img_size
-        self.img_type = img_type
-        self.min_count = min_count
-        self.map_others = map_others
-        self.test_split = test_split
-        self.random_seed = random_seed
-        self.memmap_directory = memmap_directory
-
-        self.filenames: FilenamesDataset = None
-        self.images: ImageDataset = None
-        self.train_idx = None
-        self.test_idx = None
-        self.cls = None
-        self.cls_onehot = None
-        self.cls_labels = None
-        self.num_classes = None
-        self.class_weights = None
-
-    def get_class_weights(self):
-        count = np.bincount(self.data_df['cls'])
-        weights = gmean(count) / count
-        weights[weights < 0.1] = 0.1
-        weights[weights > 10] = 10
-        return weights
-
-    def load(self):
-        # Get filenames
-        fs = FilenamesDataset(self.source, has_classes=True)
-        fs.load(self.min_count, self.map_others)
-        self.filenames = fs
-        self.cls = self.filenames.cls
-        self.cls_labels = fs.cls_labels
-        self.num_classes = fs.num_classes
-
-        # Create one hot
-        self.cls_onehot = to_categorical(fs.cls)
-
-        # Class weights
-        weights = gmean(fs.cls_counts) / fs.cls_counts
-        weights[weights < 0.1] = 0.1
-        weights[weights > 10] = 10
-        self.class_weights = weights
-
-        # Create split
-        self.train_idx, self.test_idx = train_test_split(np.arange(len(self.filenames.filenames)),
-                                                         stratify=self.cls,
-                                                         test_size=self.test_split,
-                                                         random_state=self.random_seed)
-
-        # Load images
-        to_greyscale = False
-        if self.img_type == 'k' or self.img_type == 'greyscale':
-            to_greyscale = True
-        # print(self.img_size)
-        self.images = ImageDataset(self.filenames.filenames,
-                                   self.cls_onehot,
-                                   transform_fn='resize_with_pad',
-                                   transform_args=[self.img_size, to_greyscale],
-                                   memmap_directory=self.memmap_directory)
-        self.images.load()
-
-    def train_generator(self, batch_size=32, shuffle=True, one_shot=False, undersample=False, map_fn=TFGenerator.map_fn_divide_255):
-        return self.images.create_generator(batch_size, self.train_idx, map_fn=map_fn, shuffle=shuffle, one_shot=one_shot, undersample=undersample)
-
-    def test_generator(self, batch_size=32, shuffle=True, one_shot=False, undersample=False, map_fn=TFGenerator.map_fn_divide_255):
-        return self.images.create_generator(batch_size, self.test_idx, map_fn=map_fn, shuffle=shuffle, one_shot=one_shot, undersample=undersample)
-
-    def release(self):
-        self.images.release()
-
-
-if __name__ == "__main__":
-    source = "/Users/chaos/Documents/Development/Data/Modern_Coretop_Source/project.xml"
-    import matplotlib.pyplot as plt
-    # XML
-    ts = TrainingDataset(source,
-                         img_size=[224, 224, 1],
-                         img_type='k',
-                         min_count=10,
-                         map_others=False,
-                         test_split=0.2,
-                         random_seed=0,
-                         memmap_directory=None)
-    ts.load(32)
-    im = ts.images.data[0]
-    plt.imshow(im)
-    plt.title("shape: {}, max: {}, min: {}".format(im.shape, im.max(), im.min()))
-    plt.show()
-
-    ts = TrainingDataset(source,
-                         img_size=[224, 224, 3],
-                         img_type='k',
-                         min_count=10,
-                         map_others=False,
-                         test_split=0.2,
-                         random_seed=0,
-                         memmap_directory=None)
-    ts.load(32)
-    im = ts.images.data[0]
-    plt.imshow(im)
-    plt.title("shape: {}, max: {}, min: {}".format(im.shape, im.max(), im.min()))
-    plt.show()
-
-    ts = TrainingDataset(source,
-                         img_size=[224, 224, 3],
-                         img_type='rgb',
-                         min_count=10,
-                         map_others=False,
-                         test_split=0.2,
-                         random_seed=0,
-                         memmap_directory=None)
-    ts.load(32)
-    im = ts.images.data[0]
-    plt.imshow(im)
-    plt.title("shape: {}, max: {}, min: {}".format(im.shape, im.max(), im.min()))
-    plt.show()
+from typing import NamedTuple
+
+from sklearn.model_selection import train_test_split
+from tensorflow.keras.utils import to_categorical
+import numpy as np
+from scipy.stats.mstats import gmean
+
+from miso.data.filenames_dataset import FilenamesDataset
+from miso.data.image_dataset import ImageDataset
+from miso.data.tf_generator import TFGenerator
+
+
+class TrainingDataset(object):
+    def __init__(self,
+                 source,
+                 img_size=(224, 224, 3),
+                 img_type='rgb',
+                 min_count=0,
+                 map_others=False,
+                 test_split=0.2,
+                 random_seed=0,
+                 memmap_directory=None):
+        if len(img_size) != 3:
+            raise ValueError("img_size must be in format [height, width, num_channels]")
+        self.source = source
+        self.img_size = img_size
+        self.img_type = img_type
+        self.min_count = min_count
+        self.map_others = map_others
+        self.test_split = test_split
+        self.random_seed = random_seed
+        self.memmap_directory = memmap_directory
+
+        self.filenames: FilenamesDataset = None
+        self.images: ImageDataset = None
+        self.train_idx = None
+        self.test_idx = None
+        self.cls = None
+        self.cls_onehot = None
+        self.cls_labels = None
+        self.num_classes = None
+        self.class_weights = None
+
+    def get_class_weights(self):
+        count = np.bincount(self.data_df['cls'])
+        weights = gmean(count) / count
+        weights[weights < 0.1] = 0.1
+        weights[weights > 10] = 10
+        return weights
+
+    def load(self):
+        # Get filenames
+        fs = FilenamesDataset(self.source, has_classes=True)
+        fs.load(self.min_count, self.map_others)
+        self.filenames = fs
+        self.cls = self.filenames.cls
+        self.cls_labels = fs.cls_labels
+        self.num_classes = fs.num_classes
+
+        # Create one hot
+        self.cls_onehot = to_categorical(fs.cls)
+
+        # Class weights
+        weights = gmean(fs.cls_counts) / fs.cls_counts
+        weights[weights < 0.1] = 0.1
+        weights[weights > 10] = 10
+        self.class_weights = weights
+
+        # Create split
+        if self.test_split > 0:
+            self.train_idx, self.test_idx = train_test_split(np.arange(len(self.filenames.filenames)),
+                                                             stratify=self.cls,
+                                                             test_size=self.test_split,
+                                                             random_state=self.random_seed)
+        else:
+            self.train_idx = np.arange(len(self.filenames.filenames))
+            self.test_idx = []
+
+        # Load images
+        to_greyscale = False
+        if self.img_type == 'k' or self.img_type == 'greyscale':
+            to_greyscale = True
+        # print(self.img_size)
+        self.images = ImageDataset(self.filenames.filenames,
+                                   self.cls_onehot,
+                                   transform_fn='resize_with_pad',
+                                   transform_args=[self.img_size, to_greyscale],
+                                   memmap_directory=self.memmap_directory)
+        self.images.load()
+
+    def train_generator(self, batch_size=32, shuffle=True, one_shot=False, undersample=False, map_fn=TFGenerator.map_fn_divide_255):
+        return self.images.create_generator(batch_size, self.train_idx, map_fn=map_fn, shuffle=shuffle, one_shot=one_shot, undersample=undersample)
+
+    def test_generator(self, batch_size=32, shuffle=True, one_shot=False, undersample=False, map_fn=TFGenerator.map_fn_divide_255):
+        return self.images.create_generator(batch_size, self.test_idx, map_fn=map_fn, shuffle=shuffle, one_shot=one_shot, undersample=undersample)
+
+    def release(self):
+        self.images.release()
+
+
+if __name__ == "__main__":
+    source = "/Users/chaos/Documents/Development/Data/Modern_Coretop_Source/project.xml"
+    import matplotlib.pyplot as plt
+    # XML
+    ts = TrainingDataset(source,
+                         img_size=[224, 224, 1],
+                         img_type='k',
+                         min_count=10,
+                         map_others=False,
+                         test_split=0.2,
+                         random_seed=0,
+                         memmap_directory=None)
+    ts.load(32)
+    im = ts.images.data[0]
+    plt.imshow(im)
+    plt.title("shape: {}, max: {}, min: {}".format(im.shape, im.max(), im.min()))
+    plt.show()
+
+    ts = TrainingDataset(source,
+                         img_size=[224, 224, 3],
+                         img_type='k',
+                         min_count=10,
+                         map_others=False,
+                         test_split=0.2,
+                         random_seed=0,
+                         memmap_directory=None)
+    ts.load(32)
+    im = ts.images.data[0]
+    plt.imshow(im)
+    plt.title("shape: {}, max: {}, min: {}".format(im.shape, im.max(), im.min()))
+    plt.show()
+
+    ts = TrainingDataset(source,
+                         img_size=[224, 224, 3],
+                         img_type='rgb',
+                         min_count=10,
+                         map_others=False,
+                         test_split=0.2,
+                         random_seed=0,
+                         memmap_directory=None)
+    ts.load(32)
+    im = ts.images.data[0]
+    plt.imshow(im)
+    plt.title("shape: {}, max: {}, min: {}".format(im.shape, im.max(), im.min()))
+    plt.show()
```

### Comparing `miso2-3.0.3/miso/data/utils.py` & `miso2-3.0.4/miso/data/utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import glob
-import os
-from collections import OrderedDict
-import pandas as pd
-import platform
-
-
-def list_directory(source_dir):
-    return sorted(glob.glob(os.path.join(source_dir, "*")))
-
-
-def parse_directory(source_dir, verbose=True, skip='~', has_classes=True, sub_directories=[]):
-    """
-    Parses a directory consisting of subdirectories named by class and stores the image filenames in a dictionary
-    :param source_dir: The directory to parse
-    :param verbose: Print out the progress
-    :param skip: If a subdirectory starts with this character it will be skipped ('_' and '.' are skipped always, unless skip is None)
-    :param has_classes: The files are arranged in subsdirectories by class name
-    :return: Dictionary with class names for the keys and lists of filenames for the values
-    """
-    if has_classes:
-        sub_dirs = sorted(glob.glob(os.path.join(source_dir, "*")))
-    else:
-        sub_dirs = [source_dir]
-    filenames = OrderedDict()
-    if verbose:
-        print("Parsing directory {}".format(source_dir))
-    for sub_dir in sub_dirs:
-        if os.path.isdir(sub_dir) is False:
-            continue
-        # Get the directory name
-        sub_name = os.path.basename(sub_dir)
-        # Skip directories starting with ~
-        if sub_name.startswith(skip) or \
-            sub_name.startswith('_') or \
-            sub_name.startswith('.'):
-            continue
-        # Get the files
-        if verbose:
-            print("- {}".format(sub_name), end='')
-        files = []
-        for ext in ["*.jpg", "*.jpeg", "*.png", "*.tif", "*.tiff", "*.bmp"]:
-            sub_files1 = sorted(glob.glob(os.path.join(sub_dir, *sub_directories, ext)))
-            files.extend(sub_files1)
-            if platform.system() == 'Linux':
-                sub_files2 = sorted(glob.glob(os.path.join(sub_dir, *sub_directories, ext.upper())))
-                files.extend(sub_files2)
-        # Add to dictionary
-        if verbose:
-            print(" ({} files)".format(len(files)))
-        if has_classes:
-            filenames[sub_name] = files
-        else:
-            filenames['null'] = files
-    return filenames
-
-
-def flatten_to_list(filenames_dict: dict):
-    filenames = []
-    for value in filenames_dict.values():
-        filenames.extend(value)
-    return filenames
-
-
-def parse_csv(csv_file, source_dir, file_idx=0, cls_idx=1, cls_label_idx=2, verbose=True):
-    if verbose:
-        print("Parsing csv file {} for directory {}".format(csv_file, source_dir))
-    df = pd.read_csv(csv_file)
-    num_classes = np.max(df.iloc[:, cls_idx]) + 1
-    cls_labels = [df.loc[df.iloc[:, cls_idx] == i].iloc[0, cls_label_idx] for i in range(num_classes)]
-    filenames = OrderedDict()
-    for i in range(num_classes):
-        if verbose:
-            print("- {}".format(cls_labels[i]), end='')
-        names = df.loc[df.iloc[:, cls_idx] == i].iloc[:, file_idx]
-        paths = [os.path.join(source_dir, n) for n in names]
-        filenames[cls_labels[i]] = paths
-        if verbose:
-            print(" ({} files)".format(len(paths)))
-    return filenames
-
-
-if __name__ == "__main__":
-    from mml.data.filenames_dataset import FilenamesDataset
-    import numpy as np
-
-    result = parse_csv(r"D:\Datasets\Weeds\labels.csv",
-                       r"D:\Datasets\Weeds\DeepWeeds")
-
-    # fs = FilenamesDataset(r"C:\data\SeagrassFrames")
-    # fs.split(0.2)
-    # arr = np.zeros(len(fs.train_filenames))
+import glob
+import os
+from collections import OrderedDict
+import pandas as pd
+import platform
+
+
+def list_directory(source_dir):
+    return sorted(glob.glob(os.path.join(source_dir, "*")))
+
+
+def parse_directory(source_dir, verbose=True, skip='~', has_classes=True, sub_directories=[]):
+    """
+    Parses a directory consisting of subdirectories named by class and stores the image filenames in a dictionary
+    :param source_dir: The directory to parse
+    :param verbose: Print out the progress
+    :param skip: If a subdirectory starts with this character it will be skipped ('_' and '.' are skipped always, unless skip is None)
+    :param has_classes: The files are arranged in subsdirectories by class name
+    :return: Dictionary with class names for the keys and lists of filenames for the values
+    """
+    if has_classes:
+        sub_dirs = sorted(glob.glob(os.path.join(source_dir, "*")))
+    else:
+        sub_dirs = [source_dir]
+    filenames = OrderedDict()
+    if verbose:
+        print("Parsing directory {}".format(source_dir))
+    for sub_dir in sub_dirs:
+        if os.path.isdir(sub_dir) is False:
+            continue
+        # Get the directory name
+        sub_name = os.path.basename(sub_dir)
+        # Skip directories starting with ~
+        if sub_name.startswith(skip) or \
+            sub_name.startswith('_') or \
+            sub_name.startswith('.'):
+            continue
+        # Get the files
+        if verbose:
+            print("- {}".format(sub_name), end='')
+        files = []
+        for ext in ["*.jpg", "*.jpeg", "*.png", "*.tif", "*.tiff", "*.bmp"]:
+            sub_files1 = sorted(glob.glob(os.path.join(sub_dir, *sub_directories, ext)))
+            files.extend(sub_files1)
+            if platform.system() == 'Linux':
+                sub_files2 = sorted(glob.glob(os.path.join(sub_dir, *sub_directories, ext.upper())))
+                files.extend(sub_files2)
+        # Add to dictionary
+        if verbose:
+            print(" ({} files)".format(len(files)))
+        if has_classes:
+            filenames[sub_name] = files
+        else:
+            filenames['null'] = files
+    return filenames
+
+
+def flatten_to_list(filenames_dict: dict):
+    filenames = []
+    for value in filenames_dict.values():
+        filenames.extend(value)
+    return filenames
+
+
+def parse_csv(csv_file, source_dir, file_idx=0, cls_idx=1, cls_label_idx=2, verbose=True):
+    if verbose:
+        print("Parsing csv file {} for directory {}".format(csv_file, source_dir))
+    df = pd.read_csv(csv_file)
+    num_classes = np.max(df.iloc[:, cls_idx]) + 1
+    cls_labels = [df.loc[df.iloc[:, cls_idx] == i].iloc[0, cls_label_idx] for i in range(num_classes)]
+    filenames = OrderedDict()
+    for i in range(num_classes):
+        if verbose:
+            print("- {}".format(cls_labels[i]), end='')
+        names = df.loc[df.iloc[:, cls_idx] == i].iloc[:, file_idx]
+        paths = [os.path.join(source_dir, n) for n in names]
+        filenames[cls_labels[i]] = paths
+        if verbose:
+            print(" ({} files)".format(len(paths)))
+    return filenames
+
+
+if __name__ == "__main__":
+    from mml.data.filenames_dataset import FilenamesDataset
+    import numpy as np
+
+    result = parse_csv(r"D:\Datasets\Weeds\labels.csv",
+                       r"D:\Datasets\Weeds\DeepWeeds")
+
+    # fs = FilenamesDataset(r"C:\data\SeagrassFrames")
+    # fs.split(0.2)
+    # arr = np.zeros(len(fs.train_filenames))
     # load_images(fs.train_filenames, arr, None)
```

### Comparing `miso2-3.0.3/miso/deploy/inference.py` & `miso2-3.0.4/miso/deploy/inference.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-"""
-Performs inference on a directory of images organised by subdirectories, returning a pandas dataframe with the filename
-and its classification
-"""
-import tensorflow as tf
-from tensorflow.keras.utils import Sequence, OrderedEnqueuer
-import numpy as np
-from miso.archive.datasource import DataSource
-import lxml.etree as ET
-from tensorflow.python.platform import gfile
-import tensorflow.keras.backend as K
-import os
-import pandas as pd
-import multiprocessing
-from pathlib import Path
-
-
-class InferenceGenerator(Sequence):
-    def __init__(self, source_dir, batch_size, img_size, img_type):
-        self.source_dir = source_dir
-        self.batch_size = batch_size
-        self.img_size = img_size
-        self.img_type = img_type
-        filenames = DataSource.parse_directory(source_dir)
-        self.filenames = [v for key, val in filenames.items() for v in val]
-
-    def __data_generation(self, filenames):
-        images = []
-        for filename in filenames:
-            image = DataSource.load_image(filename, self.img_size, self.img_type)
-            image = DataSource.preprocess_image(image)
-            images.append(image)
-        return filenames, np.asarray(images)
-
-    def __getitem__(self, index):
-        batch_filenames = self.filenames[index * self.batch_size:(index + 1) * self.batch_size]
-        filenames_and_images = self.__data_generation(batch_filenames)
-        return filenames_and_images
-
-    def __len__(self):
-        return int(np.ceil(len(self.filenames) / self.batch_size))
-
-
-def load_from_frozen(source: str,
-                     input_tensor="input_1:0",
-                     output_tensor="conv2d_23/Sigmoid:0",
-                     session=None):
-    if not os.path.exists(source):
-        raise FileNotFoundError('The graph file was not found on the system.\nThe path was: ' + source)
-    # Load network
-    if session is None:
-        session = K.get_session()
-    with gfile.Open(source, 'rb') as f:
-        graph_def = tf.GraphDef()
-        graph_def.ParseFromString(f.read())
-        session.graph.as_default()
-        tf.import_graph_def(graph_def, name='')
-    input = session.graph.get_tensor_by_name(input_tensor)
-    output = session.graph.get_tensor_by_name(output_tensor)
-    return session, input, output
-
-
-def load_from_xml(filename, session=None):
-    project = ET.parse(filename).getroot()
-
-    protobuf = project.find('protobuf').text
-    print("protobuf: " + protobuf)
-
-    input = None
-    output = None
-    img_size = np.zeros(3, dtype=np.int)
-    cls_labels = []
-
-    list_xml = project.find('labels')
-    for i, entry_xml  in enumerate(list_xml.iter('label')):
-        code = entry_xml.find('code').text
-        cls_labels.append(code)
-
-    list_xml = project.find('inputs')
-    for i, entry_xml in enumerate(list_xml.iter('input')):
-        if i == 0:
-            input_name = entry_xml.find('operation').text + ":0"
-            img_size[0] = int(entry_xml.find('height').text)
-            img_size[1] = int(entry_xml.find('width').text)
-            img_size[2] = int(entry_xml.find('channels').text)
-
-    list_xml = project.find('outputs')
-    for i, entry_xml in enumerate(list_xml.iter('output')):
-        if i == 0:
-            output_name = entry_xml.find('operation').text + ":0"
-
-    full_protobuf_path = os.path.join(os.path.dirname(filename), protobuf)
-    session, input, output = load_from_frozen(full_protobuf_path, input_name, output_name)
-    return session, input, output, img_size, cls_labels
-
-
-def process(network_info, images_dir, output_dir, threshold=0.8):
-    session, input_tensor, output_tensor, img_size, cls_labels = load_from_xml(network_info)
-    print("Input tensor: {}".format(input_tensor))
-    print("Output tensor: {}".format(output_tensor))
-    print("Image size: {}".format(img_size))
-    print("Classes: {}".format(cls_labels))
-    print()
-    print("Parsing source directory... (this can take some time)")
-    if img_size[2] == 3:
-        img_type = 'rgb'
-    else:
-        img_type = 'greyscale'
-    gen = InferenceGenerator(images_dir, 64, img_size, img_type)
-
-    print("Files: {}".format(len(gen.filenames)))
-    print("Batches: {}".format(len(gen)))
-
-    workers = np.min((multiprocessing.cpu_count(), 8))
-    print("Workers: {}".format(workers))
-    print()
-
-    filenames = []
-    cls_index = []
-    cls_names = []
-    score = []
-    enq = OrderedEnqueuer(gen, use_multiprocessing=True)
-    enq.start(workers=workers, max_queue_size=multiprocessing.cpu_count()*4)
-    output_generator = enq.get()
-    for i in range(len(gen)):
-        print("\r{} / {}".format(i, len(gen)), end='')
-        batch_filenames, batch_images = next(output_generator)
-        result = session.run(output_tensor, feed_dict={input_tensor: batch_images})
-        cls = np.argmax(result, axis=1)
-        scr = np.max(result, axis=1)
-        cls_name = [cls_labels[i] for i in cls]
-        filenames.extend(batch_filenames)
-        cls_index.extend(cls)
-        cls_names.extend(cls_name)
-        score.extend(scr)
-    enq.stop()
-    print()
-    print("Done")
-    print("See {} for results".format(output_dir))
-
-    parents = [Path(f).parent.name for f in filenames]
-    files = [Path(f).name for f in filenames]
-
-    df = pd.DataFrame(data={'filename': filenames, 'parent': parents, 'file': files, 'class': cls_names, 'class_index': cls_index, 'score': score})
-    os.makedirs(output_directory, exist_ok=True)
-    df.to_csv(os.path.join(output_dir, "inference.csv"))
-
-
-if __name__ == "__main__":
-    network_info = r"D:\Development\Microfossil\PaperExperiments\Paper1CNNForMicrofossil\MD972138\Output\MD972138_base_cyclic_8_20200410-173126\model\network_info.xml"
-    images_directory = r"D:\Datasets\Foraminifera\images_20200226_114546 Fifth with background"
-    output_directory = r"D:\output"
-    process(network_info, images_directory, output_directory)
-
+"""
+Performs inference on a directory of images organised by subdirectories, returning a pandas dataframe with the filename
+and its classification
+"""
+import tensorflow as tf
+from tensorflow.keras.utils import Sequence, OrderedEnqueuer
+import numpy as np
+from miso.archive.datasource import DataSource
+import lxml.etree as ET
+from tensorflow.python.platform import gfile
+import tensorflow.keras.backend as K
+import os
+import pandas as pd
+import multiprocessing
+from pathlib import Path
+
+
+class InferenceGenerator(Sequence):
+    def __init__(self, source_dir, batch_size, img_size, img_type):
+        self.source_dir = source_dir
+        self.batch_size = batch_size
+        self.img_size = img_size
+        self.img_type = img_type
+        filenames = DataSource.parse_directory(source_dir)
+        self.filenames = [v for key, val in filenames.items() for v in val]
+
+    def __data_generation(self, filenames):
+        images = []
+        for filename in filenames:
+            image = DataSource.load_image(filename, self.img_size, self.img_type)
+            image = DataSource.preprocess_image(image)
+            images.append(image)
+        return filenames, np.asarray(images)
+
+    def __getitem__(self, index):
+        batch_filenames = self.filenames[index * self.batch_size:(index + 1) * self.batch_size]
+        filenames_and_images = self.__data_generation(batch_filenames)
+        return filenames_and_images
+
+    def __len__(self):
+        return int(np.ceil(len(self.filenames) / self.batch_size))
+
+
+def load_from_frozen(source: str,
+                     input_tensor="input_1:0",
+                     output_tensor="conv2d_23/Sigmoid:0",
+                     session=None):
+    if not os.path.exists(source):
+        raise FileNotFoundError('The graph file was not found on the system.\nThe path was: ' + source)
+    # Load network
+    if session is None:
+        session = K.get_session()
+    with gfile.Open(source, 'rb') as f:
+        graph_def = tf.GraphDef()
+        graph_def.ParseFromString(f.read())
+        session.graph.as_default()
+        tf.import_graph_def(graph_def, name='')
+    input = session.graph.get_tensor_by_name(input_tensor)
+    output = session.graph.get_tensor_by_name(output_tensor)
+    return session, input, output
+
+
+def load_from_xml(filename, session=None):
+    project = ET.parse(filename).getroot()
+
+    protobuf = project.find('protobuf').text
+    print("protobuf: " + protobuf)
+
+    input = None
+    output = None
+    img_size = np.zeros(3, dtype=np.int)
+    cls_labels = []
+
+    list_xml = project.find('labels')
+    for i, entry_xml  in enumerate(list_xml.iter('label')):
+        code = entry_xml.find('code').text
+        cls_labels.append(code)
+
+    list_xml = project.find('inputs')
+    for i, entry_xml in enumerate(list_xml.iter('input')):
+        if i == 0:
+            input_name = entry_xml.find('operation').text + ":0"
+            img_size[0] = int(entry_xml.find('height').text)
+            img_size[1] = int(entry_xml.find('width').text)
+            img_size[2] = int(entry_xml.find('channels').text)
+
+    list_xml = project.find('outputs')
+    for i, entry_xml in enumerate(list_xml.iter('output')):
+        if i == 0:
+            output_name = entry_xml.find('operation').text + ":0"
+
+    full_protobuf_path = os.path.join(os.path.dirname(filename), protobuf)
+    session, input, output = load_from_frozen(full_protobuf_path, input_name, output_name)
+    return session, input, output, img_size, cls_labels
+
+
+def process(network_info, images_dir, output_dir, threshold=0.8):
+    session, input_tensor, output_tensor, img_size, cls_labels = load_from_xml(network_info)
+    print("Input tensor: {}".format(input_tensor))
+    print("Output tensor: {}".format(output_tensor))
+    print("Image size: {}".format(img_size))
+    print("Classes: {}".format(cls_labels))
+    print()
+    print("Parsing source directory... (this can take some time)")
+    if img_size[2] == 3:
+        img_type = 'rgb'
+    else:
+        img_type = 'greyscale'
+    gen = InferenceGenerator(images_dir, 64, img_size, img_type)
+
+    print("Files: {}".format(len(gen.filenames)))
+    print("Batches: {}".format(len(gen)))
+
+    workers = np.min((multiprocessing.cpu_count(), 8))
+    print("Workers: {}".format(workers))
+    print()
+
+    filenames = []
+    cls_index = []
+    cls_names = []
+    score = []
+    enq = OrderedEnqueuer(gen, use_multiprocessing=True)
+    enq.start(workers=workers, max_queue_size=multiprocessing.cpu_count()*4)
+    output_generator = enq.get()
+    for i in range(len(gen)):
+        print("\r{} / {}".format(i, len(gen)), end='')
+        batch_filenames, batch_images = next(output_generator)
+        result = session.run(output_tensor, feed_dict={input_tensor: batch_images})
+        cls = np.argmax(result, axis=1)
+        scr = np.max(result, axis=1)
+        cls_name = [cls_labels[i] for i in cls]
+        filenames.extend(batch_filenames)
+        cls_index.extend(cls)
+        cls_names.extend(cls_name)
+        score.extend(scr)
+    enq.stop()
+    print()
+    print("Done")
+    print("See {} for results".format(output_dir))
+
+    parents = [Path(f).parent.name for f in filenames]
+    files = [Path(f).name for f in filenames]
+
+    df = pd.DataFrame(data={'filename': filenames, 'parent': parents, 'file': files, 'class': cls_names, 'class_index': cls_index, 'score': score})
+    os.makedirs(output_directory, exist_ok=True)
+    df.to_csv(os.path.join(output_dir, "inference.csv"))
+
+
+if __name__ == "__main__":
+    network_info = r"D:\Development\Microfossil\PaperExperiments\Paper1CNNForMicrofossil\MD972138\Output\MD972138_base_cyclic_8_20200410-173126\model\network_info.xml"
+    images_directory = r"D:\Datasets\Foraminifera\images_20200226_114546 Fifth with background"
+    output_directory = r"D:\output"
+    process(network_info, images_directory, output_directory)
+
```

### Comparing `miso2-3.0.3/miso/deploy/saving.py` & `miso2-3.0.4/miso/deploy/saving.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,221 +1,221 @@
-import os
-import shutil
-import tensorflow as tf
-from tensorflow.python.platform import gfile
-from tensorflow.python.tools import freeze_graph
-from miso.deploy.model_info import ModelInfo
-import tensorflow.keras.backend as K
-import tempfile
-import lxml.etree as ET
-import numpy as np
-import tf2onnx
-
-
-def remove(path):
-    """ param <path> could either be relative or absolute. """
-    if os.path.isfile(path):
-        os.remove(path)  # remove the file
-    elif os.path.isdir(path):
-        shutil.rmtree(path)  # remove dir and all contains
-    # else:
-    #     raise ValueError("file {} is not a file or dir.".format(path))
-
-
-def convert_to_inference_mode(model, model_factory):
-    # Trick to get around bugs in tensorflow 1.14.0
-    # https://github.com/tensorflow/tensorflow/issues/31331#issuecomment-518655879
-    with tempfile.TemporaryDirectory() as dirpath:
-        weights_filename = os.path.join(dirpath, "weights.h5")
-        model.save_weights(weights_filename)
-        K.clear_session()
-        K.set_learning_phase(0)
-        model = model_factory()
-        model.load_weights(weights_filename)
-        remove(weights_filename)
-    return model
-
-
-def convert_to_inference_mode_tf2(model, model_factory):
-    # Trick to get around bugs in tensorflow 1.14.0
-    # https://github.com/tensorflow/tensorflow/issues/31331#issuecomment-518655879
-    with tempfile.TemporaryDirectory() as dirpath:
-        weights_filename = os.path.join(dirpath, "weights.tf")
-        model.save_weights(weights_filename)
-        K.clear_session()
-        K.set_learning_phase(0)
-        model = model_factory()
-        model.load_weights(weights_filename)
-        remove(weights_filename)
-    return model
-
-
-def save(model, save_dir):
-    tf.saved_model.simple_save(K.get_session(),
-                               save_dir,
-                               inputs={"input": model.inputs[0]},
-                               outputs={"output": model.outputs[0]})
-
-
-def freeze(model, save_dir):
-    # if metadata is not None:
-    #     metadata_tensor = K.constant(metadata.to_xml(), name="metadata", dtype='string')
-    #     model = Model(model.inputs[0], [model.outputs[0], metadata_tensor])
-    # K.set_learning_phase(0)
-
-    # Save using simple save
-    save(model, save_dir)
-    freeze_graph.freeze_graph(None,
-                              None,
-                              None,
-                              None,
-                              model.outputs[0].op.name,
-                              None,
-                              None,
-                              os.path.join(save_dir, "frozen_model.pb"),
-                              False,
-                              "",
-                              input_saved_model_dir=save_dir)
-    # Delete saved models
-    remove(os.path.join(save_dir, "saved_model.pb"))
-    remove(os.path.join(save_dir, "variables"))
-
-def load_frozen_model(source: str,
-                      input_tensor="input_1:0",
-                      output_tensor="conv2d_23/Sigmoid:0",
-                      session=None):
-    if not os.path.exists(source):
-        raise FileNotFoundError('The graph file was not found on the system.\nThe path was: ' + source)
-    # Load network
-    if session is None:
-        session = K.get_session()
-    with gfile.Open(source, 'rb') as f:
-        graph_def = tf.compat.v1.GraphDef()
-        graph_def.ParseFromString(f.read())
-        session.graph.as_default()
-        tf.import_graph_def(graph_def, name='')
-    # Information
-    # names = [n.name for n in tf.get_default_graph().as_graph_def().node]
-    # for n in names:
-    #     print(n)
-    # Input / output tensors
-    input = session.graph.get_tensor_by_name(input_tensor)
-    output = session.graph.get_tensor_by_name(output_tensor)
-    return session, input, output
-
-
-def load_from_xml(filename, session=None):
-    project = ET.parse(filename).getroot()
-
-    protobuf = project.find('protobuf').text
-    print("protobuf: " + protobuf)
-
-    input = None
-    output = None
-    img_size = np.zeros(3, dtype=np.int32)
-    cls_labels = []
-
-    list_xml = project.find('labels')
-    for i, entry_xml in enumerate(list_xml.iter('label')):
-        code = entry_xml.find('code').text
-        cls_labels.append(code)
-
-    list_xml = project.find('inputs')
-    for i, entry_xml in enumerate(list_xml.iter('input')):
-        if i == 0:
-            input_name = entry_xml.find('operation').text + ":0"
-            img_size[0] = int(entry_xml.find('height').text)
-            img_size[1] = int(entry_xml.find('width').text)
-            img_size[2] = int(entry_xml.find('channels').text)
-
-    list_xml = project.find('outputs')
-    for i, entry_xml in enumerate(list_xml.iter('output')):
-        if i == 0:
-            output_name = entry_xml.find('operation').text + ":0"
-
-    full_protobuf_path = os.path.join(os.path.dirname(filename), protobuf)
-    if int(tf.__version__[0]) == 2:
-        model = load_frozen_model_tf2(full_protobuf_path, input_name, output_name)
-        return model, img_size, cls_labels
-    else:
-        session, input, output = load_frozen_model(full_protobuf_path, input_name, output_name)
-        return session, input, output, img_size, cls_labels
-
-
-
-"""
-Adapted from https://leimao.github.io/blog/Save-Load-Inference-From-TF2-Frozen-Graph/
-"""
-from tensorflow.python.framework.convert_to_constants import convert_variables_to_constants_v2
-
-
-def wrap_frozen_graph_tf2(graph_def, inputs, outputs, print_graph=False):
-    def _imports_graph_def():
-        tf.compat.v1.import_graph_def(graph_def, name="")
-
-    wrapped_import = tf.compat.v1.wrap_function(_imports_graph_def, [])
-    import_graph = wrapped_import.graph
-    if print_graph == True:
-        print("-" * 50)
-        print("Frozen model layers: ")
-        layers = [op.name for op in import_graph.get_operations()]
-        for layer in layers:
-            print(layer)
-        print("-" * 50)
-    return wrapped_import.prune(
-        tf.nest.map_structure(import_graph.as_graph_element, inputs),
-        tf.nest.map_structure(import_graph.as_graph_element, outputs))
-
-
-def save_frozen_model_tf2(model, out_dir, filename):
-    print("-" * 80)
-    print("Freezing model")
-    # Convert Keras model to ConcreteFunction
-    full_model = tf.function(lambda x: model(x))
-    full_model = full_model.get_concrete_function(
-        tf.TensorSpec(model.inputs[0].shape, model.inputs[0].dtype))
-
-    # Get frozen ConcreteFunction
-    frozen_func = convert_variables_to_constants_v2(full_model)
-    frozen_func.graph.as_graph_def()
-
-    # layers = [op.name for op in frozen_func.graph.get_operations()]
-    # for layer in layers:
-    #     print(layer)
-
-    print("- model inputs: {}".format(frozen_func.inputs))
-    print("- model outputs: {}".format(frozen_func.outputs))
-
-    # Save frozen graph from frozen ConcreteFunction to hard drive
-    # logdir="./frozen_models",
-    print(out_dir)
-    print(filename)
-    tf.io.write_graph(graph_or_graph_def=frozen_func.graph,
-                      logdir=os.path.join(out_dir),
-                      name=filename,
-                      as_text=False)
-    return frozen_func
-
-
-def save_model_as_onnx(model, input_name, input_shape, out_dir, opset=13):
-    spec = (tf.TensorSpec(input_shape, tf.float32, name=input_name),)
-    output_path = os.path.join(out_dir, "model.onnx")
-    model_proto, _ = tf2onnx.convert.from_keras(model, input_signature=spec, opset=opset, output_path=output_path)
-    output_names = [n.name for n in model_proto.graph.output]
-    print(output_names)
-
-
-def load_frozen_model_tf2(filepath, inputs, outputs):
-    with tf.io.gfile.GFile(filepath, "rb") as f:
-        graph_def = tf.compat.v1.GraphDef()
-        loaded = graph_def.ParseFromString(f.read())
-    # Wrap frozen graph to ConcreteFunctions
-    frozen_func = wrap_frozen_graph_tf2(graph_def=graph_def,
-                                        inputs=inputs,
-                                        outputs=outputs,
-                                        print_graph=False)
-    print("-" * 80)
-    print("Frozen model inputs: ")
-    print(frozen_func.inputs)
-    print("Frozen model outputs: ")
-    print(frozen_func.outputs)
-    return frozen_func
+import os
+import shutil
+import tensorflow as tf
+from tensorflow.python.platform import gfile
+from tensorflow.python.tools import freeze_graph
+from miso.deploy.model_info import ModelInfo
+import tensorflow.keras.backend as K
+import tempfile
+import lxml.etree as ET
+import numpy as np
+import tf2onnx
+
+
+def remove(path):
+    """ param <path> could either be relative or absolute. """
+    if os.path.isfile(path):
+        os.remove(path)  # remove the file
+    elif os.path.isdir(path):
+        shutil.rmtree(path)  # remove dir and all contains
+    # else:
+    #     raise ValueError("file {} is not a file or dir.".format(path))
+
+
+def convert_to_inference_mode(model, model_factory):
+    # Trick to get around bugs in tensorflow 1.14.0
+    # https://github.com/tensorflow/tensorflow/issues/31331#issuecomment-518655879
+    with tempfile.TemporaryDirectory() as dirpath:
+        weights_filename = os.path.join(dirpath, "weights.h5")
+        model.save_weights(weights_filename)
+        K.clear_session()
+        K.set_learning_phase(0)
+        model = model_factory()
+        model.load_weights(weights_filename)
+        remove(weights_filename)
+    return model
+
+
+def convert_to_inference_mode_tf2(model, model_factory):
+    # Trick to get around bugs in tensorflow 1.14.0
+    # https://github.com/tensorflow/tensorflow/issues/31331#issuecomment-518655879
+    with tempfile.TemporaryDirectory() as dirpath:
+        weights_filename = os.path.join(dirpath, "weights.tf")
+        model.save_weights(weights_filename)
+        K.clear_session()
+        K.set_learning_phase(0)
+        model = model_factory()
+        model.load_weights(weights_filename)
+        remove(weights_filename)
+    return model
+
+
+def save(model, save_dir):
+    tf.saved_model.simple_save(K.get_session(),
+                               save_dir,
+                               inputs={"input": model.inputs[0]},
+                               outputs={"output": model.outputs[0]})
+
+
+def freeze(model, save_dir):
+    # if metadata is not None:
+    #     metadata_tensor = K.constant(metadata.to_xml(), name="metadata", dtype='string')
+    #     model = Model(model.inputs[0], [model.outputs[0], metadata_tensor])
+    # K.set_learning_phase(0)
+
+    # Save using simple save
+    save(model, save_dir)
+    freeze_graph.freeze_graph(None,
+                              None,
+                              None,
+                              None,
+                              model.outputs[0].op.name,
+                              None,
+                              None,
+                              os.path.join(save_dir, "frozen_model.pb"),
+                              False,
+                              "",
+                              input_saved_model_dir=save_dir)
+    # Delete saved models
+    remove(os.path.join(save_dir, "saved_model.pb"))
+    remove(os.path.join(save_dir, "variables"))
+
+def load_frozen_model(source: str,
+                      input_tensor="input_1:0",
+                      output_tensor="conv2d_23/Sigmoid:0",
+                      session=None):
+    if not os.path.exists(source):
+        raise FileNotFoundError('The graph file was not found on the system.\nThe path was: ' + source)
+    # Load network
+    if session is None:
+        session = K.get_session()
+    with gfile.Open(source, 'rb') as f:
+        graph_def = tf.compat.v1.GraphDef()
+        graph_def.ParseFromString(f.read())
+        session.graph.as_default()
+        tf.import_graph_def(graph_def, name='')
+    # Information
+    # names = [n.name for n in tf.get_default_graph().as_graph_def().node]
+    # for n in names:
+    #     print(n)
+    # Input / output tensors
+    input = session.graph.get_tensor_by_name(input_tensor)
+    output = session.graph.get_tensor_by_name(output_tensor)
+    return session, input, output
+
+
+def load_from_xml(filename, session=None):
+    project = ET.parse(filename).getroot()
+
+    protobuf = project.find('protobuf').text
+    print("protobuf: " + protobuf)
+
+    input = None
+    output = None
+    img_size = np.zeros(3, dtype=np.int32)
+    cls_labels = []
+
+    list_xml = project.find('labels')
+    for i, entry_xml in enumerate(list_xml.iter('label')):
+        code = entry_xml.find('code').text
+        cls_labels.append(code)
+
+    list_xml = project.find('inputs')
+    for i, entry_xml in enumerate(list_xml.iter('input')):
+        if i == 0:
+            input_name = entry_xml.find('operation').text + ":0"
+            img_size[0] = int(entry_xml.find('height').text)
+            img_size[1] = int(entry_xml.find('width').text)
+            img_size[2] = int(entry_xml.find('channels').text)
+
+    list_xml = project.find('outputs')
+    for i, entry_xml in enumerate(list_xml.iter('output')):
+        if i == 0:
+            output_name = entry_xml.find('operation').text + ":0"
+
+    full_protobuf_path = os.path.join(os.path.dirname(filename), protobuf)
+    if int(tf.__version__[0]) == 2:
+        model = load_frozen_model_tf2(full_protobuf_path, input_name, output_name)
+        return model, img_size, cls_labels
+    else:
+        session, input, output = load_frozen_model(full_protobuf_path, input_name, output_name)
+        return session, input, output, img_size, cls_labels
+
+
+
+"""
+Adapted from https://leimao.github.io/blog/Save-Load-Inference-From-TF2-Frozen-Graph/
+"""
+from tensorflow.python.framework.convert_to_constants import convert_variables_to_constants_v2
+
+
+def wrap_frozen_graph_tf2(graph_def, inputs, outputs, print_graph=False):
+    def _imports_graph_def():
+        tf.compat.v1.import_graph_def(graph_def, name="")
+
+    wrapped_import = tf.compat.v1.wrap_function(_imports_graph_def, [])
+    import_graph = wrapped_import.graph
+    if print_graph == True:
+        print("-" * 50)
+        print("Frozen model layers: ")
+        layers = [op.name for op in import_graph.get_operations()]
+        for layer in layers:
+            print(layer)
+        print("-" * 50)
+    return wrapped_import.prune(
+        tf.nest.map_structure(import_graph.as_graph_element, inputs),
+        tf.nest.map_structure(import_graph.as_graph_element, outputs))
+
+
+def save_frozen_model_tf2(model, out_dir, filename):
+    print("-" * 80)
+    print("Freezing model")
+    # Convert Keras model to ConcreteFunction
+    full_model = tf.function(lambda x: model(x))
+    full_model = full_model.get_concrete_function(
+        tf.TensorSpec(model.inputs[0].shape, model.inputs[0].dtype))
+
+    # Get frozen ConcreteFunction
+    frozen_func = convert_variables_to_constants_v2(full_model)
+    frozen_func.graph.as_graph_def()
+
+    # layers = [op.name for op in frozen_func.graph.get_operations()]
+    # for layer in layers:
+    #     print(layer)
+
+    print("- model inputs: {}".format(frozen_func.inputs))
+    print("- model outputs: {}".format(frozen_func.outputs))
+
+    # Save frozen graph from frozen ConcreteFunction to hard drive
+    # logdir="./frozen_models",
+    print(out_dir)
+    print(filename)
+    tf.io.write_graph(graph_or_graph_def=frozen_func.graph,
+                      logdir=os.path.join(out_dir),
+                      name=filename,
+                      as_text=False)
+    return frozen_func
+
+
+def save_model_as_onnx(model, input_name, input_shape, out_dir, opset=13):
+    spec = (tf.TensorSpec(input_shape, tf.float32, name=input_name),)
+    output_path = os.path.join(out_dir, "model.onnx")
+    model_proto, _ = tf2onnx.convert.from_keras(model, input_signature=spec, opset=opset, output_path=output_path)
+    output_names = [n.name for n in model_proto.graph.output]
+    print(output_names)
+
+
+def load_frozen_model_tf2(filepath, inputs, outputs):
+    with tf.io.gfile.GFile(filepath, "rb") as f:
+        graph_def = tf.compat.v1.GraphDef()
+        loaded = graph_def.ParseFromString(f.read())
+    # Wrap frozen graph to ConcreteFunctions
+    frozen_func = wrap_frozen_graph_tf2(graph_def=graph_def,
+                                        inputs=inputs,
+                                        outputs=outputs,
+                                        print_graph=False)
+    print("-" * 80)
+    print("Frozen model inputs: ")
+    print(frozen_func.inputs)
+    print("Frozen model outputs: ")
+    print(frozen_func.outputs)
+    return frozen_func
```

### Comparing `miso2-3.0.3/miso/deploy/server.py` & `miso2-3.0.4/miso/deploy/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,322 +1,330 @@
-00000000: 696d 706f 7274 2061 7267 7061 7273 650a  import argparse.
-00000010: 6672 6f6d 2066 6c61 736b 2069 6d70 6f72  from flask impor
-00000020: 7420 466c 6173 6b2c 2072 6571 7565 7374  t Flask, request
-00000030: 2c20 666c 6173 680a 696d 706f 7274 206e  , flash.import n
-00000040: 756d 7079 2061 7320 6e70 0a66 726f 6d20  umpy as np.from 
-00000050: 6d69 736f 2e64 6174 612e 696d 6167 655f  miso.data.image_
-00000060: 7574 696c 7320 696d 706f 7274 206c 6f61  utils import loa
-00000070: 645f 696d 6167 650a 6672 6f6d 206d 6973  d_image.from mis
-00000080: 6f2e 6465 706c 6f79 2e73 6176 696e 6720  o.deploy.saving 
-00000090: 696d 706f 7274 206c 6f61 645f 6672 6f6d  import load_from
-000000a0: 5f78 6d6c 0a69 6d70 6f72 7420 7379 730a  _xml.import sys.
-000000b0: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
-000000c0: 2070 640a 696d 706f 7274 2074 656e 736f   pd.import tenso
-000000d0: 7266 6c6f 7720 6173 2074 660a 0a74 665f  rflow as tf..tf_
-000000e0: 7665 7273 696f 6e20 3d20 696e 7428 7466  version = int(tf
-000000f0: 2e5f 5f76 6572 7369 6f6e 5f5f 5b30 5d29  .__version__[0])
-00000100: 0a61 7070 203d 2046 6c61 736b 285f 5f6e  .app = Flask(__n
-00000110: 616d 655f 5f29 0a0a 0a40 6170 702e 726f  ame__)...@app.ro
-00000120: 7574 6528 272f 2729 0a64 6566 2069 6e64  ute('/').def ind
-00000130: 6578 2829 3a0a 2020 2020 7265 7475 726e  ex():.    return
-00000140: 2027 2727 0a20 2020 203c 2164 6f63 7479   '''.    <!docty
-00000150: 7065 2068 746d 6c3e 0a20 2020 203c 7469  pe html>.    <ti
-00000160: 746c 653e 4d49 534f 2043 6c61 7373 6966  tle>MISO Classif
-00000170: 6963 6174 696f 6e20 5365 7276 6572 3c2f  ication Server</
-00000180: 7469 746c 653e 0a20 2020 203c 6831 3e4d  title>.    <h1>M
-00000190: 4953 4f20 436c 6173 7369 6669 6361 7469  ISO Classificati
-000001a0: 6f6e 2053 6572 7665 723c 2f68 313e 0a20  on Server</h1>. 
-000001b0: 2020 203c 6832 3e43 6c61 7373 6966 6963     <h2>Classific
-000001c0: 6174 696f 6e3c 2f68 323e 0a20 2020 203c  ation</h2>.    <
-000001d0: 703e 5573 6520 7468 6520 3c61 2068 7265  p>Use the <a hre
-000001e0: 663d 222f 6669 6c65 223e 6669 6c65 3c2f  f="/file">file</
-000001f0: 613e 2065 6e64 2070 6f69 6e74 2074 6f20  a> end point to 
-00000200: 636c 6173 7369 6679 2061 6e20 696d 6167  classify an imag
-00000210: 653c 2f70 3e0a 2020 2020 3c70 3e55 7365  e</p>.    <p>Use
-00000220: 2074 6865 203c 6120 6872 6566 3d22 2f63   the <a href="/c
-00000230: 6f75 6e74 223e 636f 756e 743c 2f61 3e20  ount">count</a> 
-00000240: 656e 6420 706f 696e 7420 746f 2067 6574  end point to get
-00000250: 2074 6865 2063 6c61 7373 2063 6f75 6e74   the class count
-00000260: 733c 2f70 3e0a 2020 2020 2727 270a 0a0a  s</p>.    '''...
-00000270: 4061 7070 2e72 6f75 7465 2827 2f63 6f75  @app.route('/cou
-00000280: 6e74 272c 206d 6574 686f 6473 3d5b 2747  nt', methods=['G
-00000290: 4554 275d 290a 6465 6620 636f 756e 7473  ET']).def counts
-000002a0: 2829 3a0a 2020 2020 6966 2072 6571 7565  ():.    if reque
-000002b0: 7374 2e6d 6574 686f 6420 3d3d 2027 4745  st.method == 'GE
-000002c0: 5427 3a0a 2020 2020 2020 2020 6966 2027  T':.        if '
-000002d0: 666f 726d 6174 2720 696e 2072 6571 7565  format' in reque
-000002e0: 7374 2e61 7267 7320 616e 6420 7265 7175  st.args and requ
-000002f0: 6573 742e 6172 6773 5b27 666f 726d 6174  est.args['format
-00000300: 275d 203d 3d20 2763 7376 273a 0a20 2020  '] == 'csv':.   
-00000310: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000320: 6170 705f 6466 2e74 6f5f 6373 7628 290a  app_df.to_csv().
-00000330: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00000340: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00000350: 2061 7070 5f64 662e 746f 5f6a 736f 6e28   app_df.to_json(
-00000360: 290a 0a0a 4061 7070 2e72 6f75 7465 2827  )...@app.route('
-00000370: 2f66 696c 6527 2c20 6d65 7468 6f64 733d  /file', methods=
-00000380: 5b27 4745 5427 5d29 0a64 6566 2063 6c61  ['GET']).def cla
-00000390: 7373 6966 795f 6669 6c65 2829 3a0a 2020  ssify_file():.  
-000003a0: 2020 676c 6f62 616c 2061 7070 5f64 660a    global app_df.
-000003b0: 2020 2020 6966 2072 6571 7565 7374 2e6d      if request.m
-000003c0: 6574 686f 6420 3d3d 2027 4745 5427 3a0a  ethod == 'GET':.
-000003d0: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
-000003e0: 6966 2074 6865 2070 6f73 7420 7265 7175  if the post requ
-000003f0: 6573 7420 6861 7320 7468 6520 6669 6c65  est has the file
-00000400: 2070 6172 740a 2020 2020 2020 2020 7072   part.        pr
-00000410: 696e 7428 2243 6c61 7373 6966 6963 6174  int("Classificat
-00000420: 696f 6e20 7265 7175 6573 743a 2229 0a20  ion request:"). 
-00000430: 2020 2020 2020 2069 6620 2766 696c 656e         if 'filen
-00000440: 616d 6527 206e 6f74 2069 6e20 7265 7175  ame' not in requ
-00000450: 6573 742e 6172 6773 3a0a 2020 2020 2020  est.args:.      
-00000460: 2020 2020 2020 7072 696e 7428 222d 206e        print("- n
-00000470: 6f20 6669 6c65 6e61 6d65 2c20 7365 7276  o filename, serv
-00000480: 696e 6720 7765 6270 6167 6520 696e 7374  ing webpage inst
-00000490: 6561 642e 2e2e 2229 0a20 2020 2020 2020  ead...").       
-000004a0: 2020 2020 2072 6574 7572 6e20 2727 270a       return '''.
-000004b0: 2020 2020 2020 2020 2020 2020 3c21 646f              <!do
-000004c0: 6374 7970 6520 6874 6d6c 3e0a 2020 2020  ctype html>.    
-000004d0: 2020 2020 2020 2020 3c74 6974 6c65 3e49          <title>I
-000004e0: 6d70 6f72 7420 6669 6c65 3c2f 7469 746c  mport file</titl
-000004f0: 653e 0a20 2020 2020 2020 2020 2020 203c  e>.            <
-00000500: 6831 3e49 6d70 6f72 7420 616e 6420 636c  h1>Import and cl
-00000510: 6173 7369 6679 2061 2070 6172 7469 636c  assify a particl
-00000520: 6520 696d 6167 653c 2f68 313e 0a20 2020  e image</h1>.   
-00000530: 2020 2020 2020 2020 203c 703e 456e 7465           <p>Ente
-00000540: 7220 7468 6520 6675 6c6c 2066 696c 6520  r the full file 
-00000550: 7061 7468 2074 6f20 696d 706f 7274 2074  path to import t
-00000560: 6865 2069 6d61 6765 2061 6e64 2063 6c61  he image and cla
-00000570: 7373 6966 7920 6974 3c2f 703e 0a20 2020  ssify it</p>.   
-00000580: 2020 2020 2020 2020 203c 666f 726d 206d           <form m
-00000590: 6574 686f 643d 2247 4554 223e 0a20 2020  ethod="GET">.   
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 2046 696c 6520 7061 7468 3a3c 2f62 723e   File path:</br>
-000005c0: 0a20 2020 2020 2020 2020 2020 203c 696e  .            <in
-000005d0: 7075 7420 7479 7065 3d74 6578 7420 6e61  put type=text na
-000005e0: 6d65 3d66 696c 656e 616d 653e 0a20 2020  me=filename>.   
-000005f0: 2020 2020 2020 2020 203c 2f62 723e 0a20           </br>. 
-00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 2020 2053 616d 706c 653a 3c2f 6272 3e0a     Sample:</br>.
-00000620: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
-00000630: 7574 2074 7970 653d 7465 7874 206e 616d  ut type=text nam
-00000640: 653d 7361 6d70 6c65 3e0a 2020 2020 2020  e=sample>.      
-00000650: 2020 2020 2020 3c2f 6272 3e0a 2020 2020        </br>.    
-00000660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000670: 496e 6465 7820 313a 3c2f 6272 3e0a 2020  Index 1:</br>.  
-00000680: 2020 2020 2020 2020 2020 3c69 6e70 7574            <input
-00000690: 2074 7970 653d 7465 7874 206e 616d 653d   type=text name=
-000006a0: 696e 6465 7831 3e0a 2020 2020 2020 2020  index1>.        
-000006b0: 2020 2020 3c2f 6272 3e0a 2020 2020 2020      </br>.      
-000006c0: 2020 2020 2020 2020 2020 2020 2020 496e                In
-000006d0: 6465 7820 323a 3c2f 6272 3e0a 2020 2020  dex 2:</br>.    
-000006e0: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
-000006f0: 7970 653d 7465 7874 206e 616d 653d 696e  ype=text name=in
-00000700: 6465 7832 3e0a 2020 2020 2020 2020 2020  dex2>.          
-00000710: 2020 3c2f 6272 3e0a 2020 2020 2020 2020    </br>.        
-00000720: 2020 2020 2020 2020 2020 2020 5265 736f              Reso
-00000730: 6c75 7469 6f6e 2028 7069 7865 6c73 2f6d  lution (pixels/m
-00000740: 6d29 3a3c 2f62 723e 0a20 2020 2020 2020  m):</br>.       
-00000750: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
-00000760: 3d74 6578 7420 6e61 6d65 3d72 6573 6f6c  =text name=resol
-00000770: 7574 696f 6e3e 0a20 2020 2020 2020 2020  ution>.         
-00000780: 2020 2020 2020 2020 2020 203c 2f62 723e             </br>
-00000790: 0a20 2020 2020 2020 2020 2020 203c 696e  .            <in
-000007a0: 7075 7420 7479 7065 3d73 7562 6d69 7420  put type=submit 
-000007b0: 7661 6c75 653d 5570 6c6f 6164 3e0a 2020  value=Upload>.  
-000007c0: 2020 2020 2020 2020 2020 3c2f 666f 726d            </form
-000007d0: 3e27 2727 0a20 2020 2020 2020 2065 6c73  >'''.        els
-000007e0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-000007f0: 696c 656e 616d 6520 3d20 7265 7175 6573  ilename = reques
-00000800: 742e 6172 6773 5b27 6669 6c65 6e61 6d65  t.args['filename
-00000810: 275d 0a20 2020 2020 2020 2020 2020 2073  '].            s
-00000820: 616d 706c 6520 3d20 7265 7175 6573 742e  ample = request.
-00000830: 6172 6773 5b27 7361 6d70 6c65 275d 0a20  args['sample']. 
-00000840: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-00000850: 3120 3d20 7265 7175 6573 742e 6172 6773  1 = request.args
-00000860: 5b27 696e 6465 7831 275d 0a20 2020 2020  ['index1'].     
-00000870: 2020 2020 2020 2069 6e64 6578 3220 3d20         index2 = 
-00000880: 7265 7175 6573 742e 6172 6773 5b27 696e  request.args['in
-00000890: 6465 7832 275d 0a20 2020 2020 2020 2020  dex2'].         
-000008a0: 2020 2072 6573 6f6c 7574 696f 6e20 3d20     resolution = 
-000008b0: 7265 7175 6573 742e 6172 6773 5b27 7265  request.args['re
-000008c0: 736f 6c75 7469 6f6e 275d 0a20 2020 2020  solution'].     
-000008d0: 2020 2020 2020 2070 7269 6e74 2866 2220         print(f" 
-000008e0: 2d20 6669 6c65 6e61 6d65 3a20 2020 7b66  - filename:   {f
-000008f0: 696c 656e 616d 657d 2229 0a20 2020 2020  ilename}").     
-00000900: 2020 2020 2020 2070 7269 6e74 2866 2220         print(f" 
-00000910: 2d20 7361 6d70 6c65 3a20 2020 2020 7b73  - sample:     {s
-00000920: 616d 706c 657d 2229 0a20 2020 2020 2020  ample}").       
-00000930: 2020 2020 2070 7269 6e74 2866 2220 2d20       print(f" - 
-00000940: 696e 6465 7831 3a20 2020 2020 7b69 6e64  index1:     {ind
-00000950: 6578 317d 2229 0a20 2020 2020 2020 2020  ex1}").         
-00000960: 2020 2070 7269 6e74 2866 2220 2d20 696e     print(f" - in
-00000970: 6465 7832 3a20 2020 2020 7b69 6e64 6578  dex2:     {index
-00000980: 327d 2229 0a20 2020 2020 2020 2020 2020  2}").           
-00000990: 2070 7269 6e74 2866 2220 2d20 7265 736f   print(f" - reso
-000009a0: 6c75 7469 6f6e 3a20 7b72 6573 6f6c 7574  lution: {resolut
-000009b0: 696f 6e7d 2229 0a0a 2020 2020 2020 2020  ion}")..        
-000009c0: 2020 2020 6966 2066 696c 656e 616d 6520      if filename 
-000009d0: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
-000009e0: 2020 2020 2020 2066 6c61 7368 2827 7b22         flash('{"
-000009f0: 6572 726f 7222 3a22 4e6f 2066 696c 656e  error":"No filen
-00000a00: 616d 6520 7761 7320 656e 7465 7265 6422  ame was entered"
-00000a10: 7d27 290a 2020 2020 2020 2020 2020 2020  }').            
-00000a20: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00000a30: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00000a40: 2020 2020 2020 2020 2020 2020 2320 4c6f              # Lo
-00000a50: 6164 2069 6d61 6765 0a20 2020 2020 2020  ad image.       
-00000a60: 2020 2020 2020 2020 2069 6620 6170 705f           if app_
-00000a70: 696d 675f 7369 7a65 5b32 5d20 3d3d 2031  img_size[2] == 1
-00000a80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000a90: 2020 2020 2020 696d 675f 7479 7065 203d        img_type =
-00000aa0: 2027 7267 6d27 0a20 2020 2020 2020 2020   'rgm'.         
-00000ab0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ad0: 2069 6d67 5f74 7970 6520 3d20 2767 7265   img_type = 'gre
-00000ae0: 7973 6361 6c65 270a 2020 2020 2020 2020  yscale'.        
-00000af0: 2020 2020 2020 2020 696d 203d 206c 6f61          im = loa
-00000b00: 645f 696d 6167 6528 6669 6c65 6e61 6d65  d_image(filename
-00000b10: 2c20 6170 705f 696d 675f 7369 7a65 2c20  , app_img_size, 
-00000b20: 696d 675f 7479 7065 290a 0a20 2020 2020  img_type)..     
-00000b30: 2020 2020 2020 2020 2020 2023 2043 6c61             # Cla
-00000b40: 7373 6966 790a 2020 2020 2020 2020 2020  ssify.          
-00000b50: 2020 2020 2020 6966 2074 665f 7665 7273        if tf_vers
-00000b60: 696f 6e20 3d3d 2032 3a0a 2020 2020 2020  ion == 2:.      
-00000b70: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00000b80: 7375 6c74 203d 2061 7070 5f6d 6f64 656c  sult = app_model
-00000b90: 2874 662e 636f 6e76 6572 745f 746f 5f74  (tf.convert_to_t
-00000ba0: 656e 736f 7228 696d 5b6e 702e 6e65 7761  ensor(im[np.newa
-00000bb0: 7869 732c 203a 2c20 3a2c 203a 5d2c 2064  xis, :, :, :], d
-00000bc0: 7479 7065 3d74 662e 666c 6f61 7433 3229  type=tf.float32)
-00000bd0: 292e 6e75 6d70 7928 295b 305d 0a20 2020  ).numpy()[0].   
-00000be0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00000bf0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00000c00: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00000c10: 6170 705f 7365 7373 696f 6e2e 7275 6e28  app_session.run(
-00000c20: 6170 705f 6f75 7470 7574 2c20 6665 6564  app_output, feed
-00000c30: 5f64 6963 743d 7b61 7070 5f69 6e70 7574  _dict={app_input
-00000c40: 3a20 696d 5b6e 702e 6e65 7761 7869 732c  : im[np.newaxis,
-00000c50: 203a 2c20 3a2c 203a 5d7d 290a 0a20 2020   :, :, :]})..   
-00000c60: 2020 2020 2020 2020 2020 2020 2023 2050               # P
-00000c70: 7265 6469 6374 696f 6e73 0a20 2020 2020  redictions.     
-00000c80: 2020 2020 2020 2020 2020 2069 6478 203d             idx =
-00000c90: 206e 702e 6172 676d 6178 2872 6573 756c   np.argmax(resul
-00000ca0: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-00000cb0: 2020 2063 6f64 6520 3d20 6170 705f 636c     code = app_cl
-00000cc0: 735f 6c61 6265 6c73 5b69 6478 5d0a 2020  s_labels[idx].  
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00000ce0: 6f72 6520 3d20 6e70 2e6d 6178 2872 6573  ore = np.max(res
-00000cf0: 756c 7429 0a0a 2020 2020 2020 2020 2020  ult)..          
-00000d00: 2020 2020 2020 2320 466f 726d 6174 2072        # Format r
-00000d10: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
-00000d20: 2020 2020 2020 2020 7265 7375 6c74 5f73          result_s
-00000d30: 7472 203d 2022 7b7b 5c22 636f 6465 5c22  tr = "{{\"code\"
-00000d40: 3a5c 227b 7d5c 222c 205c 2273 636f 7265  :\"{}\", \"score
-00000d50: 5c22 3a7b 7d7d 7d22 2e66 6f72 6d61 7428  \":{}}}".format(
-00000d60: 636f 6465 2c20 7363 6f72 6529 0a20 2020  code, score).   
-00000d70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00000d80: 6c65 6e28 6170 705f 6466 2920 3d3d 2030  len(app_df) == 0
-00000d90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000da0: 2020 2020 2020 6170 705f 6466 203d 2061        app_df = a
-00000db0: 7070 5f64 662e 6170 7065 6e64 2870 642e  pp_df.append(pd.
-00000dc0: 5365 7269 6573 285b 7361 6d70 6c65 5d20  Series([sample] 
-00000dd0: 2b20 5b30 5d20 2a20 6c65 6e28 6170 705f  + [0] * len(app_
-00000de0: 636c 735f 6c61 6265 6c73 292c 2069 6e64  cls_labels), ind
-00000df0: 6578 3d61 7070 5f64 662e 636f 6c75 6d6e  ex=app_df.column
-00000e00: 7329 2c20 6967 6e6f 7265 5f69 6e64 6578  s), ignore_index
-00000e10: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00000e20: 2020 2020 2020 2020 2020 2061 7070 5f64             app_d
-00000e30: 662e 7365 745f 696e 6465 7828 2773 616d  f.set_index('sam
-00000e40: 706c 6527 2c20 696e 706c 6163 653d 5472  ple', inplace=Tr
-00000e50: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-00000e60: 2020 2020 656c 6966 2061 7070 5f64 662e      elif app_df.
-00000e70: 696e 6465 782e 7374 722e 636f 6e74 6169  index.str.contai
-00000e80: 6e73 2873 616d 706c 6529 2069 7320 4661  ns(sample) is Fa
-00000e90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00000ea0: 2020 2020 2020 2020 2061 7070 5f64 6620           app_df 
-00000eb0: 3d20 6170 705f 6466 2e61 7070 656e 6428  = app_df.append(
-00000ec0: 7064 2e53 6572 6965 7328 5b30 5d20 2a20  pd.Series([0] * 
-00000ed0: 6c65 6e28 6170 705f 636c 735f 6c61 6265  len(app_cls_labe
-00000ee0: 6c73 292c 206e 616d 653d 7361 6d70 6c65  ls), name=sample
-00000ef0: 2c20 696e 6465 783d 6170 705f 6466 2e63  , index=app_df.c
-00000f00: 6f6c 756d 6e73 292c 2069 676e 6f72 655f  olumns), ignore_
-00000f10: 696e 6465 783d 4661 6c73 6529 0a20 2020  index=False).   
-00000f20: 2020 2020 2020 2020 2020 2020 2061 7070               app
-00000f30: 5f64 662e 6c6f 635b 7361 6d70 6c65 5d5b  _df.loc[sample][
-00000f40: 6964 785d 203d 2061 7070 5f64 662e 6c6f  idx] = app_df.lo
-00000f50: 635b 7361 6d70 6c65 5d5b 6964 785d 202b  c[sample][idx] +
-00000f60: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
-00000f70: 2020 2070 7269 6e74 2822 5265 7375 6c74     print("Result
-00000f80: 735c 6e20 2d20 636f 6465 3a20 7b7d 5c6e  s\n - code: {}\n
-00000f90: 202d 2073 636f 7265 3a20 7b7d 222e 666f   - score: {}".fo
-00000fa0: 726d 6174 2866 696c 656e 616d 652c 2063  rmat(filename, c
-00000fb0: 6f64 652c 2073 636f 7265 2929 0a20 2020  ode, score)).   
-00000fc0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00000fd0: 7572 6e20 7265 7375 6c74 5f73 7472 0a20  urn result_str. 
-00000fe0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00000ff0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00001000: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001010: 2020 2320 4572 726f 730a 2020 2020 2020    # Erros.      
-00001020: 2020 2020 2020 2020 2020 6578 635f 7479            exc_ty
-00001030: 7065 2c20 6578 635f 6f62 6a2c 2065 7863  pe, exc_obj, exc
-00001040: 5f74 6220 3d20 7379 732e 6578 635f 696e  _tb = sys.exc_in
-00001050: 666f 2829 0a20 2020 2020 2020 2020 2020  fo().           
-00001060: 2020 2020 2070 7269 6e74 2822 4578 6365       print("Exce
-00001070: 7074 696f 6e20 6f6e 206c 696e 653a 207b  ption on line: {
-00001080: 7d22 2e66 6f72 6d61 7428 6578 635f 7462  }".format(exc_tb
-00001090: 2e74 625f 6c69 6e65 6e6f 2929 0a20 2020  .tb_lineno)).   
-000010a0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000010b0: 6e74 2865 290a 2020 2020 2020 2020 2020  nt(e).          
-000010c0: 2020 2020 2020 7265 7375 6c74 5f73 7472        result_str
-000010d0: 203d 2022 7b7b 5c22 6572 726f 725c 223a   = "{{\"error\":
-000010e0: 5c22 7b7d 5c22 7d7d 222e 666f 726d 6174  \"{}\"}}".format
-000010f0: 2865 290a 2020 2020 2020 2020 2020 2020  (e).            
-00001100: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00001110: 745f 7374 720a 0a0a 6966 205f 5f6e 616d  t_str...if __nam
-00001120: 655f 5f20 3d3d 2027 5f5f 6d61 696e 5f5f  e__ == '__main__
-00001130: 273a 0a20 2020 2070 6172 7365 7220 3d20  ':.    parser = 
-00001140: 6172 6770 6172 7365 2e41 7267 756d 656e  argparse.Argumen
-00001150: 7450 6172 7365 7228 224d 4953 4f20 436c  tParser("MISO Cl
-00001160: 6173 7369 6669 6361 7469 6f6e 2053 6572  assification Ser
-00001170: 7665 7222 290a 2020 2020 7061 7273 6572  ver").    parser
-00001180: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-00001190: 6922 2c20 222d 2d69 6e66 6f22 2c20 7265  i", "--info", re
-000011a0: 7175 6972 6564 3d54 7275 652c 2068 656c  quired=True, hel
-000011b0: 703d 2243 4e4e 206e 6574 776f 726b 2069  p="CNN network i
-000011c0: 6e66 6f72 6d61 7469 6f6e 2066 696c 6522  nformation file"
-000011d0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
-000011e0: 5f61 7267 756d 656e 7428 222d 7022 2c20  _argument("-p", 
-000011f0: 222d 2d70 6f72 7422 2c20 7265 7175 6972  "--port", requir
-00001200: 6564 3d54 7275 652c 2068 656c 703d 2253  ed=True, help="S
-00001210: 6572 7665 7220 706f 7274 2229 0a20 2020  erver port").   
-00001220: 2061 7267 7320 3d20 7061 7273 6572 2e70   args = parser.p
-00001230: 6172 7365 5f61 7267 7328 290a 0a20 2020  arse_args()..   
-00001240: 2069 6620 7466 5f76 6572 7369 6f6e 203d   if tf_version =
-00001250: 3d20 323a 0a20 2020 2020 2020 2061 7070  = 2:.        app
-00001260: 5f6d 6f64 656c 2c20 6170 705f 696d 675f  _model, app_img_
-00001270: 7369 7a65 2c20 6170 705f 636c 735f 6c61  size, app_cls_la
-00001280: 6265 6c73 203d 206c 6f61 645f 6672 6f6d  bels = load_from
-00001290: 5f78 6d6c 2861 7267 732e 696e 666f 290a  _xml(args.info).
-000012a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000012b0: 2020 6170 705f 7365 7373 696f 6e2c 2061    app_session, a
-000012c0: 7070 5f69 6e70 7574 2c20 6170 705f 6f75  pp_input, app_ou
-000012d0: 7470 7574 2c20 6170 705f 696d 675f 7369  tput, app_img_si
-000012e0: 7a65 2c20 6170 705f 636c 735f 6c61 6265  ze, app_cls_labe
-000012f0: 6c73 203d 206c 6f61 645f 6672 6f6d 5f78  ls = load_from_x
-00001300: 6d6c 2861 7267 732e 696e 666f 290a 2020  ml(args.info).  
-00001310: 2020 6170 705f 6466 203d 2070 642e 4461    app_df = pd.Da
-00001320: 7461 4672 616d 6528 636f 6c75 6d6e 733d  taFrame(columns=
-00001330: 5b27 7361 6d70 6c65 275d 202b 2061 7070  ['sample'] + app
-00001340: 5f63 6c73 5f6c 6162 656c 7329 0a20 2020  _cls_labels).   
-00001350: 2070 7269 6e74 2822 4d49 534f 2043 6c61   print("MISO Cla
-00001360: 7373 6966 6963 6174 696f 6e20 5365 7276  ssification Serv
-00001370: 6572 202d 2070 6f72 7420 7b7d 222e 666f  er - port {}".fo
-00001380: 726d 6174 2861 7267 732e 706f 7274 2929  rmat(args.port))
-00001390: 0a20 2020 2070 7269 6e74 2822 2d2d 2d2d  .    print("----
-000013a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013b0: 2d2d 2d2d 2d2d 2229 0a20 2020 2070 7269  ------").    pri
-000013c0: 6e74 2822 4c61 6265 6c73 3a22 290a 2020  nt("Labels:").  
-000013d0: 2020 7072 696e 7428 6170 705f 636c 735f    print(app_cls_
-000013e0: 6c61 6265 6c73 290a 2020 2020 6170 702e  labels).    app.
-000013f0: 7275 6e28 6465 6275 673d 4661 6c73 652c  run(debug=False,
-00001400: 2070 6f72 743d 6172 6773 2e70 6f72 7429   port=args.port)
-00001410: 0a0a 0a                                  ...
+00000000: 696d 706f 7274 2061 7267 7061 7273 650d  import argparse.
+00000010: 0a66 726f 6d20 666c 6173 6b20 696d 706f  .from flask impo
+00000020: 7274 2046 6c61 736b 2c20 7265 7175 6573  rt Flask, reques
+00000030: 742c 2066 6c61 7368 0d0a 696d 706f 7274  t, flash..import
+00000040: 206e 756d 7079 2061 7320 6e70 0d0a 6672   numpy as np..fr
+00000050: 6f6d 206d 6973 6f2e 6461 7461 2e69 6d61  om miso.data.ima
+00000060: 6765 5f75 7469 6c73 2069 6d70 6f72 7420  ge_utils import 
+00000070: 6c6f 6164 5f69 6d61 6765 0d0a 6672 6f6d  load_image..from
+00000080: 206d 6973 6f2e 6465 706c 6f79 2e73 6176   miso.deploy.sav
+00000090: 696e 6720 696d 706f 7274 206c 6f61 645f  ing import load_
+000000a0: 6672 6f6d 5f78 6d6c 0d0a 696d 706f 7274  from_xml..import
+000000b0: 2073 7973 0d0a 696d 706f 7274 2070 616e   sys..import pan
+000000c0: 6461 7320 6173 2070 640d 0a69 6d70 6f72  das as pd..impor
+000000d0: 7420 7465 6e73 6f72 666c 6f77 2061 7320  t tensorflow as 
+000000e0: 7466 0d0a 0d0a 7466 5f76 6572 7369 6f6e  tf....tf_version
+000000f0: 203d 2069 6e74 2874 662e 5f5f 7665 7273   = int(tf.__vers
+00000100: 696f 6e5f 5f5b 305d 290d 0a61 7070 203d  ion__[0])..app =
+00000110: 2046 6c61 736b 285f 5f6e 616d 655f 5f29   Flask(__name__)
+00000120: 0d0a 0d0a 0d0a 4061 7070 2e72 6f75 7465  ......@app.route
+00000130: 2827 2f27 290d 0a64 6566 2069 6e64 6578  ('/')..def index
+00000140: 2829 3a0d 0a20 2020 2072 6574 7572 6e20  ():..    return 
+00000150: 2727 270d 0a20 2020 203c 2164 6f63 7479  '''..    <!docty
+00000160: 7065 2068 746d 6c3e 0d0a 2020 2020 3c74  pe html>..    <t
+00000170: 6974 6c65 3e4d 4953 4f20 436c 6173 7369  itle>MISO Classi
+00000180: 6669 6361 7469 6f6e 2053 6572 7665 723c  fication Server<
+00000190: 2f74 6974 6c65 3e0d 0a20 2020 203c 6831  /title>..    <h1
+000001a0: 3e4d 4953 4f20 436c 6173 7369 6669 6361  >MISO Classifica
+000001b0: 7469 6f6e 2053 6572 7665 723c 2f68 313e  tion Server</h1>
+000001c0: 0d0a 2020 2020 3c68 323e 436c 6173 7369  ..    <h2>Classi
+000001d0: 6669 6361 7469 6f6e 3c2f 6832 3e0d 0a20  fication</h2>.. 
+000001e0: 2020 203c 703e 5573 6520 7468 6520 3c61     <p>Use the <a
+000001f0: 2068 7265 663d 222f 6669 6c65 223e 6669   href="/file">fi
+00000200: 6c65 3c2f 613e 2065 6e64 2070 6f69 6e74  le</a> end point
+00000210: 2074 6f20 636c 6173 7369 6679 2061 6e20   to classify an 
+00000220: 696d 6167 653c 2f70 3e0d 0a20 2020 203c  image</p>..    <
+00000230: 703e 5573 6520 7468 6520 3c61 2068 7265  p>Use the <a hre
+00000240: 663d 222f 636f 756e 7422 3e63 6f75 6e74  f="/count">count
+00000250: 3c2f 613e 2065 6e64 2070 6f69 6e74 2074  </a> end point t
+00000260: 6f20 6765 7420 7468 6520 636c 6173 7320  o get the class 
+00000270: 636f 756e 7473 3c2f 703e 0d0a 2020 2020  counts</p>..    
+00000280: 2727 270d 0a0d 0a0d 0a40 6170 702e 726f  '''......@app.ro
+00000290: 7574 6528 272f 636f 756e 7427 2c20 6d65  ute('/count', me
+000002a0: 7468 6f64 733d 5b27 4745 5427 5d29 0d0a  thods=['GET'])..
+000002b0: 6465 6620 636f 756e 7473 2829 3a0d 0a20  def counts():.. 
+000002c0: 2020 2069 6620 7265 7175 6573 742e 6d65     if request.me
+000002d0: 7468 6f64 203d 3d20 2747 4554 273a 0d0a  thod == 'GET':..
+000002e0: 2020 2020 2020 2020 6966 2027 666f 726d          if 'form
+000002f0: 6174 2720 696e 2072 6571 7565 7374 2e61  at' in request.a
+00000300: 7267 7320 616e 6420 7265 7175 6573 742e  rgs and request.
+00000310: 6172 6773 5b27 666f 726d 6174 275d 203d  args['format'] =
+00000320: 3d20 2763 7376 273a 0d0a 2020 2020 2020  = 'csv':..      
+00000330: 2020 2020 2020 7265 7475 726e 2061 7070        return app
+00000340: 5f64 662e 746f 5f63 7376 2829 0d0a 2020  _df.to_csv()..  
+00000350: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00000360: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000370: 6170 705f 6466 2e74 6f5f 6a73 6f6e 2829  app_df.to_json()
+00000380: 0d0a 0d0a 0d0a 4061 7070 2e72 6f75 7465  ......@app.route
+00000390: 2827 2f66 696c 6527 2c20 6d65 7468 6f64  ('/file', method
+000003a0: 733d 5b27 4745 5427 5d29 0d0a 6465 6620  s=['GET'])..def 
+000003b0: 636c 6173 7369 6679 5f66 696c 6528 293a  classify_file():
+000003c0: 0d0a 2020 2020 676c 6f62 616c 2061 7070  ..    global app
+000003d0: 5f64 660d 0a20 2020 2069 6620 7265 7175  _df..    if requ
+000003e0: 6573 742e 6d65 7468 6f64 203d 3d20 2747  est.method == 'G
+000003f0: 4554 273a 0d0a 2020 2020 2020 2020 2320  ET':..        # 
+00000400: 6368 6563 6b20 6966 2074 6865 2070 6f73  check if the pos
+00000410: 7420 7265 7175 6573 7420 6861 7320 7468  t request has th
+00000420: 6520 6669 6c65 2070 6172 740d 0a20 2020  e file part..   
+00000430: 2020 2020 2070 7269 6e74 2822 436c 6173       print("Clas
+00000440: 7369 6669 6361 7469 6f6e 2072 6571 7565  sification reque
+00000450: 7374 3a22 290d 0a20 2020 2020 2020 2069  st:")..        i
+00000460: 6620 2766 696c 656e 616d 6527 206e 6f74  f 'filename' not
+00000470: 2069 6e20 7265 7175 6573 742e 6172 6773   in request.args
+00000480: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00000490: 7269 6e74 2822 2d20 6e6f 2066 696c 656e  rint("- no filen
+000004a0: 616d 652c 2073 6572 7669 6e67 2077 6562  ame, serving web
+000004b0: 7061 6765 2069 6e73 7465 6164 2e2e 2e22  page instead..."
+000004c0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+000004d0: 6574 7572 6e20 2727 270d 0a20 2020 2020  eturn '''..     
+000004e0: 2020 2020 2020 203c 2164 6f63 7479 7065         <!doctype
+000004f0: 2068 746d 6c3e 0d0a 2020 2020 2020 2020   html>..        
+00000500: 2020 2020 3c74 6974 6c65 3e49 6d70 6f72      <title>Impor
+00000510: 7420 6669 6c65 3c2f 7469 746c 653e 0d0a  t file</title>..
+00000520: 2020 2020 2020 2020 2020 2020 3c68 313e              <h1>
+00000530: 496d 706f 7274 2061 6e64 2063 6c61 7373  Import and class
+00000540: 6966 7920 6120 7061 7274 6963 6c65 2069  ify a particle i
+00000550: 6d61 6765 3c2f 6831 3e0d 0a20 2020 2020  mage</h1>..     
+00000560: 2020 2020 2020 203c 703e 456e 7465 7220         <p>Enter 
+00000570: 7468 6520 6675 6c6c 2066 696c 6520 7061  the full file pa
+00000580: 7468 2074 6f20 696d 706f 7274 2074 6865  th to import the
+00000590: 2069 6d61 6765 2061 6e64 2063 6c61 7373   image and class
+000005a0: 6966 7920 6974 3c2f 703e 0d0a 2020 2020  ify it</p>..    
+000005b0: 2020 2020 2020 2020 3c66 6f72 6d20 6d65          <form me
+000005c0: 7468 6f64 3d22 4745 5422 3e0d 0a20 2020  thod="GET">..   
+000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005e0: 2046 696c 6520 7061 7468 3a3c 2f62 723e   File path:</br>
+000005f0: 0d0a 2020 2020 2020 2020 2020 2020 3c69  ..            <i
+00000600: 6e70 7574 2074 7970 653d 7465 7874 206e  nput type=text n
+00000610: 616d 653d 6669 6c65 6e61 6d65 3e0d 0a20  ame=filename>.. 
+00000620: 2020 2020 2020 2020 2020 203c 2f62 723e             </br>
+00000630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000640: 2020 2020 2020 5361 6d70 6c65 3a3c 2f62        Sample:</b
+00000650: 723e 0d0a 2020 2020 2020 2020 2020 2020  r>..            
+00000660: 3c69 6e70 7574 2074 7970 653d 7465 7874  <input type=text
+00000670: 206e 616d 653d 7361 6d70 6c65 3e0d 0a20   name=sample>.. 
+00000680: 2020 2020 2020 2020 2020 203c 2f62 723e             </br>
+00000690: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000006a0: 2020 2020 2020 496e 6465 7820 313a 3c2f        Index 1:</
+000006b0: 6272 3e0d 0a20 2020 2020 2020 2020 2020  br>..           
+000006c0: 203c 696e 7075 7420 7479 7065 3d74 6578   <input type=tex
+000006d0: 7420 6e61 6d65 3d69 6e64 6578 313e 0d0a  t name=index1>..
+000006e0: 2020 2020 2020 2020 2020 2020 3c2f 6272              </br
+000006f0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00000700: 2020 2020 2020 2049 6e64 6578 2032 3a3c         Index 2:<
+00000710: 2f62 723e 0d0a 2020 2020 2020 2020 2020  /br>..          
+00000720: 2020 3c69 6e70 7574 2074 7970 653d 7465    <input type=te
+00000730: 7874 206e 616d 653d 696e 6465 7832 3e0d  xt name=index2>.
+00000740: 0a20 2020 2020 2020 2020 2020 203c 2f62  .            </b
+00000750: 723e 0d0a 2020 2020 2020 2020 2020 2020  r>..            
+00000760: 2020 2020 2020 2020 5265 736f 6c75 7469          Resoluti
+00000770: 6f6e 2028 7069 7865 6c73 2f6d 6d29 3a3c  on (pixels/mm):<
+00000780: 2f62 723e 0d0a 2020 2020 2020 2020 2020  /br>..          
+00000790: 2020 3c69 6e70 7574 2074 7970 653d 7465    <input type=te
+000007a0: 7874 206e 616d 653d 7265 736f 6c75 7469  xt name=resoluti
+000007b0: 6f6e 3e0d 0a20 2020 2020 2020 2020 2020  on>..           
+000007c0: 2020 2020 2020 2020 203c 2f62 723e 0d0a           </br>..
+000007d0: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
+000007e0: 7574 2074 7970 653d 7375 626d 6974 2076  ut type=submit v
+000007f0: 616c 7565 3d55 706c 6f61 643e 0d0a 2020  alue=Upload>..  
+00000800: 2020 2020 2020 2020 2020 3c2f 666f 726d            </form
+00000810: 3e27 2727 0d0a 2020 2020 2020 2020 656c  >'''..        el
+00000820: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000830: 2066 696c 656e 616d 6520 3d20 7265 7175   filename = requ
+00000840: 6573 742e 6172 6773 5b27 6669 6c65 6e61  est.args['filena
+00000850: 6d65 275d 0d0a 2020 2020 2020 2020 2020  me']..          
+00000860: 2020 7361 6d70 6c65 203d 2072 6571 7565    sample = reque
+00000870: 7374 2e61 7267 735b 2773 616d 706c 6527  st.args['sample'
+00000880: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
+00000890: 6e64 6578 3120 3d20 7265 7175 6573 742e  ndex1 = request.
+000008a0: 6172 6773 5b27 696e 6465 7831 275d 0d0a  args['index1']..
+000008b0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+000008c0: 7832 203d 2072 6571 7565 7374 2e61 7267  x2 = request.arg
+000008d0: 735b 2769 6e64 6578 3227 5d0d 0a20 2020  s['index2']..   
+000008e0: 2020 2020 2020 2020 2072 6573 6f6c 7574           resolut
+000008f0: 696f 6e20 3d20 7265 7175 6573 742e 6172  ion = request.ar
+00000900: 6773 5b27 7265 736f 6c75 7469 6f6e 275d  gs['resolution']
+00000910: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00000920: 696e 7428 6622 202d 2066 696c 656e 616d  int(f" - filenam
+00000930: 653a 2020 207b 6669 6c65 6e61 6d65 7d22  e:   {filename}"
+00000940: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+00000950: 7269 6e74 2866 2220 2d20 7361 6d70 6c65  rint(f" - sample
+00000960: 3a20 2020 2020 7b73 616d 706c 657d 2229  :     {sample}")
+00000970: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00000980: 696e 7428 6622 202d 2069 6e64 6578 313a  int(f" - index1:
+00000990: 2020 2020 207b 696e 6465 7831 7d22 290d       {index1}").
+000009a0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+000009b0: 6e74 2866 2220 2d20 696e 6465 7832 3a20  nt(f" - index2: 
+000009c0: 2020 2020 7b69 6e64 6578 327d 2229 0d0a      {index2}")..
+000009d0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000009e0: 7428 6622 202d 2072 6573 6f6c 7574 696f  t(f" - resolutio
+000009f0: 6e3a 207b 7265 736f 6c75 7469 6f6e 7d22  n: {resolution}"
+00000a00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00000a10: 2069 6620 6669 6c65 6e61 6d65 203d 3d20   if filename == 
+00000a20: 2222 3a0d 0a20 2020 2020 2020 2020 2020  "":..           
+00000a30: 2020 2020 2066 6c61 7368 2827 7b22 6572       flash('{"er
+00000a40: 726f 7222 3a22 4e6f 2066 696c 656e 616d  ror":"No filenam
+00000a50: 6520 7761 7320 656e 7465 7265 6422 7d27  e was entered"}'
+00000a60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00000a70: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
+00000a80: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00000a90: 2020 2020 2020 2020 2020 2020 2023 204c               # L
+00000aa0: 6f61 6420 696d 6167 650d 0a20 2020 2020  oad image..     
+00000ab0: 2020 2020 2020 2020 2020 2069 6620 6170             if ap
+00000ac0: 705f 696d 675f 7369 7a65 5b32 5d20 3d3d  p_img_size[2] ==
+00000ad0: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+00000ae0: 2020 2020 2020 2020 2069 6d67 5f74 7970           img_typ
+00000af0: 6520 3d20 2772 676d 270d 0a20 2020 2020  e = 'rgm'..     
+00000b00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00000b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000b20: 2020 2020 2020 696d 675f 7479 7065 203d        img_type =
+00000b30: 2027 6772 6579 7363 616c 6527 0d0a 2020   'greyscale'..  
+00000b40: 2020 2020 2020 2020 2020 2020 2020 696d                im
+00000b50: 203d 206c 6f61 645f 696d 6167 6528 6669   = load_image(fi
+00000b60: 6c65 6e61 6d65 2c20 6170 705f 696d 675f  lename, app_img_
+00000b70: 7369 7a65 2c20 696d 675f 7479 7065 290d  size, img_type).
+00000b80: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00000b90: 2020 2023 2043 6c61 7373 6966 790d 0a20     # Classify.. 
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000bb0: 6620 7466 5f76 6572 7369 6f6e 203d 3d20  f tf_version == 
+00000bc0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
+00000bd0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00000be0: 2061 7070 5f6d 6f64 656c 2874 662e 636f   app_model(tf.co
+00000bf0: 6e76 6572 745f 746f 5f74 656e 736f 7228  nvert_to_tensor(
+00000c00: 696d 5b6e 702e 6e65 7761 7869 732c 203a  im[np.newaxis, :
+00000c10: 2c20 3a2c 203a 5d2c 2064 7479 7065 3d74  , :, :], dtype=t
+00000c20: 662e 666c 6f61 7433 3229 292e 6e75 6d70  f.float32)).nump
+00000c30: 7928 295b 305d 0d0a 2020 2020 2020 2020  y()[0]..        
+00000c40: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c60: 2020 2072 6573 756c 7420 3d20 6170 705f     result = app_
+00000c70: 7365 7373 696f 6e2e 7275 6e28 6170 705f  session.run(app_
+00000c80: 6f75 7470 7574 2c20 6665 6564 5f64 6963  output, feed_dic
+00000c90: 743d 7b61 7070 5f69 6e70 7574 3a20 696d  t={app_input: im
+00000ca0: 5b6e 702e 6e65 7761 7869 732c 203a 2c20  [np.newaxis, :, 
+00000cb0: 3a2c 203a 5d7d 290d 0a0d 0a20 2020 2020  :, :]})....     
+00000cc0: 2020 2020 2020 2020 2020 2023 2050 7265             # Pre
+00000cd0: 6469 6374 696f 6e73 0d0a 2020 2020 2020  dictions..      
+00000ce0: 2020 2020 2020 2020 2020 6964 7820 3d20            idx = 
+00000cf0: 6e70 2e61 7267 6d61 7828 7265 7375 6c74  np.argmax(result
+00000d00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00000d10: 2020 2063 6f64 6520 3d20 6170 705f 636c     code = app_cl
+00000d20: 735f 6c61 6265 6c73 5b69 6478 5d0d 0a20  s_labels[idx].. 
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000d40: 636f 7265 203d 206e 702e 6d61 7828 7265  core = np.max(re
+00000d50: 7375 6c74 290d 0a0d 0a20 2020 2020 2020  sult)....       
+00000d60: 2020 2020 2020 2020 2023 2046 6f72 6d61           # Forma
+00000d70: 7420 7265 7370 6f6e 7365 0d0a 2020 2020  t response..    
+00000d80: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00000d90: 6c74 5f73 7472 203d 2022 7b7b 5c22 636f  lt_str = "{{\"co
+00000da0: 6465 5c22 3a5c 227b 7d5c 222c 205c 2273  de\":\"{}\", \"s
+00000db0: 636f 7265 5c22 3a7b 7d7d 7d22 2e66 6f72  core\":{}}}".for
+00000dc0: 6d61 7428 636f 6465 2c20 7363 6f72 6529  mat(code, score)
+00000dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000de0: 2020 6966 206c 656e 2861 7070 5f64 6629    if len(app_df)
+00000df0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00000e00: 2020 2020 2020 2020 2020 2020 6170 705f              app_
+00000e10: 6466 203d 2061 7070 5f64 662e 6170 7065  df = app_df.appe
+00000e20: 6e64 2870 642e 5365 7269 6573 285b 7361  nd(pd.Series([sa
+00000e30: 6d70 6c65 5d20 2b20 5b30 5d20 2a20 6c65  mple] + [0] * le
+00000e40: 6e28 6170 705f 636c 735f 6c61 6265 6c73  n(app_cls_labels
+00000e50: 292c 2069 6e64 6578 3d61 7070 5f64 662e  ), index=app_df.
+00000e60: 636f 6c75 6d6e 7329 2c20 6967 6e6f 7265  columns), ignore
+00000e70: 5f69 6e64 6578 3d54 7275 6529 0d0a 2020  _index=True)..  
+00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e90: 2020 6170 705f 6466 2e73 6574 5f69 6e64    app_df.set_ind
+00000ea0: 6578 2827 7361 6d70 6c65 272c 2069 6e70  ex('sample', inp
+00000eb0: 6c61 6365 3d54 7275 6529 0d0a 2020 2020  lace=True)..    
+00000ec0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00000ed0: 2061 7070 5f64 662e 696e 6465 782e 7374   app_df.index.st
+00000ee0: 722e 636f 6e74 6169 6e73 2873 616d 706c  r.contains(sampl
+00000ef0: 6529 2069 7320 4661 6c73 653a 0d0a 2020  e) is False:..  
+00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f10: 2020 6170 705f 6466 203d 2061 7070 5f64    app_df = app_d
+00000f20: 662e 6170 7065 6e64 2870 642e 5365 7269  f.append(pd.Seri
+00000f30: 6573 285b 305d 202a 206c 656e 2861 7070  es([0] * len(app
+00000f40: 5f63 6c73 5f6c 6162 656c 7329 2c20 6e61  _cls_labels), na
+00000f50: 6d65 3d73 616d 706c 652c 2069 6e64 6578  me=sample, index
+00000f60: 3d61 7070 5f64 662e 636f 6c75 6d6e 7329  =app_df.columns)
+00000f70: 2c20 6967 6e6f 7265 5f69 6e64 6578 3d46  , ignore_index=F
+00000f80: 616c 7365 290d 0a20 2020 2020 2020 2020  alse)..         
+00000f90: 2020 2020 2020 2061 7070 5f64 662e 6c6f         app_df.lo
+00000fa0: 635b 7361 6d70 6c65 5d5b 6964 785d 203d  c[sample][idx] =
+00000fb0: 2061 7070 5f64 662e 6c6f 635b 7361 6d70   app_df.loc[samp
+00000fc0: 6c65 5d5b 6964 785d 202b 2031 0d0a 2020  le][idx] + 1..  
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00000fe0: 696e 7428 2252 6573 756c 7473 5c6e 202d  int("Results\n -
+00000ff0: 2063 6f64 653a 207b 7d5c 6e20 2d20 7363   code: {}\n - sc
+00001000: 6f72 653a 207b 7d22 2e66 6f72 6d61 7428  ore: {}".format(
+00001010: 6669 6c65 6e61 6d65 2c20 636f 6465 2c20  filename, code, 
+00001020: 7363 6f72 6529 290d 0a20 2020 2020 2020  score))..       
+00001030: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001040: 7265 7375 6c74 5f73 7472 0d0a 2020 2020  result_str..    
+00001050: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00001060: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2320 4572 726f 730d 0a20 2020 2020 2020  # Erros..       
+00001090: 2020 2020 2020 2020 2065 7863 5f74 7970           exc_typ
+000010a0: 652c 2065 7863 5f6f 626a 2c20 6578 635f  e, exc_obj, exc_
+000010b0: 7462 203d 2073 7973 2e65 7863 5f69 6e66  tb = sys.exc_inf
+000010c0: 6f28 290d 0a20 2020 2020 2020 2020 2020  o()..           
+000010d0: 2020 2020 2070 7269 6e74 2822 4578 6365       print("Exce
+000010e0: 7074 696f 6e20 6f6e 206c 696e 653a 207b  ption on line: {
+000010f0: 7d22 2e66 6f72 6d61 7428 6578 635f 7462  }".format(exc_tb
+00001100: 2e74 625f 6c69 6e65 6e6f 2929 0d0a 2020  .tb_lineno))..  
+00001110: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001120: 696e 7428 6529 0d0a 2020 2020 2020 2020  int(e)..        
+00001130: 2020 2020 2020 2020 7265 7375 6c74 5f73          result_s
+00001140: 7472 203d 2022 7b7b 5c22 6572 726f 725c  tr = "{{\"error\
+00001150: 223a 5c22 7b7d 5c22 7d7d 222e 666f 726d  ":\"{}\"}}".form
+00001160: 6174 2865 290d 0a20 2020 2020 2020 2020  at(e)..         
+00001170: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00001180: 7375 6c74 5f73 7472 0d0a 0d0a 0d0a 6966  sult_str......if
+00001190: 205f 5f6e 616d 655f 5f20 3d3d 2027 5f5f   __name__ == '__
+000011a0: 6d61 696e 5f5f 273a 0d0a 2020 2020 7061  main__':..    pa
+000011b0: 7273 6572 203d 2061 7267 7061 7273 652e  rser = argparse.
+000011c0: 4172 6775 6d65 6e74 5061 7273 6572 2822  ArgumentParser("
+000011d0: 4d49 534f 2043 6c61 7373 6966 6963 6174  MISO Classificat
+000011e0: 696f 6e20 5365 7276 6572 2229 0d0a 2020  ion Server")..  
+000011f0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+00001200: 756d 656e 7428 222d 6922 2c20 222d 2d69  ument("-i", "--i
+00001210: 6e66 6f22 2c20 7265 7175 6972 6564 3d54  nfo", required=T
+00001220: 7275 652c 2068 656c 703d 2243 4e4e 206e  rue, help="CNN n
+00001230: 6574 776f 726b 2069 6e66 6f72 6d61 7469  etwork informati
+00001240: 6f6e 2066 696c 6522 290d 0a20 2020 2070  on file")..    p
+00001250: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00001260: 6e74 2822 2d70 222c 2022 2d2d 706f 7274  nt("-p", "--port
+00001270: 222c 2072 6571 7569 7265 643d 5472 7565  ", required=True
+00001280: 2c20 6865 6c70 3d22 5365 7276 6572 2070  , help="Server p
+00001290: 6f72 7422 290d 0a20 2020 2061 7267 7320  ort")..    args 
+000012a0: 3d20 7061 7273 6572 2e70 6172 7365 5f61  = parser.parse_a
+000012b0: 7267 7328 290d 0a0d 0a20 2020 2069 6620  rgs()....    if 
+000012c0: 7466 5f76 6572 7369 6f6e 203d 3d20 323a  tf_version == 2:
+000012d0: 0d0a 2020 2020 2020 2020 6170 705f 6d6f  ..        app_mo
+000012e0: 6465 6c2c 2061 7070 5f69 6d67 5f73 697a  del, app_img_siz
+000012f0: 652c 2061 7070 5f63 6c73 5f6c 6162 656c  e, app_cls_label
+00001300: 7320 3d20 6c6f 6164 5f66 726f 6d5f 786d  s = load_from_xm
+00001310: 6c28 6172 6773 2e69 6e66 6f29 0d0a 2020  l(args.info)..  
+00001320: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00001330: 2061 7070 5f73 6573 7369 6f6e 2c20 6170   app_session, ap
+00001340: 705f 696e 7075 742c 2061 7070 5f6f 7574  p_input, app_out
+00001350: 7075 742c 2061 7070 5f69 6d67 5f73 697a  put, app_img_siz
+00001360: 652c 2061 7070 5f63 6c73 5f6c 6162 656c  e, app_cls_label
+00001370: 7320 3d20 6c6f 6164 5f66 726f 6d5f 786d  s = load_from_xm
+00001380: 6c28 6172 6773 2e69 6e66 6f29 0d0a 2020  l(args.info)..  
+00001390: 2020 6170 705f 6466 203d 2070 642e 4461    app_df = pd.Da
+000013a0: 7461 4672 616d 6528 636f 6c75 6d6e 733d  taFrame(columns=
+000013b0: 5b27 7361 6d70 6c65 275d 202b 2061 7070  ['sample'] + app
+000013c0: 5f63 6c73 5f6c 6162 656c 7329 0d0a 2020  _cls_labels)..  
+000013d0: 2020 7072 696e 7428 224d 4953 4f20 436c    print("MISO Cl
+000013e0: 6173 7369 6669 6361 7469 6f6e 2053 6572  assification Ser
+000013f0: 7665 7220 2d20 706f 7274 207b 7d22 2e66  ver - port {}".f
+00001400: 6f72 6d61 7428 6172 6773 2e70 6f72 7429  ormat(args.port)
+00001410: 290d 0a20 2020 2070 7269 6e74 2822 2d2d  )..    print("--
+00001420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001430: 2d2d 2d2d 2d2d 2d2d 2229 0d0a 2020 2020  --------")..    
+00001440: 7072 696e 7428 224c 6162 656c 733a 2229  print("Labels:")
+00001450: 0d0a 2020 2020 7072 696e 7428 6170 705f  ..    print(app_
+00001460: 636c 735f 6c61 6265 6c73 290d 0a20 2020  cls_labels)..   
+00001470: 2061 7070 2e72 756e 2864 6562 7567 3d46   app.run(debug=F
+00001480: 616c 7365 2c20 706f 7274 3d61 7267 732e  alse, port=args.
+00001490: 706f 7274 290d 0a0d 0a0d 0a              port)......
```

### Comparing `miso2-3.0.3/miso/layers/asoftmax.py` & `miso2-3.0.4/miso/layers/asoftmax.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import tensorflow as tf
-
-
-def ASoftmax(x, y, l, num_cls, m=2, name='asoftmax'):
-    '''
-    x: B x D - data
-    y: B x 1 - label
-    l: 1 - lambda
-    '''
-    def wrapper(x, y):
-        x = x.get_shape()
-        w = tf.get_variable("asoftmax/W", [xs[1], num_cls], dtype=tf.float32,
-                            initializer=tf.contrib.layers.xavier_initializer())
-        eps = 1e-8
-        xw = tf.matmul(x, w)
-        if m == 0:
-            return xw, tf.reduce_mean(tf.nn.sparse_softmax_cross_entropy_with_logits(labels=y, logits=xw))
-
-        w_norm = tf.norm(w, axis=0) + eps
-        logits = xw / w_norm
-
-        if y is None:
-            return logits, None
-
-        ordinal = tf.constant(list(range(0, xs[0])), tf.int64)
-        ordinal_y = tf.stack([ordinal, y], axis=1)
-
-        x_norm = tf.norm(x, axis=1) + eps
-        sel_logits = tf.gather_nd(logits, ordinal_y)
-        cos_th = tf.divide(sel_logits, x_norm)
-        if m == 1:
-            loss = tf.reduce_mean(tf.nn.sparse_softmax_cross_entropy_with_logits(labels=y, logits=logits))
-        else:
-            if m == 2:
-                cos_sign = tf.sign(cos_th)
-                res = 2 * tf.multiply(tf.sign(cos_th), tf.square(cos_th)) - 1
-            elif m == 4:
-                cos_th2 = tf.square(cos_th)
-                cos_th4 = tf.pow(cos_th, 4)
-                sign0 = tf.sign(cos_th)
-                sign3 = tf.multiply(tf.sign(2 * cos_th2 - 1), sign0)
-                sign4 = 2 * sign0 + sign3 - 3
-                res = sign3 * (8 * cos_th4 - 8 * cos_th2 + 1) + sign4
-            else:
-                raise ValueError('unsupported value of m')
-
-            scaled_logits = tf.multiply(res, x_norm)
-            f = 1.0 / (1.0 + l)
-            ff = 1.0 - f
-            comb_logits_diff = tf.add(logits, tf.scatter_nd(ordinal_y, tf.subtract(scaled_logits, sel_logits), logits.get_shape()))
-            updated_logits = ff * logits + f * comb_logits_diff
-
-            loss = tf.reduce_mean(tf.nn.sparse_softmax_cross_entropy_with_logits(labels=y, logits=updated_logits))
-
-        return logits, loss
+import tensorflow as tf
+
+
+def ASoftmax(x, y, l, num_cls, m=2, name='asoftmax'):
+    '''
+    x: B x D - data
+    y: B x 1 - label
+    l: 1 - lambda
+    '''
+    def wrapper(x, y):
+        x = x.get_shape()
+        w = tf.get_variable("asoftmax/W", [xs[1], num_cls], dtype=tf.float32,
+                            initializer=tf.contrib.layers.xavier_initializer())
+        eps = 1e-8
+        xw = tf.matmul(x, w)
+        if m == 0:
+            return xw, tf.reduce_mean(tf.nn.sparse_softmax_cross_entropy_with_logits(labels=y, logits=xw))
+
+        w_norm = tf.norm(w, axis=0) + eps
+        logits = xw / w_norm
+
+        if y is None:
+            return logits, None
+
+        ordinal = tf.constant(list(range(0, xs[0])), tf.int64)
+        ordinal_y = tf.stack([ordinal, y], axis=1)
+
+        x_norm = tf.norm(x, axis=1) + eps
+        sel_logits = tf.gather_nd(logits, ordinal_y)
+        cos_th = tf.divide(sel_logits, x_norm)
+        if m == 1:
+            loss = tf.reduce_mean(tf.nn.sparse_softmax_cross_entropy_with_logits(labels=y, logits=logits))
+        else:
+            if m == 2:
+                cos_sign = tf.sign(cos_th)
+                res = 2 * tf.multiply(tf.sign(cos_th), tf.square(cos_th)) - 1
+            elif m == 4:
+                cos_th2 = tf.square(cos_th)
+                cos_th4 = tf.pow(cos_th, 4)
+                sign0 = tf.sign(cos_th)
+                sign3 = tf.multiply(tf.sign(2 * cos_th2 - 1), sign0)
+                sign4 = 2 * sign0 + sign3 - 3
+                res = sign3 * (8 * cos_th4 - 8 * cos_th2 + 1) + sign4
+            else:
+                raise ValueError('unsupported value of m')
+
+            scaled_logits = tf.multiply(res, x_norm)
+            f = 1.0 / (1.0 + l)
+            ff = 1.0 - f
+            comb_logits_diff = tf.add(logits, tf.scatter_nd(ordinal_y, tf.subtract(scaled_logits, sel_logits), logits.get_shape()))
+            updated_logits = ff * logits + f * comb_logits_diff
+
+            loss = tf.reduce_mean(tf.nn.sparse_softmax_cross_entropy_with_logits(labels=y, logits=updated_logits))
+
+        return logits, loss
```

### Comparing `miso2-3.0.3/miso/layers/batch_instance_normalisation.py` & `miso2-3.0.4/miso/layers/batch_instance_normalisation.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import tensorflow as tf
-
-def batch_instance_norm(x, scope='batch_instance_norm'):
-    with tf.variable_scope(scope):
-        ch = x.shape[-1]
-        eps = 1e-5
-
-        batch_mean, batch_sigma = tf.nn.moments(x, axes=[0, 1, 2], keep_dims=True)
-        x_batch = (x - batch_mean) / (tf.sqrt(batch_sigma + eps))
-
-        ins_mean, ins_sigma = tf.nn.moments(x, axes=[1, 2], keep_dims=True)
-        x_ins = (x - ins_mean) / (tf.sqrt(ins_sigma + eps))
-
-        rho = tf.get_variable("rho", [ch], initializer=tf.constant_initializer(1.0), constraint=lambda x: tf.clip_by_value(x, clip_value_min=0.0, clip_value_max=1.0))
-        gamma = tf.get_variable("gamma", [ch], initializer=tf.constant_initializer(1.0))
-        beta = tf.get_variable("beta", [ch], initializer=tf.constant_initializer(0.0))
-
-        x_hat = rho * x_batch + (1 - rho) * x_ins
-        x_hat = x_hat * gamma + beta
-
-        return x_hat
-
-from tensorflow.keras import backend as K
-from tensorflow.keras.layers import Layer
-
-class BatchInstanceNormalisation(Layer):
-
-    def __init__(self, **kwargs):
-        super(BatchInstanceNormalisation, self).__init__(**kwargs)
-
-    def build(self, input_shape):
-        # Create a trainable weight variable for this layer.
-        ch = input_shape[-1]
-        self.rho = self.add_weight(name='rho',
-                                   shape=[ch],
-                                   trainable=True,
-                                   initializer=tf.constant_initializer(1.0),
-                                   constraint=lambda x: tf.clip_by_value(x, clip_value_min=0.0, clip_value_max=1.0))
-        self.gamma = self.add_weight(name='gamma',
-                                   shape=[ch],
-                                   trainable=True,
-                                   initializer=tf.constant_initializer(1.0),
-                                   constraint=lambda x: tf.clip_by_value(x, clip_value_min=0.0, clip_value_max=1.0))
-        self.beta = self.add_weight(name='beta',
-                                   shape=[ch],
-                                   trainable=True,
-                                   initializer=tf.constant_initializer(0.0),
-                                   constraint=lambda x: tf.clip_by_value(x, clip_value_min=0.0, clip_value_max=1.0))
-
-        super(BatchInstanceNormalisation, self).build(input_shape)  # Be sure to call this at the end
-
-    def call(self, x):
-        eps = 1e-5
-
-        batch_mean, batch_sigma = tf.nn.moments(x, axes=[0, 1, 2], keep_dims=True)
-        x_batch = (x - batch_mean) / (tf.sqrt(batch_sigma + eps))
-
-        ins_mean, ins_sigma = tf.nn.moments(x, axes=[1, 2], keep_dims=True)
-        x_ins = (x - ins_mean) / (tf.sqrt(ins_sigma + eps))
-
-        x_hat = self.rho * x_batch + (1 - self.rho) * x_ins
-        x_hat = x_hat * self.gamma + self.beta
-
+import tensorflow as tf
+
+def batch_instance_norm(x, scope='batch_instance_norm'):
+    with tf.variable_scope(scope):
+        ch = x.shape[-1]
+        eps = 1e-5
+
+        batch_mean, batch_sigma = tf.nn.moments(x, axes=[0, 1, 2], keep_dims=True)
+        x_batch = (x - batch_mean) / (tf.sqrt(batch_sigma + eps))
+
+        ins_mean, ins_sigma = tf.nn.moments(x, axes=[1, 2], keep_dims=True)
+        x_ins = (x - ins_mean) / (tf.sqrt(ins_sigma + eps))
+
+        rho = tf.get_variable("rho", [ch], initializer=tf.constant_initializer(1.0), constraint=lambda x: tf.clip_by_value(x, clip_value_min=0.0, clip_value_max=1.0))
+        gamma = tf.get_variable("gamma", [ch], initializer=tf.constant_initializer(1.0))
+        beta = tf.get_variable("beta", [ch], initializer=tf.constant_initializer(0.0))
+
+        x_hat = rho * x_batch + (1 - rho) * x_ins
+        x_hat = x_hat * gamma + beta
+
+        return x_hat
+
+from tensorflow.keras import backend as K
+from tensorflow.keras.layers import Layer
+
+class BatchInstanceNormalisation(Layer):
+
+    def __init__(self, **kwargs):
+        super(BatchInstanceNormalisation, self).__init__(**kwargs)
+
+    def build(self, input_shape):
+        # Create a trainable weight variable for this layer.
+        ch = input_shape[-1]
+        self.rho = self.add_weight(name='rho',
+                                   shape=[ch],
+                                   trainable=True,
+                                   initializer=tf.constant_initializer(1.0),
+                                   constraint=lambda x: tf.clip_by_value(x, clip_value_min=0.0, clip_value_max=1.0))
+        self.gamma = self.add_weight(name='gamma',
+                                   shape=[ch],
+                                   trainable=True,
+                                   initializer=tf.constant_initializer(1.0),
+                                   constraint=lambda x: tf.clip_by_value(x, clip_value_min=0.0, clip_value_max=1.0))
+        self.beta = self.add_weight(name='beta',
+                                   shape=[ch],
+                                   trainable=True,
+                                   initializer=tf.constant_initializer(0.0),
+                                   constraint=lambda x: tf.clip_by_value(x, clip_value_min=0.0, clip_value_max=1.0))
+
+        super(BatchInstanceNormalisation, self).build(input_shape)  # Be sure to call this at the end
+
+    def call(self, x):
+        eps = 1e-5
+
+        batch_mean, batch_sigma = tf.nn.moments(x, axes=[0, 1, 2], keep_dims=True)
+        x_batch = (x - batch_mean) / (tf.sqrt(batch_sigma + eps))
+
+        ins_mean, ins_sigma = tf.nn.moments(x, axes=[1, 2], keep_dims=True)
+        x_ins = (x - ins_mean) / (tf.sqrt(ins_sigma + eps))
+
+        x_hat = self.rho * x_batch + (1 - self.rho) * x_ins
+        x_hat = x_hat * self.gamma + self.beta
+
         return x_hat
```

### Comparing `miso2-3.0.3/miso/layers/cyclic.py` & `miso2-3.0.4/miso/layers/cyclic.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-import tensorflow as tf
-import numpy as np
-
-
-class CyclicSlice4(tf.keras.layers.Layer):
-    def __init__(self, **kwargs):
-        super(CyclicSlice4, self).__init__(**kwargs)
-
-    def call(self, input):
-        F = slice_4(input)
-        return F
-
-class CyclicGainSlice12(tf.keras.layers.Layer):
-    def __init__(self, **kwargs):
-        super(CyclicGainSlice12, self).__init__(**kwargs)
-
-    def call(self, input):
-        F = slice_gain_12(input)
-        return F
-
-
-class CyclicRoll4(tf.keras.layers.Layer):
-    def __init__(self, **kwargs):
-        super(CyclicRoll4, self).__init__(**kwargs)
-
-    def call(self, input):
-        return roll_4(input)
-
-
-class CyclicPool4(tf.keras.layers.Layer):
-    def __init__(self, pool_op, **kwargs):
-        super(CyclicPool4, self).__init__(**kwargs)
-        self.pool_op = pool_op
-
-    def call(self, input):
-        return pool_4(input, self.pool_op)
-
-
-class CyclicDensePool4(tf.keras.layers.Layer):
-    def __init__(self, pool_op):
-        super(CyclicDensePool4, self).__init__()
-        self.pool_op = pool_op
-
-    def call(self, input):
-        return dense_pool_4(input, self.pool_op)
-
-
-class CyclicDensePoolN(tf.keras.layers.Layer):
-    def __init__(self, pool_op, split_count=12):
-        super(CyclicDensePoolN, self).__init__()
-        self.pool_op = pool_op
-        self.n = split_count
-
-    def call(self, input):
-        return dense_pool_n(input, self.pool_op, self.n)
-
-def gain_3(X):
-    Y = []
-    Y.append(X)
-    Y.append(tf.multiply(X, 0.5))
-    Y.append(tf.multiply(X, 2))
-    return Y
-
-def rotate_4(X):
-    Y = []
-    Y.append(X)
-    Y.append(tf.reverse(tf.transpose(X, [0, 2, 1, 3]), [1]))
-    Y.append(tf.reverse(X, [1, 2]))
-    Y.append(tf.reverse(tf.transpose(X, [0, 2, 1, 3]), [2]))
-    return Y
-
-def unrotate_4(X):
-    Y = []
-    Y.append(X)
-    Y.append(tf.reverse(tf.transpose(X, [0, 2, 1, 3]), [2]))
-    Y.append(tf.reverse(X, [1, 2]))
-    Y.append(tf.reverse(tf.transpose(X, [0, 2, 1, 3]), [1]))
-    return Y
-
-def reorder_4(X, order):
-    Y = tf.split(X, 4)
-    Z = [Y[i] for i in order]
-    return tf.concat(Z, 0)
-
-
-def slice_4(X):
-    Y = rotate_4(X)
-    return tf.concat(Y, 0)
-
-def slice_gain_12(X):
-    Y = gain_3(X)
-    Y = tf.concat(Y, 0)
-    Y = rotate_4(Y)
-    return tf.concat(Y, 0)
-
-# Also try role that is a bit different
-def roll_4(X):
-    Y = unrotate_4(X)
-    Z = []
-    Z.append(X)
-    for i in range(1, 4):
-        Z.append(reorder_4(Y[i], np.roll(range(4), shift=-i)))
-    return tf.concat(Z, 3)
-
-
-def stack_4(X):
-    Y = tf.split(X, 4)
-    Z = []
-    Z.append(Y[0])
-    Z.append(tf.reverse(tf.transpose(Y[1], [0, 2, 1, 3]), [2]))
-    Z.append(tf.reverse(Y[2], [1, 2]))
-    Z.append(tf.reverse(tf.transpose(Y[3], [0, 2, 1, 3]), [1]))
-    return tf.concat(3)
-
-
-def pool_4(X, pool_op):
-    Y = tf.split(X, 4)
-    Z = []
-    Z.append(Y[0])
-    Z.append(tf.reverse(tf.transpose(Y[1], [0, 2, 1, 3]), [2]))
-    Z.append(tf.reverse(Y[2], [1, 2]))
-    Z.append(tf.reverse(tf.transpose(Y[3], [0, 2, 1, 3]), [1]))
-    W = tf.stack(Z, 4)
-    return pool_op(W, (4))
-
-
-def dense_pool_4(X, pool_op):
-    Y = tf.split(X, 4)
-    W = tf.stack(Y, 2)
-    return pool_op(W, 2)
-
-def dense_pool_n(X, pool_op, n):
-    Y = tf.split(X, n)
-    W = tf.stack(Y, 2)
-    return pool_op(W, 2)
+import tensorflow as tf
+import numpy as np
+
+
+class CyclicSlice4(tf.keras.layers.Layer):
+    def __init__(self, **kwargs):
+        super(CyclicSlice4, self).__init__(**kwargs)
+
+    def call(self, input):
+        F = slice_4(input)
+        return F
+
+class CyclicGainSlice12(tf.keras.layers.Layer):
+    def __init__(self, **kwargs):
+        super(CyclicGainSlice12, self).__init__(**kwargs)
+
+    def call(self, input):
+        F = slice_gain_12(input)
+        return F
+
+
+class CyclicRoll4(tf.keras.layers.Layer):
+    def __init__(self, **kwargs):
+        super(CyclicRoll4, self).__init__(**kwargs)
+
+    def call(self, input):
+        return roll_4(input)
+
+
+class CyclicPool4(tf.keras.layers.Layer):
+    def __init__(self, pool_op, **kwargs):
+        super(CyclicPool4, self).__init__(**kwargs)
+        self.pool_op = pool_op
+
+    def call(self, input):
+        return pool_4(input, self.pool_op)
+
+
+class CyclicDensePool4(tf.keras.layers.Layer):
+    def __init__(self, pool_op):
+        super(CyclicDensePool4, self).__init__()
+        self.pool_op = pool_op
+
+    def call(self, input):
+        return dense_pool_4(input, self.pool_op)
+
+
+class CyclicDensePoolN(tf.keras.layers.Layer):
+    def __init__(self, pool_op, split_count=12):
+        super(CyclicDensePoolN, self).__init__()
+        self.pool_op = pool_op
+        self.n = split_count
+
+    def call(self, input):
+        return dense_pool_n(input, self.pool_op, self.n)
+
+def gain_3(X):
+    Y = []
+    Y.append(X)
+    Y.append(tf.multiply(X, 0.5))
+    Y.append(tf.multiply(X, 2))
+    return Y
+
+def rotate_4(X):
+    Y = []
+    Y.append(X)
+    Y.append(tf.reverse(tf.transpose(X, [0, 2, 1, 3]), [1]))
+    Y.append(tf.reverse(X, [1, 2]))
+    Y.append(tf.reverse(tf.transpose(X, [0, 2, 1, 3]), [2]))
+    return Y
+
+def unrotate_4(X):
+    Y = []
+    Y.append(X)
+    Y.append(tf.reverse(tf.transpose(X, [0, 2, 1, 3]), [2]))
+    Y.append(tf.reverse(X, [1, 2]))
+    Y.append(tf.reverse(tf.transpose(X, [0, 2, 1, 3]), [1]))
+    return Y
+
+def reorder_4(X, order):
+    Y = tf.split(X, 4)
+    Z = [Y[i] for i in order]
+    return tf.concat(Z, 0)
+
+
+def slice_4(X):
+    Y = rotate_4(X)
+    return tf.concat(Y, 0)
+
+def slice_gain_12(X):
+    Y = gain_3(X)
+    Y = tf.concat(Y, 0)
+    Y = rotate_4(Y)
+    return tf.concat(Y, 0)
+
+# Also try role that is a bit different
+def roll_4(X):
+    Y = unrotate_4(X)
+    Z = []
+    Z.append(X)
+    for i in range(1, 4):
+        Z.append(reorder_4(Y[i], np.roll(range(4), shift=-i)))
+    return tf.concat(Z, 3)
+
+
+def stack_4(X):
+    Y = tf.split(X, 4)
+    Z = []
+    Z.append(Y[0])
+    Z.append(tf.reverse(tf.transpose(Y[1], [0, 2, 1, 3]), [2]))
+    Z.append(tf.reverse(Y[2], [1, 2]))
+    Z.append(tf.reverse(tf.transpose(Y[3], [0, 2, 1, 3]), [1]))
+    return tf.concat(3)
+
+
+def pool_4(X, pool_op):
+    Y = tf.split(X, 4)
+    Z = []
+    Z.append(Y[0])
+    Z.append(tf.reverse(tf.transpose(Y[1], [0, 2, 1, 3]), [2]))
+    Z.append(tf.reverse(Y[2], [1, 2]))
+    Z.append(tf.reverse(tf.transpose(Y[3], [0, 2, 1, 3]), [1]))
+    W = tf.stack(Z, 4)
+    return pool_op(W, (4))
+
+
+def dense_pool_4(X, pool_op):
+    Y = tf.split(X, 4)
+    W = tf.stack(Y, 2)
+    return pool_op(W, 2)
+
+def dense_pool_n(X, pool_op, n):
+    Y = tf.split(X, n)
+    W = tf.stack(Y, 2)
+    return pool_op(W, 2)
```

### Comparing `miso2-3.0.3/miso/layers/msoftmax.py` & `miso2-3.0.4/miso/layers/msoftmax.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-"""
-https://towardsdatascience.com/enhancing-the-power-of-softmax-for-image-classification-4f8f85141739
-
-https://github.com/christk1/MSH_tensorflow_keras/blob/master/mnist.py
-
-x = tf.keras.layers.Flatten()(x)
-x = tf.keras.layers.Dense(params.embedding_size, activation='relu', name='feats0')(x)
-x = tf.keras.layers.Dense(params.embedding_size, name='features')(x)
-aux_input = tf.keras.Input(shape=(params.num_classes,))
-predictions = MSoftMaxLayer(n_classes=params.num_classes, m=params.m, s=params.s, name='MSoftMaxLayer')(
-    [x, aux_input])
-model = tf.keras.models.Model(inputs=[base_model.input, aux_input], outputs=predictions)
-
-
-REMOVE RELU FROM FINAL LAYER!
-"""
-import tensorflow as tf
-
-
-class MSoftMaxLayer(tf.keras.layers.Layer):
-
-    def __init__(self, n_classes, m=0.5, s=64., **kwargs):
-        self.num_classes = n_classes
-        self.m = m
-        self.s = s
-        super(MSoftMaxLayer, self).__init__(**kwargs)
-
-    def build(self, input_shape):
-        # Create a weight variable for this layer.
-        self.kernel = self.add_weight(name='kernel',
-                                      shape=(input_shape[0][-1], self.num_classes),
-                                      initializer=tf.random_normal_initializer(stddev=0.01),
-                                      trainable=True)
-        # input_shape[0] contains the batch
-        super(MSoftMaxLayer, self).build(input_shape)  # Be sure to call this at the end
-
-    def call(self, inps):
-        # emb (N x embs), labels (N, 10) = labels one hot
-        emb, labels = inps
-
-        # normalize feature
-        emb = tf.nn.l2_normalize(emb, axis=1) * self.s  # (n, 512)
-        # normalize weights
-        W = tf.nn.l2_normalize(self.kernel, axis=0)  # (512, 10)
-        fc7 = tf.matmul(emb, W)  # n x 10
-
-        # pick elements along axis 1
-        zy = tf.reduce_max(input_tensor=tf.multiply(fc7, labels), axis=1)  # (n, 1)
-
-        cos_t = zy / self.s
-        t = tf.acos(cos_t)
-        body = tf.cos(t + self.m)
-        new_zy = body * self.s
-        diff = new_zy - zy
-        diff = tf.expand_dims(diff, 1)
-        body = tf.multiply(labels, diff)
-        fc7 = fc7 + body
-        fc7 = tf.nn.softmax(fc7)
-
-        return fc7
-
-    def get_config(self):
-        config = super(MSoftMaxLayer, self).get_config()
-        config.update({'num_classes': self.num_classes, 'm': self.m, 's': self.s})
-        return config
-
-    def compute_output_shape(self, input_shape):
+"""
+https://towardsdatascience.com/enhancing-the-power-of-softmax-for-image-classification-4f8f85141739
+
+https://github.com/christk1/MSH_tensorflow_keras/blob/master/mnist.py
+
+x = tf.keras.layers.Flatten()(x)
+x = tf.keras.layers.Dense(params.embedding_size, activation='relu', name='feats0')(x)
+x = tf.keras.layers.Dense(params.embedding_size, name='features')(x)
+aux_input = tf.keras.Input(shape=(params.num_classes,))
+predictions = MSoftMaxLayer(n_classes=params.num_classes, m=params.m, s=params.s, name='MSoftMaxLayer')(
+    [x, aux_input])
+model = tf.keras.models.Model(inputs=[base_model.input, aux_input], outputs=predictions)
+
+
+REMOVE RELU FROM FINAL LAYER!
+"""
+import tensorflow as tf
+
+
+class MSoftMaxLayer(tf.keras.layers.Layer):
+
+    def __init__(self, n_classes, m=0.5, s=64., **kwargs):
+        self.num_classes = n_classes
+        self.m = m
+        self.s = s
+        super(MSoftMaxLayer, self).__init__(**kwargs)
+
+    def build(self, input_shape):
+        # Create a weight variable for this layer.
+        self.kernel = self.add_weight(name='kernel',
+                                      shape=(input_shape[0][-1], self.num_classes),
+                                      initializer=tf.random_normal_initializer(stddev=0.01),
+                                      trainable=True)
+        # input_shape[0] contains the batch
+        super(MSoftMaxLayer, self).build(input_shape)  # Be sure to call this at the end
+
+    def call(self, inps):
+        # emb (N x embs), labels (N, 10) = labels one hot
+        emb, labels = inps
+
+        # normalize feature
+        emb = tf.nn.l2_normalize(emb, axis=1) * self.s  # (n, 512)
+        # normalize weights
+        W = tf.nn.l2_normalize(self.kernel, axis=0)  # (512, 10)
+        fc7 = tf.matmul(emb, W)  # n x 10
+
+        # pick elements along axis 1
+        zy = tf.reduce_max(input_tensor=tf.multiply(fc7, labels), axis=1)  # (n, 1)
+
+        cos_t = zy / self.s
+        t = tf.acos(cos_t)
+        body = tf.cos(t + self.m)
+        new_zy = body * self.s
+        diff = new_zy - zy
+        diff = tf.expand_dims(diff, 1)
+        body = tf.multiply(labels, diff)
+        fc7 = fc7 + body
+        fc7 = tf.nn.softmax(fc7)
+
+        return fc7
+
+    def get_config(self):
+        config = super(MSoftMaxLayer, self).get_config()
+        config.update({'num_classes': self.num_classes, 'm': self.m, 's': self.s})
+        return config
+
+    def compute_output_shape(self, input_shape):
         return None, self.num_classes
```

### Comparing `miso2-3.0.3/miso/models/factory.py` & `miso2-3.0.4/miso/models/factory.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import math
-from collections import namedtuple
-
-from miso.models.transfer_learning import *
-from miso.models.base_cyclic import *
-from miso.models.resnet_cyclic import *
-from classification_models.tfkeras import Classifiers, ModelsFactory
-from miso.training.parameters import MisoParameters
-
-try:
-    from tensorflow.keras.applications.efficientnet import *
-except ImportError:
-    pass
-
-
-def generate(tp: MisoParameters):
-    #
-    # Transfer learning
-    #
-    # Uses any of the available models in keras applications
-    if tp.cnn.id.endswith('tl'):
-        parts = tp.cnn.id.split("_")
-        if parts[0] in TRANSFER_LEARNING_PARAMS.keys():
-            model_head, model_tail = generate_tl(tp.cnn.id, tp.dataset.num_classes, tp.cnn.img_shape)
-            return combine_tl(model_head, model_tail)
-        else:
-            raise ValueError("The CNN type {} is not supported, valid CNNs are {}".format(parts[0], TRANSFER_LEARNING_PARAMS.keys()))
-
-    #
-    # Full network training
-    #
-    # Base Cyclic - custom network created at CEREGE specifically for foraminifera by adding cyclic layers
-    if tp.cnn.id.startswith("base_cyclic"):
-        model = base_cyclic(input_shape=tp.cnn.img_shape,
-                            nb_classes=tp.dataset.num_classes,
-                            filters=tp.cnn.filters,
-                            blocks=tp.cnn.blocks,
-                            dropout=0.5,
-                            dense=512,
-                            conv_activation=tp.cnn.activation,
-                            use_batch_norm=tp.cnn.use_batch_norm,
-                            global_pooling=tp.cnn.global_pooling)
-    # ResNet Cyclic - custom network created at CEREGE specifically for foraminifera by adding cyclic layers
-    elif tp.cnn.id.startswith("resnet_cyclic"):
-        blocks = int(math.log2(tp.cnn.img_shape[0]) - 2)
-        blocks -= 1  # Resnet has one block to start with already
-        resnet_params = ResnetModelParameters('resnet_cyclic',
-                                    tp.cnn.filters,
-                                    [1 for i in range(blocks)],
-                                    residual_conv_block,
-                                    None,
-                                    use_cyclic=True,
-                                    global_pooling=tp.cnn.global_pooling)
-        model = ResNetCyclic(resnet_params, tp.cnn.img_shape, None, True, tp.dataset.num_classes)
-    # EfficientNet
-    elif tp.cnn.id.lower().startswith(("efficientnet")):
-        if tp.cnn.id.lower() == "efficientnetb0":
-            model_fn = EfficientNetB0
-        elif tp.cnn.id.lower() == "efficientnetb1":
-            model_fn = EfficientNetB1
-        elif tp.cnn.id.lower() == "efficientnetb2":
-            model_fn = EfficientNetB2
-        elif tp.cnn.id.lower() == "efficientnetb3":
-            model_fn = EfficientNetB3
-        elif tp.cnn.id.lower() == "efficientnetb4":
-            model_fn = EfficientNetB4
-        elif tp.cnn.id.lower() == "efficientnetb5":
-            model_fn = EfficientNetB5
-        elif tp.cnn.id.lower() == "efficientnetb6":
-            model_fn = EfficientNetB6
-        elif tp.cnn.id.lower() == "efficientnetb7":
-            model_fn = EfficientNetB7
-        model = model_fn(weights=None,
-                         input_shape=tp.cnn.img_shape,
-                         classes=tp.dataset.num_classes)
-    # ResNet, SEResNet, DenseNet and others from qubvel's image-classifiers python package
-    elif tp.cnn.id in ModelsFactory().models.keys():
-        classifier, preprocess_input = Classifiers.get(tp.cnn.id)
-        model = classifier(input_shape=tp.cnn.img_shape,
-                           weights=None,
-                           classes=tp.dataset.num_classes)
-    else:
-        raise ValueError(
-            "The CNN type {} is not supported, valid CNNs are base_cyclic, resnet_cyclic, efficientnetb[0-7] and {}".format(tp.cnn.id, ModelsFactory().models.keys()))
-    model.compile(optimizer='adam', loss='categorical_crossentropy', metrics=['accuracy'])
-    return model
-
-
-def generate_tl_head(cnn_type, img_shape):
-    model_head = head(cnn_type, input_shape=img_shape)
-    return model_head
-
-
-def generate_tl_tail(num_classes, input_shape):
-    model_tail = tail(num_classes, input_shape)
-    return model_tail
-
-
-def generate_tl(cnn_type, num_classes, img_shape):
-    model_head = generate_tl_head(cnn_type, img_shape)
-    model_tail = tail(num_classes, [model_head.layers[-1].output.shape[-1], ])
-    return model_head, model_tail
-
-def combine_tl(model_head, model_tail):
-    return Model(inputs=model_head.input, outputs=model_tail.call(model_head.output))
-
-
-def generate_vector(model, cnn_type):
-    if cnn_type.endswith("tl"):
-        vector_tensor = model.get_layer(index=-2).get_output_at(1)
-        vector_model = Model(model.inputs, vector_tensor)
-    elif cnn_type.startswith("base_cyclic"):
-        vector_layer = model.get_layer(index=-2)
-        vector_model = Model(model.inputs, vector_layer.output)
-    elif cnn_type.startswith("resnet_cyclic"):
-        vector_layer = model.get_layer(index=-2)
-        vector_model = Model(model.inputs, vector_layer.output)
-    elif cnn_type.startswith("resnet") or cnn_type.startswith("seresnet"):
-        vector_layer = model.get_layer(index=-3)
-        vector_model = Model(model.inputs, vector_layer.output)
-    elif cnn_type.startswith("vgg") or cnn_type.startswith("densenet"):
-        vector_layer = model.get_layer(index=-2)
-        vector_model = Model(model.inputs, vector_layer.output)
-    else:
-        vector_layer = model.get_layer(index=-2)
-        vector_model = Model(model.inputs, vector_layer.output)
-    return vector_model
+import math
+from collections import namedtuple
+
+from miso.models.transfer_learning import *
+from miso.models.base_cyclic import *
+from miso.models.resnet_cyclic import *
+from classification_models.tfkeras import Classifiers, ModelsFactory
+from miso.training.parameters import MisoParameters
+
+try:
+    from tensorflow.keras.applications.efficientnet import *
+except ImportError:
+    pass
+
+
+def generate(tp: MisoParameters):
+    #
+    # Transfer learning
+    #
+    # Uses any of the available models in keras applications
+    if tp.cnn.id.endswith('tl'):
+        parts = tp.cnn.id.split("_")
+        if parts[0] in TRANSFER_LEARNING_PARAMS.keys():
+            model_head, model_tail = generate_tl(tp.cnn.id, tp.dataset.num_classes, tp.cnn.img_shape)
+            return combine_tl(model_head, model_tail)
+        else:
+            raise ValueError("The CNN type {} is not supported, valid CNNs are {}".format(parts[0], TRANSFER_LEARNING_PARAMS.keys()))
+
+    #
+    # Full network training
+    #
+    # Base Cyclic - custom network created at CEREGE specifically for foraminifera by adding cyclic layers
+    if tp.cnn.id.startswith("base_cyclic"):
+        model = base_cyclic(input_shape=tp.cnn.img_shape,
+                            nb_classes=tp.dataset.num_classes,
+                            filters=tp.cnn.filters,
+                            blocks=tp.cnn.blocks,
+                            dropout=0.5,
+                            dense=512,
+                            conv_activation=tp.cnn.activation,
+                            use_batch_norm=tp.cnn.use_batch_norm,
+                            global_pooling=tp.cnn.global_pooling)
+    # ResNet Cyclic - custom network created at CEREGE specifically for foraminifera by adding cyclic layers
+    elif tp.cnn.id.startswith("resnet_cyclic"):
+        blocks = int(math.log2(tp.cnn.img_shape[0]) - 2)
+        blocks -= 1  # Resnet has one block to start with already
+        resnet_params = ResnetModelParameters('resnet_cyclic',
+                                    tp.cnn.filters,
+                                    [1 for i in range(blocks)],
+                                    residual_conv_block,
+                                    None,
+                                    use_cyclic=True,
+                                    global_pooling=tp.cnn.global_pooling)
+        model = ResNetCyclic(resnet_params, tp.cnn.img_shape, None, True, tp.dataset.num_classes)
+    # EfficientNet
+    elif tp.cnn.id.lower().startswith(("efficientnet")):
+        if tp.cnn.id.lower() == "efficientnetb0":
+            model_fn = EfficientNetB0
+        elif tp.cnn.id.lower() == "efficientnetb1":
+            model_fn = EfficientNetB1
+        elif tp.cnn.id.lower() == "efficientnetb2":
+            model_fn = EfficientNetB2
+        elif tp.cnn.id.lower() == "efficientnetb3":
+            model_fn = EfficientNetB3
+        elif tp.cnn.id.lower() == "efficientnetb4":
+            model_fn = EfficientNetB4
+        elif tp.cnn.id.lower() == "efficientnetb5":
+            model_fn = EfficientNetB5
+        elif tp.cnn.id.lower() == "efficientnetb6":
+            model_fn = EfficientNetB6
+        elif tp.cnn.id.lower() == "efficientnetb7":
+            model_fn = EfficientNetB7
+        model = model_fn(weights=None,
+                         input_shape=tp.cnn.img_shape,
+                         classes=tp.dataset.num_classes)
+    # ResNet, SEResNet, DenseNet and others from qubvel's image-classifiers python package
+    elif tp.cnn.id in ModelsFactory().models.keys():
+        classifier, preprocess_input = Classifiers.get(tp.cnn.id)
+        model = classifier(input_shape=tp.cnn.img_shape,
+                           weights=None,
+                           classes=tp.dataset.num_classes)
+    else:
+        raise ValueError(
+            "The CNN type {} is not supported, valid CNNs are base_cyclic, resnet_cyclic, efficientnetb[0-7] and {}".format(tp.cnn.id, ModelsFactory().models.keys()))
+    model.compile(optimizer='adam', loss='categorical_crossentropy', metrics=['accuracy'])
+    return model
+
+
+def generate_tl_head(cnn_type, img_shape):
+    model_head = head(cnn_type, input_shape=img_shape)
+    return model_head
+
+
+def generate_tl_tail(num_classes, input_shape):
+    model_tail = tail(num_classes, input_shape)
+    return model_tail
+
+
+def generate_tl(cnn_type, num_classes, img_shape):
+    model_head = generate_tl_head(cnn_type, img_shape)
+    model_tail = tail(num_classes, [model_head.layers[-1].output.shape[-1], ])
+    return model_head, model_tail
+
+def combine_tl(model_head, model_tail):
+    return Model(inputs=model_head.input, outputs=model_tail.call(model_head.output))
+
+
+def generate_vector(model, cnn_type):
+    if cnn_type.endswith("tl"):
+        vector_tensor = model.get_layer(index=-2).get_output_at(1)
+        vector_model = Model(model.inputs, vector_tensor)
+    elif cnn_type.startswith("base_cyclic"):
+        vector_layer = model.get_layer(index=-2)
+        vector_model = Model(model.inputs, vector_layer.output)
+    elif cnn_type.startswith("resnet_cyclic"):
+        vector_layer = model.get_layer(index=-2)
+        vector_model = Model(model.inputs, vector_layer.output)
+    elif cnn_type.startswith("resnet") or cnn_type.startswith("seresnet"):
+        vector_layer = model.get_layer(index=-3)
+        vector_model = Model(model.inputs, vector_layer.output)
+    elif cnn_type.startswith("vgg") or cnn_type.startswith("densenet"):
+        vector_layer = model.get_layer(index=-2)
+        vector_model = Model(model.inputs, vector_layer.output)
+    else:
+        vector_layer = model.get_layer(index=-2)
+        vector_model = Model(model.inputs, vector_layer.output)
+    return vector_model
```

### Comparing `miso2-3.0.3/miso/models/resnet_cyclic.py` & `miso2-3.0.4/miso/models/resnet_cyclic.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,318 +1,318 @@
-import os
-import collections
-import tensorflow as tf
-import tensorflow.keras as tfkeras
-from miso.layers._common_blocks import ChannelSE
-from miso.layers.cyclic import *
-from tensorflow.keras.layers import GlobalMaxPooling2D, GlobalAveragePooling2D
-
-
-# -------------------------------------------------------------------------
-#   Helpers functions
-# -------------------------------------------------------------------------
-
-def handle_block_names(stage, block):
-    name_base = 'stage{}_unit{}_'.format(stage + 1, block + 1)
-    conv_name = name_base + 'conv'
-    bn_name = name_base + 'bn'
-    relu_name = name_base + 'relu'
-    sc_name = name_base + 'sc'
-    return conv_name, bn_name, relu_name, sc_name
-
-
-def get_conv_params(**params):
-    default_conv_params = {
-        'kernel_initializer': 'he_uniform',
-        'use_bias': False,
-        'padding': 'valid',
-    }
-    default_conv_params.update(params)
-    return default_conv_params
-
-
-def get_bn_params(**params):
-    axis = 3 if tfkeras.backend.image_data_format() == 'channels_last' else 1
-    default_bn_params = {
-        'axis': axis,
-        'momentum': 0.99,
-        'epsilon': 2e-5,
-        'center': True,
-        'scale': True,
-    }
-    default_bn_params.update(params)
-    return default_bn_params
-
-
-# -------------------------------------------------------------------------
-#   Residual blocks
-# -------------------------------------------------------------------------
-
-def residual_conv_block(filters, stage, block, strides=(1, 1), attention=None, cut='pre', use_cyclic=False):
-    """The identity block is the block that has no conv layer at shortcut.
-    # Arguments
-        input_tensor: input tensor
-        kernel_size: default 3, the kernel size of
-            middle conv layer at main path
-        filters: list of integers, the filters of 3 conv layer at main path
-        stage: integer, current stage label, used for generating layer names
-        block: 'a','b'..., current block label, used for generating layer names
-        cut: one of 'pre', 'post'. used to decide where skip connection is taken
-    # Returns
-        Output tensor for the block.
-    """
-
-    def layer(input_tensor):
-
-        # get params and names of layers
-        conv_params = get_conv_params()
-        bn_params = get_bn_params()
-        conv_name, bn_name, relu_name, sc_name = handle_block_names(stage, block)
-
-        x = tfkeras.layers.BatchNormalization(name=bn_name + '1', **bn_params)(input_tensor)
-        x = tfkeras.layers.Activation('relu', name=relu_name + '1')(x)
-
-        # defining shortcut connection
-        if cut == 'pre':
-            shortcut = input_tensor
-        elif cut == 'post':
-            shortcut = tfkeras.layers.Conv2D(filters, (1, 1), name=sc_name, strides=strides, **conv_params)(x)
-        else:
-            raise ValueError('Cut type not in ["pre", "post"]')
-
-        # continue with convolution layers
-        x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
-        x = tfkeras.layers.Conv2D(filters, (3, 3), strides=strides, name=conv_name + '1', **conv_params)(x)
-        # if use_cyclic:
-        #     x = CyclicRoll4()(x)
-
-        x = tfkeras.layers.BatchNormalization(name=bn_name + '2', **bn_params)(x)
-        x = tfkeras.layers.Activation('relu', name=relu_name + '2')(x)
-        x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
-        x = tfkeras.layers.Conv2D(filters, (3, 3), name=conv_name + '2', **conv_params)(x)
-        if use_cyclic:
-            x = CyclicRoll4()(x)
-
-        # use attention block if defined
-        if attention is not None:
-            x = attention(x)
-
-        # add residual connection
-        x = tfkeras.layers.Add()([x, shortcut])
-        return x
-
-    return layer
-
-
-def residual_bottleneck_block(filters, stage, block, strides=None, attention=None, cut='pre', use_cyclic=False):
-    """The identity block is the block that has no conv layer at shortcut.
-    # Arguments
-        input_tensor: input tensor
-        kernel_size: default 3, the kernel size of
-            middle conv layer at main path
-        filters: list of integers, the filters of 3 conv layer at main path
-        stage: integer, current stage label, used for generating layer names
-        block: 'a','b'..., current block label, used for generating layer names
-        cut: one of 'pre', 'post'. used to decide where skip connection is taken
-    # Returns
-        Output tensor for the block.
-    """
-
-    def layer(input_tensor):
-
-        # get params and names of layers
-        conv_params = get_conv_params()
-        bn_params = get_bn_params()
-        conv_name, bn_name, relu_name, sc_name = handle_block_names(stage, block)
-
-        x = tfkeras.layers.BatchNormalization(name=bn_name + '1', **bn_params)(input_tensor)
-        x = tfkeras.layers.Activation('relu', name=relu_name + '1')(x)
-
-        # defining shortcut connection
-        if cut == 'pre':
-            shortcut = input_tensor
-        elif cut == 'post':
-            shortcut = tfkeras.layers.Conv2D(filters * 4, (1, 1), name=sc_name, strides=strides, **conv_params)(x)
-        else:
-            raise ValueError('Cut type not in ["pre", "post"]')
-
-        # continue with convolution layers
-        x = tfkeras.layers.Conv2D(filters, (1, 1), name=conv_name + '1', **conv_params)(x)
-
-        x = tfkeras.layers.BatchNormalization(name=bn_name + '2', **bn_params)(x)
-        x = tfkeras.layers.Activation('relu', name=relu_name + '2')(x)
-        x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
-        x = tfkeras.layers.Conv2D(filters, (3, 3), strides=strides, name=conv_name + '2', **conv_params)(x)
-
-        x = tfkeras.layers.BatchNormalization(name=bn_name + '3', **bn_params)(x)
-        x = tfkeras.layers.Activation('relu', name=relu_name + '3')(x)
-        x = tfkeras.layers.Conv2D(filters * 4, (1, 1), name=conv_name + '3', **conv_params)(x)
-
-        # use attention block if defined
-        if attention is not None:
-            x = attention(x)
-
-        # add residual connection
-        x = tfkeras.layers.Add()([x, shortcut])
-
-        return x
-
-    return layer
-
-
-# -------------------------------------------------------------------------
-#   Residual Model Builder
-# -------------------------------------------------------------------------
-
-
-def ResNetCyclic(model_params,
-                 input_shape=None,
-                 input_tensor=None,
-                 include_top=True,
-                 classes=1000,
-                 weights='imagenet',
-                 **kwargs):
-    """Instantiates the ResNet, SEResNet architecture.
-    Optionally loads weights pre-trained on ImageNet.
-    Note that the data format convention used by the model is
-    the one specified in your Keras config at `~/.keras/keras.json`.
-
-    Args:
-        include_top: whether to include the fully-connected
-            layer at the top of the network.
-        weights: one of `None` (random initialization),
-              'imagenet' (pre-training on ImageNet),
-              or the path to the weights file to be loaded.
-        input_tensor: optional Keras tensor
-            (i.e. output of `tfkeras.layers.Input()`)
-            to use as image input for the model.
-        input_shape: optional shape tuple, only to be specified
-            if `include_top` is False (otherwise the input shape
-            has to be `(224, 224, 3)` (with `channels_last` data format)
-            or `(3, 224, 224)` (with `channels_first` data format).
-            It should have exactly 3 inputs channels.
-        classes: optional number of classes to classify images
-            into, only to be specified if `include_top` is True, and
-            if no `weights` argument is specified.
-
-    Returns:
-        A Keras model instance.
-
-    Raises:
-        ValueError: in case of invalid argument for `weights`,
-            or invalid input shape.
-    """
-
-    if input_tensor is None:
-        img_input = tfkeras.layers.Input(input_shape)
-    else:
-        if not tfkeras.backend.is_keras_tensor(input_tensor):
-            img_input = tfkeras.layers.Input(tensor=input_tensor, shape=input_shape)
-        else:
-            img_input = input_tensor
-
-    # choose residual block type
-    ResidualBlock = model_params.residual_block
-    if model_params.attention:
-        Attention = model_params.attention(**kwargs)
-    else:
-        Attention = None
-
-    # get parameters for model layers
-    no_scale_bn_params = get_bn_params(scale=False)
-    bn_params = get_bn_params()
-    conv_params = get_conv_params()
-    init_filters = model_params.filters
-
-    # resnet bottom
-    if model_params.use_cyclic:
-        x = CyclicSlice4()(img_input)
-        # x = tfkeras.layers.BatchNormalization(name='bn_data', **no_scale_bn_params)(x)
-    else:
-        x = img_input
-        # x = tfkeras.layers.BatchNormalization(name='bn_data', **no_scale_bn_params)(img_input)
-    # x = tfkeras.layers.ZeroPadding2D(padding=(3, 3))(x)
-    # x = tfkeras.layers.Conv2D(init_filters, (7, 7), strides=(2, 2), name='conv0', **conv_params)(x)
-
-    # 2 layers of 3 x 3 to start!
-    x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
-    x = tfkeras.layers.Conv2D(init_filters, (3, 3), strides=(1, 1), name='conv0a', **conv_params)(x)
-    # if model_params.use_cyclic:
-    #     x = CyclicRoll4()(x)
-    x = tfkeras.layers.BatchNormalization(name='bn0', **bn_params)(x)
-    x = tfkeras.layers.Activation('relu', name='relu0')(x)
-
-    x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
-    x = tfkeras.layers.Conv2D(init_filters, (3, 3), strides=(1, 1), name='conv0b', **conv_params)(x)
-    if model_params.use_cyclic:
-        x = CyclicRoll4()(x)
-
-    # x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
-    # x = tfkeras.layers.MaxPooling2D((3, 3), strides=(2, 2), padding='valid', name='pooling0')(x)
-
-    # resnet body
-    for stage, rep in enumerate(model_params.repetitions):
-        for block in range(rep):
-
-            filters = init_filters * (2 ** (stage + 1))
-
-            # first block of first stage without strides because we have maxpooling before
-            # if block == 0 and stage == 0:
-            #     x = ResidualBlock(filters, stage, block, strides=(1, 1),
-            #                       cut='post', attention=Attention)(x)
-
-            if block == 0:
-                x = ResidualBlock(filters, stage, block, strides=(2, 2),
-                                  cut='post', attention=Attention)(x)
-
-            else:
-                x = ResidualBlock(filters, stage, block, strides=(1, 1),
-                                  cut='pre', attention=Attention)(x)
-
-    x = tfkeras.layers.BatchNormalization(name='bn1', **bn_params)(x)
-    x = tfkeras.layers.Activation('relu', name='relu1')(x)
-
-    if model_params.global_pooling == 'avg':
-        x = GlobalAveragePooling2D()(x)
-    elif model_params.global_pooling == 'max':
-        x = GlobalMaxPooling2D()(x)
-
-    x = tfkeras.layers.Flatten()(x)
-    x = CyclicDensePool4(pool_op=tf.reduce_mean)(x)
-    x = tfkeras.layers.Dropout(0.5)(x)
-    x = tfkeras.layers.Dense(512, activation='relu')(x)
-    x = tfkeras.layers.Dense(classes, activation='softmax')(x)
-
-    # # resnet top
-    # if include_top:
-    #     x = tfkeras.layers.GlobalAveragePooling2D(name='pool1')(x)
-    #     x = tfkeras.layers.Dense(classes, name='fc1')(x)
-    #     x = tfkeras.layers.Activation('softmax', name='softmax')(x)
-    # Ensure that the model takes into account any potential predecessors of `input_tensor`.
-    if input_tensor is not None:
-        inputs = tfkeras.keras_utils.get_source_inputs(input_tensor)
-    else:
-        inputs = img_input
-
-    # Create model.
-    model = tfkeras.models.Model(inputs, x)
-    return model
-
-
-ResnetModelParameters = collections.namedtuple(
-    'ModelParams',
-    ['model_name', 'filters', 'repetitions', 'residual_block', 'attention', 'use_cyclic', 'global_pooling']
-)
-
-MODELS_PARAMS = {
-    'resnet18': ResnetModelParameters('resnet18', 64, (2, 2, 2, 2), residual_conv_block, None, use_cyclic=True, global_pooling=None),
-    'resnet34': ResnetModelParameters('resnet34', 64, (3, 4, 6, 3), residual_conv_block, None, use_cyclic=True, global_pooling=None),
-    'resnet50': ResnetModelParameters('resnet50', 64, (3, 4, 6, 3), residual_bottleneck_block, None, use_cyclic=True, global_pooling=None),
-    'resnet101': ResnetModelParameters('resnet101', 64, (3, 4, 23, 3), residual_bottleneck_block, None,
-                                       use_cyclic=True, global_pooling=None),
-    'resnet152': ResnetModelParameters('resnet152', 64, (3, 8, 36, 3), residual_bottleneck_block, None,
-                                       use_cyclic=True, global_pooling=None),
-    'seresnet18': ResnetModelParameters('seresnet18', 64, (2, 2, 2, 2), residual_conv_block, ChannelSE,
-                                        use_cyclic=True, global_pooling=None),
-    'seresnet34': ResnetModelParameters('seresnet34', 64, (3, 4, 6, 3), residual_conv_block, ChannelSE,
-                                        use_cyclic=True, global_pooling=None),
-}
+import os
+import collections
+import tensorflow as tf
+import tensorflow.keras as tfkeras
+from miso.layers._common_blocks import ChannelSE
+from miso.layers.cyclic import *
+from tensorflow.keras.layers import GlobalMaxPooling2D, GlobalAveragePooling2D
+
+
+# -------------------------------------------------------------------------
+#   Helpers functions
+# -------------------------------------------------------------------------
+
+def handle_block_names(stage, block):
+    name_base = 'stage{}_unit{}_'.format(stage + 1, block + 1)
+    conv_name = name_base + 'conv'
+    bn_name = name_base + 'bn'
+    relu_name = name_base + 'relu'
+    sc_name = name_base + 'sc'
+    return conv_name, bn_name, relu_name, sc_name
+
+
+def get_conv_params(**params):
+    default_conv_params = {
+        'kernel_initializer': 'he_uniform',
+        'use_bias': False,
+        'padding': 'valid',
+    }
+    default_conv_params.update(params)
+    return default_conv_params
+
+
+def get_bn_params(**params):
+    axis = 3 if tfkeras.backend.image_data_format() == 'channels_last' else 1
+    default_bn_params = {
+        'axis': axis,
+        'momentum': 0.99,
+        'epsilon': 2e-5,
+        'center': True,
+        'scale': True,
+    }
+    default_bn_params.update(params)
+    return default_bn_params
+
+
+# -------------------------------------------------------------------------
+#   Residual blocks
+# -------------------------------------------------------------------------
+
+def residual_conv_block(filters, stage, block, strides=(1, 1), attention=None, cut='pre', use_cyclic=False):
+    """The identity block is the block that has no conv layer at shortcut.
+    # Arguments
+        input_tensor: input tensor
+        kernel_size: default 3, the kernel size of
+            middle conv layer at main path
+        filters: list of integers, the filters of 3 conv layer at main path
+        stage: integer, current stage label, used for generating layer names
+        block: 'a','b'..., current block label, used for generating layer names
+        cut: one of 'pre', 'post'. used to decide where skip connection is taken
+    # Returns
+        Output tensor for the block.
+    """
+
+    def layer(input_tensor):
+
+        # get params and names of layers
+        conv_params = get_conv_params()
+        bn_params = get_bn_params()
+        conv_name, bn_name, relu_name, sc_name = handle_block_names(stage, block)
+
+        x = tfkeras.layers.BatchNormalization(name=bn_name + '1', **bn_params)(input_tensor)
+        x = tfkeras.layers.Activation('relu', name=relu_name + '1')(x)
+
+        # defining shortcut connection
+        if cut == 'pre':
+            shortcut = input_tensor
+        elif cut == 'post':
+            shortcut = tfkeras.layers.Conv2D(filters, (1, 1), name=sc_name, strides=strides, **conv_params)(x)
+        else:
+            raise ValueError('Cut type not in ["pre", "post"]')
+
+        # continue with convolution layers
+        x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
+        x = tfkeras.layers.Conv2D(filters, (3, 3), strides=strides, name=conv_name + '1', **conv_params)(x)
+        # if use_cyclic:
+        #     x = CyclicRoll4()(x)
+
+        x = tfkeras.layers.BatchNormalization(name=bn_name + '2', **bn_params)(x)
+        x = tfkeras.layers.Activation('relu', name=relu_name + '2')(x)
+        x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
+        x = tfkeras.layers.Conv2D(filters, (3, 3), name=conv_name + '2', **conv_params)(x)
+        if use_cyclic:
+            x = CyclicRoll4()(x)
+
+        # use attention block if defined
+        if attention is not None:
+            x = attention(x)
+
+        # add residual connection
+        x = tfkeras.layers.Add()([x, shortcut])
+        return x
+
+    return layer
+
+
+def residual_bottleneck_block(filters, stage, block, strides=None, attention=None, cut='pre', use_cyclic=False):
+    """The identity block is the block that has no conv layer at shortcut.
+    # Arguments
+        input_tensor: input tensor
+        kernel_size: default 3, the kernel size of
+            middle conv layer at main path
+        filters: list of integers, the filters of 3 conv layer at main path
+        stage: integer, current stage label, used for generating layer names
+        block: 'a','b'..., current block label, used for generating layer names
+        cut: one of 'pre', 'post'. used to decide where skip connection is taken
+    # Returns
+        Output tensor for the block.
+    """
+
+    def layer(input_tensor):
+
+        # get params and names of layers
+        conv_params = get_conv_params()
+        bn_params = get_bn_params()
+        conv_name, bn_name, relu_name, sc_name = handle_block_names(stage, block)
+
+        x = tfkeras.layers.BatchNormalization(name=bn_name + '1', **bn_params)(input_tensor)
+        x = tfkeras.layers.Activation('relu', name=relu_name + '1')(x)
+
+        # defining shortcut connection
+        if cut == 'pre':
+            shortcut = input_tensor
+        elif cut == 'post':
+            shortcut = tfkeras.layers.Conv2D(filters * 4, (1, 1), name=sc_name, strides=strides, **conv_params)(x)
+        else:
+            raise ValueError('Cut type not in ["pre", "post"]')
+
+        # continue with convolution layers
+        x = tfkeras.layers.Conv2D(filters, (1, 1), name=conv_name + '1', **conv_params)(x)
+
+        x = tfkeras.layers.BatchNormalization(name=bn_name + '2', **bn_params)(x)
+        x = tfkeras.layers.Activation('relu', name=relu_name + '2')(x)
+        x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
+        x = tfkeras.layers.Conv2D(filters, (3, 3), strides=strides, name=conv_name + '2', **conv_params)(x)
+
+        x = tfkeras.layers.BatchNormalization(name=bn_name + '3', **bn_params)(x)
+        x = tfkeras.layers.Activation('relu', name=relu_name + '3')(x)
+        x = tfkeras.layers.Conv2D(filters * 4, (1, 1), name=conv_name + '3', **conv_params)(x)
+
+        # use attention block if defined
+        if attention is not None:
+            x = attention(x)
+
+        # add residual connection
+        x = tfkeras.layers.Add()([x, shortcut])
+
+        return x
+
+    return layer
+
+
+# -------------------------------------------------------------------------
+#   Residual Model Builder
+# -------------------------------------------------------------------------
+
+
+def ResNetCyclic(model_params,
+                 input_shape=None,
+                 input_tensor=None,
+                 include_top=True,
+                 classes=1000,
+                 weights='imagenet',
+                 **kwargs):
+    """Instantiates the ResNet, SEResNet architecture.
+    Optionally loads weights pre-trained on ImageNet.
+    Note that the data format convention used by the model is
+    the one specified in your Keras config at `~/.keras/keras.json`.
+
+    Args:
+        include_top: whether to include the fully-connected
+            layer at the top of the network.
+        weights: one of `None` (random initialization),
+              'imagenet' (pre-training on ImageNet),
+              or the path to the weights file to be loaded.
+        input_tensor: optional Keras tensor
+            (i.e. output of `tfkeras.layers.Input()`)
+            to use as image input for the model.
+        input_shape: optional shape tuple, only to be specified
+            if `include_top` is False (otherwise the input shape
+            has to be `(224, 224, 3)` (with `channels_last` data format)
+            or `(3, 224, 224)` (with `channels_first` data format).
+            It should have exactly 3 inputs channels.
+        classes: optional number of classes to classify images
+            into, only to be specified if `include_top` is True, and
+            if no `weights` argument is specified.
+
+    Returns:
+        A Keras model instance.
+
+    Raises:
+        ValueError: in case of invalid argument for `weights`,
+            or invalid input shape.
+    """
+
+    if input_tensor is None:
+        img_input = tfkeras.layers.Input(input_shape)
+    else:
+        if not tfkeras.backend.is_keras_tensor(input_tensor):
+            img_input = tfkeras.layers.Input(tensor=input_tensor, shape=input_shape)
+        else:
+            img_input = input_tensor
+
+    # choose residual block type
+    ResidualBlock = model_params.residual_block
+    if model_params.attention:
+        Attention = model_params.attention(**kwargs)
+    else:
+        Attention = None
+
+    # get parameters for model layers
+    no_scale_bn_params = get_bn_params(scale=False)
+    bn_params = get_bn_params()
+    conv_params = get_conv_params()
+    init_filters = model_params.filters
+
+    # resnet bottom
+    if model_params.use_cyclic:
+        x = CyclicSlice4()(img_input)
+        # x = tfkeras.layers.BatchNormalization(name='bn_data', **no_scale_bn_params)(x)
+    else:
+        x = img_input
+        # x = tfkeras.layers.BatchNormalization(name='bn_data', **no_scale_bn_params)(img_input)
+    # x = tfkeras.layers.ZeroPadding2D(padding=(3, 3))(x)
+    # x = tfkeras.layers.Conv2D(init_filters, (7, 7), strides=(2, 2), name='conv0', **conv_params)(x)
+
+    # 2 layers of 3 x 3 to start!
+    x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
+    x = tfkeras.layers.Conv2D(init_filters, (3, 3), strides=(1, 1), name='conv0a', **conv_params)(x)
+    # if model_params.use_cyclic:
+    #     x = CyclicRoll4()(x)
+    x = tfkeras.layers.BatchNormalization(name='bn0', **bn_params)(x)
+    x = tfkeras.layers.Activation('relu', name='relu0')(x)
+
+    x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
+    x = tfkeras.layers.Conv2D(init_filters, (3, 3), strides=(1, 1), name='conv0b', **conv_params)(x)
+    if model_params.use_cyclic:
+        x = CyclicRoll4()(x)
+
+    # x = tfkeras.layers.ZeroPadding2D(padding=(1, 1))(x)
+    # x = tfkeras.layers.MaxPooling2D((3, 3), strides=(2, 2), padding='valid', name='pooling0')(x)
+
+    # resnet body
+    for stage, rep in enumerate(model_params.repetitions):
+        for block in range(rep):
+
+            filters = init_filters * (2 ** (stage + 1))
+
+            # first block of first stage without strides because we have maxpooling before
+            # if block == 0 and stage == 0:
+            #     x = ResidualBlock(filters, stage, block, strides=(1, 1),
+            #                       cut='post', attention=Attention)(x)
+
+            if block == 0:
+                x = ResidualBlock(filters, stage, block, strides=(2, 2),
+                                  cut='post', attention=Attention)(x)
+
+            else:
+                x = ResidualBlock(filters, stage, block, strides=(1, 1),
+                                  cut='pre', attention=Attention)(x)
+
+    x = tfkeras.layers.BatchNormalization(name='bn1', **bn_params)(x)
+    x = tfkeras.layers.Activation('relu', name='relu1')(x)
+
+    if model_params.global_pooling == 'avg':
+        x = GlobalAveragePooling2D()(x)
+    elif model_params.global_pooling == 'max':
+        x = GlobalMaxPooling2D()(x)
+
+    x = tfkeras.layers.Flatten()(x)
+    x = CyclicDensePool4(pool_op=tf.reduce_mean)(x)
+    x = tfkeras.layers.Dropout(0.5)(x)
+    x = tfkeras.layers.Dense(512, activation='relu')(x)
+    x = tfkeras.layers.Dense(classes, activation='softmax')(x)
+
+    # # resnet top
+    # if include_top:
+    #     x = tfkeras.layers.GlobalAveragePooling2D(name='pool1')(x)
+    #     x = tfkeras.layers.Dense(classes, name='fc1')(x)
+    #     x = tfkeras.layers.Activation('softmax', name='softmax')(x)
+    # Ensure that the model takes into account any potential predecessors of `input_tensor`.
+    if input_tensor is not None:
+        inputs = tfkeras.keras_utils.get_source_inputs(input_tensor)
+    else:
+        inputs = img_input
+
+    # Create model.
+    model = tfkeras.models.Model(inputs, x)
+    return model
+
+
+ResnetModelParameters = collections.namedtuple(
+    'ModelParams',
+    ['model_name', 'filters', 'repetitions', 'residual_block', 'attention', 'use_cyclic', 'global_pooling']
+)
+
+MODELS_PARAMS = {
+    'resnet18': ResnetModelParameters('resnet18', 64, (2, 2, 2, 2), residual_conv_block, None, use_cyclic=True, global_pooling=None),
+    'resnet34': ResnetModelParameters('resnet34', 64, (3, 4, 6, 3), residual_conv_block, None, use_cyclic=True, global_pooling=None),
+    'resnet50': ResnetModelParameters('resnet50', 64, (3, 4, 6, 3), residual_bottleneck_block, None, use_cyclic=True, global_pooling=None),
+    'resnet101': ResnetModelParameters('resnet101', 64, (3, 4, 23, 3), residual_bottleneck_block, None,
+                                       use_cyclic=True, global_pooling=None),
+    'resnet152': ResnetModelParameters('resnet152', 64, (3, 8, 36, 3), residual_bottleneck_block, None,
+                                       use_cyclic=True, global_pooling=None),
+    'seresnet18': ResnetModelParameters('seresnet18', 64, (2, 2, 2, 2), residual_conv_block, ChannelSE,
+                                        use_cyclic=True, global_pooling=None),
+    'seresnet34': ResnetModelParameters('seresnet34', 64, (3, 4, 6, 3), residual_conv_block, ChannelSE,
+                                        use_cyclic=True, global_pooling=None),
+}
```

### Comparing `miso2-3.0.3/miso/models/transfer_learning.py` & `miso2-3.0.4/miso/models/transfer_learning.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import collections
-import tensorflow as tf
-import tensorflow.keras.applications as ka
-from tensorflow.keras.layers import Dense, Dropout, Flatten, Conv2D, MaxPooling2D, Input, Lambda
-from tensorflow.keras.models import Model, Sequential
-from miso.layers.cyclic import *
-
-# Input range is [0,1], not [0,255] as expected by keras
-# So all prepro are adjusted to this.
-from miso.layers.msoftmax import MSoftMaxLayer
-
-
-def tf_prepro(input_shape):
-    # (x / 127.5) - 1
-    inputs = Input(shape=input_shape)
-    x = Lambda(lambda y: tf.subtract(tf.multiply(y, 2), 1))
-    return inputs, x
-
-
-def torch_prepro(input_shape):
-    # (x / 255 - mean) / std_dev
-    inputs = Input(shape=input_shape)
-    x = Lambda(lambda y: tf.subtract(y, tf.reshape(tf.constant([0.485, 0.456, 0.406]), [1, 1, 1, 3])))(inputs)
-    x = Lambda(lambda y: tf.divide(y, tf.reshape(tf.constant([0.229, 0.224, 0.225]), [1, 1, 1, 3])))(x)
-    return inputs, x
-
-
-def default_prepro(input_shape):
-    # Convert to BGR then x - mean
-    inputs = Input(shape=input_shape)
-    x = Lambda(lambda y: tf.reverse(y, axis=[-1]))(inputs)
-    x = Lambda(lambda y: tf.subtract(tf.multiply(y, 255.0),
-                                     tf.reshape(tf.constant([103.939, 116.779, 128.68]), [1, 1, 1, 3])))(x)
-    return inputs, x
-
-
-def head(cnn_type, input_shape):
-    subtypes = cnn_type.split('_')
-    model_type = subtypes[0]
-    if 'cyclic' in subtypes:
-        use_cyclic = True
-    else:
-        use_cyclic = False
-    if 'gain' in subtypes:
-        use_gain = True
-    else:
-        use_gain = False
-
-    params = TRANSFER_LEARNING_PARAMS[model_type]
-    inputs, x = params.prepro_func(input_shape)
-    if use_cyclic:
-        if use_gain:
-            x = CyclicGainSlice12()(x)
-        else:
-            x = CyclicSlice4()(x)
-    x = params.model_func(include_top=False, weights='imagenet', pooling='avg', input_shape=input_shape).call(x)
-    if use_cyclic:
-        if use_gain:
-            x = CyclicDensePoolN(pool_op=tf.reduce_mean)(x)
-        else:
-            x = CyclicDensePool4(pool_op=tf.reduce_mean)(x)
-    model = Model(inputs=inputs, outputs=x)
-    for layer in model.layers:
-        layer.trainable = False
-    return model
-
-# TODO make adjustable
-def tail(num_classes, input_shape, dropout=(0.5, 0.5)):
-    inp = Input(shape=input_shape)
-    outp = Dropout(dropout[0])(inp)
-    outp = Dense(512, activation='relu')(outp)
-    # outp = Dropout(dropout[1])(outp)
-    # outp = Dense(512, activation='relu')(outp)
-    outp = Dense(num_classes, activation='softmax')(outp)
-    return Model(inp, outp)
-
-
-def tail_vector(num_classes, input_shape, dropout=(0.5, 0.5)):
-    inp = Input(shape=input_shape)
-    outp = Dropout(dropout[0])(inp)
-    outp = Dense(512, activation='relu')(outp)
-    # outp = Dropout(dropout[1])(outp)
-    # outp = Dense(512, activation='relu')(outp)
-    return Model(inp, outp)
-
-
-TransferLearningParams = collections.namedtuple(
-    'TransferLearningParams',
-    ['model_func', 'prepro_func', 'default_input_shape']
-)
-
-# TODO Update for tensorflow 2
-TRANSFER_LEARNING_PARAMS = {
-    'xception': TransferLearningParams(ka.xception.Xception, tf_prepro, [299, 299, 3]),
-    'vgg16': TransferLearningParams(ka.vgg16.VGG16, default_prepro, [224, 224, 3]),
-    'vgg19': TransferLearningParams(ka.vgg19.VGG19, default_prepro, [224, 224, 3]),
-    'resnet50': TransferLearningParams(ka.resnet50.ResNet50, default_prepro, [224, 224, 3]),
-    # 'resnet101': TransferLearningParams(ka.xception.Xception, default_prepro, [224,224,3]),
-    # 'resnet152': TransferLearningParams(ka.xception.Xception, default_prepro, [224,224,3]),
-    # 'resnet50V2': TransferLearningParams(ka.xception.Xception, default_prepro, [224,224,3]),
-    # 'resnet101V2': TransferLearningParams(ka.xception.Xception, default_prepro, [224,224,3]),
-    # 'resnet152V2': TransferLearningParams(ka.xception.Xception, default_prepro, [224,224,3]),
-    'inceptionV3': TransferLearningParams(ka.inception_v3.InceptionV3, tf_prepro, [299, 299, 3]),
-    'inceptionresnetV2': TransferLearningParams(ka.inception_resnet_v2.InceptionResNetV2, tf_prepro, [299, 299, 3]),
-    'mobilenet': TransferLearningParams(ka.mobilenet.MobileNet, tf_prepro, [224, 224, 3]),
-    'mobilenetV2': TransferLearningParams(ka.mobilenet_v2.MobileNetV2, tf_prepro, [224, 224, 3]),
-    'densenet121': TransferLearningParams(ka.densenet.DenseNet121, torch_prepro, [224, 224, 3]),
-    'densenet169': TransferLearningParams(ka.densenet.DenseNet169, torch_prepro, [224, 224, 3]),
-    'densenet201': TransferLearningParams(ka.densenet.DenseNet201, torch_prepro, [224, 224, 3]),
-    'nasnetmobile': TransferLearningParams(ka.nasnet.NASNetMobile, tf_prepro, [224, 224, 3]),
-    'nasnetlarge': TransferLearningParams(ka.nasnet.NASNetLarge, tf_prepro, [331, 331, 3])
-}
+import collections
+import tensorflow as tf
+import tensorflow.keras.applications as ka
+from tensorflow.keras.layers import Dense, Dropout, Flatten, Conv2D, MaxPooling2D, Input, Lambda
+from tensorflow.keras.models import Model, Sequential
+from miso.layers.cyclic import *
+
+# Input range is [0,1], not [0,255] as expected by keras
+# So all prepro are adjusted to this.
+from miso.layers.msoftmax import MSoftMaxLayer
+
+
+def tf_prepro(input_shape):
+    # (x / 127.5) - 1
+    inputs = Input(shape=input_shape)
+    x = Lambda(lambda y: tf.subtract(tf.multiply(y, 2), 1))
+    return inputs, x
+
+
+def torch_prepro(input_shape):
+    # (x / 255 - mean) / std_dev
+    inputs = Input(shape=input_shape)
+    x = Lambda(lambda y: tf.subtract(y, tf.reshape(tf.constant([0.485, 0.456, 0.406]), [1, 1, 1, 3])))(inputs)
+    x = Lambda(lambda y: tf.divide(y, tf.reshape(tf.constant([0.229, 0.224, 0.225]), [1, 1, 1, 3])))(x)
+    return inputs, x
+
+
+def default_prepro(input_shape):
+    # Convert to BGR then x - mean
+    inputs = Input(shape=input_shape)
+    x = Lambda(lambda y: tf.reverse(y, axis=[-1]))(inputs)
+    x = Lambda(lambda y: tf.subtract(tf.multiply(y, 255.0),
+                                     tf.reshape(tf.constant([103.939, 116.779, 128.68]), [1, 1, 1, 3])))(x)
+    return inputs, x
+
+
+def head(cnn_type, input_shape):
+    subtypes = cnn_type.split('_')
+    model_type = subtypes[0]
+    if 'cyclic' in subtypes:
+        use_cyclic = True
+    else:
+        use_cyclic = False
+    if 'gain' in subtypes:
+        use_gain = True
+    else:
+        use_gain = False
+
+    params = TRANSFER_LEARNING_PARAMS[model_type]
+    inputs, x = params.prepro_func(input_shape)
+    if use_cyclic:
+        if use_gain:
+            x = CyclicGainSlice12()(x)
+        else:
+            x = CyclicSlice4()(x)
+    x = params.model_func(include_top=False, weights='imagenet', pooling='avg', input_shape=input_shape).call(x)
+    if use_cyclic:
+        if use_gain:
+            x = CyclicDensePoolN(pool_op=tf.reduce_mean)(x)
+        else:
+            x = CyclicDensePool4(pool_op=tf.reduce_mean)(x)
+    model = Model(inputs=inputs, outputs=x)
+    for layer in model.layers:
+        layer.trainable = False
+    return model
+
+# TODO make adjustable
+def tail(num_classes, input_shape, dropout=(0.5, 0.5)):
+    inp = Input(shape=input_shape)
+    outp = Dropout(dropout[0])(inp)
+    outp = Dense(512, activation='relu')(outp)
+    # outp = Dropout(dropout[1])(outp)
+    # outp = Dense(512, activation='relu')(outp)
+    outp = Dense(num_classes, activation='softmax')(outp)
+    return Model(inp, outp)
+
+
+def tail_vector(num_classes, input_shape, dropout=(0.5, 0.5)):
+    inp = Input(shape=input_shape)
+    outp = Dropout(dropout[0])(inp)
+    outp = Dense(512, activation='relu')(outp)
+    # outp = Dropout(dropout[1])(outp)
+    # outp = Dense(512, activation='relu')(outp)
+    return Model(inp, outp)
+
+
+TransferLearningParams = collections.namedtuple(
+    'TransferLearningParams',
+    ['model_func', 'prepro_func', 'default_input_shape']
+)
+
+# TODO Update for tensorflow 2
+TRANSFER_LEARNING_PARAMS = {
+    'xception': TransferLearningParams(ka.xception.Xception, tf_prepro, [299, 299, 3]),
+    'vgg16': TransferLearningParams(ka.vgg16.VGG16, default_prepro, [224, 224, 3]),
+    'vgg19': TransferLearningParams(ka.vgg19.VGG19, default_prepro, [224, 224, 3]),
+    'resnet50': TransferLearningParams(ka.resnet50.ResNet50, default_prepro, [224, 224, 3]),
+    # 'resnet101': TransferLearningParams(ka.xception.Xception, default_prepro, [224,224,3]),
+    # 'resnet152': TransferLearningParams(ka.xception.Xception, default_prepro, [224,224,3]),
+    # 'resnet50V2': TransferLearningParams(ka.xception.Xception, default_prepro, [224,224,3]),
+    # 'resnet101V2': TransferLearningParams(ka.xception.Xception, default_prepro, [224,224,3]),
+    # 'resnet152V2': TransferLearningParams(ka.xception.Xception, default_prepro, [224,224,3]),
+    'inceptionV3': TransferLearningParams(ka.inception_v3.InceptionV3, tf_prepro, [299, 299, 3]),
+    'inceptionresnetV2': TransferLearningParams(ka.inception_resnet_v2.InceptionResNetV2, tf_prepro, [299, 299, 3]),
+    'mobilenet': TransferLearningParams(ka.mobilenet.MobileNet, tf_prepro, [224, 224, 3]),
+    'mobilenetV2': TransferLearningParams(ka.mobilenet_v2.MobileNetV2, tf_prepro, [224, 224, 3]),
+    'densenet121': TransferLearningParams(ka.densenet.DenseNet121, torch_prepro, [224, 224, 3]),
+    'densenet169': TransferLearningParams(ka.densenet.DenseNet169, torch_prepro, [224, 224, 3]),
+    'densenet201': TransferLearningParams(ka.densenet.DenseNet201, torch_prepro, [224, 224, 3]),
+    'nasnetmobile': TransferLearningParams(ka.nasnet.NASNetMobile, tf_prepro, [224, 224, 3]),
+    'nasnetlarge': TransferLearningParams(ka.nasnet.NASNetLarge, tf_prepro, [331, 331, 3])
+}
```

### Comparing `miso2-3.0.3/miso/stats/accuracy.py` & `miso2-3.0.4/miso/stats/accuracy.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import matplotlib.pyplot as plt
-import numpy as np
-from sklearn.metrics import precision_recall_fscore_support, accuracy_score
-
-
-def plot_precision_recall(y_true,
-                          y_pred,
-                          cls_labels,
-                          fig_size=(6, 4),
-                          rotate_labels=90,
-                          show=False):
-    p, r, f1, s = precision_recall_fscore_support(y_true, y_pred, labels=range(len(cls_labels)))
-    plt.figure(facecolor="white", figsize=fig_size)
-    ax = plt.subplot(111)
-    ax.set_axisbelow(True)
-    ax.yaxis.grid(color='gray', linestyle='dashed')
-    w = 0.2
-    x = np.arange(len(p))
-    class_precision = p * 100
-    class_recall = r * 100
-    ax = plt.gca()
-    h1 = ax.bar(x - w, class_recall, width=2 * w, align='center')
-    h2 = ax.bar(x + w, class_precision, width=2 * w, align='center')
-    h3 = ax.plot(x, f1*100, 'k.')
-    plt.xticks(x, cls_labels, rotation=rotate_labels)
-    plt.ylim(0, 100)
-    plt.xlim(x[0]-0.5, x[-1]+0.5)
-    plt.legend((h1[0], h2[0], h3[0]),
-               ['recall: {0:.1f}%'.format(np.mean(r) * 100),
-                'precision: {0:.1f}%'.format(100 * np.mean(p)),
-                'f1: {0:.1f}%'.format(100 * np.mean(f1))],
-               loc=(0, 1.04),
-               ncol=3)
-    plt.xlabel('Accuracy {0:.1f}%'.format(accuracy_score(y_true, y_pred)*100))
-    plt.tight_layout()
-    # plt.subplots_adjust(top=0.85)
-    if show:
-        plt.show()
+import matplotlib.pyplot as plt
+import numpy as np
+from sklearn.metrics import precision_recall_fscore_support, accuracy_score
+
+
+def plot_precision_recall(y_true,
+                          y_pred,
+                          cls_labels,
+                          fig_size=(6, 4),
+                          rotate_labels=90,
+                          show=False):
+    p, r, f1, s = precision_recall_fscore_support(y_true, y_pred, labels=range(len(cls_labels)))
+    plt.figure(facecolor="white", figsize=fig_size)
+    ax = plt.subplot(111)
+    ax.set_axisbelow(True)
+    ax.yaxis.grid(color='gray', linestyle='dashed')
+    w = 0.2
+    x = np.arange(len(p))
+    class_precision = p * 100
+    class_recall = r * 100
+    ax = plt.gca()
+    h1 = ax.bar(x - w, class_recall, width=2 * w, align='center')
+    h2 = ax.bar(x + w, class_precision, width=2 * w, align='center')
+    h3 = ax.plot(x, f1*100, 'k.')
+    plt.xticks(x, cls_labels, rotation=rotate_labels)
+    plt.ylim(0, 100)
+    plt.xlim(x[0]-0.5, x[-1]+0.5)
+    plt.legend((h1[0], h2[0], h3[0]),
+               ['recall: {0:.1f}%'.format(np.mean(r) * 100),
+                'precision: {0:.1f}%'.format(100 * np.mean(p)),
+                'f1: {0:.1f}%'.format(100 * np.mean(f1))],
+               loc=(0, 1.04),
+               ncol=3)
+    plt.xlabel('Accuracy {0:.1f}%'.format(accuracy_score(y_true, y_pred)*100))
+    plt.tight_layout()
+    # plt.subplots_adjust(top=0.85)
+    if show:
+        plt.show()
```

### Comparing `miso2-3.0.3/miso/stats/confusion_matrix.py` & `miso2-3.0.4/miso/stats/confusion_matrix.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,344 +1,344 @@
-import numpy as np
-import itertools
-import matplotlib.pyplot as plt
-import matplotlib.patches as pch
-import matplotlib.lines as lines
-from sklearn.metrics import confusion_matrix, precision_recall_fscore_support, accuracy_score
-from matplotlib.collections import PatchCollection
-
-
-def plot_confusion_matrix(y_true,
-                          y_pred,
-                          cls_labels,
-                          normalise=True,
-                          title='Confusion matrix',
-                          cmap=plt.cm.Blues,
-                          figsize=None,
-                          style='checker',
-                          show=False):
-    """
-    This function prints and plots the confusion matrix.
-    Normalization can be applied by setting `normalize=True`.
-    """
-    # If figsize is None, estimate the plot size
-    if figsize is None:
-        figsize = (len(cls_labels) / 3, len(cls_labels) / 3)
-    # Calculate precision, recall, etc
-    p, r, f1, s = precision_recall_fscore_support(y_true, y_pred, labels=range(len(cls_labels)))
-    # Calculate confusion matrix
-    cm = confusion_matrix(y_true=y_true,
-                          y_pred=y_pred,
-                          labels=range(len(cls_labels)))
-    # Normalise the values
-    if normalise:
-        count = cm.sum(axis=1)[:, np.newaxis]
-        count[count == 0] = 1
-        cm = cm.astype('float') / count
-        cm = np.nan_to_num(cm)
-        cm = np.round(cm * 100).astype(int)
-    # Plot confusion matrix
-    plt.figure(facecolor="white", figsize=figsize)
-    plt.imshow(cm, interpolation='nearest', cmap=cmap)
-    plt.title(title)
-    # Add axes cls
-    tick_marks = np.arange(len(cls_labels))
-    plt.xticks(tick_marks, cls_labels, rotation=90)
-    plt.yticks(tick_marks, cls_labels)
-    # Add grid
-    if style == 'grid':
-        ax = plt.gca()
-        minor_tick_marks = tick_marks[:-1] + 0.5
-        ax.set_xticks(minor_tick_marks, minor=True)
-        ax.set_yticks(minor_tick_marks, minor=True)
-        plt.grid(which='minor')
-    # Add percentages in boxes
-    thresh = cm.max() / 2.
-    for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
-        if cm[i, j] != 0 or style == 'checker':
-            plt.text(j, i + 0.25, cm[i, j],
-                     horizontalalignment="center",
-                     color="white" if cm[i, j] > thresh else "black")
-    plt.ylabel('True label')
-    plt.xlabel('Predicted label')
-    plt.tight_layout()
-    if show is True:
-        plt.show()
-
-
-def get_text_width(txt):
-    f = plt.figure()
-    r = f.canvas.get_renderer()
-    t = plt.text(0.5, 0.5, txt)
-    plt.tight_layout()
-    bb = t.get_window_extent(renderer=r)
-    width = bb.width
-    plt.close('all')
-    return width
-
-
-def plot_confusion_accuracy_matrix(y_true,
-                                   y_pred,
-                                   cls_labels,
-                                   normalise=True,
-                                   title='Confusion matrix',
-                                   cmap=plt.cm.Blues,
-                                   figsize=None,
-                                   style='grid5',
-                                   show=False):
-    """
-    This function prints and plots the confusion matrix.
-    Normalization can be applied by setting `normalize=True`.
-    """
-    mult = 3
-    # If figsize is None, estimate the plot size
-    max_word = cls_labels[np.argmax([len(f"{lab}") for lab in cls_labels])]
-    txt_width = get_text_width(max_word) / 40
-    # print(txt_width)
-    sz = len(cls_labels) / mult + txt_width + 1.5
-    sz2 = len(cls_labels) / mult + 1.5
-    if figsize is None:
-        figsize = (sz, sz)
-    # Calculate precision, recall, etc
-    p, r, f1, s = precision_recall_fscore_support(y_true, y_pred, labels=range(len(cls_labels)))
-    # Calculate confusion matrix
-    cm = confusion_matrix(y_true=y_true,
-                          y_pred=y_pred,
-                          labels=range(len(cls_labels)))
-    # Normalise the values
-    if normalise:
-        cm = cm.astype('float') / cm.sum(axis=1)[:, np.newaxis]
-        cm = np.nan_to_num(cm)
-        cm = np.round(cm * 100).astype(int)
-    # Create combined plots
-    f, ax = plt.subplots(2, 2,
-                         gridspec_kw={'width_ratios': [sz2 - 1.5, 1],
-                                      'height_ratios': [1, sz2 - 1.5],
-                                      'wspace': 0,
-                                      'hspace': 0},
-                         figsize=figsize)
-    # Add counts to class cls
-    cls_labels = ['{} ({})'.format(cls_labels[i], s[i]) for i in range(len(cls_labels))]
-    thresh = cm.max() / 2.
-    # Axes
-    ax_cm = ax[1, 0]
-    ax_right = ax[1, 1]
-    ax_top = ax[0, 0]
-    ax_unused = ax[0, 1]
-    ax_unused.axis('off')
-    # Axes cls
-    tick_marks = np.arange(len(cls_labels))
-    ax_cm.set_xticks(tick_marks)
-    ax_cm.set_xticklabels(cls_labels, rotation=90)
-    ax_cm.set_yticks(tick_marks)
-    ax_cm.set_yticklabels(cls_labels)
-    # ax_cm.set_xticks(tick_marks)
-    # ax_cm.set_xticklabels(cls_labels)
-    ax_cm.set_xlim(-0.5, len(cls_labels) - 0.5)
-    ax_cm.set_ylim(-0.5, len(cls_labels) - 0.5)
-    ax_cm.invert_yaxis()
-    # Bar plots
-    remove_frame(ax_top)
-    ax_top.bar(tick_marks, p, width=0.8, color=cmap(p), edgecolor=(0, 0, 0, 0.6))
-    ax_top.set_xlim((-0.5, len(tick_marks) - 0.5))
-    for i, v in enumerate(p):
-        if np.mean(cmap(v)[:-1]) < 0.5:
-            clr = 'white'
-        else:
-            clr = 'black'
-        ax_top.text(i, 0.15, '{:.1f}'.format(v * 100), color=clr, ha='center', rotation=90, alpha=0.7)
-    remove_frame(ax_right)
-    ax_right.barh(tick_marks, r, height=0.8, color=cmap(r), edgecolor=(0, 0, 0, 0.6))
-    ax_right.set_ylim((-0.5, len(tick_marks) - 0.5))
-    for i, v in enumerate(r):
-        if np.mean(cmap(v)[:-1]) < 0.5:
-            clr = 'white'
-        else:
-            clr = 'black'
-        ax_right.text(0.05, i, '{:.1f}'.format(v * 100), color=clr, va='center', alpha=0.7)
-    ax_right.invert_yaxis()
-    # Confusion matrix
-    patches = []
-    colors = []
-    for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
-        patches.append(pch.Rectangle((j - 0.5, i - 0.5), 1, 1))
-        colors.append(cm[i, j] / 100)
-        # if cm[i, j] != 0 or style == 'checker':
-        ax_cm.text(j, i + 0.25, cm[i, j],
-                   horizontalalignment="center",
-                   color="white" if cm[i, j] > thresh else "black")
-    patcol = PatchCollection(patches, alpha=1, cmap=cmap)
-    patcol.set_array(np.array(colors))
-    ax_cm.add_collection(patcol)
-    # Grid
-    if style == 'grid':
-        for i in range(len(cls_labels) - 1):
-            line1 = lines.Line2D([i + 0.5, i + 0.5], [-0.5, len(cls_labels) + 0.5], color=(0, 0, 0, 0.05))
-            line2 = lines.Line2D([-0.5, len(cls_labels) + 0.5], [i + 0.5, i + 0.5], color=(0, 0, 0, 0.05))
-            ax_cm.add_line(line1)
-            ax_cm.add_line(line2)
-    if style == 'grid5':
-        for i in range(len(cls_labels) - 1):
-            if i % 5 == 4:
-                line1 = lines.Line2D([i + 0.5, i + 0.5], [-0.5, len(cls_labels) + 0.5], color=(0, 0, 0, 0.2))
-                line2 = lines.Line2D([-0.5, len(cls_labels) + 0.5], [i + 0.5, i + 0.5], color=(0, 0, 0, 0.2))
-                ax_cm.add_line(line1)
-                ax_cm.add_line(line2)
-    # Labels
-    ax_cm.set_ylabel('True label')
-    ax_cm.set_xlabel('Predicted label')
-    ax_right.set_ylabel('Recall {:.1f}%'.format(np.mean(r) * 100))
-    ax_right.yaxis.set_label_position('right')
-    ax_top.set_xlabel('Precision {:.1f}%'.format(np.mean(p) * 100))
-    ax_top.xaxis.set_label_position('top')
-    ax_top.set_title('Overall accuracy {:.1f}%'.format(accuracy_score(y_true, y_pred) * 100))
-    ax_cm.set_zorder(100)
-    plt.tight_layout()
-    if show is True:
-        plt.show()
-
-
-def remove_frame(ax):
-    ax.spines['top'].set_visible(False)
-    ax.spines['right'].set_visible(False)
-    ax.spines['bottom'].set_visible(False)
-    ax.spines['left'].set_visible(False)
-    ax.get_xaxis().set_ticks([])
-    ax.get_yaxis().set_ticks([])
-
-
-def plot_comparison_matrix(y_true,
-                           y_pred,
-                           true_cls_labels,
-                           pred_cls_labels,
-                           normalise=True,
-                           title='Comparison matrix',
-                           cmap=plt.cm.Blues,
-                           figsize=None,
-                           style='grid5',
-                           show=False
-                           ):
-    """
-    This function prints and plots the confusion matrix.
-    Normalization can be applied by setting `normalize=True`.
-    """
-    # If figsize is None, estimate the plot size
-    if figsize is None:
-        figsize = (len(pred_cls_labels) / 2.75 + 2, len(true_cls_labels) / 2.75 + 2)
-
-    # Calculate confusion matrix
-    max_labels = np.max((len(true_cls_labels), len(pred_cls_labels)))
-    cm = confusion_matrix(y_true=y_true,
-                          y_pred=y_pred,
-                          labels=range(max_labels))
-    cm = cm[0:len(true_cls_labels), 0:len(pred_cls_labels)]
-    support = np.sum(cm, axis=1)
-    # Normalise the values
-    if normalise:
-        cm = cm.astype('float') / cm.sum(axis=1)[:, np.newaxis]
-        cm = np.round(cm * 100).astype(int)
-    # Create combined plots
-    # f, ax = plt.subplots(2, 2,
-    #                      gridspec_kw={'width_ratios': [6, 1],
-    #                                   'height_ratios': [1, 6],
-    #                                   'wspace': 0,
-    #                                   'hspace': 0},
-    #                      figsize=figsize)
-    # Add counts to class cls
-
-    true_cls_labels = ['{} ({})'.format(true_cls_labels[i], support[i]) for i in range(len(true_cls_labels))]
-    thresh = cm.max() / 2.
-
-    fig, ax = plt.subplots(1, 1, figsize=figsize)
-    # Axes cls
-    true_tick_marks = np.arange(len(true_cls_labels))
-    pred_tick_marks = np.arange(len(pred_cls_labels))
-
-    ax.set_yticks(true_tick_marks)
-    ax.set_yticklabels(true_cls_labels)
-    ax.set_ylim(-0.5, len(true_cls_labels) - 0.5)
-
-    ax.set_xticks(pred_tick_marks)
-    ax.set_xticklabels(pred_cls_labels, rotation=90)
-    ax.set_xlim(-0.5, len(pred_cls_labels) - 0.5)
-
-    ax.invert_yaxis()
-
-    # Confusion matrix
-    patches = []
-    colors = []
-    for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
-        patches.append(pch.Rectangle((j - 0.5, i - 0.5), 1, 1))
-        colors.append(cm[i, j] / 100)
-        # if cm[i, j] != 0 or style == 'checker':
-        ax.text(j, i + 0.25, cm[i, j],
-                horizontalalignment="center",
-                color="white" if cm[i, j] > thresh else "black")
-    patcol = PatchCollection(patches, alpha=1, cmap=cmap)
-    patcol.set_array(np.array(colors))
-    ax.add_collection(patcol)
-
-    # Grid
-    if style == 'grid':
-        for i in range(len(pred_cls_labels) - 1):
-            line1 = lines.Line2D([i + 0.5, i + 0.5], [-0.5, len(true_cls_labels) + 0.5], color=(0, 0, 0, 0.05))
-            ax.add_line(line1)
-        for i in range(len(true_cls_labels) - 1):
-            line2 = lines.Line2D([-0.5, len(pred_cls_labels) + 0.5], [i + 0.5, i + 0.5], color=(0, 0, 0, 0.05))
-            ax.add_line(line2)
-
-    if style == 'grid5':
-        for i in range(len(pred_cls_labels) - 1):
-            if i % 5 == 4:
-                line1 = lines.Line2D([i + 0.5, i + 0.5], [-0.5, len(true_cls_labels) + 0.5], color=(0, 0, 0, 0.2))
-                line2 = lines.Line2D([-0.5, len(true_cls_labels) + 0.5], [i + 0.5, i + 0.5], color=(0, 0, 0, 0.2))
-                ax.add_line(line1)
-                ax.add_line(line2)
-        for i in range(len(true_cls_labels) - 1):
-            if i % 5 == 4:
-                line1 = lines.Line2D([i + 0.5, i + 0.5], [-0.5, len(pred_cls_labels) + 0.5], color=(0, 0, 0, 0.2))
-                line2 = lines.Line2D([-0.5, len(pred_cls_labels) + 0.5], [i + 0.5, i + 0.5], color=(0, 0, 0, 0.2))
-                ax.add_line(line1)
-                ax.add_line(line2)
-    # Labels
-    ax.set_ylabel('True cls')
-    ax.set_xlabel('Predicted cls')
-    plt.tight_layout()
-    if show is True:
-        plt.show()
-
-#
-# if __name__ == "__main__":
-#     import string
-#     import random
-#
-#     def get_random_string(length):
-#         # choose from all lowercase letter
-#         letters = string.ascii_lowercase
-#         result_str = ''.join(random.choice(letters) for i in range(length))
-#         # print("Random string of length", length, "is:", result_str)
-#         return result_str
-#
-#     offset = 0
-#     for i in [3,4,30,50]:
-#         y_true = np.arange(i+offset)
-#         y_pred = np.arange(i+offset)
-#         cls_labels = [get_random_string(np.random.randint(3,30)) for j in range(i+offset)]
-#         cls_labels[0] = "DIAT-Chaetoceros"
-#         cls_labels[1] = "DIAT-Other"
-#         cls_labels[2] = "DIAT-Pseudo-nitzschia"
-#         # cls_labels[0] = "DIAT-"
-#         # cls_labels[1] = "DIAT-"
-#         # cls_labels[2] = "DIAT-"
-#         if len(cls_labels) > 3:
-#             cls_labels[3] = "DIAT-Pseudo-nitzschia"
-#         print(cls_labels)
-#         plot_confusion_accuracy_matrix(y_true,
-#                                        y_pred,
-#                                        cls_labels,
-#                                        normalise=True,
-#                                        title='Confusion matrix',
-#                                        cmap=plt.cm.Blues,
-#                                        figsize=None,
-#                                        style='grid5',
-#                                        show=False)
-#         plt.show()
+import numpy as np
+import itertools
+import matplotlib.pyplot as plt
+import matplotlib.patches as pch
+import matplotlib.lines as lines
+from sklearn.metrics import confusion_matrix, precision_recall_fscore_support, accuracy_score
+from matplotlib.collections import PatchCollection
+
+
+def plot_confusion_matrix(y_true,
+                          y_pred,
+                          cls_labels,
+                          normalise=True,
+                          title='Confusion matrix',
+                          cmap=plt.cm.Blues,
+                          figsize=None,
+                          style='checker',
+                          show=False):
+    """
+    This function prints and plots the confusion matrix.
+    Normalization can be applied by setting `normalize=True`.
+    """
+    # If figsize is None, estimate the plot size
+    if figsize is None:
+        figsize = (len(cls_labels) / 3, len(cls_labels) / 3)
+    # Calculate precision, recall, etc
+    p, r, f1, s = precision_recall_fscore_support(y_true, y_pred, labels=range(len(cls_labels)))
+    # Calculate confusion matrix
+    cm = confusion_matrix(y_true=y_true,
+                          y_pred=y_pred,
+                          labels=range(len(cls_labels)))
+    # Normalise the values
+    if normalise:
+        count = cm.sum(axis=1)[:, np.newaxis]
+        count[count == 0] = 1
+        cm = cm.astype('float') / count
+        cm = np.nan_to_num(cm)
+        cm = np.round(cm * 100).astype(int)
+    # Plot confusion matrix
+    plt.figure(facecolor="white", figsize=figsize)
+    plt.imshow(cm, interpolation='nearest', cmap=cmap)
+    plt.title(title)
+    # Add axes cls
+    tick_marks = np.arange(len(cls_labels))
+    plt.xticks(tick_marks, cls_labels, rotation=90)
+    plt.yticks(tick_marks, cls_labels)
+    # Add grid
+    if style == 'grid':
+        ax = plt.gca()
+        minor_tick_marks = tick_marks[:-1] + 0.5
+        ax.set_xticks(minor_tick_marks, minor=True)
+        ax.set_yticks(minor_tick_marks, minor=True)
+        plt.grid(which='minor')
+    # Add percentages in boxes
+    thresh = cm.max() / 2.
+    for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
+        if cm[i, j] != 0 or style == 'checker':
+            plt.text(j, i + 0.25, cm[i, j],
+                     horizontalalignment="center",
+                     color="white" if cm[i, j] > thresh else "black")
+    plt.ylabel('True label')
+    plt.xlabel('Predicted label')
+    plt.tight_layout()
+    if show is True:
+        plt.show()
+
+
+def get_text_width(txt):
+    f = plt.figure()
+    r = f.canvas.get_renderer()
+    t = plt.text(0.5, 0.5, txt)
+    plt.tight_layout()
+    bb = t.get_window_extent(renderer=r)
+    width = bb.width
+    plt.close('all')
+    return width
+
+
+def plot_confusion_accuracy_matrix(y_true,
+                                   y_pred,
+                                   cls_labels,
+                                   normalise=True,
+                                   title='Confusion matrix',
+                                   cmap=plt.cm.Blues,
+                                   figsize=None,
+                                   style='grid5',
+                                   show=False):
+    """
+    This function prints and plots the confusion matrix.
+    Normalization can be applied by setting `normalize=True`.
+    """
+    mult = 3
+    # If figsize is None, estimate the plot size
+    max_word = cls_labels[np.argmax([len(f"{lab}") for lab in cls_labels])]
+    txt_width = get_text_width(max_word) / 40
+    # print(txt_width)
+    sz = len(cls_labels) / mult + txt_width + 1.5
+    sz2 = len(cls_labels) / mult + 1.5
+    if figsize is None:
+        figsize = (sz, sz)
+    # Calculate precision, recall, etc
+    p, r, f1, s = precision_recall_fscore_support(y_true, y_pred, labels=range(len(cls_labels)))
+    # Calculate confusion matrix
+    cm = confusion_matrix(y_true=y_true,
+                          y_pred=y_pred,
+                          labels=range(len(cls_labels)))
+    # Normalise the values
+    if normalise:
+        cm = cm.astype('float') / cm.sum(axis=1)[:, np.newaxis]
+        cm = np.nan_to_num(cm)
+        cm = np.round(cm * 100).astype(int)
+    # Create combined plots
+    f, ax = plt.subplots(2, 2,
+                         gridspec_kw={'width_ratios': [sz2 - 1.5, 1],
+                                      'height_ratios': [1, sz2 - 1.5],
+                                      'wspace': 0,
+                                      'hspace': 0},
+                         figsize=figsize)
+    # Add counts to class cls
+    cls_labels = ['{} ({})'.format(cls_labels[i], s[i]) for i in range(len(cls_labels))]
+    thresh = cm.max() / 2.
+    # Axes
+    ax_cm = ax[1, 0]
+    ax_right = ax[1, 1]
+    ax_top = ax[0, 0]
+    ax_unused = ax[0, 1]
+    ax_unused.axis('off')
+    # Axes cls
+    tick_marks = np.arange(len(cls_labels))
+    ax_cm.set_xticks(tick_marks)
+    ax_cm.set_xticklabels(cls_labels, rotation=90)
+    ax_cm.set_yticks(tick_marks)
+    ax_cm.set_yticklabels(cls_labels)
+    # ax_cm.set_xticks(tick_marks)
+    # ax_cm.set_xticklabels(cls_labels)
+    ax_cm.set_xlim(-0.5, len(cls_labels) - 0.5)
+    ax_cm.set_ylim(-0.5, len(cls_labels) - 0.5)
+    ax_cm.invert_yaxis()
+    # Bar plots
+    remove_frame(ax_top)
+    ax_top.bar(tick_marks, p, width=0.8, color=cmap(p), edgecolor=(0, 0, 0, 0.6))
+    ax_top.set_xlim((-0.5, len(tick_marks) - 0.5))
+    for i, v in enumerate(p):
+        if np.mean(cmap(v)[:-1]) < 0.5:
+            clr = 'white'
+        else:
+            clr = 'black'
+        ax_top.text(i, 0.15, '{:.1f}'.format(v * 100), color=clr, ha='center', rotation=90, alpha=0.7)
+    remove_frame(ax_right)
+    ax_right.barh(tick_marks, r, height=0.8, color=cmap(r), edgecolor=(0, 0, 0, 0.6))
+    ax_right.set_ylim((-0.5, len(tick_marks) - 0.5))
+    for i, v in enumerate(r):
+        if np.mean(cmap(v)[:-1]) < 0.5:
+            clr = 'white'
+        else:
+            clr = 'black'
+        ax_right.text(0.05, i, '{:.1f}'.format(v * 100), color=clr, va='center', alpha=0.7)
+    ax_right.invert_yaxis()
+    # Confusion matrix
+    patches = []
+    colors = []
+    for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
+        patches.append(pch.Rectangle((j - 0.5, i - 0.5), 1, 1))
+        colors.append(cm[i, j] / 100)
+        # if cm[i, j] != 0 or style == 'checker':
+        ax_cm.text(j, i + 0.25, cm[i, j],
+                   horizontalalignment="center",
+                   color="white" if cm[i, j] > thresh else "black")
+    patcol = PatchCollection(patches, alpha=1, cmap=cmap)
+    patcol.set_array(np.array(colors))
+    ax_cm.add_collection(patcol)
+    # Grid
+    if style == 'grid':
+        for i in range(len(cls_labels) - 1):
+            line1 = lines.Line2D([i + 0.5, i + 0.5], [-0.5, len(cls_labels) + 0.5], color=(0, 0, 0, 0.05))
+            line2 = lines.Line2D([-0.5, len(cls_labels) + 0.5], [i + 0.5, i + 0.5], color=(0, 0, 0, 0.05))
+            ax_cm.add_line(line1)
+            ax_cm.add_line(line2)
+    if style == 'grid5':
+        for i in range(len(cls_labels) - 1):
+            if i % 5 == 4:
+                line1 = lines.Line2D([i + 0.5, i + 0.5], [-0.5, len(cls_labels) + 0.5], color=(0, 0, 0, 0.2))
+                line2 = lines.Line2D([-0.5, len(cls_labels) + 0.5], [i + 0.5, i + 0.5], color=(0, 0, 0, 0.2))
+                ax_cm.add_line(line1)
+                ax_cm.add_line(line2)
+    # Labels
+    ax_cm.set_ylabel('True label')
+    ax_cm.set_xlabel('Predicted label')
+    ax_right.set_ylabel('Recall {:.1f}%'.format(np.mean(r) * 100))
+    ax_right.yaxis.set_label_position('right')
+    ax_top.set_xlabel('Precision {:.1f}%'.format(np.mean(p) * 100))
+    ax_top.xaxis.set_label_position('top')
+    ax_top.set_title('Overall accuracy {:.1f}%'.format(accuracy_score(y_true, y_pred) * 100))
+    ax_cm.set_zorder(100)
+    plt.tight_layout()
+    if show is True:
+        plt.show()
+
+
+def remove_frame(ax):
+    ax.spines['top'].set_visible(False)
+    ax.spines['right'].set_visible(False)
+    ax.spines['bottom'].set_visible(False)
+    ax.spines['left'].set_visible(False)
+    ax.get_xaxis().set_ticks([])
+    ax.get_yaxis().set_ticks([])
+
+
+def plot_comparison_matrix(y_true,
+                           y_pred,
+                           true_cls_labels,
+                           pred_cls_labels,
+                           normalise=True,
+                           title='Comparison matrix',
+                           cmap=plt.cm.Blues,
+                           figsize=None,
+                           style='grid5',
+                           show=False
+                           ):
+    """
+    This function prints and plots the confusion matrix.
+    Normalization can be applied by setting `normalize=True`.
+    """
+    # If figsize is None, estimate the plot size
+    if figsize is None:
+        figsize = (len(pred_cls_labels) / 2.75 + 2, len(true_cls_labels) / 2.75 + 2)
+
+    # Calculate confusion matrix
+    max_labels = np.max((len(true_cls_labels), len(pred_cls_labels)))
+    cm = confusion_matrix(y_true=y_true,
+                          y_pred=y_pred,
+                          labels=range(max_labels))
+    cm = cm[0:len(true_cls_labels), 0:len(pred_cls_labels)]
+    support = np.sum(cm, axis=1)
+    # Normalise the values
+    if normalise:
+        cm = cm.astype('float') / cm.sum(axis=1)[:, np.newaxis]
+        cm = np.round(cm * 100).astype(int)
+    # Create combined plots
+    # f, ax = plt.subplots(2, 2,
+    #                      gridspec_kw={'width_ratios': [6, 1],
+    #                                   'height_ratios': [1, 6],
+    #                                   'wspace': 0,
+    #                                   'hspace': 0},
+    #                      figsize=figsize)
+    # Add counts to class cls
+
+    true_cls_labels = ['{} ({})'.format(true_cls_labels[i], support[i]) for i in range(len(true_cls_labels))]
+    thresh = cm.max() / 2.
+
+    fig, ax = plt.subplots(1, 1, figsize=figsize)
+    # Axes cls
+    true_tick_marks = np.arange(len(true_cls_labels))
+    pred_tick_marks = np.arange(len(pred_cls_labels))
+
+    ax.set_yticks(true_tick_marks)
+    ax.set_yticklabels(true_cls_labels)
+    ax.set_ylim(-0.5, len(true_cls_labels) - 0.5)
+
+    ax.set_xticks(pred_tick_marks)
+    ax.set_xticklabels(pred_cls_labels, rotation=90)
+    ax.set_xlim(-0.5, len(pred_cls_labels) - 0.5)
+
+    ax.invert_yaxis()
+
+    # Confusion matrix
+    patches = []
+    colors = []
+    for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
+        patches.append(pch.Rectangle((j - 0.5, i - 0.5), 1, 1))
+        colors.append(cm[i, j] / 100)
+        # if cm[i, j] != 0 or style == 'checker':
+        ax.text(j, i + 0.25, cm[i, j],
+                horizontalalignment="center",
+                color="white" if cm[i, j] > thresh else "black")
+    patcol = PatchCollection(patches, alpha=1, cmap=cmap)
+    patcol.set_array(np.array(colors))
+    ax.add_collection(patcol)
+
+    # Grid
+    if style == 'grid':
+        for i in range(len(pred_cls_labels) - 1):
+            line1 = lines.Line2D([i + 0.5, i + 0.5], [-0.5, len(true_cls_labels) + 0.5], color=(0, 0, 0, 0.05))
+            ax.add_line(line1)
+        for i in range(len(true_cls_labels) - 1):
+            line2 = lines.Line2D([-0.5, len(pred_cls_labels) + 0.5], [i + 0.5, i + 0.5], color=(0, 0, 0, 0.05))
+            ax.add_line(line2)
+
+    if style == 'grid5':
+        for i in range(len(pred_cls_labels) - 1):
+            if i % 5 == 4:
+                line1 = lines.Line2D([i + 0.5, i + 0.5], [-0.5, len(true_cls_labels) + 0.5], color=(0, 0, 0, 0.2))
+                line2 = lines.Line2D([-0.5, len(true_cls_labels) + 0.5], [i + 0.5, i + 0.5], color=(0, 0, 0, 0.2))
+                ax.add_line(line1)
+                ax.add_line(line2)
+        for i in range(len(true_cls_labels) - 1):
+            if i % 5 == 4:
+                line1 = lines.Line2D([i + 0.5, i + 0.5], [-0.5, len(pred_cls_labels) + 0.5], color=(0, 0, 0, 0.2))
+                line2 = lines.Line2D([-0.5, len(pred_cls_labels) + 0.5], [i + 0.5, i + 0.5], color=(0, 0, 0, 0.2))
+                ax.add_line(line1)
+                ax.add_line(line2)
+    # Labels
+    ax.set_ylabel('True cls')
+    ax.set_xlabel('Predicted cls')
+    plt.tight_layout()
+    if show is True:
+        plt.show()
+
+#
+# if __name__ == "__main__":
+#     import string
+#     import random
+#
+#     def get_random_string(length):
+#         # choose from all lowercase letter
+#         letters = string.ascii_lowercase
+#         result_str = ''.join(random.choice(letters) for i in range(length))
+#         # print("Random string of length", length, "is:", result_str)
+#         return result_str
+#
+#     offset = 0
+#     for i in [3,4,30,50]:
+#         y_true = np.arange(i+offset)
+#         y_pred = np.arange(i+offset)
+#         cls_labels = [get_random_string(np.random.randint(3,30)) for j in range(i+offset)]
+#         cls_labels[0] = "DIAT-Chaetoceros"
+#         cls_labels[1] = "DIAT-Other"
+#         cls_labels[2] = "DIAT-Pseudo-nitzschia"
+#         # cls_labels[0] = "DIAT-"
+#         # cls_labels[1] = "DIAT-"
+#         # cls_labels[2] = "DIAT-"
+#         if len(cls_labels) > 3:
+#             cls_labels[3] = "DIAT-Pseudo-nitzschia"
+#         print(cls_labels)
+#         plot_confusion_accuracy_matrix(y_true,
+#                                        y_pred,
+#                                        cls_labels,
+#                                        normalise=True,
+#                                        title='Confusion matrix',
+#                                        cmap=plt.cm.Blues,
+#                                        figsize=None,
+#                                        style='grid5',
+#                                        show=False)
+#         plt.show()
```

### Comparing `miso2-3.0.3/miso/stats/embedding.py` & `miso2-3.0.4/miso/stats/embedding.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-"""
-Set of methods to make some common plots for the CNN outputs
-"""
-import matplotlib.pyplot as plt
-import numpy as np
-from matplotlib.offsetbox import OffsetImage, AnnotationBbox
-from scipy.spatial.distance import cdist
-import scipy.ndimage as nd
-
-
-def plot_embedding(X, y, num_classes, labels=None, title=None, indices=None, alpha=1.0, figsize=(8,8)):
-    """
-    Scatter plot of classes and their 2D embedding
-    :param X: The 2D co-ordinates of each class value
-    :param y: The classes
-    :param num_classes: Total number of classes
-    :param labels: Names of each class (if None, y values is used)
-    :param title: Title of the plot
-    :param indices: Extra label to append to each class point, e.g. the index of the image
-    :param alpha: Transparency of the class label (0 - fully transparent, 1 - fully opaque)
-    :param figsize: Size of the figure
-    :return:
-    """
-    if labels is None:
-        labels = ["{}".format(i) for i in range(num_classes)]
-    # print(labels)
-    # TODO: This can be simplified
-    target_values = np.array(range(num_classes))
-    colors = target_values / num_classes
-    plt.figure(figsize=figsize)
-    x_min, x_max = np.min(X, 0), np.max(X, 0)
-    # X = (X - x_min) / (x_max - x_min)
-    plt.axis([x_min[0], x_max[0], x_min[1], x_max[1]])
-    points = [[] for k in range(len(target_values))]
-    for i in range(X.shape[0]):
-        for j in range(len(target_values)):
-            if y[i] == target_values[j]:
-                lbl = "{}".format(labels[y[i]])
-                if indices is not None:
-                    lbl += " {}".format(indices[i])
-                plt.text(X[i, 0], X[i, 1], lbl,
-                         color=plt.cm.tab20(colors[j]),
-                         fontdict={'weight': 'bold', 'size': 9},alpha=alpha)
-                points[j].append([X[i, 0], X[i, 1]])
-                break
-    plt.xticks([]), plt.yticks([])
-    plt.tight_layout()
-    if title is not None:
-        plt.title(title)
-    plt.gca().axis('off')
-
-
-def plot_embedding_with_images(X, y, num_classes, images, face_colour="black", class_border=False, mask_level=(0.3, 0.7), scale_adj=1.0, figsize=None):
-    """
-    Scatter plot of classes and their 2D embedding. Instead of class name, the actual image is used.
-    The dark parts of the images will be masked (used mainly for foraminifera images)
-    :param X: The 2D co-ordinates of each class value
-    :param y: The classes
-    :param num_classes: Total number of classes
-    :param images: The images corresponding to each class entry
-    :param face_colour: Colour of the figure background
-    :param class_border: Make a border with the colour of the class (not implemented)
-    :param mask_level: Two values [0] is mask threshold, [1] is intensity above which everything is opaque
-    :param scale_adj:
-    :param figsize: Size of the figure. If None, it is scaled automatically (recommended)
-    :return:
-    """
-    # Normalise the co-ordinates
-    x_min, x_max = np.min(X, 0), np.max(X, 0)
-    X = (X - x_min) / (x_max - x_min)
-    # Calculate the scaling amount
-    scale = images.shape[1] // 64 / scale_adj
-    # Create the figure
-    if figsize is None:
-        figsize = (20*scale, 20*scale)
-    plt.figure(figsize=figsize, dpi=50, facecolor=face_colour, edgecolor=face_colour)
-    plt.gca().set_facecolor(face_colour)
-    # Plot
-    clrs = plt.cm.get_cmap('tab20')
-    for j in range(X.shape[0]):
-        img = np.squeeze(images[j,:,:,0])
-        # Create a mask with a soft border
-        # mask_level[0] is the threshold
-        # mask_level[1] is the intensity value above which everything is fully opaque
-        mask = img > mask_level[0]
-        mask = nd.morphology.binary_fill_holes(mask)
-        # if class_border:
-        #     clr = clrs(y/num_classes)
-        #     cmask = np.stack((mask*clr[0], mask*clr[1], mask*clr[2], np.ones(mask.shape)), axis=-1)
-        th = img / mask_level[1]
-        th[th > 1] = 1
-        th[mask == True] = 1
-        img = np.stack((img, img, img, th), axis=-1)
-        ab = AnnotationBbox(OffsetImage(img), (0.03 + X[j, 0]*0.94, 0.03 + X[j, 1] * 0.94), xycoords="axes fraction", frameon=False)
-        plt.gca().add_artist(ab)
-    plt.xticks([])
-    plt.yticks([])
-    plt.tight_layout()
-
-
-def plot_embedding_with_colour_images(X, images, face_colour="black", scale_adj=1.0, figsize=(10,10)):
-    # Normalise the co-ordinates
-    x_min, x_max = np.min(X, 0), np.max(X, 0)
-    X = (X - x_min) / (x_max - x_min)
-    # Calculate the scaling amount
-    scale = images.shape[1] // 64 / scale_adj
-    # Create the figure
-    if figsize is None:
-        figsize = (20*scale, 20*scale)
-    plt.figure(figsize=figsize, dpi=50, facecolor=face_colour, edgecolor=face_colour)
-    plt.gca().set_facecolor(face_colour)
-    # Plot
-    for j in range(X.shape[0]):
-        img = images[j,:,:,:]
-        ab = AnnotationBbox(OffsetImage(img), (0.03 + X[j, 0]*0.94, 0.03 + X[j, 1] * 0.94), xycoords="axes fraction", frameon=False)
-        plt.gca().add_artist(ab)
-    plt.xticks([])
-    plt.yticks([])
-    plt.tight_layout()
-
-
-def plot_embedding_with_images_on_grid(X, y, num_classes, images, width=128, mask_level=0.7, scale_adj=1.0):
-    """
-    2D image scatter plots, but with the images in a grid.
-    Requires lapjv which can be installed with 'pip install lapjv' BUT you need a C compiler installed as well
-    :param X:
-    :param y:
-    :param num_classes:
-    :param images:
-    :param width:
-    :param mask_level:
-    :param scale_adj:
-    :return:
-    """
-    grid_width = int(np.min((np.floor(np.sqrt(len(y))),20)))
-    grid = np.dstack(np.meshgrid(np.linspace(0, 1, grid_width), np.linspace(0, 1, grid_width))).reshape(-1, 2)
-    X = X[0:grid_width*grid_width,:]
-    x_min, x_max = np.min(X, 0), np.max(X, 0)
-    X = (X - x_min) / (x_max - x_min)
-    cost_matrix = cdist(grid, X, "sqeuclidean").astype(np.float32)
-    cost_matrix = cost_matrix * (100000 / cost_matrix.max())
-    row_asses, col_asses, _ = lapjv(cost_matrix)
-    grid_jv = grid[col_asses]
-    plot_embedding_with_images(grid_jv, y, num_classes, images, face_colour="black", class_border=False, mask_level=mask_level, scale_adj=scale_adj)
+"""
+Set of methods to make some common plots for the CNN outputs
+"""
+import matplotlib.pyplot as plt
+import numpy as np
+from matplotlib.offsetbox import OffsetImage, AnnotationBbox
+from scipy.spatial.distance import cdist
+import scipy.ndimage as nd
+
+
+def plot_embedding(X, y, num_classes, labels=None, title=None, indices=None, alpha=1.0, figsize=(8,8)):
+    """
+    Scatter plot of classes and their 2D embedding
+    :param X: The 2D co-ordinates of each class value
+    :param y: The classes
+    :param num_classes: Total number of classes
+    :param labels: Names of each class (if None, y values is used)
+    :param title: Title of the plot
+    :param indices: Extra label to append to each class point, e.g. the index of the image
+    :param alpha: Transparency of the class label (0 - fully transparent, 1 - fully opaque)
+    :param figsize: Size of the figure
+    :return:
+    """
+    if labels is None:
+        labels = ["{}".format(i) for i in range(num_classes)]
+    # print(labels)
+    # TODO: This can be simplified
+    target_values = np.array(range(num_classes))
+    colors = target_values / num_classes
+    plt.figure(figsize=figsize)
+    x_min, x_max = np.min(X, 0), np.max(X, 0)
+    # X = (X - x_min) / (x_max - x_min)
+    plt.axis([x_min[0], x_max[0], x_min[1], x_max[1]])
+    points = [[] for k in range(len(target_values))]
+    for i in range(X.shape[0]):
+        for j in range(len(target_values)):
+            if y[i] == target_values[j]:
+                lbl = "{}".format(labels[y[i]])
+                if indices is not None:
+                    lbl += " {}".format(indices[i])
+                plt.text(X[i, 0], X[i, 1], lbl,
+                         color=plt.cm.tab20(colors[j]),
+                         fontdict={'weight': 'bold', 'size': 9},alpha=alpha)
+                points[j].append([X[i, 0], X[i, 1]])
+                break
+    plt.xticks([]), plt.yticks([])
+    plt.tight_layout()
+    if title is not None:
+        plt.title(title)
+    plt.gca().axis('off')
+
+
+def plot_embedding_with_images(X, y, num_classes, images, face_colour="black", class_border=False, mask_level=(0.3, 0.7), scale_adj=1.0, figsize=None):
+    """
+    Scatter plot of classes and their 2D embedding. Instead of class name, the actual image is used.
+    The dark parts of the images will be masked (used mainly for foraminifera images)
+    :param X: The 2D co-ordinates of each class value
+    :param y: The classes
+    :param num_classes: Total number of classes
+    :param images: The images corresponding to each class entry
+    :param face_colour: Colour of the figure background
+    :param class_border: Make a border with the colour of the class (not implemented)
+    :param mask_level: Two values [0] is mask threshold, [1] is intensity above which everything is opaque
+    :param scale_adj:
+    :param figsize: Size of the figure. If None, it is scaled automatically (recommended)
+    :return:
+    """
+    # Normalise the co-ordinates
+    x_min, x_max = np.min(X, 0), np.max(X, 0)
+    X = (X - x_min) / (x_max - x_min)
+    # Calculate the scaling amount
+    scale = images.shape[1] // 64 / scale_adj
+    # Create the figure
+    if figsize is None:
+        figsize = (20*scale, 20*scale)
+    plt.figure(figsize=figsize, dpi=50, facecolor=face_colour, edgecolor=face_colour)
+    plt.gca().set_facecolor(face_colour)
+    # Plot
+    clrs = plt.cm.get_cmap('tab20')
+    for j in range(X.shape[0]):
+        img = np.squeeze(images[j,:,:,0])
+        # Create a mask with a soft border
+        # mask_level[0] is the threshold
+        # mask_level[1] is the intensity value above which everything is fully opaque
+        mask = img > mask_level[0]
+        mask = nd.morphology.binary_fill_holes(mask)
+        # if class_border:
+        #     clr = clrs(y/num_classes)
+        #     cmask = np.stack((mask*clr[0], mask*clr[1], mask*clr[2], np.ones(mask.shape)), axis=-1)
+        th = img / mask_level[1]
+        th[th > 1] = 1
+        th[mask == True] = 1
+        img = np.stack((img, img, img, th), axis=-1)
+        ab = AnnotationBbox(OffsetImage(img), (0.03 + X[j, 0]*0.94, 0.03 + X[j, 1] * 0.94), xycoords="axes fraction", frameon=False)
+        plt.gca().add_artist(ab)
+    plt.xticks([])
+    plt.yticks([])
+    plt.tight_layout()
+
+
+def plot_embedding_with_colour_images(X, images, face_colour="black", scale_adj=1.0, figsize=(10,10)):
+    # Normalise the co-ordinates
+    x_min, x_max = np.min(X, 0), np.max(X, 0)
+    X = (X - x_min) / (x_max - x_min)
+    # Calculate the scaling amount
+    scale = images.shape[1] // 64 / scale_adj
+    # Create the figure
+    if figsize is None:
+        figsize = (20*scale, 20*scale)
+    plt.figure(figsize=figsize, dpi=50, facecolor=face_colour, edgecolor=face_colour)
+    plt.gca().set_facecolor(face_colour)
+    # Plot
+    for j in range(X.shape[0]):
+        img = images[j,:,:,:]
+        ab = AnnotationBbox(OffsetImage(img), (0.03 + X[j, 0]*0.94, 0.03 + X[j, 1] * 0.94), xycoords="axes fraction", frameon=False)
+        plt.gca().add_artist(ab)
+    plt.xticks([])
+    plt.yticks([])
+    plt.tight_layout()
+
+
+def plot_embedding_with_images_on_grid(X, y, num_classes, images, width=128, mask_level=0.7, scale_adj=1.0):
+    """
+    2D image scatter plots, but with the images in a grid.
+    Requires lapjv which can be installed with 'pip install lapjv' BUT you need a C compiler installed as well
+    :param X:
+    :param y:
+    :param num_classes:
+    :param images:
+    :param width:
+    :param mask_level:
+    :param scale_adj:
+    :return:
+    """
+    grid_width = int(np.min((np.floor(np.sqrt(len(y))),20)))
+    grid = np.dstack(np.meshgrid(np.linspace(0, 1, grid_width), np.linspace(0, 1, grid_width))).reshape(-1, 2)
+    X = X[0:grid_width*grid_width,:]
+    x_min, x_max = np.min(X, 0), np.max(X, 0)
+    X = (X - x_min) / (x_max - x_min)
+    cost_matrix = cdist(grid, X, "sqeuclidean").astype(np.float32)
+    cost_matrix = cost_matrix * (100000 / cost_matrix.max())
+    row_asses, col_asses, _ = lapjv(cost_matrix)
+    grid_jv = grid[col_asses]
+    plot_embedding_with_images(grid_jv, y, num_classes, images, face_colour="black", class_border=False, mask_level=mask_level, scale_adj=scale_adj)
```

### Comparing `miso2-3.0.3/miso/stats/mislabelling.py` & `miso2-3.0.4/miso/stats/mislabelling.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-import matplotlib.pyplot as plt
-from sklearn.neighbors import KNeighborsClassifier
-import numpy as np
-from sklearn.utils.extmath import weighted_mode
-from sklearn.preprocessing import normalize
-import os
-
-from tqdm import tqdm
-
-
-def find_and_save_mislabelled(images,
-                              vectors,
-                              cls,
-                              cls_labels,
-                              image_names,
-                              output_dir,
-                              num_neighbours=11):
-    """
-    Uses nearest neighbour to classify the vectors and checks this matches the actual classifications.
-    If not, prints the most similar other images. Also writes to a csv file with this list.
-    Args:
-        images: Images (for use in plots)
-        vectors: Vectors for each image
-        cls: Class label for each image
-        cls_labels: List of class cls in order [class_0, class_1, ..., class_N]
-        image_names: List of ids for each image, e.g. their filenames
-        output_dir: Directory to save the results
-        num_neighbours: Number of neighbours to use for the kNN classification
-    Returns: None
-    """
-    # Normalise vectors
-    vectors = normalize(vectors, axis=1)
-    # Nearest neighbours fit
-    neigh = KNeighborsClassifier(n_neighbors=num_neighbours + 1, algorithm='brute')
-    neigh.fit(vectors, cls)
-
-    # Find the k nearest vectors
-    # The first will be the same vector as passed in so ignore it
-    knn = neigh.kneighbors(vectors, n_neighbors=num_neighbours + 1)
-    distance = knn[0][:, 1:]
-    idx = knn[1][:, 1:]
-    # Get the predicted class from knn (ignoring the same vector)
-    knn_cls = cls[idx]
-    wm = weighted_mode(knn_cls, np.max(distance) - distance, axis=1)
-    pred_cls = wm[0].astype(int).flatten()
-    pred_w = wm[1]
-
-    # Get the index of images with a different k-NN prediction to their label
-    diff_idx = np.where(cls != pred_cls)[0]
-
-    # Write a CSV of the mislabelled
-    with open(os.path.join(output_dir, "mislabeled.csv"), 'w+') as f:
-        f.write("filename, label, predicted_label\n")
-        for i in diff_idx:
-            f.write("{},{},{}\n".format(image_names[i], cls_labels[cls[i]], cls_labels[pred_cls[i]]))
-
-    if num_neighbours == 1:
-        nx = 2
-        ny = 1
-    elif num_neighbours == 2:
-        nx = 3
-        ny = 1
-    elif num_neighbours == 3:
-        nx = 2
-        ny = 2
-    elif num_neighbours == 5:
-        nx = 3
-        ny = 2
-    else:
-        nx = 4
-        ny = int(np.ceil((num_neighbours + 1) / 4))
-
-    # Plot each image
-    for im_idx in tqdm(diff_idx):
-        fig, axes = plt.subplots(nrows=ny, ncols=nx, figsize=(2 * nx, 2 * ny + 1),
-                                 gridspec_kw={"top": (2 * ny + 0.5) / (2 * ny + 1),
-                                              "left": 0.05,
-                                              "right": 0.95,
-                                              "bottom": 0.5 / (2 * ny + 1)})
-        plt.set_cmap('gray')
-        fig.set_facecolor("white")
-        for i, ax in enumerate(axes.flat):
-            if i == 0:
-                image = images[im_idx].astype(np.uint8)
-                if images.shape[3] == 1:
-                    ax.imshow(image[:, :, 0])
-                else:
-                    ax.imshow(image)
-                if cls_labels is None:
-                    xlabel = "{0}\n({1})?".format(cls[im_idx], pred_cls[im_idx])
-                else:
-                    xlabel = "{0}\n{1}?".format(cls_labels[cls[im_idx]], cls_labels[pred_cls[im_idx]])
-                ax.set_xlabel(xlabel)
-            else:
-                kidx = idx[im_idx, i - 1]
-                image = images[kidx].astype(np.uint8)
-                if images.shape[3] == 1:
-                    ax.imshow(image[:, :, 0])
-                else:
-                    ax.imshow(image)
-                if cls_labels is None:
-                    xlabel = "{0}".format(cls[kidx])
-                else:
-                    xlabel = "{0}".format(cls_labels[cls[kidx]])
-                ax.set_xlabel(xlabel)
-            # Remove ticks from the plot.
-            ax.set_xticks([])
-            ax.set_yticks([])
-        # Tight layout looks nicer
-        fig.tight_layout()
-        plt.suptitle(image_names[im_idx])
-        # print("- actual: {} predicted: {} - {}".format(cls_labels[cls[im_idx]], cls_labels[pred_cls[im_idx]], image_names[im_idx]))
-        os.makedirs(os.path.join(output_dir,
-                                 "mislabeled",
-                                 cls_labels[cls[im_idx]]).replace("\\", "/"),
-                    exist_ok=True)
-        plt.savefig(os.path.join(output_dir,
-                                 "mislabeled",
-                                 cls_labels[cls[im_idx]],
-                                 image_names[im_idx]).replace("\\", "/"))
-        plt.clf()
-        plt.close('all')
+import matplotlib.pyplot as plt
+from sklearn.neighbors import KNeighborsClassifier
+import numpy as np
+from sklearn.utils.extmath import weighted_mode
+from sklearn.preprocessing import normalize
+import os
+
+from tqdm import tqdm
+
+
+def find_and_save_mislabelled(images,
+                              vectors,
+                              cls,
+                              cls_labels,
+                              image_names,
+                              output_dir,
+                              num_neighbours=11):
+    """
+    Uses nearest neighbour to classify the vectors and checks this matches the actual classifications.
+    If not, prints the most similar other images. Also writes to a csv file with this list.
+    Args:
+        images: Images (for use in plots)
+        vectors: Vectors for each image
+        cls: Class label for each image
+        cls_labels: List of class cls in order [class_0, class_1, ..., class_N]
+        image_names: List of ids for each image, e.g. their filenames
+        output_dir: Directory to save the results
+        num_neighbours: Number of neighbours to use for the kNN classification
+    Returns: None
+    """
+    # Normalise vectors
+    vectors = normalize(vectors, axis=1)
+    # Nearest neighbours fit
+    neigh = KNeighborsClassifier(n_neighbors=num_neighbours + 1, algorithm='brute')
+    neigh.fit(vectors, cls)
+
+    # Find the k nearest vectors
+    # The first will be the same vector as passed in so ignore it
+    knn = neigh.kneighbors(vectors, n_neighbors=num_neighbours + 1)
+    distance = knn[0][:, 1:]
+    idx = knn[1][:, 1:]
+    # Get the predicted class from knn (ignoring the same vector)
+    knn_cls = cls[idx]
+    wm = weighted_mode(knn_cls, np.max(distance) - distance, axis=1)
+    pred_cls = wm[0].astype(int).flatten()
+    pred_w = wm[1]
+
+    # Get the index of images with a different k-NN prediction to their label
+    diff_idx = np.where(cls != pred_cls)[0]
+
+    # Write a CSV of the mislabelled
+    with open(os.path.join(output_dir, "mislabeled.csv"), 'w+') as f:
+        f.write("filename, label, predicted_label\n")
+        for i in diff_idx:
+            f.write("{},{},{}\n".format(image_names[i], cls_labels[cls[i]], cls_labels[pred_cls[i]]))
+
+    if num_neighbours == 1:
+        nx = 2
+        ny = 1
+    elif num_neighbours == 2:
+        nx = 3
+        ny = 1
+    elif num_neighbours == 3:
+        nx = 2
+        ny = 2
+    elif num_neighbours == 5:
+        nx = 3
+        ny = 2
+    else:
+        nx = 4
+        ny = int(np.ceil((num_neighbours + 1) / 4))
+
+    # Plot each image
+    for im_idx in tqdm(diff_idx):
+        fig, axes = plt.subplots(nrows=ny, ncols=nx, figsize=(2 * nx, 2 * ny + 1),
+                                 gridspec_kw={"top": (2 * ny + 0.5) / (2 * ny + 1),
+                                              "left": 0.05,
+                                              "right": 0.95,
+                                              "bottom": 0.5 / (2 * ny + 1)})
+        plt.set_cmap('gray')
+        fig.set_facecolor("white")
+        for i, ax in enumerate(axes.flat):
+            if i == 0:
+                image = images[im_idx].astype(np.uint8)
+                if images.shape[3] == 1:
+                    ax.imshow(image[:, :, 0])
+                else:
+                    ax.imshow(image)
+                if cls_labels is None:
+                    xlabel = "{0}\n({1})?".format(cls[im_idx], pred_cls[im_idx])
+                else:
+                    xlabel = "{0}\n{1}?".format(cls_labels[cls[im_idx]], cls_labels[pred_cls[im_idx]])
+                ax.set_xlabel(xlabel)
+            else:
+                kidx = idx[im_idx, i - 1]
+                image = images[kidx].astype(np.uint8)
+                if images.shape[3] == 1:
+                    ax.imshow(image[:, :, 0])
+                else:
+                    ax.imshow(image)
+                if cls_labels is None:
+                    xlabel = "{0}".format(cls[kidx])
+                else:
+                    xlabel = "{0}".format(cls_labels[cls[kidx]])
+                ax.set_xlabel(xlabel)
+            # Remove ticks from the plot.
+            ax.set_xticks([])
+            ax.set_yticks([])
+        # Tight layout looks nicer
+        fig.tight_layout()
+        plt.suptitle(image_names[im_idx])
+        # print("- actual: {} predicted: {} - {}".format(cls_labels[cls[im_idx]], cls_labels[pred_cls[im_idx]], image_names[im_idx]))
+        os.makedirs(os.path.join(output_dir,
+                                 "mislabeled",
+                                 cls_labels[cls[im_idx]]).replace("\\", "/"),
+                    exist_ok=True)
+        plt.savefig(os.path.join(output_dir,
+                                 "mislabeled",
+                                 cls_labels[cls[im_idx]],
+                                 image_names[im_idx]).replace("\\", "/"))
+        plt.clf()
+        plt.close('all')
```

### Comparing `miso2-3.0.3/miso/stats/most_representative.py` & `miso2-3.0.4/miso/stats/most_representative.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import os
-import numpy as np
-import matplotlib.pyplot as plt
-from sklearn.neighbors.nearest_centroid import NearestCentroid
-from sklearn.preprocessing import normalize
-from sklearn.metrics import pairwise_distances_argmin_min
-
-
-def plot_most_representative(images, vectors, cls, cls_labels, output_dir):
-    # Normalise vectors
-    vectors = normalize(vectors, axis=1)
-    # Find centroids
-    clf = NearestCentroid()
-    clf.fit(vectors, cls)
-    # Get nearest
-    im_idx, dist = pairwise_distances_argmin_min(clf.centroids_, vectors)
-
-    for i, idx in enumerate(im_idx):
-        plt.clf()
-        plt.imshow(images[idx])
-        plt.axis('off')
-        plt.title('{}  -  {}'.format(i, cls_labels[i]))
-        plt.tight_layout()
-        plt.show()
-        output_file = os.path.join(output_dir, 'archetypes', '{}_{}.png'.format(i, cls_labels[i]))
-        plt.imsave(output_file)
-
+import os
+import numpy as np
+import matplotlib.pyplot as plt
+from sklearn.neighbors.nearest_centroid import NearestCentroid
+from sklearn.preprocessing import normalize
+from sklearn.metrics import pairwise_distances_argmin_min
+
+
+def plot_most_representative(images, vectors, cls, cls_labels, output_dir):
+    # Normalise vectors
+    vectors = normalize(vectors, axis=1)
+    # Find centroids
+    clf = NearestCentroid()
+    clf.fit(vectors, cls)
+    # Get nearest
+    im_idx, dist = pairwise_distances_argmin_min(clf.centroids_, vectors)
+
+    for i, idx in enumerate(im_idx):
+        plt.clf()
+        plt.imshow(images[idx])
+        plt.axis('off')
+        plt.title('{}  -  {}'.format(i, cls_labels[i]))
+        plt.tight_layout()
+        plt.show()
+        output_file = os.path.join(output_dir, 'archetypes', '{}_{}.png'.format(i, cls_labels[i]))
+        plt.imsave(output_file)
+
```

### Comparing `miso2-3.0.3/miso/stats/training.py` & `miso2-3.0.4/miso/stats/training.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-Plots of training and accuracy
-"""
-import numpy as np
-from tensorflow.keras.callbacks import History
-import matplotlib.pyplot as plt
-
-
-def plot_loss_vs_epochs(history: History, figsize=(8, 4)):
-    epochs = history.epoch
-    loss = history.history['loss']
-    val_loss = history.history['val_loss']
-    plt.figure(figsize=figsize)
-    plt.plot(epochs, loss)
-    plt.plot(epochs, val_loss)
-    plt.grid()
-    plt.title("Loss")
-    plt.legend(("Training", "Validation"))
-    plt.xlim(left=0)
-    plt.ylim(bottom=0)
-
-
-def plot_accuracy_vs_epochs(history: History, metric='acc', figsize=(8, 4)):
-    epochs = history.epoch
-    acc = np.asarray(history.history[metric])
-    val_acc = np.asarray(history.history['val_' + metric])
-    plt.figure(figsize=figsize)
-    plt.plot(epochs, acc * 100)
-    plt.plot(epochs, val_acc * 100)
-    plt.grid()
-    plt.title("Accuracy")
-    plt.legend(("Training", "Validation"))
-    plt.xlim(left=0)
-    plt.ylim(top=100)
-
-
+"""
+Plots of training and accuracy
+"""
+import numpy as np
+from tensorflow.keras.callbacks import History
+import matplotlib.pyplot as plt
+
+
+def plot_loss_vs_epochs(history: History, figsize=(8, 4)):
+    epochs = history.epoch
+    loss = history.history['loss']
+    val_loss = history.history['val_loss']
+    plt.figure(figsize=figsize)
+    plt.plot(epochs, loss)
+    plt.plot(epochs, val_loss)
+    plt.grid()
+    plt.title("Loss")
+    plt.legend(("Training", "Validation"))
+    plt.xlim(left=0)
+    plt.ylim(bottom=0)
+
+
+def plot_accuracy_vs_epochs(history: History, metric='acc', figsize=(8, 4)):
+    epochs = history.epoch
+    acc = np.asarray(history.history[metric])
+    val_acc = np.asarray(history.history['val_' + metric])
+    plt.figure(figsize=figsize)
+    plt.plot(epochs, acc * 100)
+    plt.plot(epochs, val_acc * 100)
+    plt.grid()
+    plt.title("Accuracy")
+    plt.legend(("Training", "Validation"))
+    plt.xlim(left=0)
+    plt.ylim(top=100)
+
+
```

### Comparing `miso2-3.0.3/miso/training/adaptive_learning_rate.py` & `miso2-3.0.4/miso/training/adaptive_learning_rate.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import tensorflow as tf
-from tensorflow.keras.callbacks import Callback
-import tensorflow.keras.backend as K
-from miso.utils.rolling_buffer import RollingBuffer
-import math
-import time
-
-
-def graph_to_console(epoch, batch, acc, loss, val_acc, val_loss, lr_prob, lr_prob_active, time_difference):
-    acc_i = round(acc * 50)
-    val_acc_i = round(val_acc * 50)
-    lr_prob_i = round(lr_prob * 50)
-
-    for j in range(51):
-        if j == acc_i:
-            print('#', end="")
-        # elif j == trainsdi:
-        #     print('@', end="")
-        elif j == val_acc_i:
-            print('*', end="")
-        elif j == lr_prob_i and j != 100 and lr_prob_active:
-            print('+', end="")
-        elif j % 10 == 0:
-            print('|', end="")
-        else:
-            print(' ', end="")
-    # msg = " {} #T {:.1f}%/{:.4f}, *V {:.1f}%/{:.4f} ({:.2f}s)"
-    # print(msg.format(epoch, acc * 100, loss, val_acc * 100, val_loss, time_difference))
-    msg = " {} #T{:.1f}%/*V{:.1f}% ({:.2f}s)"
-    print(msg.format(epoch, acc * 100, val_acc * 100, time_difference))
-
-
-class AdaptiveLearningRateScheduler(Callback):
-    """
-    Adaptive learning rate scheduler
-
-    Decreases learning rate by a certain factor each time it is no longer improving
-    """
-
-    def __init__(self, drop_rate=0.5, nb_drops=4, nb_epochs=10, verbose=1, monitor='loss'):
-        super(AdaptiveLearningRateScheduler, self).__init__()
-        self.monitor = monitor
-        self.drop_rate = drop_rate
-        self.nb_drops = nb_drops
-        self.nb_epochs = nb_epochs
-        self.verbose = verbose
-        self.current_epoch = 0
-        self.current_batch = 0
-        self.drop_count = 0
-        self.buffer = None
-        self.previous_time = None
-        self.finished = False
-
-    def on_train_begin(self, logs=None):
-        # if 'batch_size' in self.params and self.params['batch_size'] is not None:
-        #     batch_size = self.params['batch_size']
-        #     samples = self.params['samples']
-        #     self.buffer = RollingBuffer(math.ceil(samples * self.nb_epochs / batch_size))
-        # else:
-        self.buffer = RollingBuffer(self.nb_epochs)
-        self.previous_time = time.time()
-
-    def on_epoch_begin(self, epoch, logs=None):
-        self.current_epoch = epoch
-
-    def on_epoch_end(self, epoch, logs=None):
-        loss = logs.get("loss")
-        acc = logs.get("acc") or logs.get('accuracy') or logs.get('iou_score') or logs.get('cosine_proximity')
-        val_loss = logs.get("val_loss") or 0
-        val_acc = logs.get("val_acc") or logs.get('val_accuracy') or logs.get('val_iou_score') or logs.get(
-            'val_cosine_proximity') or 0
-        if 'cosine_proximity' in logs:
-            acc += 1
-            val_acc += 1
-
-        # Elapsed time
-        current_time = time.time()
-        if self.previous_time is None:
-            time_difference = 0
-        else:
-            time_difference = current_time - self.previous_time
-        self.previous_time = current_time
-
-        # Update learning rate
-        self.update_learning_rate(self.current_epoch, logs)
-
-        # Graph to console
-        if val_acc is not None:
-            print("\r", end="")
-            graph_to_console(self.current_epoch, self.current_batch,
-                             acc, loss, val_acc, val_loss,
-                             self.buffer.slope_probability_less_than(0), self.buffer.full(),
-                             time_difference)
-
-        if self.finished is True:
-            self.model.stop_training = True
-            print("Training finished".format(self.model.optimizer.lr))
-
-    def on_batch_end(self, batch, logs=None):
-        self.current_batch += 1
-
-    def update_learning_rate(self, count, logs):
-        monitor_value = logs.get(self.monitor)
-        self.buffer.append(monitor_value)
-
-        if count >= self.buffer.length() * 3 and self.buffer.full() and self.finished is False:
-            # if count % 20 == 19:
-            #     lr = float(K.get_value(self.model.optimizer.lr))
-            #     new_lr = lr * self.drop_rate
-            #     K.set_value(self.model.optimizer.lr, new_lr)
-            #     print("Learning rate dropped ({}/{}) to {}".format(self.drop_count, self.nb_drops, new_lr))
-            if self.buffer.slope_probability_less_than(0) < 0.50:
-                lr = float(K.get_value(self.model.optimizer.lr))
-                # lr = self.model.optimizer.lr.read_value()
-                new_lr = lr * self.drop_rate
-                K.set_value(self.model.optimizer.lr, new_lr)
-                # self.model.optimizer.lr.assign(new_lr)
-                self.buffer.clear()
-                self.drop_count += 1
-                if self.drop_count == self.nb_drops:
-                    self.finished = True
-                    return
-                if self.verbose == 1:
-                    print("Learning rate dropped ({}/{}) to {}".format(self.drop_count, self.nb_drops, new_lr))
+import tensorflow as tf
+from tensorflow.keras.callbacks import Callback
+import tensorflow.keras.backend as K
+from miso.utils.rolling_buffer import RollingBuffer
+import math
+import time
+
+
+def graph_to_console(epoch, batch, acc, loss, val_acc, val_loss, lr_prob, lr_prob_active, time_difference):
+    acc_i = round(acc * 50)
+    val_acc_i = round(val_acc * 50)
+    lr_prob_i = round(lr_prob * 50)
+
+    for j in range(51):
+        if j == acc_i:
+            print('#', end="")
+        # elif j == trainsdi:
+        #     print('@', end="")
+        elif j == val_acc_i:
+            print('*', end="")
+        elif j == lr_prob_i and j != 100 and lr_prob_active:
+            print('+', end="")
+        elif j % 10 == 0:
+            print('|', end="")
+        else:
+            print(' ', end="")
+    # msg = " {} #T {:.1f}%/{:.4f}, *V {:.1f}%/{:.4f} ({:.2f}s)"
+    # print(msg.format(epoch, acc * 100, loss, val_acc * 100, val_loss, time_difference))
+    msg = " {} #T{:.1f}%/*V{:.1f}% ({:.2f}s)"
+    print(msg.format(epoch, acc * 100, val_acc * 100, time_difference))
+
+
+class AdaptiveLearningRateScheduler(Callback):
+    """
+    Adaptive learning rate scheduler
+
+    Decreases learning rate by a certain factor each time it is no longer improving
+    """
+
+    def __init__(self, drop_rate=0.5, nb_drops=4, nb_epochs=10, verbose=1, monitor='loss'):
+        super(AdaptiveLearningRateScheduler, self).__init__()
+        self.monitor = monitor
+        self.drop_rate = drop_rate
+        self.nb_drops = nb_drops
+        self.nb_epochs = nb_epochs
+        self.verbose = verbose
+        self.current_epoch = 0
+        self.current_batch = 0
+        self.drop_count = 0
+        self.buffer = None
+        self.previous_time = None
+        self.finished = False
+
+    def on_train_begin(self, logs=None):
+        # if 'batch_size' in self.params and self.params['batch_size'] is not None:
+        #     batch_size = self.params['batch_size']
+        #     samples = self.params['samples']
+        #     self.buffer = RollingBuffer(math.ceil(samples * self.nb_epochs / batch_size))
+        # else:
+        self.buffer = RollingBuffer(self.nb_epochs)
+        self.previous_time = time.time()
+
+    def on_epoch_begin(self, epoch, logs=None):
+        self.current_epoch = epoch
+
+    def on_epoch_end(self, epoch, logs=None):
+        loss = logs.get("loss")
+        acc = logs.get("acc") or logs.get('accuracy') or logs.get('iou_score') or logs.get('cosine_proximity')
+        val_loss = logs.get("val_loss") or 0
+        val_acc = logs.get("val_acc") or logs.get('val_accuracy') or logs.get('val_iou_score') or logs.get(
+            'val_cosine_proximity') or 0
+        if 'cosine_proximity' in logs:
+            acc += 1
+            val_acc += 1
+
+        # Elapsed time
+        current_time = time.time()
+        if self.previous_time is None:
+            time_difference = 0
+        else:
+            time_difference = current_time - self.previous_time
+        self.previous_time = current_time
+
+        # Update learning rate
+        self.update_learning_rate(self.current_epoch, logs)
+
+        # Graph to console
+        if val_acc is not None:
+            print("\r", end="")
+            graph_to_console(self.current_epoch, self.current_batch,
+                             acc, loss, val_acc, val_loss,
+                             self.buffer.slope_probability_less_than(0), self.buffer.full(),
+                             time_difference)
+
+        if self.finished is True:
+            self.model.stop_training = True
+            print("Training finished".format(self.model.optimizer.lr))
+
+    def on_batch_end(self, batch, logs=None):
+        self.current_batch += 1
+
+    def update_learning_rate(self, count, logs):
+        monitor_value = logs.get(self.monitor)
+        self.buffer.append(monitor_value)
+
+        if count >= self.buffer.length() * 3 and self.buffer.full() and self.finished is False:
+            # if count % 20 == 19:
+            #     lr = float(K.get_value(self.model.optimizer.lr))
+            #     new_lr = lr * self.drop_rate
+            #     K.set_value(self.model.optimizer.lr, new_lr)
+            #     print("Learning rate dropped ({}/{}) to {}".format(self.drop_count, self.nb_drops, new_lr))
+            if self.buffer.slope_probability_less_than(0) < 0.50:
+                lr = float(K.get_value(self.model.optimizer.lr))
+                # lr = self.model.optimizer.lr.read_value()
+                new_lr = lr * self.drop_rate
+                K.set_value(self.model.optimizer.lr, new_lr)
+                # self.model.optimizer.lr.assign(new_lr)
+                self.buffer.clear()
+                self.drop_count += 1
+                if self.drop_count == self.nb_drops:
+                    self.finished = True
+                    return
+                if self.verbose == 1:
+                    print("Learning rate dropped ({}/{}) to {}".format(self.drop_count, self.nb_drops, new_lr))
```

### Comparing `miso2-3.0.3/miso/training/tf_augmentation.py` & `miso2-3.0.4/miso/training/tf_augmentation.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-import tensorflow as tf
-import numpy as np
-
-if int(tf.__version__[0]) == 2:
-    try:
-        import tensorflow_addons as tfa
-    except ImportError:
-        pass
-
-
-def aug_all_fn(rotation=(0, 360),
-               gain=(0.8, 1.0, 1.2),
-               gamma=(0.5, 1.0, 2),
-               zoom=(0.9, 1.0, 1.1),
-               gaussian_noise=None,
-               bias=None,
-               random_crop=None,
-               divide=255):
-    def wrapper(im_x):
-        im_x = tf.cast(im_x, tf.float32)
-        if divide is not None:
-            im_x = tf.divide(im_x, tf.constant(divide, dtype=tf.float32))
-        im_x = aug_rotation(im_x, rotation)
-        im_x = aug_zoom(im_x, zoom)
-        im_x = aug_gain_gamma(im_x, gain, gamma)
-        im_x = aug_gaussian_noise(im_x, gaussian_noise)
-        im_x = aug_bias(im_x, bias)
-        im_x = aug_random_crop(im_x, random_crop)
-        return im_x
-    return wrapper
-
-
-def aug_rotation(im_x, rotation=(0, 360)):
-    if rotation is not None:
-        if len(rotation) > 2:
-            rotation_factor = tf.random.shuffle(tf.constant(rotation))[0]
-        elif len(rotation) == 2:
-            rotation_factor = tf.random.uniform([], rotation[0] / 180 * np.pi, rotation[1] / 180 * np.pi)
-        else:
-            raise ValueError("Rotation needs at least 2 values")
-        if int(tf.__version__[0]) == 2:
-            im_x = tfa.image.rotate(im_x, rotation_factor, interpolation='bilinear')
-        else:
-            im_x = tf.contrib.image.rotate(im_x, rotation_factor, interpolation='BILINEAR')
-    return im_x
-
-
-def aug_zoom(im_x, zoom=(0.9, 1.0, 1.1)):
-    if zoom is not None:
-        if len(zoom) > 2:
-            zoom_value = tf.random.shuffle(tf.constant(zoom))[0]
-        elif len(zoom) == 2:
-            zoom_value = tf.random.uniform([], zoom[0], zoom[1])
-        else:
-            raise ValueError("Zoom needs at least 2 values")
-        zoom_start_factor = tf.divide(tf.subtract(1.0, zoom_value), 2)
-        zoom_end_factor = tf.subtract(1.0, zoom_start_factor)
-        zoom_factor = [[zoom_start_factor, zoom_start_factor, zoom_end_factor, zoom_end_factor]]
-        if int(tf.__version__[0]) == 2:
-            im_x = tf.image.crop_and_resize([im_x],
-                                            boxes=zoom_factor,
-                                            box_indices=tf.constant([0]),
-                                            crop_size=tf.shape(im_x)[0:2],
-                                            method='bilinear',
-                                            extrapolation_value=0)[0]
-        else:
-            im_x = tf.image.crop_and_resize([im_x],
-                                            boxes=zoom_factor,
-                                            box_ind=tf.constant([0]),
-                                            crop_size=tf.shape(im_x)[0:2],
-                                            method='bilinear',
-                                            extrapolation_value=0)[0]
-    return im_x
-
-
-def aug_gain_gamma(im_x, gain=(0.8, 1.0, 1.2), gamma=(0.5, 1.0, 2)):
-    # Gain
-    if gain is not None:
-        if len(gain) > 2:
-            gain_factor = tf.random.shuffle(tf.constant(gain))[0]
-        elif len(gain) == 2:
-            gain_factor = tf.random.uniform([], gain[0], gain[1])
-        else:
-            raise ValueError("Gain needs at least 2 values")
-    else:
-        gain_factor = tf.constant(1.0)
-    # Gamma
-    if gamma is not None:
-        if len(gamma) > 2:
-            gamma_factor = tf.random.shuffle(tf.constant(gamma))[0]
-        elif len(gamma) == 2:
-            gamma_factor = tf.random.uniform([], gamma[0], gamma[1])
-        else:
-            raise ValueError("Gamma needs at least 2 values")
-    else:
-        gamma_factor = tf.constant(1.0)
-    if gamma is not None or gain is not None:
-        im_x = tf.image.adjust_gamma(im_x, gamma_factor, gain_factor)
-    return im_x
-
-
-def aug_gaussian_noise(im_x, gaussian_noise=None):
-    shape = tf.shape(im_x)
-    if gaussian_noise is not None:
-        if len(gaussian_noise) > 2:
-            gaussian_noise_factor = tf.random.shuffle(tf.constant(gaussian_noise))[0]
-        elif len(gaussian_noise) == 2:
-            gaussian_noise_factor = tf.random.uniform([], gaussian_noise[0], gaussian_noise[1])
-        else:
-            raise ValueError("Noise needs at least 2 values")
-        noise_tensor = tf.random.normal(shape,
-                                        mean=0.0,
-                                        stddev=gaussian_noise_factor,
-                                        dtype=tf.float32,
-                                        seed=None,
-                                        name=None)
-        im_x = tf.add(im_x, noise_tensor)
-    return im_x
-
-
-def aug_bias(im_x, bias=(-0.5, 0.5)):
-    if bias is not None:
-        if len(bias) > 2:
-            bias_factor = tf.random.shuffle(tf.constant(bias))[0]
-        elif len(bias) == 2:
-            bias_factor = tf.random.uniform([], bias[0], bias[1])
-        else:
-            raise ValueError("Offset needs at least 2 values")
-        im_x = tf.add(im_x, bias_factor)
-    return im_x
-
-
-def aug_random_crop(im_x, crop_size):
-    if crop_size is not None:
-        im_x = tf.image.random_crop(im_x, crop_size)
-    return im_x
+import tensorflow as tf
+import numpy as np
+
+if int(tf.__version__[0]) == 2:
+    try:
+        import tensorflow_addons as tfa
+    except ImportError:
+        pass
+
+
+def aug_all_fn(rotation=(0, 360),
+               gain=(0.8, 1.0, 1.2),
+               gamma=(0.5, 1.0, 2),
+               zoom=(0.9, 1.0, 1.1),
+               gaussian_noise=None,
+               bias=None,
+               random_crop=None,
+               divide=255):
+    def wrapper(im_x):
+        im_x = tf.cast(im_x, tf.float32)
+        if divide is not None:
+            im_x = tf.divide(im_x, tf.constant(divide, dtype=tf.float32))
+        im_x = aug_rotation(im_x, rotation)
+        im_x = aug_zoom(im_x, zoom)
+        im_x = aug_gain_gamma(im_x, gain, gamma)
+        im_x = aug_gaussian_noise(im_x, gaussian_noise)
+        im_x = aug_bias(im_x, bias)
+        im_x = aug_random_crop(im_x, random_crop)
+        return im_x
+    return wrapper
+
+
+def aug_rotation(im_x, rotation=(0, 360)):
+    if rotation is not None:
+        if len(rotation) > 2:
+            rotation_factor = tf.random.shuffle(tf.constant(rotation))[0]
+        elif len(rotation) == 2:
+            rotation_factor = tf.random.uniform([], rotation[0] / 180 * np.pi, rotation[1] / 180 * np.pi)
+        else:
+            raise ValueError("Rotation needs at least 2 values")
+        if int(tf.__version__[0]) == 2:
+            im_x = tfa.image.rotate(im_x, rotation_factor, interpolation='bilinear')
+        else:
+            im_x = tf.contrib.image.rotate(im_x, rotation_factor, interpolation='BILINEAR')
+    return im_x
+
+
+def aug_zoom(im_x, zoom=(0.9, 1.0, 1.1)):
+    if zoom is not None:
+        if len(zoom) > 2:
+            zoom_value = tf.random.shuffle(tf.constant(zoom))[0]
+        elif len(zoom) == 2:
+            zoom_value = tf.random.uniform([], zoom[0], zoom[1])
+        else:
+            raise ValueError("Zoom needs at least 2 values")
+        zoom_start_factor = tf.divide(tf.subtract(1.0, zoom_value), 2)
+        zoom_end_factor = tf.subtract(1.0, zoom_start_factor)
+        zoom_factor = [[zoom_start_factor, zoom_start_factor, zoom_end_factor, zoom_end_factor]]
+        if int(tf.__version__[0]) == 2:
+            im_x = tf.image.crop_and_resize([im_x],
+                                            boxes=zoom_factor,
+                                            box_indices=tf.constant([0]),
+                                            crop_size=tf.shape(im_x)[0:2],
+                                            method='bilinear',
+                                            extrapolation_value=0)[0]
+        else:
+            im_x = tf.image.crop_and_resize([im_x],
+                                            boxes=zoom_factor,
+                                            box_ind=tf.constant([0]),
+                                            crop_size=tf.shape(im_x)[0:2],
+                                            method='bilinear',
+                                            extrapolation_value=0)[0]
+    return im_x
+
+
+def aug_gain_gamma(im_x, gain=(0.8, 1.0, 1.2), gamma=(0.5, 1.0, 2)):
+    # Gain
+    if gain is not None:
+        if len(gain) > 2:
+            gain_factor = tf.random.shuffle(tf.constant(gain))[0]
+        elif len(gain) == 2:
+            gain_factor = tf.random.uniform([], gain[0], gain[1])
+        else:
+            raise ValueError("Gain needs at least 2 values")
+    else:
+        gain_factor = tf.constant(1.0)
+    # Gamma
+    if gamma is not None:
+        if len(gamma) > 2:
+            gamma_factor = tf.random.shuffle(tf.constant(gamma))[0]
+        elif len(gamma) == 2:
+            gamma_factor = tf.random.uniform([], gamma[0], gamma[1])
+        else:
+            raise ValueError("Gamma needs at least 2 values")
+    else:
+        gamma_factor = tf.constant(1.0)
+    if gamma is not None or gain is not None:
+        im_x = tf.image.adjust_gamma(im_x, gamma_factor, gain_factor)
+    return im_x
+
+
+def aug_gaussian_noise(im_x, gaussian_noise=None):
+    shape = tf.shape(im_x)
+    if gaussian_noise is not None:
+        if len(gaussian_noise) > 2:
+            gaussian_noise_factor = tf.random.shuffle(tf.constant(gaussian_noise))[0]
+        elif len(gaussian_noise) == 2:
+            gaussian_noise_factor = tf.random.uniform([], gaussian_noise[0], gaussian_noise[1])
+        else:
+            raise ValueError("Noise needs at least 2 values")
+        noise_tensor = tf.random.normal(shape,
+                                        mean=0.0,
+                                        stddev=gaussian_noise_factor,
+                                        dtype=tf.float32,
+                                        seed=None,
+                                        name=None)
+        im_x = tf.add(im_x, noise_tensor)
+    return im_x
+
+
+def aug_bias(im_x, bias=(-0.5, 0.5)):
+    if bias is not None:
+        if len(bias) > 2:
+            bias_factor = tf.random.shuffle(tf.constant(bias))[0]
+        elif len(bias) == 2:
+            bias_factor = tf.random.uniform([], bias[0], bias[1])
+        else:
+            raise ValueError("Offset needs at least 2 values")
+        im_x = tf.add(im_x, bias_factor)
+    return im_x
+
+
+def aug_random_crop(im_x, crop_size):
+    if crop_size is not None:
+        im_x = tf.image.random_crop(im_x, crop_size)
+    return im_x
```

### Comparing `miso2-3.0.3/miso/training/trainer.py` & `miso2-3.0.4/miso/training/trainer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,689 +1,666 @@
-"""
-Creates and trains a generic network
-"""
-import os
-import skimage.io
-import warnings
-
-warnings.simplefilter(action="ignore", category=FutureWarning)
-
-import time
-import datetime
-from collections import OrderedDict
-import tensorflow.keras.backend as K
-from sklearn.manifold import TSNE
-
-from miso.data.tf_generator import TFGenerator
-from miso.data.training_dataset import TrainingDataset
-from miso.stats.embedding import plot_embedding
-from miso.stats.mislabelling import find_and_save_mislabelled
-from miso.training.adaptive_learning_rate import AdaptiveLearningRateScheduler
-from miso.training.training_result import TrainingResult
-from miso.stats.confusion_matrix import *
-from miso.stats.training import *
-from miso.training.tf_augmentation import aug_all_fn
-from miso.deploy.saving import (
-    freeze,
-    convert_to_inference_mode,
-    save_frozen_model_tf2,
-    convert_to_inference_mode_tf2,
-    load_from_xml,
-    save_model_as_onnx,
-)
-from miso.deploy.model_info import ModelInfo
-from miso.models.factory import *
-
-import matplotlib.pyplot as plt
-import pandas as pd
-
-
-def predict_in_batches(model, generator):
-    results = []
-    try:
-        for x, y in iter(generator):
-            results.append(model.predict(x))
-    except tf.errors.OutOfRangeError:
-        pass
-    results = np.concatenate(results, axis=0)
-    return results
-
-
-def train_image_classification_model(tp: MisoParameters):
-    tf_version = int(tf.__version__[0])
-
-    # Hack to make RTX cards work
-    if tf_version == 2:
-        physical_devices = tf.config.list_physical_devices("GPU")
-        for device in physical_devices:
-            tf.config.experimental.set_memory_growth(device, True)
-    else:
-        config = tf.ConfigProto()
-        config.gpu_options.allow_growth = True
-        session = tf.Session(config=config)
-
-    K.clear_session()
-
-    # Clean the training parameters
-    tp.sanitise()
-
-    print(
-        "+---------------------------------------------------------------------------+"
-    )
-    print(
-        "| MISO Particle Classification Library                                      |"
-    )
-    print(
-        "+---------------------------------------------------------------------------+"
-    )
-    print(
-        "| Stable version:                                                           |"
-    )
-    print(
-        "| pip install miso2                                                         |"
-    )
-    print(
-        "| Development version:                                                      |"
-    )
-    print(
-        "| pip install git+http://www.github.com/microfossil/particle-classification |"
-    )
-    print(
-        "+---------------------------------------------------------------------------+"
-    )
-    print("Tensorflow version: {}".format(tf.__version__))
-    print("-" * 80)
-    print("Train information:")
-    print("- name: {}".format(tp.name))
-    print("- description: {}".format(tp.description))
-    print("- CNN type: {}".format(tp.cnn.id))
-    print("- image type: {}".format(tp.cnn.img_type))
-    print("- image shape: {}".format(tp.cnn.img_shape))
-    print()
-
-    # Load data
-    ds = TrainingDataset(
-        tp.dataset.source,
-        tp.cnn.img_shape,
-        tp.cnn.img_type,
-        tp.dataset.min_count,
-        tp.dataset.map_others,
-        tp.dataset.val_split,
-        tp.dataset.random_seed,
-        tp.dataset.memmap_directory,
-    )
-    ds.load()
-    tp.dataset.num_classes = ds.num_classes
-
-    # Create save lodations
-    now = datetime.datetime.now()
-    save_dir = os.path.join(
-        tp.output.save_dir, "{0}_{1:%Y%m%d-%H%M%S}".format(tp.name, now)
-    )
-    os.makedirs(save_dir, exist_ok=True)
-
-    # ------------------------------------------------------------------------------
-    # Transfer learning
-    # ------------------------------------------------------------------------------
-    if tp.cnn.id.endswith("tl"):
-        print("-" * 80)
-        print("Transfer learning network training")
-        start = time.time()
-
-        # Generate head model and predict vectors
-        model_head = generate_tl_head(tp.cnn.id, tp.cnn.img_shape)
-
-        # Calculate vectors
-        print("- calculating vectors")
-        t = time.time()
-        gen = ds.images.create_generator(
-            tp.training.batch_size, shuffle=False, one_shot=True
-        )
-        if tf_version == 2:
-            vectors = model_head.predict(gen.create())
-        else:
-            vectors = predict_in_batches(model_head, gen.create())
-        print(
-            "! {}s elapsed, ({}/{} vectors)".format(
-                time.time() - t, len(vectors), len(ds.images.data)
-            )
-        )
-
-        # Clear session
-        # K.clear_session()
-
-        # Generate tail model and compile
-        model_tail = generate_tl_tail(
-            tp.dataset.num_classes,
-            [
-                vectors.shape[-1],
-            ],
-        )
-        model_tail.compile(
-            optimizer="adam", loss="categorical_crossentropy", metrics=["accuracy"]
-        )
-
-        # Learning rate scheduler
-        alr_cb = AdaptiveLearningRateScheduler(
-            nb_epochs=tp.training.alr_epochs, nb_drops=tp.training.alr_drops, verbose=1
-        )
-        print("-" * 80)
-        print("Training")
-
-        # Training generator
-        train_gen = TFGenerator(
-            vectors,
-            ds.cls_onehot,
-            ds.train_idx,
-            tp.training.batch_size,
-            shuffle=True,
-            one_shot=False,
-            undersample=tp.training.use_class_undersampling,
-        )
-
-        # Validation generator
-        if tf_version == 2:
-            val_one_shot = True
-        else:
-            # One repeat for validation for TF1 otherwise we get end of dataset errors
-            val_one_shot = False
-        if tp.dataset.val_split > 0:
-            val_gen = TFGenerator(
-                vectors,
-                ds.cls_onehot,
-                ds.test_idx,
-                tp.training.batch_size,
-                shuffle=False,
-                one_shot=val_one_shot,
-            )
-            val_data = val_gen.create()
-            val_steps = len(val_gen)
-        else:
-            val_gen = None
-            val_data = None
-            val_steps = None
-
-        # Class weights (only if over sampling is not used)
-        if (
-            tp.training.use_class_weights is True
-            and tp.training.use_class_undersampling is False
-        ):
-            class_weights = ds.class_weights
-            print("- class weights: {}".format(class_weights))
-            if tf_version == 2:
-                class_weights = dict(enumerate(class_weights))
-        else:
-            class_weights = None
-        if tp.training.use_class_undersampling:
-            print("- class balancing using random under sampling")
-
-        # v = model_tail.predict(vectors[0:1])
-        # print(v[0, :10])
-
-        # model_head.summary()
-
-        # model = Model(inputs=model_head.input, outputs=model_tail(model_head.output))
-        # vector_model = Model(model.inputs, model.get_layer(index=-2).get_output_at(0))
-        # v = vector_model.predict(ds.images.data[0:1] / 255)
-        # print(v[0, :10])
-        # v = vector_model.predict(ds.images.data[0:1])
-        # print(v[0, :10])
-
-        # Train
-        if tf_version == 2:
-            train_fn = model_tail.fit
-        else:
-            train_fn = model_tail.fit_generator
-        history = train_fn(
-            train_gen.create(),
-            steps_per_epoch=len(train_gen),
-            validation_data=val_data,
-            validation_steps=val_steps,
-            epochs=tp.training.max_epochs,
-            verbose=0,
-            shuffle=False,
-            max_queue_size=1,
-            class_weight=class_weights,
-            callbacks=[alr_cb],
-        )
-        # Elapsed time
-        end = time.time()
-        training_time = end - start
-        print("- training time: {}s".format(training_time))
-        time.sleep(3)
-
-        # Now we join the trained dense layers to the resnet model to create a model that accepts images as input
-        # model_head = generate_tl_head(tp.cnn.id, tp.cnn.img_shape)
-        model = combine_tl(model_head, model_tail)
-        # model.summary()
-
-        # print(model.layers[-1])
-        # print(model.layers[-2])
-        #
-        # vector_model = Model(inputs=model.inputs, outputs=model.layers[-2].get_output_at(1))
-        # print(vector_model.layers[-1])
-        # print(vector_model.layers[-2])
-        # v = vector_model.predict(ds.images.data[0:1] / 255)
-        # print(v[0, :10])
-        # v = vector_model.predict(ds.images.data[0:1])
-        # print(v[0, :10])
-
-        # model = Model(inputs=model_head.input, outputs=model_tail(model_head.layers[-1].layers[-1].output))
-        # model.summary()
-
-        # print(model_tail.get_layer(index=-2).get_weights())
-        #
-        # vector_tensor = model_tail.get_layer(index=-2).get_output_at(0)
-        # vector_model = Model(model_tail.inputs, vector_tensor)
-        vector_model = generate_vector(model, tp.cnn.id)
-        # v = vector_model.predict(vectors[0:1])
-        # print(v[0, :10])
-        #
-        # vectors = model_head.predict(next(iter(gen.create())))
-        # v = vector_model.predict(vectors[0:1])
-        # print(v[0, :10])
-
-    # ------------------------------------------------------------------------------
-    # Full network train
-    # ------------------------------------------------------------------------------
-    else:
-        print("-" * 80)
-        print("Full network training")
-        start = time.time()
-
-        # Generate model
-        model = generate(tp)
-        # model.summary()
-
-        # Augmentation
-        if tp.augmentation.rotation is True:
-            tp.augmentation.rotation = [0, 360]
-        elif tp.augmentation.rotation is False:
-            tp.augmentation.rotation = None
-        if tp.training.use_augmentation is True:
-            print("- using augmentation")
-            augment_fn = aug_all_fn(
-                rotation=tp.augmentation.rotation,
-                gain=tp.augmentation.gain,
-                gamma=tp.augmentation.gamma,
-                zoom=tp.augmentation.zoom,
-                gaussian_noise=tp.augmentation.gaussian_noise,
-                bias=tp.augmentation.bias,
-                random_crop=tp.augmentation.random_crop,
-                divide=255,
-            )
-        else:
-            print("- NOT using augmentation")
-            augment_fn = TFGenerator.map_fn_divide_255
-
-        # Learning rate scheduler
-        alr_cb = AdaptiveLearningRateScheduler(
-            nb_epochs=tp.training.alr_epochs, nb_drops=tp.training.alr_drops, verbose=1
-        )
-
-        # Training generator
-        train_gen = ds.train_generator(
-            batch_size=tp.training.batch_size,
-            map_fn=augment_fn,
-            undersample=tp.training.use_class_undersampling,
-        )
-
-        # Save example of training data
-        print("- saving example training batch")
-        training_examples_dir = os.path.join(save_dir, "examples", "training")
-        os.makedirs(training_examples_dir)
-        images, labels = next(iter(train_gen.create()))
-        for t_idx, im in enumerate(images):
-            im = im.numpy() * 255
-            im[im > 255] = 255
-            if np.ndim(im) == 2:
-                im = np.repeat(im[:, :, np.newaxis], 3, axis=-1)
-            elif im.shape[-1] == 1:
-                im = np.repeat(im, 3, axis=-1)
-            skimage.io.imsave(
-                os.path.join(training_examples_dir, "{:03d}.jpg".format(t_idx)),
-                im.astype(np.uint8),
-            )
-
-        # Validation generator
-        if tf_version == 2:
-            val_one_shot = True
-        else:
-            # One repeat for validation for TF1 otherwise we get end of dataset errors
-            val_one_shot = False
-        if tp.dataset.val_split > 0:
-            # Maximum 8 in batch otherwise validation results jump around a bit because
-            val_gen = ds.test_generator(
-                min(tp.training.batch_size, 16), shuffle=False, one_shot=val_one_shot
-            )
-            # val_gen = ds.test_generator(tp.training.batch_size, shuffle=False, one_shot=val_one_shot)
-            val_data = val_gen.create()
-            val_steps = len(val_gen)
-        else:
-            val_gen = None
-            val_data = None
-            val_steps = None
-
-        # Class weights
-        if (
-            tp.training.use_class_weights is True
-            and tp.training.use_class_undersampling is False
-        ):
-            class_weights = ds.class_weights
-            print("- class weights: {}".format(class_weights))
-            if tf_version == 2:
-                class_weights = dict(enumerate(class_weights))
-        else:
-            class_weights = None
-        if tp.training.use_class_undersampling:
-            print("- class balancing using random under sampling")
-
-        # Train the model
-        if tf_version == 2:
-            train_fn = model.fit
-        else:
-            train_fn = model.fit_generator
-        history = train_fn(
-            train_gen.create(),
-            steps_per_epoch=len(train_gen),
-            validation_data=val_data,
-            validation_steps=val_steps,
-            epochs=tp.training.max_epochs,
-            verbose=0,
-            shuffle=False,
-            max_queue_size=1,
-            class_weight=class_weights,
-            callbacks=[alr_cb],
-        )
-
-        # Elapsed time
-        end = time.time()
-        training_time = end - start
-        print()
-        print("Total training time: {}s".format(training_time))
-        time.sleep(3)
-
-        # Vector model
-        vector_model = generate_vector(model, tp.cnn.id)
-
-    # ------------------------------------------------------------------------------
-    # Results
-    # ------------------------------------------------------------------------------
-    print("-" * 80)
-    print("Evaluating model")
-    # Accuracy
-    if tp.dataset.val_split > 0:
-        y_true = ds.cls[ds.test_idx]
-        gen = ds.test_generator(tp.training.batch_size, shuffle=False, one_shot=True)
-        if tf_version == 2:
-            y_prob = model.predict(gen.create())
-        else:
-            y_prob = predict_in_batches(model, gen.create())
-        y_pred = y_prob.argmax(axis=1)
-    else:
-        y_true = np.asarray([])
-        y_prob = np.asarray([])
-        y_pred = np.asarray([])
-    # Inference time
-    print("- calculating inference time:", end="")
-    max_count = np.min([128, len(ds.images.data)])
-    inf_times = []
-    for i in range(3):
-        gen = ds.images.create_generator(
-            tp.training.batch_size,
-            idxs=np.arange(max_count),
-            shuffle=False,
-            one_shot=True,
-        )
-        start = time.time()
-        if tf_version == 2:
-            model.predict(gen.create())
-        else:
-            predict_in_batches(model, gen.create())
-        end = time.time()
-        diff = (end - start) / max_count * 1000
-        inf_times.append(diff)
-        print(" {:.3f}ms".format(diff), end="")
-    inference_time = np.median(inf_times)
-    print(", median: {}".format(inference_time))
-    # Store results
-    # - fix to make key same for tensorflow 1 and 2
-    if "accuracy" in history.history:
-        history.history["acc"] = history.history.pop("accuracy")
-        history.history["val_acc"] = history.history.pop("val_accuracy")
-    result = TrainingResult(
-        tp,
-        history,
-        y_true,
-        y_pred,
-        y_prob,
-        ds.cls_labels,
-        training_time,
-        inference_time,
-    )
-    print("- accuracy {:.2f}".format(result.accuracy * 100))
-    print("- mean precision {:.2f}".format(result.mean_precision * 100))
-    print("- mean recall {:.2f}".format(result.mean_recall * 100))
-    # ------------------------------------------------------------------------------
-    # Save results
-    # ------------------------------------------------------------------------------
-    if tp.description is None:
-        tp.description = (
-            "{}: {} model trained on data from {} ({} images in {} classes).\n"
-            "Accuracy: {:.1f} (P: {:.1f}, R: {:.1f}, F1 {:.1f})".format(
-                tp.name,
-                tp.cnn.id,
-                tp.dataset.source,
-                len(ds.filenames.filenames),
-                len(ds.cls_labels),
-                result.accuracy * 100,
-                result.mean_precision * 100,
-                result.mean_recall * 100,
-                result.mean_f1_score * 100,
-            )
-        )
-
-    # Create model info with all the parameters
-    inputs = OrderedDict()
-    inputs["image"] = model.inputs[0]
-    outputs = OrderedDict()
-    outputs["pred"] = model.outputs[0]
-    outputs["vector"] = vector_model.outputs[0]
-    info = ModelInfo(
-        tp.name,
-        tp.description,
-        tp.cnn.id,
-        now,
-        "frozen_model.pb",
-        tp,
-        inputs,
-        outputs,
-        tp.dataset.source,
-        ds.cls_labels,
-        ds.filenames.cls_counts,
-        "rescale",
-        [255, 0, 1],
-        result.accuracy,
-        result.precision,
-        result.recall,
-        result.f1_score,
-        result.support,
-        result.epochs[-1],
-        training_time,
-        tp.dataset.val_split,
-        inference_time,
-    )
-    # ------------------------------------------------------------------------------
-    # Cleanlab health report
-    # ------------------------------------------------------------------------------
-    print("-" * 80)
-    print("Health report")
-    import cleanlab
-
-    report = cleanlab.dataset.health_summary(y_true, y_prob, class_names=ds.cls_labels)
-    with open(os.path.join(save_dir, "health_summary.txt"), "w") as fp:
-        fp.write("Dataset health report\n")
-        fp.write("\n")
-        fp.write("This is calculated using the test data\n")
-        fp.write("\n" + "-" * 80 + "\n")
-        fp.write(f"Overall label heath: {report['overall_label_health_score']}")
-        # fp.write("-" * 80 + "\n")
-        # fp.write("Joint probabilities\n")
-        # fp.write(report["joint"])
-        fp.write("\n" + "-" * 80 + "\n")
-        fp.write("Classes by label quality\n")
-        fp.write(report["classes_by_label_quality"].to_string())
-        fp.write("\n" + "-" * 80 + "\n")
-        fp.write("Overlapping classes\n")
-        fp.write(report["overlapping_classes"].to_string())
-
-    # ------------------------------------------------------------------------------
-    # Plots
-    # ------------------------------------------------------------------------------
-    # Plot the graphs
-    # plot_model(model, to_file=os.path.join(save_dir, "model_plot.pdf"), show_shapes=True)
-    print("-" * 80)
-    print("Plotting")
-    if tp.dataset.val_split > 0:
-        print("- loss")
-        plot_loss_vs_epochs(history)
-        plt.savefig(os.path.join(save_dir, "loss_vs_epoch.pdf"))
-        print("- accuracy")
-        plot_accuracy_vs_epochs(history)
-        plt.savefig(os.path.join(save_dir, "accuracy_vs_epoch.pdf"))
-        print("- confusion matrix")
-        plot_confusion_accuracy_matrix(y_true, y_pred, ds.cls_labels)
-        plt.savefig(os.path.join(save_dir, "confusion_matrix.pdf"))
-        plt.close("all")
-
-    if tp.output.save_mislabeled is True:
-        print("- mislabeled")
-        print("- calculating vectors... ", end="")
-        gen = ds.images.create_generator(
-            tp.training.batch_size, shuffle=False, one_shot=True
-        )
-        if tf_version == 2:
-            vectors = vector_model.predict(gen.create())
-        else:
-            vectors = predict_in_batches(vector_model, gen.create())
-        print("{} total".format(len(vectors)))
-        find_and_save_mislabelled(
-            ds.images.data,
-            vectors,
-            ds.cls,
-            ds.cls_labels,
-            [os.path.basename(f) for f in ds.filenames.filenames],
-            save_dir,
-            11,
-        )
-
-    # t-SNE
-    print("- t-SNE (1024 vectors max)")
-    print("- calculating vectors... ", end="")
-    idxs = np.random.choice(
-        np.arange(len(ds.images.data)),
-        np.min((1024, len(ds.images.data))),
-        replace=False,
-    )
-    gen = ds.images.create_generator(
-        tp.training.batch_size, idxs=idxs, shuffle=False, one_shot=True
-    )
-    if tf_version == 2:
-        vec_subset = vector_model.predict(gen.create())
-    else:
-        vec_subset = predict_in_batches(vector_model, gen.create())
-    X = TSNE(n_components=2).fit_transform(vec_subset)
-    plot_embedding(X, ds.cls[idxs], ds.num_classes)
-    plt.savefig(os.path.join(save_dir, "tsne.pdf"))
-    cls_info = pd.DataFrame({"index": range(ds.num_classes), "label": ds.cls_labels})
-    cls_info.to_csv(os.path.join(save_dir, "legend.csv"), sep=";")
-
-    # ------------------------------------------------------------------------------
-    # Save model (has to be last thing it seems)
-    # ------------------------------------------------------------------------------
-    print("-" * 80)
-    print("Saving model")
-    # Convert if necessary to fix TF batch normalisation issues
-
-    # Freeze and save graph
-    if tp.output.save_model is not None:
-        if tf_version == 2:
-            inference_model = convert_to_inference_mode_tf2(model, lambda: generate(tp))
-            # tf.saved_model.save(inference_model, os.path.join(os.path.join(save_dir, "model_keras")))
-            frozen_func = save_frozen_model_tf2(
-                inference_model, os.path.join(save_dir, "model"), "frozen_model.pb"
-            )
-            save_model_as_onnx(
-                inference_model,
-                inference_model.inputs[0].name,
-                [
-                    None,
-                ]
-                + tp.cnn.img_shape,
-                os.path.join(os.path.join(save_dir, "model_onnx")),
-            )
-            info.protobuf = "model.onnx"
-            info.inputs["image"] = inference_model.inputs[0]
-            info.outputs["pred"] = inference_model.outputs[0]
-            info.save(os.path.join(save_dir, "model_onnx", "network_info.xml"))
-            info.protobuf = "frozen_model.pb"
-            info.inputs["image"] = frozen_func.inputs[0]
-            info.outputs["pred"] = frozen_func.outputs[0]
-            info.save(os.path.join(save_dir, "model", "network_info.xml"))
-        else:
-            inference_model = convert_to_inference_mode(model, lambda: generate(tp))
-            tf.saved_model.save(
-                inference_model, os.path.join(os.path.join(save_dir, "model_keras"))
-            )
-            freeze(inference_model, os.path.join(save_dir, "model"))
-            info.save(os.path.join(save_dir, "model", "network_info.xml"))
-    
-
-    # ------------------------------------------------------------------------------
-    # Confirm model save
-    # ------------------------------------------------------------------------------
-    if tp.output.save_model is not None and tp.dataset.val_split > 0:
-        print("-" * 80)
-        print("Validate saved model")
-        y_pred_old = y_pred
-        y_true = ds.cls[ds.test_idx]
-        gen = ds.test_generator(32, shuffle=False, one_shot=True)
-        y_prob = []
-        if tf_version == 2:
-            model, img_size, cls_labels = load_from_xml(
-                os.path.join(save_dir, "model", "network_info.xml")
-            )
-            for b in iter(gen.to_tfdataset()):
-                y_prob.append(model(b[0]).numpy())
-        else:
-            session, input, output, img_size, cls_labels = load_from_xml(
-                os.path.join(save_dir, "model", "network_info.xml")
-            )
-            iterator = iter(gen.tf1_compat_generator())
-            for bi in range(len(gen)):
-                b = next(iterator)
-                y_p = session.run(output, feed_dict={input: b[0]})
-                y_prob.append(y_p)
-        y_prob = np.concatenate(y_prob, axis=0)
-        y_pred = y_prob.argmax(axis=1)
-        acc = accuracy_score(y_true, y_pred)
-        p, r, f1, _ = precision_recall_fscore_support(y_true, y_pred)
-        print(
-            "Saved model on test set: acc {:.2f}, prec {:.2f}, rec {:.2f}, f1 {:.2f}".format(
-                acc, np.mean(p), np.mean(r), np.mean(f1)
-            )
-        )
-        acc = accuracy_score(y_pred_old, y_pred)
-        if acc == 1.0:
-            print("Overlap: {:.2f}% - PASSED".format(acc * 100))
-        else:
-            print("Overlap: {:.2f}% - FAILED".format(acc * 100))
-
-    # ------------------------------------------------------------------------------
-    # Clean up
-    # ------------------------------------------------------------------------------
-    print("- cleaning up")
-    ds.release()
-    print("- complete")
-    print("-" * 80)
-    print()
-    return model, vector_model, ds, result
+"""
+Creates and trains a generic network
+"""
+import os
+import skimage.io
+import warnings
+
+warnings.simplefilter(action="ignore", category=FutureWarning)
+
+# from clearml import Task
+
+import time
+import datetime
+from collections import OrderedDict
+import tensorflow.keras.backend as K
+from sklearn.manifold import TSNE
+
+from miso.data.tf_generator import TFGenerator
+from miso.data.training_dataset import TrainingDataset
+from miso.stats.embedding import plot_embedding
+from miso.stats.mislabelling import find_and_save_mislabelled
+from miso.training.adaptive_learning_rate import AdaptiveLearningRateScheduler
+from miso.training.training_result import TrainingResult
+from miso.stats.confusion_matrix import *
+from miso.stats.training import *
+from miso.training.tf_augmentation import aug_all_fn
+from miso.deploy.saving import (
+    freeze,
+    convert_to_inference_mode,
+    save_frozen_model_tf2,
+    convert_to_inference_mode_tf2,
+    load_from_xml,
+    save_model_as_onnx,
+)
+from miso.deploy.model_info import ModelInfo
+from miso.models.factory import *
+
+import matplotlib.pyplot as plt
+import pandas as pd
+
+
+def predict_in_batches(model, generator):
+    results = []
+    try:
+        for x, y in iter(generator):
+            results.append(model.predict(x))
+    except tf.errors.OutOfRangeError:
+        pass
+    results = np.concatenate(results, axis=0)
+    return results
+
+
+def train_image_classification_model(tp: MisoParameters):
+    tf_version = int(tf.__version__[0])
+    now = datetime.datetime.now()
+
+    # ClearML task
+    # print(f"ClearML initialising")
+    # task = Task.init(project_name='MISO',
+    #                  task_name=f"{tp.name}_{now:%Y%m%d-%H%M%S}")
+    # task.connect(tp)
+
+    # Hack to make RTX cards work
+    if tf_version == 2:
+        physical_devices = tf.config.list_physical_devices("GPU")
+        print(physical_devices)
+        for device in physical_devices:
+            tf.config.experimental.set_memory_growth(device, True)
+    else:
+        config = tf.ConfigProto()
+        config.gpu_options.allow_growth = True
+        session = tf.Session(config=config)
+
+    K.clear_session()
+
+    # Clean the training parameters
+    tp.sanitise()
+
+    print("+---------------------------------------------------------------------------+")
+    print("| MISO Particle Classification Library                                      |")
+    print("+---------------------------------------------------------------------------+")
+    print("| Stable version:                                                           |")
+    print("| pip install miso2                                                         |")
+    print("| Development version:                                                      |")
+    print("| pip install git+http://www.github.com/microfossil/particle-classification |")
+    print("+---------------------------------------------------------------------------+")
+    print("Tensorflow version: {}".format(tf.__version__))
+    print("-" * 80)
+    print("Train information:")
+    print("- name: {}".format(tp.name))
+    print("- description: {}".format(tp.description))
+    print("- CNN type: {}".format(tp.cnn.id))
+    print("- image type: {}".format(tp.cnn.img_type))
+    print("- image shape: {}".format(tp.cnn.img_shape))
+    print()
+
+    # Load data
+    ds = TrainingDataset(
+        tp.dataset.source,
+        tp.cnn.img_shape,
+        tp.cnn.img_type,
+        tp.dataset.min_count,
+        tp.dataset.map_others,
+        tp.dataset.val_split,
+        tp.dataset.random_seed,
+        tp.dataset.memmap_directory,
+    )
+    ds.load()
+    tp.dataset.num_classes = ds.num_classes
+
+    # Create save lodations
+    save_dir = os.path.join(
+        tp.output.save_dir, "{0}_{1:%Y%m%d-%H%M%S}".format(tp.name, now)
+    )
+    os.makedirs(save_dir, exist_ok=True)
+
+    # ------------------------------------------------------------------------------
+    # Transfer learning
+    # ------------------------------------------------------------------------------
+    if tp.cnn.id.endswith("tl"):
+        print("-" * 80)
+        print("Transfer learning network training")
+        start = time.time()
+
+        # Generate head model and predict vectors
+        model_head = generate_tl_head(tp.cnn.id, tp.cnn.img_shape)
+
+        # Calculate vectors
+        print("- calculating vectors")
+        t = time.time()
+        gen = ds.images.create_generator(
+            tp.training.batch_size, shuffle=False, one_shot=True
+        )
+        if tf_version == 2:
+            vectors = model_head.predict(gen.create())
+        else:
+            vectors = predict_in_batches(model_head, gen.create())
+        print(f"! {time.time() - t}s elapsed, ({len(vectors)}/{len(ds.images.data)} vectors)")
+
+        # Clear session
+        # K.clear_session()
+
+        # Generate tail model and compile
+        model_tail = generate_tl_tail(tp.dataset.num_classes, [vectors.shape[-1]])
+        model_tail.compile(optimizer="adam",
+                           loss="categorical_crossentropy",
+                           metrics=["accuracy"])
+
+        # Learning rate scheduler
+        alr_cb = AdaptiveLearningRateScheduler(nb_epochs=tp.training.alr_epochs,
+                                               nb_drops=tp.training.alr_drops,
+                                               verbose=1)
+        print("-" * 80)
+        print("Training")
+
+        # Training generator
+        train_gen = TFGenerator(vectors,
+                                ds.cls_onehot,
+                                ds.train_idx,
+                                tp.training.batch_size,
+                                shuffle=True,
+                                one_shot=False,
+                                undersample=tp.training.use_class_undersampling)
+
+        # Validation generator
+        if tf_version == 2:
+            val_one_shot = True
+        else:
+            # One repeat for validation for TF1 otherwise we get end of dataset errors
+            val_one_shot = False
+        if tp.dataset.val_split > 0:
+            val_gen = TFGenerator(
+                vectors,
+                ds.cls_onehot,
+                ds.test_idx,
+                tp.training.batch_size,
+                shuffle=False,
+                one_shot=val_one_shot,
+            )
+            val_data = val_gen.create()
+            val_steps = len(val_gen)
+        else:
+            val_gen = None
+            val_data = None
+            val_steps = None
+
+        # Class weights (only if over sampling is not used)
+        if tp.training.use_class_weights is True and tp.training.use_class_undersampling is False:
+            class_weights = ds.class_weights
+            print("- class weights: {}".format(class_weights))
+            if tf_version == 2:
+                class_weights = dict(enumerate(class_weights))
+        else:
+            class_weights = None
+        if tp.training.use_class_undersampling:
+            print("- class balancing using random under sampling")
+
+        # v = model_tail.predict(vectors[0:1])
+        # print(v[0, :10])
+
+        # model_head.summary()
+
+        # model = Model(inputs=model_head.input, outputs=model_tail(model_head.output))
+        # vector_model = Model(model.inputs, model.get_layer(index=-2).get_output_at(0))
+        # v = vector_model.predict(ds.images.data[0:1] / 255)
+        # print(v[0, :10])
+        # v = vector_model.predict(ds.images.data[0:1])
+        # print(v[0, :10])
+
+        # Train
+        if tf_version == 2:
+            train_fn = model_tail.fit
+        else:
+            train_fn = model_tail.fit_generator
+        history = train_fn(train_gen.create(),
+                           steps_per_epoch=len(train_gen),
+                           validation_data=val_data,
+                           validation_steps=val_steps,
+                           epochs=tp.training.max_epochs,
+                           verbose=0,
+                           shuffle=False,
+                           max_queue_size=1,
+                           class_weight=class_weights,
+                           callbacks=[alr_cb])
+        # Elapsed time
+        end = time.time()
+        training_time = end - start
+        print("- training time: {}s".format(training_time))
+        time.sleep(3)
+
+        # Now we join the trained dense layers to the resnet model to create a model that accepts images as input
+        # model_head = generate_tl_head(tp.cnn.id, tp.cnn.img_shape)
+        model = combine_tl(model_head, model_tail)
+        # model.summary()
+
+        # print(model.layers[-1])
+        # print(model.layers[-2])
+        #
+        # vector_model = Model(inputs=model.inputs, outputs=model.layers[-2].get_output_at(1))
+        # print(vector_model.layers[-1])
+        # print(vector_model.layers[-2])
+        # v = vector_model.predict(ds.images.data[0:1] / 255)
+        # print(v[0, :10])
+        # v = vector_model.predict(ds.images.data[0:1])
+        # print(v[0, :10])
+
+        # model = Model(inputs=model_head.input, outputs=model_tail(model_head.layers[-1].layers[-1].output))
+        # model.summary()
+
+        # print(model_tail.get_layer(index=-2).get_weights())
+        #
+        # vector_tensor = model_tail.get_layer(index=-2).get_output_at(0)
+        # vector_model = Model(model_tail.inputs, vector_tensor)
+        vector_model = generate_vector(model, tp.cnn.id)
+        # v = vector_model.predict(vectors[0:1])
+        # print(v[0, :10])
+        #
+        # vectors = model_head.predict(next(iter(gen.create())))
+        # v = vector_model.predict(vectors[0:1])
+        # print(v[0, :10])
+
+    # ------------------------------------------------------------------------------
+    # Full network train
+    # ------------------------------------------------------------------------------
+    else:
+        print("-" * 80)
+        print("Full network training")
+        start = time.time()
+
+        # Generate model
+        model = generate(tp)
+        # model.summary()
+
+        # Augmentation
+        if tp.augmentation.rotation is True:
+            tp.augmentation.rotation = [0, 360]
+        elif tp.augmentation.rotation is False:
+            tp.augmentation.rotation = None
+        if tp.training.use_augmentation is True:
+            print("- using augmentation")
+            augment_fn = aug_all_fn(
+                rotation=tp.augmentation.rotation,
+                gain=tp.augmentation.gain,
+                gamma=tp.augmentation.gamma,
+                zoom=tp.augmentation.zoom,
+                gaussian_noise=tp.augmentation.gaussian_noise,
+                bias=tp.augmentation.bias,
+                random_crop=tp.augmentation.random_crop,
+                divide=255,
+            )
+        else:
+            print("- NOT using augmentation")
+            augment_fn = TFGenerator.map_fn_divide_255
+
+        # Learning rate scheduler
+        alr_cb = AdaptiveLearningRateScheduler(
+            nb_epochs=tp.training.alr_epochs, nb_drops=tp.training.alr_drops, verbose=1
+        )
+
+        # Training generator
+        train_gen = ds.train_generator(
+            batch_size=tp.training.batch_size,
+            map_fn=augment_fn,
+            undersample=tp.training.use_class_undersampling,
+        )
+
+        # Save example of training data
+        print("- saving example training batch")
+        training_examples_dir = os.path.join(save_dir, "examples", "training")
+        os.makedirs(training_examples_dir)
+        images, labels = next(iter(train_gen.create()))
+        for t_idx, im in enumerate(images):
+            im = im.numpy() * 255
+            im[im > 255] = 255
+            if np.ndim(im) == 2:
+                im = np.repeat(im[:, :, np.newaxis], 3, axis=-1)
+            elif im.shape[-1] == 1:
+                im = np.repeat(im, 3, axis=-1)
+            skimage.io.imsave(
+                os.path.join(training_examples_dir, "{:03d}.jpg".format(t_idx)),
+                im.astype(np.uint8),
+            )
+
+        # Validation generator
+        if tf_version == 2:
+            val_one_shot = True
+        else:
+            # One repeat for validation for TF1 otherwise we get end of dataset errors
+            val_one_shot = False
+        if tp.dataset.val_split > 0:
+            # Maximum 8 in batch otherwise validation results jump around a bit because
+            val_gen = ds.test_generator(
+                min(tp.training.batch_size, 16), shuffle=False, one_shot=val_one_shot
+            )
+            # val_gen = ds.test_generator(tp.training.batch_size, shuffle=False, one_shot=val_one_shot)
+            val_data = val_gen.create()
+            val_steps = len(val_gen)
+        else:
+            val_gen = None
+            val_data = None
+            val_steps = None
+
+        # Class weights
+        if (
+                tp.training.use_class_weights is True
+                and tp.training.use_class_undersampling is False
+        ):
+            class_weights = ds.class_weights
+            print("- class weights: {}".format(class_weights))
+            if tf_version == 2:
+                class_weights = dict(enumerate(class_weights))
+        else:
+            class_weights = None
+        if tp.training.use_class_undersampling:
+            print("- class balancing using random under sampling")
+
+        # Train the model
+        if tf_version == 2:
+            train_fn = model.fit
+        else:
+            train_fn = model.fit_generator
+        history = train_fn(
+            train_gen.create(),
+            steps_per_epoch=len(train_gen),
+            validation_data=val_data,
+            validation_steps=val_steps,
+            epochs=tp.training.max_epochs,
+            verbose=0,
+            shuffle=False,
+            max_queue_size=1,
+            class_weight=class_weights,
+            callbacks=[alr_cb],
+        )
+
+        # Elapsed time
+        end = time.time()
+        training_time = end - start
+        print()
+        print("Total training time: {}s".format(training_time))
+        time.sleep(3)
+
+        # Vector model
+        vector_model = generate_vector(model, tp.cnn.id)
+
+    # ------------------------------------------------------------------------------
+    # Results
+    # ------------------------------------------------------------------------------
+    print("-" * 80)
+    print("Evaluating model")
+    # Accuracy
+    if tp.dataset.val_split > 0:
+        y_true = ds.cls[ds.test_idx]
+        gen = ds.test_generator(tp.training.batch_size, shuffle=False, one_shot=True)
+        if tf_version == 2:
+            y_prob = model.predict(gen.create())
+        else:
+            y_prob = predict_in_batches(model, gen.create())
+        y_pred = y_prob.argmax(axis=1)
+    else:
+        y_true = np.asarray([])
+        y_prob = np.asarray([])
+        y_pred = np.asarray([])
+    # Inference time
+    print("- calculating inference time:", end="")
+    max_count = np.min([128, len(ds.images.data)])
+    inf_times = []
+    for i in range(3):
+        gen = ds.images.create_generator(
+            tp.training.batch_size,
+            idxs=np.arange(max_count),
+            shuffle=False,
+            one_shot=True,
+        )
+        start = time.time()
+        if tf_version == 2:
+            model.predict(gen.create())
+        else:
+            predict_in_batches(model, gen.create())
+        end = time.time()
+        diff = (end - start) / max_count * 1000
+        inf_times.append(diff)
+        print(" {:.3f}ms".format(diff), end="")
+    inference_time = np.median(inf_times)
+    print(", median: {}".format(inference_time))
+    # Store results
+    # - fix to make key same for tensorflow 1 and 2
+    if "accuracy" in history.history:
+        history.history["acc"] = history.history.pop("accuracy")
+    if "val_accuracy" in history.history:
+        history.history["val_acc"] = history.history.pop("val_accuracy")
+    result = TrainingResult(
+        tp,
+        history,
+        y_true,
+        y_pred,
+        y_prob,
+        ds.cls_labels,
+        training_time,
+        inference_time,
+    )
+    print("- accuracy {:.2f}".format(result.accuracy * 100))
+    print("- mean precision {:.2f}".format(result.mean_precision * 100))
+    print("- mean recall {:.2f}".format(result.mean_recall * 100))
+    # ------------------------------------------------------------------------------
+    # Save results
+    # ------------------------------------------------------------------------------
+    if tp.description is None:
+        tp.description = (
+            "{}: {} model trained on data from {} ({} images in {} classes).\n"
+            "Accuracy: {:.1f} (P: {:.1f}, R: {:.1f}, F1 {:.1f})".format(
+                tp.name,
+                tp.cnn.id,
+                tp.dataset.source,
+                len(ds.filenames.filenames),
+                len(ds.cls_labels),
+                result.accuracy * 100,
+                result.mean_precision * 100,
+                result.mean_recall * 100,
+                result.mean_f1_score * 100,
+            )
+        )
+
+    # Create model info with all the parameters
+    inputs = OrderedDict()
+    inputs["image"] = model.inputs[0]
+    outputs = OrderedDict()
+    outputs["pred"] = model.outputs[0]
+    outputs["vector"] = vector_model.outputs[0]
+    info = ModelInfo(
+        tp.name,
+        tp.description,
+        tp.cnn.id,
+        now,
+        "frozen_model.pb",
+        tp,
+        inputs,
+        outputs,
+        tp.dataset.source,
+        ds.cls_labels,
+        ds.filenames.cls_counts,
+        "rescale",
+        [255, 0, 1],
+        result.accuracy,
+        result.precision,
+        result.recall,
+        result.f1_score,
+        result.support,
+        result.epochs[-1],
+        training_time,
+        tp.dataset.val_split,
+        inference_time,
+    )
+    # ------------------------------------------------------------------------------
+    # Cleanlab health report
+    # ------------------------------------------------------------------------------
+    print("-" * 80)
+    print("Health report")
+    import cleanlab
+
+    report = cleanlab.dataset.health_summary(y_true, y_prob, class_names=ds.cls_labels)
+    with open(os.path.join(save_dir, "health_summary.txt"), "w") as fp:
+        fp.write("Dataset health report\n")
+        fp.write("\n")
+        fp.write("This is calculated using the test data\n")
+        fp.write("\n" + "-" * 80 + "\n")
+        fp.write(f"Overall label heath: {report['overall_label_health_score']}")
+        # fp.write("-" * 80 + "\n")
+        # fp.write("Joint probabilities\n")
+        # fp.write(report["joint"])
+        fp.write("\n" + "-" * 80 + "\n")
+        fp.write("Classes by label quality\n")
+        fp.write(report["classes_by_label_quality"].to_string())
+        fp.write("\n" + "-" * 80 + "\n")
+        fp.write("Overlapping classes\n")
+        fp.write(report["overlapping_classes"].to_string())
+
+    # ------------------------------------------------------------------------------
+    # Plots
+    # ------------------------------------------------------------------------------
+    # Plot the graphs
+    # plot_model(model, to_file=os.path.join(save_dir, "model_plot.pdf"), show_shapes=True)
+    print("-" * 80)
+    print("Plotting")
+    if tp.dataset.val_split > 0:
+        print("- loss")
+        plot_loss_vs_epochs(history)
+        plt.savefig(os.path.join(save_dir, "loss_vs_epoch.pdf"))
+        print("- accuracy")
+        plot_accuracy_vs_epochs(history)
+        plt.savefig(os.path.join(save_dir, "accuracy_vs_epoch.pdf"))
+        print("- confusion matrix")
+        plot_confusion_accuracy_matrix(y_true, y_pred, ds.cls_labels)
+        plt.savefig(os.path.join(save_dir, "confusion_matrix.pdf"))
+        plt.close("all")
+
+    if tp.output.save_mislabeled is True:
+        print("- mislabeled")
+        print("- calculating vectors... ", end="")
+        gen = ds.images.create_generator(
+            tp.training.batch_size, shuffle=False, one_shot=True
+        )
+        if tf_version == 2:
+            vectors = vector_model.predict(gen.create())
+        else:
+            vectors = predict_in_batches(vector_model, gen.create())
+        print("{} total".format(len(vectors)))
+        find_and_save_mislabelled(
+            ds.images.data,
+            vectors,
+            ds.cls,
+            ds.cls_labels,
+            [os.path.basename(f) for f in ds.filenames.filenames],
+            save_dir,
+            11,
+        )
+
+    # t-SNE
+    print("- t-SNE (1024 vectors max)")
+    print("- calculating vectors... ", end="")
+    idxs = np.random.choice(
+        np.arange(len(ds.images.data)),
+        np.min((1024, len(ds.images.data))),
+        replace=False,
+    )
+    gen = ds.images.create_generator(
+        tp.training.batch_size, idxs=idxs, shuffle=False, one_shot=True
+    )
+    if tf_version == 2:
+        vec_subset = vector_model.predict(gen.create())
+    else:
+        vec_subset = predict_in_batches(vector_model, gen.create())
+    X = TSNE(n_components=2).fit_transform(vec_subset)
+    plot_embedding(X, ds.cls[idxs], ds.num_classes)
+    plt.savefig(os.path.join(save_dir, "tsne.pdf"))
+    cls_info = pd.DataFrame({"index": range(ds.num_classes), "label": ds.cls_labels})
+    cls_info.to_csv(os.path.join(save_dir, "legend.csv"), sep=";")
+
+    # ------------------------------------------------------------------------------
+    # Save model (has to be last thing it seems)
+    # ------------------------------------------------------------------------------
+    print("-" * 80)
+    print("Saving model")
+    # Convert if necessary to fix TF batch normalisation issues
+
+    # Freeze and save graph
+    if tp.output.save_model is not None:
+        if tf_version == 2:
+            inference_model = convert_to_inference_mode_tf2(model, lambda: generate(tp))
+            # tf.saved_model.save(inference_model, os.path.join(os.path.join(save_dir, "model_keras")))
+            frozen_func = save_frozen_model_tf2(
+                inference_model, os.path.join(save_dir, "model"), "frozen_model.pb"
+            )
+            save_model_as_onnx(
+                inference_model,
+                inference_model.inputs[0].name,
+                [
+                    None,
+                ]
+                + tp.cnn.img_shape,
+                os.path.join(os.path.join(save_dir, "model_onnx")),
+            )
+            info.protobuf = "model.onnx"
+            info.inputs["image"] = inference_model.inputs[0]
+            info.outputs["pred"] = inference_model.outputs[0]
+            info.save(os.path.join(save_dir, "model_onnx", "network_info.xml"))
+            info.protobuf = "frozen_model.pb"
+            info.inputs["image"] = frozen_func.inputs[0]
+            info.outputs["pred"] = frozen_func.outputs[0]
+            info.save(os.path.join(save_dir, "model", "network_info.xml"))
+        else:
+            inference_model = convert_to_inference_mode(model, lambda: generate(tp))
+            tf.saved_model.save(
+                inference_model, os.path.join(os.path.join(save_dir, "model_keras"))
+            )
+            freeze(inference_model, os.path.join(save_dir, "model"))
+            info.save(os.path.join(save_dir, "model", "network_info.xml"))
+
+    # ------------------------------------------------------------------------------
+    # Confirm model save
+    # ------------------------------------------------------------------------------
+    if tp.output.save_model is not None and tp.dataset.val_split > 0:
+        print("-" * 80)
+        print("Validate saved model")
+        y_pred_old = y_pred
+        y_true = ds.cls[ds.test_idx]
+        gen = ds.test_generator(32, shuffle=False, one_shot=True)
+        y_prob = []
+        if tf_version == 2:
+            model, img_size, cls_labels = load_from_xml(
+                os.path.join(save_dir, "model", "network_info.xml")
+            )
+            for b in iter(gen.to_tfdataset()):
+                y_prob.append(model(b[0]).numpy())
+        else:
+            session, input, output, img_size, cls_labels = load_from_xml(
+                os.path.join(save_dir, "model", "network_info.xml")
+            )
+            iterator = iter(gen.tf1_compat_generator())
+            for bi in range(len(gen)):
+                b = next(iterator)
+                y_p = session.run(output, feed_dict={input: b[0]})
+                y_prob.append(y_p)
+        y_prob = np.concatenate(y_prob, axis=0)
+        y_pred = y_prob.argmax(axis=1)
+        acc = accuracy_score(y_true, y_pred)
+        p, r, f1, _ = precision_recall_fscore_support(y_true, y_pred)
+        print(
+            "Saved model on test set: acc {:.2f}, prec {:.2f}, rec {:.2f}, f1 {:.2f}".format(
+                acc, np.mean(p), np.mean(r), np.mean(f1)
+            )
+        )
+        acc = accuracy_score(y_pred_old, y_pred)
+        if acc == 1.0:
+            print("Overlap: {:.2f}% - PASSED".format(acc * 100))
+        else:
+            print("Overlap: {:.2f}% - FAILED".format(acc * 100))
+
+    # ------------------------------------------------------------------------------
+    # Clean up
+    # ------------------------------------------------------------------------------
+    print("- cleaning up")
+    ds.release()
+    print("- complete")
+    print("-" * 80)
+    print()
+    return model, vector_model, ds, result
```

### Comparing `miso2-3.0.3/miso/training/training_result.py` & `miso2-3.0.4/miso/training/training_result.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-"""
-Results of training
-"""
-import numpy as np
-from sklearn.metrics import precision_recall_fscore_support, accuracy_score
-
-
-class TrainingResult:
-    def __init__(self,
-                 model_params,
-                 history,
-                 y_true,
-                 y_pred,
-                 y_prob,
-                 cls_labels,
-                 training_time,
-                 inference_time):
-
-        # Model configuration
-        self.model_params = model_params
-        self.cls_labels = cls_labels
-
-        # Training statistics
-        self.training_time = training_time
-        self.inference_time = inference_time
-
-        # Overall accuracy
-        self.accuracy = accuracy_score(y_true, y_pred)
-
-        # Training history
-        self.epochs = history.epoch
-        self.loss = history.history['loss']
-        self.acc = history.history.get('acc') or history.history.get('accuracy')
-        if 'val_loss' in history.history.keys():
-            self.val_loss = history.history['val_loss']
-            self.val_acc = history.history.get('val_acc') or history.history.get('val_accuracy')
-        else:
-            self.val_loss = []
-            self.val_acc = []
-
-        # Accuracy metrics
-        p, r, f1, s = precision_recall_fscore_support(y_true, y_pred, labels=range(len(self.cls_labels)))
-        self.recall = r
-        self.precision = p
-        self.f1_score = f1
-        self.support = s
-        self.mean_precision = np.mean(self.precision)
-        self.mean_recall = np.mean(self.recall)
-        self.mean_f1_score = np.mean(self.f1_score)
-
-        # Save predictions (for later analysis)
-        self.y_true = y_true
-        self.y_pred = y_pred
-        self.y_prob = y_prob
-
+"""
+Results of training
+"""
+import numpy as np
+from sklearn.metrics import precision_recall_fscore_support, accuracy_score
+
+
+class TrainingResult:
+    def __init__(self,
+                 model_params,
+                 history,
+                 y_true,
+                 y_pred,
+                 y_prob,
+                 cls_labels,
+                 training_time,
+                 inference_time):
+
+        # Model configuration
+        self.model_params = model_params
+        self.cls_labels = cls_labels
+
+        # Training statistics
+        self.training_time = training_time
+        self.inference_time = inference_time
+
+        # Overall accuracy
+        self.accuracy = accuracy_score(y_true, y_pred)
+
+        # Training history
+        self.epochs = history.epoch
+        self.loss = history.history['loss']
+        self.acc = history.history.get('acc') or history.history.get('accuracy')
+        if 'val_loss' in history.history.keys():
+            self.val_loss = history.history['val_loss']
+            self.val_acc = history.history.get('val_acc') or history.history.get('val_accuracy')
+        else:
+            self.val_loss = []
+            self.val_acc = []
+
+        # Accuracy metrics
+        p, r, f1, s = precision_recall_fscore_support(y_true, y_pred, labels=range(len(self.cls_labels)))
+        self.recall = r
+        self.precision = p
+        self.f1_score = f1
+        self.support = s
+        self.mean_precision = np.mean(self.precision)
+        self.mean_recall = np.mean(self.recall)
+        self.mean_f1_score = np.mean(self.f1_score)
+
+        # Save predictions (for later analysis)
+        self.y_true = y_true
+        self.y_pred = y_pred
+        self.y_prob = y_prob
+
```

### Comparing `miso2-3.0.3/miso/utils/flowcam.py` & `miso2-3.0.4/miso/utils/flowcam.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,245 +1,245 @@
-import pandas as pd
-import os
-import skimage.io as skio
-from collections import OrderedDict
-from glob import glob
-from tqdm import tqdm
-import argparse
-
-
-def process_dir(input_dir, save_dir, campaign_name, species_filename=None, save_csv=True):
-    # Find all lst files
-    lst_filenames = sorted(glob(os.path.join(input_dir, "**", "*.lst"), recursive=True))
-    print(lst_filenames)
-    # Extract the base directories
-    dirs = [os.path.dirname(fn) for fn in lst_filenames]
-    # Only take unique ones
-    dirs = sorted(list(set(dirs)))
-    # dirs = [d for d in sorted(glob(os.path.join(input_dir, "*"))) if os.path.isdir(d)]
-    df_master = None
-    for d in dirs:
-        # Directory
-        if d == input_dir:
-            run_name = os.path.basename(d).replace("/", "_").replace(" ", "_").replace("\\", "_")
-        else:
-            run_name = d[len(input_dir)+1:].replace("/", "_").replace(" ", "_").replace("\\", "_")
-        df = process(d, save_dir, campaign_name, run_name, species_filename, save_csv=True)
-        if df_master is None:
-            df_master = df
-            print("first")
-            print(len(df_master))
-        else:
-            df_master = df_master.append(df)
-            print("append")
-            print(len(df_master))
-    if save_csv:
-        df_master.to_csv(os.path.join(save_dir, campaign_name, "{}_data.csv".format(campaign_name)), index=False)
-    return df_master
-
-
-def process(input_dir, save_dir, campaign_name, run_name, species_filename=None, save_csv=True, save_mask=False):
-    # Load species conversion list
-    if species_filename is not None and species_filename != "":
-        # noms = pd.read_excel(species_filename, sheet_name=0, engine='openpyxl').dropna()
-        doublons = pd.read_excel(species_filename, sheet_name=1, engine='openpyxl').dropna()
-        # feuil1 = pd.read_excel(species_filename, sheet_name=2, engine='openpyxl').dropna()
-    else:
-        doublons = None
-
-    # The directory where we will save the images
-    im_save_dir = os.path.join(save_dir, campaign_name, "images", run_name)
-    os.makedirs(im_save_dir, exist_ok=True)
-    if save_mask:
-        mask_save_dir = os.path.join(save_dir, campaign_name, "masks", run_name)
-        os.makedirs(mask_save_dir, exist_ok=True)
-    save_dir = os.path.join(save_dir, campaign_name, run_name)
-
-    print('-' * 80)
-    # print("Flowcam segmenter")
-    # print('-' * 80)
-    # print("- species XLSX: {}".format(species_filename))
-    print("Campaign: {}".format(campaign_name))
-    print("Sample: {}".format(run_name))
-    print("- input directory: {}".format(input_dir))
-
-    # Image data
-    lst_filename = glob(os.path.join(input_dir, "*.lst"))
-    if len(lst_filename) == 0:
-        print("! No .lst file found in {}, skipping !".format(input_dir))
-        return
-    lst_filename = lst_filename[0]
-    df = parse_image_list(lst_filename)
-
-    # Classification data
-    cla_filename = glob(os.path.join(input_dir, "*.cla"))
-    if len(cla_filename) == 0 or os.path.getsize(cla_filename[0]) == 0:
-        print("- classification (.cla) file is missing or empty, all images will be placed in \"unlabeled\" class")
-        cls_dict = dict()
-    else:
-        cla_filename = cla_filename[0]
-        cls_dict = parse_classifications(cla_filename)
-        print("- classification filename: {}".format(cla_filename))
-    print("- image data filename: {}".format(lst_filename))
-    print("- output directory: {}".format(save_dir))
-    print("Processing...")
-
-    # Group the results by image
-    df_grouped = df.groupby("collage_file")
-
-    # Extra info to save
-    df_filename = [""] * len(df)
-    df_cls = [""] * len(df)
-    df_campaign = [campaign_name] * len(df)
-    df_sample = [run_name] * len(df)
-
-    # Process each image
-    for filename, group in tqdm(df_grouped):
-        # Load the image
-        im_filename = os.path.join(input_dir, filename)
-        mask_filename = os.path.join(input_dir, filename[:-4] + "_bin.tif")
-
-        if os.path.exists(im_filename):
-            try:
-                im = skio.imread(im_filename)
-            except:
-                print("Error opening image {}".format(im_filename))
-                continue
-        else:
-            print("Image not found {}".format(im_filename))
-
-        is_mask = False
-        if save_mask:
-            if os.path.exists(mask_filename):
-                try:
-                    mask = skio.imread(mask_filename)
-                    is_mask = True
-                except:
-                    print("Error opening {}".format(mask_filename))
-            else:
-                print("Mask not found {}".format(mask_filename))
-
-        # Cut each image out
-        for row in group.iterrows():
-            row_id = row[0]
-            row = row[1]
-            # Get image number
-            id = row['id']
-            # Get class
-            if id in cls_dict:
-                cls = cls_dict[id]
-            else:
-                cls = "unlabeled"
-            # Modify class to correct if needed
-            if doublons is not None and cls in doublons.iloc[:, 0].values:
-                vals = doublons[doublons.iloc[:, 0] == cls]
-                new_cls = vals.iloc[0, 1]
-                cls = new_cls
-            # Get image coordinates
-            x = row['image_x']
-            y = row['image_y']
-            width = row['image_w']
-            height = row['image_h']
-            # Get the segmented image
-            seg_im = im[y:y + height, x:x + width, ...]
-            seg_im_filename = os.path.join(im_save_dir, cls, "{}_{}_{:08d}.png".format(campaign_name, run_name, id))
-            os.makedirs(os.path.dirname(seg_im_filename), exist_ok=True)
-            skio.imsave(seg_im_filename, seg_im)
-            if is_mask:
-                seg_mask = mask[y:y + height, x:x + width, ...]
-                seg_mask_filename = os.path.join(mask_save_dir, cls, "{}_{}_{:08d}.png".format(campaign_name, run_name, id))
-                os.makedirs(os.path.dirname(seg_mask_filename), exist_ok=True)
-                skio.imsave(seg_mask_filename, seg_mask)
-            df_cls[id-1] = cls
-            df_filename[id-1] = seg_im_filename
-    df.insert(0, 'filename', df_filename)
-    df.insert(2, 'campaign', df_campaign)
-    df.insert(3, 'sample', df_sample)
-    df.insert(4, 'class', df_cls)
-    if save_csv:
-        df.to_csv(os.path.join(im_save_dir, "{}_{}_data.csv".format(campaign_name, run_name)), index=False)
-    print("Complete!")
-    return df
-
-
-def parse_classifications(filename):
-    cls_dict = OrderedDict()
-    with open(filename, "r") as f:
-        f.readline()
-        f.readline()
-        f.readline()
-        num_classes = int(f.readline())
-        for i in range(num_classes):
-            cls_name = f.readline()[:-1]
-            f.readline()
-            f.readline()
-            num_images = int(f.readline())
-            for j in range(num_images):
-                idx = int(f.readline())
-                cls_dict[idx] = cls_name
-    return cls_dict
-
-
-def parse_image_list(filename):
-    field_names = []
-    with open(filename, "r") as f:
-        f.readline()
-        numfields = int(f.readline().split('|')[1])
-        for i in range(numfields):
-            field_names.append(f.readline().split('|')[0])
-        # print(field_names)
-    df = pd.read_csv(filename, '|', skiprows=numfields + 2, header=None)
-    df.columns = field_names
-    return df
-
-#
-# def process(folder):
-#     cla_filename = glob(os.path.join(folder, "*.cla"))[0]
-#     lst_filename = glob(os.path.join(folder, "*.lst"))[0]
-#     run_id = os.path.basename(cla_filename)[:-4]
-#
-#     cls_dict = class_list(cla_filename)
-#
-#     field_names = []
-#     with open(lst_filename, "r") as f:
-#         numfields = int(f.readline().split('|')[1])
-#         for i in range(numfields):
-#             field_names.append(f.readline().split('|')[0])
-#         print(field_names)
-#     df = pd.read_csv(lst_filename, '|', skiprows=numfields + 2, header=None)
-#     df.columns = field_names
-#
-#     last_image_name = None
-#     last_image = None
-#     for row in df.iterrows():
-#         row_id = row[0]
-#         row = row[1]
-#         if row['collage_file'] != last_image_name:
-#             last_image_name = row['collage_file']
-#             last_image = skio.imread(os.path.join(folder, last_image_name))
-#         id = row['id']
-#         if id in cls_dict:
-#             cls_name = cls_dict[id]
-#         else:
-#             cls_name = "sans_etiquette"
-#         save_dir = os.path.join(folder, os.path.basename(cla_filename)[:-4] + "_images_individuelles", cls_name)
-#         os.makedirs(save_dir, exist_ok=True)
-#         im = last_image[row['image_y']:row['image_y'] + row['image_h'], row['image_x']:row['image_x'] + row['image_w'], :]
-#         print(os.path.join(save_dir, run_id + "_{:08d}.png".format(id)))
-#         sub_filename = os.path.join(save_dir, run_id + "_{:08d}.png".format(id))
-#         skio.imsave(sub_filename, im)
-#         df.loc[row_id, 'file'] = os.path.basename(sub_filename)
-#     df.to_csv(os.path.join(folder, run_id + "_info.csv"))
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description='Segment flowcam images into individual images sorted by class')
-    parser.add_argument("-i", "--input", type=str, help="Input directory containing the flowcam data CSV file and collated images")
-    parser.add_argument("-o", "--output", type=str, default=None, required=True, help="Output directory to save images (if not used, images will be saved in a directory alongside the data CSV file)")
-    parser.add_argument("-n", "--name", required=True, help="Name of the campaign this sample is from")
-    parser.add_argument("-s", "--species", type=str, required=False,  help="XLSX file with the map of class names to true species identifiers")
-    args = parser.parse_args()
-
-    print('-' * 80)
-    print("Flowcam segmenter")
-    print("- species XLSX: {}".format(args.species))
-    process_dir(args.input, args.output,  args.name, args.species, True)
+import pandas as pd
+import os
+import skimage.io as skio
+from collections import OrderedDict
+from glob import glob
+from tqdm import tqdm
+import argparse
+
+
+def process_dir(input_dir, save_dir, campaign_name, species_filename=None, save_csv=True):
+    # Find all lst files
+    lst_filenames = sorted(glob(os.path.join(input_dir, "**", "*.lst"), recursive=True))
+    print(lst_filenames)
+    # Extract the base directories
+    dirs = [os.path.dirname(fn) for fn in lst_filenames]
+    # Only take unique ones
+    dirs = sorted(list(set(dirs)))
+    # dirs = [d for d in sorted(glob(os.path.join(input_dir, "*"))) if os.path.isdir(d)]
+    df_master = None
+    for d in dirs:
+        # Directory
+        if d == input_dir:
+            run_name = os.path.basename(d).replace("/", "_").replace(" ", "_").replace("\\", "_")
+        else:
+            run_name = d[len(input_dir)+1:].replace("/", "_").replace(" ", "_").replace("\\", "_")
+        df = process(d, save_dir, campaign_name, run_name, species_filename, save_csv=True)
+        if df_master is None:
+            df_master = df
+            print("first")
+            print(len(df_master))
+        else:
+            df_master = df_master.append(df)
+            print("append")
+            print(len(df_master))
+    if save_csv:
+        df_master.to_csv(os.path.join(save_dir, campaign_name, "{}_data.csv".format(campaign_name)), index=False)
+    return df_master
+
+
+def process(input_dir, save_dir, campaign_name, run_name, species_filename=None, save_csv=True, save_mask=False):
+    # Load species conversion list
+    if species_filename is not None and species_filename != "":
+        # noms = pd.read_excel(species_filename, sheet_name=0, engine='openpyxl').dropna()
+        doublons = pd.read_excel(species_filename, sheet_name=1, engine='openpyxl').dropna()
+        # feuil1 = pd.read_excel(species_filename, sheet_name=2, engine='openpyxl').dropna()
+    else:
+        doublons = None
+
+    # The directory where we will save the images
+    im_save_dir = os.path.join(save_dir, campaign_name, "images", run_name)
+    os.makedirs(im_save_dir, exist_ok=True)
+    if save_mask:
+        mask_save_dir = os.path.join(save_dir, campaign_name, "masks", run_name)
+        os.makedirs(mask_save_dir, exist_ok=True)
+    save_dir = os.path.join(save_dir, campaign_name, run_name)
+
+    print('-' * 80)
+    # print("Flowcam segmenter")
+    # print('-' * 80)
+    # print("- species XLSX: {}".format(species_filename))
+    print("Campaign: {}".format(campaign_name))
+    print("Sample: {}".format(run_name))
+    print("- input directory: {}".format(input_dir))
+
+    # Image data
+    lst_filename = glob(os.path.join(input_dir, "*.lst"))
+    if len(lst_filename) == 0:
+        print("! No .lst file found in {}, skipping !".format(input_dir))
+        return
+    lst_filename = lst_filename[0]
+    df = parse_image_list(lst_filename)
+
+    # Classification data
+    cla_filename = glob(os.path.join(input_dir, "*.cla"))
+    if len(cla_filename) == 0 or os.path.getsize(cla_filename[0]) == 0:
+        print("- classification (.cla) file is missing or empty, all images will be placed in \"unlabeled\" class")
+        cls_dict = dict()
+    else:
+        cla_filename = cla_filename[0]
+        cls_dict = parse_classifications(cla_filename)
+        print("- classification filename: {}".format(cla_filename))
+    print("- image data filename: {}".format(lst_filename))
+    print("- output directory: {}".format(save_dir))
+    print("Processing...")
+
+    # Group the results by image
+    df_grouped = df.groupby("collage_file")
+
+    # Extra info to save
+    df_filename = [""] * len(df)
+    df_cls = [""] * len(df)
+    df_campaign = [campaign_name] * len(df)
+    df_sample = [run_name] * len(df)
+
+    # Process each image
+    for filename, group in tqdm(df_grouped):
+        # Load the image
+        im_filename = os.path.join(input_dir, filename)
+        mask_filename = os.path.join(input_dir, filename[:-4] + "_bin.tif")
+
+        if os.path.exists(im_filename):
+            try:
+                im = skio.imread(im_filename)
+            except:
+                print("Error opening image {}".format(im_filename))
+                continue
+        else:
+            print("Image not found {}".format(im_filename))
+
+        is_mask = False
+        if save_mask:
+            if os.path.exists(mask_filename):
+                try:
+                    mask = skio.imread(mask_filename)
+                    is_mask = True
+                except:
+                    print("Error opening {}".format(mask_filename))
+            else:
+                print("Mask not found {}".format(mask_filename))
+
+        # Cut each image out
+        for row in group.iterrows():
+            row_id = row[0]
+            row = row[1]
+            # Get image number
+            id = row['id']
+            # Get class
+            if id in cls_dict:
+                cls = cls_dict[id]
+            else:
+                cls = "unlabeled"
+            # Modify class to correct if needed
+            if doublons is not None and cls in doublons.iloc[:, 0].values:
+                vals = doublons[doublons.iloc[:, 0] == cls]
+                new_cls = vals.iloc[0, 1]
+                cls = new_cls
+            # Get image coordinates
+            x = row['image_x']
+            y = row['image_y']
+            width = row['image_w']
+            height = row['image_h']
+            # Get the segmented image
+            seg_im = im[y:y + height, x:x + width, ...]
+            seg_im_filename = os.path.join(im_save_dir, cls, "{}_{}_{:08d}.png".format(campaign_name, run_name, id))
+            os.makedirs(os.path.dirname(seg_im_filename), exist_ok=True)
+            skio.imsave(seg_im_filename, seg_im)
+            if is_mask:
+                seg_mask = mask[y:y + height, x:x + width, ...]
+                seg_mask_filename = os.path.join(mask_save_dir, cls, "{}_{}_{:08d}.png".format(campaign_name, run_name, id))
+                os.makedirs(os.path.dirname(seg_mask_filename), exist_ok=True)
+                skio.imsave(seg_mask_filename, seg_mask)
+            df_cls[id-1] = cls
+            df_filename[id-1] = seg_im_filename
+    df.insert(0, 'filename', df_filename)
+    df.insert(2, 'campaign', df_campaign)
+    df.insert(3, 'sample', df_sample)
+    df.insert(4, 'class', df_cls)
+    if save_csv:
+        df.to_csv(os.path.join(im_save_dir, "{}_{}_data.csv".format(campaign_name, run_name)), index=False)
+    print("Complete!")
+    return df
+
+
+def parse_classifications(filename):
+    cls_dict = OrderedDict()
+    with open(filename, "r") as f:
+        f.readline()
+        f.readline()
+        f.readline()
+        num_classes = int(f.readline())
+        for i in range(num_classes):
+            cls_name = f.readline()[:-1]
+            f.readline()
+            f.readline()
+            num_images = int(f.readline())
+            for j in range(num_images):
+                idx = int(f.readline())
+                cls_dict[idx] = cls_name
+    return cls_dict
+
+
+def parse_image_list(filename):
+    field_names = []
+    with open(filename, "r") as f:
+        f.readline()
+        numfields = int(f.readline().split('|')[1])
+        for i in range(numfields):
+            field_names.append(f.readline().split('|')[0])
+        # print(field_names)
+    df = pd.read_csv(filename, '|', skiprows=numfields + 2, header=None)
+    df.columns = field_names
+    return df
+
+#
+# def process(folder):
+#     cla_filename = glob(os.path.join(folder, "*.cla"))[0]
+#     lst_filename = glob(os.path.join(folder, "*.lst"))[0]
+#     run_id = os.path.basename(cla_filename)[:-4]
+#
+#     cls_dict = class_list(cla_filename)
+#
+#     field_names = []
+#     with open(lst_filename, "r") as f:
+#         numfields = int(f.readline().split('|')[1])
+#         for i in range(numfields):
+#             field_names.append(f.readline().split('|')[0])
+#         print(field_names)
+#     df = pd.read_csv(lst_filename, '|', skiprows=numfields + 2, header=None)
+#     df.columns = field_names
+#
+#     last_image_name = None
+#     last_image = None
+#     for row in df.iterrows():
+#         row_id = row[0]
+#         row = row[1]
+#         if row['collage_file'] != last_image_name:
+#             last_image_name = row['collage_file']
+#             last_image = skio.imread(os.path.join(folder, last_image_name))
+#         id = row['id']
+#         if id in cls_dict:
+#             cls_name = cls_dict[id]
+#         else:
+#             cls_name = "sans_etiquette"
+#         save_dir = os.path.join(folder, os.path.basename(cla_filename)[:-4] + "_images_individuelles", cls_name)
+#         os.makedirs(save_dir, exist_ok=True)
+#         im = last_image[row['image_y']:row['image_y'] + row['image_h'], row['image_x']:row['image_x'] + row['image_w'], :]
+#         print(os.path.join(save_dir, run_id + "_{:08d}.png".format(id)))
+#         sub_filename = os.path.join(save_dir, run_id + "_{:08d}.png".format(id))
+#         skio.imsave(sub_filename, im)
+#         df.loc[row_id, 'file'] = os.path.basename(sub_filename)
+#     df.to_csv(os.path.join(folder, run_id + "_info.csv"))
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description='Segment flowcam images into individual images sorted by class')
+    parser.add_argument("-i", "--input", type=str, help="Input directory containing the flowcam data CSV file and collated images")
+    parser.add_argument("-o", "--output", type=str, default=None, required=True, help="Output directory to save images (if not used, images will be saved in a directory alongside the data CSV file)")
+    parser.add_argument("-n", "--name", required=True, help="Name of the campaign this sample is from")
+    parser.add_argument("-s", "--species", type=str, required=False,  help="XLSX file with the map of class names to true species identifiers")
+    args = parser.parse_args()
+
+    print('-' * 80)
+    print("Flowcam segmenter")
+    print("- species XLSX: {}".format(args.species))
+    process_dir(args.input, args.output,  args.name, args.species, True)
```

### Comparing `miso2-3.0.3/miso/utils/rolling_buffer.py` & `miso2-3.0.4/miso/utils/rolling_buffer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import numpy as np
-import scipy.stats as stats
-
-class RollingBuffer:
-
-    def __init__(self, buffer_len):
-        self.__buffer = np.zeros(buffer_len)
-        self.__counter = 0
-        self.__buffer_len = buffer_len
-
-    def append(self, data):
-        self.__buffer = np.roll(self.__buffer, -1)
-        self.__buffer[-1] = data
-        self.__counter += 1
-        if self.__counter > self.__buffer_len:
-            self.__counter = self.__buffer_len
-
-    def values(self):
-        return self.__buffer[-self.__counter:]
-
-    def mean(self):
-        return np.sum(self.__buffer) / self.__counter
-
-    def indices(self):
-        return range(self.__counter)
-
-    def clear(self):
-        self.__counter = 0
-
-    def length(self):
-        return self.__buffer_len
-
-    def full(self):
-        return self.__counter == self.__buffer_len
-
-    def slope_probability_less_than(self, prob):
-        idxs = self.indices()
-        n = len(idxs)
-        if n < 3:
-            return 1
-        values = self.values()
-        n = float(n)
-        slope, intercept, r_value, p_value, std_err = stats.linregress(idxs, values)
-        residuals = idxs * slope + intercept
-        variance = np.sum(np.power(residuals - values, 2)) / (n - 2)
-        slope_std_error = np.sqrt(variance * (12.0 / (np.power(n, 3) - n)))
-        p_less_than_zero = stats.norm.cdf(prob, slope, slope_std_error)
-        return p_less_than_zero
+import numpy as np
+import scipy.stats as stats
+
+class RollingBuffer:
+
+    def __init__(self, buffer_len):
+        self.__buffer = np.zeros(buffer_len)
+        self.__counter = 0
+        self.__buffer_len = buffer_len
+
+    def append(self, data):
+        self.__buffer = np.roll(self.__buffer, -1)
+        self.__buffer[-1] = data
+        self.__counter += 1
+        if self.__counter > self.__buffer_len:
+            self.__counter = self.__buffer_len
+
+    def values(self):
+        return self.__buffer[-self.__counter:]
+
+    def mean(self):
+        return np.sum(self.__buffer) / self.__counter
+
+    def indices(self):
+        return range(self.__counter)
+
+    def clear(self):
+        self.__counter = 0
+
+    def length(self):
+        return self.__buffer_len
+
+    def full(self):
+        return self.__counter == self.__buffer_len
+
+    def slope_probability_less_than(self, prob):
+        idxs = self.indices()
+        n = len(idxs)
+        if n < 3:
+            return 1
+        values = self.values()
+        n = float(n)
+        slope, intercept, r_value, p_value, std_err = stats.linregress(idxs, values)
+        residuals = idxs * slope + intercept
+        variance = np.sum(np.power(residuals - values, 2)) / (n - 2)
+        slope_std_error = np.sqrt(variance * (12.0 / (np.power(n, 3) - n)))
+        p_less_than_zero = stats.norm.cdf(prob, slope, slope_std_error)
+        return p_less_than_zero
```

### Comparing `miso2-3.0.3/miso/utils/singleton.py` & `miso2-3.0.4/miso/utils/singleton.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-"""
-Taken from https://github.com/pycontribs/tendo/blob/master/tendo/singleton.py on 01/01/2021 and modified to remove error message
-"""
-
-from multiprocessing import Process
-import os
-import sys
-import tempfile
-import atexit
-
-
-if sys.platform != "win32":
-    import fcntl
-
-
-class SingleInstanceException(BaseException):
-    pass
-
-
-class SingleInstance(object):
-
-    """Class that can be instantiated only once per machine.
-
-    If you want to prevent your script from running in parallel just instantiate SingleInstance() class. If is there another instance already running it will throw a `SingleInstanceException`.
-
-    This option is very useful if you have scripts executed by crontab at small amounts of time.
-
-    Remember that this works by creating a lock file with a filename based on the full path to the script file.
-
-    Providing a flavor_id will augment the filename with the provided flavor_id, allowing you to create multiple singleton instances from the same file. This is particularly useful if you want specific functions to have their own singleton instances.
-    """
-
-    def __init__(self, flavor_id="", lockfile=""):
-        self.initialized = False
-        if lockfile:
-            self.lockfile = lockfile
-        else:
-            basename = os.path.splitext(os.path.abspath(sys.argv[0]))[0].replace(
-                "/", "-").replace(":", "").replace("\\", "-") + '-%s' % flavor_id + '.lock'
-            self.lockfile = os.path.normpath(
-                tempfile.gettempdir() + '/' + basename)
-
-        # logger.debug("SingleInstance lockfile: " + self.lockfile)
-        if sys.platform == 'win32':
-            try:
-                # file already exists, we try to remove (in case previous
-                # execution was interrupted)
-                if os.path.exists(self.lockfile):
-                    os.unlink(self.lockfile)
-                self.fd = os.open(
-                    self.lockfile, os.O_CREAT | os.O_EXCL | os.O_RDWR)
-            except OSError:
-                type, e, tb = sys.exc_info()
-                if e.errno == 13:
-                    # logger.error(
-                    #     "Another instance is already running, quitting.")
-                    raise SingleInstanceException()
-                print(e.errno)
-                raise
-        else:  # non Windows
-            self.fp = open(self.lockfile, 'w')
-            self.fp.flush()
-            try:
-                fcntl.lockf(self.fp, fcntl.LOCK_EX | fcntl.LOCK_NB)
-            except IOError:
-                # logger.warning(
-                #     "Another instance is already running, quitting.")
-                raise SingleInstanceException()
-        self.initialized = True
-        atexit.register(self.__close)
-
-    def __close(self):
-        if not self.initialized:
-            return
-        try:
-            if sys.platform == 'win32':
-                if hasattr(self, 'fd'):
-                    os.close(self.fd)
-                    os.unlink(self.lockfile)
-            else:
-                fcntl.lockf(self.fp, fcntl.LOCK_UN)
-                # os.close(self.fp)
-                if os.path.isfile(self.lockfile):
-                    os.unlink(self.lockfile)
-        except Exception as e:
-            # if logger:
-            #     logger.warning(e)
-            # else:
-            print("Error: %s" % e)
-            sys.exit(-1)
-
-
-def f(name):
-    # tmp = logger.level
-    # logger.setLevel(logging.CRITICAL)  # we do not want to see the warning
-    try:
-        me2 = SingleInstance(flavor_id=name)  # noqa
-    except SingleInstanceException:
-        sys.exit(-1)
-    # logger.setLevel(tmp)
-    pass
-
-
-# class testSingleton(unittest.TestCase):
-#
-#     def test_1(self):
-#         me = SingleInstance(flavor_id="test-1")
-#         del me  # now the lock should be removed
-#         assert True
-#
-#     def test_2(self):
-#         p = Process(target=f, args=("test-2",))
-#         p.start()
-#         p.join()
-#         # the called function should succeed
-#         assert p.exitcode == 0, "%s != 0" % p.exitcode
-#
-#     def test_3(self):
-#         me = SingleInstance(flavor_id="test-3")  # noqa -- me should still kept
-#         p = Process(target=f, args=("test-3",))
-#         p.start()
-#         p.join()
-#         # the called function should fail because we already have another
-#         # instance running
-#         assert p.exitcode != 0, "%s != 0 (2nd execution)" % p.exitcode
-#         # note, we return -1 but this translates to 255 meanwhile we'll
-#         # consider that anything different from 0 is good
-#         p = Process(target=f, args=("test-3",))
-#         p.start()
-#         p.join()
-#         # the called function should fail because we already have another
-#         # instance running
-#         assert p.exitcode != 0, "%s != 0 (3rd execution)" % p.exitcode
-#
-#     def test_4(self):
-#         lockfile = '/tmp/foo.lock'
-#         me = SingleInstance(lockfile=lockfile)
-#         assert me.lockfile == lockfile
-#
-#
-# logger = logging.getLogger("tendo.singleton")
-
-# if __name__ == "__main__":
-#     logger.addHandler(logging.StreamHandler())
-#     logger.setLevel(logging.DEBUG)
+"""
+Taken from https://github.com/pycontribs/tendo/blob/master/tendo/singleton.py on 01/01/2021 and modified to remove error message
+"""
+
+from multiprocessing import Process
+import os
+import sys
+import tempfile
+import atexit
+
+
+if sys.platform != "win32":
+    import fcntl
+
+
+class SingleInstanceException(BaseException):
+    pass
+
+
+class SingleInstance(object):
+
+    """Class that can be instantiated only once per machine.
+
+    If you want to prevent your script from running in parallel just instantiate SingleInstance() class. If is there another instance already running it will throw a `SingleInstanceException`.
+
+    This option is very useful if you have scripts executed by crontab at small amounts of time.
+
+    Remember that this works by creating a lock file with a filename based on the full path to the script file.
+
+    Providing a flavor_id will augment the filename with the provided flavor_id, allowing you to create multiple singleton instances from the same file. This is particularly useful if you want specific functions to have their own singleton instances.
+    """
+
+    def __init__(self, flavor_id="", lockfile=""):
+        self.initialized = False
+        if lockfile:
+            self.lockfile = lockfile
+        else:
+            basename = os.path.splitext(os.path.abspath(sys.argv[0]))[0].replace(
+                "/", "-").replace(":", "").replace("\\", "-") + '-%s' % flavor_id + '.lock'
+            self.lockfile = os.path.normpath(
+                tempfile.gettempdir() + '/' + basename)
+
+        # logger.debug("SingleInstance lockfile: " + self.lockfile)
+        if sys.platform == 'win32':
+            try:
+                # file already exists, we try to remove (in case previous
+                # execution was interrupted)
+                if os.path.exists(self.lockfile):
+                    os.unlink(self.lockfile)
+                self.fd = os.open(
+                    self.lockfile, os.O_CREAT | os.O_EXCL | os.O_RDWR)
+            except OSError:
+                type, e, tb = sys.exc_info()
+                if e.errno == 13:
+                    # logger.error(
+                    #     "Another instance is already running, quitting.")
+                    raise SingleInstanceException()
+                print(e.errno)
+                raise
+        else:  # non Windows
+            self.fp = open(self.lockfile, 'w')
+            self.fp.flush()
+            try:
+                fcntl.lockf(self.fp, fcntl.LOCK_EX | fcntl.LOCK_NB)
+            except IOError:
+                # logger.warning(
+                #     "Another instance is already running, quitting.")
+                raise SingleInstanceException()
+        self.initialized = True
+        atexit.register(self.__close)
+
+    def __close(self):
+        if not self.initialized:
+            return
+        try:
+            if sys.platform == 'win32':
+                if hasattr(self, 'fd'):
+                    os.close(self.fd)
+                    os.unlink(self.lockfile)
+            else:
+                fcntl.lockf(self.fp, fcntl.LOCK_UN)
+                # os.close(self.fp)
+                if os.path.isfile(self.lockfile):
+                    os.unlink(self.lockfile)
+        except Exception as e:
+            # if logger:
+            #     logger.warning(e)
+            # else:
+            print("Error: %s" % e)
+            sys.exit(-1)
+
+
+def f(name):
+    # tmp = logger.level
+    # logger.setLevel(logging.CRITICAL)  # we do not want to see the warning
+    try:
+        me2 = SingleInstance(flavor_id=name)  # noqa
+    except SingleInstanceException:
+        sys.exit(-1)
+    # logger.setLevel(tmp)
+    pass
+
+
+# class testSingleton(unittest.TestCase):
+#
+#     def test_1(self):
+#         me = SingleInstance(flavor_id="test-1")
+#         del me  # now the lock should be removed
+#         assert True
+#
+#     def test_2(self):
+#         p = Process(target=f, args=("test-2",))
+#         p.start()
+#         p.join()
+#         # the called function should succeed
+#         assert p.exitcode == 0, "%s != 0" % p.exitcode
+#
+#     def test_3(self):
+#         me = SingleInstance(flavor_id="test-3")  # noqa -- me should still kept
+#         p = Process(target=f, args=("test-3",))
+#         p.start()
+#         p.join()
+#         # the called function should fail because we already have another
+#         # instance running
+#         assert p.exitcode != 0, "%s != 0 (2nd execution)" % p.exitcode
+#         # note, we return -1 but this translates to 255 meanwhile we'll
+#         # consider that anything different from 0 is good
+#         p = Process(target=f, args=("test-3",))
+#         p.start()
+#         p.join()
+#         # the called function should fail because we already have another
+#         # instance running
+#         assert p.exitcode != 0, "%s != 0 (3rd execution)" % p.exitcode
+#
+#     def test_4(self):
+#         lockfile = '/tmp/foo.lock'
+#         me = SingleInstance(lockfile=lockfile)
+#         assert me.lockfile == lockfile
+#
+#
+# logger = logging.getLogger("tendo.singleton")
+
+# if __name__ == "__main__":
+#     logger.addHandler(logging.StreamHandler())
+#     logger.setLevel(logging.DEBUG)
 #     unittest.main()
```

### Comparing `miso2-3.0.3/miso/utils/wave.py` & `miso2-3.0.4/miso/utils/wave.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-def wave():
-    print("+----------------------------------------------------------------------------------+")
-    # print(",,,.............................................  ... ...   ..........  . ..... ..  .        .      ..                  .           . ...      ........ .  ....")
-    # print(",,,......................................... ..... .. .        .           .....                           ...                                .... ..  .   ....")
-    # print(",,,....................................     .....    .                     . ..                                                               ..  .  .      ...")
-    # print(",,......,,,,,,...........................  . . .       .      .               .                                                      .       . ..... .      ...")
-    # print(",......,..(. ,.........................    ....    .    ,.,.,,            ... ...                           .          .                      .....         ...")
-    # print(",......,../. ,.......................  .    .../.                ..  .                                                                        .  ..          ..")
-    # print(",,.....,..,, ,.....................   .  .*               ,* . .*,.   ,.   .   .                                                             .   ...         ..")
-    # print(",......,..*. ,.... .........           *                  .  **   ., *,  .                                                            .       .     .. .    . .")
-    # print(",.....,,..** *............         ,,                    .*/  *     ../,     .                                                      .     ...... .   ...... ...")
-    # print(",,*/,,.,..(* *.....  .....      /         ..       ,*,*,/   ./ .,, .,/.* .*,*.,    .. . .                                          .   ........... ............")
-    # print("...,/,.....,,*.........  .    (            .*/.    ,*.,, .%*  ..,..**, ,.., //..  ......                                        . . ...........................")
-    # print(",.,*(,,,...,.,.........    ..            .**.(%%%.. //#%%,#%%,*,*. ..*/.*..,,/.*.......                                 .       ...............................")
-    # print(",,,((,,,.,(..,,........../.          ..*..*  .,*%#%%,/*.%%%%%%.   , **.*....,,......                                    .    . ........ .......... ............")
-    # print(",,,/*,,,.,...,,.,...../               .,,,****(%%%%#%%%%(%#%%%%%,,.*. . *.          .*,*.                         .     . ........................  ...........")
-    # print(",,,(*,,,,//,*.,,,...,,             ,%%*%#%.%%%/%%#%%%%%#%%%%%(%% , /(**. .*/.,,   ..,..* ,.                        .   .  .....................................")
-    # print(",,,*/,,,,,,,,,,,,..*                %%#%%%%#%%%/(%#%%%#%%%/%%#%%%%/#(#/. ,... ,.. *.  ...,..                                   ................................")
-    # print(",,,,*,,,,,,,,,,,,/                  %%#%%%(%%%(/%%%%#/%%%%%#%%%%%%%*(*  ,.  */ ,, . *,    ,*.                                    ..............................")
-    # print(",,,,,.,,,,,,,,,/..                   ##%%((%%%#%%%%#(%%%%/%%%/%%%#(#. . .,. *,,, . ,.   ../  **                            .      .  .  . .       ...... . ....")
-    # print(",,,,,,,,,,,,*/.                            (%#*%%%%(%%%#(%%*%&%##(##,.,  * ,**..*    ,,, /        .            .                  ..                          .")
-    # print(",,,,,,**((#...  .        ..,              **.,#%###(%%%###%%%%*###..    *** * . *.   .*,*,     .                                                              .")
-    # print("#%%#%(#**.. .   . .., .,..,*        ,/**   .*%(%%%##%(%.%%*%%%/#,         ,*,,* *. ., ,*.,.*. .  .                                                      .      ")
-    # print("####.... .  .   ...,....*/,.   ... .*..,.*   /#(. ,.#/###%#%%###             /.     ,  ,..  *       .                                                         .")
-    # print("............     ,*... .*.,,**  *, *,,..**/       (*%%(#%%%%###(     .             ,.* ../                                                              .   ,  ")
-    # print("...,,,.,,,*,..,,/,*, .   **,,*..* ,.,, ,.  **,..,,   ,,..(%%###*            .        ,*  /....                   .                                       ..    ")
-    # print("......,*(*/,*,,,*%##/,(.,,../** .,..%%/* #/(%(. ..,,  /#%%(%%##           . .      . .. .......                                                   .    ,       ")
-    # print("...,*/*,//.**.  (%##%,%%,... ,*,,/. %%#*#%%%#//%#    #%%#%/%%(#                   .      .                                                            .        ")
-    # print(".,*,,*,*,/,.,,,***/(%*%%% ,./,,,.,    ,(,./#%%/#*%% %%(%%##%%%/*                                                         .                          .      .,*,")
-    # print("***,,,,,%%*..,*..(*###%%(,..*/.* .*.*. *.*,%%#%%#%%%*/#%(#%%%%(#          .       .                                                                .         ,.")
-    # print(".*,,/#..(%%%###%,%%((%(#.***.,/,/*/ ,. ..,,.%%*#%(#*,/%#%%#%%%%/...... . ...      .                       . .                  . ........   ..  **       .. *..")
-    # print("*,,#*%%,,,#(%*%%#%%%#(%(#...%,#,#*#%,*/*,%*((%%%(%#%####((/*#/(%(,.. .. .. ......      . .   ....       . ...     . .    .. .. .......... .*.,,/.      *,/.(,/#")
-    # print("...,((...,*,/%#%#%%%#/#%%/.#%%%(#(%%%/**.%//%(%/%###    ###%%%%%##/....................  ... .  ...... .........................,,,,.,,,.,//*.*        **,../#%")
-    # print("**..../**.,/,//(%%(%%##/#,%##%#*(*#%#(##%*%%%(##(%(           (%#%%#,,,,,,,,,,........ ........................,...,,.,,,,,,,*,********,#%#*,        ..,* .###%")
-    # print(",*/,,.*/...   ,.**/%%%####%%%(%%%%###%%%%%#%#((#%.              %(#%(*******.,,,,,,,,,.,.,,,,,,,,,,,,,,.,,,,,,,,,,**,,*********/////.#(,##/            /  ,%%%%")
-    # print(".*.,*.*,,.. ,*,,,.*/(*/#%###/*%#%%#%*(#/###(.%,                  #%###****/./**,**********,*************************//*//////////*##,*#(/.        ,....###%(#%%")
-    # print(".*/.**.*.... .///,.//.,/*#*(%#%##%(/%%##/#/%%                    ,.#%%#/,***//////////////////////////////*/////////////////////#(.(///.          *#((%%#%##%%%")
-    # print(",,,,(%,***.((/*/./.*.*,**,,.,/(#/*#%#/#%%%%            .*         ,  /%%/#/////(///////////////////.  .////////////////////////.,//**    ... .(#,(#%%%%#####,.*")
-    # print(",,/%%%*%%(/(%%#,,///*,(,,..*.****...**..             /.,..          .    (#(//((/*(((((((((/(////        ///((((((////////////,..,      .  *.. ,%%%%%%%(...*   ")
-    # print("...%%%#%/%*%%%(##/*/**,*,,/,*#%#*/#*             ./ .*,*             ..      *((/((/((((*((((((            (/((((/(/(#(##*...,/          .###%%%%%#/  .*((    .")
-    # print("....%#(##(.#%*%%%##.*.*,*(*..,##,                .    ...,  .         ..  .*..  (/(((/(((/(,.,/#/%%#*  #,.    /((((/.....,(,      . *..,., #(*/   ..#(#/  .....")
-    # print("......(%,#%,%%((#%#,      ..                ,/.   .,.... .,.,,  . , .   *  ,      /%%%(#%%(%%%#.,(((((((#(#(#(####(,,/(.   ,,.. .**#/#(((*     ./(##(. ........")
-    # print("..........                   ,,,..         ,*. , ....,.     .... #*,*    ,.,/.   /      .#%%%%%%%%########/(,//#(,     ,.*. .*/###(,       ...**/(/  ........*#")
-    # print("..........         ...       .**....  .*,/**,.,.....  *.,* ...,..*(#..,   ,#.((,./##,  #...  *.                 .  .#(.##//,.   ....  ..*/(#(#(#  ........,####")
-    # print("....,,,,,,.        /...      .**,.....  .*.. .*        ..... .##/#,/#*.../  .(%%# /(*(*.##*...            .                 .  /##(#####%#%##/  ......(###(###(")
-    # print("....,,,/,,/*.* ..,.*...    .*, ,..  (.         .,. .    ***   #/#.#*,/.///#   .#%%,#%%#(.#%##....  ....         .. .   ....  .*,,,,........,   ../##%%%%%%#/###")
-    # print("............,*,..,.... %%#,.,..  *.*/.         *.** *..,/ .   /,(((#/,,/##((.*   ,%%#%%%%# ##%%,. .. ....... ......##(/,,. .((####%%%%%%#                .,,*((")
-    # print("........./* *,.(/.,..//.%#/,**/  ,..  ... .  ...../.*. ,.. ,   *(%(#%##,,/,/#//(*.    %%%%%#.(%%%#*...  (%%#... ..(/...*#%%%%%%####((*,  ........../##%%%%%%%%%")
-    # print("....../((***.,%*%%*#.%%%%#**,,/.,, *........ ,. *,,,.*,/ ,.,.   #%#%#%%%#,*//(//,/(#,#(..#%%%%%#%%%%%#*..  (%%%%%/. /%%%%#(//*,/,*(,   .....*//*,(###(/*,**.   ")
-    # print("....#*##%%,%(%*%#%%%%####* ,/,.. ,..... ..,  *.,.. %% ##*.....   .%%%#%%%%(*/,./(/,*(,,,((...,(%%%%%%%%%%#,.. (%%%%%%#(##%###%((/       ....*,/(#(/,   .(######")
-    # print("..,%%%##/(%%(%#%%(%/#. ../,,. %%#,. ....*....,... /%##(* ##*...,.  %#%#%%%#%%*,*,///*,,/(//*,,,,,,*//*,/#%%%%#(*(#.,#(.##,/##.      .((################%%%%%%%%")
-    # print("..%%(,%%*.*,#(%%%//(%%.,(#%%#/%(%%%.* .,/*......   .%%%%%/#/ /(/...  #%%%%%%%#%(,,/*//*,,,,,,,,,,,,,,,,,,,,,,,*(**///*((/    ......*#%%%%%%%%%%%####%%%%%#%%%%%")
-    # print(".*%#%%#%%%%%(#%/%((%%%%%#%#%%%%(##%%%%      ,#     ,*  ./#%##/#%/      .#%%##%%%#%(,*,.............,,**///(///////((.    ..,*##%%%%%##**###(*/(*,.          .,/")
-    # print(".,%#(%(%%%/(%%#%%%%%(%%(#%%*#%%#&%%(.. ../*%%% * .%%/,,*(&/#%&%#..*..   .#%%#%%%%#%%(//...,,*,.....,/**(###*.      ,%%%%%%%%%%%%%%%%%%#.    . ...............  ")
-    # print(".#%/%%#%#%%%%/#%%(%#%%*%##%%%%#%%#%%%, ..,/%.,//,,%%*./..*#%*%/&%&/#/*,..,.    ./%%%%%%%%%#%%%%%%%%%#/,        . ..       .,....     ..........................")
-
-
-def intro():
-    print("+----------------------------------------------------------------------------------+")
-    print("|  MISO Particle Classification Library                                            |")
-    print("+----------------------------------------------------------------------------------+")
-    print("|  To update library:                                                              |")
-    print("|  pip install -U git+http://www.github.com/microfossil/particle-classification    |")
-    print("+----------------------------------------------------------------------------------+")
-
-
+def wave():
+    print("+----------------------------------------------------------------------------------+")
+    # print(",,,.............................................  ... ...   ..........  . ..... ..  .        .      ..                  .           . ...      ........ .  ....")
+    # print(",,,......................................... ..... .. .        .           .....                           ...                                .... ..  .   ....")
+    # print(",,,....................................     .....    .                     . ..                                                               ..  .  .      ...")
+    # print(",,......,,,,,,...........................  . . .       .      .               .                                                      .       . ..... .      ...")
+    # print(",......,..(. ,.........................    ....    .    ,.,.,,            ... ...                           .          .                      .....         ...")
+    # print(",......,../. ,.......................  .    .../.                ..  .                                                                        .  ..          ..")
+    # print(",,.....,..,, ,.....................   .  .*               ,* . .*,.   ,.   .   .                                                             .   ...         ..")
+    # print(",......,..*. ,.... .........           *                  .  **   ., *,  .                                                            .       .     .. .    . .")
+    # print(",.....,,..** *............         ,,                    .*/  *     ../,     .                                                      .     ...... .   ...... ...")
+    # print(",,*/,,.,..(* *.....  .....      /         ..       ,*,*,/   ./ .,, .,/.* .*,*.,    .. . .                                          .   ........... ............")
+    # print("...,/,.....,,*.........  .    (            .*/.    ,*.,, .%*  ..,..**, ,.., //..  ......                                        . . ...........................")
+    # print(",.,*(,,,...,.,.........    ..            .**.(%%%.. //#%%,#%%,*,*. ..*/.*..,,/.*.......                                 .       ...............................")
+    # print(",,,((,,,.,(..,,........../.          ..*..*  .,*%#%%,/*.%%%%%%.   , **.*....,,......                                    .    . ........ .......... ............")
+    # print(",,,/*,,,.,...,,.,...../               .,,,****(%%%%#%%%%(%#%%%%%,,.*. . *.          .*,*.                         .     . ........................  ...........")
+    # print(",,,(*,,,,//,*.,,,...,,             ,%%*%#%.%%%/%%#%%%%%#%%%%%(%% , /(**. .*/.,,   ..,..* ,.                        .   .  .....................................")
+    # print(",,,*/,,,,,,,,,,,,..*                %%#%%%%#%%%/(%#%%%#%%%/%%#%%%%/#(#/. ,... ,.. *.  ...,..                                   ................................")
+    # print(",,,,*,,,,,,,,,,,,/                  %%#%%%(%%%(/%%%%#/%%%%%#%%%%%%%*(*  ,.  */ ,, . *,    ,*.                                    ..............................")
+    # print(",,,,,.,,,,,,,,,/..                   ##%%((%%%#%%%%#(%%%%/%%%/%%%#(#. . .,. *,,, . ,.   ../  **                            .      .  .  . .       ...... . ....")
+    # print(",,,,,,,,,,,,*/.                            (%#*%%%%(%%%#(%%*%&%##(##,.,  * ,**..*    ,,, /        .            .                  ..                          .")
+    # print(",,,,,,**((#...  .        ..,              **.,#%###(%%%###%%%%*###..    *** * . *.   .*,*,     .                                                              .")
+    # print("#%%#%(#**.. .   . .., .,..,*        ,/**   .*%(%%%##%(%.%%*%%%/#,         ,*,,* *. ., ,*.,.*. .  .                                                      .      ")
+    # print("####.... .  .   ...,....*/,.   ... .*..,.*   /#(. ,.#/###%#%%###             /.     ,  ,..  *       .                                                         .")
+    # print("............     ,*... .*.,,**  *, *,,..**/       (*%%(#%%%%###(     .             ,.* ../                                                              .   ,  ")
+    # print("...,,,.,,,*,..,,/,*, .   **,,*..* ,.,, ,.  **,..,,   ,,..(%%###*            .        ,*  /....                   .                                       ..    ")
+    # print("......,*(*/,*,,,*%##/,(.,,../** .,..%%/* #/(%(. ..,,  /#%%(%%##           . .      . .. .......                                                   .    ,       ")
+    # print("...,*/*,//.**.  (%##%,%%,... ,*,,/. %%#*#%%%#//%#    #%%#%/%%(#                   .      .                                                            .        ")
+    # print(".,*,,*,*,/,.,,,***/(%*%%% ,./,,,.,    ,(,./#%%/#*%% %%(%%##%%%/*                                                         .                          .      .,*,")
+    # print("***,,,,,%%*..,*..(*###%%(,..*/.* .*.*. *.*,%%#%%#%%%*/#%(#%%%%(#          .       .                                                                .         ,.")
+    # print(".*,,/#..(%%%###%,%%((%(#.***.,/,/*/ ,. ..,,.%%*#%(#*,/%#%%#%%%%/...... . ...      .                       . .                  . ........   ..  **       .. *..")
+    # print("*,,#*%%,,,#(%*%%#%%%#(%(#...%,#,#*#%,*/*,%*((%%%(%#%####((/*#/(%(,.. .. .. ......      . .   ....       . ...     . .    .. .. .......... .*.,,/.      *,/.(,/#")
+    # print("...,((...,*,/%#%#%%%#/#%%/.#%%%(#(%%%/**.%//%(%/%###    ###%%%%%##/....................  ... .  ...... .........................,,,,.,,,.,//*.*        **,../#%")
+    # print("**..../**.,/,//(%%(%%##/#,%##%#*(*#%#(##%*%%%(##(%(           (%#%%#,,,,,,,,,,........ ........................,...,,.,,,,,,,*,********,#%#*,        ..,* .###%")
+    # print(",*/,,.*/...   ,.**/%%%####%%%(%%%%###%%%%%#%#((#%.              %(#%(*******.,,,,,,,,,.,.,,,,,,,,,,,,,,.,,,,,,,,,,**,,*********/////.#(,##/            /  ,%%%%")
+    # print(".*.,*.*,,.. ,*,,,.*/(*/#%###/*%#%%#%*(#/###(.%,                  #%###****/./**,**********,*************************//*//////////*##,*#(/.        ,....###%(#%%")
+    # print(".*/.**.*.... .///,.//.,/*#*(%#%##%(/%%##/#/%%                    ,.#%%#/,***//////////////////////////////*/////////////////////#(.(///.          *#((%%#%##%%%")
+    # print(",,,,(%,***.((/*/./.*.*,**,,.,/(#/*#%#/#%%%%            .*         ,  /%%/#/////(///////////////////.  .////////////////////////.,//**    ... .(#,(#%%%%#####,.*")
+    # print(",,/%%%*%%(/(%%#,,///*,(,,..*.****...**..             /.,..          .    (#(//((/*(((((((((/(////        ///((((((////////////,..,      .  *.. ,%%%%%%%(...*   ")
+    # print("...%%%#%/%*%%%(##/*/**,*,,/,*#%#*/#*             ./ .*,*             ..      *((/((/((((*((((((            (/((((/(/(#(##*...,/          .###%%%%%#/  .*((    .")
+    # print("....%#(##(.#%*%%%##.*.*,*(*..,##,                .    ...,  .         ..  .*..  (/(((/(((/(,.,/#/%%#*  #,.    /((((/.....,(,      . *..,., #(*/   ..#(#/  .....")
+    # print("......(%,#%,%%((#%#,      ..                ,/.   .,.... .,.,,  . , .   *  ,      /%%%(#%%(%%%#.,(((((((#(#(#(####(,,/(.   ,,.. .**#/#(((*     ./(##(. ........")
+    # print("..........                   ,,,..         ,*. , ....,.     .... #*,*    ,.,/.   /      .#%%%%%%%%########/(,//#(,     ,.*. .*/###(,       ...**/(/  ........*#")
+    # print("..........         ...       .**....  .*,/**,.,.....  *.,* ...,..*(#..,   ,#.((,./##,  #...  *.                 .  .#(.##//,.   ....  ..*/(#(#(#  ........,####")
+    # print("....,,,,,,.        /...      .**,.....  .*.. .*        ..... .##/#,/#*.../  .(%%# /(*(*.##*...            .                 .  /##(#####%#%##/  ......(###(###(")
+    # print("....,,,/,,/*.* ..,.*...    .*, ,..  (.         .,. .    ***   #/#.#*,/.///#   .#%%,#%%#(.#%##....  ....         .. .   ....  .*,,,,........,   ../##%%%%%%#/###")
+    # print("............,*,..,.... %%#,.,..  *.*/.         *.** *..,/ .   /,(((#/,,/##((.*   ,%%#%%%%# ##%%,. .. ....... ......##(/,,. .((####%%%%%%#                .,,*((")
+    # print("........./* *,.(/.,..//.%#/,**/  ,..  ... .  ...../.*. ,.. ,   *(%(#%##,,/,/#//(*.    %%%%%#.(%%%#*...  (%%#... ..(/...*#%%%%%%####((*,  ........../##%%%%%%%%%")
+    # print("....../((***.,%*%%*#.%%%%#**,,/.,, *........ ,. *,,,.*,/ ,.,.   #%#%#%%%#,*//(//,/(#,#(..#%%%%%#%%%%%#*..  (%%%%%/. /%%%%#(//*,/,*(,   .....*//*,(###(/*,**.   ")
+    # print("....#*##%%,%(%*%#%%%%####* ,/,.. ,..... ..,  *.,.. %% ##*.....   .%%%#%%%%(*/,./(/,*(,,,((...,(%%%%%%%%%%#,.. (%%%%%%#(##%###%((/       ....*,/(#(/,   .(######")
+    # print("..,%%%##/(%%(%#%%(%/#. ../,,. %%#,. ....*....,... /%##(* ##*...,.  %#%#%%%#%%*,*,///*,,/(//*,,,,,,*//*,/#%%%%#(*(#.,#(.##,/##.      .((################%%%%%%%%")
+    # print("..%%(,%%*.*,#(%%%//(%%.,(#%%#/%(%%%.* .,/*......   .%%%%%/#/ /(/...  #%%%%%%%#%(,,/*//*,,,,,,,,,,,,,,,,,,,,,,,*(**///*((/    ......*#%%%%%%%%%%%####%%%%%#%%%%%")
+    # print(".*%#%%#%%%%%(#%/%((%%%%%#%#%%%%(##%%%%      ,#     ,*  ./#%##/#%/      .#%%##%%%#%(,*,.............,,**///(///////((.    ..,*##%%%%%##**###(*/(*,.          .,/")
+    # print(".,%#(%(%%%/(%%#%%%%%(%%(#%%*#%%#&%%(.. ../*%%% * .%%/,,*(&/#%&%#..*..   .#%%#%%%%#%%(//...,,*,.....,/**(###*.      ,%%%%%%%%%%%%%%%%%%#.    . ...............  ")
+    # print(".#%/%%#%#%%%%/#%%(%#%%*%##%%%%#%%#%%%, ..,/%.,//,,%%*./..*#%*%/&%&/#/*,..,.    ./%%%%%%%%%#%%%%%%%%%#/,        . ..       .,....     ..........................")
+
+
+def intro():
+    print("+----------------------------------------------------------------------------------+")
+    print("|  MISO Particle Classification Library                                            |")
+    print("+----------------------------------------------------------------------------------+")
+    print("|  To update library:                                                              |")
+    print("|  pip install -U git+http://www.github.com/microfossil/particle-classification    |")
+    print("+----------------------------------------------------------------------------------+")
+
+
```

### Comparing `miso2-3.0.3/miso2.egg-info/PKG-INFO` & `miso2-3.0.4/miso2.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1
-Name: miso2
-Version: 3.0.3
-Summary: Python scripts for training CNNs for particle classification
-Home-page: https://github.com/microfossil/particle-classification
-Author: Ross Marchant
-Author-email: ross.g.marchant@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/microfossil/particle-classification
-Project-URL: Paper, https://jm.copernicus.org/articles/39/183/2020/
-Keywords: microfossil,cnn
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
-# particle-classification
-Python scripts for particle classification
-
-https://stackoverflow.com/questions/53779509/upload-failed-403-invalid-or-non-existent-authentication-information-python
+Metadata-Version: 2.1
+Name: miso2
+Version: 3.0.4
+Summary: Python scripts for training CNNs for particle classification
+Home-page: https://github.com/microfossil/particle-classification
+Author: Ross Marchant
+Author-email: ross.g.marchant@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/microfossil/particle-classification
+Project-URL: Paper, https://jm.copernicus.org/articles/39/183/2020/
+Keywords: microfossil,cnn
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
+# particle-classification
+Python scripts for particle classification
+
+https://stackoverflow.com/questions/53779509/upload-failed-403-invalid-or-non-existent-authentication-information-python
```

### Comparing `miso2-3.0.3/miso2.egg-info/SOURCES.txt` & `miso2-3.0.4/miso2.egg-info/SOURCES.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 LICENCE.txt
 README.md
 setup.py
 miso/__init__.py
 miso/__main__.py
+miso2.egg-info/PKG-INFO
+miso2.egg-info/SOURCES.txt
+miso2.egg-info/dependency_links.txt
+miso2.egg-info/requires.txt
+miso2.egg-info/top_level.txt
 miso/data/__init__.py
 miso/data/dataset.py
 miso/data/download.py
 miso/data/filenames_dataset.py
 miso/data/image_dataset.py
 miso/data/image_loader.py
 miso/data/image_utils.py
@@ -47,13 +52,8 @@
 miso/training/training_result.py
 miso/utils/__init__.py
 miso/utils/flowcam.py
 miso/utils/lock.py
 miso/utils/misc.py
 miso/utils/rolling_buffer.py
 miso/utils/singleton.py
-miso/utils/wave.py
-miso2.egg-info/PKG-INFO
-miso2.egg-info/SOURCES.txt
-miso2.egg-info/dependency_links.txt
-miso2.egg-info/requires.txt
-miso2.egg-info/top_level.txt
+miso/utils/wave.py
```

### Comparing `miso2-3.0.3/setup.py` & `miso2-3.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from setuptools import setup
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-long_description = (here / 'README.md').read_text(encoding='utf-8')
-
-setup(
-    name='miso2',
-    version='3.0.3',
-    description='Python scripts for training CNNs for particle classification',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='Ross Marchant',
-    author_email='ross.g.marchant@gmail.com',
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Science/Research',
-    ],
-    keywords='microfossil, cnn',
-    python_requires='>=3.6',
-    packages=['miso', 'miso.data', 'miso.deploy', 'miso.layers', 'miso.models', 'miso.stats', 'miso.training', 'miso.utils'],
-    install_requires=['image-classifiers>=1.0.0',
-                      'lxml',
-                      'matplotlib',
-                      'numpy',
-                      'pandas',
-                      'Pillow',
-                      'imagecodecs',
-                      'scikit-image',
-                      'scikit-learn',
-                      'scipy',
-                      'segmentation-models',
-                      'dill',
-                      'flask==1.1.2',
-                      'itsdangerous==1.1.0',
-                      'tqdm',
-                      'openpyxl',
-                      'imblearn',
-                      'tf2onnx',
-                      'cleanlab',
-                      'packaging',
-                      'tensorflow_addons'],
-    url='https://github.com/microfossil/particle-classification',
-    license='MIT',
-    project_urls={  # Optional
-        'Source': 'https://github.com/microfossil/particle-classification',
-        'Paper': 'https://jm.copernicus.org/articles/39/183/2020/',
-    },
-)
+from setuptools import setup
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+long_description = (here / 'README.md').read_text(encoding='utf-8')
+
+setup(
+    name='miso2',
+    version='3.0.4',
+    description='Python scripts for training CNNs for particle classification',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author='Ross Marchant',
+    author_email='ross.g.marchant@gmail.com',
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Science/Research',
+    ],
+    keywords='microfossil, cnn',
+    python_requires='>=3.6',
+    packages=['miso', 'miso.data', 'miso.deploy', 'miso.layers', 'miso.models', 'miso.stats', 'miso.training', 'miso.utils'],
+    install_requires=['image-classifiers>=1.0.0',
+                      'lxml',
+                      'matplotlib',
+                      'numpy',
+                      'pandas',
+                      'Pillow',
+                      'imagecodecs',
+                      'scikit-image',
+                      'scikit-learn',
+                      'scipy',
+                      'segmentation-models',
+                      'dill',
+                      'flask==1.1.2',
+                      'itsdangerous==1.1.0',
+                      'tqdm',
+                      'openpyxl',
+                      'imblearn',
+                      'tf2onnx',
+                      'cleanlab',
+                      'packaging',
+                      'tensorflow_addons'],
+    url='https://github.com/microfossil/particle-classification',
+    license='MIT',
+    project_urls={  # Optional
+        'Source': 'https://github.com/microfossil/particle-classification',
+        'Paper': 'https://jm.copernicus.org/articles/39/183/2020/',
+    },
+)
```


# Comparing `tmp/tensorneko-0.2.8.tar.gz` & `tmp/tensorneko-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorneko-0.2.8.tar", last modified: Mon Nov 21 22:38:17 2022, max compression
+gzip compressed data, was "tensorneko-0.2.9.tar", last modified: Mon Jan 30 22:08:36 2023, max compression
```

## Comparing `tensorneko-0.2.8.tar` & `tensorneko-0.2.9.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.789716 tensorneko-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-11-21 22:36:12.000000 tensorneko-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18039 2022-11-21 22:38:17.785716 tensorneko-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16993 2022-11-21 22:36:12.000000 tensorneko-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-21 22:38:17.789716 tensorneko-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-11-21 22:36:12.000000 tensorneko-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.757716 tensorneko-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.765716 tensorneko-0.2.8/src/tensorneko/
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.765716 tensorneko-0.2.8/src/tensorneko/arch/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/arch/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     7194 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/arch/gan.py
--rw-r--r--   0 runner    (1001) docker     (121)     3730 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/arch/vqvae.py
--rw-r--r--   0 runner    (1001) docker     (121)     4712 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/arch/wgan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.769716 tensorneko-0.2.8/src/tensorneko/backend/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.769716 tensorneko-0.2.8/src/tensorneko/callback/
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/callback/display_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/callback/earlystop_lr.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/callback/epoch_num_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/callback/epoch_time_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/callback/lr_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/callback/nil_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.773716 tensorneko-0.2.8/src/tensorneko/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/dataset/nested_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/dataset/round_robin_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.773716 tensorneko-0.2.8/src/tensorneko/debug/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.773716 tensorneko-0.2.8/src/tensorneko/evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/evaluation/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     4371 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/evaluation/fid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2914 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/evaluation/iou.py
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/evaluation/psnr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/evaluation/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.773716 tensorneko-0.2.8/src/tensorneko/io/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.773716 tensorneko-0.2.8/src/tensorneko/io/mesh/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/io/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/io/mesh/mesh_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/io/mesh/mesh_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/io/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.777716 tensorneko-0.2.8/src/tensorneko/layer/
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6360 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/attention.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (121)     5904 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/conv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3283 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     4796 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/masked_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/noise.py
--rw-r--r--   0 runner    (1001) docker     (121)     6585 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/patching.py
--rw-r--r--   0 runner    (1001) docker     (121)     4283 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/positional_embedding.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/reshape.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2178 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/layer/vector_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.781716 tensorneko-0.2.8/src/tensorneko/module/
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3060 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/module/dense.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/module/gated_conv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2462 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/module/inception.py
--rw-r--r--   0 runner    (1001) docker     (121)     3361 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/module/mlp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2958 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/module/residual.py
--rw-r--r--   0 runner    (1001) docker     (121)     7602 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/module/transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9231 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/neko_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/neko_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     8482 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/neko_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.781716 tensorneko-0.2.8/src/tensorneko/notebook/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.781716 tensorneko-0.2.8/src/tensorneko/optim/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.781716 tensorneko-0.2.8/src/tensorneko/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/optim/lr_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.785716 tensorneko-0.2.8/src/tensorneko/preprocess/
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/preprocess/crop.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/preprocess/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.785716 tensorneko-0.2.8/src/tensorneko/preprocess/face_detector/
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/preprocess/face_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/preprocess/pad.py
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/preprocess/resize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.785716 tensorneko-0.2.8/src/tensorneko/util/
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2455 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/util/dispatched_func.py
--rw-r--r--   0 runner    (1001) docker     (121)     4523 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/util/func.py
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/util/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/util/string_getter.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/util/type.py
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-21 22:38:17.000000 tensorneko-0.2.8/src/tensorneko/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.785716 tensorneko-0.2.8/src/tensorneko/visualization/
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.785716 tensorneko-0.2.8/src/tensorneko/visualization/image_browser/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/visualization/image_browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/visualization/log_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/visualization/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.785716 tensorneko-0.2.8/src/tensorneko/visualization/watcher/
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-11-21 22:36:12.000000 tensorneko-0.2.8/src/tensorneko/visualization/watcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.765716 tensorneko-0.2.8/src/tensorneko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18039 2022-11-21 22:38:17.000000 tensorneko-0.2.8/src/tensorneko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-11-21 22:38:17.000000 tensorneko-0.2.8/src/tensorneko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 22:38:17.000000 tensorneko-0.2.8/src/tensorneko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-11-21 22:38:17.000000 tensorneko-0.2.8/src/tensorneko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-21 22:38:17.000000 tensorneko-0.2.8/src/tensorneko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 22:38:17.785716 tensorneko-0.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-21 22:36:12.000000 tensorneko-0.2.8/test/test_library_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-11-21 22:36:12.000000 tensorneko-0.2.8/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.785670 tensorneko-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-01-30 22:06:06.000000 tensorneko-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    18081 2023-01-30 22:08:36.785670 tensorneko-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17035 2023-01-30 22:06:06.000000 tensorneko-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-30 22:08:36.785670 tensorneko-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-01-30 22:06:06.000000 tensorneko-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.737670 tensorneko-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.745670 tensorneko-0.2.9/src/tensorneko/
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.745670 tensorneko-0.2.9/src/tensorneko/arch/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/arch/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7194 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/arch/gan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3730 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/arch/vqvae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/arch/wgan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.749670 tensorneko-0.2.9/src/tensorneko/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.753670 tensorneko-0.2.9/src/tensorneko/callback/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/display_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/earlystop_lr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/epoch_num_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/epoch_time_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/gpu_stats_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/lr_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/nil_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/system_stats_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.753670 tensorneko-0.2.9/src/tensorneko/dataset/
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/dataset/nested_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/dataset/round_robin_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.753670 tensorneko-0.2.9/src/tensorneko/debug/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.757670 tensorneko-0.2.9/src/tensorneko/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/fid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/iou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.757670 tensorneko-0.2.9/src/tensorneko/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.761670 tensorneko-0.2.9/src/tensorneko/io/mesh/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/mesh/mesh_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/mesh/mesh_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.769670 tensorneko-0.2.9/src/tensorneko/layer/
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6360 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4796 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/masked_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/noise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4283 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/positional_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/stack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/vector_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.773670 tensorneko-0.2.9/src/tensorneko/module/
+-rw-r--r--   0 runner    (1001) docker     (122)      403 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/dense.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/gated_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/inception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/residual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7602 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9231 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/neko_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/neko_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8734 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/neko_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.773670 tensorneko-0.2.9/src/tensorneko/notebook/
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.773670 tensorneko-0.2.9/src/tensorneko/optim/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.773670 tensorneko-0.2.9/src/tensorneko/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/optim/lr_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.773670 tensorneko-0.2.9/src/tensorneko/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/crop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.777670 tensorneko-0.2.9/src/tensorneko/preprocess/face_detector/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/face_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/pad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2262 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/resize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.781670 tensorneko-0.2.9/src/tensorneko/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/dispatched_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4523 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/string_getter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/type.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.781670 tensorneko-0.2.9/src/tensorneko/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.781670 tensorneko-0.2.9/src/tensorneko/visualization/image_browser/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/visualization/image_browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1507 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/visualization/log_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/visualization/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.781670 tensorneko-0.2.9/src/tensorneko/visualization/watcher/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/visualization/watcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.745670 tensorneko-0.2.9/src/tensorneko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    18081 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.785670 tensorneko-0.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-01-30 22:06:06.000000 tensorneko-0.2.9/test/test_library_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-01-30 22:06:06.000000 tensorneko-0.2.9/test/test_version.py
```

### Comparing `tensorneko-0.2.8/LICENSE` & `tensorneko-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/PKG-INFO` & `tensorneko-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
@@ -38,16 +38,16 @@
 <div align="center">    
     <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tensorneko?style=flat-square"></a>
     <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-%3E%3D1.9.0-EE4C2C?style=flat-square&logo=pytorch"></a>
     <a href="https://www.pytorchlightning.ai/"><img src="https://img.shields.io/badge/Pytorch%20Lightning-1.7.*-792EE5?style=flat-square&logo=pytorch-lightning"></a>
 </div>
 
 <div align="center">
-    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/workflow/status/ControlNet/tensorneko/Unittest/dev?label=unittest&style=flat-square"></a>
-    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/workflow/status/ControlNet/tensorneko/Release/master?label=release&style=flat-square"></a>
+    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/unittest.yml?branch=dev&label=unittest&style=flat-square"></a>
+    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/release.yml?branch=master&label=release&style=flat-square"></a>
 </div>
 
 Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 
 ## Install
 
 ```shell
@@ -421,15 +421,15 @@
 - `psnr_image`
 - `ssim_video`
 - `ssim_image`
 
 
 ## Neko Utilities
 
-### Functional
+### Misc functions
 
 `__`: The arguments to pipe operator. (Inspired from [fn.py](https://github.com/kachayev/fn.py))
 ```python
 from tensorneko.util import __, _
 result = __(20) >> (_ + 1) >> (_ * 2) >> __.get
 print(result)
 # 42
```

### Comparing `tensorneko-0.2.8/README.md` & `tensorneko-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 <div align="center">    
     <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tensorneko?style=flat-square"></a>
     <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-%3E%3D1.9.0-EE4C2C?style=flat-square&logo=pytorch"></a>
     <a href="https://www.pytorchlightning.ai/"><img src="https://img.shields.io/badge/Pytorch%20Lightning-1.7.*-792EE5?style=flat-square&logo=pytorch-lightning"></a>
 </div>
 
 <div align="center">
-    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/workflow/status/ControlNet/tensorneko/Unittest/dev?label=unittest&style=flat-square"></a>
-    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/workflow/status/ControlNet/tensorneko/Release/master?label=release&style=flat-square"></a>
+    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/unittest.yml?branch=dev&label=unittest&style=flat-square"></a>
+    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/release.yml?branch=master&label=release&style=flat-square"></a>
 </div>
 
 Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 
 ## Install
 
 ```shell
@@ -395,15 +395,15 @@
 - `psnr_image`
 - `ssim_video`
 - `ssim_image`
 
 
 ## Neko Utilities
 
-### Functional
+### Misc functions
 
 `__`: The arguments to pipe operator. (Inspired from [fn.py](https://github.com/kachayev/fn.py))
 ```python
 from tensorneko.util import __, _
 result = __(20) >> (_ + 1) >> (_ * 2) >> __.get
 print(result)
 # 42
```

### Comparing `tensorneko-0.2.8/setup.py` & `tensorneko-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/__init__.py` & `tensorneko-0.2.9/src/tensorneko/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/arch/auto_encoder.py` & `tensorneko-0.2.9/src/tensorneko/arch/auto_encoder.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/arch/gan.py` & `tensorneko-0.2.9/src/tensorneko/arch/gan.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/arch/vqvae.py` & `tensorneko-0.2.9/src/tensorneko/arch/vqvae.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/arch/wgan.py` & `tensorneko-0.2.9/src/tensorneko/arch/wgan.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/callback/earlystop_lr.py` & `tensorneko-0.2.9/src/tensorneko/callback/earlystop_lr.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/callback/epoch_time_logger.py` & `tensorneko-0.2.9/src/tensorneko/callback/epoch_time_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/callback/lr_logger.py` & `tensorneko-0.2.9/src/tensorneko/callback/lr_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/dataset/nested_dataset.py` & `tensorneko-0.2.9/src/tensorneko/dataset/nested_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/dataset/round_robin_dataset.py` & `tensorneko-0.2.9/src/tensorneko/dataset/round_robin_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/evaluation/fid.py` & `tensorneko-0.2.9/src/tensorneko/evaluation/fid.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/evaluation/iou.py` & `tensorneko-0.2.9/src/tensorneko/evaluation/iou.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/evaluation/psnr.py` & `tensorneko-0.2.9/src/tensorneko/evaluation/psnr.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/evaluation/ssim.py` & `tensorneko-0.2.9/src/tensorneko/evaluation/ssim.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/io/reader.py` & `tensorneko-0.2.9/src/tensorneko/io/reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/io/writer.py` & `tensorneko-0.2.9/src/tensorneko/io/writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/__init__.py` & `tensorneko-0.2.9/src/tensorneko/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/aggregation.py` & `tensorneko-0.2.9/src/tensorneko/layer/aggregation.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/attention.py` & `tensorneko-0.2.9/src/tensorneko/layer/attention.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/concatenate.py` & `tensorneko-0.2.9/src/tensorneko/layer/concatenate.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/conv.py` & `tensorneko-0.2.9/src/tensorneko/layer/conv.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/linear.py` & `tensorneko-0.2.9/src/tensorneko/layer/linear.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/log.py` & `tensorneko-0.2.9/src/tensorneko/layer/log.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/masked_conv2d.py` & `tensorneko-0.2.9/src/tensorneko/layer/masked_conv2d.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/noise.py` & `tensorneko-0.2.9/src/tensorneko/layer/noise.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/patching.py` & `tensorneko-0.2.9/src/tensorneko/layer/patching.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/positional_embedding.py` & `tensorneko-0.2.9/src/tensorneko/layer/positional_embedding.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/reshape.py` & `tensorneko-0.2.9/src/tensorneko/layer/reshape.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/stack.py` & `tensorneko-0.2.9/src/tensorneko/layer/stack.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/layer/vector_quantizer.py` & `tensorneko-0.2.9/src/tensorneko/layer/vector_quantizer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/module/dense.py` & `tensorneko-0.2.9/src/tensorneko/module/dense.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/module/gated_conv.py` & `tensorneko-0.2.9/src/tensorneko/module/gated_conv.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/module/inception.py` & `tensorneko-0.2.9/src/tensorneko/module/inception.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/module/mlp.py` & `tensorneko-0.2.9/src/tensorneko/module/mlp.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/module/residual.py` & `tensorneko-0.2.9/src/tensorneko/module/residual.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/module/transformer.py` & `tensorneko-0.2.9/src/tensorneko/module/transformer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/neko_model.py` & `tensorneko-0.2.9/src/tensorneko/neko_model.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/neko_module.py` & `tensorneko-0.2.9/src/tensorneko/neko_module.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/neko_trainer.py` & `tensorneko-0.2.9/src/tensorneko/neko_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pytorch_lightning.callbacks import ModelCheckpoint, Checkpoint
 from pytorch_lightning.loggers import Logger, TensorBoardLogger
 from pytorch_lightning.plugins import PLUGIN_INPUT
 from pytorch_lightning.profilers import Profiler
 from pytorch_lightning.strategies import Strategy
 from pytorch_lightning.trainer.connectors.accelerator_connector import _LITERAL_WARN
 
-from .callback import NilCallback, LrLogger, EpochNumLogger, EpochTimeLogger
+from .callback import NilCallback, LrLogger, EpochNumLogger, EpochTimeLogger, GpuStatsLogger, SystemStatsLogger
 
 
 class NekoTrainer(Trainer):
 
     def __init__(self,
         logger: Optional[str],
         enable_checkpointing: bool = True,
@@ -102,14 +102,30 @@
             cbs = [callbacks, new_callback]
         else:
             cbs = callbacks + [new_callback]
 
         # set learning rate logger
         cbs.extend([LrLogger(), EpochNumLogger(), EpochTimeLogger()])
 
+        # if gpumonitor is installed, enable callback
+        try:
+            gpu_cb = GpuStatsLogger()
+        except ImportError:
+            pass
+        else:
+            cbs.append(gpu_cb)
+
+        # if psutil is installed, enable callback
+        try:
+            sys_cb = SystemStatsLogger()
+        except ImportError:
+            pass
+        else:
+            cbs.append(sys_cb)
+
         # setup the log mode
         self.log_every_n_steps = log_every_n_steps
         self.log_on_epoch = log_every_n_steps == 0
         self.log_on_step = log_every_n_steps > 0
         if self.log_on_epoch:
             log_every_n_steps = 10000000
 
@@ -166,20 +182,20 @@
             move_metrics_to_cpu=move_metrics_to_cpu,
             multiple_trainloader_mode=multiple_trainloader_mode
         )
         # init loggers for training and validation
         self.has_no_logger = logger is None
 
         self.logger_train = TensorBoardLogger(save_dir=self.default_root_dir, name="logs",
-                                              version=os.path.join(self.log_name, "train"), log_graph=False
-                                              # TODO: Fix log_Graph
-                                              ) if self.has_no_logger is not None else None
+            version=os.path.join(self.log_name, "train"), log_graph=False
+            # TODO: Fix log_Graph
+        ) if self.has_no_logger is not None else None
         self.logger_val = TensorBoardLogger(save_dir=self.default_root_dir, name="logs",
-                                            version=os.path.join(self.log_name, "val"), log_graph=False
-                                            ) if self.has_no_logger is not None else None
+            version=os.path.join(self.log_name, "val"), log_graph=False
+        ) if self.has_no_logger is not None else None
         self._loggers = []
 
     @property
     def logger(self) -> Optional[Logger]:
         if self.has_no_logger:
             return None
         if self.training:
```

### Comparing `tensorneko-0.2.8/src/tensorneko/preprocess/__init__.py` & `tensorneko-0.2.9/src/tensorneko/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/preprocess/crop.py` & `tensorneko-0.2.9/src/tensorneko/preprocess/crop.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/preprocess/enum.py` & `tensorneko-0.2.9/src/tensorneko/preprocess/enum.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/preprocess/pad.py` & `tensorneko-0.2.9/src/tensorneko/preprocess/pad.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/preprocess/resize.py` & `tensorneko-0.2.9/src/tensorneko/preprocess/resize.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/util/__init__.py` & `tensorneko-0.2.9/src/tensorneko/util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from einops.layers.torch import Rearrange as _Rearrange
 
 from tensorneko_util.util import dispatch, AverageMeter, tensorneko_util_path
 from tensorneko_util.util.fp import Seq, AbstractSeq, curry, F, Stream, return_option, Option, Monad, Eval, _, __
 from tensorneko_util.util import ref, Timer, Singleton
 from tensorneko_util.util.eventbus import Event, EventBus, EventHandler, subscribe, subscribe_async, \
     subscribe_process, subscribe_thread
+from tensorneko_util.util import download_file, WindowMerger
 from . import type
 from .configuration import Configuration
-from .func import reduce_dict_by, summarize_dict_by, with_printed_shape, is_bad_num, count_parameters, compose, \
+from .misc import reduce_dict_by, summarize_dict_by, with_printed_shape, is_bad_num, count_parameters, compose, \
     generate_inf_seq, listdir, with_printed, ifelse, dict_add, as_list, identity, list_to_dict, circular_pad
-from .func import get_tensorneko_path
-from .dispatched_func import sparse2binary, binary2sparse
+from .misc import get_tensorneko_path
+from .dispatched_misc import sparse2binary, binary2sparse
 from .reproducibility import Seed
 from .string_getter import get_activation, get_loss
 from .type import ModuleFactory, Shape, Device
 
 Rearrange = _Rearrange
 
 tensorneko_path = get_tensorneko_path()
@@ -53,23 +54,24 @@
     "Rearrange",
     "_",
     "F",
     "tensorneko_path",
     "tensorneko_util_path",
     "sparse2binary",
     "binary2sparse",
-    "AbstractServer",
     "dispatch",
     "AverageMeter",
     "AbstractSeq",
     "curry",
     "Timer",
     "Event",
     "EventBus",
     "EventHandler",
     "subscribe",
     "subscribe_async",
     "subscribe_process",
     "subscribe_thread",
     "Singleton",
-    "circular_pad"
+    "circular_pad",
+    "download_file",
+    "WindowMerger",
 ]
```

### Comparing `tensorneko-0.2.8/src/tensorneko/util/configuration.py` & `tensorneko-0.2.9/src/tensorneko/util/configuration.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/util/dispatched_func.py` & `tensorneko-0.2.9/src/tensorneko/util/dispatched_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from torch import Tensor
 
 from tensorneko_util.util import dispatch
-from tensorneko_util.util.dispatched_func import sparse2binary as _sparse2binary
-from tensorneko_util.util.dispatched_func import binary2sparse as _binary2sparse
+from tensorneko_util.util.dispatched_misc import sparse2binary as _sparse2binary
+from tensorneko_util.util.dispatched_misc import binary2sparse as _binary2sparse
 
 
 @dispatch.base(_sparse2binary)
 def sparse2binary(x: Tensor, length: int = None) -> Tensor:
     """
     Convert a sparse tensor to a binary tensor.
```

### Comparing `tensorneko-0.2.8/src/tensorneko/util/func.py` & `tensorneko-0.2.9/src/tensorneko/util/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy
 import numpy as np
 import torch
 from torch import Tensor
 from torch.nn import Module
 
 from tensorneko_util.util import F, _
-from tensorneko_util.util.func import generate_inf_seq, listdir, with_printed, ifelse, dict_add, as_list, \
+from tensorneko_util.util.misc import generate_inf_seq, listdir, with_printed, ifelse, dict_add, as_list, \
     identity, list_to_dict, compose, circular_pad
 from .type import T, A
 
 
 def reduce_dict_by(key: str, op: Callable[[T, T], T]) -> Callable[[List[Dict[str, T]]], T]:
     """
     Apply reducer function to a list of dictionaries.
```

### Comparing `tensorneko-0.2.8/src/tensorneko/util/reproducibility.py` & `tensorneko-0.2.9/src/tensorneko/util/reproducibility.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/util/string_getter.py` & `tensorneko-0.2.9/src/tensorneko/util/string_getter.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/util/type.py` & `tensorneko-0.2.9/src/tensorneko/util/type.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/visualization/__init__.py` & `tensorneko-0.2.9/src/tensorneko/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/visualization/log_graph.py` & `tensorneko-0.2.9/src/tensorneko/visualization/log_graph.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko/visualization/matplotlib.py` & `tensorneko-0.2.9/src/tensorneko/visualization/matplotlib.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.8/src/tensorneko.egg-info/PKG-INFO` & `tensorneko-0.2.9/src/tensorneko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
@@ -38,16 +38,16 @@
 <div align="center">    
     <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tensorneko?style=flat-square"></a>
     <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-%3E%3D1.9.0-EE4C2C?style=flat-square&logo=pytorch"></a>
     <a href="https://www.pytorchlightning.ai/"><img src="https://img.shields.io/badge/Pytorch%20Lightning-1.7.*-792EE5?style=flat-square&logo=pytorch-lightning"></a>
 </div>
 
 <div align="center">
-    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/workflow/status/ControlNet/tensorneko/Unittest/dev?label=unittest&style=flat-square"></a>
-    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/workflow/status/ControlNet/tensorneko/Release/master?label=release&style=flat-square"></a>
+    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/unittest.yml?branch=dev&label=unittest&style=flat-square"></a>
+    <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/release.yml?branch=master&label=release&style=flat-square"></a>
 </div>
 
 Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 
 ## Install
 
 ```shell
@@ -421,15 +421,15 @@
 - `psnr_image`
 - `ssim_video`
 - `ssim_image`
 
 
 ## Neko Utilities
 
-### Functional
+### Misc functions
 
 `__`: The arguments to pipe operator. (Inspired from [fn.py](https://github.com/kachayev/fn.py))
 ```python
 from tensorneko.util import __, _
 result = __(20) >> (_ + 1) >> (_ * 2) >> __.get
 print(result)
 # 42
```

### Comparing `tensorneko-0.2.8/src/tensorneko.egg-info/SOURCES.txt` & `tensorneko-0.2.9/src/tensorneko.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 src/tensorneko/arch/wgan.py
 src/tensorneko/backend/__init__.py
 src/tensorneko/callback/__init__.py
 src/tensorneko/callback/display_metrics_callback.py
 src/tensorneko/callback/earlystop_lr.py
 src/tensorneko/callback/epoch_num_logger.py
 src/tensorneko/callback/epoch_time_logger.py
+src/tensorneko/callback/gpu_stats_logger.py
 src/tensorneko/callback/lr_logger.py
 src/tensorneko/callback/nil_callback.py
+src/tensorneko/callback/system_stats_logger.py
 src/tensorneko/dataset/__init__.py
 src/tensorneko/dataset/nested_dataset.py
 src/tensorneko/dataset/round_robin_dataset.py
 src/tensorneko/debug/__init__.py
 src/tensorneko/evaluation/__init__.py
 src/tensorneko/evaluation/enum.py
 src/tensorneko/evaluation/fid.py
@@ -68,16 +70,16 @@
 src/tensorneko/preprocess/crop.py
 src/tensorneko/preprocess/enum.py
 src/tensorneko/preprocess/pad.py
 src/tensorneko/preprocess/resize.py
 src/tensorneko/preprocess/face_detector/__init__.py
 src/tensorneko/util/__init__.py
 src/tensorneko/util/configuration.py
-src/tensorneko/util/dispatched_func.py
-src/tensorneko/util/func.py
+src/tensorneko/util/dispatched_misc.py
+src/tensorneko/util/misc.py
 src/tensorneko/util/reproducibility.py
 src/tensorneko/util/string_getter.py
 src/tensorneko/util/type.py
 src/tensorneko/visualization/__init__.py
 src/tensorneko/visualization/log_graph.py
 src/tensorneko/visualization/matplotlib.py
 src/tensorneko/visualization/image_browser/__init__.py
```

### Comparing `tensorneko-0.2.8/test/test_version.py` & `tensorneko-0.2.9/test/test_version.py`

 * *Files identical despite different names*


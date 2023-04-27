# Comparing `tmp/chunkflow-1.1.5.tar.gz` & `tmp/chunkflow-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunkflow-1.1.5.tar", last modified: Wed Apr 26 18:13:34 2023, max compression
+gzip compressed data, was "chunkflow-1.1.6.tar", last modified: Wed Apr 26 18:27:27 2023, max compression
```

## Comparing `chunkflow-1.1.5.tar` & `chunkflow-1.1.6.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.769557 chunkflow-1.1.5/
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)    11357 2020-08-10 15:53:37.000000 chunkflow-1.1.5/LICENSE
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      181 2020-08-10 15:53:37.000000 chunkflow-1.1.5/MANIFEST.in
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     8811 2023-04-26 18:13:34.766870 chunkflow-1.1.5/PKG-INFO
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     8011 2023-04-26 17:27:33.000000 chunkflow-1.1.5/README.md
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.288592 chunkflow-1.1.5/chunkflow/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      178 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       45 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/__main__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       18 2023-04-26 18:12:55.000000 chunkflow-1.1.5/chunkflow/__version__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.357872 chunkflow-1.1.5/chunkflow/chunk/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       66 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/chunk/__init__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.369549 chunkflow-1.1.5/chunkflow/chunk/affinity_map/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       29 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/affinity_map/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1447 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/chunk/affinity_map/base.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)    31292 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/chunk/base.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.386544 chunkflow-1.1.5/chunkflow/chunk/image/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       24 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     9513 2022-12-06 02:16:24.000000 chunkflow-1.1.5/chunkflow/chunk/image/adjust_grey.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4532 2022-12-22 17:42:06.000000 chunkflow-1.1.5/chunkflow/chunk/image/base.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.397132 chunkflow-1.1.5/chunkflow/chunk/image/convnet/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)    21829 2022-09-26 15:05:03.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/inferencer.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.436700 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/__init__.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2932 2022-04-01 14:45:22.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/base.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1747 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/identity.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2548 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/patch_mask.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     4447 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/pytorch.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     1240 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/pznet.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2747 2022-09-20 18:00:38.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/universal.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1857 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/chunk/probability_map.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4468 2022-11-15 22:01:01.000000 chunkflow-1.1.5/chunkflow/chunk/segmentation.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2461 2022-04-01 14:41:10.000000 chunkflow-1.1.5/chunkflow/chunk/validate.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.544155 chunkflow-1.1.5/chunkflow/flow/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/flow/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2190 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/flow/aggregate_skeleton_fragments.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      292 2021-02-16 16:29:56.000000 chunkflow-1.1.5/chunkflow/flow/base.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      778 2021-02-16 16:29:56.000000 chunkflow-1.1.5/chunkflow/flow/cloud_watch.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4183 2023-04-26 17:11:23.000000 chunkflow-1.1.5/chunkflow/flow/downsample_upload.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)    96194 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/flow.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1941 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/flow/load_pngs.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     8118 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/load_precomputed.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     1942 2022-04-01 14:41:10.000000 chunkflow-1.1.5/chunkflow/flow/log_summary.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4087 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/mask.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     6645 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/mesh.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2396 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/flow/mesh_manifest.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)    10625 2023-04-26 17:27:32.000000 chunkflow-1.1.5/chunkflow/flow/neuroglancer.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4386 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/plugin.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1859 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/flow/save_pngs.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     5213 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/save_precomputed.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     9147 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/flow/setup_env.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1114 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/skeletonize.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      675 2021-02-16 16:29:56.000000 chunkflow-1.1.5/chunkflow/flow/view.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.582365 chunkflow-1.1.5/chunkflow/lib/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      349 2021-02-16 16:29:56.000000 chunkflow-1.1.5/chunkflow/lib/__init__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.598398 chunkflow-1.1.5/chunkflow/lib/aws/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/lib/aws/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1952 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/lib/aws/cloud_watch.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     7319 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/aws/sqs_queue.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)    23021 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/cartesian_coordinate.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4143 2023-01-24 15:51:25.000000 chunkflow-1.1.5/chunkflow/lib/flow.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.608570 chunkflow-1.1.5/chunkflow/lib/gala/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2021-04-26 17:46:23.000000 chunkflow-1.1.5/chunkflow/lib/gala/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)    48548 2022-09-26 15:05:03.000000 chunkflow-1.1.5/chunkflow/lib/gala/evaluate.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.631085 chunkflow-1.1.5/chunkflow/lib/igneous/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/lib/igneous/__init__.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)    13737 2022-04-01 14:41:11.000000 chunkflow-1.1.5/chunkflow/lib/igneous/downsample.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     4832 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/lib/igneous/downsample_scales.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2525 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/igneous/tasks.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4524 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/region_of_interest.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)    27402 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/synapses.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      497 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/utils.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1337 2023-04-26 17:27:32.000000 chunkflow-1.1.5/chunkflow/point_cloud.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     7051 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/volume.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.329157 chunkflow-1.1.5/chunkflow.egg-info/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     8811 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/PKG-INFO
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2914 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/SOURCES.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/dependency_links.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       55 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/entry_points.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2020-08-10 16:01:41.000000 chunkflow-1.1.5/chunkflow.egg-info/not-zip-safe
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      300 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/requires.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       16 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/top_level.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      301 2023-01-25 17:39:25.000000 chunkflow-1.1.5/requirements.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       38 2023-04-26 18:13:34.770756 chunkflow-1.1.5/setup.cfg
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2251 2022-09-20 17:57:52.000000 chunkflow-1.1.5/setup.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.647773 chunkflow-1.1.5/tests/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      134 2022-04-01 14:41:11.000000 chunkflow-1.1.5/tests/__init__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.663884 chunkflow-1.1.5/tests/chunk/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/__init__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.679714 chunkflow-1.1.5/tests/chunk/image/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/image/__init__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.697556 chunkflow-1.1.5/tests/chunk/image/convnet/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/image/convnet/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     5238 2023-02-01 21:21:25.000000 chunkflow-1.1.5/tests/chunk/image/convnet/test_inferencer.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      739 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/image/convnet/test_patch_mask.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/image/test_adjust_grey.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      294 2022-12-22 16:53:55.000000 chunkflow-1.1.5/tests/chunk/image/test_image.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.708247 chunkflow-1.1.5/tests/chunk/segmentation/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/segmentation/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      643 2022-04-01 14:41:11.000000 chunkflow-1.1.5/tests/chunk/segmentation/test_segmentation.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     6226 2023-04-26 17:27:33.000000 chunkflow-1.1.5/tests/chunk/test_chunk.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      522 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/test_validate.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.760305 chunkflow-1.1.5/tests/flow/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/flow/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      339 2020-09-01 21:59:09.000000 chunkflow-1.1.5/tests/flow/test_cloud_watch.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1900 2022-09-20 17:57:52.000000 chunkflow-1.1.5/tests/flow/test_downsample_upload.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     6958 2023-04-26 17:27:33.000000 chunkflow-1.1.5/tests/flow/test_flow.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2263 2023-01-25 17:33:29.000000 chunkflow-1.1.5/tests/flow/test_load_precomputed.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1839 2022-09-20 17:57:52.000000 chunkflow-1.1.5/tests/flow/test_load_save.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      556 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/flow/test_mesh.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      429 2023-01-25 17:33:14.000000 chunkflow-1.1.5/tests/flow/test_normalize_section_contrast.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1119 2022-09-20 17:57:52.000000 chunkflow-1.1.5/tests/flow/test_save_precomputed.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      140 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/test_command_line.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      948 2023-04-26 17:27:33.000000 chunkflow-1.1.5/tests/test_volume.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.362930 chunkflow-1.1.6/
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)    11357 2020-08-10 15:53:37.000000 chunkflow-1.1.6/LICENSE
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      181 2020-08-10 15:53:37.000000 chunkflow-1.1.6/MANIFEST.in
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     8811 2023-04-26 18:27:27.360571 chunkflow-1.1.6/PKG-INFO
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     8011 2023-04-26 17:27:33.000000 chunkflow-1.1.6/README.md
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:26.925125 chunkflow-1.1.6/chunkflow/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      178 2022-09-20 17:57:52.000000 chunkflow-1.1.6/chunkflow/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       45 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/__main__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       18 2023-04-26 18:26:31.000000 chunkflow-1.1.6/chunkflow/__version__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:26.987660 chunkflow-1.1.6/chunkflow/chunk/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       66 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/chunk/__init__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:26.998527 chunkflow-1.1.6/chunkflow/chunk/affinity_map/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       29 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/chunk/affinity_map/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1447 2022-09-20 17:57:52.000000 chunkflow-1.1.6/chunkflow/chunk/affinity_map/base.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)    31334 2023-04-26 18:21:17.000000 chunkflow-1.1.6/chunkflow/chunk/base.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.015128 chunkflow-1.1.6/chunkflow/chunk/image/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       24 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/chunk/image/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     9513 2022-12-06 02:16:24.000000 chunkflow-1.1.6/chunkflow/chunk/image/adjust_grey.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4532 2022-12-22 17:42:06.000000 chunkflow-1.1.6/chunkflow/chunk/image/base.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.025196 chunkflow-1.1.6/chunkflow/chunk/image/convnet/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/chunk/image/convnet/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)    21829 2022-09-26 15:05:03.000000 chunkflow-1.1.6/chunkflow/chunk/image/convnet/inferencer.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.061371 chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/__init__.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2932 2022-04-01 14:45:22.000000 chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/base.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1747 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/identity.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2548 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/patch_mask.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     4447 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/pytorch.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     1240 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/pznet.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2747 2022-09-20 18:00:38.000000 chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/universal.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1857 2022-09-20 17:57:52.000000 chunkflow-1.1.6/chunkflow/chunk/probability_map.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4468 2022-11-15 22:01:01.000000 chunkflow-1.1.6/chunkflow/chunk/segmentation.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2461 2022-04-01 14:41:10.000000 chunkflow-1.1.6/chunkflow/chunk/validate.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.161090 chunkflow-1.1.6/chunkflow/flow/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/flow/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2190 2022-09-20 17:57:52.000000 chunkflow-1.1.6/chunkflow/flow/aggregate_skeleton_fragments.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      292 2021-02-16 16:29:56.000000 chunkflow-1.1.6/chunkflow/flow/base.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      778 2021-02-16 16:29:56.000000 chunkflow-1.1.6/chunkflow/flow/cloud_watch.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4183 2023-04-26 17:11:23.000000 chunkflow-1.1.6/chunkflow/flow/downsample_upload.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)    96194 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/flow/flow.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1941 2022-09-20 17:57:52.000000 chunkflow-1.1.6/chunkflow/flow/load_pngs.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     8118 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/flow/load_precomputed.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     1942 2022-04-01 14:41:10.000000 chunkflow-1.1.6/chunkflow/flow/log_summary.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4087 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/flow/mask.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     6645 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/flow/mesh.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2396 2022-09-20 17:57:52.000000 chunkflow-1.1.6/chunkflow/flow/mesh_manifest.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)    10625 2023-04-26 17:27:32.000000 chunkflow-1.1.6/chunkflow/flow/neuroglancer.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4386 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/flow/plugin.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1859 2022-09-20 17:57:52.000000 chunkflow-1.1.6/chunkflow/flow/save_pngs.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     5213 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/flow/save_precomputed.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     9147 2022-09-20 17:57:52.000000 chunkflow-1.1.6/chunkflow/flow/setup_env.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1114 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/flow/skeletonize.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      675 2021-02-16 16:29:56.000000 chunkflow-1.1.6/chunkflow/flow/view.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.193524 chunkflow-1.1.6/chunkflow/lib/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      349 2021-02-16 16:29:56.000000 chunkflow-1.1.6/chunkflow/lib/__init__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.208195 chunkflow-1.1.6/chunkflow/lib/aws/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/lib/aws/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1952 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/lib/aws/cloud_watch.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     7319 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/lib/aws/sqs_queue.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)    23021 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/lib/cartesian_coordinate.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4143 2023-01-24 15:51:25.000000 chunkflow-1.1.6/chunkflow/lib/flow.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.217935 chunkflow-1.1.6/chunkflow/lib/gala/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2021-04-26 17:46:23.000000 chunkflow-1.1.6/chunkflow/lib/gala/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)    48548 2022-09-26 15:05:03.000000 chunkflow-1.1.6/chunkflow/lib/gala/evaluate.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.238065 chunkflow-1.1.6/chunkflow/lib/igneous/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.6/chunkflow/lib/igneous/__init__.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)    13737 2022-04-01 14:41:11.000000 chunkflow-1.1.6/chunkflow/lib/igneous/downsample.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     4832 2022-09-20 17:57:52.000000 chunkflow-1.1.6/chunkflow/lib/igneous/downsample_scales.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2525 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/lib/igneous/tasks.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4524 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/lib/region_of_interest.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)    27402 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/lib/synapses.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      497 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/lib/utils.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1337 2023-04-26 17:27:32.000000 chunkflow-1.1.6/chunkflow/point_cloud.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     7051 2023-04-26 17:27:33.000000 chunkflow-1.1.6/chunkflow/volume.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:26.961600 chunkflow-1.1.6/chunkflow.egg-info/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     8811 2023-04-26 18:27:26.000000 chunkflow-1.1.6/chunkflow.egg-info/PKG-INFO
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2914 2023-04-26 18:27:26.000000 chunkflow-1.1.6/chunkflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2023-04-26 18:27:26.000000 chunkflow-1.1.6/chunkflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       55 2023-04-26 18:27:26.000000 chunkflow-1.1.6/chunkflow.egg-info/entry_points.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2020-08-10 16:01:41.000000 chunkflow-1.1.6/chunkflow.egg-info/not-zip-safe
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      306 2023-04-26 18:27:26.000000 chunkflow-1.1.6/chunkflow.egg-info/requires.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       16 2023-04-26 18:27:26.000000 chunkflow-1.1.6/chunkflow.egg-info/top_level.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      306 2023-04-26 18:22:14.000000 chunkflow-1.1.6/requirements.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       38 2023-04-26 18:27:27.363986 chunkflow-1.1.6/setup.cfg
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2251 2022-09-20 17:57:52.000000 chunkflow-1.1.6/setup.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.253719 chunkflow-1.1.6/tests/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      134 2022-04-01 14:41:11.000000 chunkflow-1.1.6/tests/__init__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.268702 chunkflow-1.1.6/tests/chunk/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.6/tests/chunk/__init__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.283840 chunkflow-1.1.6/tests/chunk/image/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.6/tests/chunk/image/__init__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.299423 chunkflow-1.1.6/tests/chunk/image/convnet/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.6/tests/chunk/image/convnet/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     5238 2023-02-01 21:21:25.000000 chunkflow-1.1.6/tests/chunk/image/convnet/test_inferencer.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      739 2020-08-10 15:53:37.000000 chunkflow-1.1.6/tests/chunk/image/convnet/test_patch_mask.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2020-08-10 15:53:37.000000 chunkflow-1.1.6/tests/chunk/image/test_adjust_grey.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      294 2022-12-22 16:53:55.000000 chunkflow-1.1.6/tests/chunk/image/test_image.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.309166 chunkflow-1.1.6/tests/chunk/segmentation/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.6/tests/chunk/segmentation/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      643 2022-04-01 14:41:11.000000 chunkflow-1.1.6/tests/chunk/segmentation/test_segmentation.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     6226 2023-04-26 17:27:33.000000 chunkflow-1.1.6/tests/chunk/test_chunk.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      522 2020-08-10 15:53:37.000000 chunkflow-1.1.6/tests/chunk/test_validate.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:27:27.354837 chunkflow-1.1.6/tests/flow/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.6/tests/flow/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      339 2020-09-01 21:59:09.000000 chunkflow-1.1.6/tests/flow/test_cloud_watch.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1900 2022-09-20 17:57:52.000000 chunkflow-1.1.6/tests/flow/test_downsample_upload.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     6958 2023-04-26 17:27:33.000000 chunkflow-1.1.6/tests/flow/test_flow.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2263 2023-01-25 17:33:29.000000 chunkflow-1.1.6/tests/flow/test_load_precomputed.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1839 2022-09-20 17:57:52.000000 chunkflow-1.1.6/tests/flow/test_load_save.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      556 2020-08-10 15:53:37.000000 chunkflow-1.1.6/tests/flow/test_mesh.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      429 2023-01-25 17:33:14.000000 chunkflow-1.1.6/tests/flow/test_normalize_section_contrast.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1119 2022-09-20 17:57:52.000000 chunkflow-1.1.6/tests/flow/test_save_precomputed.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      140 2020-08-10 15:53:37.000000 chunkflow-1.1.6/tests/test_command_line.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      948 2023-04-26 17:27:33.000000 chunkflow-1.1.6/tests/test_volume.py
```

### Comparing `chunkflow-1.1.5/LICENSE` & `chunkflow-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/PKG-INFO` & `chunkflow-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chunkflow
-Version: 1.1.5
+Version: 1.1.6
 Summary: Composable image chunk operators to create pipeline for distributed computation.
 Home-page: https://github.com/seung-lab/chunkflow
 Author: Jingpeng Wu
 Author-email: jingpeng.wu@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `chunkflow-1.1.5/README.md` & `chunkflow-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/affinity_map/base.py` & `chunkflow-1.1.6/chunkflow/chunk/affinity_map/base.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/base.py` & `chunkflow-1.1.6/chunkflow/chunk/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 import numpy as np
 import nrrd
 from numpy.core.numerictypes import issubdtype
 from numpy.lib.mixins import NDArrayOperatorsMixin
 
 import tifffile
 import cc3d
-from cloudvolume.lib import yellow, Bbox
+from scipy.ndimage import gaussian_filter
 
+from cloudvolume.lib import yellow, Bbox
 from chunkflow.lib.cartesian_coordinate import BoundingBox, Cartesian
 
 # from typing import Tuple
 # Offset = Tuple[int, int, int]
 from .validate import validate_by_template_matching
 
 def layer_type_is_valid(type: str):
```

### Comparing `chunkflow-1.1.5/chunkflow/chunk/image/adjust_grey.py` & `chunkflow-1.1.6/chunkflow/chunk/image/adjust_grey.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/image/base.py` & `chunkflow-1.1.6/chunkflow/chunk/image/base.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/image/convnet/inferencer.py` & `chunkflow-1.1.6/chunkflow/chunk/image/convnet/inferencer.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/base.py` & `chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/base.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/identity.py` & `chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/identity.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/patch_mask.py` & `chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/patch_mask.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/pytorch.py` & `chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/pytorch.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/pznet.py` & `chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/pznet.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/universal.py` & `chunkflow-1.1.6/chunkflow/chunk/image/convnet/patch/universal.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/probability_map.py` & `chunkflow-1.1.6/chunkflow/chunk/probability_map.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/segmentation.py` & `chunkflow-1.1.6/chunkflow/chunk/segmentation.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/chunk/validate.py` & `chunkflow-1.1.6/chunkflow/chunk/validate.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/aggregate_skeleton_fragments.py` & `chunkflow-1.1.6/chunkflow/flow/aggregate_skeleton_fragments.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/cloud_watch.py` & `chunkflow-1.1.6/chunkflow/flow/cloud_watch.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/downsample_upload.py` & `chunkflow-1.1.6/chunkflow/flow/downsample_upload.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/flow.py` & `chunkflow-1.1.6/chunkflow/flow/flow.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/load_pngs.py` & `chunkflow-1.1.6/chunkflow/flow/load_pngs.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/load_precomputed.py` & `chunkflow-1.1.6/chunkflow/flow/load_precomputed.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/log_summary.py` & `chunkflow-1.1.6/chunkflow/flow/log_summary.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/mask.py` & `chunkflow-1.1.6/chunkflow/flow/mask.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/mesh.py` & `chunkflow-1.1.6/chunkflow/flow/mesh.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/mesh_manifest.py` & `chunkflow-1.1.6/chunkflow/flow/mesh_manifest.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/neuroglancer.py` & `chunkflow-1.1.6/chunkflow/flow/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/plugin.py` & `chunkflow-1.1.6/chunkflow/flow/plugin.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/save_pngs.py` & `chunkflow-1.1.6/chunkflow/flow/save_pngs.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/save_precomputed.py` & `chunkflow-1.1.6/chunkflow/flow/save_precomputed.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/setup_env.py` & `chunkflow-1.1.6/chunkflow/flow/setup_env.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/skeletonize.py` & `chunkflow-1.1.6/chunkflow/flow/skeletonize.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/flow/view.py` & `chunkflow-1.1.6/chunkflow/flow/view.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/lib/aws/cloud_watch.py` & `chunkflow-1.1.6/chunkflow/lib/aws/cloud_watch.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/lib/aws/sqs_queue.py` & `chunkflow-1.1.6/chunkflow/lib/aws/sqs_queue.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/lib/cartesian_coordinate.py` & `chunkflow-1.1.6/chunkflow/lib/cartesian_coordinate.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/lib/flow.py` & `chunkflow-1.1.6/chunkflow/lib/flow.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/lib/gala/evaluate.py` & `chunkflow-1.1.6/chunkflow/lib/gala/evaluate.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/lib/igneous/downsample.py` & `chunkflow-1.1.6/chunkflow/lib/igneous/downsample.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/lib/igneous/downsample_scales.py` & `chunkflow-1.1.6/chunkflow/lib/igneous/downsample_scales.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/lib/igneous/tasks.py` & `chunkflow-1.1.6/chunkflow/lib/igneous/tasks.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/lib/region_of_interest.py` & `chunkflow-1.1.6/chunkflow/lib/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/lib/synapses.py` & `chunkflow-1.1.6/chunkflow/lib/synapses.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/point_cloud.py` & `chunkflow-1.1.6/chunkflow/point_cloud.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow/volume.py` & `chunkflow-1.1.6/chunkflow/volume.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/chunkflow.egg-info/PKG-INFO` & `chunkflow-1.1.6/chunkflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chunkflow
-Version: 1.1.5
+Version: 1.1.6
 Summary: Composable image chunk operators to create pipeline for distributed computation.
 Home-page: https://github.com/seung-lab/chunkflow
 Author: Jingpeng Wu
 Author-email: jingpeng.wu@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `chunkflow-1.1.5/chunkflow.egg-info/SOURCES.txt` & `chunkflow-1.1.6/chunkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/setup.py` & `chunkflow-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/chunk/image/convnet/test_inferencer.py` & `chunkflow-1.1.6/tests/chunk/image/convnet/test_inferencer.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/chunk/image/convnet/test_patch_mask.py` & `chunkflow-1.1.6/tests/chunk/image/convnet/test_patch_mask.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/chunk/segmentation/test_segmentation.py` & `chunkflow-1.1.6/tests/chunk/segmentation/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/chunk/test_chunk.py` & `chunkflow-1.1.6/tests/chunk/test_chunk.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/chunk/test_validate.py` & `chunkflow-1.1.6/tests/chunk/test_validate.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/flow/test_downsample_upload.py` & `chunkflow-1.1.6/tests/flow/test_downsample_upload.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/flow/test_flow.py` & `chunkflow-1.1.6/tests/flow/test_flow.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/flow/test_load_precomputed.py` & `chunkflow-1.1.6/tests/flow/test_load_precomputed.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/flow/test_load_save.py` & `chunkflow-1.1.6/tests/flow/test_load_save.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/flow/test_mesh.py` & `chunkflow-1.1.6/tests/flow/test_mesh.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/flow/test_save_precomputed.py` & `chunkflow-1.1.6/tests/flow/test_save_precomputed.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.5/tests/test_volume.py` & `chunkflow-1.1.6/tests/test_volume.py`

 * *Files identical despite different names*


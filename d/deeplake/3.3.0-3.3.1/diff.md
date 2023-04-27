# Comparing `tmp/deeplake-3.3.0.tar.gz` & `tmp/deeplake-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.3.0.tar", last modified: Fri Apr 21 16:42:44 2023, max compression
+gzip compressed data, was "deeplake-3.3.1.tar", last modified: Thu Apr 27 11:15:50 2023, max compression
```

## Comparing `deeplake-3.3.0.tar` & `deeplake-3.3.1.tar`

### file list

```diff
@@ -1,359 +1,359 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.899397 deeplake-3.3.0/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-04-21 16:17:02.000000 deeplake-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-21 16:17:02.000000 deeplake-3.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    22282 2023-04-21 16:42:44.899397 deeplake-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21602 2023-04-21 16:17:02.000000 deeplake-3.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.866897 deeplake-3.3.0/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.866897 deeplake-3.3.0/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88813 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    79221 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6439 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    23071 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     6352 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     3308 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    17730 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2331 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7389 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7081 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12918 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5926 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17970 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     5936 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9632 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   108709 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   166412 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    14750 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11405 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4242 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    18879 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    11242 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15953 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13294 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    19976 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    23069 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      441 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    18475 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    24900 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    48988 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7404 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    10122 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4547 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47159 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    28835 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5373 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     5774 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19402 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5745 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    28992 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4349 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    24153 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22695 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     4890 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5463 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61310 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6052 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7073 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4053 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     5010 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      390 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      179 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     3931 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    15328 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.899397 deeplake-3.3.0/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-21 16:19:35.000000 deeplake-3.3.0/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4435 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5381 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34379 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37298 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.899397 deeplake-3.3.0/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4206 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     6762 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.899397 deeplake-3.3.0/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    23774 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31017 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.899397 deeplake-3.3.0/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.866897 deeplake-3.3.0/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22282 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10849 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 16:38:18.000000 deeplake-3.3.0/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      918 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-04-21 16:42:44.899397 deeplake-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3289 2023-04-21 16:17:02.000000 deeplake-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.404925 deeplake-3.3.1/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-04-27 11:10:18.000000 deeplake-3.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-27 11:10:18.000000 deeplake-3.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    22282 2023-04-27 11:15:50.404925 deeplake-3.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21602 2023-04-27 11:10:18.000000 deeplake-3.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88813 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    79221 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    23071 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    17730 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7081 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12918 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5926 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17970 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     5936 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   108710 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   166287 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14750 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11405 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    18879 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    11242 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15953 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13294 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    19976 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    18475 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    24900 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    48988 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7404 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    10122 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47159 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    28835 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5373 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     5774 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19402 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5745 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    28992 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4349 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    24153 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22695 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5463 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6270 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7073 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     5010 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      179 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.394925 deeplake-3.3.1/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    15328 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.404925 deeplake-3.3.1/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-27 11:12:06.000000 deeplake-3.3.1/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5381 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34379 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37298 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.404925 deeplake-3.3.1/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     6762 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.404925 deeplake-3.3.1/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    23774 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31017 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.404925 deeplake-3.3.1/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-04-27 11:10:18.000000 deeplake-3.3.1/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:15:50.384925 deeplake-3.3.1/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22282 2023-04-27 11:15:50.000000 deeplake-3.3.1/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10849 2023-04-27 11:15:50.000000 deeplake-3.3.1/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:15:50.000000 deeplake-3.3.1/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-27 11:15:50.000000 deeplake-3.3.1/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:15:24.000000 deeplake-3.3.1/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      918 2023-04-27 11:15:50.000000 deeplake-3.3.1/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-27 11:15:50.000000 deeplake-3.3.1/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-04-27 11:15:50.404925 deeplake-3.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-04-27 11:10:18.000000 deeplake-3.3.1/setup.py
```

### Comparing `deeplake-3.3.0/LICENSE` & `deeplake-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/PKG-INFO` & `deeplake-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.3.0
+Version: 3.3.1
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.3.0 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.3.1 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
 Provides-Extra: gcp Provides-Extra: gdrive Provides-Extra: medical Provides-
```

### Comparing `deeplake-3.3.0/README.md` & `deeplake-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/__init__.py` & `deeplake-3.3.1/deeplake/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.3.0"
+__version__ = "3.3.1"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.3.0/deeplake/api/dataset.py` & `deeplake-3.3.1/deeplake/api/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/info.py` & `deeplake-3.3.1/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/link.py` & `deeplake-3.3.1/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/link_tiled.py` & `deeplake-3.3.1/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/read.py` & `deeplake-3.3.1/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_access_method.py` & `deeplake-3.3.1/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_agreement.py` & `deeplake-3.3.1/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_api.py` & `deeplake-3.3.1/deeplake/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.3.1/deeplake/api/tests/test_api_tiling.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,7 +195,20 @@
     num_chunks = 0
     for k in ds.storage:
         if k.startswith("image/chunks/"):
             chunk = ds.storage[k].tobytes()
             num_chunks += 1
             assert 16 * MB < len(chunk) < 20 * MB
     assert num_chunks == 4
+
+
+def test_tiled_indexing(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("abc", sample_compression="lz4")
+        arr = np.random.randn(10, 50, 193, 501)
+        ds.abc.extend(arr)
+        np.testing.assert_array_equal(ds.abc[:, 2], arr[:, 2])
+        np.testing.assert_array_equal(ds.abc[:, [2]], arr[:, [2]])
+        np.testing.assert_array_equal(ds.abc[:, [3, 4, 5]], arr[:, [3, 4, 5]])
+        np.testing.assert_array_equal(
+            ds.abc[:, [3, 4, 5], [6, 7, 8]], arr[:, [3, 4, 5], [6, 7, 8]]
+        )
```

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.3.1/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.3.1/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.3.1/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_dataset.py` & `deeplake-3.3.1/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_dicom.py` & `deeplake-3.3.1/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_downsample.py` & `deeplake-3.3.1/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_events.py` & `deeplake-3.3.1/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_grayscale.py` & `deeplake-3.3.1/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_info.py` & `deeplake-3.3.1/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.3.1/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_json.py` & `deeplake-3.3.1/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_link.py` & `deeplake-3.3.1/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.3.1/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_linking.py` & `deeplake-3.3.1/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_mesh.py` & `deeplake-3.3.1/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_meta.py` & `deeplake-3.3.1/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_nifti.py` & `deeplake-3.3.1/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_none.py` & `deeplake-3.3.1/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.3.1/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_pickle.py` & `deeplake-3.3.1/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.3.1/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_polygons.py` & `deeplake-3.3.1/deeplake/api/tests/test_polygons.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             assert len(s1) == len(s2)
             assert type(s2) == list
             for p1, p2 in zip(s1, s2):
                 assert isinstance(p2, np.ndarray)
                 np.testing.assert_array_equal(p1, p2)
     for i, sample in enumerate(ds.pytorch(num_workers=2)):
         assert len(samples[i]) == len(sample["polygons"])
+
         for p1, p2 in zip(samples[i], sample["polygons"]):
             np.testing.assert_array_equal(p1, p2[0])
     idxs = [2, 2, 6, 4, 6, 7]
     view = ds[idxs]
     ds.commit()
     view.save_view()
     materialized = deeplake.empty("mem://")
@@ -88,7 +89,30 @@
     arr2 = np.random.randint(0, 10, (3, 3, 2))
     with memory_ds as ds:
         ds.create_tensor("polygons", htype="polygon", chunk_compression="lz4")
         ds.polygons.append(arr1)
         ds.polygons.append(arr2)
     np.testing.assert_array_equal(ds.polygons.numpy()[0], arr1)
     np.testing.assert_array_equal(ds.polygons.numpy()[1], arr2)
+
+
+def test_polygon_transform_bug(local_ds):
+    @deeplake.compute
+    def upload(stuff, ds):
+        ds.p1.append(stuff["p_sample"])
+        ds.p2.append(stuff["p_chunk"])
+        ds.p3.append(stuff["p_none"])
+
+    with local_ds as ds:
+        ds.create_tensor("p_none", htype="polygon")
+        ds.p_none.extend(np.random.randint(0, 10, (10, 3, 3, 2)))
+        ds.create_tensor("p_sample", htype="polygon", sample_compression="lz4")
+        ds.p_sample.extend(np.random.randint(0, 10, (10, 3, 3, 2)))
+        ds.create_tensor("p_chunk", htype="polygon", chunk_compression="lz4")
+        ds.p_chunk.extend(np.random.randint(0, 10, (10, 3, 3, 2)))
+
+    ds2 = deeplake.empty(local_ds.path + "_2", overwrite=True)
+    ds2.create_tensor("p1", htype="polygon")
+    ds2.create_tensor("p2", htype="polygon", sample_compression="lz4")
+    ds2.create_tensor("p3", htype="polygon", chunk_compression="lz4")
+
+    upload().eval(ds, ds2, num_workers=2)
```

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_pop.py` & `deeplake-3.3.1/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_readonly.py` & `deeplake-3.3.1/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_rechunk.py` & `deeplake-3.3.1/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_reset.py` & `deeplake-3.3.1/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_sample_info.py` & `deeplake-3.3.1/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_text.py` & `deeplake-3.3.1/deeplake/api/tests/test_text.py`

 * *Files 23% similar despite different names*

```diff
@@ -73,7 +73,24 @@
     ds = memory_ds
     with ds:
         ds.create_tensor("x", htype="text", max_chunk_size=16, **args)
         ds.x.extend(["abcd"] * 100)
         assert len(ds.x.chunk_engine.chunk_id_encoder.array) > 2
         ds.rechunk()
     assert ds.x.numpy().reshape(-1).tolist() == ["abcd"] * 100
+
+
+def test_text_tensor_append(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("x", htype="text", chunk_compression="lz4")
+        ds.create_tensor("y", htype="json")
+        ds.x.extend(["x", "y", "z"])
+        ds.y.extend([{"a": "b"}, {"b": "c"}, {"c": "d"}])
+        ds2 = deeplake.empty("mem://")
+        with ds2:
+            ds2.create_tensor("x", htype="text")
+            ds2.create_tensor("y", htype="json", chunk_compression="lz4")
+            ds2.x.extend(ds.x)
+            ds2.y.extend(ds.y)
+        for i in range(3):
+            assert ds.x[i].data() == ds2.x[i].data()
+            assert ds.y[i].data() == ds2.y[i].data()
```

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_update_samples.py` & `deeplake-3.3.1/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_video.py` & `deeplake-3.3.1/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tests/test_views.py` & `deeplake-3.3.1/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/api/tiled.py` & `deeplake-3.3.1/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/structured/base.py` & `deeplake-3.3.1/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/structured/dataframe.py` & `deeplake-3.3.1/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.3.1/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.3.1/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.3.1/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.3.1/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/unstructured/base.py` & `deeplake-3.3.1/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.3.1/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.3.1/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.3.1/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.3.1/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.3.1/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.3.1/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/unstructured/util.py` & `deeplake-3.3.1/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.3.1/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.3.1/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/cli/auth.py` & `deeplake-3.3.1/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/cli/test_cli.py` & `deeplake-3.3.1/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/client/client.py` & `deeplake-3.3.1/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/client/config.py` & `deeplake-3.3.1/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/client/log.py` & `deeplake-3.3.1/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/client/test_client.py` & `deeplake-3.3.1/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/client/utils.py` & `deeplake-3.3.1/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/compression.py` & `deeplake-3.3.1/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/constants.py` & `deeplake-3.3.1/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/chunk/base_chunk.py` & `deeplake-3.3.1/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.3.1/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.3.1/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.3.1/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.3.1/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.3.1/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.3.1/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,27 +221,28 @@
                 else:
                     raise e
 
             if not bps_empty:
                 sb, eb = bps[local_index]
                 buffer = buffer[sb:eb]
 
+        if self.tensor_meta.htype == "polygon":
+            return Polygons.frombuffer(
+                bytes(buffer),
+                dtype=self.tensor_meta.dtype,
+                ndim=shape[-1],
+            )
+
         if not decompress:
             if copy:
                 buffer = bytes(buffer)
             return buffer
         if self.is_text_like:
             buffer = bytes(buffer)
             return bytes_to_text(buffer, self.htype)
-        if self.tensor_meta.htype == "polygon":
-            return Polygons.frombuffer(
-                bytes(buffer),
-                dtype=self.tensor_meta.dtype,
-                ndim=shape[-1],
-            )
         ret = np.frombuffer(buffer, dtype=self.dtype).reshape(shape)
         if copy and not ret.flags["WRITEABLE"]:
             ret = ret.copy()
         return ret
 
     def update_sample(self, local_index: int, sample: InputSample):
         self.prepare_for_write()
```

### Comparing `deeplake-3.3.0/deeplake/core/chunk_engine.py` & `deeplake-3.3.1/deeplake/core/chunk_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1612,15 +1612,15 @@
         dt, ht = tensor_meta.dtype, tensor_meta.htype
         samples = intelligent_cast(samples, dt, ht)
         getattr(view, operator)(samples)
         self._update(index1, arr)
 
     def read_bytes_for_sample(self, global_sample_index: int) -> bytes:
         if self.chunk_compression:
-            raise Exception(
+            raise ValueError(
                 "Cannot retreive original bytes for samples in chunk-wise compressed tensors."
             )
         enc = self.chunk_id_encoder
         chunks = self.get_chunks_for_sample(global_sample_index)
         if len(chunks) > 1:
             raise NotImplementedError(
                 "read_bytes_for_sample() is not implemented for tiled samples."
```

### Comparing `deeplake-3.3.0/deeplake/core/compression.py` & `deeplake-3.3.1/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/compute/process.py` & `deeplake-3.3.1/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/compute/provider.py` & `deeplake-3.3.1/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/compute/ray.py` & `deeplake-3.3.1/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/compute/serial.py` & `deeplake-3.3.1/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/compute/thread.py` & `deeplake-3.3.1/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/dataset/__init__.py` & `deeplake-3.3.1/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/dataset/dataset.py` & `deeplake-3.3.1/deeplake/core/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -3427,39 +3427,37 @@
             ]
             if unlink
             else False,
         )
 
         def _copy_tensor(sample_in, sample_out):
             for tensor_name in dest_ds.tensors:
-                src = self[tensor_name]
+                src = sample_in[tensor_name]
                 if (
                     unlink
                     and src.is_link
                     and (src.base_htype != "video" or deeplake.constants._UNLINK_VIDEOS)
                 ):
-                    if len(self.index) > 1:
-                        sample_out[tensor_name].extend(sample_in[tensor_name])
+                    if len(sample_in.index) > 1:
+                        sample_out[tensor_name].extend(src)
                     else:
-                        if self.index.subscriptable_at(0):
-                            sample_idxs = list(
-                                sample_in.index.values[0].indices(len(self))
+                        if sample_in.index.subscriptable_at(0):
+                            sample_idxs = sample_in.index.values[0].indices(
+                                src.num_samples
                             )
                         else:
-                            sample_idxs = [self.index.values[0].value]
+                            sample_idxs = [sample_in.index.values[0].value]
                         sample_out[tensor_name].extend(
                             [
-                                sample_in[
-                                    tensor_name
-                                ].chunk_engine.get_deeplake_read_sample(sample_idx)
-                                for sample_idx in sample_idxs
+                                src.chunk_engine.get_deeplake_read_sample(i)
+                                for i in sample_idxs
                             ]
                         )
                 else:
-                    sample_out[tensor_name].extend(sample_in[tensor_name])
+                    sample_out[tensor_name].extend(src)
 
         if not self.index.subscriptable_at(0):
             old_first_index = self.index.values[0]
             new_first_index = IndexEntry(
                 slice(old_first_index.value, old_first_index.value + 1)
             )
             self.index.values[0] = new_first_index
```

### Comparing `deeplake-3.3.0/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.3.1/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.3.1/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.3.1/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/dataset/invalid_view.py` & `deeplake-3.3.1/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/dataset/view_entry.py` & `deeplake-3.3.1/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/fast_forwarding.py` & `deeplake-3.3.1/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/index/index.py` & `deeplake-3.3.1/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/io.py` & `deeplake-3.3.1/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/ipc.py` & `deeplake-3.3.1/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/link_creds.py` & `deeplake-3.3.1/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/linked_chunk_engine.py` & `deeplake-3.3.1/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/linked_sample.py` & `deeplake-3.3.1/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/linked_tiled_sample.py` & `deeplake-3.3.1/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/lock.py` & `deeplake-3.3.1/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/dataset_meta.py` & `deeplake-3.3.1/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.3.1/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.3.1/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.3.1/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/creds.py` & `deeplake-3.3.1/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/pad.py` & `deeplake-3.3.1/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/sequence.py` & `deeplake-3.3.1/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/shape.py` & `deeplake-3.3.1/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.3.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.3.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.3.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.3.1/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.3.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/encode/tile.py` & `deeplake-3.3.1/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/meta/tensor_meta.py` & `deeplake-3.3.1/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/partial_reader.py` & `deeplake-3.3.1/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/partial_sample.py` & `deeplake-3.3.1/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/polygon.py` & `deeplake-3.3.1/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/query/autocomplete.py` & `deeplake-3.3.1/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/query/filter.py` & `deeplake-3.3.1/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/query/query.py` & `deeplake-3.3.1/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/sample.py` & `deeplake-3.3.1/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/serialize.py` & `deeplake-3.3.1/deeplake/core/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,20 +435,14 @@
 
 def check_sample_shape(shape, num_dims):
     if shape is not None and len(shape) != num_dims:
         raise TensorInvalidSampleShapeError(shape, num_dims)
 
 
 def text_to_bytes(sample, dtype, htype):
-    if isinstance(sample, deeplake.core.tensor.Tensor):
-        try:
-            if sample.htype == htype or sample.htype == "json" and htype == "list":
-                return sample.tobytes(), sample.shape
-        except (ValueError, NotImplementedError):  # sliced sample or tiled sample
-            sample = sample.data()
     if htype in ("json", "list"):
         if isinstance(sample, np.ndarray):
             if htype == "list":
                 sample = list(sample) if sample.dtype == object else sample.tolist()
             elif htype == "json":
                 if sample.ndim == 0 or sample.dtype != object:
                     sample = sample.tolist()  # actually returns dict
@@ -489,23 +483,23 @@
     incoming_sample: SampleValue,
     sample_compression: Optional[str],
     dtype: str,
     htype: str,
 ):
     """Converts the sample into bytes"""
     if isinstance(incoming_sample, deeplake.core.tensor.Tensor):
-        return serialize_tensor(
-            incoming_sample=incoming_sample,
-            sample_compression=sample_compression,
-            chunk_compression=None,
-            dtype=dtype,
-            htype=htype,
-            min_chunk_size=0,
-            break_into_tiles=False,
-        )
+        try:
+            if (
+                incoming_sample.htype == htype
+                or incoming_sample.htype == "json"
+                and htype == "list"
+            ):
+                return incoming_sample.tobytes(), incoming_sample.shape
+        except (ValueError, NotImplementedError):  # sliced sample or tiled sample
+            incoming_sample = incoming_sample.data()["value"]
     incoming_sample, shape = text_to_bytes(incoming_sample, dtype, htype)
     if sample_compression:
         incoming_sample = compress_bytes(incoming_sample, sample_compression)  # type: ignore
     return incoming_sample, shape
 
 
 def serialize_polygons(
```

### Comparing `deeplake-3.3.0/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.3.1/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/storage/gcs.py` & `deeplake-3.3.1/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/storage/google_drive.py` & `deeplake-3.3.1/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/storage/local.py` & `deeplake-3.3.1/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/storage/lru_cache.py` & `deeplake-3.3.1/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/storage/memory.py` & `deeplake-3.3.1/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/storage/provider.py` & `deeplake-3.3.1/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/storage/s3.py` & `deeplake-3.3.1/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tensor.py` & `deeplake-3.3.1/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tensor_link.py` & `deeplake-3.3.1/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/test_serialize.py` & `deeplake-3.3.1/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tests/test_compression.py` & `deeplake-3.3.1/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tests/test_compute.py` & `deeplake-3.3.1/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.3.1/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tests/test_io.py` & `deeplake-3.3.1/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tests/test_locking.py` & `deeplake-3.3.1/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tests/test_readonly.py` & `deeplake-3.3.1/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tests/test_serialize.py` & `deeplake-3.3.1/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tiling/deserialize.py` & `deeplake-3.3.1/deeplake/core/tiling/deserialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,16 +89,21 @@
                 s += sample_shape[i]
             ts = s // tile_shape[i]
             tiles_index.append(slice(ts, ts + 1))
             sample_index.append(s % tile_shape[i])
         elif isinstance(s, list):
             s = [x + sample_shape[i] if x < 0 else x for x in s]
             mn, mx = min(s), max(s)
+            if s != list(range(mn, mx + 1)):
+                raise NotImplementedError(
+                    "Non-contiguous indexing for tiled samples is not supported yet."
+                )
             tiles_index.append(slice(mn // tile_shape[i], mx // tile_shape[i] + 1))
-            sample_index.append([x - mn for x in s])
+            offset = mn - (mn % tile_shape[i])
+            sample_index.append([x - offset for x in s])
         elif isinstance(s, slice):
             start, stop, step = s.start, s.stop, s.step
             if start is None:
                 start = 0
             elif start < 0:
                 start += sample_shape[i]
             if stop is None:
```

### Comparing `deeplake-3.3.0/deeplake/core/tiling/optimizer.py` & `deeplake-3.3.1/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.3.1/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tiling/serialize.py` & `deeplake-3.3.1/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.3.1/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/tiling/test_serialize.py` & `deeplake-3.3.1/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/transform/test_transform.py` & `deeplake-3.3.1/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/transform/transform.py` & `deeplake-3.3.1/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/transform/transform_dataset.py` & `deeplake-3.3.1/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/transform/transform_tensor.py` & `deeplake-3.3.1/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.3.1/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/version_control/commit_diff.py` & `deeplake-3.3.1/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/version_control/commit_node.py` & `deeplake-3.3.1/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.3.1/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/version_control/test_merge.py` & `deeplake-3.3.1/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/core/version_control/test_version_control.py` & `deeplake-3.3.1/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.3.1/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/enterprise/dataloader.py` & `deeplake-3.3.1/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.3.1/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.3.1/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/enterprise/test_pytorch.py` & `deeplake-3.3.1/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/enterprise/test_query.py` & `deeplake-3.3.1/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.3.1/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/enterprise/util.py` & `deeplake-3.3.1/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/hooks.py` & `deeplake-3.3.1/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/htype.py` & `deeplake-3.3.1/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.3.1/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.3.1/deeplake/integrations/mmdet/mmdet_.py`

 * *Files 1% similar despite different names*

```diff
@@ -935,14 +935,15 @@
             poly2mask = True
 
     bbox_info = dataset[boxes_tensor].info
     classes = dataset[labels_tensor].info.class_names
     dataset.CLASSES = classes
     pipeline = build_pipeline(pipeline)
     metrics_format = train_loader_config.get("metrics_format")
+    persistent_workers = train_loader_config.get("persistent_workers", False)
     dist = train_loader_config["dist"]
     if dist and implementation == "python":
         raise NotImplementedError(
             "Distributed training is not supported by the python data loader. Set deeplake_dataloader_type='c++' to use the C++ dtaloader instead."
         )
     transform_fn = partial(
         transform,
@@ -975,14 +976,20 @@
         batch_size = train_loader_config["samples_per_gpu"]
 
     collate_fn = partial(collate, samples_per_gpu=batch_size)
 
     decode_method = {images_tensor: "numpy"}
 
     if implementation == "python":
+        if persistent_workers:
+            always_warn(
+                "Persistent workers are not supported for OSS dataloader. "
+                "persistent_workers=False will be used instead."
+            )
+
         loader = dataset.pytorch(
             tensors_dict=tensors_dict,
             num_workers=num_workers,
             shuffle=shuffle,
             transform=transform_fn,
             tensors=tensors,
             collate_fn=collate_fn,
@@ -1021,14 +1028,15 @@
             .batch(batch_size)
             .pytorch(
                 num_workers=num_workers,
                 collate_fn=collate_fn,
                 tensors=tensors,
                 distributed=dist,
                 decode_method=decode_method,
+                persistent_workers=persistent_workers,
             )
         )
 
         mmdet_ds = MMDetDataset(
             dataset=dataset,
             metrics_format=metrics_format,
             pipeline=pipeline,
@@ -1259,15 +1267,14 @@
         samples_per_gpu=batch_size,
         workers_per_gpu=num_workers,
         # `num_gpus` will be ignored if distributed
         num_gpus=len(cfg.gpu_ids),
         dist=distributed,
         seed=cfg.seed,
         runner_type=runner_type,
-        persistent_workers=False,
         metrics_format=metrics_format,
     )
 
     train_loader_cfg = {
         **train_dataloader_default_args,
         **cfg.data.get("train_dataloader", {}),
         **cfg.data.train.get("deeplake_dataloader", {}),
@@ -1360,25 +1367,28 @@
     # register eval hooks
     if validate:
         val_dataloader_default_args = dict(
             samples_per_gpu=batch_size,
             workers_per_gpu=num_workers,
             dist=distributed,
             shuffle=False,
-            persistent_workers=False,
             mode="val",
             metrics_format=metrics_format,
             num_gpus=len(cfg.gpu_ids),
         )
 
         val_dataloader_args = {
             **cfg.data.val.get("deeplake_dataloader", {}),
             **val_dataloader_default_args,
         }
 
+        train_persistent_workers = train_loader_cfg.get("persistent_workers", False)
+        val_persistent_workers = val_dataloader_args.get("persistent_workers", False)
+        check_persistent_workers(train_persistent_workers, val_persistent_workers)
+
         if val_dataloader_args.get("shuffle", False):
             always_warn("shuffle argument for validation dataset will be ignored.")
 
         if ds_val is None:
             cfg_ds_val = cfg.data.get("val")
             if cfg_ds_val is None:
                 raise Exception(
@@ -1456,14 +1466,32 @@
     if cfg.resume_from:
         runner.resume(cfg.resume_from)
     elif cfg.load_from:
         runner.load_checkpoint(cfg.load_from)
     runner.run([data_loader], cfg.workflow)
 
 
+def check_persistent_workers(train_persistent_workers, val_persistent_workers):
+    if train_persistent_workers != val_persistent_workers:
+        if train_persistent_workers:
+            always_warn(
+                "persistent workers for training and evaluation should be identical, "
+                "otherwise, this could lead to performance issues. "
+                "Either both of then should be `True` or both of them should `False`. "
+                "If you want to use persistent workers set True for validation"
+            )
+        else:
+            always_warn(
+                "persistent workers for training and evaluation should be identical, "
+                "otherwise, this could lead to performance issues. "
+                "Either both of then should be `True` or both of them should `False`. "
+                "If you want to use persistent workers set True for training"
+            )
+
+
 def ddp_setup(rank: int, world_size: int, port: int):
     """
     Args:
         rank: Unique identifier of each process
         world_size: Total number of processes
         port: Port number
     """
```

### Comparing `deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.3.1/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.3.1/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/integrations/pytorch/common.py` & `deeplake-3.3.1/deeplake/integrations/pytorch/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,22 @@
 
     if isinstance(elem, np.ndarray) and elem.size > 0 and isinstance(elem[0], str):
         batch = [it[0] for it in batch]
     elif isinstance(elem, (tuple, list)) and len(elem) > 0 and isinstance(elem[0], str):
         batch = [it[0] for it in batch]
     elif isinstance(elem, Polygons):
         batch = [it.numpy() for it in batch]
-    elif isinstance(elem, (tuple, list)):
-        elem_type = type(elem)
-        return [elem_type([torch.tensor(item) for item in sample]) for sample in batch]
+    elif isinstance(elem, list) and all(
+        map(lambda e: isinstance(e, np.ndarray), elem)
+    ):  # special case for video query api
+        if elem[0].shape[1] not in [2, 3]:  # checking whether it is not a polygon
+            elem_type = type(elem)
+            return [
+                elem_type([torch.tensor(item) for item in sample]) for sample in batch
+            ]
     return default_collate(batch)
 
 
 def convert_fn(data):
     from torch.utils.data._utils.collate import default_convert
 
     if isinstance(data, IterableOrderedDict):
```

### Comparing `deeplake-3.3.0/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.3.1/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.3.1/deeplake/integrations/pytorch/pytorch.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     batch_size,
     collate_fn,
     pin_memory,
     drop_last,
     return_index,
     pad_tensors,
     decode_method,
+    persistent_workers,
 ):
     import torch
     import torch.utils.data
     from deeplake.integrations.pytorch.dataset import SubIterableDataset
 
     return torch.utils.data.DataLoader(
         # this data set is more efficient also shuffles
@@ -42,14 +43,15 @@
             pad_tensors=pad_tensors,
             decode_method=decode_method,
         ),
         batch_size=batch_size,
         collate_fn=collate_fn,
         pin_memory=pin_memory,
         drop_last=drop_last,
+        persistent_workers=persistent_workers,
     )
 
 
 def dataset_to_pytorch(
     dataset,
     num_workers: int,
     batch_size: int,
@@ -61,14 +63,15 @@
     buffer_size: int,
     use_local_cache: bool,
     transform: Optional[Union[Dict, Callable]] = None,
     tensors: Optional[Sequence[str]] = None,
     return_index: bool = True,
     pad_tensors: bool = True,
     decode_method: Optional[Dict[str, str]] = None,
+    persistent_workers: bool = False,
     **kwargs,
 ):
     import torch
     from deeplake.integrations.pytorch.dataset import TorchDataset
 
     try_flushing(dataset)
 
@@ -108,14 +111,15 @@
             batch_size,
             collate_fn,
             pin_memory,
             drop_last,
             return_index,
             pad_tensors,
             decode_method,
+            persistent_workers,
         )
     else:
         return torch.utils.data.DataLoader(
             TorchDataset(
                 dataset,
                 tensors=tensors,
                 use_local_cache=use_local_cache,
@@ -129,8 +133,9 @@
                 batch_size=batch_size,
             ),
             batch_size=batch_size,
             collate_fn=collate_fn,
             pin_memory=pin_memory,
             num_workers=num_workers,
             drop_last=drop_last,
+            persistent_workers=persistent_workers,
         )
```

### Comparing `deeplake-3.3.0/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.3.1/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/integrations/tf/common.py` & `deeplake-3.3.1/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.3.1/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.3.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/integrations/wandb/wandb.py` & `deeplake-3.3.1/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/tests/cache_fixtures.py` & `deeplake-3.3.1/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/tests/client_fixtures.py` & `deeplake-3.3.1/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/tests/common.py` & `deeplake-3.3.1/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/tests/dataset_fixtures.py` & `deeplake-3.3.1/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/tests/path_fixtures.py` & `deeplake-3.3.1/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/tests/storage_fixtures.py` & `deeplake-3.3.1/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/access_method.py` & `deeplake-3.3.1/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/agreement.py` & `deeplake-3.3.1/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/array_list.py` & `deeplake-3.3.1/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/assert_byte_indexes.py` & `deeplake-3.3.1/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/auto.py` & `deeplake-3.3.1/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/bugout_reporter.py` & `deeplake-3.3.1/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/cache_chain.py` & `deeplake-3.3.1/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/casting.py` & `deeplake-3.3.1/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/check_latest_version.py` & `deeplake-3.3.1/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/chunk_engine.py` & `deeplake-3.3.1/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/class_label.py` & `deeplake-3.3.1/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/compute.py` & `deeplake-3.3.1/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/connect_dataset.py` & `deeplake-3.3.1/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/dataset.py` & `deeplake-3.3.1/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/diff.py` & `deeplake-3.3.1/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/downsample.py` & `deeplake-3.3.1/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/encoder.py` & `deeplake-3.3.1/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/exceptions.py` & `deeplake-3.3.1/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/exif.py` & `deeplake-3.3.1/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/from_tfds.py` & `deeplake-3.3.1/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/htype.py` & `deeplake-3.3.1/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/image.py` & `deeplake-3.3.1/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/invalid_view_op.py` & `deeplake-3.3.1/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/iteration_warning.py` & `deeplake-3.3.1/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/json.py` & `deeplake-3.3.1/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/keys.py` & `deeplake-3.3.1/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/link.py` & `deeplake-3.3.1/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/logging.py` & `deeplake-3.3.1/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/merge.py` & `deeplake-3.3.1/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/modified.py` & `deeplake-3.3.1/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/notebook.py` & `deeplake-3.3.1/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/object_3d/mesh.py` & `deeplake-3.3.1/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.3.1/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.3.1/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.3.1/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.3.1/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.3.1/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.3.1/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.3.1/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.3.1/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.3.1/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/path.py` & `deeplake-3.3.1/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/pretty_print.py` & `deeplake-3.3.1/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/remove_cache.py` & `deeplake-3.3.1/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/scheduling.py` & `deeplake-3.3.1/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/shape_interval.py` & `deeplake-3.3.1/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/spinner.py` & `deeplake-3.3.1/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/split.py` & `deeplake-3.3.1/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/storage.py` & `deeplake-3.3.1/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/tag.py` & `deeplake-3.3.1/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/testing.py` & `deeplake-3.3.1/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/tests/test_auto.py` & `deeplake-3.3.1/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.3.1/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.3.1/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/tests/test_read.py` & `deeplake-3.3.1/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.3.1/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/tests/test_split.py` & `deeplake-3.3.1/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/tests/test_version_control.py` & `deeplake-3.3.1/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/transform.py` & `deeplake-3.3.1/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/version_control.py` & `deeplake-3.3.1/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/util/video.py` & `deeplake-3.3.1/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/visualizer/video_streaming.py` & `deeplake-3.3.1/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake/visualizer/visualizer.py` & `deeplake-3.3.1/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake.egg-info/PKG-INFO` & `deeplake-3.3.1/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.3.0
+Version: 3.3.1
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.3.0 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.3.1 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
 Provides-Extra: gcp Provides-Extra: gdrive Provides-Extra: medical Provides-
```

### Comparing `deeplake-3.3.0/deeplake.egg-info/SOURCES.txt` & `deeplake-3.3.1/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/deeplake.egg-info/requires.txt` & `deeplake-3.3.1/deeplake.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.0/setup.py` & `deeplake-3.3.1/setup.py`

 * *Files identical despite different names*


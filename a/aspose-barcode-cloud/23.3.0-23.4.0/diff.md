# Comparing `tmp/aspose-barcode-cloud-23.3.0.tar.gz` & `tmp/aspose-barcode-cloud-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aspose-barcode-cloud-23.3.0.tar", last modified: Mon Mar 27 13:50:36 2023, max compression
+gzip compressed data, was "dist/aspose-barcode-cloud-23.4.0.tar", last modified: Thu Apr 27 16:36:19 2023, max compression
```

## Comparing `aspose-barcode-cloud-23.3.0.tar` & `aspose-barcode-cloud-23.4.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/
--rw-r--r--   0 root         (0) root         (0)    16501 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12053 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/
--rw-r--r--   0 root         (0) root         (0)     6716 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api/
--rw-r--r--   0 root         (0) root         (0)      319 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99111 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api/barcode_api.py
--rw-r--r--   0 root         (0) root         (0)    24296 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api/file_api.py
--rw-r--r--   0 root         (0) root         (0)    22451 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api/folder_api.py
--rw-r--r--   0 root         (0) root         (0)    16119 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api/storage_api.py
--rw-r--r--   0 root         (0) root         (0)    26047 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api_client.py
--rw-r--r--   0 root         (0) root         (0)    10460 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/
--rw-r--r--   0 root         (0) root         (0)     6260 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6521 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/api_error.py
--rw-r--r--   0 root         (0) root         (0)     4574 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/api_error_response.py
--rw-r--r--   0 root         (0) root         (0)     5429 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/australian_post_params.py
--rw-r--r--   0 root         (0) root         (0)     3371 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/auto_size_mode.py
--rw-r--r--   0 root         (0) root         (0)     3417 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/available_graphics_unit.py
--rw-r--r--   0 root         (0) root         (0)     6810 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/aztec_params.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/aztec_symbol_mode.py
--rw-r--r--   0 root         (0) root         (0)     6225 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/barcode_response.py
--rw-r--r--   0 root         (0) root         (0)     4135 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/barcode_response_list.py
--rw-r--r--   0 root         (0) root         (0)     3413 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/border_dash_style.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/caption_params.py
--rw-r--r--   0 root         (0) root         (0)     3371 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/checksum_validation.py
--rw-r--r--   0 root         (0) root         (0)     3361 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/codabar_checksum_mode.py
--rw-r--r--   0 root         (0) root         (0)     6349 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/codabar_params.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/codabar_symbol.py
--rw-r--r--   0 root         (0) root         (0)     5474 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/codablock_params.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/code128_emulation.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/code16_k_params.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/code_location.py
--rw-r--r--   0 root         (0) root         (0)     4238 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/coupon_params.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py
--rw-r--r--   0 root         (0) root         (0)     8008 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/data_bar_params.py
--rw-r--r--   0 root         (0) root         (0)     3469 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py
--rw-r--r--   0 root         (0) root         (0)     3527 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)    10136 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/data_matrix_params.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/decode_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/disc_usage.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/dot_code_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     9394 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/dot_code_params.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/eci_encodings.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/enable_checksum.py
--rw-r--r--   0 root         (0) root         (0)     5359 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/encode_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)     5970 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/error.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)     8827 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/file_version.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/file_versions.py
--rw-r--r--   0 root         (0) root         (0)     3995 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/files_list.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/files_upload_result.py
--rw-r--r--   0 root         (0) root         (0)     3317 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/font_mode.py
--rw-r--r--   0 root         (0) root         (0)     5207 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/font_params.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/font_style.py
--rw-r--r--   0 root         (0) root         (0)    54639 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/generator_params.py
--rw-r--r--   0 root         (0) root         (0)     5896 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/generator_params_list.py
--rw-r--r--   0 root         (0) root         (0)     3407 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/itf14_border_type.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/itf_params.py
--rw-r--r--   0 root         (0) root         (0)     3367 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/macro_character.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/maxi_code_mode.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/maxi_code_params.py
--rw-r--r--   0 root         (0) root         (0)     4944 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/object_exist.py
--rw-r--r--   0 root         (0) root         (0)     5750 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/padding.py
--rw-r--r--   0 root         (0) root         (0)     5467 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/patch_code_params.py
--rw-r--r--   0 root         (0) root         (0)     3441 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/patch_format.py
--rw-r--r--   0 root         (0) root         (0)     3407 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/pdf417_error_level.py
--rw-r--r--   0 root         (0) root         (0)     3381 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py
--rw-r--r--   0 root         (0) root         (0)    24492 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/pdf417_params.py
--rw-r--r--   0 root         (0) root         (0)     4177 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/postal_params.py
--rw-r--r--   0 root         (0) root         (0)     3523 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/preset_type.py
--rw-r--r--   0 root         (0) root         (0)     3459 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/qr_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3369 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/qr_encode_type.py
--rw-r--r--   0 root         (0) root         (0)     3381 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/qr_error_level.py
--rw-r--r--   0 root         (0) root         (0)    11027 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/qr_params.py
--rw-r--r--   0 root         (0) root         (0)     4531 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/qr_version.py
--rw-r--r--   0 root         (0) root         (0)    46250 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/reader_params.py
--rw-r--r--   0 root         (0) root         (0)     4540 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/region_point.py
--rw-r--r--   0 root         (0) root         (0)     5716 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/result_image_info.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/storage_exist.py
--rw-r--r--   0 root         (0) root         (0)     7017 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/storage_file.py
--rw-r--r--   0 root         (0) root         (0)     6065 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/structured_append.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/text_alignment.py
--rw-r--r--   0 root         (0) root         (0)    14400 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16501 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3966 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/aspose_barcode_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 13:50:36.000000 aspose-barcode-cloud-23.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5740 2023-03-27 13:49:14.000000 aspose-barcode-cloud-23.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/
+-rw-r--r--   0 root         (0) root         (0)    16507 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12059 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/
+-rw-r--r--   0 root         (0) root         (0)     6716 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99385 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/barcode_api.py
+-rw-r--r--   0 root         (0) root         (0)    24296 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/file_api.py
+-rw-r--r--   0 root         (0) root         (0)    22451 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/folder_api.py
+-rw-r--r--   0 root         (0) root         (0)    16119 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/storage_api.py
+-rw-r--r--   0 root         (0) root         (0)    26047 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    10460 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/
+-rw-r--r--   0 root         (0) root         (0)     6260 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/api_error.py
+-rw-r--r--   0 root         (0) root         (0)     4574 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/api_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     5429 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/australian_post_params.py
+-rw-r--r--   0 root         (0) root         (0)     3371 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/auto_size_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/available_graphics_unit.py
+-rw-r--r--   0 root         (0) root         (0)     6810 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/aztec_params.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/aztec_symbol_mode.py
+-rw-r--r--   0 root         (0) root         (0)     6225 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/barcode_response.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/barcode_response_list.py
+-rw-r--r--   0 root         (0) root         (0)     3413 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/border_dash_style.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/caption_params.py
+-rw-r--r--   0 root         (0) root         (0)     3371 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/checksum_validation.py
+-rw-r--r--   0 root         (0) root         (0)     3361 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_checksum_mode.py
+-rw-r--r--   0 root         (0) root         (0)     6349 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_params.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_symbol.py
+-rw-r--r--   0 root         (0) root         (0)     5474 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codablock_params.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code128_emulation.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code16_k_params.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     4238 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/coupon_params.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_bar_params.py
+-rw-r--r--   0 root         (0) root         (0)     3469 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py
+-rw-r--r--   0 root         (0) root         (0)     3527 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)    10136 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_params.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/decode_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/disc_usage.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/dot_code_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     9394 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/dot_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/eci_encodings.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/enable_checksum.py
+-rw-r--r--   0 root         (0) root         (0)     5359 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/encode_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)     5970 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)     8827 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/file_version.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/file_versions.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/files_list.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/files_upload_result.py
+-rw-r--r--   0 root         (0) root         (0)     3317 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_params.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_style.py
+-rw-r--r--   0 root         (0) root         (0)    55723 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/generator_params.py
+-rw-r--r--   0 root         (0) root         (0)     5896 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/generator_params_list.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/itf14_border_type.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/itf_params.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/macro_character.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/object_exist.py
+-rw-r--r--   0 root         (0) root         (0)     5750 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/padding.py
+-rw-r--r--   0 root         (0) root         (0)     5467 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/patch_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/patch_format.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_error_level.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py
+-rw-r--r--   0 root         (0) root         (0)    24492 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_params.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/postal_params.py
+-rw-r--r--   0 root         (0) root         (0)     3523 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/preset_type.py
+-rw-r--r--   0 root         (0) root         (0)     3459 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3369 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_encode_type.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_error_level.py
+-rw-r--r--   0 root         (0) root         (0)    11027 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_params.py
+-rw-r--r--   0 root         (0) root         (0)     4531 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_version.py
+-rw-r--r--   0 root         (0) root         (0)    46322 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/reader_params.py
+-rw-r--r--   0 root         (0) root         (0)     4540 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/region_point.py
+-rw-r--r--   0 root         (0) root         (0)     5716 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/result_image_info.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/storage_exist.py
+-rw-r--r--   0 root         (0) root         (0)     7017 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/storage_file.py
+-rw-r--r--   0 root         (0) root         (0)     6065 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/structured_append.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/text_alignment.py
+-rw-r--r--   0 root         (0) root         (0)    14400 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16507 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3966 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5750 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/setup.py
```

### Comparing `aspose-barcode-cloud-23.3.0/PKG-INFO` & `aspose-barcode-cloud-23.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-barcode-cloud
-Version: 23.3.0
+Version: 23.4.0
 Summary: Aspose.Barcode Cloud API Reference
 Home-page: https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Author: Aspose Barcode Cloud
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Project-URL: Website, https://www.aspose.cloud
 Project-URL: Product Home, https://products.aspose.cloud/barcode/
@@ -15,15 +15,15 @@
 Description: # Aspose.BarCode Cloud SDK for Python
         
         [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
         [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
         [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
         
         - API version: 3.0
-        - Package version: 23.3.0
+        - Package version: 23.4.0
         
         ## Demo applications
         
         [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
         :---: | :---: | :---:
         [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
         [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -102,15 +102,15 @@
                                                                   preset=aspose_barcode_cloud.PresetType.HIGHPERFORMANCE)
         pprint(response)
         ```
         
         ## Requirements
         
         - six >= 1.10
-        - urllib3 >= 1.15.1
+        - urllib3 >= 1.21.1, <2.0
         
         ## Licensing
         
         All Aspose.BarCode for Cloud SDKs, helper scripts and templates are licensed under [MIT License](LICENSE).
         
         ## Resources
```

### Comparing `aspose-barcode-cloud-23.3.0/README.md` & `aspose-barcode-cloud-23.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
 [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 23.3.0
+- Package version: 23.4.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -88,15 +88,15 @@
                                                           preset=aspose_barcode_cloud.PresetType.HIGHPERFORMANCE)
 pprint(response)
 ```
 
 ## Requirements
 
 - six >= 1.10
-- urllib3 >= 1.15.1
+- urllib3 >= 1.21.1, <2.0
 
 ## Licensing
 
 All Aspose.BarCode for Cloud SDKs, helper scripts and templates are licensed under [MIT License](LICENSE).
 
 ## Resources
```

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/__init__.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api/barcode_api.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/barcode_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         filled_bars=None,
         always_show_checksum=None,
         wide_narrow_ratio=None,
         validate_text=None,
         supplement_data=None,
         supplement_space=None,
         bar_width_reduction=None,
+        use_anti_alias=None,
         format=None,
         async_req=False,
         **kwargs
     ):
         """Generate barcode.
 
         This method makes a synchronous HTTP request by default. To make an
@@ -123,14 +124,15 @@
         :param bool filled_bars: Value indicating whether bars are filled. Only for 1D barcodes. Default value: true. # noqa: E501
         :param bool always_show_checksum: Always display checksum digit in the human readable text for Code128 and GS1Code128 barcodes. # noqa: E501
         :param float wide_narrow_ratio: Wide bars to Narrow bars ratio. Default value: 3, that is, wide bars are 3 times as wide as narrow bars. Used for ITF, PZN, PharmaCode, Standard2of5, Interleaved2of5, Matrix2of5, ItalianPost25, IATA2of5, VIN, DeutschePost, OPC, Code32, DataLogic2of5, PatchCode, Code39Extended, Code39Standard # noqa: E501
         :param bool validate_text: Only for 1D barcodes. If codetext is incorrect and value set to true - exception will be thrown. Otherwise codetext will be corrected to match barcode's specification. Exception always will be thrown for: Databar symbology if codetext is incorrect. Exception always will not be thrown for: AustraliaPost, SingaporePost, Code39Extended, Code93Extended, Code16K, Code128 symbology if codetext is incorrect. # noqa: E501
         :param str supplement_data: Supplement parameters. Used for Interleaved2of5, Standard2of5, EAN13, EAN8, UPCA, UPCE, ISBN, ISSN, ISMN. # noqa: E501
         :param float supplement_space: Space between main the BarCode and supplement BarCode. # noqa: E501
         :param float bar_width_reduction: Bars reduction value that is used to compensate ink spread while printing. # noqa: E501
+        :param bool use_anti_alias: Indicates whether is used anti-aliasing mode to render image. Anti-aliasing mode is applied to barcode and text drawing. # noqa: E501
         :param str format: Result image format. # noqa: E501
         :param async_req bool
         :return: file
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs["_return_http_data_only"] = True
@@ -166,14 +168,15 @@
                 filled_bars=filled_bars,
                 always_show_checksum=always_show_checksum,
                 wide_narrow_ratio=wide_narrow_ratio,
                 validate_text=validate_text,
                 supplement_data=supplement_data,
                 supplement_space=supplement_space,
                 bar_width_reduction=bar_width_reduction,
+                use_anti_alias=use_anti_alias,
                 format=format,
                 **kwargs
             )
         else:
             (data) = self.get_barcode_generate_with_http_info(
                 type,
                 text,
@@ -205,14 +208,15 @@
                 filled_bars=filled_bars,
                 always_show_checksum=always_show_checksum,
                 wide_narrow_ratio=wide_narrow_ratio,
                 validate_text=validate_text,
                 supplement_data=supplement_data,
                 supplement_space=supplement_space,
                 bar_width_reduction=bar_width_reduction,
+                use_anti_alias=use_anti_alias,
                 format=format,
                 **kwargs
             )
             return data
 
     def get_barcode_generate_with_http_info(self, type, text, **kwargs):
         """Generate barcode.
@@ -260,14 +264,15 @@
             "filled_bars",
             "always_show_checksum",
             "wide_narrow_ratio",
             "validate_text",
             "supplement_data",
             "supplement_space",
             "bar_width_reduction",
+            "use_anti_alias",
             "format",
         }
         all_params.add("async_req")
         all_params.add("_return_http_data_only")
         all_params.add("_preload_content")
         all_params.add("_request_timeout")
 
@@ -356,14 +361,16 @@
             query_params.append(("ValidateText", params["validate_text"]))
         if "supplement_data" in params:
             query_params.append(("SupplementData", params["supplement_data"]))
         if "supplement_space" in params:
             query_params.append(("SupplementSpace", params["supplement_space"]))
         if "bar_width_reduction" in params:
             query_params.append(("BarWidthReduction", params["bar_width_reduction"]))
+        if "use_anti_alias" in params:
+            query_params.append(("UseAntiAlias", params["use_anti_alias"]))
         if "format" in params:
             query_params.append(("format", params["format"]))
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -431,15 +438,14 @@
         region_likelihood_threshold_percent=None,
         scan_window_sizes=None,
         similarity=None,
         skip_diagonal_search=None,
         read_tiny_barcodes=None,
         australian_post_encoding_table=None,
         ignore_ending_filling_patterns_for_c_table=None,
-        rectangle_region=None,
         storage=None,
         folder=None,
         async_req=False,
         **kwargs
     ):
         """Recognize barcode from a file on server.
 
@@ -449,16 +455,16 @@
         >>> result = thread.get()
 
         :param str name: The image file name. # noqa: E501
         :param str type: The type of barcode to read. # noqa: E501
         :param str checksum_validation: Enable checksum validation during recognition for 1D barcodes. Default is treated as Yes for symbologies which must contain checksum, as No where checksum only possible. Checksum never used: Codabar Checksum is possible: Code39 Standard/Extended, Standard2of5, Interleaved2of5, Matrix2of5, ItalianPost25, DeutschePostIdentcode, DeutschePostLeitcode, VIN Checksum always used: Rest symbologies # noqa: E501
         :param bool detect_encoding: A flag which force engine to detect codetext encoding for Unicode. # noqa: E501
         :param str preset: Preset allows to configure recognition quality and speed manually. You can quickly set up Preset by embedded presets: HighPerformance, NormalQuality, HighQuality, MaxBarCodes or you can manually configure separate options. Default value of Preset is NormalQuality. # noqa: E501
-        :param int rect_x: Set X for area for recognition. # noqa: E501
-        :param int rect_y: Set Y for area for recognition. # noqa: E501
+        :param int rect_x: Set X of top left corner of area for recognition. # noqa: E501
+        :param int rect_y: Set Y of top left corner of area for recognition. # noqa: E501
         :param int rect_width: Set Width of area for recognition. # noqa: E501
         :param int rect_height: Set Height of area for recognition. # noqa: E501
         :param bool strip_fnc: Value indicating whether FNC symbol strip must be done. # noqa: E501
         :param int timeout: Timeout of recognition process in milliseconds. Default value is 15_000 (15 seconds). Maximum value is 60_000 (1 minute). In case of a timeout RequestTimeout (408) status will be returned. Try reducing the image size to avoid timeout. # noqa: E501
         :param int median_smoothing_window_size: Window size for median smoothing. Typical values are 3 or 4. Default value is 3. AllowMedianSmoothing must be set. # noqa: E501
         :param bool allow_median_smoothing: Allows engine to enable median smoothing as additional scan. Mode helps to recognize noised barcodes. # noqa: E501
         :param bool allow_complex_background: Allows engine to recognize color barcodes on color background as additional scan. Extremely slow mode. # noqa: E501
@@ -479,15 +485,14 @@
         :param float region_likelihood_threshold_percent: Sets threshold for detected regions that may contain barcodes. Value 0.7 means that bottom 70% of possible regions are filtered out and not processed further. Region likelihood threshold must be between [0.05, 0.9] Use high values for clear images with few barcodes. Use low values for images with many barcodes or for noisy images. Low value may lead to a bigger recognition time. # noqa: E501
         :param list[int] scan_window_sizes: Scan window sizes in pixels. Allowed sizes are 10, 15, 20, 25, 30. Scanning with small window size takes more time and provides more accuracy but may fail in detecting very big barcodes. Combining of several window sizes can improve detection quality. # noqa: E501
         :param float similarity: Similarity coefficient depends on how homogeneous barcodes are. Use high value for for clear barcodes. Use low values to detect barcodes that ara partly damaged or not lighten evenly. Similarity coefficient must be between [0.5, 0.9] # noqa: E501
         :param bool skip_diagonal_search: Allows detector to skip search for diagonal barcodes. Setting it to false will increase detection time but allow to find diagonal barcodes that can be missed otherwise. Enabling of diagonal search leads to a bigger detection time. # noqa: E501
         :param bool read_tiny_barcodes: Allows engine to recognize tiny barcodes on large images. Ignored if AllowIncorrectBarcodes is set to True. Default value: False. # noqa: E501
         :param str australian_post_encoding_table: Interpreting Type for the Customer Information of AustralianPost BarCode.Default is CustomerInformationInterpretingType.Other. # noqa: E501
         :param bool ignore_ending_filling_patterns_for_c_table: The flag which force AustraliaPost decoder to ignore last filling patterns in Customer Information Field during decoding as CTable method. CTable encoding method does not have any gaps in encoding table and sequence \"333\" of filling patterns is decoded as letter \"z\". # noqa: E501
-        :param str rectangle_region: # noqa: E501
         :param str storage: The image storage. # noqa: E501
         :param str folder: The image folder. # noqa: E501
         :param async_req bool
         :return: BarcodeResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -525,15 +530,14 @@
                 region_likelihood_threshold_percent=region_likelihood_threshold_percent,
                 scan_window_sizes=scan_window_sizes,
                 similarity=similarity,
                 skip_diagonal_search=skip_diagonal_search,
                 read_tiny_barcodes=read_tiny_barcodes,
                 australian_post_encoding_table=australian_post_encoding_table,
                 ignore_ending_filling_patterns_for_c_table=ignore_ending_filling_patterns_for_c_table,
-                rectangle_region=rectangle_region,
                 storage=storage,
                 folder=folder,
                 **kwargs
             )
         else:
             (data) = self.get_barcode_recognize_with_http_info(
                 name,
@@ -567,15 +571,14 @@
                 region_likelihood_threshold_percent=region_likelihood_threshold_percent,
                 scan_window_sizes=scan_window_sizes,
                 similarity=similarity,
                 skip_diagonal_search=skip_diagonal_search,
                 read_tiny_barcodes=read_tiny_barcodes,
                 australian_post_encoding_table=australian_post_encoding_table,
                 ignore_ending_filling_patterns_for_c_table=ignore_ending_filling_patterns_for_c_table,
-                rectangle_region=rectangle_region,
                 storage=storage,
                 folder=folder,
                 **kwargs
             )
             return data
 
     def get_barcode_recognize_with_http_info(self, name, **kwargs):
@@ -624,15 +627,14 @@
             "region_likelihood_threshold_percent",
             "scan_window_sizes",
             "similarity",
             "skip_diagonal_search",
             "read_tiny_barcodes",
             "australian_post_encoding_table",
             "ignore_ending_filling_patterns_for_c_table",
-            "rectangle_region",
             "storage",
             "folder",
         }
         all_params.add("async_req")
         all_params.add("_return_http_data_only")
         all_params.add("_preload_content")
         all_params.add("_request_timeout")
@@ -724,16 +726,14 @@
             query_params.append(("ReadTinyBarcodes", params["read_tiny_barcodes"]))
         if "australian_post_encoding_table" in params:
             query_params.append(("AustralianPostEncodingTable", params["australian_post_encoding_table"]))
         if "ignore_ending_filling_patterns_for_c_table" in params:
             query_params.append(
                 ("IgnoreEndingFillingPatternsForCTable", params["ignore_ending_filling_patterns_for_c_table"])
             )
-        if "rectangle_region" in params:
-            query_params.append(("RectangleRegion", params["rectangle_region"]))
         if "storage" in params:
             query_params.append(("storage", params["storage"]))
         if "folder" in params:
             query_params.append(("folder", params["folder"]))
 
         header_params = {}
 
@@ -800,15 +800,14 @@
         region_likelihood_threshold_percent=None,
         scan_window_sizes=None,
         similarity=None,
         skip_diagonal_search=None,
         read_tiny_barcodes=None,
         australian_post_encoding_table=None,
         ignore_ending_filling_patterns_for_c_table=None,
-        rectangle_region=None,
         url=None,
         image=None,
         async_req=False,
         **kwargs
     ):
         """Recognize barcode from an url or from request body. Request body can contain raw data bytes of the image with content-type \"application/octet-stream\". An image can also be passed as a form field.
 
@@ -817,16 +816,16 @@
         >>> thread = BarcodeApi().post_barcode_recognize_from_url_or_content(async_req=True)
         >>> result = thread.get()
 
         :param str type: The type of barcode to read. # noqa: E501
         :param str checksum_validation: Enable checksum validation during recognition for 1D barcodes. Default is treated as Yes for symbologies which must contain checksum, as No where checksum only possible. Checksum never used: Codabar Checksum is possible: Code39 Standard/Extended, Standard2of5, Interleaved2of5, Matrix2of5, ItalianPost25, DeutschePostIdentcode, DeutschePostLeitcode, VIN Checksum always used: Rest symbologies # noqa: E501
         :param bool detect_encoding: A flag which force engine to detect codetext encoding for Unicode. # noqa: E501
         :param str preset: Preset allows to configure recognition quality and speed manually. You can quickly set up Preset by embedded presets: HighPerformance, NormalQuality, HighQuality, MaxBarCodes or you can manually configure separate options. Default value of Preset is NormalQuality. # noqa: E501
-        :param int rect_x: Set X for area for recognition. # noqa: E501
-        :param int rect_y: Set Y for area for recognition. # noqa: E501
+        :param int rect_x: Set X of top left corner of area for recognition. # noqa: E501
+        :param int rect_y: Set Y of top left corner of area for recognition. # noqa: E501
         :param int rect_width: Set Width of area for recognition. # noqa: E501
         :param int rect_height: Set Height of area for recognition. # noqa: E501
         :param bool strip_fnc: Value indicating whether FNC symbol strip must be done. # noqa: E501
         :param int timeout: Timeout of recognition process in milliseconds. Default value is 15_000 (15 seconds). Maximum value is 60_000 (1 minute). In case of a timeout RequestTimeout (408) status will be returned. Try reducing the image size to avoid timeout. # noqa: E501
         :param int median_smoothing_window_size: Window size for median smoothing. Typical values are 3 or 4. Default value is 3. AllowMedianSmoothing must be set. # noqa: E501
         :param bool allow_median_smoothing: Allows engine to enable median smoothing as additional scan. Mode helps to recognize noised barcodes. # noqa: E501
         :param bool allow_complex_background: Allows engine to recognize color barcodes on color background as additional scan. Extremely slow mode. # noqa: E501
@@ -847,15 +846,14 @@
         :param float region_likelihood_threshold_percent: Sets threshold for detected regions that may contain barcodes. Value 0.7 means that bottom 70% of possible regions are filtered out and not processed further. Region likelihood threshold must be between [0.05, 0.9] Use high values for clear images with few barcodes. Use low values for images with many barcodes or for noisy images. Low value may lead to a bigger recognition time. # noqa: E501
         :param list[int] scan_window_sizes: Scan window sizes in pixels. Allowed sizes are 10, 15, 20, 25, 30. Scanning with small window size takes more time and provides more accuracy but may fail in detecting very big barcodes. Combining of several window sizes can improve detection quality. # noqa: E501
         :param float similarity: Similarity coefficient depends on how homogeneous barcodes are. Use high value for for clear barcodes. Use low values to detect barcodes that ara partly damaged or not lighten evenly. Similarity coefficient must be between [0.5, 0.9] # noqa: E501
         :param bool skip_diagonal_search: Allows detector to skip search for diagonal barcodes. Setting it to false will increase detection time but allow to find diagonal barcodes that can be missed otherwise. Enabling of diagonal search leads to a bigger detection time. # noqa: E501
         :param bool read_tiny_barcodes: Allows engine to recognize tiny barcodes on large images. Ignored if AllowIncorrectBarcodes is set to True. Default value: False. # noqa: E501
         :param str australian_post_encoding_table: Interpreting Type for the Customer Information of AustralianPost BarCode.Default is CustomerInformationInterpretingType.Other. # noqa: E501
         :param bool ignore_ending_filling_patterns_for_c_table: The flag which force AustraliaPost decoder to ignore last filling patterns in Customer Information Field during decoding as CTable method. CTable encoding method does not have any gaps in encoding table and sequence \"333\" of filling patterns is decoded as letter \"z\". # noqa: E501
-        :param str rectangle_region: # noqa: E501
         :param str url: The image file url. # noqa: E501
         :param file image: Image data # noqa: E501
         :param async_req bool
         :return: BarcodeResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -892,15 +890,14 @@
                 region_likelihood_threshold_percent=region_likelihood_threshold_percent,
                 scan_window_sizes=scan_window_sizes,
                 similarity=similarity,
                 skip_diagonal_search=skip_diagonal_search,
                 read_tiny_barcodes=read_tiny_barcodes,
                 australian_post_encoding_table=australian_post_encoding_table,
                 ignore_ending_filling_patterns_for_c_table=ignore_ending_filling_patterns_for_c_table,
-                rectangle_region=rectangle_region,
                 url=url,
                 image=image,
                 **kwargs
             )
         else:
             (data) = self.post_barcode_recognize_from_url_or_content_with_http_info(
                 type=type,
@@ -933,15 +930,14 @@
                 region_likelihood_threshold_percent=region_likelihood_threshold_percent,
                 scan_window_sizes=scan_window_sizes,
                 similarity=similarity,
                 skip_diagonal_search=skip_diagonal_search,
                 read_tiny_barcodes=read_tiny_barcodes,
                 australian_post_encoding_table=australian_post_encoding_table,
                 ignore_ending_filling_patterns_for_c_table=ignore_ending_filling_patterns_for_c_table,
-                rectangle_region=rectangle_region,
                 url=url,
                 image=image,
                 **kwargs
             )
             return data
 
     def post_barcode_recognize_from_url_or_content_with_http_info(self, **kwargs):
@@ -988,15 +984,14 @@
             "region_likelihood_threshold_percent",
             "scan_window_sizes",
             "similarity",
             "skip_diagonal_search",
             "read_tiny_barcodes",
             "australian_post_encoding_table",
             "ignore_ending_filling_patterns_for_c_table",
-            "rectangle_region",
             "url",
             "image",
         }
         all_params.add("async_req")
         all_params.add("_return_http_data_only")
         all_params.add("_preload_content")
         all_params.add("_request_timeout")
@@ -1086,16 +1081,14 @@
             query_params.append(("ReadTinyBarcodes", params["read_tiny_barcodes"]))
         if "australian_post_encoding_table" in params:
             query_params.append(("AustralianPostEncodingTable", params["australian_post_encoding_table"]))
         if "ignore_ending_filling_patterns_for_c_table" in params:
             query_params.append(
                 ("IgnoreEndingFillingPatternsForCTable", params["ignore_ending_filling_patterns_for_c_table"])
             )
-        if "rectangle_region" in params:
-            query_params.append(("RectangleRegion", params["rectangle_region"]))
         if "url" in params:
             query_params.append(("url", params["url"]))
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -1269,14 +1262,15 @@
         filled_bars=None,
         always_show_checksum=None,
         wide_narrow_ratio=None,
         validate_text=None,
         supplement_data=None,
         supplement_space=None,
         bar_width_reduction=None,
+        use_anti_alias=None,
         storage=None,
         folder=None,
         format=None,
         async_req=False,
         **kwargs
     ):
         """Generate barcode and save on server (from query params or from file with json or xml content)
@@ -1317,14 +1311,15 @@
         :param bool filled_bars: Value indicating whether bars are filled. Only for 1D barcodes. Default value: true. # noqa: E501
         :param bool always_show_checksum: Always display checksum digit in the human readable text for Code128 and GS1Code128 barcodes. # noqa: E501
         :param float wide_narrow_ratio: Wide bars to Narrow bars ratio. Default value: 3, that is, wide bars are 3 times as wide as narrow bars. Used for ITF, PZN, PharmaCode, Standard2of5, Interleaved2of5, Matrix2of5, ItalianPost25, IATA2of5, VIN, DeutschePost, OPC, Code32, DataLogic2of5, PatchCode, Code39Extended, Code39Standard # noqa: E501
         :param bool validate_text: Only for 1D barcodes. If codetext is incorrect and value set to true - exception will be thrown. Otherwise codetext will be corrected to match barcode's specification. Exception always will be thrown for: Databar symbology if codetext is incorrect. Exception always will not be thrown for: AustraliaPost, SingaporePost, Code39Extended, Code93Extended, Code16K, Code128 symbology if codetext is incorrect. # noqa: E501
         :param str supplement_data: Supplement parameters. Used for Interleaved2of5, Standard2of5, EAN13, EAN8, UPCA, UPCE, ISBN, ISSN, ISMN. # noqa: E501
         :param float supplement_space: Space between main the BarCode and supplement BarCode. # noqa: E501
         :param float bar_width_reduction: Bars reduction value that is used to compensate ink spread while printing. # noqa: E501
+        :param bool use_anti_alias: Indicates whether is used anti-aliasing mode to render image. Anti-aliasing mode is applied to barcode and text drawing. # noqa: E501
         :param str storage: Image's storage. # noqa: E501
         :param str folder: Image's folder. # noqa: E501
         :param str format: The image format. # noqa: E501
         :param async_req bool
         :return: ResultImageInfo
                  If the method is called asynchronously,
                  returns the request thread.
@@ -1363,14 +1358,15 @@
                 filled_bars=filled_bars,
                 always_show_checksum=always_show_checksum,
                 wide_narrow_ratio=wide_narrow_ratio,
                 validate_text=validate_text,
                 supplement_data=supplement_data,
                 supplement_space=supplement_space,
                 bar_width_reduction=bar_width_reduction,
+                use_anti_alias=use_anti_alias,
                 storage=storage,
                 folder=folder,
                 format=format,
                 **kwargs
             )
         else:
             (data) = self.put_barcode_generate_file_with_http_info(
@@ -1405,14 +1401,15 @@
                 filled_bars=filled_bars,
                 always_show_checksum=always_show_checksum,
                 wide_narrow_ratio=wide_narrow_ratio,
                 validate_text=validate_text,
                 supplement_data=supplement_data,
                 supplement_space=supplement_space,
                 bar_width_reduction=bar_width_reduction,
+                use_anti_alias=use_anti_alias,
                 storage=storage,
                 folder=folder,
                 format=format,
                 **kwargs
             )
             return data
 
@@ -1464,14 +1461,15 @@
             "filled_bars",
             "always_show_checksum",
             "wide_narrow_ratio",
             "validate_text",
             "supplement_data",
             "supplement_space",
             "bar_width_reduction",
+            "use_anti_alias",
             "storage",
             "folder",
             "format",
         }
         all_params.add("async_req")
         all_params.add("_return_http_data_only")
         all_params.add("_preload_content")
@@ -1567,14 +1565,16 @@
             query_params.append(("ValidateText", params["validate_text"]))
         if "supplement_data" in params:
             query_params.append(("SupplementData", params["supplement_data"]))
         if "supplement_space" in params:
             query_params.append(("SupplementSpace", params["supplement_space"]))
         if "bar_width_reduction" in params:
             query_params.append(("BarWidthReduction", params["bar_width_reduction"]))
+        if "use_anti_alias" in params:
+            query_params.append(("UseAntiAlias", params["use_anti_alias"]))
         if "storage" in params:
             query_params.append(("storage", params["storage"]))
         if "folder" in params:
             query_params.append(("folder", params["folder"]))
         if "format" in params:
             query_params.append(("format", params["format"]))
```

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api/file_api.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/file_api.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api/folder_api.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/folder_api.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api/storage_api.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/storage_api.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/api_client.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,21 +86,21 @@
         self.configuration = configuration
 
         # Use the pool property to lazily initialize the ThreadPool.
         self._pool = None
         self.rest_client = RESTClientObject(configuration)
         self.default_headers = {
             "x-aspose-client": "python sdk",
-            "x-aspose-client-version": "23.3.0",
+            "x-aspose-client-version": "23.4.0",
         }
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "Aspose-Barcode-SDK/23.3.0/python"
+        self.user_agent = "Aspose-Barcode-SDK/23.4.0/python"
 
     def __del__(self):
         self.rest_client.close()
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/configuration.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 3.0\n"
-            "SDK Package Version: 23.3.0".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 23.4.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     @staticmethod
     def fetch_token(client_id, client_secret, token_url):
         with contextlib.closing(
             RESTClientObject(Configuration(client_id=client_id, client_secret=client_secret, token_url=token_url))
         ) as client:
```

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/__init__.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/api_error.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/api_error.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/api_error_response.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/australian_post_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/australian_post_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/auto_size_mode.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/auto_size_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/available_graphics_unit.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/available_graphics_unit.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/aztec_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/aztec_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/aztec_symbol_mode.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/aztec_symbol_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/barcode_response.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/barcode_response.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/barcode_response_list.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/barcode_response_list.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/border_dash_style.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/border_dash_style.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/caption_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/caption_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/checksum_validation.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/checksum_validation.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/codabar_checksum_mode.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_checksum_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/codabar_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/codabar_symbol.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_symbol.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/codablock_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codablock_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/code128_emulation.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code128_emulation.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/code16_k_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code16_k_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/code_location.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code_location.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/coupon_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/coupon_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/data_bar_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_bar_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/data_matrix_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/decode_barcode_type.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/decode_barcode_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/disc_usage.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/dot_code_encode_mode.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/dot_code_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/dot_code_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/dot_code_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/eci_encodings.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/eci_encodings.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/enable_checksum.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/enable_checksum.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/encode_barcode_type.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/encode_barcode_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/error.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/error.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/error_details.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/file_version.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/file_versions.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/files_list.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/files_upload_result.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/font_mode.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/font_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/font_style.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_style.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/generator_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/generator_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         "filled_bars": "bool",
         "always_show_checksum": "bool",
         "wide_narrow_ratio": "float",
         "validate_text": "bool",
         "supplement_data": "str",
         "supplement_space": "float",
         "bar_width_reduction": "float",
+        "use_anti_alias": "bool",
         "australian_post": "AustralianPostParams",
         "aztec": "AztecParams",
         "codabar": "CodabarParams",
         "codablock": "CodablockParams",
         "code16_k": "Code16KParams",
         "coupon": "CouponParams",
         "data_bar": "DataBarParams",
@@ -135,14 +136,15 @@
         "filled_bars": "FilledBars",
         "always_show_checksum": "AlwaysShowChecksum",
         "wide_narrow_ratio": "WideNarrowRatio",
         "validate_text": "ValidateText",
         "supplement_data": "SupplementData",
         "supplement_space": "SupplementSpace",
         "bar_width_reduction": "BarWidthReduction",
+        "use_anti_alias": "UseAntiAlias",
         "australian_post": "AustralianPost",
         "aztec": "Aztec",
         "codabar": "Codabar",
         "codablock": "Codablock",
         "code16_k": "Code16K",
         "coupon": "Coupon",
         "data_bar": "DataBar",
@@ -192,14 +194,15 @@
         filled_bars=None,
         always_show_checksum=None,
         wide_narrow_ratio=None,
         validate_text=None,
         supplement_data=None,
         supplement_space=None,
         bar_width_reduction=None,
+        use_anti_alias=None,
         australian_post=None,
         aztec=None,
         codabar=None,
         codablock=None,
         code16_k=None,
         coupon=None,
         data_bar=None,
@@ -248,14 +251,15 @@
         self._filled_bars = None
         self._always_show_checksum = None
         self._wide_narrow_ratio = None
         self._validate_text = None
         self._supplement_data = None
         self._supplement_space = None
         self._bar_width_reduction = None
+        self._use_anti_alias = None
         self._australian_post = None
         self._aztec = None
         self._codabar = None
         self._codablock = None
         self._code16_k = None
         self._coupon = None
         self._data_bar = None
@@ -339,14 +343,16 @@
             self.validate_text = validate_text
         if supplement_data is not None:
             self.supplement_data = supplement_data
         if supplement_space is not None:
             self.supplement_space = supplement_space
         if bar_width_reduction is not None:
             self.bar_width_reduction = bar_width_reduction
+        if use_anti_alias is not None:
+            self.use_anti_alias = use_anti_alias
         if australian_post is not None:
             self.australian_post = australian_post
         if aztec is not None:
             self.aztec = aztec
         if codabar is not None:
             self.codabar = codabar
         if codablock is not None:
@@ -1249,14 +1255,37 @@
         :param bar_width_reduction: The bar_width_reduction of this GeneratorParams.  # noqa: E501
         :type: float
         """
 
         self._bar_width_reduction = bar_width_reduction
 
     @property
+    def use_anti_alias(self):
+        """Gets the use_anti_alias of this GeneratorParams.  # noqa: E501
+
+        Indicates whether is used anti-aliasing mode to render image. Anti-aliasing mode is applied to barcode and text drawing.  # noqa: E501
+
+        :return: The use_anti_alias of this GeneratorParams.  # noqa: E501
+        :rtype: bool
+        """
+        return self._use_anti_alias
+
+    @use_anti_alias.setter
+    def use_anti_alias(self, use_anti_alias):
+        """Sets the use_anti_alias of this GeneratorParams.
+
+        Indicates whether is used anti-aliasing mode to render image. Anti-aliasing mode is applied to barcode and text drawing.  # noqa: E501
+
+        :param use_anti_alias: The use_anti_alias of this GeneratorParams.  # noqa: E501
+        :type: bool
+        """
+
+        self._use_anti_alias = use_anti_alias
+
+    @property
     def australian_post(self):
         """Gets the australian_post of this GeneratorParams.  # noqa: E501
 
         AustralianPost params.  # noqa: E501
 
         :return: The australian_post of this GeneratorParams.  # noqa: E501
         :rtype: AustralianPostParams
```

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/generator_params_list.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/generator_params_list.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/itf14_border_type.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/itf14_border_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/itf_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/itf_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/macro_character.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/macro_character.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/maxi_code_mode.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/maxi_code_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/object_exist.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/padding.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/padding.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/patch_code_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/patch_code_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/patch_format.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/patch_format.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/pdf417_error_level.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_error_level.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/pdf417_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/postal_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/postal_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/preset_type.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/preset_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/qr_encode_mode.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/qr_encode_type.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_encode_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/qr_error_level.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_error_level.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/qr_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/qr_version.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_version.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/reader_params.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/reader_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,49 +354,49 @@
 
         self._preset = preset
 
     @property
     def rect_x(self):
         """Gets the rect_x of this ReaderParams.  # noqa: E501
 
-        Set X for area for recognition.  # noqa: E501
+        Set X of top left corner of area for recognition.  # noqa: E501
 
         :return: The rect_x of this ReaderParams.  # noqa: E501
         :rtype: int
         """
         return self._rect_x
 
     @rect_x.setter
     def rect_x(self, rect_x):
         """Sets the rect_x of this ReaderParams.
 
-        Set X for area for recognition.  # noqa: E501
+        Set X of top left corner of area for recognition.  # noqa: E501
 
         :param rect_x: The rect_x of this ReaderParams.  # noqa: E501
         :type: int
         """
 
         self._rect_x = rect_x
 
     @property
     def rect_y(self):
         """Gets the rect_y of this ReaderParams.  # noqa: E501
 
-        Set Y for area for recognition.  # noqa: E501
+        Set Y of top left corner of area for recognition.  # noqa: E501
 
         :return: The rect_y of this ReaderParams.  # noqa: E501
         :rtype: int
         """
         return self._rect_y
 
     @rect_y.setter
     def rect_y(self, rect_y):
         """Sets the rect_y of this ReaderParams.
 
-        Set Y for area for recognition.  # noqa: E501
+        Set Y of top left corner of area for recognition.  # noqa: E501
 
         :param rect_y: The rect_y of this ReaderParams.  # noqa: E501
         :type: int
         """
 
         self._rect_y = rect_y
```

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/region_point.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/region_point.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/result_image_info.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/result_image_info.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/storage_exist.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/storage_file.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/structured_append.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/structured_append.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/models/text_alignment.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/text_alignment.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud/rest.py` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/rest.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud.egg-info/PKG-INFO` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-barcode-cloud
-Version: 23.3.0
+Version: 23.4.0
 Summary: Aspose.Barcode Cloud API Reference
 Home-page: https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Author: Aspose Barcode Cloud
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Project-URL: Website, https://www.aspose.cloud
 Project-URL: Product Home, https://products.aspose.cloud/barcode/
@@ -15,15 +15,15 @@
 Description: # Aspose.BarCode Cloud SDK for Python
         
         [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
         [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
         [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
         
         - API version: 3.0
-        - Package version: 23.3.0
+        - Package version: 23.4.0
         
         ## Demo applications
         
         [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
         :---: | :---: | :---:
         [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
         [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -102,15 +102,15 @@
                                                                   preset=aspose_barcode_cloud.PresetType.HIGHPERFORMANCE)
         pprint(response)
         ```
         
         ## Requirements
         
         - six >= 1.10
-        - urllib3 >= 1.15.1
+        - urllib3 >= 1.21.1, <2.0
         
         ## Licensing
         
         All Aspose.BarCode for Cloud SDKs, helper scripts and templates are licensed under [MIT License](LICENSE).
         
         ## Resources
```

### Comparing `aspose-barcode-cloud-23.3.0/aspose_barcode_cloud.egg-info/SOURCES.txt` & `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.3.0/setup.py` & `aspose-barcode-cloud-23.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 """
 
 import os
 
 from setuptools import setup, find_packages
 
 NAME = "aspose-barcode-cloud"
-VERSION = "23.3.0"
+VERSION = "23.4.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
-REQUIRES = ["certifi>=2017.4.17", "python-dateutil>=2.1", "six>=1.10", "urllib3>=1.23"]
+REQUIRES = ["certifi>=2017.4.17", "python-dateutil>=2.1", "six>=1.10", "urllib3 >= 1.21.1, <2.0"]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "README.md"), "rt") as f:
     long_description = f.read()
 
 setup(
```


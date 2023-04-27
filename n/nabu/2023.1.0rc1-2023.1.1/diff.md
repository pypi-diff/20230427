# Comparing `tmp/nabu-2023.1.0rc1.tar.gz` & `tmp/nabu-2023.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nabu-2023.1.0rc1.tar", last modified: Tue Mar 14 07:57:18 2023, max compression
+gzip compressed data, was "nabu-2023.1.1.tar", last modified: Thu Apr 27 11:47:17 2023, max compression
```

## Comparing `nabu-2023.1.0rc1.tar` & `nabu-2023.1.1.tar`

### file list

```diff
@@ -1,247 +1,247 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.627090 nabu-2023.1.0rc1/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1061 2020-04-08 07:02:06.000000 nabu-2023.1.0rc1/LICENSE
--rw-r--r--   0 pierre    (1000) pierre    (1000)      273 2023-03-14 07:57:18.627090 nabu-2023.1.0rc1/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1614 2021-05-20 09:15:33.000000 nabu-2023.1.0rc1/README.md
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.607090 nabu-2023.1.0rc1/nabu/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      239 2023-03-14 07:56:48.000000 nabu-2023.1.0rc1/nabu/__init__.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.611090 nabu-2023.1.0rc1/nabu/app/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/app/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3233 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/app/bootstrap.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      733 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/app/bootstrap_stitching.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8921 2023-03-07 14:24:36.000000 nabu-2023.1.0rc1/nabu/app/cast_volume.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    14128 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/app/cli_configs.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3327 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/app/compare_volumes.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3412 2023-03-14 07:56:18.000000 nabu-2023.1.0rc1/nabu/app/composite_cor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4665 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/app/create_distortion_map_from_poly.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5437 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/app/double_flatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8879 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/app/generate_header.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7905 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/app/histogram.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4963 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/app/nx_z_splitter.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3779 2023-03-14 07:56:18.000000 nabu-2023.1.0rc1/nabu/app/prepare_weights_double.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3773 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/app/reconstruct.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3859 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/app/reconstruct_helical.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6422 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/app/rotate.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3494 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/app/shrink_dataset.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      789 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/app/stitching.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      984 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/app/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3360 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/app/validator.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.611090 nabu-2023.1.0rc1/nabu/cuda/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-05-26 09:53:09.000000 nabu-2023.1.0rc1/nabu/cuda/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    15326 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/cuda/convolution.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6552 2023-03-07 07:21:31.000000 nabu-2023.1.0rc1/nabu/cuda/kernel.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5787 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/cuda/medfilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4784 2023-03-07 07:21:31.000000 nabu-2023.1.0rc1/nabu/cuda/padding.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5500 2023-03-07 07:21:31.000000 nabu-2023.1.0rc1/nabu/cuda/processing.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.611090 nabu-2023.1.0rc1/nabu/cuda/src/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4770 2023-03-07 07:21:31.000000 nabu-2023.1.0rc1/nabu/cuda/src/ElementOp.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5154 2022-01-06 13:21:23.000000 nabu-2023.1.0rc1/nabu/cuda/src/backproj.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1851 2021-05-20 15:41:47.000000 nabu-2023.1.0rc1/nabu/cuda/src/backproj_polar.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2898 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/cuda/src/boundary.h
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7353 2020-08-05 14:37:44.000000 nabu-2023.1.0rc1/nabu/cuda/src/convolution.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2220 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/cuda/src/fftshift.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2058 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/cuda/src/flatfield.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      553 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/cuda/src/fourier_wavelets.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1476 2021-12-08 12:46:24.000000 nabu-2023.1.0rc1/nabu/cuda/src/halftomo.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2014 2022-11-24 08:53:51.000000 nabu-2023.1.0rc1/nabu/cuda/src/helical_padding.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      808 2020-10-27 10:43:16.000000 nabu-2023.1.0rc1/nabu/cuda/src/histogram.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2405 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/cuda/src/hst_backproj.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      839 2021-08-12 07:07:29.000000 nabu-2023.1.0rc1/nabu/cuda/src/interpolation.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2449 2021-08-12 07:07:29.000000 nabu-2023.1.0rc1/nabu/cuda/src/medfilt.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1407 2020-09-21 06:10:47.000000 nabu-2023.1.0rc1/nabu/cuda/src/normalization.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4424 2022-12-24 06:48:14.000000 nabu-2023.1.0rc1/nabu/cuda/src/padding.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      657 2021-03-04 08:50:36.000000 nabu-2023.1.0rc1/nabu/cuda/src/rotation.cu
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.611090 nabu-2023.1.0rc1/nabu/cuda/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/cuda/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2721 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/cuda/tests/test_medfilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7101 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/cuda/tests/test_padding.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8384 2023-03-09 16:41:35.000000 nabu-2023.1.0rc1/nabu/cuda/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.611090 nabu-2023.1.0rc1/nabu/estimation/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      379 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    20914 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/alignment.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    36802 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/estimation/cor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6494 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/estimation/cor_sino.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4701 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/estimation/distortion.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    15765 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/focus.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.615090 nabu-2023.1.0rc1/nabu/estimation/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-05-20 09:15:33.000000 nabu-2023.1.0rc1/nabu/estimation/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2491 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/tests/test_alignment.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    17119 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/tests/test_cor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4170 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/tests/test_focus.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1658 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/tests/test_tilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2999 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/tests/test_translation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8596 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/tilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8301 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/translation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1401 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/estimation/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.615090 nabu-2023.1.0rc1/nabu/io/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      176 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/io/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    15085 2023-03-07 14:24:36.000000 nabu-2023.1.0rc1/nabu/io/cast_volume.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    11744 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/io/detector_distortion.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    22555 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/io/reader.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4477 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/io/reader_helical.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.615090 nabu-2023.1.0rc1/nabu/io/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-08-05 06:12:22.000000 nabu-2023.1.0rc1/nabu/io/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8883 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/io/tests/test_cast_volume.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6335 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/io/tests/test_detector_distortion.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7188 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/io/tests/test_writers.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3841 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/io/tiffwriter_zmm.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8867 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/io/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    28503 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/io/writer.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.615090 nabu-2023.1.0rc1/nabu/misc/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/misc/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2920 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/binning.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      604 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/filters.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5691 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/misc/fourier_filters.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    11316 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/histogram.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3243 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/histogram_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2713 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/padding.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1856 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/misc/rotation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2783 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/rotation_cuda.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.615090 nabu-2023.1.0rc1/nabu/misc/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/misc/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1884 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/tests/test_binning.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2320 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/tests/test_histogram.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2392 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/tests/test_interpolation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2684 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/misc/tests/test_rotation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2897 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/tests/test_unsharp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2682 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/unsharp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2119 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/unsharp_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2884 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/unsharp_opencl.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3906 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/misc/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.615090 nabu-2023.1.0rc1/nabu/opencl/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/opencl/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5168 2023-03-07 07:21:31.000000 nabu-2023.1.0rc1/nabu/opencl/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.619090 nabu-2023.1.0rc1/nabu/pipeline/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2023.1.0rc1/nabu/pipeline/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9301 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/pipeline/config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    14025 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/config_validators.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6520 2023-03-14 07:56:12.000000 nabu-2023.1.0rc1/nabu/pipeline/datadump.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9207 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/dataset_validator.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      920 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/detector_distortion_provider.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    32033 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/estimators.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6086 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/fallback_utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.619090 nabu-2023.1.0rc1/nabu/pipeline/fullfield/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2023.1.0rc1/nabu/pipeline/fullfield/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    36047 2023-03-14 07:56:12.000000 nabu-2023.1.0rc1/nabu/pipeline/fullfield/chunked.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5405 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/fullfield/chunked_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8829 2023-03-14 07:56:12.000000 nabu-2023.1.0rc1/nabu/pipeline/fullfield/computations.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3055 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/fullfield/dataset_validator.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    28634 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/fullfield/nabu_config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    35427 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/fullfield/processconfig.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    34682 2023-03-09 16:41:35.000000 nabu-2023.1.0rc1/nabu/pipeline/fullfield/reconstruction.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.619090 nabu-2023.1.0rc1/nabu/pipeline/helical/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-06-24 07:40:44.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      382 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/dataset_validator.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5580 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/fbp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    10353 2023-03-07 07:21:31.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/filtering.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    20672 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/gridded_accumulator.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    62315 2023-03-14 07:56:18.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/helical_chunked_regridded.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4013 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/helical_chunked_regridded_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    22216 2023-03-09 15:31:10.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/helical_reconstruction.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1439 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/helical_utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7299 2023-03-09 15:31:10.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/nabu_config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2571 2023-03-04 19:02:12.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/processconfig.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    25043 2023-03-09 15:31:10.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/span_strategy.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.619090 nabu-2023.1.0rc1/nabu/pipeline/helical/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-06-24 07:40:44.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6159 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/tests/test_accumulator.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    14569 2023-03-09 16:41:35.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/tests/test_pipeline_elements_full.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2721 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/tests/test_strategy.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1555 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3981 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/helical/weight_balancer.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2778 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/params.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8539 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/processconfig.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2730 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/pipeline/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    10920 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/pipeline/writer.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.619090 nabu-2023.1.0rc1/nabu/pipeline/xrdct/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2023.1.0rc1/nabu/pipeline/xrdct/__init__.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.623090 nabu-2023.1.0rc1/nabu/preproc/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      284 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/preproc/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      379 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/preproc/alignment.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5144 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/preproc/ccd.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6062 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/preproc/ccd_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    14891 2023-03-09 16:41:35.000000 nabu-2023.1.0rc1/nabu/preproc/ctf.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4972 2023-03-09 16:41:35.000000 nabu-2023.1.0rc1/nabu/preproc/ctf_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3309 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/preproc/distortion.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7864 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/preproc/double_flatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6132 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/preproc/double_flatfield_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2279 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/preproc/double_flatfield_variable_region.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    19202 2023-03-07 07:21:54.000000 nabu-2023.1.0rc1/nabu/preproc/flatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5438 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/preproc/flatfield_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3155 2023-03-07 07:21:54.000000 nabu-2023.1.0rc1/nabu/preproc/flatfield_variable_region.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    16572 2023-03-09 16:41:35.000000 nabu-2023.1.0rc1/nabu/preproc/phase.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4863 2023-03-09 16:41:35.000000 nabu-2023.1.0rc1/nabu/preproc/phase_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3424 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/preproc/shift.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2477 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/preproc/shift_cuda.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.623090 nabu-2023.1.0rc1/nabu/preproc/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/preproc/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2249 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/preproc/tests/test_ccd_corr.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9853 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/preproc/tests/test_ctf.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2601 2023-03-07 07:21:31.000000 nabu-2023.1.0rc1/nabu/preproc/tests/test_double_flatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    23498 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/preproc/tests/test_flatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2182 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/preproc/tests/test_paganin.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2284 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/preproc/tests/test_vshift.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.623090 nabu-2023.1.0rc1/nabu/reconstruction/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      163 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    11057 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/cone.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    15436 2023-03-07 07:21:31.000000 nabu-2023.1.0rc1/nabu/reconstruction/fbp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3644 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/reconstruction/fbp_opencl.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8004 2023-03-07 07:21:31.000000 nabu-2023.1.0rc1/nabu/reconstruction/filtering.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7299 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/reconstructor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1759 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/reconstructor_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2405 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/rings.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5316 2023-03-09 16:41:35.000000 nabu-2023.1.0rc1/nabu/reconstruction/rings_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    14784 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/sinogram.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9285 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/sinogram_cuda.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.623090 nabu-2023.1.0rc1/nabu/reconstruction/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/reconstruction/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    11813 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/tests/test_cone.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3221 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/tests/test_deringer.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6471 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/reconstruction/tests/test_fbp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6995 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/tests/test_halftomo.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3221 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/tests/test_reconstructor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3692 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/reconstruction/tests/test_sino_normalization.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.623090 nabu-2023.1.0rc1/nabu/resources/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/resources/__init__.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.623090 nabu-2023.1.0rc1/nabu/resources/cli/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/resources/cli/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      170 2021-10-01 06:59:16.000000 nabu-2023.1.0rc1/nabu/resources/cor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    12760 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/resources/dataset_analyzer.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5701 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/resources/gpu.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3758 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/resources/logger.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9204 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/resources/nxflatfield.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.623090 nabu-2023.1.0rc1/nabu/resources/templates/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-11-24 08:53:51.000000 nabu-2023.1.0rc1/nabu/resources/templates/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      394 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/resources/templates/bm05_pag.conf
--rw-r--r--   0 pierre    (1000) pierre    (1000)      842 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/resources/templates/id16_ctf.conf
--rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/resources/templates/id16_holo.conf
--rw-r--r--   0 pierre    (1000) pierre    (1000)      384 2022-11-24 08:53:51.000000 nabu-2023.1.0rc1/nabu/resources/templates/id19_pag.conf
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.623090 nabu-2023.1.0rc1/nabu/resources/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-09-08 07:42:25.000000 nabu-2023.1.0rc1/nabu/resources/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4298 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/resources/tests/test_nxflatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2155 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/resources/tests/test_units.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5485 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/resources/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.627090 nabu-2023.1.0rc1/nabu/stitching/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/stitching/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    18413 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/stitching/config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7385 2023-03-04 19:02:16.000000 nabu-2023.1.0rc1/nabu/stitching/frame_composition.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6178 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/stitching/overlap.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7909 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/stitching/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    43070 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/stitching/z_stitching.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1400 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/tests.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    10857 2023-02-07 09:23:45.000000 nabu-2023.1.0rc1/nabu/testutils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.627090 nabu-2023.1.0rc1/nabu/thirdparty/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/thirdparty/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4500 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/thirdparty/pore3d_deringer_munch.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8634 2020-02-16 18:41:31.000000 nabu-2023.1.0rc1/nabu/thirdparty/tomopy_phase.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5611 2021-05-20 15:41:47.000000 nabu-2023.1.0rc1/nabu/thirdparty/tomwer_load_flats_darks.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    21956 2023-03-09 16:41:35.000000 nabu-2023.1.0rc1/nabu/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-03-14 07:57:18.607090 nabu-2023.1.0rc1/nabu.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      273 2023-03-14 07:57:18.000000 nabu-2023.1.0rc1/nabu.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6550 2023-03-14 07:57:18.000000 nabu-2023.1.0rc1/nabu.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-03-14 07:57:18.000000 nabu-2023.1.0rc1/nabu.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)      965 2023-03-14 07:57:18.000000 nabu-2023.1.0rc1/nabu.egg-info/entry_points.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)      202 2023-03-14 07:57:18.000000 nabu-2023.1.0rc1/nabu.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        5 2023-03-14 07:57:18.000000 nabu-2023.1.0rc1/nabu.egg-info/top_level.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-04-16 09:51:10.000000 nabu-2023.1.0rc1/nabu.egg-info/zip-safe
--rw-r--r--   0 pierre    (1000) pierre    (1000)       38 2023-03-14 07:57:18.627090 nabu-2023.1.0rc1/setup.cfg
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2743 2023-03-14 07:56:12.000000 nabu-2023.1.0rc1/setup.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.472733 nabu-2023.1.1/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1061 2020-04-08 07:02:06.000000 nabu-2023.1.1/LICENSE
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      270 2023-04-27 11:47:17.472733 nabu-2023.1.1/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1614 2021-05-20 09:15:33.000000 nabu-2023.1.1/README.md
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.452733 nabu-2023.1.1/nabu/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      235 2023-04-27 10:05:45.000000 nabu-2023.1.1/nabu/__init__.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.452733 nabu-2023.1.1/nabu/app/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/app/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3233 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/bootstrap.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      733 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/bootstrap_stitching.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8921 2023-03-28 09:40:32.000000 nabu-2023.1.1/nabu/app/cast_volume.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    14128 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/app/cli_configs.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3327 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/compare_volumes.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3412 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/composite_cor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4665 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/create_distortion_map_from_poly.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5437 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/double_flatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8879 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/generate_header.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7905 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/histogram.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4963 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/nx_z_splitter.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3779 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/prepare_weights_double.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3773 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/reconstruct.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3859 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/reconstruct_helical.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6422 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/rotate.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3494 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/shrink_dataset.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      789 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/app/stitching.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      984 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/app/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3360 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/app/validator.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.456733 nabu-2023.1.1/nabu/cuda/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-05-26 09:53:09.000000 nabu-2023.1.1/nabu/cuda/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    15326 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/cuda/convolution.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6552 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/cuda/kernel.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5787 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/cuda/medfilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4784 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/cuda/padding.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5500 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/cuda/processing.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.456733 nabu-2023.1.1/nabu/cuda/src/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4770 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/cuda/src/ElementOp.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5154 2022-01-06 13:21:23.000000 nabu-2023.1.1/nabu/cuda/src/backproj.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1851 2021-05-20 15:41:47.000000 nabu-2023.1.1/nabu/cuda/src/backproj_polar.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2898 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/cuda/src/boundary.h
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7353 2020-08-05 14:37:44.000000 nabu-2023.1.1/nabu/cuda/src/convolution.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2220 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/cuda/src/fftshift.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2058 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/cuda/src/flatfield.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      553 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/cuda/src/fourier_wavelets.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1476 2021-12-08 12:46:24.000000 nabu-2023.1.1/nabu/cuda/src/halftomo.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2014 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/cuda/src/helical_padding.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      808 2020-10-27 10:43:16.000000 nabu-2023.1.1/nabu/cuda/src/histogram.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2405 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/cuda/src/hst_backproj.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      839 2021-08-12 07:07:29.000000 nabu-2023.1.1/nabu/cuda/src/interpolation.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2449 2021-08-12 07:07:29.000000 nabu-2023.1.1/nabu/cuda/src/medfilt.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1407 2020-09-21 06:10:47.000000 nabu-2023.1.1/nabu/cuda/src/normalization.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4424 2022-12-24 06:48:14.000000 nabu-2023.1.1/nabu/cuda/src/padding.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      657 2021-03-04 08:50:36.000000 nabu-2023.1.1/nabu/cuda/src/rotation.cu
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.456733 nabu-2023.1.1/nabu/cuda/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/cuda/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2721 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/cuda/tests/test_medfilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7101 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/cuda/tests/test_padding.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8384 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/cuda/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.456733 nabu-2023.1.1/nabu/estimation/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      379 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/estimation/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    21253 2023-04-27 10:13:17.000000 nabu-2023.1.1/nabu/estimation/alignment.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    36802 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/estimation/cor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6494 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/estimation/cor_sino.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4701 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/estimation/distortion.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    15765 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/estimation/focus.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.456733 nabu-2023.1.1/nabu/estimation/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-05-20 09:15:33.000000 nabu-2023.1.1/nabu/estimation/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2491 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/estimation/tests/test_alignment.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    17119 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/estimation/tests/test_cor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4170 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/estimation/tests/test_focus.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1658 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/estimation/tests/test_tilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2999 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/estimation/tests/test_translation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8648 2023-04-27 10:13:17.000000 nabu-2023.1.1/nabu/estimation/tilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8301 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/estimation/translation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1401 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/estimation/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.460733 nabu-2023.1.1/nabu/io/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      176 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/io/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    14817 2023-04-27 10:15:05.000000 nabu-2023.1.1/nabu/io/cast_volume.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    11744 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/io/detector_distortion.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    22555 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/io/reader.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4477 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/io/reader_helical.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.460733 nabu-2023.1.1/nabu/io/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-08-05 06:12:22.000000 nabu-2023.1.1/nabu/io/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8883 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/io/tests/test_cast_volume.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6335 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/io/tests/test_detector_distortion.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7188 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/io/tests/test_writers.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3841 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/io/tiffwriter_zmm.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8867 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/io/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    28503 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/io/writer.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.460733 nabu-2023.1.1/nabu/misc/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/misc/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2920 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/binning.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      604 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/filters.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5691 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/misc/fourier_filters.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    11316 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/histogram.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3243 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/histogram_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2713 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/padding.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1856 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/misc/rotation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2783 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/rotation_cuda.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.460733 nabu-2023.1.1/nabu/misc/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/misc/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1884 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/tests/test_binning.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2320 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/tests/test_histogram.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2392 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/tests/test_interpolation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2684 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/misc/tests/test_rotation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2897 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/tests/test_unsharp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2682 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/unsharp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2119 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/unsharp_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2884 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/unsharp_opencl.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3906 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/misc/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.460733 nabu-2023.1.1/nabu/opencl/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/opencl/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5168 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/opencl/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.460733 nabu-2023.1.1/nabu/pipeline/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2023.1.1/nabu/pipeline/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9301 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/pipeline/config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    14025 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/config_validators.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6520 2023-03-28 09:40:32.000000 nabu-2023.1.1/nabu/pipeline/datadump.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9207 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/dataset_validator.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      920 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/detector_distortion_provider.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    32033 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/estimators.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6086 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/fallback_utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.464733 nabu-2023.1.1/nabu/pipeline/fullfield/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2023.1.1/nabu/pipeline/fullfield/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    36047 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/pipeline/fullfield/chunked.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5405 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/pipeline/fullfield/chunked_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8829 2023-03-28 09:40:32.000000 nabu-2023.1.1/nabu/pipeline/fullfield/computations.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3055 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/fullfield/dataset_validator.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    28634 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/pipeline/fullfield/nabu_config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    35427 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/fullfield/processconfig.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    34682 2023-03-09 16:41:35.000000 nabu-2023.1.1/nabu/pipeline/fullfield/reconstruction.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.464733 nabu-2023.1.1/nabu/pipeline/helical/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-06-24 07:40:44.000000 nabu-2023.1.1/nabu/pipeline/helical/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      382 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/pipeline/helical/dataset_validator.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5580 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/pipeline/helical/fbp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    10353 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/pipeline/helical/filtering.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    20672 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/helical/gridded_accumulator.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    62315 2023-03-28 09:40:32.000000 nabu-2023.1.1/nabu/pipeline/helical/helical_chunked_regridded.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4013 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/pipeline/helical/helical_chunked_regridded_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    22216 2023-03-28 09:40:32.000000 nabu-2023.1.1/nabu/pipeline/helical/helical_reconstruction.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1439 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/pipeline/helical/helical_utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7299 2023-03-28 09:40:32.000000 nabu-2023.1.1/nabu/pipeline/helical/nabu_config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2571 2023-03-04 19:02:12.000000 nabu-2023.1.1/nabu/pipeline/helical/processconfig.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    25043 2023-03-28 09:40:32.000000 nabu-2023.1.1/nabu/pipeline/helical/span_strategy.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.464733 nabu-2023.1.1/nabu/pipeline/helical/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-06-24 07:40:44.000000 nabu-2023.1.1/nabu/pipeline/helical/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6159 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/helical/tests/test_accumulator.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    14569 2023-03-09 16:41:35.000000 nabu-2023.1.1/nabu/pipeline/helical/tests/test_pipeline_elements_full.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2721 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/helical/tests/test_strategy.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1555 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/pipeline/helical/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3981 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/helical/weight_balancer.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2778 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/params.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8539 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/processconfig.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2730 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/pipeline/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    10920 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/pipeline/writer.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.464733 nabu-2023.1.1/nabu/pipeline/xrdct/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2023.1.1/nabu/pipeline/xrdct/__init__.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.464733 nabu-2023.1.1/nabu/preproc/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      284 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/preproc/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      379 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/preproc/alignment.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5144 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/preproc/ccd.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6062 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/preproc/ccd_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    14891 2023-03-09 16:41:35.000000 nabu-2023.1.1/nabu/preproc/ctf.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4972 2023-03-09 16:41:35.000000 nabu-2023.1.1/nabu/preproc/ctf_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3309 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/preproc/distortion.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7864 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/preproc/double_flatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6132 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/preproc/double_flatfield_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2279 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/preproc/double_flatfield_variable_region.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    19202 2023-03-28 09:40:32.000000 nabu-2023.1.1/nabu/preproc/flatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5438 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/preproc/flatfield_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3155 2023-03-28 09:40:32.000000 nabu-2023.1.1/nabu/preproc/flatfield_variable_region.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    16572 2023-03-09 16:41:35.000000 nabu-2023.1.1/nabu/preproc/phase.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4863 2023-03-09 16:41:35.000000 nabu-2023.1.1/nabu/preproc/phase_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3424 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/preproc/shift.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2477 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/preproc/shift_cuda.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.468733 nabu-2023.1.1/nabu/preproc/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/preproc/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2249 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/preproc/tests/test_ccd_corr.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9853 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/preproc/tests/test_ctf.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2601 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/preproc/tests/test_double_flatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    23498 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/preproc/tests/test_flatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2182 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/preproc/tests/test_paganin.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2284 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/preproc/tests/test_vshift.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.468733 nabu-2023.1.1/nabu/reconstruction/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      163 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/reconstruction/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    11057 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/reconstruction/cone.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    15436 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/reconstruction/fbp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3644 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/reconstruction/fbp_opencl.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8004 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/reconstruction/filtering.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7299 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/reconstruction/reconstructor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1759 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/reconstruction/reconstructor_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2405 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/reconstruction/rings.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5316 2023-03-09 16:41:35.000000 nabu-2023.1.1/nabu/reconstruction/rings_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    14784 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/reconstruction/sinogram.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9285 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/reconstruction/sinogram_cuda.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.468733 nabu-2023.1.1/nabu/reconstruction/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/reconstruction/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    11813 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/reconstruction/tests/test_cone.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3221 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/reconstruction/tests/test_deringer.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6471 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/reconstruction/tests/test_fbp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6995 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/reconstruction/tests/test_halftomo.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3221 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/reconstruction/tests/test_reconstructor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3692 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/reconstruction/tests/test_sino_normalization.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.468733 nabu-2023.1.1/nabu/resources/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/resources/__init__.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.468733 nabu-2023.1.1/nabu/resources/cli/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/resources/cli/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      170 2021-10-01 06:59:16.000000 nabu-2023.1.1/nabu/resources/cor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    13219 2023-04-27 10:14:25.000000 nabu-2023.1.1/nabu/resources/dataset_analyzer.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5701 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/resources/gpu.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3758 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/resources/logger.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9204 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/resources/nxflatfield.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.468733 nabu-2023.1.1/nabu/resources/templates/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-11-24 08:53:51.000000 nabu-2023.1.1/nabu/resources/templates/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      394 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/resources/templates/bm05_pag.conf
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      842 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/resources/templates/id16_ctf.conf
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/resources/templates/id16_holo.conf
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      384 2022-11-24 08:53:51.000000 nabu-2023.1.1/nabu/resources/templates/id19_pag.conf
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.468733 nabu-2023.1.1/nabu/resources/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-09-08 07:42:25.000000 nabu-2023.1.1/nabu/resources/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4298 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/resources/tests/test_nxflatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2155 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/resources/tests/test_units.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5485 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/resources/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.468733 nabu-2023.1.1/nabu/stitching/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/stitching/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    18413 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/stitching/config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7385 2023-03-04 19:02:16.000000 nabu-2023.1.1/nabu/stitching/frame_composition.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6178 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/stitching/overlap.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7909 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/stitching/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    43070 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/stitching/z_stitching.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1400 2023-02-07 09:23:45.000000 nabu-2023.1.1/nabu/tests.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    10857 2023-03-24 07:15:11.000000 nabu-2023.1.1/nabu/testutils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.468733 nabu-2023.1.1/nabu/thirdparty/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/thirdparty/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4500 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/thirdparty/pore3d_deringer_munch.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8634 2020-02-16 18:41:31.000000 nabu-2023.1.1/nabu/thirdparty/tomopy_phase.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5611 2021-05-20 15:41:47.000000 nabu-2023.1.1/nabu/thirdparty/tomwer_load_flats_darks.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    21956 2023-04-27 10:05:11.000000 nabu-2023.1.1/nabu/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-04-27 11:47:17.452733 nabu-2023.1.1/nabu.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      270 2023-04-27 11:47:17.000000 nabu-2023.1.1/nabu.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6550 2023-04-27 11:47:17.000000 nabu-2023.1.1/nabu.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-04-27 11:47:17.000000 nabu-2023.1.1/nabu.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      965 2023-04-27 11:47:17.000000 nabu-2023.1.1/nabu.egg-info/entry_points.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      202 2023-04-27 11:47:17.000000 nabu-2023.1.1/nabu.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        5 2023-04-27 11:47:17.000000 nabu-2023.1.1/nabu.egg-info/top_level.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-04-16 09:51:10.000000 nabu-2023.1.1/nabu.egg-info/zip-safe
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       38 2023-04-27 11:47:17.472733 nabu-2023.1.1/setup.cfg
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2743 2023-04-27 10:05:11.000000 nabu-2023.1.1/setup.py
```

### Comparing `nabu-2023.1.0rc1/LICENSE` & `nabu-2023.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/README.md` & `nabu-2023.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/bootstrap.py` & `nabu-2023.1.1/nabu/app/bootstrap.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/bootstrap_stitching.py` & `nabu-2023.1.1/nabu/app/bootstrap_stitching.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/cast_volume.py` & `nabu-2023.1.1/nabu/app/cast_volume.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/cli_configs.py` & `nabu-2023.1.1/nabu/app/cli_configs.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/compare_volumes.py` & `nabu-2023.1.1/nabu/app/compare_volumes.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/composite_cor.py` & `nabu-2023.1.1/nabu/app/composite_cor.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/create_distortion_map_from_poly.py` & `nabu-2023.1.1/nabu/app/create_distortion_map_from_poly.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/double_flatfield.py` & `nabu-2023.1.1/nabu/app/double_flatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/generate_header.py` & `nabu-2023.1.1/nabu/app/generate_header.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/histogram.py` & `nabu-2023.1.1/nabu/app/histogram.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/nx_z_splitter.py` & `nabu-2023.1.1/nabu/app/nx_z_splitter.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/prepare_weights_double.py` & `nabu-2023.1.1/nabu/app/prepare_weights_double.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/reconstruct.py` & `nabu-2023.1.1/nabu/app/reconstruct.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/reconstruct_helical.py` & `nabu-2023.1.1/nabu/app/reconstruct_helical.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/rotate.py` & `nabu-2023.1.1/nabu/app/rotate.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/shrink_dataset.py` & `nabu-2023.1.1/nabu/app/shrink_dataset.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/stitching.py` & `nabu-2023.1.1/nabu/app/stitching.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/utils.py` & `nabu-2023.1.1/nabu/app/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/app/validator.py` & `nabu-2023.1.1/nabu/app/validator.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/convolution.py` & `nabu-2023.1.1/nabu/cuda/convolution.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/kernel.py` & `nabu-2023.1.1/nabu/cuda/kernel.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/medfilt.py` & `nabu-2023.1.1/nabu/cuda/medfilt.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/padding.py` & `nabu-2023.1.1/nabu/cuda/padding.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/processing.py` & `nabu-2023.1.1/nabu/cuda/processing.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/ElementOp.cu` & `nabu-2023.1.1/nabu/cuda/src/ElementOp.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/backproj.cu` & `nabu-2023.1.1/nabu/cuda/src/backproj.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/backproj_polar.cu` & `nabu-2023.1.1/nabu/cuda/src/backproj_polar.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/boundary.h` & `nabu-2023.1.1/nabu/cuda/src/boundary.h`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/convolution.cu` & `nabu-2023.1.1/nabu/cuda/src/convolution.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/fftshift.cu` & `nabu-2023.1.1/nabu/cuda/src/fftshift.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/flatfield.cu` & `nabu-2023.1.1/nabu/cuda/src/flatfield.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/fourier_wavelets.cu` & `nabu-2023.1.1/nabu/cuda/src/fourier_wavelets.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/halftomo.cu` & `nabu-2023.1.1/nabu/cuda/src/halftomo.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/helical_padding.cu` & `nabu-2023.1.1/nabu/cuda/src/helical_padding.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/histogram.cu` & `nabu-2023.1.1/nabu/cuda/src/histogram.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/hst_backproj.cu` & `nabu-2023.1.1/nabu/cuda/src/hst_backproj.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/interpolation.cu` & `nabu-2023.1.1/nabu/cuda/src/interpolation.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/medfilt.cu` & `nabu-2023.1.1/nabu/cuda/src/medfilt.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/normalization.cu` & `nabu-2023.1.1/nabu/cuda/src/normalization.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/padding.cu` & `nabu-2023.1.1/nabu/cuda/src/padding.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/src/rotation.cu` & `nabu-2023.1.1/nabu/cuda/src/rotation.cu`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/tests/test_medfilt.py` & `nabu-2023.1.1/nabu/cuda/tests/test_medfilt.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/tests/test_padding.py` & `nabu-2023.1.1/nabu/cuda/tests/test_padding.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/cuda/utils.py` & `nabu-2023.1.1/nabu/cuda/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/alignment.py` & `nabu-2023.1.1/nabu/estimation/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,24 @@
 
 
 local_fftn = scipy.fft.rfftn
 local_ifftn = scipy.fft.irfftn
 
 
 class AlignmentBase:
+    default_extra_options = {"blocking_plots": False}
+
     def __init__(
         self,
         vert_fft_width=False,
         horz_fft_width=False,
         verbose=False,
         logger=None,
         data_type=np.float32,
+        extra_options=None,
     ):
         """
         Alignment basic functions.
 
         Parameters
         ----------
         vert_fft_width: boolean, optional
@@ -62,27 +65,29 @@
 
         verbose: boolean, optional
             When True it will produce verbose output, including plots.
         data_type: `numpy.float32`
             Computation data type.
         """
 
-        self._init_parameters(vert_fft_width, horz_fft_width, verbose, logger, data_type)
+        self._init_parameters(vert_fft_width, horz_fft_width, verbose, logger, data_type, extra_options=extra_options)
         self._plot_windows = {}
 
-    def _init_parameters(self, vert_fft_width, horz_fft_width, verbose, logger, data_type):
+    def _init_parameters(self, vert_fft_width, horz_fft_width, verbose, logger, data_type, extra_options=None):
         self.logger = LoggerOrPrint(logger)
         self.truncate_vert_pow2 = vert_fft_width
         self.truncate_horz_pow2 = horz_fft_width
 
         if verbose and not __have_matplotlib__:
             self.logger.warning("Matplotlib not available. Plotting disabled, despite being activated by user")
             verbose = False
         self.verbose = verbose
         self.data_type = data_type
+        self.extra_options = self.default_extra_options.copy()
+        self.extra_options.update(extra_options or {})
 
     @staticmethod
     def _check_img_stack_size(img_stack: np.ndarray, img_pos: np.ndarray):
         shape_stack = np.squeeze(img_stack).shape
         shape_pos = np.squeeze(img_pos).shape
         if not len(shape_stack) == 3:
             raise ValueError(
@@ -198,15 +203,15 @@
                     vertex_min_yx[1],
                     vertex_max_yx[1],
                 )
             )
         return vertex_yx
 
     @staticmethod
-    def refine_max_position_1d(f_vals, fx=None, return_vertex_val=False):
+    def refine_max_position_1d(f_vals, fx=None, return_vertex_val=False, return_all_coeffs=False):
         """Computes the sub-pixel max position of the given function sampling.
 
         Parameters
         ----------
         f_vals: numpy.ndarray
             Function values of the sampled points
         fx: numpy.ndarray, optional
@@ -250,15 +255,17 @@
             coeffs = poly.convert().coef
         else:
             coords = np.array([np.ones(num_vals), fx, fx**2])
             coeffs = np.linalg.lstsq(coords.T, f_vals, rcond=None)[0]
 
         # For a 1D parabola `f(x) = c + bx + ax^2`, the vertex position is:
         # x_v = -b / 2a.
-        vertex_x = (-coeffs[1, :] / (2 * coeffs[2, :]))[0]
+        vertex_x = -coeffs[1, :] / (2 * coeffs[2, :])
+        if not return_all_coeffs:
+            vertex_x = vertex_x[0]
 
         vertex_min_x = np.min(fx)
         vertex_max_x = np.max(fx)
         lower_bound_ok = vertex_min_x < vertex_x
         upper_bound_ok = vertex_x < vertex_max_x
         if not np.all(lower_bound_ok * upper_bound_ok):
             if len(f_vals.shape) == 1:
```

### Comparing `nabu-2023.1.0rc1/nabu/estimation/cor.py` & `nabu-2023.1.1/nabu/estimation/cor.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/cor_sino.py` & `nabu-2023.1.1/nabu/estimation/cor_sino.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/distortion.py` & `nabu-2023.1.1/nabu/estimation/distortion.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/focus.py` & `nabu-2023.1.1/nabu/estimation/focus.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/tests/test_alignment.py` & `nabu-2023.1.1/nabu/estimation/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/tests/test_cor.py` & `nabu-2023.1.1/nabu/estimation/tests/test_cor.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/tests/test_focus.py` & `nabu-2023.1.1/nabu/estimation/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/tests/test_tilt.py` & `nabu-2023.1.1/nabu/estimation/tests/test_tilt.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/tests/test_translation.py` & `nabu-2023.1.1/nabu/estimation/tests/test_translation.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/tilt.py` & `nabu-2023.1.1/nabu/estimation/tilt.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             img_1, img_2, padding_mode, axes=(-1,), high_pass=high_pass, low_pass=low_pass
         )
 
         img_shape = img_2.shape
         cc_h_coords = np.fft.fftfreq(img_shape[-1], 1 / img_shape[-1])
 
         (f_vals, fh) = self.extract_peak_regions_1d(cc, peak_radius=peak_fit_radius, cc_coords=cc_h_coords)
-        fitted_shifts_h = self.refine_max_position_1d(f_vals)
+        fitted_shifts_h = self.refine_max_position_1d(f_vals, return_all_coeffs=True)
         fitted_shifts_h += fh[1, :]
 
         # Computing tilt
         fitted_shifts_h = median_filter(fitted_shifts_h, size=3)
 
         half_img_size = (img_shape[-2] - 1) / 2
         cc_v_coords = np.linspace(-half_img_size, half_img_size, img_shape[-2])
@@ -153,18 +153,18 @@
                 "Fitted center of rotation (pixels):",
                 cor_offset_pix,
                 "and camera tilt (degrees):",
                 tilt_deg,
             )
             f, ax = plt.subplots(1, 1)
             self._add_plot_window(f, ax=ax)
-            ax.scatter(cc_v_coords, fitted_shifts_h)
+            ax.plot(cc_v_coords, fitted_shifts_h)
             ax.plot(cc_v_coords, polyval(cc_v_coords, coeffs_h), "-C1")
             ax.set_title("Correlation peaks")
-            plt.show(block=False)
+            plt.show(block=self.extra_options["blocking_plots"])
 
         return cor_offset_pix, tilt_deg
 
     def _compute_angle_fftpolar(
         self, img_1: np.ndarray, img_2: np.ndarray, padding_mode=None, peak_fit_radius=1, high_pass=None, low_pass=None
     ):
         img_shape = img_2.shape
```

### Comparing `nabu-2023.1.0rc1/nabu/estimation/translation.py` & `nabu-2023.1.1/nabu/estimation/translation.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/estimation/utils.py` & `nabu-2023.1.1/nabu/estimation/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/io/cast_volume.py` & `nabu-2023.1.1/nabu/io/cast_volume.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,18 +49,20 @@
     if isinstance(input_volume, (EDFVolume, TIFFVolume, JP2KVolume)):
         if output_type == "hdf5":
             file_path = os.path.join(
                 input_volume.data_url.file_path(),
                 output_dir,
                 input_volume.get_volume_basename() + ".hdf5",
             )
-            return HDF5Volume(
+            volume = HDF5Volume(
                 file_path=file_path,
                 data_path="/volume",
             )
+            assert volume.get_identifier() is not None, "volume should be able to create an identifier"
+            return volume
         elif output_type in ("tiff", "edf", "jp2"):
             if output_type == "tiff":
                 Constructor = TIFFVolume
             elif output_type == "edf":
                 Constructor = EDFVolume
             elif output_type == "jp2":
                 Constructor = JP2KVolume
@@ -79,44 +81,33 @@
             # replace extension:
             data_file_name = ".".join(
                 [
                     os.path.splitext(data_file_name)[0],
                     "hdf5",
                 ]
             )
-            metadata_file_parent_path, metadata_file_name = os.path.split(input_volume.metadata_url.file_path())
             if isinstance(input_volume, HDF5Volume):
                 data_data_path = input_volume.data_url.data_path()
                 metadata_data_path = input_volume.metadata_url.data_path()
-                data_scheme = input_volume.data_url.scheme()
-                metadata_scheme = input_volume.metadata_url.scheme()
+                try:
+                    data_path = os.path.commonprefix([data_data_path, metadata_data_path])
+                except Exception:
+                    data_path = "volume"
             else:
                 data_data_path = HDF5Volume.DATA_DATASET_NAME
                 metadata_data_path = HDF5Volume.METADATA_GROUP_NAME
-                metadata_file_name = data_file_name
-                data_scheme = "silx"
-                metadata_scheme = "silx"
+                file_path = data_file_name
+                data_path = "volume"
 
-            data_scheme
-            data_url = DataUrl(
+            volume = HDF5Volume(
                 file_path=os.path.join(data_file_parent_path, output_dir, data_file_name),
-                data_path=data_data_path,
-                scheme=data_scheme,
-            )
-
-            metadata_url = DataUrl(
-                file_path=os.path.join(metadata_file_parent_path, output_dir, metadata_file_name),
-                data_path=metadata_data_path,
-                scheme=metadata_scheme,
-            )
-
-            return HDF5Volume(
-                data_url=data_url,
-                metadata_url=metadata_url,
+                data_path=data_path,
             )
+            assert volume.get_identifier() is not None, "volume should be able to create an identifier"
+            return volume
         elif output_type in ("tiff", "edf", "jp2"):
             if output_type == "tiff":
                 Constructor = TIFFVolume
             elif output_type == "edf":
                 Constructor = EDFVolume
             elif output_type == "jp2":
                 Constructor = JP2KVolume
```

### Comparing `nabu-2023.1.0rc1/nabu/io/detector_distortion.py` & `nabu-2023.1.1/nabu/io/detector_distortion.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/io/reader.py` & `nabu-2023.1.1/nabu/io/reader.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/io/reader_helical.py` & `nabu-2023.1.1/nabu/io/reader_helical.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/io/tests/test_cast_volume.py` & `nabu-2023.1.1/nabu/io/tests/test_cast_volume.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/io/tests/test_detector_distortion.py` & `nabu-2023.1.1/nabu/io/tests/test_detector_distortion.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/io/tests/test_writers.py` & `nabu-2023.1.1/nabu/io/tests/test_writers.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/io/tiffwriter_zmm.py` & `nabu-2023.1.1/nabu/io/tiffwriter_zmm.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/io/utils.py` & `nabu-2023.1.1/nabu/io/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/io/writer.py` & `nabu-2023.1.1/nabu/io/writer.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/binning.py` & `nabu-2023.1.1/nabu/misc/binning.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/filters.py` & `nabu-2023.1.1/nabu/misc/filters.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/fourier_filters.py` & `nabu-2023.1.1/nabu/misc/fourier_filters.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/histogram.py` & `nabu-2023.1.1/nabu/misc/histogram.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/histogram_cuda.py` & `nabu-2023.1.1/nabu/misc/histogram_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/padding.py` & `nabu-2023.1.1/nabu/misc/padding.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/rotation.py` & `nabu-2023.1.1/nabu/misc/rotation.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/rotation_cuda.py` & `nabu-2023.1.1/nabu/misc/rotation_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/tests/test_binning.py` & `nabu-2023.1.1/nabu/misc/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/tests/test_histogram.py` & `nabu-2023.1.1/nabu/misc/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/tests/test_interpolation.py` & `nabu-2023.1.1/nabu/misc/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/tests/test_rotation.py` & `nabu-2023.1.1/nabu/misc/tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/tests/test_unsharp.py` & `nabu-2023.1.1/nabu/misc/tests/test_unsharp.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/unsharp.py` & `nabu-2023.1.1/nabu/misc/unsharp.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/unsharp_cuda.py` & `nabu-2023.1.1/nabu/misc/unsharp_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/unsharp_opencl.py` & `nabu-2023.1.1/nabu/misc/unsharp_opencl.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/misc/utils.py` & `nabu-2023.1.1/nabu/misc/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/opencl/utils.py` & `nabu-2023.1.1/nabu/opencl/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/config.py` & `nabu-2023.1.1/nabu/pipeline/config.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/config_validators.py` & `nabu-2023.1.1/nabu/pipeline/config_validators.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/datadump.py` & `nabu-2023.1.1/nabu/pipeline/datadump.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/dataset_validator.py` & `nabu-2023.1.1/nabu/pipeline/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/detector_distortion_provider.py` & `nabu-2023.1.1/nabu/pipeline/detector_distortion_provider.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/estimators.py` & `nabu-2023.1.1/nabu/pipeline/estimators.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/fallback_utils.py` & `nabu-2023.1.1/nabu/pipeline/fallback_utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/fullfield/chunked.py` & `nabu-2023.1.1/nabu/pipeline/fullfield/chunked.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/fullfield/chunked_cuda.py` & `nabu-2023.1.1/nabu/pipeline/fullfield/chunked_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/fullfield/computations.py` & `nabu-2023.1.1/nabu/pipeline/fullfield/computations.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/fullfield/dataset_validator.py` & `nabu-2023.1.1/nabu/pipeline/fullfield/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/fullfield/nabu_config.py` & `nabu-2023.1.1/nabu/pipeline/fullfield/nabu_config.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/fullfield/processconfig.py` & `nabu-2023.1.1/nabu/pipeline/fullfield/processconfig.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/fullfield/reconstruction.py` & `nabu-2023.1.1/nabu/pipeline/fullfield/reconstruction.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/fbp.py` & `nabu-2023.1.1/nabu/pipeline/helical/fbp.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/filtering.py` & `nabu-2023.1.1/nabu/pipeline/helical/filtering.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/gridded_accumulator.py` & `nabu-2023.1.1/nabu/pipeline/helical/gridded_accumulator.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/helical_chunked_regridded.py` & `nabu-2023.1.1/nabu/pipeline/helical/helical_chunked_regridded.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/helical_chunked_regridded_cuda.py` & `nabu-2023.1.1/nabu/pipeline/helical/helical_chunked_regridded_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/helical_reconstruction.py` & `nabu-2023.1.1/nabu/pipeline/helical/helical_reconstruction.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/helical_utils.py` & `nabu-2023.1.1/nabu/pipeline/helical/helical_utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/nabu_config.py` & `nabu-2023.1.1/nabu/pipeline/helical/nabu_config.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/processconfig.py` & `nabu-2023.1.1/nabu/pipeline/helical/processconfig.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/span_strategy.py` & `nabu-2023.1.1/nabu/pipeline/helical/span_strategy.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/tests/test_accumulator.py` & `nabu-2023.1.1/nabu/pipeline/helical/tests/test_accumulator.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/tests/test_pipeline_elements_full.py` & `nabu-2023.1.1/nabu/pipeline/helical/tests/test_pipeline_elements_full.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/tests/test_strategy.py` & `nabu-2023.1.1/nabu/pipeline/helical/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/utils.py` & `nabu-2023.1.1/nabu/pipeline/helical/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/helical/weight_balancer.py` & `nabu-2023.1.1/nabu/pipeline/helical/weight_balancer.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/params.py` & `nabu-2023.1.1/nabu/pipeline/params.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/processconfig.py` & `nabu-2023.1.1/nabu/pipeline/processconfig.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/utils.py` & `nabu-2023.1.1/nabu/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/pipeline/writer.py` & `nabu-2023.1.1/nabu/pipeline/writer.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/ccd.py` & `nabu-2023.1.1/nabu/preproc/ccd.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/ccd_cuda.py` & `nabu-2023.1.1/nabu/preproc/ccd_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/ctf.py` & `nabu-2023.1.1/nabu/preproc/ctf.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/ctf_cuda.py` & `nabu-2023.1.1/nabu/preproc/ctf_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/distortion.py` & `nabu-2023.1.1/nabu/preproc/distortion.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/double_flatfield.py` & `nabu-2023.1.1/nabu/preproc/double_flatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/double_flatfield_cuda.py` & `nabu-2023.1.1/nabu/preproc/double_flatfield_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/double_flatfield_variable_region.py` & `nabu-2023.1.1/nabu/preproc/double_flatfield_variable_region.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/flatfield.py` & `nabu-2023.1.1/nabu/preproc/flatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/flatfield_cuda.py` & `nabu-2023.1.1/nabu/preproc/flatfield_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/flatfield_variable_region.py` & `nabu-2023.1.1/nabu/preproc/flatfield_variable_region.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/phase.py` & `nabu-2023.1.1/nabu/preproc/phase.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/phase_cuda.py` & `nabu-2023.1.1/nabu/preproc/phase_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/shift.py` & `nabu-2023.1.1/nabu/preproc/shift.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/shift_cuda.py` & `nabu-2023.1.1/nabu/preproc/shift_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/tests/test_ccd_corr.py` & `nabu-2023.1.1/nabu/preproc/tests/test_ccd_corr.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/tests/test_ctf.py` & `nabu-2023.1.1/nabu/preproc/tests/test_ctf.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/tests/test_double_flatfield.py` & `nabu-2023.1.1/nabu/preproc/tests/test_double_flatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/tests/test_flatfield.py` & `nabu-2023.1.1/nabu/preproc/tests/test_flatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/tests/test_paganin.py` & `nabu-2023.1.1/nabu/preproc/tests/test_paganin.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/preproc/tests/test_vshift.py` & `nabu-2023.1.1/nabu/preproc/tests/test_vshift.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/cone.py` & `nabu-2023.1.1/nabu/reconstruction/cone.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/fbp.py` & `nabu-2023.1.1/nabu/reconstruction/fbp.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/fbp_opencl.py` & `nabu-2023.1.1/nabu/reconstruction/fbp_opencl.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/filtering.py` & `nabu-2023.1.1/nabu/reconstruction/filtering.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/reconstructor.py` & `nabu-2023.1.1/nabu/reconstruction/reconstructor.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/reconstructor_cuda.py` & `nabu-2023.1.1/nabu/reconstruction/reconstructor_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/rings.py` & `nabu-2023.1.1/nabu/reconstruction/rings.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/rings_cuda.py` & `nabu-2023.1.1/nabu/reconstruction/rings_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/sinogram.py` & `nabu-2023.1.1/nabu/reconstruction/sinogram.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/sinogram_cuda.py` & `nabu-2023.1.1/nabu/reconstruction/sinogram_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/tests/test_cone.py` & `nabu-2023.1.1/nabu/reconstruction/tests/test_cone.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/tests/test_deringer.py` & `nabu-2023.1.1/nabu/reconstruction/tests/test_deringer.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/tests/test_fbp.py` & `nabu-2023.1.1/nabu/reconstruction/tests/test_fbp.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/tests/test_halftomo.py` & `nabu-2023.1.1/nabu/reconstruction/tests/test_halftomo.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/tests/test_reconstructor.py` & `nabu-2023.1.1/nabu/reconstruction/tests/test_reconstructor.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/reconstruction/tests/test_sino_normalization.py` & `nabu-2023.1.1/nabu/reconstruction/tests/test_sino_normalization.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/resources/dataset_analyzer.py` & `nabu-2023.1.1/nabu/resources/dataset_analyzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -243,14 +243,23 @@
         Not applicable for EDF (return None)
         """
         return None
 
     def _is_halftomo(self):
         return None
 
+    def _get_rotation_angles(self):
+        if self._rotation_angles is None:
+            scan_range = self.dataset_scanner.scan_range
+            if scan_range is not None:
+                fullturn = abs(scan_range - 360) < abs(scan_range - 180)
+                angles = np.linspace(0, scan_range, num=self.dataset_scanner.tomo_n, endpoint=fullturn, dtype="f")
+                self._rotation_angles = np.deg2rad(angles)
+        return self._rotation_angles
+
 
 class HDF5DatasetAnalyzer(DatasetAnalyzer):
     """
     HDF5 dataset analyzer
     """
 
     _scanner = HDF5TomoScan
```

### Comparing `nabu-2023.1.0rc1/nabu/resources/gpu.py` & `nabu-2023.1.1/nabu/resources/gpu.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/resources/logger.py` & `nabu-2023.1.1/nabu/resources/logger.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/resources/nxflatfield.py` & `nabu-2023.1.1/nabu/resources/nxflatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/resources/templates/id16_ctf.conf` & `nabu-2023.1.1/nabu/resources/templates/id16_ctf.conf`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/resources/templates/id16_holo.conf` & `nabu-2023.1.1/nabu/resources/templates/id16_holo.conf`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/resources/tests/test_nxflatfield.py` & `nabu-2023.1.1/nabu/resources/tests/test_nxflatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/resources/tests/test_units.py` & `nabu-2023.1.1/nabu/resources/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/resources/utils.py` & `nabu-2023.1.1/nabu/resources/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/stitching/config.py` & `nabu-2023.1.1/nabu/stitching/config.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/stitching/frame_composition.py` & `nabu-2023.1.1/nabu/stitching/frame_composition.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/stitching/overlap.py` & `nabu-2023.1.1/nabu/stitching/overlap.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/stitching/utils.py` & `nabu-2023.1.1/nabu/stitching/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/stitching/z_stitching.py` & `nabu-2023.1.1/nabu/stitching/z_stitching.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/tests.py` & `nabu-2023.1.1/nabu/tests.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/testutils.py` & `nabu-2023.1.1/nabu/testutils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/thirdparty/pore3d_deringer_munch.py` & `nabu-2023.1.1/nabu/thirdparty/pore3d_deringer_munch.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/thirdparty/tomopy_phase.py` & `nabu-2023.1.1/nabu/thirdparty/tomopy_phase.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/thirdparty/tomwer_load_flats_darks.py` & `nabu-2023.1.1/nabu/thirdparty/tomwer_load_flats_darks.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu/utils.py` & `nabu-2023.1.1/nabu/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu.egg-info/SOURCES.txt` & `nabu-2023.1.1/nabu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/nabu.egg-info/entry_points.txt` & `nabu-2023.1.1/nabu.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `nabu-2023.1.0rc1/setup.py` & `nabu-2023.1.1/setup.py`

 * *Files identical despite different names*


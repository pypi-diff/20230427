# Comparing `tmp/BioTEMPy-2.0.0.tar.gz` & `tmp/BioTEMPy-2.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BioTEMPy-2.0.0.tar", last modified: Tue Jul 12 15:20:41 2022, max compression
+gzip compressed data, was "dist/BioTEMPy-2.1.0a0.tar", last modified: Thu Apr 27 08:07:31 2023, max compression
```

## Comparing `BioTEMPy-2.0.0.tar` & `BioTEMPy-2.1.0a0.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/BioTEMPy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      497 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/BioTEMPy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1418 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/BioTEMPy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/BioTEMPy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      169 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/BioTEMPy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/BioTEMPy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/BioTEMPy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      497 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3137 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/
--rw-rw-rw-   0 root         (0) root         (0)       52 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/assembly/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/assembly/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    13073 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/assembly/assembly.py
--rw-rw-rw-   0 root         (0) root         (0)    46912 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/assembly/gamma.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5194 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/cli/arg_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    11044 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/cli/class_arg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/core/data/
--rw-rw-rw-   0 root         (0) root         (0)       82 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/core/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1778 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/core/data/download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/core/errors/
--rw-rw-rw-   0 root         (0) root         (0)       86 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/core/errors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/core/errors/instance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/graphics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/graphics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20832 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/graphics/show_plot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/map_process/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/map_process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23863 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/map_process/map_filters.py
--rw-rw-rw-   0 root         (0) root         (0)    31367 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/map_process/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/maps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/maps/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    95185 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/maps/em_map.py
--rwxrwxrwx   0 root         (0) root         (0)    17392 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/maps/map_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4070 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/maps/map_transform_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/math/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/math/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29185 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/math/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)    25634 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/math/consensus.py
--rw-rw-rw-   0 root         (0) root         (0)    11869 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/math/fourier.py
--rw-rw-rw-   0 root         (0) root         (0)     5064 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/math/quaternion.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/math/transform_parser.py
--rwxrwxrwx   0 root         (0) root         (0)    16972 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/math/vector.py
--rwxrwxrwx   0 root         (0) root         (0)     4746 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/math/vq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/optimisation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/optimisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10371 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/optimisation/ensemble_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/protein/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/protein/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14634 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/protein/mmcif.py
--rw-rw-rw-   0 root         (0) root         (0)    70893 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/protein/prot_rep_biopy.py
--rw-rw-rw-   0 root         (0) root         (0)    11687 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/protein/rigid_body_parser.py
--rw-rw-rw-   0 root         (0) root         (0)   142093 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/protein/scoring_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    54324 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/protein/structure_blurrer.py
--rw-rw-rw-   0 root         (0) root         (0)    23532 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/protein/structure_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/script/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 13:26:42.000000 BioTEMPy-2.0.0/TEMPy/script/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10663 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/script/gamma.py
--rw-rw-rw-   0 root         (0) root         (0)     8760 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/script/loqfit.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/script/sccc.py
--rw-rw-rw-   0 root         (0) root         (0)     7527 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/script/smoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/TEMPy/tempy_data/
--rw-rw-rw-   0 root         (0) root         (0)   523370 2022-07-12 12:03:45.000000 BioTEMPy-2.0.0/TEMPy/tempy_data/quaternion_vectors_5000.pk
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-12 15:20:41.000000 BioTEMPy-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1315 2022-07-12 14:46:38.000000 BioTEMPy-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/BioTEMPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/BioTEMPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/BioTEMPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/BioTEMPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      169 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/BioTEMPy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/BioTEMPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/BioTEMPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3137 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/assembly/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/assembly/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    13073 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/assembly/assembly.py
+-rw-rw-rw-   0 root         (0) root         (0)    46912 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/assembly/gamma.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14120 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/cli/arg_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    11044 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/cli/class_arg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/core/data/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/core/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/core/data/download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/core/errors/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/core/errors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/core/errors/instance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/graphics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/graphics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20832 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/graphics/show_plot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/map_process/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/map_process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23863 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/map_process/map_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)    31367 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/map_process/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/maps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/maps/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    95185 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/maps/em_map.py
+-rwxrwxrwx   0 root         (0) root         (0)    17392 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/maps/map_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4070 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/maps/map_transform_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/math/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/math/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29185 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/math/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)    25634 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/math/consensus.py
+-rw-rw-rw-   0 root         (0) root         (0)    11869 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/math/fourier.py
+-rw-rw-rw-   0 root         (0) root         (0)     5064 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/math/quaternion.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/math/transform_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)    16972 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/math/vector.py
+-rwxrwxrwx   0 root         (0) root         (0)     4746 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/math/vq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/optimisation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/optimisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10371 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/optimisation/ensemble_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/protein/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/protein/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14647 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/protein/mmcif.py
+-rw-rw-rw-   0 root         (0) root         (0)    70893 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/protein/prot_rep_biopy.py
+-rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/protein/rigid_body_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)   142093 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/protein/scoring_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    54324 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/protein/structure_blurrer.py
+-rw-rw-rw-   0 root         (0) root         (0)    19448 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/protein/structure_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/script/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/script/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10663 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/script/gamma.py
+-rw-rw-rw-   0 root         (0) root         (0)     5045 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/script/loqfit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/script/mi.py
+-rw-rw-rw-   0 root         (0) root         (0)    11963 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/script/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/script/sccc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/script/smoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/TEMPy/tempy_data/
+-rw-rw-rw-   0 root         (0) root         (0)   523370 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/TEMPy/tempy_data/quaternion_vectors_5000.pk
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 08:07:31.000000 BioTEMPy-2.1.0a0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-04-27 08:07:19.000000 BioTEMPy-2.1.0a0/setup.py
```

### Comparing `BioTEMPy-2.0.0/BioTEMPy.egg-info/SOURCES.txt` & `BioTEMPy-2.1.0a0/BioTEMPy.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -44,10 +44,12 @@
 TEMPy/protein/rigid_body_parser.py
 TEMPy/protein/scoring_functions.py
 TEMPy/protein/structure_blurrer.py
 TEMPy/protein/structure_parser.py
 TEMPy/script/__init__.py
 TEMPy/script/gamma.py
 TEMPy/script/loqfit.py
+TEMPy/script/mi.py
+TEMPy/script/output.py
 TEMPy/script/sccc.py
 TEMPy/script/smoc.py
 TEMPy/tempy_data/quaternion_vectors_5000.pk
```

### Comparing `BioTEMPy-2.0.0/README.md` & `BioTEMPy-2.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/assembly/assembly.py` & `BioTEMPy-2.1.0a0/TEMPy/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/assembly/gamma.py` & `BioTEMPy-2.1.0a0/TEMPy/assembly/gamma.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/cli/class_arg.py` & `BioTEMPy-2.1.0a0/TEMPy/cli/class_arg.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/core/data/download.py` & `BioTEMPy-2.1.0a0/TEMPy/core/data/download.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/graphics/show_plot.py` & `BioTEMPy-2.1.0a0/TEMPy/graphics/show_plot.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/map_process/map_filters.py` & `BioTEMPy-2.1.0a0/TEMPy/map_process/map_filters.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/map_process/process.py` & `BioTEMPy-2.1.0a0/TEMPy/map_process/process.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/maps/em_map.py` & `BioTEMPy-2.1.0a0/TEMPy/maps/em_map.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/maps/map_parser.py` & `BioTEMPy-2.1.0a0/TEMPy/maps/map_parser.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/maps/map_transform_score.py` & `BioTEMPy-2.1.0a0/TEMPy/maps/map_transform_score.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/math/cluster.py` & `BioTEMPy-2.1.0a0/TEMPy/math/cluster.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/math/consensus.py` & `BioTEMPy-2.1.0a0/TEMPy/math/consensus.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/math/fourier.py` & `BioTEMPy-2.1.0a0/TEMPy/math/fourier.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/math/quaternion.py` & `BioTEMPy-2.1.0a0/TEMPy/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/math/transform_parser.py` & `BioTEMPy-2.1.0a0/TEMPy/math/transform_parser.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/math/vector.py` & `BioTEMPy-2.1.0a0/TEMPy/math/vector.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/math/vq.py` & `BioTEMPy-2.1.0a0/TEMPy/math/vq.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/optimisation/ensemble_generation.py` & `BioTEMPy-2.1.0a0/TEMPy/optimisation/ensemble_generation.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/protein/mmcif.py` & `BioTEMPy-2.1.0a0/TEMPy/protein/mmcif.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         try:
             cif_data_block = gemmi.cif.read(
                                             self.tempy_structure.filename
                                             ).sole_block()
             gstructure = gemmi.make_structure_from_block(cif_data_block)
             del gstructure[0]
-        except RuntimeError:  # filename couldn't be found
+        except ValueError: #RuntimeError:  # filename couldn't be found
             gstructure = gemmi.Structure()
             gstructure.name = self.tempy_structure.pdb_id
 
         model = gemmi.Model('1')
 
         for chain_name, indexes in self.tempy_structure.chain_indexes.items():
             chain = (gemmi.Chain(chain_name))
```

### Comparing `BioTEMPy-2.0.0/TEMPy/protein/prot_rep_biopy.py` & `BioTEMPy-2.1.0a0/TEMPy/protein/prot_rep_biopy.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/protein/rigid_body_parser.py` & `BioTEMPy-2.1.0a0/TEMPy/protein/rigid_body_parser.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/protein/scoring_functions.py` & `BioTEMPy-2.1.0a0/TEMPy/protein/scoring_functions.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/protein/structure_blurrer.py` & `BioTEMPy-2.1.0a0/TEMPy/protein/structure_blurrer.py`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/TEMPy/protein/structure_parser.py` & `BioTEMPy-2.1.0a0/TEMPy/protein/structure_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -297,83 +297,14 @@
                                             structure,
                                             filename,
                                             water=water,
                                             hetatm=hetatm,
                                             )
 
     @staticmethod
-    def old_read_PDB_file(
-            structure_id,
-            filename,
-            hetatm=False,
-            water=False,
-            chain=None,
-    ):
-        """ Read PDB file and create Structure instance based upon it.
-
-        Args:
-            structure_id: Structure_id code of pdb file
-            filename: Filename of pdb file
-            hetatm: If True, HETATM atoms are included in the
-                :class:`Structure instance <TEMPy.protein.prot_rep_biopy.gemmi_Structure>`
-                returned after parsing. If False, HETATM atoms are ignored.
-            water: If True, HETATM, water atoms are included in the
-                :class:`Structure instance <TEMPy.protein.prot_rep_biopy.gemmi_Structure>`
-                instance returned after parsing. If False, HETATM atoms are
-                ignored.
-        Returns:
-            :class:`Structure instance <TEMPy.protein.prot_rep_biopy.gemmi_Structure>`:
-                Parsed structure.
-        """
-        from Bio.PDB import PDBParser as PDBParserBiopy
-
-        p = PDBParserBiopy(QUIET=True)
-        structure = p.get_structure(structure_id, filename)
-        return PDBParser._bio_strcuture_to_TEMpy(
-            filename,
-            structure,
-            structure_id,
-            hetatm,
-            water,
-        )
-
-    @staticmethod
-    def read_PDB_file_BioPy(
-            structure_id,
-            filename,
-            hetatm=False,
-            water=False,
-            chain=None,
-    ):
-        """ Read PDB file using and create Structure instance based upon it.
-
-        Uses the `Biopython <https://biopython.org/>`_ library to parse the
-        input PDB file.
-
-        Args:
-            structure_id: Structure_id code of pdb file
-            filename: Filename of pdb file
-            hetatm: If True, HETATM atoms are included in the
-                :class:`Structure instance <TEMPy.protein.prot_rep_biopy.gemmi_Structure>`
-                returned after parsing. If False, HETATM atoms are ignored.
-            water: If True, HETATM, water atoms are included in the
-                :class:`Structure instance <TEMPy.protein.prot_rep_biopy.gemmi_Structure>`
-                instance returned after parsing. If False, HETATM atoms are
-                ignored.
-        Returns:
-            :class:`BioPy Structure instance <TEMPy.protein.prot_rep_biopy.gemmi_Structure>`:
-                Parsed structure.
-        """
-        from Bio.PDB import PDBParser as PDBParserBiopy
-
-        p = PDBParserBiopy(QUIET=True)
-        structure = p.get_structure(structure_id, filename)
-        return structure
-
-    @staticmethod
     def fetch_PDB(
             structure_id,
             local_filename,
             hetatm=False,
             water=False,
     ):
         """ Fetch PDB file from the PDB and create Structure instance based
@@ -400,53 +331,14 @@
         new_file, someinfo = urllib.request.urlretrieve(
                                                     url,
                                                     filename=local_filename)
 
         return PDBParser.read_PDB_file(structure_id, new_file)
 
     @staticmethod
-    def fetch_PDB_BioPy(
-            structure_id,
-            filename,
-            hetatm=False,
-            water=False,
-    ):
-        """Fetch PDB file and create Structure instance based upon it.
-
-        Uses the `Biopython <https://biopython.org/>`_ library to parse the
-        input PDB file.
-
-        Args:
-            structure_id: Structure_id code of pdb file
-            filename: Filename of pdb file
-            hetatm: If True, HETATM atoms are included in the
-                :class:`Structure instance <TEMPy.protein.prot_rep_biopy.gemmi_Structure>`
-                returned after parsing. If False, HETATM atoms are ignored.
-            water: If True, HETATM, water atoms are included in the
-                :class:`Structure instance <TEMPy.protein.prot_rep_biopy.gemmi_Structure>`
-                instance returned after parsing. If False, HETATM atoms are
-                ignored.
-        Returns:
-            :class:`BioPy Structure instance <TEMPy.protein.prot_rep_biopy.BioPy_Structure>`:
-                Parsed structure.
-        """
-        from Bio.PDB import PDBParser as PDBParserBiopy
-
-        url = 'http://www.rcsb.org/pdb/files/%s.pdb' % structure_id
-        p = PDBParserBiopy(QUIET=True)
-        urllib.urlretrieve(url, filename)
-        structure = p.get_structure(
-            structure_id,
-            filename,
-            hetatm=hetatm,
-            water=water,
-        )
-        return structure
-
-    @staticmethod
     def _bio_strcuture_to_TEMpy(
             filename,
             structure,
             pdb_id,
             hetatm=False,
             water=False,
     ):
```

### Comparing `BioTEMPy-2.0.0/TEMPy/script/gamma.py` & `BioTEMPy-2.1.0a0/TEMPy/script/gamma.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,9 +319,9 @@
     # finish job
     f = open(output_name + ".log", "a")
     f.write(
         "------------------------------------------------------------------------------------------\n"
     )
     f.write("Execution time (sec): " + str(time.time() - start_time) + "\n")
     f.close()
-    print("Finished gemmi tempy run!")
+    print("Finished gamma tempy run!")
     exit(0)
```

### Comparing `BioTEMPy-2.0.0/TEMPy/script/sccc.py` & `BioTEMPy-2.1.0a0/TEMPy/script/sccc.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 def get_parser():
     return parser.parser
 
 
 class SCCCScript:
     def __init__(self):
-        args = parser.parser.parse_args()
+        args = parser.parse_args()
         self.model = args.model
         self.map = args.map
         self.resolution = args.resolution
         self.prefix = args.output_prefix
         self.output_format = args.output_format
 
     def run(self):
@@ -91,12 +91,12 @@
 
 
 def main():
     sccc = SCCCScript()
     try:
         sccc.run()
     except Exception as e:
-        print(e)
+        raise e
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `BioTEMPy-2.0.0/TEMPy/tempy_data/quaternion_vectors_5000.pk` & `BioTEMPy-2.1.0a0/TEMPy/tempy_data/quaternion_vectors_5000.pk`

 * *Files identical despite different names*

### Comparing `BioTEMPy-2.0.0/setup.py` & `BioTEMPy-2.1.0a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 
 if os.path.exists('build') is True:
     print('build exists')
     shutil.rmtree('./build')
 
 setup(
     name='BioTEMPy',
-    version='2.0.0',
+    version='2.1.0-alpha',
     author='Maya Topf, Daven Vasishtan, Arun Prasad Pandurangan, Irene Farabella, Agnel-Praveen Joseph, Harpal Sahota',
     author_email='tempy-help@cryst.bbk.ac.uk',
     packages=setuptools.find_packages(),
     url='http://tempy.ismb.lon.ac.uk/',
     description='TEMPy: a Python Library for Assessment of 3D Electron Microscopy Density Fits',
     package_dir={'TEMPy': 'TEMPy'},
     python_requires='>=3.7',
     install_requires=[
         'biopython==1.73',
         'numpy>=1.16.1',
         'scipy>=1.2.0',
         'matplotlib',
-        'gemmi==0.4.5',
+        'gemmi==0.5.6',
         'voxcov>=0.2.6',
         'mrcfile',
         'pyfftw',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```


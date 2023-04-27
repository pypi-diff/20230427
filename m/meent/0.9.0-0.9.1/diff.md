# Comparing `tmp/meent-0.9.0.tar.gz` & `tmp/meent-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meent-0.9.0.tar", last modified: Sun Apr  2 16:17:30 2023, max compression
+gzip compressed data, was "meent-0.9.1.tar", last modified: Thu Apr 27 05:56:38 2023, max compression
```

## Comparing `meent-0.9.0.tar` & `meent-0.9.1.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.059456 meent-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-02 16:17:12.000000 meent-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-02 16:17:30.059456 meent-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-02 16:17:12.000000 meent-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.047456 meent-0.9.0/meent/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-02 16:17:12.000000 meent-0.9.0/meent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-02 16:17:12.000000 meent-0.9.0/meent/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.043456 meent-0.9.0/meent/nk_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.047456 meent-0.9.0/meent/nk_data/filmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-02 16:17:12.000000 meent-0.9.0/meent/nk_data/filmetrics/Al2O3.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-02 16:17:12.000000 meent-0.9.0/meent/nk_data/filmetrics/Si.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-02 16:17:12.000000 meent-0.9.0/meent/nk_data/filmetrics/Si3N4.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-02 16:17:12.000000 meent-0.9.0/meent/nk_data/filmetrics/SiO2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.047456 meent-0.9.0/meent/nk_data/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-04-02 16:17:12.000000 meent-0.9.0/meent/nk_data/matlab/p_Si.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.047456 meent-0.9.0/meent/on_jax/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.051456 meent-0.9.0/meent/on_jax/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    38785 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    16210 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.051456 meent-0.9.0/meent/on_jax/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.051456 meent-0.9.0/meent/on_jax/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_jax/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.051456 meent-0.9.0/meent/on_numpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.051456 meent-0.9.0/meent/on_numpy/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    27388 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.051456 meent-0.9.0/meent/on_numpy/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_numpy/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.051456 meent-0.9.0/meent/on_torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.055456 meent-0.9.0/meent/on_torch/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.055456 meent-0.9.0/meent/on_torch/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.059456 meent-0.9.0/meent/on_torch/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-02 16:17:12.000000 meent-0.9.0/meent/on_torch/optimizer/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-02 16:17:12.000000 meent-0.9.0/meent/testcase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:17:30.047456 meent-0.9.0/meent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-02 16:17:30.000000 meent-0.9.0/meent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-02 16:17:30.000000 meent-0.9.0/meent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 16:17:30.000000 meent-0.9.0/meent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-02 16:17:30.000000 meent-0.9.0/meent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-02 16:17:30.000000 meent-0.9.0/meent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 16:17:30.059456 meent-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-02 16:17:12.000000 meent-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.059154 meent-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-27 05:56:27.000000 meent-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-27 05:56:38.059154 meent-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-27 05:56:27.000000 meent-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.051154 meent-0.9.1/meent/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 05:56:27.000000 meent-0.9.1/meent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-27 05:56:27.000000 meent-0.9.1/meent/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.051154 meent-0.9.1/meent/nk_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/nk_data/filmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-27 05:56:27.000000 meent-0.9.1/meent/nk_data/filmetrics/Al2O3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-27 05:56:27.000000 meent-0.9.1/meent/nk_data/filmetrics/Si.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-27 05:56:27.000000 meent-0.9.1/meent/nk_data/filmetrics/Si3N4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-27 05:56:27.000000 meent-0.9.1/meent/nk_data/filmetrics/SiO2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/nk_data/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-04-27 05:56:27.000000 meent-0.9.1/meent/nk_data/matlab/p_Si.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_jax/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_jax/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_jax/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_numpy/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_numpy/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.059154 meent-0.9.1/meent/on_torch/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28821 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.059154 meent-0.9.1/meent/on_torch/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.059154 meent-0.9.1/meent/on_torch/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.051154 meent-0.9.1/meent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-27 05:56:38.000000 meent-0.9.1/meent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-27 05:56:38.000000 meent-0.9.1/meent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 05:56:38.000000 meent-0.9.1/meent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 05:56:38.000000 meent-0.9.1/meent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 05:56:38.000000 meent-0.9.1/meent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 05:56:38.059154 meent-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-27 05:56:27.000000 meent-0.9.1/setup.py
```

### Comparing `meent-0.9.0/LICENSE` & `meent-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/README.md` & `meent-0.9.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-<p align="center"><img src="images/meent_logo.svg" width=80% /></p>
+[//]: # (<p align="center"><img src="images/meent_logo.svg" width=80% /></p>)
+<p align="center"><img src="images/meent_logo.png" width=50% /></p>
 
 # Meent
 
 [//]: # ([![GitHub license]&#40;https://badgen.net/github/license/Naereen/Strapdown.js&#41;]&#40;https://github.com/Naereen/StrapDown.js/blob/master/LICENSE&#41;)
 
 Meent is an Electromagnetic(EM) simulation package with Python, composed of three main parts:
 * Modeling
@@ -59,15 +60,27 @@
 # backend 1 = JAX
 # backend 2 = PyTorch
 
 backend = 1
 mee = meent.call_mee(backend=backend, ...)
 ```
 ## Tutorials
-Jupyter notebooks are prepared in [examples](examples) to give a (very) brief introduction.
+Jupyter notebooks are prepared in [tutorials](tutorials) to give a brief introduction.
+
+## Citation
+To cite this repository:
+
+```
+@software{Kim_Meent_Electromagnetic_simulation,
+  author = {Kim, Yongha and Kim, Sanmun and Lee, Jinmyoung and Jeong, Anthony Wonseok and Kim, Seolho},
+  license = {MIT},
+  title = {{Meent:Electromagnetic simulation & optimization package in Python}},
+  url = {https://github.com/kc-ml2/meent}
+}
+```
 
 ## Reference
 Will be updated.
 
 [1] https://opg.optica.org/josa/abstract.cfm?uri=josa-71-7-811, Rigorous coupled-wave analysis of planar-grating diffraction \
 [2] https://opg.optica.org/josaa/abstract.cfm?uri=josaa-12-5-1068 \
 [3] https://opg.optica.org/josaa/abstract.cfm?uri=josaa-12-5-1077 \
```

### Comparing `meent-0.9.0/meent/main.py` & `meent-0.9.1/meent/main.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/nk_data/filmetrics/Al2O3.txt` & `meent-0.9.1/meent/nk_data/filmetrics/Al2O3.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/nk_data/filmetrics/Si.txt` & `meent-0.9.1/meent/nk_data/filmetrics/Si.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/nk_data/filmetrics/Si3N4.txt` & `meent-0.9.1/meent/nk_data/filmetrics/Si3N4.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/nk_data/filmetrics/SiO2.txt` & `meent-0.9.1/meent/nk_data/filmetrics/SiO2.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/nk_data/matlab/p_Si.mat` & `meent-0.9.1/meent/nk_data/matlab/p_Si.mat`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_jax/emsolver/_base.py` & `meent-0.9.1/meent/on_jax/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_jax/emsolver/convolution_matrix.py` & `meent-0.9.1/meent/on_jax/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_jax/emsolver/field_distribution.py` & `meent-0.9.1/meent/on_jax/emsolver/field_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -929,15 +929,15 @@
 
 
 def field_plot(field_cell, pol=0, plot_indices=(1, 1, 1, 1, 1, 1), y_slice=0, z_slice=-1, zx=True, yx=True):
     try:
         import matplotlib.pyplot as plt
     except (ImportError, ModuleNotFoundError) as e:
         print(e)
-        print('To use field_plot(), please install matplotlib')
+        print('To use cal_field(), please install matplotlib')
         raise e
 
     if field_cell.shape[-1] == 6:  # 2D grating
         title = ['2D Ex', '2D Ey', '2D Ez', '2D Hx', '2D Hy', '2D Hz', ]
     else:  # 1D grating
         if pol == 0:  # TE
             title = ['1D Ey', '1D Hx', '1D Hz', ]
```

### Comparing `meent-0.9.0/meent/on_jax/emsolver/primitives.py` & `meent-0.9.1/meent/on_jax/emsolver/primitives.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import jax.numpy as jnp
 
 from functools import partial
 
 
 def conj(arr):
     return arr.real + arr.imag * -1j
-    # return arr.conj()
+    # return arr.conj()  # TODO: this bug will be fixed. replace.
 
 
 @partial(jax.custom_vjp, nondiff_argnums=(1, 2, 3))
 def eig(x, type_complex=jnp.complex128, perturbation=1E-10, device='cpu'):
 
     _eig = jax.jit(jnp.linalg.eig, device=jax.devices('cpu')[0])
 
@@ -29,16 +29,17 @@
 def eig_fwd(x, type_complex, perturbation, device):
     return eig(x, type_complex, perturbation), (eig(x, type_complex, perturbation), x)
 
 
 def eig_bwd(type_complex, perturbation, device, res, g):
     """
     Gradient of a general square (complex valued) matrix
-    Eq. 30~32 in https://www.sciencedirect.com/science/article/abs/pii/S0010465522002715
+    Eq 2~5 in https://www.nature.com/articles/s42005-021-00568-6
     Eq 4.77 in https://arxiv.org/pdf/1701.00392.pdf
+    Eq. 30~32 in https://www.sciencedirect.com/science/article/abs/pii/S0010465522002715
     https://github.com/kch3782/torcwa
     https://github.com/weiliangjinca/grcwa
     https://github.com/pytorch/pytorch/issues/41857
     https://jax.readthedocs.io/en/latest/notebooks/autodiff_cookbook.html#Complex-numbers-and-differentiation
     https://discuss.pytorch.org/t/autograd-on-complex-numbers/144687/3
     """
```

### Comparing `meent-0.9.0/meent/on_jax/emsolver/rcwa.py` & `meent-0.9.1/meent/on_jax/emsolver/rcwa.py`

 * *Files 18% similar despite different names*

```diff
@@ -145,55 +145,19 @@
         de_ri, de_ti, layer_info_list, T1, kx_vector = self._solve(self.wavelength, E_conv_all, o_E_conv_all)
         return de_ri, de_ti, layer_info_list, T1, kx_vector
 
     @jax.jit
     def _conv_solve_jit(self):
         return self._conv_solve()
 
-    # @jax.jit
-    # def _conv_solve_jit(self):
-    #
-    #     if self.fft_type == 0:
-    #         E_conv_all, o_E_conv_all = to_conv_mat_discrete(self.ucell, self.fourier_order[0], self.fourier_order[1],
-    #                                                         type_complex=self.type_complex,
-    #                                                         improve_dft=self.improve_dft)
-    #     elif self.fft_type == 1:
-    #         E_conv_all, o_E_conv_all = to_conv_mat_continuous(self.ucell, self.fourier_order[0], self.fourier_order[1],
-    #                                                           type_complex=self.type_complex)
-    #     elif self.fft_type == 2:
-    #         E_conv_all, o_E_conv_all = to_conv_mat_continuous_vector(self.ucell_info_list,
-    #                                                                  self.fourier_order[0], self.fourier_order[1],
-    #                                                                  type_complex=self.type_complex)
-    #     else:
-    #         raise ValueError
-    #
-    #     de_ri, de_ti, layer_info_list, T1, kx_vector = self._solve(self.wavelength, E_conv_all, o_E_conv_all)
-    #     return de_ri, de_ti, layer_info_list, T1, kx_vector
-
-    # @jax.jit
-    # def _conv_solve_jit_discrete(self):
-    #     E_conv_all, o_E_conv_all = to_conv_mat_discrete(self.ucell, self.fourier_order[0], self.fourier_order[1],
-    #                                                     type_complex=self.type_complex,
-    #                                                     improve_dft=self.improve_dft)
-    #     de_ri, de_ti, layer_info_list, T1, kx_vector = self._solve(self.wavelength, E_conv_all, o_E_conv_all)
-    #     return de_ri, de_ti, layer_info_list, T1, kx_vector
-    #
-    # @jax.jit
-    # def _conv_solve_jit_cont_vector(self):
-    #     E_conv_all, o_E_conv_all = to_conv_mat_continuous_vector(self.ucell_info_list,
-    #                                                              self.fourier_order[0], self.fourier_order[1],
-    #                                                              type_complex=self.type_complex)
-    #     de_ri, de_ti, layer_info_list, T1, kx_vector = self._solve(self.wavelength, E_conv_all, o_E_conv_all)
-    #     return de_ri, de_ti, layer_info_list, T1, kx_vector
-
     @_BaseRCWA.jax_device_set
     def conv_solve(self, **kwargs):
         [setattr(self, k, v) for k, v in kwargs.items()]  # needed for optimization
         if self.fft_type == 1:
-            print('CFT (fft_type=1) is not supported for jit-compilation. Using non-jit-compiled method.')
+            # print('CFT (fft_type=1) is not supported for jit-compilation. Using non-jit-compiled method.')
             de_ri, de_ti, layer_info_list, T1, kx_vector = self._conv_solve()
 
         else:
             de_ri, de_ti, layer_info_list, T1, kx_vector = self._conv_solve_jit()
 
         self.layer_info_list = layer_info_list
         self.T1 = T1
@@ -201,15 +165,15 @@
 
         return de_ri, de_ti
 
     @_BaseRCWA.jax_device_set
     def calculate_field(self, res_x=20, res_y=20, res_z=20, field_algo=2):
 
         if self.grating_type == 0:
-
+            res_y = 1
             if field_algo == 0:
                 field_cell = field_dist_1d_vanilla(self.wavelength, self.kx_vector,
                                                    self.T1, self.layer_info_list, self.period, self.pol,
                                                    res_x=res_x, res_y=res_y, res_z=res_z,
                                                    type_complex=self.type_complex)
             elif field_algo == 1:
                 field_cell = field_dist_1d_vectorized_ji(self.wavelength, self.kx_vector, self.T1, self.layer_info_list,
@@ -220,15 +184,15 @@
                                                           self.layer_info_list, self.period, self.pol,
                                                           res_x=res_x, res_y=res_y, res_z=res_z,
                                                           type_complex=self.type_complex, type_float=self.type_float)
             else:
                 raise ValueError
 
         elif self.grating_type == 1:
-
+            res_y = 1
             if field_algo == 0:
                 field_cell = field_dist_1d_conical_vanilla(self.wavelength, self.kx_vector, self.n_I, self.theta,
                                                            self.phi, self.T1, self.layer_info_list, self.period,
                                                            res_x=res_x, res_y=res_y, res_z=res_z,
                                                            type_complex=self.type_complex)
             elif field_algo == 1:
                 field_cell = field_dist_1d_conical_vectorized_ji(self.wavelength, self.kx_vector, self.n_I, self.theta,
```

### Comparing `meent-0.9.0/meent/on_jax/emsolver/scattering_method.py` & `meent-0.9.1/meent/on_jax/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_jax/emsolver/smm_util.py` & `meent-0.9.1/meent/on_jax/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_jax/emsolver/transfer_method.py` & `meent-0.9.1/meent/on_jax/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_jax/mee.py` & `meent-0.9.1/meent/on_jax/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_jax/modeler/modeling.py` & `meent-0.9.1/meent/on_jax/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_jax/optimizer/loss.py` & `meent-0.9.1/meent/on_jax/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_jax/optimizer/optimizer.py` & `meent-0.9.1/meent/on_jax/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_numpy/emsolver/_base.py` & `meent-0.9.1/meent/on_numpy/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_numpy/emsolver/convolution_matrix.py` & `meent-0.9.1/meent/on_numpy/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_numpy/emsolver/field_distribution.py` & `meent-0.9.1/meent/on_numpy/emsolver/field_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -639,15 +639,15 @@
 
 
 def field_plot(field_cell, pol=0, plot_indices=(1, 1, 1, 1, 1, 1), y_slice=0, z_slice=-1, zx=True, yx=True):
     try:
         import matplotlib.pyplot as plt
     except (ImportError, ModuleNotFoundError) as e:
         print(e)
-        print('To use field_plot(), please install matplotlib')
+        print('To use cal_field(), please install matplotlib')
         raise e
 
     if field_cell.shape[-1] == 6:  # 2D grating
         title = ['2D Ex', '2D Ey', '2D Ez', '2D Hx', '2D Hy', '2D Hz', ]
     else:  # 1D grating
         if pol == 0:  # TE
             title = ['1D Ey', '1D Hx', '1D Hz', ]
```

### Comparing `meent-0.9.0/meent/on_numpy/emsolver/rcwa.py` & `meent-0.9.1/meent/on_numpy/emsolver/rcwa.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         self.T1 = T1
         self.kx_vector = kx_vector
 
         return de_ri, de_ti
 
     def calculate_field(self, res_x=20, res_y=20, res_z=20, field_algo=2):
         if self.grating_type == 0:
+            res_y = 1
             if field_algo == 0:
                 field_cell = field_dist_1d_vanilla(self.wavelength, self.kx_vector,
                                                    self.T1, self.layer_info_list, self.period, self.pol,
                                                    res_x=res_x, res_y=res_y, res_z=res_z, type_complex=self.type_complex)
             elif field_algo == 1:
                 field_cell = field_dist_1d_vectorized_ji(self.wavelength, self.kx_vector, self.T1, self.layer_info_list,
                                                          self.period, self.pol, res_x=res_x, res_y=res_y, res_z=res_z,
@@ -127,14 +128,15 @@
             elif field_algo == 2:
                 field_cell = field_dist_1d_vectorized_kji(self.wavelength, self.kx_vector, self.T1,
                                                           self.layer_info_list, self.period, self.pol,
                                                           res_x=res_x, res_y=res_y, res_z=res_z, type_complex=self.type_complex)
             else:
                 raise ValueError
         elif self.grating_type == 1:
+            res_y = 1
             if field_algo == 0:
                 field_cell = field_dist_1d_conical_vanilla(self.wavelength, self.kx_vector, self.n_I, self.theta,
                                                            self.phi, self.T1, self.layer_info_list, self.period,
                                                            res_x=res_x, res_y=res_y, res_z=res_z, type_complex=self.type_complex)
             elif field_algo == 1:
                 field_cell = field_dist_1d_conical_vectorized_ji(self.wavelength, self.kx_vector, self.n_I, self.theta,
                                                                  self.phi, self.T1, self.layer_info_list, self.period,
```

### Comparing `meent-0.9.0/meent/on_numpy/emsolver/scattering_method.py` & `meent-0.9.1/meent/on_numpy/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_numpy/emsolver/smm_util.py` & `meent-0.9.1/meent/on_numpy/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_numpy/emsolver/transfer_method.py` & `meent-0.9.1/meent/on_numpy/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_numpy/mee.py` & `meent-0.9.1/meent/on_numpy/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_numpy/modeler/modeling.py` & `meent-0.9.1/meent/on_numpy/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_torch/emsolver/_base.py` & `meent-0.9.1/meent/on_torch/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_torch/emsolver/convolution_matrix.py` & `meent-0.9.1/meent/on_torch/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_torch/emsolver/field_distribution.py` & `meent-0.9.1/meent/on_torch/emsolver/field_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,15 +637,15 @@
 
 
 def field_plot(field_cell, pol=0, plot_indices=(1, 1, 1, 1, 1, 1), y_slice=0, z_slice=-1, zx=True, yx=True):
     try:
         import matplotlib.pyplot as plt
     except (ImportError, ModuleNotFoundError) as e:
         print(e)
-        print('To use field_plot(), please install matplotlib')
+        print('To use cal_field(), please install matplotlib')
         raise e
 
     if field_cell.shape[-1] == 6:  # 2D grating
         title = ['2D Ex', '2D Ey', '2D Ez', '2D Hx', '2D Hy', '2D Hz', ]
     else:  # 1D grating
         if pol == 0:  # TE
             title = ['1D Ey', '1D Hx', '1D Hz', ]
```

### Comparing `meent-0.9.0/meent/on_torch/emsolver/primitives.py` & `meent-0.9.1/meent/on_torch/emsolver/primitives.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,17 @@
         eigval, eigvec = output
         ctx.save_for_backward(matrix, eigval, eigvec)
 
     @staticmethod
     def backward(ctx, grad_eigval, grad_eigvec):
         """
         Gradient of a general square (complex valued) matrix
-        Eq. 30~32 in https://www.sciencedirect.com/science/article/abs/pii/S0010465522002715
+        Eq 2~5 in https://www.nature.com/articles/s42005-021-00568-6
         Eq 4.77 in https://arxiv.org/pdf/1701.00392.pdf
+        Eq. 30~32 in https://www.sciencedirect.com/science/article/abs/pii/S0010465522002715
         https://github.com/kch3782/torcwa
         https://github.com/weiliangjinca/grcwa
         https://github.com/pytorch/pytorch/issues/41857
         https://discuss.pytorch.org/t/autograd-on-complex-numbers/144687/3
         """
 
         matrix, eig_val, eig_vector = ctx.saved_tensors
```

### Comparing `meent-0.9.0/meent/on_torch/emsolver/rcwa.py` & `meent-0.9.1/meent/on_torch/emsolver/rcwa.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,16 @@
         self.layer_info_list = layer_info_list
         self.T1 = T1
         self.kx_vector = kx_vector
 
         return de_ri, de_ti
 
     def calculate_field(self, res_x=20, res_y=20, res_z=20, field_algo=2):
-
         if self.grating_type == 0:
+            res_y = 1
             if field_algo == 0:
                 field_cell = field_dist_1d_vanilla(self.wavelength, self.kx_vector,
                                                    self.T1, self.layer_info_list, self.period, self.pol,
                                                    res_x=res_x, res_y=res_y, res_z=res_z,
                                                    type_complex=self.type_complex)
             elif field_algo == 1:
                 field_cell = field_dist_1d_vectorized_ji(self.wavelength, self.kx_vector, self.T1, self.layer_info_list,
@@ -141,16 +141,16 @@
                 field_cell = field_dist_1d_vectorized_kji(self.wavelength, self.kx_vector, self.T1,
                                                           self.layer_info_list, self.period, self.pol,
                                                           res_x=res_x, res_y=res_y, res_z=res_z,
                                                           type_complex=self.type_complex,
                                                           type_float=self.type_float)
             else:
                 raise ValueError
-
         elif self.grating_type == 1:
+            res_y = 1
             if field_algo == 0:
                 field_cell = field_dist_1d_conical_vanilla(self.wavelength, self.kx_vector, self.n_I, self.theta,
                                                            self.phi, self.T1, self.layer_info_list, self.period,
                                                            res_x=res_x, res_y=res_y, res_z=res_z, device=self.device,
                                                            type_complex=self.type_complex)
             elif field_algo == 1:
                 field_cell = field_dist_1d_conical_vectorized_ji(self.wavelength, self.kx_vector, self.n_I, self.theta,
```

### Comparing `meent-0.9.0/meent/on_torch/emsolver/scattering_method.py` & `meent-0.9.1/meent/on_torch/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_torch/emsolver/smm_util.py` & `meent-0.9.1/meent/on_torch/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_torch/emsolver/transfer_method.py` & `meent-0.9.1/meent/on_torch/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_torch/modeler/modeling.py` & `meent-0.9.1/meent/on_torch/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_torch/optimizer/loss.py` & `meent-0.9.1/meent/on_torch/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent/on_torch/optimizer/optimizer.py` & `meent-0.9.1/meent/on_torch/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.0/meent.egg-info/SOURCES.txt` & `meent-0.9.1/meent.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 setup.py
 meent/__init__.py
 meent/main.py
-meent/testcase.py
 meent.egg-info/PKG-INFO
 meent.egg-info/SOURCES.txt
 meent.egg-info/dependency_links.txt
 meent.egg-info/requires.txt
 meent.egg-info/top_level.txt
 meent/nk_data/filmetrics/Al2O3.txt
 meent/nk_data/filmetrics/Si.txt
```

### Comparing `meent-0.9.0/setup.py` & `meent-0.9.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             ],
     'pytorch': ['torch>=2.0.0',
                 'tqdm>=4.64.1',
                 ],
 }
 setup(
     name='meent',
-    version='0.9.0',
+    version='0.9.1',
     url='https://github.com/kc-ml2/meent',
     author='KC ML2',
     author_email='yongha@kc-ml2.com',
     packages=['meent'] + find_packages(include=['meent.*']),
     install_requires=[
         'numpy>=1.23.3',
         'scipy>=1.9.1',
```


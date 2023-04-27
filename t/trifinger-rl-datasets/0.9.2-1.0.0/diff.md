# Comparing `tmp/trifinger_rl_datasets-0.9.2.tar.gz` & `tmp/trifinger_rl_datasets-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trifinger_rl_datasets-0.9.2.tar", last modified: Wed Mar 29 14:28:31 2023, max compression
+gzip compressed data, was "trifinger_rl_datasets-1.0.0.tar", last modified: Thu Apr 27 13:48:26 2023, max compression
```

## Comparing `trifinger_rl_datasets-0.9.2.tar` & `trifinger_rl_datasets-1.0.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-03-29 14:28:31.055894 trifinger_rl_datasets-0.9.2/
--rw-rw-r--   0 nguertler  (7419) is        (1040)     1532 2022-09-07 07:59:18.000000 trifinger_rl_datasets-0.9.2/LICENSE
--rw-r--r--   0 nguertler  (7419) is        (1040)     6257 2023-03-29 14:28:31.056894 trifinger_rl_datasets-0.9.2/PKG-INFO
--rw-r--r--   0 nguertler  (7419) is        (1040)     4958 2023-01-20 15:23:15.000000 trifinger_rl_datasets-0.9.2/README.md
--rw-rw-r--   0 nguertler  (7419) is        (1040)      142 2022-09-07 07:59:18.000000 trifinger_rl_datasets-0.9.2/pyproject.toml
--rw-r--r--   0 nguertler  (7419) is        (1040)      784 2023-03-29 14:28:31.059911 trifinger_rl_datasets-0.9.2/setup.cfg
--rw-r--r--   0 nguertler  (7419) is        (1040)       38 2023-03-23 14:08:48.000000 trifinger_rl_datasets-0.9.2/setup.py
-drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-03-29 14:28:30.874899 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/
--rw-r--r--   0 nguertler  (7419) is        (1040)     1693 2023-03-29 14:28:07.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/__init__.py
-drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-03-29 14:28:31.010902 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/
--rw-r--r--   0 nguertler  (7419) is        (1040)        0 2023-01-20 15:23:15.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/__init__.py
--rw-r--r--   0 nguertler  (7419) is        (1040)     1170 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r1_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1176 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r1_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1177 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r1_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r3_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1172 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r3_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r3_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1178 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r4_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1178 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r4_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1169 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r4_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1188 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r5_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1177 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r5_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r5_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1184 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r6_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1173 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r6_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1167 2023-02-20 18:18:55.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r6_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:56.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r7_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:56.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r7_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1174 2023-02-20 18:18:56.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r7_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:56.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r8_camera180.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1176 2023-02-20 18:18:56.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r8_camera300.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)     1171 2023-02-20 18:18:56.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r8_camera60.yml
--rw-r--r--   0 nguertler  (7419) is        (1040)  1556408 2023-01-20 15:23:15.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/trifingerpro_shuffle_cube_trajectory_fast.npy
--rw-r--r--   0 nguertler  (7419) is        (1040)    38177 2023-03-29 11:06:03.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/dataset_env.py
--rw-r--r--   0 nguertler  (7419) is        (1040)     3104 2023-03-23 14:08:48.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/evaluate_sim.py
--rw-r--r--   0 nguertler  (7419) is        (1040)     3139 2023-03-23 14:08:48.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/evaluation.py
--rw-r--r--   0 nguertler  (7419) is        (1040)     2067 2023-03-23 14:08:48.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/policy_base.py
--rw-r--r--   0 nguertler  (7419) is        (1040)        0 2023-01-20 15:23:15.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/py.typed
--rw-r--r--   0 nguertler  (7419) is        (1040)     1673 2023-01-20 15:23:15.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/sampling_utils.py
--rw-r--r--   0 nguertler  (7419) is        (1040)    27152 2023-03-29 13:37:09.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/sim_env.py
--rw-r--r--   0 nguertler  (7419) is        (1040)     2743 2023-01-20 15:23:15.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/utils.py
-drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-03-29 14:28:30.891904 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets.egg-info/
--rw-r--r--   0 nguertler  (7419) is        (1040)     6257 2023-03-29 14:28:30.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets.egg-info/PKG-INFO
--rw-r--r--   0 nguertler  (7419) is        (1040)     1621 2023-03-29 14:28:30.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 nguertler  (7419) is        (1040)        1 2023-03-29 14:28:30.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 nguertler  (7419) is        (1040)       90 2023-03-29 14:28:30.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets.egg-info/requires.txt
--rw-r--r--   0 nguertler  (7419) is        (1040)       22 2023-03-29 14:28:30.000000 trifinger_rl_datasets-0.9.2/trifinger_rl_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-04-27 13:48:26.442073 trifinger_rl_datasets-1.0.0/
+-rw-rw-r--   0 nguertler  (7419) is        (1040)     1532 2022-09-07 07:59:18.000000 trifinger_rl_datasets-1.0.0/LICENSE
+-rw-r--r--   0 nguertler  (7419) is        (1040)     6702 2023-04-27 13:48:26.443076 trifinger_rl_datasets-1.0.0/PKG-INFO
+-rw-r--r--   0 nguertler  (7419) is        (1040)     5307 2023-04-27 13:43:01.000000 trifinger_rl_datasets-1.0.0/README.md
+-rw-rw-r--   0 nguertler  (7419) is        (1040)      142 2022-09-07 07:59:18.000000 trifinger_rl_datasets-1.0.0/pyproject.toml
+-rw-r--r--   0 nguertler  (7419) is        (1040)      784 2023-04-27 13:48:26.446081 trifinger_rl_datasets-1.0.0/setup.cfg
+-rw-r--r--   0 nguertler  (7419) is        (1040)       38 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.0/setup.py
+drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-04-27 13:48:26.297082 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/
+-rw-r--r--   0 nguertler  (7419) is        (1040)     3236 2023-04-27 13:47:58.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/__init__.py
+drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-04-27 13:48:26.416080 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/
+-rw-r--r--   0 nguertler  (7419) is        (1040)        0 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/__init__.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1170 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1176 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1177 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1172 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1178 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1178 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1169 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1188 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1177 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1184 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1173 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1167 2023-02-20 18:18:55.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1175 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1174 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1180 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera180.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1176 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera300.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1171 2023-02-20 18:18:56.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera60.yml
+-rw-r--r--   0 nguertler  (7419) is        (1040)  1556408 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/trifingerpro_shuffle_cube_trajectory_fast.npy
+-rw-r--r--   0 nguertler  (7419) is        (1040)    39661 2023-04-27 11:37:43.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/dataset_env.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)     3104 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/evaluate_sim.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)     3139 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/evaluation.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)     2067 2023-03-23 14:08:48.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/policy_base.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)        0 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/py.typed
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1673 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/sampling_utils.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)    27363 2023-04-26 16:31:32.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/sim_env.py
+-rw-r--r--   0 nguertler  (7419) is        (1040)     2743 2023-01-20 15:23:15.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/utils.py
+drwxr-xr-x   0 nguertler  (7419) is        (1040)        0 2023-04-27 13:48:26.314081 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/
+-rw-r--r--   0 nguertler  (7419) is        (1040)     6702 2023-04-27 13:48:26.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 nguertler  (7419) is        (1040)     1621 2023-04-27 13:48:26.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 nguertler  (7419) is        (1040)        1 2023-04-27 13:48:26.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 nguertler  (7419) is        (1040)       90 2023-04-27 13:48:26.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/requires.txt
+-rw-r--r--   0 nguertler  (7419) is        (1040)       22 2023-04-27 13:48:26.000000 trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/top_level.txt
```

### Comparing `trifinger_rl_datasets-0.9.2/LICENSE` & `trifinger_rl_datasets-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/PKG-INFO` & `trifinger_rl_datasets-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,116 +1,128 @@
 Metadata-Version: 2.1
 Name: trifinger_rl_datasets
-Version: 0.9.2
+Version: 1.0.0
 Summary: Gym environments which provide offline RL datasets collected on the TriFinger system.
 Home-page: UNKNOWN
 Author: Nico Gürtler
 Author-email: nico.guertler@tuebingen.mpg.de
 License: BSD 3-Clause
 Description: # TriFinger RL Datasets
         
-        This repository provides offline reinforcement learning datasets collected on the TriFinger platform (simulated or real). The paper "Benchmarking Offline Reinforcement Learning on Real-Robot Hardware" (TODO: Link) discusses the datasets and benchmarks offline reinforcement learning methods on them. The code for loading the datasets follows the interface suggested by [D4RL](https://github.com/rail-berkeley/d4rl). 
+        This repository provides offline reinforcement learning datasets collected on the real TriFinger platform and in a simulated version of the environment. The paper ["Benchmarking Offline Reinforcement Learning on Real-Robot Hardware"](https://openreview.net/pdf?id=3k5CUGDLNdd) provides more details on the datasets and benchmarks offline RL algorithms on them. All datasets are available with camera images as well.
         
-        TODO: Link to documentation.
-        TODO: Prominently mention (and repeat later on) that the repository also provides versions of the datasets with image observations from three cameras.
+        More detailed information about the simulated environment, the datasets and on how to run experiments on a cluster of real TriFinger robots can be found in the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/).
         
         Some of the datasets were used during the [Real Robot Challenge 2022](https://real-robot-challenge.com).
         
         ## Installation
         
         To install the package run with python 3.8 in the root directory of the repository (we recommend doing this in a virtual environment):
         
         ```bash
-        pip install --upgrade pip  # make sure recent version of pip is installed
+        pip install --upgrade pip  # make sure the most recent version of pip is installed
         pip install .
         ```
         
         ## Usage
         
-        ### Loading the dataset
+        This section provides short examples of how to load datasets and evaluate a policy in simulation. More details on how to work with the datasets can be found in the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/).
         
-        The datasets are accessible via gym environments which are automatically registered when importing the package. They are automatically downloaded when requested and stored in `~/.trifinger_rl_datasets` as HDF5 files.
         
-        The datasets are named following the pattern `trifinger-cube-task-source-quality-v0` where `task` is either `push` or `lift`, `source` is either `sim` or `real` and `quality` can be either `mixed` or `expert`.
+        ### Loading a dataset
+        
+        The datasets are accessible via gym environments which are automatically registered when importing the package. They are automatically downloaded when requested and stored in `~/.trifinger_rl_datasets` as Zarr files by default (see the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/) for custom paths to the datasets). The code for loading the datasets follows the interface suggested by [D4RL](https://github.com/rail-berkeley/d4rl) and extends it where needed. 
+        
+        The datasets are named following the pattern `trifinger-cube-task-source-type-v0` where `task` is either `push` or `lift`, `source` is either `sim` or `real` and `type` can be either `mixed`, `weak-n-expert` or `expert`.
         
         By default the observations are loaded as flat arrays. For the simulated datasets the environment can be stepped and visualized. Example usage (also see `demo/load_dataset.py`):
         
         ```python
         import gymnasium as gym
         
         import trifinger_rl_datasets
         
         env = gym.make(
             "trifinger-cube-push-sim-expert-v0",
-            disable_env_checker=True,
             visualization=True,  # enable visualization
         )
         
         dataset = env.get_dataset()
         
         print("First observation: ", dataset["observations"][0])
         print("First action: ", dataset["actions"][0])
         print("First reward: ", dataset["rewards"][0])
         
-        obs = env.reset()
-        done = False
-        while not done:
-            obs, rew, done, info = env.step(env.action_space.sample())
+        obs, info = env.reset()
+        truncated = False
+        
+        while not truncated:
+            obs, rew, terminated, truncated, info = env.step(env.action_space.sample())
         ```
         
         Alternatively, the observations can be obtained as nested dictionaries. This simplifies working with the data. As some parts of the observations might be more useful than others, it is also possible to filter the observations when requesting dictionaries (see `demo/load_filtered_dicts.py`):
+        
         ```python
             # Nested dictionary defines which observations to keep.
             # Everything that is not included or has value False
             # will be dropped.
             obs_to_keep = {
                 "robot_observation": {
                     "position": True,
                     "velocity": True,
                     "fingertip_force": False,
                 },
                 "object_observation": {"keypoints": True},
             }
             env = gym.make(
                 args.env_name,
-                disable_env_checker=True,
                 # filter observations,
                 obs_to_keep=obs_to_keep,
             )
         ```
-        To transform the observation back to a flat array after filtering, simply set the keyword argument `flatten_obs` to true. Note that the step and reset functions will transform observations in the same manner as the `get_dataset` method to ensure compatibility. A downside of working with observations in the form of dictionaries is that they cause a considerable memory overhead during dataset loading.
         
         All datasets come in two versions: with and without camera observations. The versions with camera observations contain `-image` in their name. Despite PNG image compression they are more than one order of magnitude bigger than the imageless versions. To avoid running out of memory, a part of a dataset can be loaded by specifying a range of timesteps:
+        
         ```python
         env = gym.make(
             "trifinger-cube-push-real-expert-image-v0",
             disable_env_checker=True
         )
         
         # load only a subset of obervations, actions and rewards
         dataset = env.get_dataset(rng=(1000, 2000))
         ```
+        
         The camera observations corresponding to this range are then returned in `dataset["images"]` with the following dimensions:
+        
         ```python
         n_timesteps, n_cameras, n_channels, height, width = dataset["images"].shape
         ```
-        Since the camera frequency is lower than the control frequency, a camera image will repeat over several time steps. To load an array of camera images without this redundancy, the `get_image_data` method can be used:
-        ```python
-        # images from 3 cameras for each timestep
-        image_stats = env.get_image_stats()
-        n_cameras = image_stats["n_cameras"]
-        images = env.get_image_data(rng=(0, n_cameras * n_camera_frames_to_load)) 
-        ```
         
         ### Evaluating a policy in simulation
         
         This package contains an executable module `trifinger_rl_datasets.evaluate_sim`, which
         can be used to evaluate a policy in simulation.  As arguments it expects the task
         ("push" or "lift") and a Python class that implements the policy, following the
         `PolicyBase` interface:
         
             python3 -m trifinger_rl_datasets.evaluate_sim push my_package.MyPolicy
         
         For more options see `--help`.
+        
+        ## How to cite
+        
+        The paper ["Benchmarking Offline Reinforcement Learning on Real-Robot Hardware"](https://openreview.net/pdf?id=3k5CUGDLNdd) introducing the datasets was published at ICLR 2023:
+        
+        ```
+        @inproceedings{
+        guertler2023benchmarking,
+        title={Benchmarking Offline Reinforcement Learning on Real-Robot Hardware},
+        author={Nico G{\"u}rtler and Sebastian Blaes and Pavel Kolev and Felix Widmaier and Manuel Wuthrich and Stefan Bauer and Bernhard Sch{\"o}lkopf and Georg Martius},
+        booktitle={The Eleventh International Conference on Learning Representations },
+        year={2023},
+        url={https://openreview.net/forum?id=3k5CUGDLNdd}
+        }
+        ```
 Keywords: offline reinforcement learning,reinforcement learning,robotics,TriFinger,Real Robot Challenge,dexterous manipulation
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `trifinger_rl_datasets-0.9.2/README.md` & `trifinger_rl_datasets-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,117 @@
 # TriFinger RL Datasets
 
-This repository provides offline reinforcement learning datasets collected on the TriFinger platform (simulated or real). The paper "Benchmarking Offline Reinforcement Learning on Real-Robot Hardware" (TODO: Link) discusses the datasets and benchmarks offline reinforcement learning methods on them. The code for loading the datasets follows the interface suggested by [D4RL](https://github.com/rail-berkeley/d4rl). 
+This repository provides offline reinforcement learning datasets collected on the real TriFinger platform and in a simulated version of the environment. The paper ["Benchmarking Offline Reinforcement Learning on Real-Robot Hardware"](https://openreview.net/pdf?id=3k5CUGDLNdd) provides more details on the datasets and benchmarks offline RL algorithms on them. All datasets are available with camera images as well.
 
-TODO: Link to documentation.
-TODO: Prominently mention (and repeat later on) that the repository also provides versions of the datasets with image observations from three cameras.
+More detailed information about the simulated environment, the datasets and on how to run experiments on a cluster of real TriFinger robots can be found in the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/).
 
 Some of the datasets were used during the [Real Robot Challenge 2022](https://real-robot-challenge.com).
 
 ## Installation
 
 To install the package run with python 3.8 in the root directory of the repository (we recommend doing this in a virtual environment):
 
 ```bash
-pip install --upgrade pip  # make sure recent version of pip is installed
+pip install --upgrade pip  # make sure the most recent version of pip is installed
 pip install .
 ```
 
 ## Usage
 
-### Loading the dataset
+This section provides short examples of how to load datasets and evaluate a policy in simulation. More details on how to work with the datasets can be found in the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/).
 
-The datasets are accessible via gym environments which are automatically registered when importing the package. They are automatically downloaded when requested and stored in `~/.trifinger_rl_datasets` as HDF5 files.
 
-The datasets are named following the pattern `trifinger-cube-task-source-quality-v0` where `task` is either `push` or `lift`, `source` is either `sim` or `real` and `quality` can be either `mixed` or `expert`.
+### Loading a dataset
+
+The datasets are accessible via gym environments which are automatically registered when importing the package. They are automatically downloaded when requested and stored in `~/.trifinger_rl_datasets` as Zarr files by default (see the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/) for custom paths to the datasets). The code for loading the datasets follows the interface suggested by [D4RL](https://github.com/rail-berkeley/d4rl) and extends it where needed. 
+
+The datasets are named following the pattern `trifinger-cube-task-source-type-v0` where `task` is either `push` or `lift`, `source` is either `sim` or `real` and `type` can be either `mixed`, `weak-n-expert` or `expert`.
 
 By default the observations are loaded as flat arrays. For the simulated datasets the environment can be stepped and visualized. Example usage (also see `demo/load_dataset.py`):
 
 ```python
 import gymnasium as gym
 
 import trifinger_rl_datasets
 
 env = gym.make(
     "trifinger-cube-push-sim-expert-v0",
-    disable_env_checker=True,
     visualization=True,  # enable visualization
 )
 
 dataset = env.get_dataset()
 
 print("First observation: ", dataset["observations"][0])
 print("First action: ", dataset["actions"][0])
 print("First reward: ", dataset["rewards"][0])
 
-obs = env.reset()
-done = False
-while not done:
-    obs, rew, done, info = env.step(env.action_space.sample())
+obs, info = env.reset()
+truncated = False
+
+while not truncated:
+    obs, rew, terminated, truncated, info = env.step(env.action_space.sample())
 ```
 
 Alternatively, the observations can be obtained as nested dictionaries. This simplifies working with the data. As some parts of the observations might be more useful than others, it is also possible to filter the observations when requesting dictionaries (see `demo/load_filtered_dicts.py`):
+
 ```python
     # Nested dictionary defines which observations to keep.
     # Everything that is not included or has value False
     # will be dropped.
     obs_to_keep = {
         "robot_observation": {
             "position": True,
             "velocity": True,
             "fingertip_force": False,
         },
         "object_observation": {"keypoints": True},
     }
     env = gym.make(
         args.env_name,
-        disable_env_checker=True,
         # filter observations,
         obs_to_keep=obs_to_keep,
     )
 ```
-To transform the observation back to a flat array after filtering, simply set the keyword argument `flatten_obs` to true. Note that the step and reset functions will transform observations in the same manner as the `get_dataset` method to ensure compatibility. A downside of working with observations in the form of dictionaries is that they cause a considerable memory overhead during dataset loading.
 
 All datasets come in two versions: with and without camera observations. The versions with camera observations contain `-image` in their name. Despite PNG image compression they are more than one order of magnitude bigger than the imageless versions. To avoid running out of memory, a part of a dataset can be loaded by specifying a range of timesteps:
+
 ```python
 env = gym.make(
     "trifinger-cube-push-real-expert-image-v0",
     disable_env_checker=True
 )
 
 # load only a subset of obervations, actions and rewards
 dataset = env.get_dataset(rng=(1000, 2000))
 ```
+
 The camera observations corresponding to this range are then returned in `dataset["images"]` with the following dimensions:
+
 ```python
 n_timesteps, n_cameras, n_channels, height, width = dataset["images"].shape
 ```
-Since the camera frequency is lower than the control frequency, a camera image will repeat over several time steps. To load an array of camera images without this redundancy, the `get_image_data` method can be used:
-```python
-# images from 3 cameras for each timestep
-image_stats = env.get_image_stats()
-n_cameras = image_stats["n_cameras"]
-images = env.get_image_data(rng=(0, n_cameras * n_camera_frames_to_load)) 
-```
 
 ### Evaluating a policy in simulation
 
 This package contains an executable module `trifinger_rl_datasets.evaluate_sim`, which
 can be used to evaluate a policy in simulation.  As arguments it expects the task
 ("push" or "lift") and a Python class that implements the policy, following the
 `PolicyBase` interface:
 
     python3 -m trifinger_rl_datasets.evaluate_sim push my_package.MyPolicy
 
-For more options see `--help`.
+For more options see `--help`.
+
+## How to cite
+
+The paper ["Benchmarking Offline Reinforcement Learning on Real-Robot Hardware"](https://openreview.net/pdf?id=3k5CUGDLNdd) introducing the datasets was published at ICLR 2023:
+
+```
+@inproceedings{
+guertler2023benchmarking,
+title={Benchmarking Offline Reinforcement Learning on Real-Robot Hardware},
+author={Nico G{\"u}rtler and Sebastian Blaes and Pavel Kolev and Felix Widmaier and Manuel Wuthrich and Stefan Bauer and Bernhard Sch{\"o}lkopf and Georg Martius},
+booktitle={The Eleventh International Conference on Learning Representations },
+year={2023},
+url={https://openreview.net/forum?id=3k5CUGDLNdd}
+}
+```
```

### Comparing `trifinger_rl_datasets-0.9.2/setup.cfg` & `trifinger_rl_datasets-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r1_camera180.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r1_camera300.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r1_camera60.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r1_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r3_camera180.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r3_camera300.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r3_camera60.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r3_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r4_camera180.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r4_camera300.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r4_camera60.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r4_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r5_camera180.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r5_camera300.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r5_camera60.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r5_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r6_camera180.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r6_camera300.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r6_camera60.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r6_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r7_camera180.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r7_camera300.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r7_camera60.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r7_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r8_camera180.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera180.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r8_camera300.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera300.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/r8_camera60.yml` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/r8_camera60.yml`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/data/trifingerpro_shuffle_cube_trajectory_fast.npy` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/data/trifingerpro_shuffle_cube_trajectory_fast.npy`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/dataset_env.py` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/dataset_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         self,
         name,
         dataset_url,
         ref_max_score,
         ref_min_score,
         trifinger_kwargs,
         real_robot=False,
-        image_obs=True,
+        image_obs=False,
         visualization=False,
         obs_to_keep=None,
         flatten_obs=True,
         scale_obs=False,
         set_terminals=False,
         data_dir=None,
         **kwargs,
@@ -187,30 +187,41 @@
 
         self.t_kwargs = deepcopy(trifinger_kwargs)
         self.t_kwargs["image_obs"] = image_obs
         self.t_kwargs["visualization"] = visualization
 
         # underlying simulated TriFinger environment
         self.sim_env = SimTriFingerCubeEnv(**self.t_kwargs)
-        self._orig_obs_space = self.sim_env.observation_space
-
-        # remove camera observations from space used for flattening as images
-        # are treated separetely and not flattened
+        # a copy of the original observation space which is used when
+        # filtering the observations
+        self._orig_obs_space = deepcopy(self.sim_env.observation_space)
+        # the space used for unflattening the observations (images will
+        # be removed from this space)
+        self._unflattening_space = deepcopy(self.sim_env.observation_space)
+
+        # remove camera observations from space used for flattening
+        # and unflattening as images are treated separetely and not
+        # flattened
         if self.image_obs:
             stripped_camera_observations = spaces.Dict(
                 {
                     k: v
                     for k, v in self._orig_obs_space.spaces[
                         "camera_observation"
                     ].spaces.items()
                     if k != "images"
                 }
             )
-            self._orig_obs_space["camera_observation"] = stripped_camera_observations
+            self._unflattening_space["camera_observation"] = stripped_camera_observations
+            if self.flatten_obs:
+                # if the observations are eventually flattened, they do not contain
+                # images anymore
+                self._orig_obs_space["camera_observation"] = stripped_camera_observations
         self._orig_flat_obs_space = spaces.flatten_space(self._orig_obs_space)
+        self._flat_unflattening_space = spaces.flatten_space(self._unflattening_space)
 
         if scale_obs and not flatten_obs:
             raise NotImplementedError(
                 "Scaling of observations only "
                 "implemented for flattened observations, i.e., for "
                 "flatten_obs=True."
             )
@@ -493,19 +504,19 @@
             rng: Optional range of images to return. rng=(m,n) means that the
                 images with indices m to n-1 are returned.
             indices: Optional array of image indices for which to load data. rng
                 and indices are mutually exclusive, only one of them can be set.
             zarr_path:  Optional path to a Zarr directory containing the dataset,
                 which will be used instead of the default.
             timestep_dimension: Whether to include the timestep dimension in the
-                returned array. This is useful if the given range or indices
+                returned array. This is useful if the given range of indices
                 always contains `n_cameras` of image indices in a row which
                 correspond to the camera images at one camera timestep.
-            cameras are contained in rng or indices. If this assumption is violated,
-            the first dimension will not correspond to camera timesteps anymore.
+                If this assumption is violated, the first dimension will not
+                correspond to camera timesteps anymore.
 
             n_threads: Number of threads to use for processing the images. If None,
                 the number of threads is set to the number of CPUs available to the
                 process.
         Returns:
             The image data (or a part of it specified by rng or indices) as a numpy
             array. If `timestep_dimension` is True the shape will be
@@ -555,17 +566,41 @@
                 reorder_pixels=reorder_pixels,
                 timestep_dimension=timestep_dimension,
             )
             threads.append(image_loader)
             image_loader.start()
         for thread in threads:
             thread.join()
+        store.close()
 
         return unique_images
 
+    def convert_timestep_to_image_index(
+            self,
+            timesteps: np.ndarray,
+            zarr_path: Union[str, os.PathLike] = None,
+        ) -> np.ndarray:
+        """Convert camera timesteps to image indices.
+
+        Args:
+            timesteps:  Array of camera timesteps.
+        Returns:
+            Array of image indices.
+        """
+        if zarr_path is None:
+            zarr_path = self._download_dataset()
+        store = zarr.LMDBStore(zarr_path, readonly=True)
+        root = zarr.open(store=store)
+
+        # mapping from observation index to image index
+        # (necessary since the camera frequency < control frequency)
+        image_indices = root["obs_to_image_index"].get_coordinate_selection(timesteps)
+        store.close()
+        return image_indices
+
     def get_dataset(
         self,
         zarr_path: Union[str, os.PathLike] = None,
         clip: bool = True,
         rng: Optional[Tuple[int, int]] = None,
         indices: Optional[np.ndarray] = None,
         n_threads: Optional[int] = None,
@@ -597,15 +632,15 @@
                 - rewards: Array containing the rewards.
                 - timeouts: Array containing the timeouts (True only at
                     the end of an episode by default. Always False if
                     `set_terminals` is True).
                 - terminals: Array containing the terminals (Always
                     False by default. If `set_terminals` is True, only
                     True at the last timestep of an episode).
-                - image_data (only if present in dataset): Array of the
+                - images (only if present in dataset): Array of the
                     shape (n_control_timesteps, n_cameras, n_channels,
                     height, width) containing the image data. The cannels
                     are ordered as RGB.
         """
 
         # The offline RL dataset is loaded from a Zarr directory which contains
         # the following Zarr arrays (this is an implementation detail and
@@ -682,26 +717,26 @@
                 data_dict[k] = root[k].get_coordinate_selection(indices)
 
         n_control_timesteps = data_dict["observations"].shape[0]
 
         # clip to make sure that there are no outliers in the data
         if clip:
             data_dict["observations"] = data_dict["observations"].clip(
-                min=self._orig_flat_obs_space.low,
-                max=self._orig_flat_obs_space.high,
-                dtype=self._orig_flat_obs_space.dtype,
+                min=self._flat_unflattening_space.low,
+                max=self._flat_unflattening_space.high,
+                dtype=self._flat_unflattening_space.dtype,
             )
 
         if not (self.flatten_obs and self.obs_to_keep is None):
             # unflatten observations, i.e., turn them into dicts again
             unflattened_obs = []
             obs = data_dict["observations"]
             for i in range(obs.shape[0]):
                 unflattened_obs.append(
-                    spaces.unflatten(self._orig_obs_space, obs[i, ...])
+                    spaces.unflatten(self._unflattening_space, obs[i, ...])
                 )
             data_dict["observations"] = unflattened_obs
 
         # timeouts, terminals and info
         if self.set_terminals:
             data_dict["terminals"] = data_dict["timeouts"]
             data_dict["timeouts"] = np.zeros(n_control_timesteps, dtype=bool)
@@ -760,14 +795,16 @@
                     index = (obs_to_image_index[i] - obs_to_image_index[0]) // n_cameras
                 else:
                     # map from original image index to unique image index
                     index = unique_to_original[i * n_cameras] // n_cameras
                 images[i] = unique_images[index]
             data_dict["images"] = images
 
+        store.close()
+
         return data_dict
 
     def get_dataset_chunk(self, chunk_id, zarr_path=None):
         raise NotImplementedError()
 
     def compute_reward(
         self, achieved_goal: dict, desired_goal: dict, info: dict
```

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/evaluate_sim.py` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/evaluate_sim.py`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/evaluation.py` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/evaluation.py`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/policy_base.py` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/policy_base.py`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/sampling_utils.py` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/sim_env.py` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/sim_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 from time import sleep, time
 from typing import Tuple, Dict, Any, Optional
 import logging
 
+import cv2
 import gymnasium as gym
 import numpy as np
 from pybullet import ER_TINY_RENDERER
 
 import trifinger_simulation
 import trifinger_simulation.visual_objects
 from trifinger_simulation import trifingerpro_limits
@@ -562,19 +563,21 @@
             # time elapsed since capturing of pose in seconds
             "delay": np.array(
                 [self._get_pose_delay(camera_observation, t)], dtype=np.float32
             ),
             "confidence": np.array([object_observation.confidence], dtype=np.float32),
         }
         if self.image_obs:
-            # RGB camera images created with software renderer
-            # (using openGL requires GUI to run)
-            images = np.array([cam.image for cam in camera_observation.cameras])
-            print(observation.cameras[0].image.shape)
-            print(images.shape)
+            if len(camera_observation.cameras[0].image.shape) == 2:
+                # images from real platform have to be debayered
+                images = np.array([cv2.cvtColor(cam.image, cv2.COLOR_BAYER_BG2RGB) for cam in camera_observation.cameras])
+            else:
+                # RGB camera images created with software renderer
+                # (using openGL requires GUI to run)
+                images = np.array([cam.image for cam in camera_observation.cameras])
             # convert to channel first
             images = np.transpose(images, (0, 3, 1, 2))
             camera_obs_processed["images"] = images
         if self.keypoint_obs:
             camera_obs_processed["object_keypoints"] = get_keypoints_from_pose(
                 object_observation
             )
```

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets/utils.py` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets.egg-info/PKG-INFO` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,128 @@
 Metadata-Version: 2.1
 Name: trifinger-rl-datasets
-Version: 0.9.2
+Version: 1.0.0
 Summary: Gym environments which provide offline RL datasets collected on the TriFinger system.
 Home-page: UNKNOWN
 Author: Nico Gürtler
 Author-email: nico.guertler@tuebingen.mpg.de
 License: BSD 3-Clause
 Description: # TriFinger RL Datasets
         
-        This repository provides offline reinforcement learning datasets collected on the TriFinger platform (simulated or real). The paper "Benchmarking Offline Reinforcement Learning on Real-Robot Hardware" (TODO: Link) discusses the datasets and benchmarks offline reinforcement learning methods on them. The code for loading the datasets follows the interface suggested by [D4RL](https://github.com/rail-berkeley/d4rl). 
+        This repository provides offline reinforcement learning datasets collected on the real TriFinger platform and in a simulated version of the environment. The paper ["Benchmarking Offline Reinforcement Learning on Real-Robot Hardware"](https://openreview.net/pdf?id=3k5CUGDLNdd) provides more details on the datasets and benchmarks offline RL algorithms on them. All datasets are available with camera images as well.
         
-        TODO: Link to documentation.
-        TODO: Prominently mention (and repeat later on) that the repository also provides versions of the datasets with image observations from three cameras.
+        More detailed information about the simulated environment, the datasets and on how to run experiments on a cluster of real TriFinger robots can be found in the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/).
         
         Some of the datasets were used during the [Real Robot Challenge 2022](https://real-robot-challenge.com).
         
         ## Installation
         
         To install the package run with python 3.8 in the root directory of the repository (we recommend doing this in a virtual environment):
         
         ```bash
-        pip install --upgrade pip  # make sure recent version of pip is installed
+        pip install --upgrade pip  # make sure the most recent version of pip is installed
         pip install .
         ```
         
         ## Usage
         
-        ### Loading the dataset
+        This section provides short examples of how to load datasets and evaluate a policy in simulation. More details on how to work with the datasets can be found in the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/).
         
-        The datasets are accessible via gym environments which are automatically registered when importing the package. They are automatically downloaded when requested and stored in `~/.trifinger_rl_datasets` as HDF5 files.
         
-        The datasets are named following the pattern `trifinger-cube-task-source-quality-v0` where `task` is either `push` or `lift`, `source` is either `sim` or `real` and `quality` can be either `mixed` or `expert`.
+        ### Loading a dataset
+        
+        The datasets are accessible via gym environments which are automatically registered when importing the package. They are automatically downloaded when requested and stored in `~/.trifinger_rl_datasets` as Zarr files by default (see the [documentation](https://webdav.tuebingen.mpg.de/trifinger-rl/docs/) for custom paths to the datasets). The code for loading the datasets follows the interface suggested by [D4RL](https://github.com/rail-berkeley/d4rl) and extends it where needed. 
+        
+        The datasets are named following the pattern `trifinger-cube-task-source-type-v0` where `task` is either `push` or `lift`, `source` is either `sim` or `real` and `type` can be either `mixed`, `weak-n-expert` or `expert`.
         
         By default the observations are loaded as flat arrays. For the simulated datasets the environment can be stepped and visualized. Example usage (also see `demo/load_dataset.py`):
         
         ```python
         import gymnasium as gym
         
         import trifinger_rl_datasets
         
         env = gym.make(
             "trifinger-cube-push-sim-expert-v0",
-            disable_env_checker=True,
             visualization=True,  # enable visualization
         )
         
         dataset = env.get_dataset()
         
         print("First observation: ", dataset["observations"][0])
         print("First action: ", dataset["actions"][0])
         print("First reward: ", dataset["rewards"][0])
         
-        obs = env.reset()
-        done = False
-        while not done:
-            obs, rew, done, info = env.step(env.action_space.sample())
+        obs, info = env.reset()
+        truncated = False
+        
+        while not truncated:
+            obs, rew, terminated, truncated, info = env.step(env.action_space.sample())
         ```
         
         Alternatively, the observations can be obtained as nested dictionaries. This simplifies working with the data. As some parts of the observations might be more useful than others, it is also possible to filter the observations when requesting dictionaries (see `demo/load_filtered_dicts.py`):
+        
         ```python
             # Nested dictionary defines which observations to keep.
             # Everything that is not included or has value False
             # will be dropped.
             obs_to_keep = {
                 "robot_observation": {
                     "position": True,
                     "velocity": True,
                     "fingertip_force": False,
                 },
                 "object_observation": {"keypoints": True},
             }
             env = gym.make(
                 args.env_name,
-                disable_env_checker=True,
                 # filter observations,
                 obs_to_keep=obs_to_keep,
             )
         ```
-        To transform the observation back to a flat array after filtering, simply set the keyword argument `flatten_obs` to true. Note that the step and reset functions will transform observations in the same manner as the `get_dataset` method to ensure compatibility. A downside of working with observations in the form of dictionaries is that they cause a considerable memory overhead during dataset loading.
         
         All datasets come in two versions: with and without camera observations. The versions with camera observations contain `-image` in their name. Despite PNG image compression they are more than one order of magnitude bigger than the imageless versions. To avoid running out of memory, a part of a dataset can be loaded by specifying a range of timesteps:
+        
         ```python
         env = gym.make(
             "trifinger-cube-push-real-expert-image-v0",
             disable_env_checker=True
         )
         
         # load only a subset of obervations, actions and rewards
         dataset = env.get_dataset(rng=(1000, 2000))
         ```
+        
         The camera observations corresponding to this range are then returned in `dataset["images"]` with the following dimensions:
+        
         ```python
         n_timesteps, n_cameras, n_channels, height, width = dataset["images"].shape
         ```
-        Since the camera frequency is lower than the control frequency, a camera image will repeat over several time steps. To load an array of camera images without this redundancy, the `get_image_data` method can be used:
-        ```python
-        # images from 3 cameras for each timestep
-        image_stats = env.get_image_stats()
-        n_cameras = image_stats["n_cameras"]
-        images = env.get_image_data(rng=(0, n_cameras * n_camera_frames_to_load)) 
-        ```
         
         ### Evaluating a policy in simulation
         
         This package contains an executable module `trifinger_rl_datasets.evaluate_sim`, which
         can be used to evaluate a policy in simulation.  As arguments it expects the task
         ("push" or "lift") and a Python class that implements the policy, following the
         `PolicyBase` interface:
         
             python3 -m trifinger_rl_datasets.evaluate_sim push my_package.MyPolicy
         
         For more options see `--help`.
+        
+        ## How to cite
+        
+        The paper ["Benchmarking Offline Reinforcement Learning on Real-Robot Hardware"](https://openreview.net/pdf?id=3k5CUGDLNdd) introducing the datasets was published at ICLR 2023:
+        
+        ```
+        @inproceedings{
+        guertler2023benchmarking,
+        title={Benchmarking Offline Reinforcement Learning on Real-Robot Hardware},
+        author={Nico G{\"u}rtler and Sebastian Blaes and Pavel Kolev and Felix Widmaier and Manuel Wuthrich and Stefan Bauer and Bernhard Sch{\"o}lkopf and Georg Martius},
+        booktitle={The Eleventh International Conference on Learning Representations },
+        year={2023},
+        url={https://openreview.net/forum?id=3k5CUGDLNdd}
+        }
+        ```
 Keywords: offline reinforcement learning,reinforcement learning,robotics,TriFinger,Real Robot Challenge,dexterous manipulation
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `trifinger_rl_datasets-0.9.2/trifinger_rl_datasets.egg-info/SOURCES.txt` & `trifinger_rl_datasets-1.0.0/trifinger_rl_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*


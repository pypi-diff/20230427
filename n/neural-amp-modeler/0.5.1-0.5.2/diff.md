# Comparing `tmp/neural-amp-modeler-0.5.1.tar.gz` & `tmp/neural-amp-modeler-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-amp-modeler-0.5.1.tar", last modified: Wed Apr 26 02:50:57 2023, max compression
+gzip compressed data, was "neural-amp-modeler-0.5.2.tar", last modified: Thu Apr 27 02:14:55 2023, max compression
```

## Comparing `neural-amp-modeler-0.5.1.tar` & `neural-amp-modeler-0.5.2.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 02:50:57.669599 neural-amp-modeler-0.5.1/
--rw-r--r--   0 steve      (501) staff       (20)     1072 2022-12-20 07:51:29.000000 neural-amp-modeler-0.5.1/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       49 2023-04-01 05:02:40.000000 neural-amp-modeler-0.5.1/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)      211 2023-04-26 02:50:57.669072 neural-amp-modeler-0.5.1/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     4541 2023-04-26 02:42:34.000000 neural-amp-modeler-0.5.1/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 02:50:57.648293 neural-amp-modeler-0.5.1/nam/
--rw-r--r--   0 steve      (501) staff       (20)      729 2023-03-18 16:36:25.000000 neural-amp-modeler-0.5.1/nam/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      362 2023-03-18 16:36:25.000000 neural-amp-modeler-0.5.1/nam/_core.py
--rw-r--r--   0 steve      (501) staff       (20)       22 2023-04-10 01:24:24.000000 neural-amp-modeler-0.5.1/nam/_version.py
--rw-r--r--   0 steve      (501) staff       (20)    22084 2023-03-18 16:36:25.000000 neural-amp-modeler-0.5.1/nam/data.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 02:50:57.655431 neural-amp-modeler-0.5.1/nam/models/
--rw-r--r--   0 steve      (501) staff       (20)      372 2023-02-21 06:40:52.000000 neural-amp-modeler-0.5.1/nam/models/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      209 2023-04-10 01:24:24.000000 neural-amp-modeler-0.5.1/nam/models/_activations.py
--rw-r--r--   0 steve      (501) staff       (20)     5327 2023-04-25 01:51:12.000000 neural-amp-modeler-0.5.1/nam/models/_base.py
--rw-r--r--   0 steve      (501) staff       (20)     4356 2023-04-25 01:51:12.000000 neural-amp-modeler-0.5.1/nam/models/_exportable.py
--rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.5.1/nam/models/_names.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 02:50:57.656142 neural-amp-modeler-0.5.1/nam/models/_resources/
--rw-r--r--   0 steve      (501) staff       (20)   144044 2023-04-01 05:02:40.000000 neural-amp-modeler-0.5.1/nam/models/_resources/loudness_input.wav
--rw-r--r--   0 steve      (501) staff       (20)    11011 2023-04-01 05:02:56.000000 neural-amp-modeler-0.5.1/nam/models/base.py
--rw-r--r--   0 steve      (501) staff       (20)     9052 2022-12-20 07:51:29.000000 neural-amp-modeler-0.5.1/nam/models/conv_net.py
--rw-r--r--   0 steve      (501) staff       (20)     1952 2022-12-20 07:51:29.000000 neural-amp-modeler-0.5.1/nam/models/linear.py
--rw-r--r--   0 steve      (501) staff       (20)     2154 2023-04-25 01:51:12.000000 neural-amp-modeler-0.5.1/nam/models/losses.py
--rw-r--r--   0 steve      (501) staff       (20)     1017 2023-04-25 01:51:12.000000 neural-amp-modeler-0.5.1/nam/models/metadata.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 02:50:57.660181 neural-amp-modeler-0.5.1/nam/models/parametric/
--rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.5.1/nam/models/parametric/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6572 2023-04-10 01:24:24.000000 neural-amp-modeler-0.5.1/nam/models/parametric/catnets.py
--rw-r--r--   0 steve      (501) staff       (20)    18233 2023-03-17 03:52:30.000000 neural-amp-modeler-0.5.1/nam/models/parametric/hyper_net.py
--rw-r--r--   0 steve      (501) staff       (20)     1521 2022-12-20 07:51:29.000000 neural-amp-modeler-0.5.1/nam/models/parametric/params.py
--rw-r--r--   0 steve      (501) staff       (20)    16232 2023-04-25 01:51:12.000000 neural-amp-modeler-0.5.1/nam/models/recurrent.py
--rw-r--r--   0 steve      (501) staff       (20)    12371 2023-02-21 06:40:52.000000 neural-amp-modeler-0.5.1/nam/models/wavenet.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 02:50:57.663710 neural-amp-modeler-0.5.1/nam/train/
--rw-r--r--   0 steve      (501) staff       (20)      108 2022-12-20 07:51:29.000000 neural-amp-modeler-0.5.1/nam/train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      665 2023-04-10 01:24:24.000000 neural-amp-modeler-0.5.1/nam/train/_version.py
--rw-r--r--   0 steve      (501) staff       (20)     3249 2023-04-25 01:51:12.000000 neural-amp-modeler-0.5.1/nam/train/colab.py
--rw-r--r--   0 steve      (501) staff       (20)    14035 2023-04-26 02:42:34.000000 neural-amp-modeler-0.5.1/nam/train/core.py
--rw-r--r--   0 steve      (501) staff       (20)    19277 2023-04-25 01:51:12.000000 neural-amp-modeler-0.5.1/nam/train/gui.py
--rw-r--r--   0 steve      (501) staff       (20)      307 2023-02-21 06:40:52.000000 neural-amp-modeler-0.5.1/nam/util.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 02:50:57.667521 neural-amp-modeler-0.5.1/neural_amp_modeler.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      211 2023-04-26 02:50:57.000000 neural-amp-modeler-0.5.1/neural_amp_modeler.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      926 2023-04-26 02:50:57.000000 neural-amp-modeler-0.5.1/neural_amp_modeler.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-26 02:50:57.000000 neural-amp-modeler-0.5.1/neural_amp_modeler.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       42 2023-04-26 02:50:57.000000 neural-amp-modeler-0.5.1/neural_amp_modeler.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)      114 2023-04-26 02:50:57.000000 neural-amp-modeler-0.5.1/neural_amp_modeler.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        4 2023-04-26 02:50:57.000000 neural-amp-modeler-0.5.1/neural_amp_modeler.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-26 02:50:57.669762 neural-amp-modeler-0.5.1/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)      966 2023-04-26 02:50:16.000000 neural-amp-modeler-0.5.1/setup.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 02:50:57.668351 neural-amp-modeler-0.5.1/tests/
--rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.5.1/tests/test_install.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.419704 neural-amp-modeler-0.5.2/
+-rw-rw-rw-   0        0        0     1093 2022-04-21 06:27:49.000000 neural-amp-modeler-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-03-25 00:10:46.000000 neural-amp-modeler-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      219 2023-04-27 02:14:55.419704 neural-amp-modeler-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4677 2023-04-27 02:02:18.000000 neural-amp-modeler-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.371704 neural-amp-modeler-0.5.2/nam/
+-rw-rw-rw-   0        0        0      754 2023-03-19 00:42:20.000000 neural-amp-modeler-0.5.2/nam/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-03-25 00:10:46.000000 neural-amp-modeler-0.5.2/nam/_core.py
+-rw-rw-rw-   0        0        0       23 2023-04-27 02:08:12.000000 neural-amp-modeler-0.5.2/nam/_version.py
+-rw-rw-rw-   0        0        0    22751 2023-04-18 01:51:50.000000 neural-amp-modeler-0.5.2/nam/data.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.385703 neural-amp-modeler-0.5.2/nam/models/
+-rw-rw-rw-   0        0        0      383 2023-02-16 06:08:00.000000 neural-amp-modeler-0.5.2/nam/models/__init__.py
+-rw-rw-rw-   0        0        0      218 2023-04-09 17:49:31.000000 neural-amp-modeler-0.5.2/nam/models/_activations.py
+-rw-rw-rw-   0        0        0     5510 2023-04-23 01:03:30.000000 neural-amp-modeler-0.5.2/nam/models/_base.py
+-rw-rw-rw-   0        0        0     4675 2023-04-27 02:05:48.000000 neural-amp-modeler-0.5.2/nam/models/_exportable.py
+-rw-rw-rw-   0        0        0      250 2022-09-03 21:37:15.000000 neural-amp-modeler-0.5.2/nam/models/_names.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.389702 neural-amp-modeler-0.5.2/nam/models/_resources/
+-rw-rw-rw-   0        0        0   144044 2023-03-25 00:10:46.000000 neural-amp-modeler-0.5.2/nam/models/_resources/loudness_input.wav
+-rw-rw-rw-   0        0        0    11326 2023-04-09 17:50:14.000000 neural-amp-modeler-0.5.2/nam/models/base.py
+-rw-rw-rw-   0        0        0     9342 2022-09-04 21:58:20.000000 neural-amp-modeler-0.5.2/nam/models/conv_net.py
+-rw-rw-rw-   0        0        0     2022 2022-09-03 21:37:15.000000 neural-amp-modeler-0.5.2/nam/models/linear.py
+-rw-rw-rw-   0        0        0     2230 2023-04-23 01:03:30.000000 neural-amp-modeler-0.5.2/nam/models/losses.py
+-rw-rw-rw-   0        0        0     1240 2023-04-27 02:03:11.000000 neural-amp-modeler-0.5.2/nam/models/metadata.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.394704 neural-amp-modeler-0.5.2/nam/models/parametric/
+-rw-rw-rw-   0        0        0      108 2023-04-09 17:49:31.000000 neural-amp-modeler-0.5.2/nam/models/parametric/__init__.py
+-rw-rw-rw-   0        0        0     6787 2023-04-09 17:49:31.000000 neural-amp-modeler-0.5.2/nam/models/parametric/catnets.py
+-rw-rw-rw-   0        0        0    18792 2023-02-16 06:08:00.000000 neural-amp-modeler-0.5.2/nam/models/parametric/hyper_net.py
+-rw-rw-rw-   0        0        0     1592 2022-09-03 21:37:15.000000 neural-amp-modeler-0.5.2/nam/models/parametric/params.py
+-rw-rw-rw-   0        0        0    16701 2023-04-22 22:14:48.000000 neural-amp-modeler-0.5.2/nam/models/recurrent.py
+-rw-rw-rw-   0        0        0     1177 2022-12-15 07:10:30.000000 neural-amp-modeler-0.5.2/nam/models/undersampling.py
+-rw-rw-rw-   0        0        0    12766 2023-02-17 03:42:58.000000 neural-amp-modeler-0.5.2/nam/models/wavenet.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.406703 neural-amp-modeler-0.5.2/nam/train/
+-rw-rw-rw-   0        0        0      111 2023-01-29 07:48:38.000000 neural-amp-modeler-0.5.2/nam/train/__init__.py
+-rw-rw-rw-   0        0        0      690 2023-04-09 17:49:31.000000 neural-amp-modeler-0.5.2/nam/train/_version.py
+-rw-rw-rw-   0        0        0     3351 2023-04-23 01:10:20.000000 neural-amp-modeler-0.5.2/nam/train/colab.py
+-rw-rw-rw-   0        0        0    14470 2023-04-27 02:02:18.000000 neural-amp-modeler-0.5.2/nam/train/core.py
+-rw-rw-rw-   0        0        0    19942 2023-04-27 02:03:19.000000 neural-amp-modeler-0.5.2/nam/train/gui.py
+-rw-rw-rw-   0        0        0     1578 2023-02-14 06:14:54.000000 neural-amp-modeler-0.5.2/nam/train/ir.py
+-rw-rw-rw-   0        0        0      321 2023-02-16 06:08:00.000000 neural-amp-modeler-0.5.2/nam/util.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.417703 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      970 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 02:14:55.419704 neural-amp-modeler-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-04-27 02:02:18.000000 neural-amp-modeler-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.418704 neural-amp-modeler-0.5.2/tests/
+-rw-rw-rw-   0        0        0      250 2022-04-21 06:27:49.000000 neural-amp-modeler-0.5.2/tests/test_install.py
```

### Comparing `neural-amp-modeler-0.5.1/LICENSE` & `neural-amp-modeler-0.5.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Steven Atkinson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Steven Atkinson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `neural-amp-modeler-0.5.1/README.md` & `neural-amp-modeler-0.5.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-# NAM: neural amp modeler
-
-This repository handles training, reamping, and exporting the weights of a model.
-For playing trained models in real time in a standalone application or plugin, see the partner repo,
-[NeuralAmpModelerPlugin](https://github.com/sdatkinson/NeuralAmpModelerPlugin).
-
-## How to use (Google Colab)
-
-If you don't have a good computer for training ML models, you use Google Colab to train
-in the cloud using the pre-made notebooks under `bin\train`.
-
-For the very easiest experience, open 
-[`easy_colab.ipynb` on Google Colab](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/7c7b46b/bin/train/easy_colab.ipynb) 
-and follow the steps!
-
-For a little more visibility under the hood, you can use [colab.ipynb](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/main/bin/train/colab.ipynb) instead.
-
-**Pros:**
-
-- No local installation required!
-- Decent GPUs are available if you don't have one on your computer.
-
-**Cons:**
-
-- Uploading your data can take a long time.
-- The session will time out after a few hours (for free accounts), so extended
-  training runs aren't really feasible. Also, there's a usage limit so you can't hang
-  out all day. I've tried to set you up with a good model that should train reasonably
-  quickly!
-
-## How to use (Local)
-
-Alternatively, you can clone this repo to your computer and use it locally.
-
-### Installation
-
-Installation uses [Anaconda](https://www.anaconda.com/) for package management.
-
-For computers with a CUDA-capable GPU (recommended):
-
-```bash
-conda env create -f environment_gpu.yml
-```
-
-Otherwise, for a CPU-only install (will train much more slowly):
-
-```bash
-conda env create -f environment_cpu.yml
-```
-
-Then activate the environment you've created with
-
-```bash
-conda activate nam
-```
-
-### Train models (GUI)
-After installing, you can open a GUI trainer by running
-
-```bash
-nam
-```
-
-from the terminal.
-
-### Train models (Python script)
-For users looking to get more fine-grained control over the modeling process, 
-NAM includes a training script that can be run from the terminal. In order to run it
-#### Download audio files
-Download the [v1_1_1.wav](https://drive.google.com/file/d/1v2xFXeQ9W2Ks05XrqsMCs2viQcKPAwBk/view?usp=share_link) and [overdrive.wav](https://drive.google.com/file/d/14w2utgL16NozmESzAJO_I0_VCt-5Wgpv/view?usp=share_link) to a folder of your choice 
-
-#### Update data configuration 
-Edit `bin/train/data/single_pair.json` to point to relevant audio files 
-```json
-    "common": {
-        "x_path": "C:\\path\\to\\v1_1_1.wav",
-        "y_path": "C:\\path\\to\\overdrive.wav",
-        "delay": 0
-    }
-```
-
-#### Run training script
-Open up a terminal. Activate your nam environment and call the training with
-```bash
-python bin/train/main.py \
-bin/train/inputs/data/single_pair.json \
-bin/train/inputs/models/demonet.json \
-bin/train/inputs/learning/demo.json \
-bin/train/outputs/MyAmp
-```
-
-`data/single_pair.json` contains the information about the data you're training
-on   
-`models/demonet.json` contains information about the model architecture that
-is being trained. The example used here uses a `feather` configured `wavenet`.  
-`learning/demo.json` contains information about the training run itself (e.g. number of epochs).
-
-The configuration above runs a short (demo) training. For a real training you may prefer to run something like,
-
-```bash
-python bin/train/main.py \
-bin/train/inputs/data/single_pair.json \
-bin/train/inputs/models/wavenet.json \
-bin/train/inputs/learning/default.json \
-bin/train/outputs/MyAmp
-```
-
-As a side note, NAM uses [PyTorch Lightning](https://lightning.ai/pages/open-source/) 
-under the hood as a modeling framework, and you can control many of the Pytorch Lightning configuration options from `bin/train/inputs/learning/default.json`
-
-#### Export a model (to use with [the plugin](https://github.com/sdatkinson/NeuralAmpModelerPlugin))
-Exporting the trained model to a `.nam` file for use with the plugin can be done
-with:
-
-```bash
-python bin/export.py \
-path/to/config_model.json \
-path/to/checkpoints/epoch=123_val_loss=0.000010.ckpt \
-path/to/exported_models/MyAmp
-```
-
-Then, point the plugin at the exported `model.nam` file and you're good to go!
-
-### Other utilities
-
-#### Run a model on an input signal ("reamping")
-
-Handy if you want to just check it out without needing to use the plugin:
-
-```bash
-python bin/run.py \
-path/to/source.wav \
-path/to/config_model.json \
-path/to/checkpoints/epoch=123_val_loss=0.000010.ckpt \
-path/to/output.wav
-```
+# NAM: neural amp modeler
+
+This repository handles training, reamping, and exporting the weights of a model.
+For playing trained models in real time in a standalone application or plugin, see the partner repo,
+[NeuralAmpModelerPlugin](https://github.com/sdatkinson/NeuralAmpModelerPlugin).
+
+## How to use (Google Colab)
+
+If you don't have a good computer for training ML models, you use Google Colab to train
+in the cloud using the pre-made notebooks under `bin\train`.
+
+For the very easiest experience, open 
+[`easy_colab.ipynb` on Google Colab](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/b1aa204/bin/train/easy_colab.ipynb) 
+and follow the steps!
+
+For a little more visibility under the hood, you can use [colab.ipynb](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/main/bin/train/colab.ipynb) instead.
+
+**Pros:**
+
+- No local installation required!
+- Decent GPUs are available if you don't have one on your computer.
+
+**Cons:**
+
+- Uploading your data can take a long time.
+- The session will time out after a few hours (for free accounts), so extended
+  training runs aren't really feasible. Also, there's a usage limit so you can't hang
+  out all day. I've tried to set you up with a good model that should train reasonably
+  quickly!
+
+## How to use (Local)
+
+Alternatively, you can clone this repo to your computer and use it locally.
+
+### Installation
+
+Installation uses [Anaconda](https://www.anaconda.com/) for package management.
+
+For computers with a CUDA-capable GPU (recommended):
+
+```bash
+conda env create -f environment_gpu.yml
+```
+
+Otherwise, for a CPU-only install (will train much more slowly):
+
+```bash
+conda env create -f environment_cpu.yml
+```
+
+Then activate the environment you've created with
+
+```bash
+conda activate nam
+```
+
+### Train models (GUI)
+After installing, you can open a GUI trainer by running
+
+```bash
+nam
+```
+
+from the terminal.
+
+### Train models (Python script)
+For users looking to get more fine-grained control over the modeling process, 
+NAM includes a training script that can be run from the terminal. In order to run it
+#### Download audio files
+Download the [v1_1_1.wav](https://drive.google.com/file/d/1v2xFXeQ9W2Ks05XrqsMCs2viQcKPAwBk/view?usp=share_link) and [overdrive.wav](https://drive.google.com/file/d/14w2utgL16NozmESzAJO_I0_VCt-5Wgpv/view?usp=share_link) to a folder of your choice 
+
+#### Update data configuration 
+Edit `bin/train/data/single_pair.json` to point to relevant audio files 
+```json
+    "common": {
+        "x_path": "C:\\path\\to\\v1_1_1.wav",
+        "y_path": "C:\\path\\to\\overdrive.wav",
+        "delay": 0
+    }
+```
+
+#### Run training script
+Open up a terminal. Activate your nam environment and call the training with
+```bash
+python bin/train/main.py \
+bin/train/inputs/data/single_pair.json \
+bin/train/inputs/models/demonet.json \
+bin/train/inputs/learning/demo.json \
+bin/train/outputs/MyAmp
+```
+
+`data/single_pair.json` contains the information about the data you're training
+on   
+`models/demonet.json` contains information about the model architecture that
+is being trained. The example used here uses a `feather` configured `wavenet`.  
+`learning/demo.json` contains information about the training run itself (e.g. number of epochs).
+
+The configuration above runs a short (demo) training. For a real training you may prefer to run something like,
+
+```bash
+python bin/train/main.py \
+bin/train/inputs/data/single_pair.json \
+bin/train/inputs/models/wavenet.json \
+bin/train/inputs/learning/default.json \
+bin/train/outputs/MyAmp
+```
+
+As a side note, NAM uses [PyTorch Lightning](https://lightning.ai/pages/open-source/) 
+under the hood as a modeling framework, and you can control many of the Pytorch Lightning configuration options from `bin/train/inputs/learning/default.json`
+
+#### Export a model (to use with [the plugin](https://github.com/sdatkinson/NeuralAmpModelerPlugin))
+Exporting the trained model to a `.nam` file for use with the plugin can be done
+with:
+
+```bash
+python bin/export.py \
+path/to/config_model.json \
+path/to/checkpoints/epoch=123_val_loss=0.000010.ckpt \
+path/to/exported_models/MyAmp
+```
+
+Then, point the plugin at the exported `model.nam` file and you're good to go!
+
+### Other utilities
+
+#### Run a model on an input signal ("reamping")
+
+Handy if you want to just check it out without needing to use the plugin:
+
+```bash
+python bin/run.py \
+path/to/source.wav \
+path/to/config_model.json \
+path/to/checkpoints/epoch=123_val_loss=0.000010.ckpt \
+path/to/output.wav
+```
```

### Comparing `neural-amp-modeler-0.5.1/nam/__init__.py` & `neural-amp-modeler-0.5.2/nam/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# File: __init__.py
-# File Created: Tuesday, 2nd February 2021 9:42:50 pm
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-# Hack to recover graceful shutdowns in Windows.
-# This has to happen ASAP
-# See:
-# https://github.com/sdatkinson/neural-amp-modeler/issues/105
-# https://stackoverflow.com/a/44822794
-def _ensure_graceful_shutdowns():
-    import os
-
-    if os.name == "nt":  # OS is Windows
-        os.environ["FOR_DISABLE_CONSOLE_CTRL_HANDLER"] = "1"
-
-
-_ensure_graceful_shutdowns()
-
-from ._version import __version__  # Must be before models or else circular
-
-from . import _core  # noqa F401
-from . import data  # noqa F401
-from . import models  # noqa F401
-from . import util  # noqa F401
-from . import train  # noqa F401
+# File: __init__.py
+# File Created: Tuesday, 2nd February 2021 9:42:50 pm
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+# Hack to recover graceful shutdowns in Windows.
+# This has to happen ASAP
+# See:
+# https://github.com/sdatkinson/neural-amp-modeler/issues/105
+# https://stackoverflow.com/a/44822794
+def _ensure_graceful_shutdowns():
+    import os
+
+    if os.name == "nt":  # OS is Windows
+        os.environ["FOR_DISABLE_CONSOLE_CTRL_HANDLER"] = "1"
+
+
+_ensure_graceful_shutdowns()
+
+from ._version import __version__  # Must be before models or else circular
+
+from . import _core  # noqa F401
+from . import data  # noqa F401
+from . import models  # noqa F401
+from . import util  # noqa F401
+from . import train  # noqa F401
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/_base.py` & `neural-amp-modeler-0.5.2/nam/models/_base.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-# File: _base.py
-# Created Date: Tuesday February 8th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-The foundation of the model without the PyTorch Lightning attributes (losses, training 
-steps)
-"""
-
-import abc
-import math
-import pkg_resources
-from typing import Any, Dict, Optional, Tuple, Union
-
-import numpy as np
-import torch
-import torch.nn as nn
-
-from .._core import InitializableFromConfig
-from ..data import REQUIRED_RATE, wav_to_tensor
-from ._exportable import Exportable
-
-
-class _Base(nn.Module, InitializableFromConfig, Exportable):
-    @abc.abstractproperty
-    def pad_start_default(self) -> bool:
-        pass
-
-    @abc.abstractproperty
-    def receptive_field(self) -> int:
-        """
-        Receptive field of the model
-        """
-        pass
-
-    @abc.abstractmethod
-    def forward(self, *args, **kwargs) -> torch.Tensor:
-        pass
-
-    def _metadata_loudness(self, gain: float = 1.0, db: bool = True) -> float:
-        """
-        How loud is this model when given a standardized input?
-        In dB
-
-        :param gain: Multiplies input signal
-        """
-        x = wav_to_tensor(
-            pkg_resources.resource_filename(
-                "nam", "models/_resources/loudness_input.wav"
-            )
-        )
-        y = self._at_nominal_settings(gain * x)
-        loudness = torch.sqrt(torch.mean(torch.square(y)))
-        if db:
-            loudness = 20.0 * torch.log10(loudness)
-        return loudness.item()
-
-    def _metadata_gain(self) -> float:
-        """
-        Between 0 and 1, how much gain / compression does the model seem to have?
-        """
-        x = np.linspace(0.0, 1.0, 11)
-        y = np.array([self._metadata_loudness(gain=gain, db=False) for gain in x])
-        #
-        # O ^ o o o o o o
-        # u | o       x   +-------------------------------------+
-        # t | o     x     | x: Minimum gain (no compression)    |
-        # p | o   x       | o: Max gain     (100% compression)  |
-        # u | o x         +-------------------------------------+
-        # t | o
-        #   +------------->
-        #       Input
-        #
-        max_gain = y[-1] * len(x)  # "Square"
-        min_gain = 0.5 * max_gain  # "Triangle"
-        gain_range = max_gain - min_gain
-        this_gain = y.sum()
-        normalized_gain = (this_gain - min_gain) / gain_range
-        return np.clip(normalized_gain, 0.0, 1.0)
-
-    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
-        # parametric?...
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def _forward(self, *args) -> torch.Tensor:
-        """
-        The true forward method.
-
-        :param x: (N,L1)
-        :return: (N,L1-RF+1)
-        """
-        pass
-
-    def _export_input_output_args(self) -> Tuple[Any]:
-        """
-        Create any other args necessesary (e.g. params to eval at)
-        """
-        return ()
-
-    def _export_input_output(self) -> Tuple[np.ndarray, np.ndarray]:
-        args = self._export_input_output_args()
-        rate = REQUIRED_RATE
-        x = torch.cat(
-            [
-                torch.zeros((rate,)),
-                0.5
-                * torch.sin(
-                    2.0 * math.pi * 220.0 * torch.linspace(0.0, 1.0, rate + 1)[:-1]
-                ),
-                torch.zeros((rate,)),
-            ]
-        )
-        # Use pad start to ensure same length as requested by ._export_input_output()
-        return (
-            x.detach().cpu().numpy(),
-            self(*args, x, pad_start=True).detach().cpu().numpy(),
-        )
-
-
-class BaseNet(_Base):
-    def forward(self, x: torch.Tensor, pad_start: Optional[bool] = None):
-        pad_start = self.pad_start_default if pad_start is None else pad_start
-        scalar = x.ndim == 1
-        if scalar:
-            x = x[None]
-        if pad_start:
-            x = torch.cat((torch.zeros((len(x), self.receptive_field - 1)), x), dim=1)
-        y = self._forward(x)
-        if scalar:
-            y = y[0]
-        return y
-
-    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
-        return self(x)
-
-    @abc.abstractmethod
-    def _forward(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        The true forward method.
-
-        :param x: (N,L1)
-        :return: (N,L1-RF+1)
-        """
-        pass
-
-    def _get_non_user_metadata(self) -> Dict[str, Union[str, int, float]]:
-        d = super()._get_non_user_metadata()
-        d["loudness"] = self._metadata_loudness()
-        d["gain"] = self._metadata_gain()
-        return d
-
-
-class ParametricBaseNet(_Base):
-    """
-    Parametric inputs
-    """
-
-    def forward(
-        self, params: torch.Tensor, x: torch.Tensor, pad_start: Optional[bool] = None
-    ):
-        pad_start = self.pad_start_default if pad_start is None else pad_start
-        scalar = x.ndim == 1
-        if scalar:
-            x = x[None]
-            params = params[None]
-        if pad_start:
-            x = torch.cat((torch.zeros((len(x), self.receptive_field - 1)), x), dim=1)
-        y = self._forward(params, x)
-        if scalar:
-            y = y[0]
-        return y
-
-    @abc.abstractmethod
-    def _forward(self, params: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
-        """
-        The true forward method.
-
-        :param params: (N,D)
-        :param x: (N,L1)
-        :return: (N,L1-RF+1)
-        """
-        pass
+# File: _base.py
+# Created Date: Tuesday February 8th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+The foundation of the model without the PyTorch Lightning attributes (losses, training 
+steps)
+"""
+
+import abc
+import math
+import pkg_resources
+from typing import Any, Dict, Optional, Tuple, Union
+
+import numpy as np
+import torch
+import torch.nn as nn
+
+from .._core import InitializableFromConfig
+from ..data import REQUIRED_RATE, wav_to_tensor
+from ._exportable import Exportable
+
+
+class _Base(nn.Module, InitializableFromConfig, Exportable):
+    @abc.abstractproperty
+    def pad_start_default(self) -> bool:
+        pass
+
+    @abc.abstractproperty
+    def receptive_field(self) -> int:
+        """
+        Receptive field of the model
+        """
+        pass
+
+    @abc.abstractmethod
+    def forward(self, *args, **kwargs) -> torch.Tensor:
+        pass
+
+    def _metadata_loudness(self, gain: float = 1.0, db: bool = True) -> float:
+        """
+        How loud is this model when given a standardized input?
+        In dB
+
+        :param gain: Multiplies input signal
+        """
+        x = wav_to_tensor(
+            pkg_resources.resource_filename(
+                "nam", "models/_resources/loudness_input.wav"
+            )
+        )
+        y = self._at_nominal_settings(gain * x)
+        loudness = torch.sqrt(torch.mean(torch.square(y)))
+        if db:
+            loudness = 20.0 * torch.log10(loudness)
+        return loudness.item()
+
+    def _metadata_gain(self) -> float:
+        """
+        Between 0 and 1, how much gain / compression does the model seem to have?
+        """
+        x = np.linspace(0.0, 1.0, 11)
+        y = np.array([self._metadata_loudness(gain=gain, db=False) for gain in x])
+        #
+        # O ^ o o o o o o
+        # u | o       x   +-------------------------------------+
+        # t | o     x     | x: Minimum gain (no compression)    |
+        # p | o   x       | o: Max gain     (100% compression)  |
+        # u | o x         +-------------------------------------+
+        # t | o
+        #   +------------->
+        #       Input
+        #
+        max_gain = y[-1] * len(x)  # "Square"
+        min_gain = 0.5 * max_gain  # "Triangle"
+        gain_range = max_gain - min_gain
+        this_gain = y.sum()
+        normalized_gain = (this_gain - min_gain) / gain_range
+        return np.clip(normalized_gain, 0.0, 1.0)
+
+    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
+        # parametric?...
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def _forward(self, *args) -> torch.Tensor:
+        """
+        The true forward method.
+
+        :param x: (N,L1)
+        :return: (N,L1-RF+1)
+        """
+        pass
+
+    def _export_input_output_args(self) -> Tuple[Any]:
+        """
+        Create any other args necessesary (e.g. params to eval at)
+        """
+        return ()
+
+    def _export_input_output(self) -> Tuple[np.ndarray, np.ndarray]:
+        args = self._export_input_output_args()
+        rate = REQUIRED_RATE
+        x = torch.cat(
+            [
+                torch.zeros((rate,)),
+                0.5
+                * torch.sin(
+                    2.0 * math.pi * 220.0 * torch.linspace(0.0, 1.0, rate + 1)[:-1]
+                ),
+                torch.zeros((rate,)),
+            ]
+        )
+        # Use pad start to ensure same length as requested by ._export_input_output()
+        return (
+            x.detach().cpu().numpy(),
+            self(*args, x, pad_start=True).detach().cpu().numpy(),
+        )
+
+
+class BaseNet(_Base):
+    def forward(self, x: torch.Tensor, pad_start: Optional[bool] = None):
+        pad_start = self.pad_start_default if pad_start is None else pad_start
+        scalar = x.ndim == 1
+        if scalar:
+            x = x[None]
+        if pad_start:
+            x = torch.cat((torch.zeros((len(x), self.receptive_field - 1)), x), dim=1)
+        y = self._forward(x)
+        if scalar:
+            y = y[0]
+        return y
+
+    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
+        return self(x)
+
+    @abc.abstractmethod
+    def _forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        The true forward method.
+
+        :param x: (N,L1)
+        :return: (N,L1-RF+1)
+        """
+        pass
+
+    def _get_non_user_metadata(self) -> Dict[str, Union[str, int, float]]:
+        d = super()._get_non_user_metadata()
+        d["loudness"] = self._metadata_loudness()
+        d["gain"] = self._metadata_gain()
+        return d
+
+
+class ParametricBaseNet(_Base):
+    """
+    Parametric inputs
+    """
+
+    def forward(
+        self, params: torch.Tensor, x: torch.Tensor, pad_start: Optional[bool] = None
+    ):
+        pad_start = self.pad_start_default if pad_start is None else pad_start
+        scalar = x.ndim == 1
+        if scalar:
+            x = x[None]
+            params = params[None]
+        if pad_start:
+            x = torch.cat((torch.zeros((len(x), self.receptive_field - 1)), x), dim=1)
+        y = self._forward(params, x)
+        if scalar:
+            y = y[0]
+        return y
+
+    @abc.abstractmethod
+    def _forward(self, params: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
+        """
+        The true forward method.
+
+        :param params: (N,D)
+        :param x: (N,L1)
+        :return: (N,L1-RF+1)
+        """
+        pass
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/_resources/loudness_input.wav` & `neural-amp-modeler-0.5.2/nam/models/_resources/loudness_input.wav`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.5.1/nam/models/base.py` & `neural-amp-modeler-0.5.2/nam/models/base.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,315 +1,315 @@
-# File: base.py
-# Created Date: Saturday February 5th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Implements the base PyTorch Lightning model.
-This is meant to combine an acutal model (subclassed from `._base.BaseNet` or 
-`._base.ParametricBaseNet`) along with loss function boilerplate.
-
-For the base *PyTorch* model containing the actual architecture, see `._base`.
-"""
-
-from dataclasses import dataclass
-from enum import Enum
-from typing import Optional, Tuple
-
-import auraloss
-import logging
-import pytorch_lightning as pl
-import torch
-import torch.nn as nn
-
-from .._core import InitializableFromConfig
-from .conv_net import ConvNet
-from .linear import Linear
-from .losses import esr, multi_resolution_stft_loss, mse_fft
-from .parametric.catnets import CatLSTM, CatWaveNet
-from .parametric.hyper_net import HyperConvNet
-from .recurrent import LSTM
-from .wavenet import WaveNet
-
-logger = logging.getLogger(__name__)
-
-
-class ValidationLoss(Enum):
-    """
-    mse: mean squared error
-    esr: error signal ratio (Eq. (10) from
-        https://www.mdpi.com/2076-3417/10/3/766/htm
-        NOTE: Be careful when computing ESR on minibatches! The average ESR over
-        a minibatch of data not the same as the ESR of all of the same data in
-        the minibatch calculated over at once (because of the denominator).
-        (Hint: think about what happens if one item in the minibatch is all
-        zeroes...)
-    """
-
-    MSE = "mse"
-    ESR = "esr"
-
-
-@dataclass
-class LossConfig(InitializableFromConfig):
-    """
-    :param mask_first: How many of the first samples to ignore when comptuing the loss.
-    :param dc_weight: Weight for the DC loss term. If 0, ignored.
-    :params val_loss: Which loss to track for the best model checkpoint.
-    :param pre_emph_coef: Coefficient of 1st-order pre-emphasis filter from
-        https://www.mdpi.com/2076-3417/10/3/766. Paper value: 0.95.
-    """
-
-    mrstft_weight: float = 0.0  # 0.0 means no multiresolution stft loss, 2e-4 works pretty well if one wants to use it
-    fourier: bool = False
-    mask_first: int = 0
-    dc_weight: float = 0.0
-    val_loss: ValidationLoss = ValidationLoss.MSE
-    pre_emph_weight: Optional[float] = None
-    pre_emph_coef: Optional[float] = None
-
-    @classmethod
-    def parse_config(cls, config):
-        config = super().parse_config(config)
-        fourier = config.get("fourier", False)
-        dc_weight = config.get("dc_weight", 0.0)
-        val_loss = ValidationLoss(config.get("val_loss", "mse"))
-        mask_first = config.get("mask_first", 0)
-        pre_emph_coef = config.get("pre_emph_coef")
-        pre_emph_weight = config.get("pre_emph_weight")
-        mrstft_weight = config.get("mstft_weight", 0.0)
-        return {
-            "fourier": fourier,
-            "mask_first": mask_first,
-            "dc_weight": dc_weight,
-            "val_loss": val_loss,
-            "pre_emph_coef": pre_emph_coef,
-            "pre_emph_weight": pre_emph_weight,
-            "mrstft_weight": mrstft_weight,
-        }
-
-    def apply_mask(self, *args):
-        """
-        :param args: (L,) or (B,)
-        :return: (L-M,) or (B, L-M)
-        """
-        return tuple(a[..., self.mask_first :] for a in args)
-
-
-class Model(pl.LightningModule, InitializableFromConfig):
-    def __init__(
-        self,
-        net,
-        optimizer_config: Optional[dict] = None,
-        scheduler_config: Optional[dict] = None,
-        loss_config: Optional[LossConfig] = None,
-    ):
-        """
-        :param scheduler_config: contains
-            Required:
-            * "class"
-            * "kwargs"
-            Optional (defaults to Lightning defaults):
-            * "interval" ("epoch" of "step")
-            * "frequency" (int)
-            * "monitor" (str)
-        """
-        super().__init__()
-        self._net = net
-        self._optimizer_config = {} if optimizer_config is None else optimizer_config
-        self._scheduler_config = scheduler_config
-        self._loss_config = LossConfig() if loss_config is None else loss_config
-        self._mrstft = None  # Multi-resolution short-time Fourier transform loss
-        # Where to compute the MRSTFT.
-        # Keeping it on-device is preferable, but if that fails, then remember to drop
-        # it to cpu from then on.
-        self._mrstft_device: Optional[torch.device] = None
-
-    @classmethod
-    def init_from_config(cls, config):
-        checkpoint_path = config.get("checkpoint_path")
-        config = cls.parse_config(config)
-        return (
-            cls(**config)
-            if checkpoint_path is None
-            else cls.load_from_checkpoint(checkpoint_path, **config)
-        )
-
-    @classmethod
-    def parse_config(cls, config):
-        """
-        e.g.
-
-        {
-            "net": {
-                "name": "ConvNet",
-                "config": {...}
-            },
-            "loss": {
-                "dc_weight": 0.1
-            },
-            "optimizer": {
-                "lr": 0.0003
-            },
-            "lr_scheduler": {
-                "class": "ReduceLROnPlateau",
-                "kwargs": {
-                    "factor": 0.8,
-                    "patience": 10,
-                    "cooldown": 15,
-                    "min_lr": 1e-06,
-                    "verbose": true
-                },
-                "monitor": "val_loss"
-            }
-        }
-        """
-        config = super().parse_config(config)
-        net_config = config["net"]
-        net = {
-            "CatLSTM": CatLSTM.init_from_config,
-            "CatWaveNet": CatWaveNet.init_from_config,
-            "ConvNet": ConvNet.init_from_config,
-            "HyperConvNet": HyperConvNet.init_from_config,
-            "Linear": Linear.init_from_config,
-            "LSTM": LSTM.init_from_config,
-            "WaveNet": WaveNet.init_from_config,
-        }[net_config["name"]](net_config["config"])
-        loss_config = LossConfig.init_from_config(config.get("loss", {}))
-        return {
-            "net": net,
-            "optimizer_config": config["optimizer"],
-            "scheduler_config": config["lr_scheduler"],
-            "loss_config": loss_config,
-        }
-
-    @property
-    def net(self) -> nn.Module:
-        return self._net
-
-    def configure_optimizers(self):
-        optimizer = torch.optim.Adam(self.parameters(), **self._optimizer_config)
-        if self._scheduler_config is None:
-            return optimizer
-        else:
-            lr_scheduler = getattr(
-                torch.optim.lr_scheduler, self._scheduler_config["class"]
-            )(optimizer, **self._scheduler_config["kwargs"])
-            lr_scheduler_config = {"scheduler": lr_scheduler}
-            for key in ("interval", "frequency", "monitor"):
-                if key in self._scheduler_config:
-                    lr_scheduler_config[key] = self._scheduler_config[key]
-            return {"optimizer": optimizer, "lr_scheduler": lr_scheduler_config}
-
-    def forward(self, *args, **kwargs):
-        return self.net(*args, **kwargs)
-
-    def _shared_step(self, batch) -> Tuple[torch.Tensor, torch.Tensor]:
-        """
-        B: Batch size
-        L: Sequence length
-
-        :return: (B,L), (B,L)
-        """
-        args, targets = batch[:-1], batch[-1]
-        preds = self(*args, pad_start=False)
-
-        return preds, targets
-
-    def training_step(self, batch, batch_idx):
-        preds, targets = self._shared_step(batch)
-
-        loss = 0.0
-        # Prediction aka MSE loss
-        if self._loss_config.fourier:
-            loss = loss + mse_fft(preds, targets)
-        else:
-            loss = loss + self._mse_loss(preds, targets)
-        if self._loss_config.mrstft_weight > 0.0:
-            loss = loss + self._loss_config.mrstft_weight * self._mrstft_loss(
-                preds, targets
-            )
-        # Pre-emphasized MSE
-        if self._loss_config.pre_emph_weight is not None:
-            if (self._loss_config.pre_emph_coef is None) != (
-                self._loss_config.pre_emph_weight is None
-            ):
-                raise ValueError("Invalid pre-emph")
-            loss = loss + self._loss_config.pre_emph_weight * self._mse_loss(
-                preds, targets, pre_emph_coef=self._loss_config.pre_emph_coef
-            )
-
-        # DC loss
-        dc_weight = self._loss_config.dc_weight
-        if dc_weight > 0.0:
-            # Denominator could be a bad idea. I'm going to omit it esp since I'm
-            # using mini batches
-            mean_dims = torch.arange(1, preds.ndim).tolist()
-            dc_loss = nn.MSELoss()(
-                preds.mean(dim=mean_dims), targets.mean(dim=mean_dims)
-            )
-            loss = loss + dc_weight * dc_loss
-        return loss
-
-    def validation_step(self, batch, batch_idx):
-        preds, targets = self._shared_step(batch)
-        mse_loss = self._mse_loss(preds, targets)
-        esr_loss = self._esr_loss(preds, targets)
-        val_loss = {ValidationLoss.MSE: mse_loss, ValidationLoss.ESR: esr_loss}[
-            self._loss_config.val_loss
-        ]
-        dict_to_log = {"MSE": mse_loss, "ESR": esr_loss, "val_loss": val_loss}
-        if self._loss_config.mrstft_weight > 0.0 and self._mrstft is not None:
-            mrstft_loss = self._mrstft_loss(preds, targets)
-            dict_to_log.update({"MRSTFT": mrstft_loss})
-        self.log_dict(dict_to_log)
-        return val_loss
-
-    def _esr_loss(self, preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
-        """
-        Error signal ratio aka ESR loss.
-
-        Eq. (10), from
-        https://www.mdpi.com/2076-3417/10/3/766/htm
-
-        B: Batch size
-        L: Sequence length
-
-        :param preds: (B,L)
-        :param targets: (B,L)
-        :return: ()
-        """
-        return esr(preds, targets)
-
-    def _mse_loss(self, preds, targets, pre_emph_coef: Optional[float] = None):
-        if pre_emph_coef is not None:
-            preds, targets = [
-                z[..., 1:] - pre_emph_coef * z[..., :-1] for z in (preds, targets)
-            ]
-        return nn.MSELoss()(preds, targets)
-
-    def _mrstft_loss(self, preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
-        """
-        Experimental Multi Resolution Short Time Fourier Transform Loss using auraloss implementation.
-        B: Batch size
-        L: Sequence length
-
-        :param preds: (B,L)
-        :param targets: (B,L)
-        :return: ()
-        """
-        if self._mrstft is None:
-            self._mrstft = auraloss.freq.MultiResolutionSTFTLoss()
-
-        backup_device = "cpu"
-
-        try:
-            return multi_resolution_stft_loss(
-                preds, targets, self._mrstft, device=self._mrstft_device
-            )
-        except Exception as e:
-            if self._mrstft_device == backup_device:
-                raise e
-            logger.warning("MRSTFT failed on device; falling back to CPU")
-            self._mrstft_device = backup_device
-            return multi_resolution_stft_loss(
-                preds, targets, self._mrstft, device=self._mrstft_device
-            )
+# File: base.py
+# Created Date: Saturday February 5th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Implements the base PyTorch Lightning model.
+This is meant to combine an acutal model (subclassed from `._base.BaseNet` or 
+`._base.ParametricBaseNet`) along with loss function boilerplate.
+
+For the base *PyTorch* model containing the actual architecture, see `._base`.
+"""
+
+from dataclasses import dataclass
+from enum import Enum
+from typing import Optional, Tuple
+
+import auraloss
+import logging
+import pytorch_lightning as pl
+import torch
+import torch.nn as nn
+
+from .._core import InitializableFromConfig
+from .conv_net import ConvNet
+from .linear import Linear
+from .losses import esr, multi_resolution_stft_loss, mse_fft
+from .parametric.catnets import CatLSTM, CatWaveNet
+from .parametric.hyper_net import HyperConvNet
+from .recurrent import LSTM
+from .wavenet import WaveNet
+
+logger = logging.getLogger(__name__)
+
+
+class ValidationLoss(Enum):
+    """
+    mse: mean squared error
+    esr: error signal ratio (Eq. (10) from
+        https://www.mdpi.com/2076-3417/10/3/766/htm
+        NOTE: Be careful when computing ESR on minibatches! The average ESR over
+        a minibatch of data not the same as the ESR of all of the same data in
+        the minibatch calculated over at once (because of the denominator).
+        (Hint: think about what happens if one item in the minibatch is all
+        zeroes...)
+    """
+
+    MSE = "mse"
+    ESR = "esr"
+
+
+@dataclass
+class LossConfig(InitializableFromConfig):
+    """
+    :param mask_first: How many of the first samples to ignore when comptuing the loss.
+    :param dc_weight: Weight for the DC loss term. If 0, ignored.
+    :params val_loss: Which loss to track for the best model checkpoint.
+    :param pre_emph_coef: Coefficient of 1st-order pre-emphasis filter from
+        https://www.mdpi.com/2076-3417/10/3/766. Paper value: 0.95.
+    """
+
+    mrstft_weight: float = 0.0  # 0.0 means no multiresolution stft loss, 2e-4 works pretty well if one wants to use it
+    fourier: bool = False
+    mask_first: int = 0
+    dc_weight: float = 0.0
+    val_loss: ValidationLoss = ValidationLoss.MSE
+    pre_emph_weight: Optional[float] = None
+    pre_emph_coef: Optional[float] = None
+
+    @classmethod
+    def parse_config(cls, config):
+        config = super().parse_config(config)
+        fourier = config.get("fourier", False)
+        dc_weight = config.get("dc_weight", 0.0)
+        val_loss = ValidationLoss(config.get("val_loss", "mse"))
+        mask_first = config.get("mask_first", 0)
+        pre_emph_coef = config.get("pre_emph_coef")
+        pre_emph_weight = config.get("pre_emph_weight")
+        mrstft_weight = config.get("mstft_weight", 0.0)
+        return {
+            "fourier": fourier,
+            "mask_first": mask_first,
+            "dc_weight": dc_weight,
+            "val_loss": val_loss,
+            "pre_emph_coef": pre_emph_coef,
+            "pre_emph_weight": pre_emph_weight,
+            "mrstft_weight": mrstft_weight,
+        }
+
+    def apply_mask(self, *args):
+        """
+        :param args: (L,) or (B,)
+        :return: (L-M,) or (B, L-M)
+        """
+        return tuple(a[..., self.mask_first :] for a in args)
+
+
+class Model(pl.LightningModule, InitializableFromConfig):
+    def __init__(
+        self,
+        net,
+        optimizer_config: Optional[dict] = None,
+        scheduler_config: Optional[dict] = None,
+        loss_config: Optional[LossConfig] = None,
+    ):
+        """
+        :param scheduler_config: contains
+            Required:
+            * "class"
+            * "kwargs"
+            Optional (defaults to Lightning defaults):
+            * "interval" ("epoch" of "step")
+            * "frequency" (int)
+            * "monitor" (str)
+        """
+        super().__init__()
+        self._net = net
+        self._optimizer_config = {} if optimizer_config is None else optimizer_config
+        self._scheduler_config = scheduler_config
+        self._loss_config = LossConfig() if loss_config is None else loss_config
+        self._mrstft = None  # Multi-resolution short-time Fourier transform loss
+        # Where to compute the MRSTFT.
+        # Keeping it on-device is preferable, but if that fails, then remember to drop
+        # it to cpu from then on.
+        self._mrstft_device: Optional[torch.device] = None
+
+    @classmethod
+    def init_from_config(cls, config):
+        checkpoint_path = config.get("checkpoint_path")
+        config = cls.parse_config(config)
+        return (
+            cls(**config)
+            if checkpoint_path is None
+            else cls.load_from_checkpoint(checkpoint_path, **config)
+        )
+
+    @classmethod
+    def parse_config(cls, config):
+        """
+        e.g.
+
+        {
+            "net": {
+                "name": "ConvNet",
+                "config": {...}
+            },
+            "loss": {
+                "dc_weight": 0.1
+            },
+            "optimizer": {
+                "lr": 0.0003
+            },
+            "lr_scheduler": {
+                "class": "ReduceLROnPlateau",
+                "kwargs": {
+                    "factor": 0.8,
+                    "patience": 10,
+                    "cooldown": 15,
+                    "min_lr": 1e-06,
+                    "verbose": true
+                },
+                "monitor": "val_loss"
+            }
+        }
+        """
+        config = super().parse_config(config)
+        net_config = config["net"]
+        net = {
+            "CatLSTM": CatLSTM.init_from_config,
+            "CatWaveNet": CatWaveNet.init_from_config,
+            "ConvNet": ConvNet.init_from_config,
+            "HyperConvNet": HyperConvNet.init_from_config,
+            "Linear": Linear.init_from_config,
+            "LSTM": LSTM.init_from_config,
+            "WaveNet": WaveNet.init_from_config,
+        }[net_config["name"]](net_config["config"])
+        loss_config = LossConfig.init_from_config(config.get("loss", {}))
+        return {
+            "net": net,
+            "optimizer_config": config["optimizer"],
+            "scheduler_config": config["lr_scheduler"],
+            "loss_config": loss_config,
+        }
+
+    @property
+    def net(self) -> nn.Module:
+        return self._net
+
+    def configure_optimizers(self):
+        optimizer = torch.optim.Adam(self.parameters(), **self._optimizer_config)
+        if self._scheduler_config is None:
+            return optimizer
+        else:
+            lr_scheduler = getattr(
+                torch.optim.lr_scheduler, self._scheduler_config["class"]
+            )(optimizer, **self._scheduler_config["kwargs"])
+            lr_scheduler_config = {"scheduler": lr_scheduler}
+            for key in ("interval", "frequency", "monitor"):
+                if key in self._scheduler_config:
+                    lr_scheduler_config[key] = self._scheduler_config[key]
+            return {"optimizer": optimizer, "lr_scheduler": lr_scheduler_config}
+
+    def forward(self, *args, **kwargs):
+        return self.net(*args, **kwargs)
+
+    def _shared_step(self, batch) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        B: Batch size
+        L: Sequence length
+
+        :return: (B,L), (B,L)
+        """
+        args, targets = batch[:-1], batch[-1]
+        preds = self(*args, pad_start=False)
+
+        return preds, targets
+
+    def training_step(self, batch, batch_idx):
+        preds, targets = self._shared_step(batch)
+
+        loss = 0.0
+        # Prediction aka MSE loss
+        if self._loss_config.fourier:
+            loss = loss + mse_fft(preds, targets)
+        else:
+            loss = loss + self._mse_loss(preds, targets)
+        if self._loss_config.mrstft_weight > 0.0:
+            loss = loss + self._loss_config.mrstft_weight * self._mrstft_loss(
+                preds, targets
+            )
+        # Pre-emphasized MSE
+        if self._loss_config.pre_emph_weight is not None:
+            if (self._loss_config.pre_emph_coef is None) != (
+                self._loss_config.pre_emph_weight is None
+            ):
+                raise ValueError("Invalid pre-emph")
+            loss = loss + self._loss_config.pre_emph_weight * self._mse_loss(
+                preds, targets, pre_emph_coef=self._loss_config.pre_emph_coef
+            )
+
+        # DC loss
+        dc_weight = self._loss_config.dc_weight
+        if dc_weight > 0.0:
+            # Denominator could be a bad idea. I'm going to omit it esp since I'm
+            # using mini batches
+            mean_dims = torch.arange(1, preds.ndim).tolist()
+            dc_loss = nn.MSELoss()(
+                preds.mean(dim=mean_dims), targets.mean(dim=mean_dims)
+            )
+            loss = loss + dc_weight * dc_loss
+        return loss
+
+    def validation_step(self, batch, batch_idx):
+        preds, targets = self._shared_step(batch)
+        mse_loss = self._mse_loss(preds, targets)
+        esr_loss = self._esr_loss(preds, targets)
+        val_loss = {ValidationLoss.MSE: mse_loss, ValidationLoss.ESR: esr_loss}[
+            self._loss_config.val_loss
+        ]
+        dict_to_log = {"MSE": mse_loss, "ESR": esr_loss, "val_loss": val_loss}
+        if self._loss_config.mrstft_weight > 0.0 and self._mrstft is not None:
+            mrstft_loss = self._mrstft_loss(preds, targets)
+            dict_to_log.update({"MRSTFT": mrstft_loss})
+        self.log_dict(dict_to_log)
+        return val_loss
+
+    def _esr_loss(self, preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
+        """
+        Error signal ratio aka ESR loss.
+
+        Eq. (10), from
+        https://www.mdpi.com/2076-3417/10/3/766/htm
+
+        B: Batch size
+        L: Sequence length
+
+        :param preds: (B,L)
+        :param targets: (B,L)
+        :return: ()
+        """
+        return esr(preds, targets)
+
+    def _mse_loss(self, preds, targets, pre_emph_coef: Optional[float] = None):
+        if pre_emph_coef is not None:
+            preds, targets = [
+                z[..., 1:] - pre_emph_coef * z[..., :-1] for z in (preds, targets)
+            ]
+        return nn.MSELoss()(preds, targets)
+
+    def _mrstft_loss(self, preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
+        """
+        Experimental Multi Resolution Short Time Fourier Transform Loss using auraloss implementation.
+        B: Batch size
+        L: Sequence length
+
+        :param preds: (B,L)
+        :param targets: (B,L)
+        :return: ()
+        """
+        if self._mrstft is None:
+            self._mrstft = auraloss.freq.MultiResolutionSTFTLoss()
+
+        backup_device = "cpu"
+
+        try:
+            return multi_resolution_stft_loss(
+                preds, targets, self._mrstft, device=self._mrstft_device
+            )
+        except Exception as e:
+            if self._mrstft_device == backup_device:
+                raise e
+            logger.warning("MRSTFT failed on device; falling back to CPU")
+            self._mrstft_device = backup_device
+            return multi_resolution_stft_loss(
+                preds, targets, self._mrstft, device=self._mrstft_device
+            )
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/conv_net.py` & `neural-amp-modeler-0.5.2/nam/models/conv_net.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,290 +1,290 @@
-# File: conv_net.py
-# Created Date: Saturday February 5th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-import json
-import math
-from enum import Enum
-from functools import partial
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Optional, Sequence, Tuple, Union
-
-import numpy as np
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-
-from .. import __version__
-from ..data import REQUIRED_RATE, wav_to_tensor
-from ._activations import get_activation
-from ._base import BaseNet
-from ._names import ACTIVATION_NAME, BATCHNORM_NAME, CONV_NAME
-
-
-class TrainStrategy(Enum):
-    STRIDE = "stride"
-    DILATE = "dilate"
-
-
-default_train_strategy = TrainStrategy.DILATE
-
-
-class _Functional(nn.Module):
-    """
-    Define a layer by a function w/ no params
-    """
-
-    def __init__(self, op):
-        super().__init__()
-        self._op = op
-
-    def forward(self, *args, **kwargs):
-        return self._op(*args, **kwargs)
-
-
-class _IR(nn.Module):
-    def __init__(self, filename: Union[str, Path]):
-        super().__init__()
-        self.register_buffer("_weight", reversed(wav_to_tensor(filename))[None, None])
-
-    @property
-    def length(self) -> int:
-        return self._weight.shape[-1]
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        :param x: (N,D)
-        :return: (N,D-length+1)
-        """
-        return F.conv1d(x[:, None], self._weight)[:, 0]
-
-
-def _conv_net(
-    channels: int = 32,
-    dilations: Sequence[int] = None,
-    batchnorm: bool = False,
-    activation: str = "Tanh",
-) -> nn.Sequential:
-    def block(cin, cout, dilation):
-        net = nn.Sequential()
-        net.add_module(
-            CONV_NAME, nn.Conv1d(cin, cout, 2, dilation=dilation, bias=not batchnorm)
-        )
-        if batchnorm:
-            net.add_module(BATCHNORM_NAME, nn.BatchNorm1d(cout))
-        net.add_module(ACTIVATION_NAME, get_activation(activation))
-        return net
-
-    def check_and_expand(n, x):
-        if x.shape[1] < n:
-            raise ValueError(
-                f"Input of length {x.shape[1]} is shorter than model receptive field ({n})"
-            )
-        return x[:, None, :]
-
-    dilations = [1, 2, 4, 8] if dilations is None else dilations
-    receptive_field = sum(dilations) + 1
-    net = nn.Sequential()
-    net.add_module("expand", _Functional(partial(check_and_expand, receptive_field)))
-    cin = 1
-    cout = channels
-    for i, dilation in enumerate(dilations):
-        net.add_module(f"block_{i}", block(cin, cout, dilation))
-        cin = cout
-    net.add_module("head", nn.Conv1d(channels, 1, 1))
-    net.add_module("flatten", nn.Flatten())
-    return net
-
-
-class ConvNet(BaseNet):
-    """
-    A straightforward convolutional neural network.
-
-    Works surprisingly well!
-    """
-
-    def __init__(
-        self,
-        *args,
-        train_strategy: TrainStrategy = default_train_strategy,
-        ir: Optional[_IR] = None,
-        **kwargs,
-    ):
-        super().__init__()
-        self._net = _conv_net(*args, **kwargs)
-        assert train_strategy == TrainStrategy.DILATE, "Stride no longer supported"
-        self._train_strategy = train_strategy
-        self._num_blocks = self._get_num_blocks(self._net)
-        self._pad_start_default = True
-        self._ir = ir
-
-    @classmethod
-    def parse_config(cls, config):
-        config = super().parse_config(config)
-        config["train_strategy"] = TrainStrategy(
-            config.get("train_strategy", default_train_strategy.value)
-        )
-        config["ir"] = (
-            None if "ir_filename" not in config else _IR(config.pop("ir_filename"))
-        )
-        return config
-
-    @property
-    def pad_start_default(self) -> bool:
-        return self._pad_start_default
-
-    @property
-    def receptive_field(self) -> int:
-        net_rf = 1 + sum(
-            self._net._modules[f"block_{i}"]._modules["conv"].dilation[0]
-            for i in range(self._num_blocks)
-        )
-        # Minus 1 because it composes w/ the net
-        ir_rf = 0 if self._ir is None else self._ir.length - 1
-        return net_rf + ir_rf
-
-    @property
-    def _activation(self):
-        return (
-            self._net._modules["block_0"]._modules[ACTIVATION_NAME].__class__.__name__
-        )
-
-    @property
-    def _channels(self) -> int:
-        return self._net._modules["block_0"]._modules[CONV_NAME].weight.shape[0]
-
-    @property
-    def _num_layers(self) -> int:
-        return self._num_blocks
-
-    @property
-    def _batchnorm(self) -> bool:
-        return BATCHNORM_NAME in self._net._modules["block_0"]._modules
-
-    def export_cpp_header(self, filename: Path):
-        with TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir)
-            self.export(Path(tmpdir))
-            with open(Path(tmpdir, "config.json"), "r") as fp:
-                _c = json.load(fp)
-            version = _c["version"]
-            config = _c["config"]
-            with open(filename, "w") as f:
-                f.writelines(
-                    (
-                        "#pragma once\n",
-                        "// Automatically-generated model file\n",
-                        "#include <vector>\n",
-                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
-                        f"const int CHANNELS = {config['channels']};\n",
-                        f"const bool BATCHNORM = {'true' if config['batchnorm'] else 'false'};\n",
-                        "std::vector<int> DILATIONS{"
-                        + ",".join([str(d) for d in config["dilations"]])
-                        + "};\n",
-                        f"const std::string ACTIVATION = \"{config['activation']}\";\n",
-                        "std::vector<float> PARAMS{"
-                        + ",".join(
-                            [f"{w:.16f}" for w in np.load(Path(tmpdir, "weights.npy"))]
-                        )
-                        + "};\n",
-                    )
-                )
-
-    def _export_config(self):
-        return {
-            "channels": self._channels,
-            "dilations": self._get_dilations(),
-            "batchnorm": self._batchnorm,
-            "activation": self._activation,
-        }
-
-    def _export_input_output(self, x=None) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        :return: (L,), (L,)
-        """
-        with torch.no_grad():
-            training = self.training
-            self.eval()
-            x = self._export_input_signal() if x is None else x
-            y = self(x, pad_start=True)
-            self.train(training)
-            return tuple(z.detach().cpu().numpy() for z in (x, y))
-
-    def _export_input_signal(self):
-        """
-        :return: (L,)
-        """
-        rate = REQUIRED_RATE
-        return torch.cat(
-            [
-                torch.zeros((rate,)),
-                0.5
-                * torch.sin(
-                    2.0 * math.pi * 220.0 * torch.linspace(0.0, 1.0, rate + 1)[:-1]
-                ),
-                torch.zeros((rate,)),
-            ]
-        )
-
-    def _export_weights(self) -> np.ndarray:
-        """
-        weights are serialized to weights.npy in the following order:
-        * (expand: no params)
-        * loop blocks 0,...,L-1
-            * conv:
-                * weight (Cout, Cin, K)
-                * bias (if no batchnorm) (Cout)
-            * BN
-                * running mean
-                * running_var
-                * weight (Cout)
-                * bias (Cout)
-                * eps ()
-        * head
-            * weight (C, 1, 1)
-            * bias (1, 1)
-        * (flatten: no params)
-        """
-        params = []
-        for i in range(self._num_layers):
-            block_name = f"block_{i}"
-            block = self._net._modules[block_name]
-            conv = block._modules[CONV_NAME]
-            params.append(conv.weight.flatten())
-            if conv.bias is not None:
-                params.append(conv.bias.flatten())
-            if self._batchnorm:
-                bn = block._modules[BATCHNORM_NAME]
-                params.append(bn.running_mean.flatten())
-                params.append(bn.running_var.flatten())
-                params.append(bn.weight.flatten())
-                params.append(bn.bias.flatten())
-                params.append(torch.Tensor([bn.eps]).to(bn.weight.device))
-        head = self._net._modules["head"]
-        params.append(head.weight.flatten())
-        params.append(head.bias.flatten())
-        params = torch.cat(params).detach().cpu().numpy()
-        return params
-
-    def _forward(self, x):
-        y = self._net(x)
-        if self._ir is not None:
-            y = self._ir(y)
-        return y
-
-    def _get_dilations(self) -> Tuple[int]:
-        return tuple(
-            self._net._modules[f"block_{i}"]._modules[CONV_NAME].dilation[0]
-            for i in range(self._num_blocks)
-        )
-
-    def _get_num_blocks(self, net: nn.Sequential):
-        i = 0
-        while True:
-            if f"block_{i}" not in net._modules:
-                break
-            else:
-                i += 1
-        return i
+# File: conv_net.py
+# Created Date: Saturday February 5th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+import json
+import math
+from enum import Enum
+from functools import partial
+from pathlib import Path
+from tempfile import TemporaryDirectory
+from typing import Optional, Sequence, Tuple, Union
+
+import numpy as np
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+
+from .. import __version__
+from ..data import REQUIRED_RATE, wav_to_tensor
+from ._activations import get_activation
+from ._base import BaseNet
+from ._names import ACTIVATION_NAME, BATCHNORM_NAME, CONV_NAME
+
+
+class TrainStrategy(Enum):
+    STRIDE = "stride"
+    DILATE = "dilate"
+
+
+default_train_strategy = TrainStrategy.DILATE
+
+
+class _Functional(nn.Module):
+    """
+    Define a layer by a function w/ no params
+    """
+
+    def __init__(self, op):
+        super().__init__()
+        self._op = op
+
+    def forward(self, *args, **kwargs):
+        return self._op(*args, **kwargs)
+
+
+class _IR(nn.Module):
+    def __init__(self, filename: Union[str, Path]):
+        super().__init__()
+        self.register_buffer("_weight", reversed(wav_to_tensor(filename))[None, None])
+
+    @property
+    def length(self) -> int:
+        return self._weight.shape[-1]
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        :param x: (N,D)
+        :return: (N,D-length+1)
+        """
+        return F.conv1d(x[:, None], self._weight)[:, 0]
+
+
+def _conv_net(
+    channels: int = 32,
+    dilations: Sequence[int] = None,
+    batchnorm: bool = False,
+    activation: str = "Tanh",
+) -> nn.Sequential:
+    def block(cin, cout, dilation):
+        net = nn.Sequential()
+        net.add_module(
+            CONV_NAME, nn.Conv1d(cin, cout, 2, dilation=dilation, bias=not batchnorm)
+        )
+        if batchnorm:
+            net.add_module(BATCHNORM_NAME, nn.BatchNorm1d(cout))
+        net.add_module(ACTIVATION_NAME, get_activation(activation))
+        return net
+
+    def check_and_expand(n, x):
+        if x.shape[1] < n:
+            raise ValueError(
+                f"Input of length {x.shape[1]} is shorter than model receptive field ({n})"
+            )
+        return x[:, None, :]
+
+    dilations = [1, 2, 4, 8] if dilations is None else dilations
+    receptive_field = sum(dilations) + 1
+    net = nn.Sequential()
+    net.add_module("expand", _Functional(partial(check_and_expand, receptive_field)))
+    cin = 1
+    cout = channels
+    for i, dilation in enumerate(dilations):
+        net.add_module(f"block_{i}", block(cin, cout, dilation))
+        cin = cout
+    net.add_module("head", nn.Conv1d(channels, 1, 1))
+    net.add_module("flatten", nn.Flatten())
+    return net
+
+
+class ConvNet(BaseNet):
+    """
+    A straightforward convolutional neural network.
+
+    Works surprisingly well!
+    """
+
+    def __init__(
+        self,
+        *args,
+        train_strategy: TrainStrategy = default_train_strategy,
+        ir: Optional[_IR] = None,
+        **kwargs,
+    ):
+        super().__init__()
+        self._net = _conv_net(*args, **kwargs)
+        assert train_strategy == TrainStrategy.DILATE, "Stride no longer supported"
+        self._train_strategy = train_strategy
+        self._num_blocks = self._get_num_blocks(self._net)
+        self._pad_start_default = True
+        self._ir = ir
+
+    @classmethod
+    def parse_config(cls, config):
+        config = super().parse_config(config)
+        config["train_strategy"] = TrainStrategy(
+            config.get("train_strategy", default_train_strategy.value)
+        )
+        config["ir"] = (
+            None if "ir_filename" not in config else _IR(config.pop("ir_filename"))
+        )
+        return config
+
+    @property
+    def pad_start_default(self) -> bool:
+        return self._pad_start_default
+
+    @property
+    def receptive_field(self) -> int:
+        net_rf = 1 + sum(
+            self._net._modules[f"block_{i}"]._modules["conv"].dilation[0]
+            for i in range(self._num_blocks)
+        )
+        # Minus 1 because it composes w/ the net
+        ir_rf = 0 if self._ir is None else self._ir.length - 1
+        return net_rf + ir_rf
+
+    @property
+    def _activation(self):
+        return (
+            self._net._modules["block_0"]._modules[ACTIVATION_NAME].__class__.__name__
+        )
+
+    @property
+    def _channels(self) -> int:
+        return self._net._modules["block_0"]._modules[CONV_NAME].weight.shape[0]
+
+    @property
+    def _num_layers(self) -> int:
+        return self._num_blocks
+
+    @property
+    def _batchnorm(self) -> bool:
+        return BATCHNORM_NAME in self._net._modules["block_0"]._modules
+
+    def export_cpp_header(self, filename: Path):
+        with TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir)
+            self.export(Path(tmpdir))
+            with open(Path(tmpdir, "config.json"), "r") as fp:
+                _c = json.load(fp)
+            version = _c["version"]
+            config = _c["config"]
+            with open(filename, "w") as f:
+                f.writelines(
+                    (
+                        "#pragma once\n",
+                        "// Automatically-generated model file\n",
+                        "#include <vector>\n",
+                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
+                        f"const int CHANNELS = {config['channels']};\n",
+                        f"const bool BATCHNORM = {'true' if config['batchnorm'] else 'false'};\n",
+                        "std::vector<int> DILATIONS{"
+                        + ",".join([str(d) for d in config["dilations"]])
+                        + "};\n",
+                        f"const std::string ACTIVATION = \"{config['activation']}\";\n",
+                        "std::vector<float> PARAMS{"
+                        + ",".join(
+                            [f"{w:.16f}" for w in np.load(Path(tmpdir, "weights.npy"))]
+                        )
+                        + "};\n",
+                    )
+                )
+
+    def _export_config(self):
+        return {
+            "channels": self._channels,
+            "dilations": self._get_dilations(),
+            "batchnorm": self._batchnorm,
+            "activation": self._activation,
+        }
+
+    def _export_input_output(self, x=None) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        :return: (L,), (L,)
+        """
+        with torch.no_grad():
+            training = self.training
+            self.eval()
+            x = self._export_input_signal() if x is None else x
+            y = self(x, pad_start=True)
+            self.train(training)
+            return tuple(z.detach().cpu().numpy() for z in (x, y))
+
+    def _export_input_signal(self):
+        """
+        :return: (L,)
+        """
+        rate = REQUIRED_RATE
+        return torch.cat(
+            [
+                torch.zeros((rate,)),
+                0.5
+                * torch.sin(
+                    2.0 * math.pi * 220.0 * torch.linspace(0.0, 1.0, rate + 1)[:-1]
+                ),
+                torch.zeros((rate,)),
+            ]
+        )
+
+    def _export_weights(self) -> np.ndarray:
+        """
+        weights are serialized to weights.npy in the following order:
+        * (expand: no params)
+        * loop blocks 0,...,L-1
+            * conv:
+                * weight (Cout, Cin, K)
+                * bias (if no batchnorm) (Cout)
+            * BN
+                * running mean
+                * running_var
+                * weight (Cout)
+                * bias (Cout)
+                * eps ()
+        * head
+            * weight (C, 1, 1)
+            * bias (1, 1)
+        * (flatten: no params)
+        """
+        params = []
+        for i in range(self._num_layers):
+            block_name = f"block_{i}"
+            block = self._net._modules[block_name]
+            conv = block._modules[CONV_NAME]
+            params.append(conv.weight.flatten())
+            if conv.bias is not None:
+                params.append(conv.bias.flatten())
+            if self._batchnorm:
+                bn = block._modules[BATCHNORM_NAME]
+                params.append(bn.running_mean.flatten())
+                params.append(bn.running_var.flatten())
+                params.append(bn.weight.flatten())
+                params.append(bn.bias.flatten())
+                params.append(torch.Tensor([bn.eps]).to(bn.weight.device))
+        head = self._net._modules["head"]
+        params.append(head.weight.flatten())
+        params.append(head.bias.flatten())
+        params = torch.cat(params).detach().cpu().numpy()
+        return params
+
+    def _forward(self, x):
+        y = self._net(x)
+        if self._ir is not None:
+            y = self._ir(y)
+        return y
+
+    def _get_dilations(self) -> Tuple[int]:
+        return tuple(
+            self._net._modules[f"block_{i}"]._modules[CONV_NAME].dilation[0]
+            for i in range(self._num_blocks)
+        )
+
+    def _get_num_blocks(self, net: nn.Sequential):
+        i = 0
+        while True:
+            if f"block_{i}" not in net._modules:
+                break
+            else:
+                i += 1
+        return i
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/linear.py` & `neural-amp-modeler-0.5.2/nam/models/linear.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# File: linear.py
-# Created Date: Tuesday February 8th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Linear model
-"""
-
-import json
-from pathlib import Path
-
-import numpy as np
-import torch
-import torch.nn as nn
-
-from .._version import __version__
-from ._base import BaseNet
-
-
-class Linear(BaseNet):
-    def __init__(self, receptive_field: int, bias: bool = False):
-        super().__init__()
-        self._net = nn.Conv1d(1, 1, receptive_field, bias=bias)
-
-    @property
-    def pad_start_default(self) -> bool:
-        return True
-
-    @property
-    def receptive_field(self) -> int:
-        return self._net.weight.shape[2]
-
-    def export(self, outdir: Path):
-        training = self.training
-        self.eval()
-        with open(Path(outdir, "config.json"), "w") as fp:
-            json.dump(
-                {
-                    "version": __version__,
-                    "architecture": self.__class__.__name__,
-                    "config": {
-                        "receptive_field": self.receptive_field,
-                        "bias": self._bias,
-                    },
-                },
-                fp,
-                indent=4,
-            )
-
-        params = [self._net.weight.flatten()]
-        if self._bias:
-            params.append(self._net.bias.flatten())
-        params = torch.cat(params).detach().cpu().numpy()
-        # Hope I don't regret using np.save...
-        np.save(Path(outdir, "weights.npy"), params)
-
-        # And an input/output to verify correct computation:
-        x, y = self._export_input_output()
-        np.save(Path(outdir, "input.npy"), x.detach().cpu().numpy())
-        np.save(Path(outdir, "output.npy"), y.detach().cpu().numpy())
-
-        # And resume training state
-        self.train(training)
-
-    @property
-    def _bias(self) -> bool:
-        return self._net.bias is not None
-
-    def _forward(self, x: torch.Tensor) -> torch.Tensor:
-        return self._net(x[:, None])[:, 0]
+# File: linear.py
+# Created Date: Tuesday February 8th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Linear model
+"""
+
+import json
+from pathlib import Path
+
+import numpy as np
+import torch
+import torch.nn as nn
+
+from .._version import __version__
+from ._base import BaseNet
+
+
+class Linear(BaseNet):
+    def __init__(self, receptive_field: int, bias: bool = False):
+        super().__init__()
+        self._net = nn.Conv1d(1, 1, receptive_field, bias=bias)
+
+    @property
+    def pad_start_default(self) -> bool:
+        return True
+
+    @property
+    def receptive_field(self) -> int:
+        return self._net.weight.shape[2]
+
+    def export(self, outdir: Path):
+        training = self.training
+        self.eval()
+        with open(Path(outdir, "config.json"), "w") as fp:
+            json.dump(
+                {
+                    "version": __version__,
+                    "architecture": self.__class__.__name__,
+                    "config": {
+                        "receptive_field": self.receptive_field,
+                        "bias": self._bias,
+                    },
+                },
+                fp,
+                indent=4,
+            )
+
+        params = [self._net.weight.flatten()]
+        if self._bias:
+            params.append(self._net.bias.flatten())
+        params = torch.cat(params).detach().cpu().numpy()
+        # Hope I don't regret using np.save...
+        np.save(Path(outdir, "weights.npy"), params)
+
+        # And an input/output to verify correct computation:
+        x, y = self._export_input_output()
+        np.save(Path(outdir, "input.npy"), x.detach().cpu().numpy())
+        np.save(Path(outdir, "output.npy"), y.detach().cpu().numpy())
+
+        # And resume training state
+        self.train(training)
+
+    @property
+    def _bias(self) -> bool:
+        return self._net.bias is not None
+
+    def _forward(self, x: torch.Tensor) -> torch.Tensor:
+        return self._net(x[:, None])[:, 0]
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/losses.py` & `neural-amp-modeler-0.5.2/nam/models/losses.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# File: losses.py
-# Created Date: Sunday January 22nd 2023
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Loss functions
-"""
-
-from typing import Optional
-
-import torch
-from auraloss.freq import MultiResolutionSTFTLoss
-
-___all__ = ["esr", "multi_resolution_stft_loss"]
-
-
-def esr(preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
-    """
-    ESR of (a batch of) predictions & targets
-
-    :param preds: (N,) or (B,N)
-    :param targets: Same as preds
-    :return: ()
-    """
-    if preds.ndim == 1 and targets.ndim == 1:
-        preds, targets = preds[None], targets[None]
-    if preds.ndim != 2:
-        raise ValueError(
-            f"Expect 2D predictions (batch_size, num_samples). Got {preds.shape}"
-        )
-    if targets.ndim != 2:
-        raise ValueError(
-            f"Expect 2D targets (batch_size, num_samples). Got {targets.shape}"
-        )
-    return torch.mean(
-        torch.mean(torch.square(preds - targets), dim=1)
-        / torch.mean(torch.square(targets), dim=1)
-    )
-
-
-def multi_resolution_stft_loss(
-    preds: torch.Tensor,
-    targets: torch.Tensor,
-    loss_func: Optional[MultiResolutionSTFTLoss] = None,
-    device: Optional[torch.device] = None,
-) -> torch.Tensor:
-    """
-    Experimental Multi Resolution Short Time Fourier Transform Loss using auraloss implementation.
-    B: Batch size
-    L: Sequence length
-
-    :param preds: (B,L)
-    :param targets: (B,L)
-    :param loss_func: A pre-initialized instance of the loss function module. Providing
-        this saves time.
-    :param device: If provided, send the preds and targets to the provided device.
-    :return: ()
-    """
-    loss_func = MultiResolutionSTFTLoss() if loss_func is None else loss_func
-    if device is not None:
-        preds, targets = [z.to(device) for z in (preds, targets)]
-    return loss_func(preds, targets)
-
-
-def mse_fft(preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
-    """
-    Fourier loss
-
-    :param preds: (N,) or (B,N)
-    :param targets: Same as preds
-    :return: ()
-    """
-    fp = torch.fft.fft(preds)
-    ft = torch.fft.fft(targets)
-    e = fp - ft
-    return torch.mean(torch.square(e.abs()))
+# File: losses.py
+# Created Date: Sunday January 22nd 2023
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Loss functions
+"""
+
+from typing import Optional
+
+import torch
+from auraloss.freq import MultiResolutionSTFTLoss
+
+___all__ = ["esr", "multi_resolution_stft_loss"]
+
+
+def esr(preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
+    """
+    ESR of (a batch of) predictions & targets
+
+    :param preds: (N,) or (B,N)
+    :param targets: Same as preds
+    :return: ()
+    """
+    if preds.ndim == 1 and targets.ndim == 1:
+        preds, targets = preds[None], targets[None]
+    if preds.ndim != 2:
+        raise ValueError(
+            f"Expect 2D predictions (batch_size, num_samples). Got {preds.shape}"
+        )
+    if targets.ndim != 2:
+        raise ValueError(
+            f"Expect 2D targets (batch_size, num_samples). Got {targets.shape}"
+        )
+    return torch.mean(
+        torch.mean(torch.square(preds - targets), dim=1)
+        / torch.mean(torch.square(targets), dim=1)
+    )
+
+
+def multi_resolution_stft_loss(
+    preds: torch.Tensor,
+    targets: torch.Tensor,
+    loss_func: Optional[MultiResolutionSTFTLoss] = None,
+    device: Optional[torch.device] = None,
+) -> torch.Tensor:
+    """
+    Experimental Multi Resolution Short Time Fourier Transform Loss using auraloss implementation.
+    B: Batch size
+    L: Sequence length
+
+    :param preds: (B,L)
+    :param targets: (B,L)
+    :param loss_func: A pre-initialized instance of the loss function module. Providing
+        this saves time.
+    :param device: If provided, send the preds and targets to the provided device.
+    :return: ()
+    """
+    loss_func = MultiResolutionSTFTLoss() if loss_func is None else loss_func
+    if device is not None:
+        preds, targets = [z.to(device) for z in (preds, targets)]
+    return loss_func(preds, targets)
+
+
+def mse_fft(preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
+    """
+    Fourier loss
+
+    :param preds: (N,) or (B,N)
+    :param targets: Same as preds
+    :return: ()
+    """
+    fp = torch.fft.fft(preds)
+    ft = torch.fft.fft(targets)
+    e = fp - ft
+    return torch.mean(torch.square(e.abs()))
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/metadata.py` & `neural-amp-modeler-0.5.2/nam/models/metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-# File: metadata.py
-# Created Date: Wednesday April 12th 2023
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Metadata about models
-"""
-
-from enum import Enum
-from typing import Optional
-
-from pydantic import BaseModel
-
-__all__ = ["GearType", "ToneType", "Date", "UserMetadata"]
-
-
-class GearType(Enum):
-    AMP = "amp"
-    PEDAL = "pedal"
-    AMP_CAB = "amp_cab"
-    AMP_PEDAL_CAB = "amp_pedal_cab"
-    PREAMP = "preamp"
-    STUDIO = "studio"
-
-
-class ToneType(Enum):
-    CLEAN = "clean"
-    OVERDRIVE = "overdrive"
-    CRUNCH = "crunch"
-    HI_GAIN = "hi_gain"
-    FUZZ = "fuzz"
-
-
-class Date(BaseModel):
-    year: int
-    month: int
-    day: int
-    hour: int
-    minute: int
-    second: int
-
-
-class UserMetadata(BaseModel):
-    """
-    Metadata that users provide for a NAM model
-    """
-
-    name: Optional[str] = None
-    modeled_by: Optional[str] = None
-    gear_type: Optional[GearType] = None
-    gear_make: Optional[str] = None
-    gear_model: Optional[str] = None
-    tone_type: Optional[ToneType] = None
+# File: metadata.py
+# Created Date: Wednesday April 12th 2023
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Metadata about models
+"""
+
+from enum import Enum
+from typing import Optional
+
+from pydantic import BaseModel
+
+__all__ = ["GearType", "ToneType", "Date", "UserMetadata"]
+
+
+# Note: if you change this enum, you need to update the options in easy_colab.ipynb!
+class GearType(Enum):
+    AMP = "amp"
+    PEDAL = "pedal"
+    AMP_CAB = "amp_cab"
+    AMP_PEDAL_CAB = "amp_pedal_cab"
+    PREAMP = "preamp"
+    STUDIO = "studio"
+
+# Note: if you change this enum, you need to update the options in easy_colab.ipynb!
+class ToneType(Enum):
+    CLEAN = "clean"
+    OVERDRIVE = "overdrive"
+    CRUNCH = "crunch"
+    HI_GAIN = "hi_gain"
+    FUZZ = "fuzz"
+
+
+class Date(BaseModel):
+    year: int
+    month: int
+    day: int
+    hour: int
+    minute: int
+    second: int
+
+
+class UserMetadata(BaseModel):
+    """
+    Metadata that users provide for a NAM model
+    """
+
+    name: Optional[str] = None
+    modeled_by: Optional[str] = None
+    gear_type: Optional[GearType] = None
+    gear_make: Optional[str] = None
+    gear_model: Optional[str] = None
+    tone_type: Optional[ToneType] = None
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/parametric/catnets.py` & `neural-amp-modeler-0.5.2/nam/models/parametric/catnets.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-# File: catnets.py
-# Created Date: Wednesday June 22nd 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-"Cat nets" -- parametric models where the parametric input is concatenated to the
-input samples
-"""
-
-import abc
-import logging
-from enum import Enum
-from contextlib import contextmanager
-from pathlib import Path
-from typing import Any, Dict, Tuple
-
-import numpy as np
-import torch
-
-from .._base import ParametricBaseNet
-from ..recurrent import LSTM
-from ..wavenet import WaveNet
-from .params import Param
-
-logger = logging.getLogger(__name__)
-
-
-class _ShapeType(Enum):
-    CONV = "conv"  # (B,C,L)
-    RNN = "rnn"  # (B,L,D)
-
-
-class _CatMixin(ParametricBaseNet):
-    """
-    Parameteric nets that concatenate the params with the input at each time point
-    Mix in with a non-parametric class like
-
-    ```
-    class CatLSTM(LSTM, _CatMixin):
-        pass
-    ```
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        # Hacky, see .export()
-        self._sidedoor_parametric_config = None
-
-    @abc.abstractproperty
-    def _shape_type(self) -> _ShapeType:
-        pass
-
-    @abc.abstractproperty
-    def _single_class(self):
-        """ "
-        The class for the non-parametric model that this is extending
-        """
-        # TODO verify that single class satisfies requirements
-        # ._export_weights()
-        # ._export_input_output()
-        pass  # HACK
-
-    def export(self, outdir: Path, parametric_config: Dict[str, Param], **kwargs):
-        """
-        Interface for exporting.
-        You should create at least a `config.json` containing the fields:
-        * "version" (str)
-        * "architecture" (str)
-        * "config": (dict w/ other necessary data like tensor shapes etc)
-
-        :param outdir: Assumed to exist. Can be edited inside at will.
-        """
-        with self._use_parametric_config(parametric_config):
-            return super().export(outdir, **kwargs)
-
-    def export_cpp_header(self, filename: Path, parametric_config: Dict[str, Param]):
-        with self._use_parametric_config(parametric_config):
-            return super().export_cpp_header(filename)
-
-    def _export_config(self):
-        """
-        Adds in the sidedoored parametric pieces
-
-        :paramtric_config: the dict of parameter info (name, type, etc)
-        """
-        config = super()._export_config()
-        if not isinstance(config, dict):
-            raise TypeError(
-                f"Parameteric models' base configs must be a dict; got {type(config)}"
-            )
-        parametric_key = "parametric"
-        if parametric_key in config:
-            raise ValueError(
-                f'Already found parametric key "{parametric_key}" in base config dict.'
-            )
-        # Yucky sidedoor
-        config[parametric_key] = {
-            k: v.to_json() for k, v in self._sidedoor_parametric_config.items()
-        }
-        return config
-
-    def _export_cpp_header_parametric(self, config):
-        if config is None:
-            return self._single_class._export_cpp_head_parametric(self, config)
-        s_parametric = [
-            'nlohmann::json PARAMETRIC = nlohmann::json::parse(R"(\n',
-            "  {\n",
-        ]
-        for i, (key, val) in enumerate(config.items(), 1):
-            s_parametric.append(f'    "{key}": ' "{\n")
-            for j, (k2, v2) in enumerate(val.items(), 1):
-                v_str = f'"{v2}"' if isinstance(v2, str) else str(v2)
-                s_parametric.append(
-                    f'      "{k2}": {v_str}' + (",\n" if j < len(val) else "\n")
-                )
-            s_parametric.append("    }" f"{',' if i < len(config) else ''}\n")
-        s_parametric.append("  }\n")
-        s_parametric.append(')");\n')
-        return tuple(s_parametric)
-
-    def _export_input_output_args(self) -> Tuple[torch.Tensor]:
-        return (self._sidedoor_params_to_tensor(),)
-
-    def _forward(self, params, x):
-        """
-        :param params: (N,D)
-        :param x: (N,L1)
-
-        :return: (N,L2)
-        """
-        sequence_length = x.shape[1]
-        x_augmented = (
-            torch.cat(
-                [
-                    x[..., None],
-                    torch.tile(params[:, None, :], (1, sequence_length, 1)),
-                ],
-                dim=2,
-            )
-            if self._shape_type == _ShapeType.RNN
-            else torch.cat(
-                [x[:, None, :], torch.tile(params[..., None], (1, 1, sequence_length))],
-                dim=1,
-            )
-        )
-        return self._single_class._forward(self, x_augmented)
-
-    def _sidedoor_params_to_tensor(self) -> torch.Tensor:
-        param_names = sorted([k for k in self._sidedoor_parametric_config.keys()])
-        params = torch.Tensor(
-            [self._sidedoor_parametric_config[k].default_value for k in param_names]
-        )
-        return params
-
-    @contextmanager
-    def _use_parametric_config(self, c):
-        """
-        Sneaks in the parametric config while exporting
-        """
-        try:
-            self._sidedoor_parametric_config = c
-            yield None
-        finally:
-            self._sidedoor_parametric_config = None
-
-
-class CatLSTM(_CatMixin, LSTM):
-    @property
-    def _shape_type(self) -> _ShapeType:
-        return _ShapeType.RNN
-
-    @property
-    def _single_class(self):
-        return LSTM
-
-    def _append_default_params(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        Requires sidedoor'd params
-
-        :param x: (B,L)
-        :return: (B,L,1+D)
-        """
-        assert x.ndim == 2
-        params = self._sidedoor_params_to_tensor()
-        sequence_length = x.shape[1]
-        return torch.cat(
-            [
-                x[:, :, None],
-                torch.tile(params[None, None, :], (1, sequence_length, 1)),
-            ],
-            dim=2,
-        )
-
-    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
-        if self._input_size != 1:
-            logger.warning(
-                "Nominal settings aren't defined for parametric models; outputting unity"
-            )
-            return x
-        params = torch.zeros(()).to(x.device)
-        return self(params, x)
-
-    def _get_initial_state(self) -> Tuple[torch.Tensor, torch.Tensor]:
-        inputs = self._append_default_params(torch.zeros((1, 48_000)))
-        return super()._get_initial_state(inputs=inputs)
-
-
-class CatWaveNet(_CatMixin, WaveNet):
-    @property
-    def _shape_type(self) -> _ShapeType:
-        return _ShapeType.CONV
-
-    @property
-    def _single_class(self):
-        return WaveNet
+# File: catnets.py
+# Created Date: Wednesday June 22nd 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+"Cat nets" -- parametric models where the parametric input is concatenated to the
+input samples
+"""
+
+import abc
+import logging
+from enum import Enum
+from contextlib import contextmanager
+from pathlib import Path
+from typing import Any, Dict, Tuple
+
+import numpy as np
+import torch
+
+from .._base import ParametricBaseNet
+from ..recurrent import LSTM
+from ..wavenet import WaveNet
+from .params import Param
+
+logger = logging.getLogger(__name__)
+
+
+class _ShapeType(Enum):
+    CONV = "conv"  # (B,C,L)
+    RNN = "rnn"  # (B,L,D)
+
+
+class _CatMixin(ParametricBaseNet):
+    """
+    Parameteric nets that concatenate the params with the input at each time point
+    Mix in with a non-parametric class like
+
+    ```
+    class CatLSTM(LSTM, _CatMixin):
+        pass
+    ```
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # Hacky, see .export()
+        self._sidedoor_parametric_config = None
+
+    @abc.abstractproperty
+    def _shape_type(self) -> _ShapeType:
+        pass
+
+    @abc.abstractproperty
+    def _single_class(self):
+        """ "
+        The class for the non-parametric model that this is extending
+        """
+        # TODO verify that single class satisfies requirements
+        # ._export_weights()
+        # ._export_input_output()
+        pass  # HACK
+
+    def export(self, outdir: Path, parametric_config: Dict[str, Param], **kwargs):
+        """
+        Interface for exporting.
+        You should create at least a `config.json` containing the fields:
+        * "version" (str)
+        * "architecture" (str)
+        * "config": (dict w/ other necessary data like tensor shapes etc)
+
+        :param outdir: Assumed to exist. Can be edited inside at will.
+        """
+        with self._use_parametric_config(parametric_config):
+            return super().export(outdir, **kwargs)
+
+    def export_cpp_header(self, filename: Path, parametric_config: Dict[str, Param]):
+        with self._use_parametric_config(parametric_config):
+            return super().export_cpp_header(filename)
+
+    def _export_config(self):
+        """
+        Adds in the sidedoored parametric pieces
+
+        :paramtric_config: the dict of parameter info (name, type, etc)
+        """
+        config = super()._export_config()
+        if not isinstance(config, dict):
+            raise TypeError(
+                f"Parameteric models' base configs must be a dict; got {type(config)}"
+            )
+        parametric_key = "parametric"
+        if parametric_key in config:
+            raise ValueError(
+                f'Already found parametric key "{parametric_key}" in base config dict.'
+            )
+        # Yucky sidedoor
+        config[parametric_key] = {
+            k: v.to_json() for k, v in self._sidedoor_parametric_config.items()
+        }
+        return config
+
+    def _export_cpp_header_parametric(self, config):
+        if config is None:
+            return self._single_class._export_cpp_head_parametric(self, config)
+        s_parametric = [
+            'nlohmann::json PARAMETRIC = nlohmann::json::parse(R"(\n',
+            "  {\n",
+        ]
+        for i, (key, val) in enumerate(config.items(), 1):
+            s_parametric.append(f'    "{key}": ' "{\n")
+            for j, (k2, v2) in enumerate(val.items(), 1):
+                v_str = f'"{v2}"' if isinstance(v2, str) else str(v2)
+                s_parametric.append(
+                    f'      "{k2}": {v_str}' + (",\n" if j < len(val) else "\n")
+                )
+            s_parametric.append("    }" f"{',' if i < len(config) else ''}\n")
+        s_parametric.append("  }\n")
+        s_parametric.append(')");\n')
+        return tuple(s_parametric)
+
+    def _export_input_output_args(self) -> Tuple[torch.Tensor]:
+        return (self._sidedoor_params_to_tensor(),)
+
+    def _forward(self, params, x):
+        """
+        :param params: (N,D)
+        :param x: (N,L1)
+
+        :return: (N,L2)
+        """
+        sequence_length = x.shape[1]
+        x_augmented = (
+            torch.cat(
+                [
+                    x[..., None],
+                    torch.tile(params[:, None, :], (1, sequence_length, 1)),
+                ],
+                dim=2,
+            )
+            if self._shape_type == _ShapeType.RNN
+            else torch.cat(
+                [x[:, None, :], torch.tile(params[..., None], (1, 1, sequence_length))],
+                dim=1,
+            )
+        )
+        return self._single_class._forward(self, x_augmented)
+
+    def _sidedoor_params_to_tensor(self) -> torch.Tensor:
+        param_names = sorted([k for k in self._sidedoor_parametric_config.keys()])
+        params = torch.Tensor(
+            [self._sidedoor_parametric_config[k].default_value for k in param_names]
+        )
+        return params
+
+    @contextmanager
+    def _use_parametric_config(self, c):
+        """
+        Sneaks in the parametric config while exporting
+        """
+        try:
+            self._sidedoor_parametric_config = c
+            yield None
+        finally:
+            self._sidedoor_parametric_config = None
+
+
+class CatLSTM(_CatMixin, LSTM):
+    @property
+    def _shape_type(self) -> _ShapeType:
+        return _ShapeType.RNN
+
+    @property
+    def _single_class(self):
+        return LSTM
+
+    def _append_default_params(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        Requires sidedoor'd params
+
+        :param x: (B,L)
+        :return: (B,L,1+D)
+        """
+        assert x.ndim == 2
+        params = self._sidedoor_params_to_tensor()
+        sequence_length = x.shape[1]
+        return torch.cat(
+            [
+                x[:, :, None],
+                torch.tile(params[None, None, :], (1, sequence_length, 1)),
+            ],
+            dim=2,
+        )
+
+    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
+        if self._input_size != 1:
+            logger.warning(
+                "Nominal settings aren't defined for parametric models; outputting unity"
+            )
+            return x
+        params = torch.zeros(()).to(x.device)
+        return self(params, x)
+
+    def _get_initial_state(self) -> Tuple[torch.Tensor, torch.Tensor]:
+        inputs = self._append_default_params(torch.zeros((1, 48_000)))
+        return super()._get_initial_state(inputs=inputs)
+
+
+class CatWaveNet(_CatMixin, WaveNet):
+    @property
+    def _shape_type(self) -> _ShapeType:
+        return _ShapeType.CONV
+
+    @property
+    def _single_class(self):
+        return WaveNet
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/parametric/hyper_net.py` & `neural-amp-modeler-0.5.2/nam/models/parametric/hyper_net.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,559 +1,559 @@
-# File: hyper_net.py
-# Created Date: Sunday May 29th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-import abc
-import json
-import math
-from dataclasses import dataclass
-from enum import Enum
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Any, Callable, List, Optional, Tuple
-
-import numpy as np
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from torch.nn.init import (
-    calculate_gain,
-    _calculate_correct_fan,
-    _calculate_fan_in_and_fan_out,
-)
-
-from ..._version import __version__
-from .._base import ParametricBaseNet
-
-
-class SpecialLayers(Enum):
-    CONV = "conv"
-    BATCHNORM = "batchnorm"
-
-
-@dataclass
-class LayerSpec:
-    """
-    Helps the hypernet
-    """
-
-    special_type: Optional[str]
-    shapes: Tuple[Tuple[int]]
-    norms: Tuple[float]
-    biases: Tuple[float]
-
-
-class _NetLayer(nn.Module, abc.ABC):
-    @abc.abstractproperty
-    def num_tensors(self) -> int:
-        pass
-
-    @abc.abstractmethod
-    def get_spec(self) -> LayerSpec:
-        pass
-
-
-class _Conv(nn.Conv1d, _NetLayer):
-    @property
-    def num_tensors(self):
-        return 2 if self.bias is not None else 1
-
-    def forward(self, params, inputs):
-        # Use depthwise convolution trick to process the convolutions together
-        cout, cin, kernel_size = self.weight.shape
-        n = len(params[0])
-        weight = params[0].reshape((n * cout, cin, kernel_size))  # (N, CinCout)
-        bias = params[1].flatten() if self.bias is not None else None
-        groups = n
-        return F.conv1d(
-            inputs.reshape((1, n * cin, -1)),
-            weight,
-            bias=bias,
-            stride=self.stride,
-            padding=self.padding,
-            dilation=self.dilation,
-            groups=groups,
-        ).reshape((n, cout, -1))
-
-    def get_spec(self):
-        shapes = (
-            (self.weight.shape,)
-            if self.bias is None
-            else (self.weight.shape, self.bias.shape)
-        )
-        norms = (
-            (self._weight_norm(),)
-            if self.bias is None
-            else (self._weight_norm(), self._bias_norm())
-        )
-        biases = (0,) if self.bias is None else (0, 0)
-        return LayerSpec(SpecialLayers("conv"), shapes, norms, biases)
-
-    def _bias_norm(self):
-        # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv1d
-        fan = _calculate_fan_in_and_fan_out(self.weight.data)[0]
-        bound = 1.0 / math.sqrt(fan)
-        std = math.sqrt(1.0 / 12.0) * (2 * bound)
-        # LayerNorm handles division by number of dimensions...
-        return std
-
-    def _weight_norm(self):
-        """
-        Std of the unfiorm distribution used in initialization
-        """
-        # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv1d
-        fan = _calculate_correct_fan(self.weight.data, "fan_in")
-        # Kaiming uniform w/ a=sqrt(5)
-        gain = calculate_gain("leaky_relu", 5.0)
-        std = gain / math.sqrt(fan)
-        # LayerNorm handles division by number of dimensions...
-        return std
-
-
-class _BatchNorm(nn.BatchNorm1d, _NetLayer):
-    def __init__(self, num_features, *args, affine=True, **kwargs):
-        # Handle affine params outside of parent class
-        super().__init__(num_features, *args, affine=False, **kwargs)
-        self._num_features = num_features
-        assert affine
-        self._affine = affine
-
-    @property
-    def num_tensors(self) -> int:
-        return 2
-
-    def get_spec(self) -> LayerSpec:
-        return LayerSpec(
-            SpecialLayers.BATCHNORM,
-            ((self._num_features,), (self._num_features,)),
-            (1.0e-5, 1.0e-5),
-            (1.0, 0.0),
-        )
-
-    def forward(self, params, inputs):
-        """
-        Only change is we need to provide *params into F.batch_norm instead of 
-        self.weight, self.bias
-        """
-        # Also use "inputs" instead of "input" to not collide w/ builtin (ew)
-        weight, bias = [z[:, :, None] for z in params]
-        pre_affine = super().forward(inputs)
-        return weight * pre_affine + bias
-
-
-class _Affine(nn.Module):
-    def __init__(self, scale: torch.Tensor, bias: torch.Tensor):
-        super().__init__()
-        self._weight = nn.Parameter(scale)
-        self._bias = nn.Parameter(bias)
-
-    @property
-    def bias(self) -> nn.Parameter:
-        return self._bias
-
-    @property
-    def weight(self) -> nn.Parameter:
-        return self._weight
-
-    def forward(self, inputs):
-        return self._weight * inputs + self._bias
-
-
-class HyperNet(nn.Module):
-    """
-    MLP followed by layer norms on split-up dims
-    """
-
-    def __init__(self, d_in, net, numels, norms, biases):
-        super().__init__()
-        self._net = net
-        # Figure out the scale factor empirically
-        norm0 = net(torch.randn((10_000, d_in))).std(dim=0).mean().item()
-        self._cum_numel = torch.cat(
-            [torch.LongTensor([0]), torch.cumsum(torch.LongTensor(numels), dim=0)]
-        )
-        affine_scale = torch.cat(
-            [torch.full((numel,), norm / norm0) for numel, norm in zip(numels, norms)]
-        )
-        affine_bias = torch.cat(
-            [
-                torch.full((numel,), bias, dtype=torch.float)
-                for numel, bias in zip(numels, biases)
-            ]
-        )
-        self._affine = _Affine(affine_scale, affine_bias)
-
-    @property
-    def batchnorm(self) -> bool:
-        """
-        Does the hypernet use batchnorm layers
-        """
-        return any(isinstance(m, nn.BatchNorm1d) for m in self.modules())
-
-    @property
-    def input_dim(self) -> int:
-        return self._net[0][0].weight.shape[1]
-
-    @property
-    def num_layers(self) -> int:
-        return len([layer for layer in self._net if isinstance(layer, _HyperNetBlock)])
-
-    @property
-    def num_units(self) -> int:
-        return self._net[0][0].weight.shape[0]
-
-    def forward(self, x) -> Tuple[torch.Tensor]:
-        """
-        Just return a flat array of param tensors for now
-        """
-        y = self._affine(self._net(x))
-        return tuple(
-            y[:, i:j] for i, j in zip(self._cum_numel[:-1], self._cum_numel[1:])
-        )
-
-    def get_export_params(self) -> np.ndarray:
-        params = []
-        for block in self._net[:-1]:
-            linear = block[0]
-            params.append(linear.weight.flatten())
-            params.append(linear.bias.flatten())
-            if self.batchnorm:
-                bn = block[1]
-                params.append(bn.running_mean.flatten())
-                params.append(bn.running_var.flatten())
-                params.append(bn.weight.flatten())
-                params.append(bn.bias.flatten())
-                params.append(torch.Tensor([bn.eps]).to(bn.weight.device))
-            assert len(block) <= 3, "Linear-(BN)-activation"
-            assert (
-                len([p for p in block[-1].parameters()]) == 0
-            ), "No params in activation"
-        head = self._net[-1]
-        params.append(head.weight.flatten())
-        params.append(head.bias.flatten())
-        affine = self._affine
-        params.append(affine.weight.flatten())
-        params.append(affine.bias.flatten())
-        return torch.cat(params).detach().cpu().numpy()
-
-
-class _Activation(abc.ABC):
-    """
-    Indicate that a module is an activation within the main net
-    """
-
-    @abc.abstractproperty
-    def name(self) -> str:
-        """
-        What to call the layer by when making a config w/ it
-        """
-        pass
-
-
-def _extend_activation(C, name: str) -> _Activation:
-    class Activation(C, _NetLayer, _Activation):
-        @property
-        def name(self):
-            return name
-
-        @property
-        def num_tensors(self) -> int:
-            return 0
-
-        def get_spec(self) -> LayerSpec:
-            return LayerSpec(None, (), (), ())
-
-        def forward(self, params, inputs):
-            return super().forward(inputs)
-
-    return Activation
-
-
-_Tanh = _extend_activation(nn.Tanh, "Tanh")
-_ReLU = _extend_activation(nn.ReLU, "ReLU")
-_Flatten = _extend_activation(nn.Flatten, "Flatten")  # Hah, works
-
-
-def _get_activation(name):
-    return {"Tanh": _Tanh, "ReLU": _ReLU}[name]()
-
-
-class _HyperNetBlock(nn.Sequential):
-    """
-    For IDing blocks of the hypernet
-    """
-
-    pass
-
-
-class HyperConvNet(ParametricBaseNet):
-    """
-    For parameteric data
-
-    Conditioning is input to a hypernetwork that outputs the parameters of the conv net.
-    """
-
-    def __init__(
-        self, hyper_net: HyperNet, net: Callable[[Any, torch.Tensor], torch.Tensor]
-    ):
-        super().__init__()
-        self._hyper_net = hyper_net
-        self._net = net
-
-    @classmethod
-    def parse_config(cls, config):
-        config = super().parse_config(config)
-        net, specs = cls._get_net(config["net"])
-        hyper_net = cls._get_hyper_net(config["hyper_net"], specs)
-        return {"hyper_net": hyper_net, "net": net}
-
-    @property
-    def pad_start_default(self) -> bool:
-        return True
-
-    @property
-    def receptive_field(self) -> int:
-        # Last conv is the collapser--compensate w/ a minus 1
-        return sum([m.dilation[0] for m in self._net if isinstance(m, _Conv)]) + 1 - 1
-
-    def export(self, outdir: Path, include_snapshot: bool=False):
-        """
-        Files created:
-        * config.json
-        * weights.npy
-        * test_signal_params.npy
-        * test_signal_input.npy
-        * test_signal_output.npy
-
-        weights are serialized to weights.npy in the following order:
-        * Hypernet
-            * Loop layers:
-                * Linear
-                    * weights (din*dout)
-                    * biases (dout)
-                * BN
-                    * running_mean (d)
-                    * running_var (d)
-                    * weight (d)
-                    * bias (d)
-                    * eps ()
-                * activation
-                    * (Assume no params bc Tanh)
-            * Linear out
-                * weights (units*dy)
-                * bias (dy)
-            * affine
-                * weights (dy)
-                * bias (dy)
-        * Main net
-            (Layers are conv-BN-act)
-            (All params are outputted by the hypernet except the BatchNorm buffers!)
-            * Loop layers
-                * BN
-                    * running_mean
-                    * running_var
-                    * eps ()
-        * (flatten: no params)
-
-        A test input & output are also provided, input.npy and output.npy
-        """
-        training = self.training
-        self.eval()
-        with open(Path(outdir, "config.json"), "w") as fp:
-            json.dump(self._export_config(), fp, indent=4)
-
-        # Hope I don't regret using np.save...
-        np.save(Path(outdir, "weights.npy"), self._export_weights())
-
-        # And an input/output to verify correct computation:
-        if include_snapshot:
-            params, x, y = self._export_input_output()
-            np.save(Path(outdir, "test_signal_params.npy"), params.detach().cpu().numpy())
-            np.save(Path(outdir, "test_signal_input.npy"), x.detach().cpu().numpy())
-            np.save(Path(outdir, "test_signal_output.npy"), y.detach().cpu().numpy())
-
-        # And resume training state
-        self.train(training)
-
-    def export_cpp_header(self, filename: Path):
-        with TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir)
-            self.export(Path(tmpdir))
-            with open(Path(tmpdir, "config.json"), "r") as fp:
-                _c = json.load(fp)
-            version = _c["version"]
-            config = _c["config"]
-            params = np.load(Path(tmpdir, "weights.npy"))
-        with open(filename, "w") as f:
-            f.writelines(
-                (
-                    "#pragma once\n",
-                    "// Automatically-generated model file\n",
-                    "// HyperConvNet model\n" "#include <vector>\n",
-                    f'#define PYTHON_MODEL_VERSION "{version}"\n',
-                    f'const int HYPER_NET_INPUT_DIM = {config["hyper_net"]["input_dim"]};\n',
-                    f'const int HYPER_NET_NUM_LAYERS = {config["hyper_net"]["num_layers"]};\n',
-                    f'const int HYPER_NET_NUM_UNITS = {config["hyper_net"]["num_units"]};\n',
-                    f'const int HYPER_NET_BATCHNORM = {"true" if config["hyper_net"]["batchnorm"] else "false"};\n',
-                    f"const int CHANNELS = {config['net']['channels']};\n",
-                    f"const bool BATCHNORM = {'true' if config['net']['batchnorm'] else 'false'};\n",
-                    "std::vector<int> DILATIONS{"
-                    + ",".join([str(d) for d in config["net"]["dilations"]])
-                    + "};\n",
-                    f"const std::string ACTIVATION = \"{config['net']['activation']}\";\n",
-                    "std::vector<float> PARAMS{"
-                    + ",".join([f"{w:.16f}" for w in params])
-                    + "};\n",
-                )
-            )
-
-    @classmethod
-    def _get_net(cls, config):
-        channels = config["channels"]
-        dilations = config["dilations"]
-        batchnorm = config["batchnorm"]
-        activation = config["activation"]
-
-        layers = []
-        layer_specs = []
-        cin = 1
-        for dilation in dilations:
-            layer = _Conv(cin, channels, 2, dilation=dilation, bias=not batchnorm)
-            layers.append(layer)
-            layer_specs.append(layer.get_spec())
-            if batchnorm:
-                # Slow momentum on main net bc it's wild
-                layer = _BatchNorm(channels, momentum=0.01)
-                layers.append(layer)
-                layer_specs.append(layer.get_spec())
-            layer = _get_activation(activation)
-            layers.append(layer)
-            layer_specs.append(layer.get_spec())
-            cin = channels
-        layer = _Conv(cin, 1, 1)
-        layers.append(layer)
-        layer_specs.append(layer.get_spec())
-        layer = _Flatten()
-        layers.append(layer)
-        layer_specs.append(layer.get_spec())
-
-        return nn.ModuleList(layers), layer_specs
-
-    @classmethod
-    def _get_hyper_net(cls, config, specs) -> HyperNet:
-        def block(dx, dy, batchnorm) -> _HyperNetBlock:
-            layer_list = [nn.Linear(dx, dy)]
-            if batchnorm:
-                layer_list.append(nn.BatchNorm1d(dy))
-            layer_list.append(nn.ReLU())
-            return _HyperNetBlock(*layer_list)
-
-        num_inputs = config["num_inputs"]
-        num_layers = config["num_layers"]
-        num_units = config["num_units"]
-        batchnorm = config["batchnorm"]
-        # Flatten specs
-        numels = [np.prod(np.array(shape)) for spec in specs for shape in spec.shapes]
-        norms = [norm for spec in specs for norm in spec.norms]
-        biases = [bias for spec in specs for bias in spec.biases]
-        num_outputs = sum(numels)
-
-        din, layer_list = num_inputs, []
-        for _ in range(num_layers):
-            layer_list.append(block(din, num_units, batchnorm))
-            din = num_units
-        layer_list.append(nn.Linear(din, num_outputs))
-        net = nn.Sequential(*layer_list)
-
-        return HyperNet(num_inputs, net, numels, norms, biases)
-
-    @property
-    def _activation(self) -> str:
-        """
-        What activation does the main net use
-        """
-        for m in self._net.modules():
-            if isinstance(m, _Activation):
-                return m.name
-
-    @property
-    def _batchnorm(self) -> bool:
-        return any(isinstance(x, _BatchNorm) for x in self._net)
-
-    @property
-    def _channels(self) -> int:
-        return self._net[0].weight.shape[0]
-
-    @property
-    def _net_no_head(self):
-        return self._net[:-2]
-
-    def _forward(self, params: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
-        net_params = self._hyper_net(params)
-        i = 0
-        for m in self._net:
-            j = i + m.num_tensors
-            x = m(net_params[i:j], x)
-            i = j
-        assert j == len(net_params)
-        return x
-
-    def _get_dilations(self) -> List[int]:
-        dilations = []
-        for (
-            layer
-        ) in self._net_no_head:  # Last two layers are a 1D conv head and flatten
-            if isinstance(layer, _Conv):
-                dilations.append(layer.dilation[0])
-        return dilations
-
-    def _export_config(self):
-        return {
-            "version": __version__,
-            "architecture": "HyperConvNet",
-            "config": {
-                "hyper_net": {
-                    "input_dim": self._hyper_net.input_dim,
-                    "num_layers": self._hyper_net.num_layers,
-                    "num_units": self._hyper_net.num_units,
-                    "batchnorm": self._hyper_net.batchnorm,
-                },
-                "net": {
-                    "channels": self._channels,
-                    "dilations": self._get_dilations(),
-                    "batchnorm": self._batchnorm,
-                    "activation": self._activation,
-                },
-            },
-        }
-
-    def _export_weights(self) -> np.ndarray:
-        """
-        Flatten the parameters of the network to be exported.
-        See doctsring for .export() for ensured layout.
-        """
-        return np.concatenate(
-            [self._hyper_net.get_export_params(), self._export_net_weights()]
-        )
-
-    def _export_net_weights(self) -> np.ndarray:
-        """
-        Only the buffers--parameters are outputted by the hypernet!
-        """
-        params = []
-        for bn in self._net_no_head:
-            if isinstance(bn, _BatchNorm):
-                params.append(bn.running_mean.flatten())
-                params.append(bn.running_var.flatten())
-                params.append(torch.Tensor([bn.eps]).to(bn.running_mean.device))
-        return (
-            np.array([])
-            if len(params) == 0
-            else torch.cat(params).detach().cpu().numpy()
-        )
-
-    def _export_input_output(self) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        params = torch.randn((self._hyper_net.input_dim,))
-        x = torch.randn((2 * self.receptive_field,))
-        x = 0.5 * x / x.abs().max()
-        y = self(params, x)
-        return params, x, y
+# File: hyper_net.py
+# Created Date: Sunday May 29th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+import abc
+import json
+import math
+from dataclasses import dataclass
+from enum import Enum
+from pathlib import Path
+from tempfile import TemporaryDirectory
+from typing import Any, Callable, List, Optional, Tuple
+
+import numpy as np
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from torch.nn.init import (
+    calculate_gain,
+    _calculate_correct_fan,
+    _calculate_fan_in_and_fan_out,
+)
+
+from ..._version import __version__
+from .._base import ParametricBaseNet
+
+
+class SpecialLayers(Enum):
+    CONV = "conv"
+    BATCHNORM = "batchnorm"
+
+
+@dataclass
+class LayerSpec:
+    """
+    Helps the hypernet
+    """
+
+    special_type: Optional[str]
+    shapes: Tuple[Tuple[int]]
+    norms: Tuple[float]
+    biases: Tuple[float]
+
+
+class _NetLayer(nn.Module, abc.ABC):
+    @abc.abstractproperty
+    def num_tensors(self) -> int:
+        pass
+
+    @abc.abstractmethod
+    def get_spec(self) -> LayerSpec:
+        pass
+
+
+class _Conv(nn.Conv1d, _NetLayer):
+    @property
+    def num_tensors(self):
+        return 2 if self.bias is not None else 1
+
+    def forward(self, params, inputs):
+        # Use depthwise convolution trick to process the convolutions together
+        cout, cin, kernel_size = self.weight.shape
+        n = len(params[0])
+        weight = params[0].reshape((n * cout, cin, kernel_size))  # (N, CinCout)
+        bias = params[1].flatten() if self.bias is not None else None
+        groups = n
+        return F.conv1d(
+            inputs.reshape((1, n * cin, -1)),
+            weight,
+            bias=bias,
+            stride=self.stride,
+            padding=self.padding,
+            dilation=self.dilation,
+            groups=groups,
+        ).reshape((n, cout, -1))
+
+    def get_spec(self):
+        shapes = (
+            (self.weight.shape,)
+            if self.bias is None
+            else (self.weight.shape, self.bias.shape)
+        )
+        norms = (
+            (self._weight_norm(),)
+            if self.bias is None
+            else (self._weight_norm(), self._bias_norm())
+        )
+        biases = (0,) if self.bias is None else (0, 0)
+        return LayerSpec(SpecialLayers("conv"), shapes, norms, biases)
+
+    def _bias_norm(self):
+        # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv1d
+        fan = _calculate_fan_in_and_fan_out(self.weight.data)[0]
+        bound = 1.0 / math.sqrt(fan)
+        std = math.sqrt(1.0 / 12.0) * (2 * bound)
+        # LayerNorm handles division by number of dimensions...
+        return std
+
+    def _weight_norm(self):
+        """
+        Std of the unfiorm distribution used in initialization
+        """
+        # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv1d
+        fan = _calculate_correct_fan(self.weight.data, "fan_in")
+        # Kaiming uniform w/ a=sqrt(5)
+        gain = calculate_gain("leaky_relu", 5.0)
+        std = gain / math.sqrt(fan)
+        # LayerNorm handles division by number of dimensions...
+        return std
+
+
+class _BatchNorm(nn.BatchNorm1d, _NetLayer):
+    def __init__(self, num_features, *args, affine=True, **kwargs):
+        # Handle affine params outside of parent class
+        super().__init__(num_features, *args, affine=False, **kwargs)
+        self._num_features = num_features
+        assert affine
+        self._affine = affine
+
+    @property
+    def num_tensors(self) -> int:
+        return 2
+
+    def get_spec(self) -> LayerSpec:
+        return LayerSpec(
+            SpecialLayers.BATCHNORM,
+            ((self._num_features,), (self._num_features,)),
+            (1.0e-5, 1.0e-5),
+            (1.0, 0.0),
+        )
+
+    def forward(self, params, inputs):
+        """
+        Only change is we need to provide *params into F.batch_norm instead of 
+        self.weight, self.bias
+        """
+        # Also use "inputs" instead of "input" to not collide w/ builtin (ew)
+        weight, bias = [z[:, :, None] for z in params]
+        pre_affine = super().forward(inputs)
+        return weight * pre_affine + bias
+
+
+class _Affine(nn.Module):
+    def __init__(self, scale: torch.Tensor, bias: torch.Tensor):
+        super().__init__()
+        self._weight = nn.Parameter(scale)
+        self._bias = nn.Parameter(bias)
+
+    @property
+    def bias(self) -> nn.Parameter:
+        return self._bias
+
+    @property
+    def weight(self) -> nn.Parameter:
+        return self._weight
+
+    def forward(self, inputs):
+        return self._weight * inputs + self._bias
+
+
+class HyperNet(nn.Module):
+    """
+    MLP followed by layer norms on split-up dims
+    """
+
+    def __init__(self, d_in, net, numels, norms, biases):
+        super().__init__()
+        self._net = net
+        # Figure out the scale factor empirically
+        norm0 = net(torch.randn((10_000, d_in))).std(dim=0).mean().item()
+        self._cum_numel = torch.cat(
+            [torch.LongTensor([0]), torch.cumsum(torch.LongTensor(numels), dim=0)]
+        )
+        affine_scale = torch.cat(
+            [torch.full((numel,), norm / norm0) for numel, norm in zip(numels, norms)]
+        )
+        affine_bias = torch.cat(
+            [
+                torch.full((numel,), bias, dtype=torch.float)
+                for numel, bias in zip(numels, biases)
+            ]
+        )
+        self._affine = _Affine(affine_scale, affine_bias)
+
+    @property
+    def batchnorm(self) -> bool:
+        """
+        Does the hypernet use batchnorm layers
+        """
+        return any(isinstance(m, nn.BatchNorm1d) for m in self.modules())
+
+    @property
+    def input_dim(self) -> int:
+        return self._net[0][0].weight.shape[1]
+
+    @property
+    def num_layers(self) -> int:
+        return len([layer for layer in self._net if isinstance(layer, _HyperNetBlock)])
+
+    @property
+    def num_units(self) -> int:
+        return self._net[0][0].weight.shape[0]
+
+    def forward(self, x) -> Tuple[torch.Tensor]:
+        """
+        Just return a flat array of param tensors for now
+        """
+        y = self._affine(self._net(x))
+        return tuple(
+            y[:, i:j] for i, j in zip(self._cum_numel[:-1], self._cum_numel[1:])
+        )
+
+    def get_export_params(self) -> np.ndarray:
+        params = []
+        for block in self._net[:-1]:
+            linear = block[0]
+            params.append(linear.weight.flatten())
+            params.append(linear.bias.flatten())
+            if self.batchnorm:
+                bn = block[1]
+                params.append(bn.running_mean.flatten())
+                params.append(bn.running_var.flatten())
+                params.append(bn.weight.flatten())
+                params.append(bn.bias.flatten())
+                params.append(torch.Tensor([bn.eps]).to(bn.weight.device))
+            assert len(block) <= 3, "Linear-(BN)-activation"
+            assert (
+                len([p for p in block[-1].parameters()]) == 0
+            ), "No params in activation"
+        head = self._net[-1]
+        params.append(head.weight.flatten())
+        params.append(head.bias.flatten())
+        affine = self._affine
+        params.append(affine.weight.flatten())
+        params.append(affine.bias.flatten())
+        return torch.cat(params).detach().cpu().numpy()
+
+
+class _Activation(abc.ABC):
+    """
+    Indicate that a module is an activation within the main net
+    """
+
+    @abc.abstractproperty
+    def name(self) -> str:
+        """
+        What to call the layer by when making a config w/ it
+        """
+        pass
+
+
+def _extend_activation(C, name: str) -> _Activation:
+    class Activation(C, _NetLayer, _Activation):
+        @property
+        def name(self):
+            return name
+
+        @property
+        def num_tensors(self) -> int:
+            return 0
+
+        def get_spec(self) -> LayerSpec:
+            return LayerSpec(None, (), (), ())
+
+        def forward(self, params, inputs):
+            return super().forward(inputs)
+
+    return Activation
+
+
+_Tanh = _extend_activation(nn.Tanh, "Tanh")
+_ReLU = _extend_activation(nn.ReLU, "ReLU")
+_Flatten = _extend_activation(nn.Flatten, "Flatten")  # Hah, works
+
+
+def _get_activation(name):
+    return {"Tanh": _Tanh, "ReLU": _ReLU}[name]()
+
+
+class _HyperNetBlock(nn.Sequential):
+    """
+    For IDing blocks of the hypernet
+    """
+
+    pass
+
+
+class HyperConvNet(ParametricBaseNet):
+    """
+    For parameteric data
+
+    Conditioning is input to a hypernetwork that outputs the parameters of the conv net.
+    """
+
+    def __init__(
+        self, hyper_net: HyperNet, net: Callable[[Any, torch.Tensor], torch.Tensor]
+    ):
+        super().__init__()
+        self._hyper_net = hyper_net
+        self._net = net
+
+    @classmethod
+    def parse_config(cls, config):
+        config = super().parse_config(config)
+        net, specs = cls._get_net(config["net"])
+        hyper_net = cls._get_hyper_net(config["hyper_net"], specs)
+        return {"hyper_net": hyper_net, "net": net}
+
+    @property
+    def pad_start_default(self) -> bool:
+        return True
+
+    @property
+    def receptive_field(self) -> int:
+        # Last conv is the collapser--compensate w/ a minus 1
+        return sum([m.dilation[0] for m in self._net if isinstance(m, _Conv)]) + 1 - 1
+
+    def export(self, outdir: Path, include_snapshot: bool=False):
+        """
+        Files created:
+        * config.json
+        * weights.npy
+        * test_signal_params.npy
+        * test_signal_input.npy
+        * test_signal_output.npy
+
+        weights are serialized to weights.npy in the following order:
+        * Hypernet
+            * Loop layers:
+                * Linear
+                    * weights (din*dout)
+                    * biases (dout)
+                * BN
+                    * running_mean (d)
+                    * running_var (d)
+                    * weight (d)
+                    * bias (d)
+                    * eps ()
+                * activation
+                    * (Assume no params bc Tanh)
+            * Linear out
+                * weights (units*dy)
+                * bias (dy)
+            * affine
+                * weights (dy)
+                * bias (dy)
+        * Main net
+            (Layers are conv-BN-act)
+            (All params are outputted by the hypernet except the BatchNorm buffers!)
+            * Loop layers
+                * BN
+                    * running_mean
+                    * running_var
+                    * eps ()
+        * (flatten: no params)
+
+        A test input & output are also provided, input.npy and output.npy
+        """
+        training = self.training
+        self.eval()
+        with open(Path(outdir, "config.json"), "w") as fp:
+            json.dump(self._export_config(), fp, indent=4)
+
+        # Hope I don't regret using np.save...
+        np.save(Path(outdir, "weights.npy"), self._export_weights())
+
+        # And an input/output to verify correct computation:
+        if include_snapshot:
+            params, x, y = self._export_input_output()
+            np.save(Path(outdir, "test_signal_params.npy"), params.detach().cpu().numpy())
+            np.save(Path(outdir, "test_signal_input.npy"), x.detach().cpu().numpy())
+            np.save(Path(outdir, "test_signal_output.npy"), y.detach().cpu().numpy())
+
+        # And resume training state
+        self.train(training)
+
+    def export_cpp_header(self, filename: Path):
+        with TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir)
+            self.export(Path(tmpdir))
+            with open(Path(tmpdir, "config.json"), "r") as fp:
+                _c = json.load(fp)
+            version = _c["version"]
+            config = _c["config"]
+            params = np.load(Path(tmpdir, "weights.npy"))
+        with open(filename, "w") as f:
+            f.writelines(
+                (
+                    "#pragma once\n",
+                    "// Automatically-generated model file\n",
+                    "// HyperConvNet model\n" "#include <vector>\n",
+                    f'#define PYTHON_MODEL_VERSION "{version}"\n',
+                    f'const int HYPER_NET_INPUT_DIM = {config["hyper_net"]["input_dim"]};\n',
+                    f'const int HYPER_NET_NUM_LAYERS = {config["hyper_net"]["num_layers"]};\n',
+                    f'const int HYPER_NET_NUM_UNITS = {config["hyper_net"]["num_units"]};\n',
+                    f'const int HYPER_NET_BATCHNORM = {"true" if config["hyper_net"]["batchnorm"] else "false"};\n',
+                    f"const int CHANNELS = {config['net']['channels']};\n",
+                    f"const bool BATCHNORM = {'true' if config['net']['batchnorm'] else 'false'};\n",
+                    "std::vector<int> DILATIONS{"
+                    + ",".join([str(d) for d in config["net"]["dilations"]])
+                    + "};\n",
+                    f"const std::string ACTIVATION = \"{config['net']['activation']}\";\n",
+                    "std::vector<float> PARAMS{"
+                    + ",".join([f"{w:.16f}" for w in params])
+                    + "};\n",
+                )
+            )
+
+    @classmethod
+    def _get_net(cls, config):
+        channels = config["channels"]
+        dilations = config["dilations"]
+        batchnorm = config["batchnorm"]
+        activation = config["activation"]
+
+        layers = []
+        layer_specs = []
+        cin = 1
+        for dilation in dilations:
+            layer = _Conv(cin, channels, 2, dilation=dilation, bias=not batchnorm)
+            layers.append(layer)
+            layer_specs.append(layer.get_spec())
+            if batchnorm:
+                # Slow momentum on main net bc it's wild
+                layer = _BatchNorm(channels, momentum=0.01)
+                layers.append(layer)
+                layer_specs.append(layer.get_spec())
+            layer = _get_activation(activation)
+            layers.append(layer)
+            layer_specs.append(layer.get_spec())
+            cin = channels
+        layer = _Conv(cin, 1, 1)
+        layers.append(layer)
+        layer_specs.append(layer.get_spec())
+        layer = _Flatten()
+        layers.append(layer)
+        layer_specs.append(layer.get_spec())
+
+        return nn.ModuleList(layers), layer_specs
+
+    @classmethod
+    def _get_hyper_net(cls, config, specs) -> HyperNet:
+        def block(dx, dy, batchnorm) -> _HyperNetBlock:
+            layer_list = [nn.Linear(dx, dy)]
+            if batchnorm:
+                layer_list.append(nn.BatchNorm1d(dy))
+            layer_list.append(nn.ReLU())
+            return _HyperNetBlock(*layer_list)
+
+        num_inputs = config["num_inputs"]
+        num_layers = config["num_layers"]
+        num_units = config["num_units"]
+        batchnorm = config["batchnorm"]
+        # Flatten specs
+        numels = [np.prod(np.array(shape)) for spec in specs for shape in spec.shapes]
+        norms = [norm for spec in specs for norm in spec.norms]
+        biases = [bias for spec in specs for bias in spec.biases]
+        num_outputs = sum(numels)
+
+        din, layer_list = num_inputs, []
+        for _ in range(num_layers):
+            layer_list.append(block(din, num_units, batchnorm))
+            din = num_units
+        layer_list.append(nn.Linear(din, num_outputs))
+        net = nn.Sequential(*layer_list)
+
+        return HyperNet(num_inputs, net, numels, norms, biases)
+
+    @property
+    def _activation(self) -> str:
+        """
+        What activation does the main net use
+        """
+        for m in self._net.modules():
+            if isinstance(m, _Activation):
+                return m.name
+
+    @property
+    def _batchnorm(self) -> bool:
+        return any(isinstance(x, _BatchNorm) for x in self._net)
+
+    @property
+    def _channels(self) -> int:
+        return self._net[0].weight.shape[0]
+
+    @property
+    def _net_no_head(self):
+        return self._net[:-2]
+
+    def _forward(self, params: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
+        net_params = self._hyper_net(params)
+        i = 0
+        for m in self._net:
+            j = i + m.num_tensors
+            x = m(net_params[i:j], x)
+            i = j
+        assert j == len(net_params)
+        return x
+
+    def _get_dilations(self) -> List[int]:
+        dilations = []
+        for (
+            layer
+        ) in self._net_no_head:  # Last two layers are a 1D conv head and flatten
+            if isinstance(layer, _Conv):
+                dilations.append(layer.dilation[0])
+        return dilations
+
+    def _export_config(self):
+        return {
+            "version": __version__,
+            "architecture": "HyperConvNet",
+            "config": {
+                "hyper_net": {
+                    "input_dim": self._hyper_net.input_dim,
+                    "num_layers": self._hyper_net.num_layers,
+                    "num_units": self._hyper_net.num_units,
+                    "batchnorm": self._hyper_net.batchnorm,
+                },
+                "net": {
+                    "channels": self._channels,
+                    "dilations": self._get_dilations(),
+                    "batchnorm": self._batchnorm,
+                    "activation": self._activation,
+                },
+            },
+        }
+
+    def _export_weights(self) -> np.ndarray:
+        """
+        Flatten the parameters of the network to be exported.
+        See doctsring for .export() for ensured layout.
+        """
+        return np.concatenate(
+            [self._hyper_net.get_export_params(), self._export_net_weights()]
+        )
+
+    def _export_net_weights(self) -> np.ndarray:
+        """
+        Only the buffers--parameters are outputted by the hypernet!
+        """
+        params = []
+        for bn in self._net_no_head:
+            if isinstance(bn, _BatchNorm):
+                params.append(bn.running_mean.flatten())
+                params.append(bn.running_var.flatten())
+                params.append(torch.Tensor([bn.eps]).to(bn.running_mean.device))
+        return (
+            np.array([])
+            if len(params) == 0
+            else torch.cat(params).detach().cpu().numpy()
+        )
+
+    def _export_input_output(self) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        params = torch.randn((self._hyper_net.input_dim,))
+        x = torch.randn((2 * self.receptive_field,))
+        x = 0.5 * x / x.abs().max()
+        y = self(params, x)
+        return params, x, y
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/parametric/params.py` & `neural-amp-modeler-0.5.2/nam/models/parametric/params.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# File: params.py
-# Created Date: Sunday July 17th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Handling parametric inputs
-"""
-
-import abc
-import inspect
-from dataclasses import dataclass, fields
-from enum import Enum
-from typing import Any
-
-from ..._core import InitializableFromConfig
-
-
-# class ParamType(Enum):
-#     CONTINUOUS = "continuous"
-#     BOOLEAN = "boolean"
-
-
-@dataclass
-class Param(InitializableFromConfig):
-    default_value: Any
-
-    @classmethod
-    def init_from_config(cls, config):
-        C, kwargs = cls.parse_config(config)
-        return C(**kwargs)
-
-    @classmethod
-    def parse_config(cls, config):
-        for C in [
-            _C
-            for _C in globals().values()
-            if inspect.isclass(_C) and _C is not Param and issubclass(_C, Param)
-        ]:
-            if C.typestr() == config["type"]:
-                config.pop("type")
-                break
-        else:
-            raise ValueError(f"Unrecognized aprameter type {config['type']}")
-        return C, config
-
-    @abc.abstractclassmethod
-    def typestr(cls) -> str:
-        pass
-
-    def to_json(self):
-        return {
-            "type": self.typestr(),
-            **{f.name: getattr(self, f.name) for f in fields(self)},
-        }
-
-
-@dataclass
-class BooleanParam(Param):
-    @classmethod
-    def typestr(cls) -> str:
-        return "boolean"
-
-
-@dataclass
-class ContinuousParam(Param):
-    minval: float
-    maxval: float
-
-    @classmethod
-    def typestr(self) -> str:
-        return "continuous"
+# File: params.py
+# Created Date: Sunday July 17th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Handling parametric inputs
+"""
+
+import abc
+import inspect
+from dataclasses import dataclass, fields
+from enum import Enum
+from typing import Any
+
+from ..._core import InitializableFromConfig
+
+
+# class ParamType(Enum):
+#     CONTINUOUS = "continuous"
+#     BOOLEAN = "boolean"
+
+
+@dataclass
+class Param(InitializableFromConfig):
+    default_value: Any
+
+    @classmethod
+    def init_from_config(cls, config):
+        C, kwargs = cls.parse_config(config)
+        return C(**kwargs)
+
+    @classmethod
+    def parse_config(cls, config):
+        for C in [
+            _C
+            for _C in globals().values()
+            if inspect.isclass(_C) and _C is not Param and issubclass(_C, Param)
+        ]:
+            if C.typestr() == config["type"]:
+                config.pop("type")
+                break
+        else:
+            raise ValueError(f"Unrecognized aprameter type {config['type']}")
+        return C, config
+
+    @abc.abstractclassmethod
+    def typestr(cls) -> str:
+        pass
+
+    def to_json(self):
+        return {
+            "type": self.typestr(),
+            **{f.name: getattr(self, f.name) for f in fields(self)},
+        }
+
+
+@dataclass
+class BooleanParam(Param):
+    @classmethod
+    def typestr(cls) -> str:
+        return "boolean"
+
+
+@dataclass
+class ContinuousParam(Param):
+    minval: float
+    maxval: float
+
+    @classmethod
+    def typestr(self) -> str:
+        return "continuous"
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/recurrent.py` & `neural-amp-modeler-0.5.2/nam/models/recurrent.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,469 +1,469 @@
-# File: recurrent.py
-# Created Date: Saturday July 2nd 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Recurrent models (LSTM)
-
-TODO batch_first=False (I get it...)
-"""
-
-import json
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Optional, Tuple
-
-import numpy as np
-import torch
-import torch.nn as nn
-
-from ._base import BaseNet
-
-
-# TODO merge LSTMCore into LSTM
-
-
-class _L(nn.LSTM):
-    """
-    Tweaks to PyTorch LSTM module
-    * Up the remembering
-    """
-
-    def reset_parameters(self) -> None:
-        super().reset_parameters()
-        # https://danijar.com/tips-for-training-recurrent-neural-networks/
-        # forget += 1
-        # ifgo
-        value = 2.0
-        idx_input = slice(0, self.hidden_size)
-        idx_forget = slice(self.hidden_size, 2 * self.hidden_size)
-        for layer in range(self.num_layers):
-            for input in ("i", "h"):
-                # Balance out the scale of the cell w/ a -=1
-                getattr(self, f"bias_{input}h_l{layer}").data[idx_input] -= value
-                getattr(self, f"bias_{input}h_l{layer}").data[idx_forget] += value
-
-
-# State:
-# L: Number of LSTM layers
-# DH: Hidden state dimension
-# [0]: hidden (L,DH)
-# [1]: cell (L,DH)
-_LSTMHiddenType = torch.Tensor
-_LSTMCellType = torch.Tensor
-_LSTMHiddenCellType = Tuple[_LSTMHiddenType, _LSTMCellType]
-
-
-class LSTMCore(_L):
-    def __init__(
-        self,
-        *args,
-        train_burn_in: Optional[int] = None,
-        train_truncate: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(*args, **kwargs)
-        if not self.batch_first:
-            raise NotImplementedError("Need batch first")
-        self._train_burn_in = train_burn_in
-        self._train_truncate = train_truncate
-        assert len(args) < 3, "Provide as kwargs"
-        self._initial_cell = nn.Parameter(
-            torch.zeros((self.num_layers, self.hidden_size))
-        )
-        self._initial_hidden = nn.Parameter(
-            torch.zeros((self.num_layers, self.hidden_size))
-        )
-
-    def forward(self, x, hidden_state=None):
-        """
-        Same as nn.LSTM.forward except:
-        * Learned inital state
-        * truncated BPTT when .training
-        """
-        if x.ndim != 3:
-            raise NotImplementedError("Need (B,L,D)")
-        last_hidden_state = (
-            self._initial_state(None if x.ndim == 2 else len(x))
-            if hidden_state is None
-            else hidden_state
-        )
-        if not self.training or self._train_truncate is None:
-            output_features = super().forward(x, last_hidden_state)[0]
-        else:
-            output_features_list = []
-            if self._train_burn_in is not None:
-                last_output_features, last_hidden_state = super().forward(
-                    x[:, : self._train_burn_in, :], last_hidden_state
-                )
-                output_features_list.append(last_output_features.detach())
-            burn_in_offset = 0 if self._train_burn_in is None else self._train_burn_in
-            for i in range(burn_in_offset, x.shape[1], self._train_truncate):
-                if i > burn_in_offset:
-                    # Don't detach the burn-in state so that we can learn it.
-                    last_hidden_state = tuple(z.detach() for z in last_hidden_state)
-                last_output_features, last_hidden_state = super().forward(
-                    x[:, i : i + self._train_truncate, :], last_hidden_state
-                )
-                output_features_list.append(last_output_features)
-            output_features = torch.cat(output_features_list, dim=1)
-        return output_features
-
-    def _initial_state(self, n: Optional[int]) -> _LSTMHiddenCellType:
-        return (
-            (self._initial_hidden, self._initial_cell)
-            if n is None
-            else (
-                torch.tile(self._initial_hidden[:, None], (1, n, 1)),
-                torch.tile(self._initial_cell[:, None], (1, n, 1)),
-            )
-        )
-
-
-class LSTM(BaseNet):
-    """
-    ABC for recurrent architectures
-    """
-
-    def __init__(
-        self,
-        hidden_size,
-        train_burn_in: Optional[int] = None,
-        train_truncate: Optional[int] = None,
-        input_size: int = 1,
-        **lstm_kwargs,
-    ):
-        """
-        :param hidden_size: for LSTM
-        :param train_burn_in: Detach calculations from first (this many) samples when
-            training to burn in the hidden state.
-        :param train_truncate: detach the hidden & cell states every this many steps
-            during training so that backpropagation through time is faster + to simulate
-            better starting states for h(t0)&c(t0) (instead of zeros)
-            TODO recognition head to start the hidden state in a good place?
-        :param input_size: Usually 1 (mono input). A catnet extending this might change
-            it and provide the parametric inputs as additional input dimensions.
-        """
-        super().__init__()
-        if "batch_first" in lstm_kwargs:
-            raise ValueError("batch_first cannot be set.")
-        self._input_size = input_size
-        self._core = _L(self._input_size, hidden_size, batch_first=True, **lstm_kwargs)
-        self._head = nn.Linear(hidden_size, 1)
-        self._train_burn_in = train_burn_in
-        self._train_truncate = train_truncate
-        self._initial_cell = nn.Parameter(
-            torch.zeros((lstm_kwargs.get("num_layers", 1), hidden_size))
-        )
-        self._initial_hidden = nn.Parameter(
-            torch.zeros((lstm_kwargs.get("num_layers", 1), hidden_size))
-        )
-
-    @property
-    def receptive_field(self) -> int:
-        return 1
-
-    @property
-    def pad_start_default(self) -> bool:
-        # I should simplify this...
-        return True
-
-    def export_cpp_header(self, filename: Path):
-        with TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir)
-            LSTM.export(self, Path(tmpdir))  # Hacky...need to work w/ CatLSTM
-            with open(Path(tmpdir, "model.nam"), "r") as fp:
-                _c = json.load(fp)
-            version = _c["version"]
-            config = _c["config"]
-            s_parametric = self._export_cpp_header_parametric(config.get("parametric"))
-            with open(filename, "w") as f:
-                f.writelines(
-                    (
-                        "#pragma once\n",
-                        "// Automatically-generated model file\n",
-                        "#include <vector>\n",
-                        '#include "json.hpp"\n',
-                        '#include "lstm.h"\n',
-                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
-                        f'const int NUM_LAYERS = {config["num_layers"]};\n',
-                        f'const int INPUT_SIZE = {config["input_size"]};\n',
-                        f'const int HIDDEN_SIZE = {config["hidden_size"]};\n',
-                    )
-                    + s_parametric
-                    + (
-                        "std::vector<float> PARAMS{"
-                        + ", ".join([f"{w:.16f}f" for w in _c["weights"]])
-                        + "};\n",
-                    )
-                )
-
-    def export_onnx(self, filename: Path):
-        if self._input_size != 1:
-            raise NotImplementedError("Multi-dimensional inputs not supported yet")
-        o = _ONNXWrapped(self)
-        x = torch.randn((64,))  # (S,)
-        h, c = [z[:, 0, :] for z in self._initial_state(1)]  # (L,DH), (L,DH)
-        torch.onnx.export(
-            o,
-            (x, h, c),
-            filename,
-            input_names=["x", "hin", "cin"],
-            output_names=["y", "hout", "cout"],
-            dynamic_axes={"x": {0: "num_frames"}, "y": {0: "num_frames"}},
-        )
-
-    def forward_onnx(
-        self, x: torch.Tensor, h: _LSTMHiddenType, c: _LSTMCellType
-    ) -> Tuple[torch.Tensor, _LSTMHiddenType, _LSTMCellType]:
-        """
-        Forward pass used by ONNX export
-        Only supports scalar inputs right now.
-
-        N: Sequeence length
-        L: Number of layers
-        DH: Hidden state dimension
-
-        :param x: (N,)
-        :param state: (L, DH)
-        :param cell: (L, DH)
-
-        :return: (N,), (L, DH), (L, DH)
-        """
-        features, (h, c) = self._core(x[None, :, None], (h[:, None, :], c[:, None, :]))
-        y = self._apply_head(features)  # (1,S)
-        return y[0, :], h[:, 0, :], c[:, 0, :]
-
-    def _apply_head(self, features: torch.Tensor) -> torch.Tensor:
-        """
-        :param features: (B,S,DH)
-        :return: (B,S)
-        """
-        return self._head(features)[:, :, 0]
-
-    def _forward(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        :param x: (B,L) or (B,L,D)
-        :return: (B,L)
-        """
-        last_hidden_state = self._initial_state(len(x))
-        if x.ndim == 2:
-            x = x[:, :, None]
-        if not self.training or self._train_truncate is None:
-            output_features = self._core(x, last_hidden_state)[0]
-        else:
-            output_features_list = []
-            if self._train_burn_in is not None:
-                last_output_features, last_hidden_state = self._core(
-                    x[:, : self._train_burn_in, :], last_hidden_state
-                )
-                output_features_list.append(last_output_features.detach())
-            burn_in_offset = 0 if self._train_burn_in is None else self._train_burn_in
-            for i in range(burn_in_offset, x.shape[1], self._train_truncate):
-                if i > burn_in_offset:
-                    # Don't detach the burn-in state so that we can learn it.
-                    last_hidden_state = tuple(z.detach() for z in last_hidden_state)
-                last_output_features, last_hidden_state = self._core(
-                    x[:, i : i + self._train_truncate, :], last_hidden_state
-                )
-                output_features_list.append(last_output_features)
-            output_features = torch.cat(output_features_list, dim=1)
-        return self._apply_head(output_features)
-
-    def _export_cell_weights(
-        self, i: int, hidden_state: torch.Tensor, cell_state: torch.Tensor
-    ) -> np.ndarray:
-        """
-        * weight matrix (xh -> ifco)
-        * bias vector
-        * Initial hidden state
-        * Initial cell state
-        """
-
-        tensors = [
-            torch.cat(
-                [
-                    getattr(self._core, f"weight_ih_l{i}").data,
-                    getattr(self._core, f"weight_hh_l{i}").data,
-                ],
-                dim=1,
-            ),
-            getattr(self._core, f"bias_ih_l{i}").data
-            + getattr(self._core, f"bias_hh_l{i}").data,
-            hidden_state,
-            cell_state,
-        ]
-        return np.concatenate([z.detach().cpu().numpy().flatten() for z in tensors])
-
-    def _export_config(self):
-        return {
-            "input_size": self._core.input_size,
-            "hidden_size": self._core.hidden_size,
-            "num_layers": self._core.num_layers,
-        }
-
-    def _export_cpp_header_parametric(self, config):
-        # TODO refactor to merge w/ WaveNet implementation
-        if config is not None:
-            raise ValueError("Got non-None parametric config")
-        return ("nlohmann::json PARAMETRIC {};\n",)
-
-    def _export_weights(self):
-        """
-        * Loop over cells:
-            * weight matrix (xh -> ifco)
-            * bias vector
-            * Initial hidden state
-            * Initial cell state
-        * Head weights
-        * Head bias
-        """
-        return np.concatenate(
-            [
-                self._export_cell_weights(i, h, c)
-                for i, (h, c) in enumerate(zip(*self._get_initial_state()))
-            ]
-            + [
-                self._head.weight.data.detach().cpu().numpy().flatten(),
-                self._head.bias.data.detach().cpu().numpy().flatten(),
-            ]
-        )
-
-    def _get_initial_state(self, inputs=None) -> _LSTMHiddenCellType:
-        """
-        Convenience function to find a good hidden state to start the plugin at
-
-        DX=input size
-        L=num layers
-        S=sequence length
-        :param inputs: (1,S,DX)
-
-        :return: (L,DH), (L,DH)
-        """
-        inputs = torch.zeros((1, 48_000, 1)) if inputs is None else inputs
-        _, (h, c) = self._core(inputs)
-        return h, c
-
-    def _initial_state(self, n: Optional[int]) -> _LSTMHiddenCellType:
-        """
-        Literally what the forward pass starts with.
-        Default is zeroes; this should be better since it can be learned.
-        """
-        return (
-            (self._initial_hidden, self._initial_cell)
-            if n is None
-            else (
-                torch.tile(self._initial_hidden[:, None], (1, n, 1)),
-                torch.tile(self._initial_cell[:, None], (1, n, 1)),
-            )
-        )
-
-
-class _ONNXWrapped(nn.Module):
-    def __init__(self, net: LSTM):
-        super().__init__()
-        self._net = net
-
-    def forward(
-        self, x: torch.Tensor, hidden: _LSTMHiddenType, cell: _LSTMCellType
-    ) -> Tuple[torch.Tensor, _LSTMHiddenType, _LSTMCellType]:
-        """
-        N: Sequeence length
-        L: Number of layers
-        DH: Hidden state dimension
-
-        :param x: (N,)
-        :param state: (L, DH)
-        :param cell: (L, DH)
-
-        :return: (N,), (L, DH), (L, DH)
-        """
-        return self._net.forward_onnx(x, hidden, cell)
-
-
-# TODO refactor together
-
-
-class _SkippyLSTM(nn.Module):
-    def __init__(
-        self, input_size, hidden_size, skip_in: bool = False, num_layers=1, **kwargs
-    ):
-        super().__init__()
-        layers_per_lstm = 1
-        self._skip_in = skip_in
-        self._lstms = nn.ModuleList(
-            [
-                _L(
-                    self._layer_input_size(input_size, hidden_size, i),
-                    hidden_size,
-                    layers_per_lstm,
-                    batch_first=True,
-                )
-                for i in range(num_layers)
-            ]
-        )
-        self._initial_hidden = nn.Parameter(
-            torch.zeros((self.num_layers, layers_per_lstm, self.hidden_size))
-        )
-        self._initial_cell = nn.Parameter(
-            torch.zeros((self.num_layers, layers_per_lstm, self.hidden_size))
-        )
-
-    @property
-    def hidden_size(self):
-        return self._lstms[0].hidden_size
-
-    @property
-    def input_size(self):
-        return self._lstms[0].input_size
-
-    @property
-    def num_layers(self):
-        return len(self._lstms)
-
-    @property
-    def output_size(self):
-        return self.num_layers * self.hidden_size
-
-    def forward(self, input, state=None):
-        """
-        :param input: (N,L,DX)
-        :param state: ((L,Li,N,DH), (L,Li,N,DH))
-
-        :return: (N,L,L*DH), ((L,Li,N,DH), (L,Li,N,DH))
-        """
-        h0, c0 = self.initial_state(input) if state is None else state
-        hiddens, h_arr, c_arr, hidden = [], [], [], None
-        for layer, h0i, c0i in zip(self._lstms, h0, c0):
-            if self._skip_in:
-                # TODO dense-block
-                layer_input = (
-                    input if hidden is None else torch.cat([input, hidden], dim=2)
-                )
-            else:
-                layer_input = input if hidden is None else hidden
-            hidden, (hi, ci) = layer(layer_input, (h0i, c0i))
-            hiddens.append(hidden)
-            h_arr.append(hi)
-            c_arr.append(ci)
-        return (torch.cat(hiddens, dim=2), (torch.stack(h_arr), torch.stack(c_arr)))
-
-    def initial_state(self, input: torch.Tensor):
-        """
-        Initial states for all the layers
-
-        :return: (L,B,Li,DH)
-        """
-        assert input.ndim == 3, "Batch only for now"
-        batch_size = len(input)  # Assume batch_first
-        return (
-            torch.tile(self._initial_hidden[:, :, None], (1, 1, batch_size, 1)),
-            torch.tile(self._initial_cell[:, :, None], (1, 1, batch_size, 1)),
-        )
-
-    def _layer_input_size(self, input_size, hidden_size, i) -> int:
-        # TODO dense-block
-        if self._skip_in:
-            return input_size + (0 if i == 0 else hidden_size)
-        else:
-            return input_size if i == 0 else hidden_size
+# File: recurrent.py
+# Created Date: Saturday July 2nd 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Recurrent models (LSTM)
+
+TODO batch_first=False (I get it...)
+"""
+
+import json
+from pathlib import Path
+from tempfile import TemporaryDirectory
+from typing import Optional, Tuple
+
+import numpy as np
+import torch
+import torch.nn as nn
+
+from ._base import BaseNet
+
+
+# TODO merge LSTMCore into LSTM
+
+
+class _L(nn.LSTM):
+    """
+    Tweaks to PyTorch LSTM module
+    * Up the remembering
+    """
+
+    def reset_parameters(self) -> None:
+        super().reset_parameters()
+        # https://danijar.com/tips-for-training-recurrent-neural-networks/
+        # forget += 1
+        # ifgo
+        value = 2.0
+        idx_input = slice(0, self.hidden_size)
+        idx_forget = slice(self.hidden_size, 2 * self.hidden_size)
+        for layer in range(self.num_layers):
+            for input in ("i", "h"):
+                # Balance out the scale of the cell w/ a -=1
+                getattr(self, f"bias_{input}h_l{layer}").data[idx_input] -= value
+                getattr(self, f"bias_{input}h_l{layer}").data[idx_forget] += value
+
+
+# State:
+# L: Number of LSTM layers
+# DH: Hidden state dimension
+# [0]: hidden (L,DH)
+# [1]: cell (L,DH)
+_LSTMHiddenType = torch.Tensor
+_LSTMCellType = torch.Tensor
+_LSTMHiddenCellType = Tuple[_LSTMHiddenType, _LSTMCellType]
+
+
+class LSTMCore(_L):
+    def __init__(
+        self,
+        *args,
+        train_burn_in: Optional[int] = None,
+        train_truncate: Optional[int] = None,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        if not self.batch_first:
+            raise NotImplementedError("Need batch first")
+        self._train_burn_in = train_burn_in
+        self._train_truncate = train_truncate
+        assert len(args) < 3, "Provide as kwargs"
+        self._initial_cell = nn.Parameter(
+            torch.zeros((self.num_layers, self.hidden_size))
+        )
+        self._initial_hidden = nn.Parameter(
+            torch.zeros((self.num_layers, self.hidden_size))
+        )
+
+    def forward(self, x, hidden_state=None):
+        """
+        Same as nn.LSTM.forward except:
+        * Learned inital state
+        * truncated BPTT when .training
+        """
+        if x.ndim != 3:
+            raise NotImplementedError("Need (B,L,D)")
+        last_hidden_state = (
+            self._initial_state(None if x.ndim == 2 else len(x))
+            if hidden_state is None
+            else hidden_state
+        )
+        if not self.training or self._train_truncate is None:
+            output_features = super().forward(x, last_hidden_state)[0]
+        else:
+            output_features_list = []
+            if self._train_burn_in is not None:
+                last_output_features, last_hidden_state = super().forward(
+                    x[:, : self._train_burn_in, :], last_hidden_state
+                )
+                output_features_list.append(last_output_features.detach())
+            burn_in_offset = 0 if self._train_burn_in is None else self._train_burn_in
+            for i in range(burn_in_offset, x.shape[1], self._train_truncate):
+                if i > burn_in_offset:
+                    # Don't detach the burn-in state so that we can learn it.
+                    last_hidden_state = tuple(z.detach() for z in last_hidden_state)
+                last_output_features, last_hidden_state = super().forward(
+                    x[:, i : i + self._train_truncate, :], last_hidden_state
+                )
+                output_features_list.append(last_output_features)
+            output_features = torch.cat(output_features_list, dim=1)
+        return output_features
+
+    def _initial_state(self, n: Optional[int]) -> _LSTMHiddenCellType:
+        return (
+            (self._initial_hidden, self._initial_cell)
+            if n is None
+            else (
+                torch.tile(self._initial_hidden[:, None], (1, n, 1)),
+                torch.tile(self._initial_cell[:, None], (1, n, 1)),
+            )
+        )
+
+
+class LSTM(BaseNet):
+    """
+    ABC for recurrent architectures
+    """
+
+    def __init__(
+        self,
+        hidden_size,
+        train_burn_in: Optional[int] = None,
+        train_truncate: Optional[int] = None,
+        input_size: int = 1,
+        **lstm_kwargs,
+    ):
+        """
+        :param hidden_size: for LSTM
+        :param train_burn_in: Detach calculations from first (this many) samples when
+            training to burn in the hidden state.
+        :param train_truncate: detach the hidden & cell states every this many steps
+            during training so that backpropagation through time is faster + to simulate
+            better starting states for h(t0)&c(t0) (instead of zeros)
+            TODO recognition head to start the hidden state in a good place?
+        :param input_size: Usually 1 (mono input). A catnet extending this might change
+            it and provide the parametric inputs as additional input dimensions.
+        """
+        super().__init__()
+        if "batch_first" in lstm_kwargs:
+            raise ValueError("batch_first cannot be set.")
+        self._input_size = input_size
+        self._core = _L(self._input_size, hidden_size, batch_first=True, **lstm_kwargs)
+        self._head = nn.Linear(hidden_size, 1)
+        self._train_burn_in = train_burn_in
+        self._train_truncate = train_truncate
+        self._initial_cell = nn.Parameter(
+            torch.zeros((lstm_kwargs.get("num_layers", 1), hidden_size))
+        )
+        self._initial_hidden = nn.Parameter(
+            torch.zeros((lstm_kwargs.get("num_layers", 1), hidden_size))
+        )
+
+    @property
+    def receptive_field(self) -> int:
+        return 1
+
+    @property
+    def pad_start_default(self) -> bool:
+        # I should simplify this...
+        return True
+
+    def export_cpp_header(self, filename: Path):
+        with TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir)
+            LSTM.export(self, Path(tmpdir))  # Hacky...need to work w/ CatLSTM
+            with open(Path(tmpdir, "model.nam"), "r") as fp:
+                _c = json.load(fp)
+            version = _c["version"]
+            config = _c["config"]
+            s_parametric = self._export_cpp_header_parametric(config.get("parametric"))
+            with open(filename, "w") as f:
+                f.writelines(
+                    (
+                        "#pragma once\n",
+                        "// Automatically-generated model file\n",
+                        "#include <vector>\n",
+                        '#include "json.hpp"\n',
+                        '#include "lstm.h"\n',
+                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
+                        f'const int NUM_LAYERS = {config["num_layers"]};\n',
+                        f'const int INPUT_SIZE = {config["input_size"]};\n',
+                        f'const int HIDDEN_SIZE = {config["hidden_size"]};\n',
+                    )
+                    + s_parametric
+                    + (
+                        "std::vector<float> PARAMS{"
+                        + ", ".join([f"{w:.16f}f" for w in _c["weights"]])
+                        + "};\n",
+                    )
+                )
+
+    def export_onnx(self, filename: Path):
+        if self._input_size != 1:
+            raise NotImplementedError("Multi-dimensional inputs not supported yet")
+        o = _ONNXWrapped(self)
+        x = torch.randn((64,))  # (S,)
+        h, c = [z[:, 0, :] for z in self._initial_state(1)]  # (L,DH), (L,DH)
+        torch.onnx.export(
+            o,
+            (x, h, c),
+            filename,
+            input_names=["x", "hin", "cin"],
+            output_names=["y", "hout", "cout"],
+            dynamic_axes={"x": {0: "num_frames"}, "y": {0: "num_frames"}},
+        )
+
+    def forward_onnx(
+        self, x: torch.Tensor, h: _LSTMHiddenType, c: _LSTMCellType
+    ) -> Tuple[torch.Tensor, _LSTMHiddenType, _LSTMCellType]:
+        """
+        Forward pass used by ONNX export
+        Only supports scalar inputs right now.
+
+        N: Sequeence length
+        L: Number of layers
+        DH: Hidden state dimension
+
+        :param x: (N,)
+        :param state: (L, DH)
+        :param cell: (L, DH)
+
+        :return: (N,), (L, DH), (L, DH)
+        """
+        features, (h, c) = self._core(x[None, :, None], (h[:, None, :], c[:, None, :]))
+        y = self._apply_head(features)  # (1,S)
+        return y[0, :], h[:, 0, :], c[:, 0, :]
+
+    def _apply_head(self, features: torch.Tensor) -> torch.Tensor:
+        """
+        :param features: (B,S,DH)
+        :return: (B,S)
+        """
+        return self._head(features)[:, :, 0]
+
+    def _forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        :param x: (B,L) or (B,L,D)
+        :return: (B,L)
+        """
+        last_hidden_state = self._initial_state(len(x))
+        if x.ndim == 2:
+            x = x[:, :, None]
+        if not self.training or self._train_truncate is None:
+            output_features = self._core(x, last_hidden_state)[0]
+        else:
+            output_features_list = []
+            if self._train_burn_in is not None:
+                last_output_features, last_hidden_state = self._core(
+                    x[:, : self._train_burn_in, :], last_hidden_state
+                )
+                output_features_list.append(last_output_features.detach())
+            burn_in_offset = 0 if self._train_burn_in is None else self._train_burn_in
+            for i in range(burn_in_offset, x.shape[1], self._train_truncate):
+                if i > burn_in_offset:
+                    # Don't detach the burn-in state so that we can learn it.
+                    last_hidden_state = tuple(z.detach() for z in last_hidden_state)
+                last_output_features, last_hidden_state = self._core(
+                    x[:, i : i + self._train_truncate, :], last_hidden_state
+                )
+                output_features_list.append(last_output_features)
+            output_features = torch.cat(output_features_list, dim=1)
+        return self._apply_head(output_features)
+
+    def _export_cell_weights(
+        self, i: int, hidden_state: torch.Tensor, cell_state: torch.Tensor
+    ) -> np.ndarray:
+        """
+        * weight matrix (xh -> ifco)
+        * bias vector
+        * Initial hidden state
+        * Initial cell state
+        """
+
+        tensors = [
+            torch.cat(
+                [
+                    getattr(self._core, f"weight_ih_l{i}").data,
+                    getattr(self._core, f"weight_hh_l{i}").data,
+                ],
+                dim=1,
+            ),
+            getattr(self._core, f"bias_ih_l{i}").data
+            + getattr(self._core, f"bias_hh_l{i}").data,
+            hidden_state,
+            cell_state,
+        ]
+        return np.concatenate([z.detach().cpu().numpy().flatten() for z in tensors])
+
+    def _export_config(self):
+        return {
+            "input_size": self._core.input_size,
+            "hidden_size": self._core.hidden_size,
+            "num_layers": self._core.num_layers,
+        }
+
+    def _export_cpp_header_parametric(self, config):
+        # TODO refactor to merge w/ WaveNet implementation
+        if config is not None:
+            raise ValueError("Got non-None parametric config")
+        return ("nlohmann::json PARAMETRIC {};\n",)
+
+    def _export_weights(self):
+        """
+        * Loop over cells:
+            * weight matrix (xh -> ifco)
+            * bias vector
+            * Initial hidden state
+            * Initial cell state
+        * Head weights
+        * Head bias
+        """
+        return np.concatenate(
+            [
+                self._export_cell_weights(i, h, c)
+                for i, (h, c) in enumerate(zip(*self._get_initial_state()))
+            ]
+            + [
+                self._head.weight.data.detach().cpu().numpy().flatten(),
+                self._head.bias.data.detach().cpu().numpy().flatten(),
+            ]
+        )
+
+    def _get_initial_state(self, inputs=None) -> _LSTMHiddenCellType:
+        """
+        Convenience function to find a good hidden state to start the plugin at
+
+        DX=input size
+        L=num layers
+        S=sequence length
+        :param inputs: (1,S,DX)
+
+        :return: (L,DH), (L,DH)
+        """
+        inputs = torch.zeros((1, 48_000, 1)) if inputs is None else inputs
+        _, (h, c) = self._core(inputs)
+        return h, c
+
+    def _initial_state(self, n: Optional[int]) -> _LSTMHiddenCellType:
+        """
+        Literally what the forward pass starts with.
+        Default is zeroes; this should be better since it can be learned.
+        """
+        return (
+            (self._initial_hidden, self._initial_cell)
+            if n is None
+            else (
+                torch.tile(self._initial_hidden[:, None], (1, n, 1)),
+                torch.tile(self._initial_cell[:, None], (1, n, 1)),
+            )
+        )
+
+
+class _ONNXWrapped(nn.Module):
+    def __init__(self, net: LSTM):
+        super().__init__()
+        self._net = net
+
+    def forward(
+        self, x: torch.Tensor, hidden: _LSTMHiddenType, cell: _LSTMCellType
+    ) -> Tuple[torch.Tensor, _LSTMHiddenType, _LSTMCellType]:
+        """
+        N: Sequeence length
+        L: Number of layers
+        DH: Hidden state dimension
+
+        :param x: (N,)
+        :param state: (L, DH)
+        :param cell: (L, DH)
+
+        :return: (N,), (L, DH), (L, DH)
+        """
+        return self._net.forward_onnx(x, hidden, cell)
+
+
+# TODO refactor together
+
+
+class _SkippyLSTM(nn.Module):
+    def __init__(
+        self, input_size, hidden_size, skip_in: bool = False, num_layers=1, **kwargs
+    ):
+        super().__init__()
+        layers_per_lstm = 1
+        self._skip_in = skip_in
+        self._lstms = nn.ModuleList(
+            [
+                _L(
+                    self._layer_input_size(input_size, hidden_size, i),
+                    hidden_size,
+                    layers_per_lstm,
+                    batch_first=True,
+                )
+                for i in range(num_layers)
+            ]
+        )
+        self._initial_hidden = nn.Parameter(
+            torch.zeros((self.num_layers, layers_per_lstm, self.hidden_size))
+        )
+        self._initial_cell = nn.Parameter(
+            torch.zeros((self.num_layers, layers_per_lstm, self.hidden_size))
+        )
+
+    @property
+    def hidden_size(self):
+        return self._lstms[0].hidden_size
+
+    @property
+    def input_size(self):
+        return self._lstms[0].input_size
+
+    @property
+    def num_layers(self):
+        return len(self._lstms)
+
+    @property
+    def output_size(self):
+        return self.num_layers * self.hidden_size
+
+    def forward(self, input, state=None):
+        """
+        :param input: (N,L,DX)
+        :param state: ((L,Li,N,DH), (L,Li,N,DH))
+
+        :return: (N,L,L*DH), ((L,Li,N,DH), (L,Li,N,DH))
+        """
+        h0, c0 = self.initial_state(input) if state is None else state
+        hiddens, h_arr, c_arr, hidden = [], [], [], None
+        for layer, h0i, c0i in zip(self._lstms, h0, c0):
+            if self._skip_in:
+                # TODO dense-block
+                layer_input = (
+                    input if hidden is None else torch.cat([input, hidden], dim=2)
+                )
+            else:
+                layer_input = input if hidden is None else hidden
+            hidden, (hi, ci) = layer(layer_input, (h0i, c0i))
+            hiddens.append(hidden)
+            h_arr.append(hi)
+            c_arr.append(ci)
+        return (torch.cat(hiddens, dim=2), (torch.stack(h_arr), torch.stack(c_arr)))
+
+    def initial_state(self, input: torch.Tensor):
+        """
+        Initial states for all the layers
+
+        :return: (L,B,Li,DH)
+        """
+        assert input.ndim == 3, "Batch only for now"
+        batch_size = len(input)  # Assume batch_first
+        return (
+            torch.tile(self._initial_hidden[:, :, None], (1, 1, batch_size, 1)),
+            torch.tile(self._initial_cell[:, :, None], (1, 1, batch_size, 1)),
+        )
+
+    def _layer_input_size(self, input_size, hidden_size, i) -> int:
+        # TODO dense-block
+        if self._skip_in:
+            return input_size + (0 if i == 0 else hidden_size)
+        else:
+            return input_size if i == 0 else hidden_size
```

### Comparing `neural-amp-modeler-0.5.1/nam/models/wavenet.py` & `neural-amp-modeler-0.5.2/nam/models/wavenet.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,395 +1,395 @@
-# File: wavenet.py
-# Created Date: Friday July 29th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-WaveNet implementation
-https://arxiv.org/abs/1609.03499
-"""
-
-import json
-from copy import deepcopy
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Dict, Optional, Sequence, Tuple
-
-import numpy as np
-import torch
-import torch.nn as nn
-
-from ._activations import get_activation
-from ._base import BaseNet
-from ._names import ACTIVATION_NAME, CONV_NAME
-
-
-class Conv1d(nn.Conv1d):
-    def export_weights(self) -> torch.Tensor:
-        tensors = []
-        if self.weight is not None:
-            tensors.append(self.weight.data.flatten())
-        if self.bias is not None:
-            tensors.append(self.bias.data.flatten())
-        if len(tensors) == 0:
-            return torch.zeros((0,))
-        else:
-            return torch.cat(tensors)
-
-
-class _Layer(nn.Module):
-    def __init__(
-        self,
-        condition_size: int,
-        channels: int,
-        kernel_size: int,
-        dilation: int,
-        activation: str,
-        gated: bool,
-    ):
-        super().__init__()
-        # Input mixer takes care of the bias
-        mid_channels = 2 * channels if gated else channels
-        self._conv = Conv1d(channels, mid_channels, kernel_size, dilation=dilation)
-        # Custom init: favors direct input-output
-        # self._conv.weight.data.zero_()
-        self._input_mixer = Conv1d(condition_size, mid_channels, 1, bias=False)
-        self._activation = get_activation(activation)
-        self._activation_name = activation
-        self._1x1 = Conv1d(channels, channels, 1)
-        self._gated = gated
-
-    @property
-    def activation_name(self) -> str:
-        return self._activation_name
-
-    @property
-    def conv(self) -> Conv1d:
-        return self._conv
-
-    @property
-    def gated(self) -> bool:
-        return self._gated
-
-    @property
-    def kernel_size(self) -> int:
-        return self._conv.kernel_size[0]
-
-    def export_weights(self) -> torch.Tensor:
-        return torch.cat(
-            [
-                self.conv.export_weights(),
-                self._input_mixer.export_weights(),
-                self._1x1.export_weights(),
-            ]
-        )
-
-    def forward(
-        self, x: torch.Tensor, h: Optional[torch.Tensor], out_length: int
-    ) -> Tuple[Optional[torch.Tensor], torch.Tensor]:
-        """
-        :param x: (B,C,L1) From last layer
-        :param h: (B,DX,L2) Conditioning. If first, ignored.
-
-        :return:
-            If not final:
-                (B,C,L1-d) to next layer
-                (B,C,L1-d) to mixer
-            If final, next layer is None
-        """
-        zconv = self.conv(x)
-        z1 = zconv + self._input_mixer(h)[:, :, -zconv.shape[2] :]
-        post_activation = (
-            self._activation(z1)
-            if not self._gated
-            else (
-                self._activation(z1[:, : self._channels])
-                * torch.sigmoid(z1[:, self._channels :])
-            )
-        )
-        return (
-            x[:, :, -post_activation.shape[2] :] + self._1x1(post_activation),
-            post_activation[:, :, -out_length:],
-        )
-
-    @property
-    def _channels(self) -> int:
-        return self._1x1.in_channels
-
-
-class _Layers(nn.Module):
-    """
-    Takes in the input and condition (and maybe the head input so far); outputs the
-    layer output and head input.
-
-    The original WaveNet only uses one of these, but you can stack multiple of this
-    module to vary the channels throughout with minimal extra channel-changing conv
-    layers.
-    """
-
-    def __init__(
-        self,
-        input_size: int,
-        condition_size: int,
-        head_size,
-        channels: int,
-        kernel_size: int,
-        dilations: Sequence[int],
-        activation: str = "Tanh",
-        gated: bool = True,
-        head_bias: bool = True,
-    ):
-        super().__init__()
-        self._rechannel = Conv1d(input_size, channels, 1, bias=False)
-        self._layers = nn.ModuleList(
-            [
-                _Layer(
-                    condition_size, channels, kernel_size, dilation, activation, gated
-                )
-                for dilation in dilations
-            ]
-        )
-        # Convert the head input from channels to head_size
-        self._head_rechannel = Conv1d(channels, head_size, 1, bias=head_bias)
-
-        self._config = {
-            "input_size": input_size,
-            "condition_size": condition_size,
-            "head_size": head_size,
-            "channels": channels,
-            "kernel_size": kernel_size,
-            "dilations": dilations,
-            "activation": activation,
-            "gated": gated,
-            "head_bias": head_bias,
-        }
-
-    @property
-    def receptive_field(self) -> int:
-        return 1 + (self._kernel_size - 1) * sum(self._dilations)
-
-    def export_config(self):
-        return deepcopy(self._config)
-
-    def export_weights(self) -> torch.Tensor:
-        return torch.cat(
-            [self._rechannel.export_weights()]
-            + [layer.export_weights() for layer in self._layers]
-            + [self._head_rechannel.export_weights()]
-        )
-
-    def forward(
-        self,
-        x: torch.Tensor,
-        c: torch.Tensor,
-        head_input: Optional[torch.Tensor] = None,
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        """
-        :param x: (B,Dx,L) layer input
-        :param c: (B,Dc,L) condition
-
-        :return:
-            (B,Dc,L-R+1) head input
-            (B,Dc,L-R+1) layer output
-        """
-        out_length = x.shape[2] - (self.receptive_field - 1)
-        x = self._rechannel(x)
-        for layer in self._layers:
-            x, head_term = layer(x, c, out_length)  # Ensures head_term sample length
-            head_input = (
-                head_term
-                if head_input is None
-                else head_input[:, :, -out_length:] + head_term
-            )
-        return self._head_rechannel(head_input), x
-
-    @property
-    def _dilations(self) -> Sequence[int]:
-        return self._config["dilations"]
-
-    @property
-    def _kernel_size(self) -> int:
-        return self._layers[0].kernel_size
-
-
-class _Head(nn.Module):
-    def __init__(
-        self,
-        in_channels: int,
-        channels: int,
-        activation: str,
-        num_layers: int,
-        out_channels: int,
-    ):
-        super().__init__()
-
-        def block(cx, cy):
-            net = nn.Sequential()
-            net.add_module(ACTIVATION_NAME, get_activation(activation))
-            net.add_module(CONV_NAME, Conv1d(cx, cy, 1))
-            return net
-
-        assert num_layers > 0
-
-        layers = nn.Sequential()
-        cin = in_channels
-        for i in range(num_layers):
-            layers.add_module(
-                f"layer_{i}",
-                block(cin, channels if i != num_layers - 1 else out_channels),
-            )
-            cin = channels
-        self._layers = layers
-
-        self._config = {
-            "channels": channels,
-            "activation": activation,
-            "num_layers": num_layers,
-            "out_channels": out_channels,
-        }
-
-    def export_config(self):
-        return deepcopy(self._config)
-
-    def export_weights(self) -> torch.Tensor:
-        return torch.cat([layer[1].export_weights() for layer in self._layers])
-
-    def forward(self, *args, **kwargs):
-        return self._layers(*args, **kwargs)
-
-
-class _WaveNet(nn.Module):
-    def __init__(
-        self,
-        layers_configs: Sequence[Dict],
-        head_config: Optional[Dict] = None,
-        head_scale: float = 1.0,
-    ):
-        super().__init__()
-
-        self._layers = nn.ModuleList([_Layers(**lc) for lc in layers_configs])
-        self._head = None if head_config is None else _Head(**head_config)
-        self._head_scale = head_scale
-
-    @property
-    def receptive_field(self) -> int:
-        return 1 + sum([(layer.receptive_field - 1) for layer in self._layers])
-
-    def export_config(self):
-        return {
-            "layers": [layers.export_config() for layers in self._layers],
-            "head": None if self._head is None else self._head.export_config(),
-            "head_scale": self._head_scale,
-        }
-
-    def export_weights(self) -> np.ndarray:
-        """
-        :return: 1D array
-        """
-        weights = torch.cat([layer.export_weights() for layer in self._layers])
-        if self._head is not None:
-            weights = torch.cat([weights, self._head.export_weights()])
-        weights = torch.cat([weights, torch.Tensor([self._head_scale])])
-        return weights.detach().cpu().numpy()
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        :param x: (B,Cx,L)
-        :return: (B,Cy,L-R)
-        """
-        y, head_input = x, None
-        for layer in self._layers:
-            head_input, y = layer(y, x, head_input=head_input)
-        head_input = self._head_scale * head_input
-        return head_input if self._head is None else self._head(head_input)
-
-
-class WaveNet(BaseNet):
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        self._net = _WaveNet(*args, **kwargs)
-
-    @property
-    def pad_start_default(self) -> bool:
-        return True
-
-    @property
-    def receptive_field(self) -> int:
-        return self._net.receptive_field
-
-    def export_cpp_header(self, filename: Path):
-        with TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir)
-            WaveNet.export(self, Path(tmpdir))  # Hacky...need to work w/ CatWaveNet
-            with open(Path(tmpdir, "model.nam"), "r") as fp:
-                _c = json.load(fp)
-            version = _c["version"]
-            config = _c["config"]
-
-            if config["head"] is not None:
-                raise NotImplementedError("No heads yet")
-            # head_scale
-            # with_head
-            # parametric
-
-            # String for layer array params:
-            s_lap = (
-                "const std::vector<wavenet::LayerArrayParams> LAYER_ARRAY_PARAMS{\n",
-            )
-            for i, lc in enumerate(config["layers"], 1):
-                s_lap_line = (
-                    f'  wavenet::LayerArrayParams({lc["input_size"]}, '
-                    f'{lc["condition_size"]}, {lc["head_size"]}, {lc["channels"]}, '
-                    f'{lc["kernel_size"]}, std::vector<int> '
-                    "{"
-                    + ", ".join([str(d) for d in lc["dilations"]])
-                    + "}, "
-                    + (
-                        f'"{lc["activation"]}", {str(lc["gated"]).lower()}, '
-                        f'{str(lc["head_bias"]).lower()})'
-                    )
-                )
-                if i < len(config["layers"]):
-                    s_lap_line += ","
-                s_lap_line += "\n"
-                s_lap += (s_lap_line,)
-            s_lap += ("};\n",)
-            s_parametric = self._export_cpp_header_parametric(config.get("parametric"))
-            with open(filename, "w") as f:
-                f.writelines(
-                    (
-                        "#pragma once\n",
-                        "// Automatically-generated model file\n",
-                        "#include <vector>\n",
-                        '#include "json.hpp"\n',
-                        '#include "wavenet.h"\n',
-                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
-                    )
-                    + s_lap
-                    + (
-                        f'const float HEAD_SCALE = {config["head_scale"]};\n',
-                        "const bool WITH_HEAD = false;\n",
-                    )
-                    + s_parametric
-                    + (
-                        "std::vector<float> PARAMS{"
-                        + ", ".join([f"{w:.16f}f" for w in _c["weights"]])
-                        + "};\n",
-                    )
-                )
-
-    def _export_config(self):
-        return self._net.export_config()
-
-    def _export_cpp_header_parametric(self, config):
-        if config is not None:
-            raise ValueError("Got non-None parametric config")
-        return ("nlohmann::json PARAMETRIC {};\n",)
-
-    def _export_weights(self) -> np.ndarray:
-        return self._net.export_weights()
-
-    def _forward(self, x):
-        if x.ndim == 2:
-            x = x[:, None, :]
-        y = self._net(x)
-        assert y.shape[1] == 1
-        return y[:, 0, :]
+# File: wavenet.py
+# Created Date: Friday July 29th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+WaveNet implementation
+https://arxiv.org/abs/1609.03499
+"""
+
+import json
+from copy import deepcopy
+from pathlib import Path
+from tempfile import TemporaryDirectory
+from typing import Dict, Optional, Sequence, Tuple
+
+import numpy as np
+import torch
+import torch.nn as nn
+
+from ._activations import get_activation
+from ._base import BaseNet
+from ._names import ACTIVATION_NAME, CONV_NAME
+
+
+class Conv1d(nn.Conv1d):
+    def export_weights(self) -> torch.Tensor:
+        tensors = []
+        if self.weight is not None:
+            tensors.append(self.weight.data.flatten())
+        if self.bias is not None:
+            tensors.append(self.bias.data.flatten())
+        if len(tensors) == 0:
+            return torch.zeros((0,))
+        else:
+            return torch.cat(tensors)
+
+
+class _Layer(nn.Module):
+    def __init__(
+        self,
+        condition_size: int,
+        channels: int,
+        kernel_size: int,
+        dilation: int,
+        activation: str,
+        gated: bool,
+    ):
+        super().__init__()
+        # Input mixer takes care of the bias
+        mid_channels = 2 * channels if gated else channels
+        self._conv = Conv1d(channels, mid_channels, kernel_size, dilation=dilation)
+        # Custom init: favors direct input-output
+        # self._conv.weight.data.zero_()
+        self._input_mixer = Conv1d(condition_size, mid_channels, 1, bias=False)
+        self._activation = get_activation(activation)
+        self._activation_name = activation
+        self._1x1 = Conv1d(channels, channels, 1)
+        self._gated = gated
+
+    @property
+    def activation_name(self) -> str:
+        return self._activation_name
+
+    @property
+    def conv(self) -> Conv1d:
+        return self._conv
+
+    @property
+    def gated(self) -> bool:
+        return self._gated
+
+    @property
+    def kernel_size(self) -> int:
+        return self._conv.kernel_size[0]
+
+    def export_weights(self) -> torch.Tensor:
+        return torch.cat(
+            [
+                self.conv.export_weights(),
+                self._input_mixer.export_weights(),
+                self._1x1.export_weights(),
+            ]
+        )
+
+    def forward(
+        self, x: torch.Tensor, h: Optional[torch.Tensor], out_length: int
+    ) -> Tuple[Optional[torch.Tensor], torch.Tensor]:
+        """
+        :param x: (B,C,L1) From last layer
+        :param h: (B,DX,L2) Conditioning. If first, ignored.
+
+        :return:
+            If not final:
+                (B,C,L1-d) to next layer
+                (B,C,L1-d) to mixer
+            If final, next layer is None
+        """
+        zconv = self.conv(x)
+        z1 = zconv + self._input_mixer(h)[:, :, -zconv.shape[2] :]
+        post_activation = (
+            self._activation(z1)
+            if not self._gated
+            else (
+                self._activation(z1[:, : self._channels])
+                * torch.sigmoid(z1[:, self._channels :])
+            )
+        )
+        return (
+            x[:, :, -post_activation.shape[2] :] + self._1x1(post_activation),
+            post_activation[:, :, -out_length:],
+        )
+
+    @property
+    def _channels(self) -> int:
+        return self._1x1.in_channels
+
+
+class _Layers(nn.Module):
+    """
+    Takes in the input and condition (and maybe the head input so far); outputs the
+    layer output and head input.
+
+    The original WaveNet only uses one of these, but you can stack multiple of this
+    module to vary the channels throughout with minimal extra channel-changing conv
+    layers.
+    """
+
+    def __init__(
+        self,
+        input_size: int,
+        condition_size: int,
+        head_size,
+        channels: int,
+        kernel_size: int,
+        dilations: Sequence[int],
+        activation: str = "Tanh",
+        gated: bool = True,
+        head_bias: bool = True,
+    ):
+        super().__init__()
+        self._rechannel = Conv1d(input_size, channels, 1, bias=False)
+        self._layers = nn.ModuleList(
+            [
+                _Layer(
+                    condition_size, channels, kernel_size, dilation, activation, gated
+                )
+                for dilation in dilations
+            ]
+        )
+        # Convert the head input from channels to head_size
+        self._head_rechannel = Conv1d(channels, head_size, 1, bias=head_bias)
+
+        self._config = {
+            "input_size": input_size,
+            "condition_size": condition_size,
+            "head_size": head_size,
+            "channels": channels,
+            "kernel_size": kernel_size,
+            "dilations": dilations,
+            "activation": activation,
+            "gated": gated,
+            "head_bias": head_bias,
+        }
+
+    @property
+    def receptive_field(self) -> int:
+        return 1 + (self._kernel_size - 1) * sum(self._dilations)
+
+    def export_config(self):
+        return deepcopy(self._config)
+
+    def export_weights(self) -> torch.Tensor:
+        return torch.cat(
+            [self._rechannel.export_weights()]
+            + [layer.export_weights() for layer in self._layers]
+            + [self._head_rechannel.export_weights()]
+        )
+
+    def forward(
+        self,
+        x: torch.Tensor,
+        c: torch.Tensor,
+        head_input: Optional[torch.Tensor] = None,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        :param x: (B,Dx,L) layer input
+        :param c: (B,Dc,L) condition
+
+        :return:
+            (B,Dc,L-R+1) head input
+            (B,Dc,L-R+1) layer output
+        """
+        out_length = x.shape[2] - (self.receptive_field - 1)
+        x = self._rechannel(x)
+        for layer in self._layers:
+            x, head_term = layer(x, c, out_length)  # Ensures head_term sample length
+            head_input = (
+                head_term
+                if head_input is None
+                else head_input[:, :, -out_length:] + head_term
+            )
+        return self._head_rechannel(head_input), x
+
+    @property
+    def _dilations(self) -> Sequence[int]:
+        return self._config["dilations"]
+
+    @property
+    def _kernel_size(self) -> int:
+        return self._layers[0].kernel_size
+
+
+class _Head(nn.Module):
+    def __init__(
+        self,
+        in_channels: int,
+        channels: int,
+        activation: str,
+        num_layers: int,
+        out_channels: int,
+    ):
+        super().__init__()
+
+        def block(cx, cy):
+            net = nn.Sequential()
+            net.add_module(ACTIVATION_NAME, get_activation(activation))
+            net.add_module(CONV_NAME, Conv1d(cx, cy, 1))
+            return net
+
+        assert num_layers > 0
+
+        layers = nn.Sequential()
+        cin = in_channels
+        for i in range(num_layers):
+            layers.add_module(
+                f"layer_{i}",
+                block(cin, channels if i != num_layers - 1 else out_channels),
+            )
+            cin = channels
+        self._layers = layers
+
+        self._config = {
+            "channels": channels,
+            "activation": activation,
+            "num_layers": num_layers,
+            "out_channels": out_channels,
+        }
+
+    def export_config(self):
+        return deepcopy(self._config)
+
+    def export_weights(self) -> torch.Tensor:
+        return torch.cat([layer[1].export_weights() for layer in self._layers])
+
+    def forward(self, *args, **kwargs):
+        return self._layers(*args, **kwargs)
+
+
+class _WaveNet(nn.Module):
+    def __init__(
+        self,
+        layers_configs: Sequence[Dict],
+        head_config: Optional[Dict] = None,
+        head_scale: float = 1.0,
+    ):
+        super().__init__()
+
+        self._layers = nn.ModuleList([_Layers(**lc) for lc in layers_configs])
+        self._head = None if head_config is None else _Head(**head_config)
+        self._head_scale = head_scale
+
+    @property
+    def receptive_field(self) -> int:
+        return 1 + sum([(layer.receptive_field - 1) for layer in self._layers])
+
+    def export_config(self):
+        return {
+            "layers": [layers.export_config() for layers in self._layers],
+            "head": None if self._head is None else self._head.export_config(),
+            "head_scale": self._head_scale,
+        }
+
+    def export_weights(self) -> np.ndarray:
+        """
+        :return: 1D array
+        """
+        weights = torch.cat([layer.export_weights() for layer in self._layers])
+        if self._head is not None:
+            weights = torch.cat([weights, self._head.export_weights()])
+        weights = torch.cat([weights, torch.Tensor([self._head_scale])])
+        return weights.detach().cpu().numpy()
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        :param x: (B,Cx,L)
+        :return: (B,Cy,L-R)
+        """
+        y, head_input = x, None
+        for layer in self._layers:
+            head_input, y = layer(y, x, head_input=head_input)
+        head_input = self._head_scale * head_input
+        return head_input if self._head is None else self._head(head_input)
+
+
+class WaveNet(BaseNet):
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        self._net = _WaveNet(*args, **kwargs)
+
+    @property
+    def pad_start_default(self) -> bool:
+        return True
+
+    @property
+    def receptive_field(self) -> int:
+        return self._net.receptive_field
+
+    def export_cpp_header(self, filename: Path):
+        with TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir)
+            WaveNet.export(self, Path(tmpdir))  # Hacky...need to work w/ CatWaveNet
+            with open(Path(tmpdir, "model.nam"), "r") as fp:
+                _c = json.load(fp)
+            version = _c["version"]
+            config = _c["config"]
+
+            if config["head"] is not None:
+                raise NotImplementedError("No heads yet")
+            # head_scale
+            # with_head
+            # parametric
+
+            # String for layer array params:
+            s_lap = (
+                "const std::vector<wavenet::LayerArrayParams> LAYER_ARRAY_PARAMS{\n",
+            )
+            for i, lc in enumerate(config["layers"], 1):
+                s_lap_line = (
+                    f'  wavenet::LayerArrayParams({lc["input_size"]}, '
+                    f'{lc["condition_size"]}, {lc["head_size"]}, {lc["channels"]}, '
+                    f'{lc["kernel_size"]}, std::vector<int> '
+                    "{"
+                    + ", ".join([str(d) for d in lc["dilations"]])
+                    + "}, "
+                    + (
+                        f'"{lc["activation"]}", {str(lc["gated"]).lower()}, '
+                        f'{str(lc["head_bias"]).lower()})'
+                    )
+                )
+                if i < len(config["layers"]):
+                    s_lap_line += ","
+                s_lap_line += "\n"
+                s_lap += (s_lap_line,)
+            s_lap += ("};\n",)
+            s_parametric = self._export_cpp_header_parametric(config.get("parametric"))
+            with open(filename, "w") as f:
+                f.writelines(
+                    (
+                        "#pragma once\n",
+                        "// Automatically-generated model file\n",
+                        "#include <vector>\n",
+                        '#include "json.hpp"\n',
+                        '#include "wavenet.h"\n',
+                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
+                    )
+                    + s_lap
+                    + (
+                        f'const float HEAD_SCALE = {config["head_scale"]};\n',
+                        "const bool WITH_HEAD = false;\n",
+                    )
+                    + s_parametric
+                    + (
+                        "std::vector<float> PARAMS{"
+                        + ", ".join([f"{w:.16f}f" for w in _c["weights"]])
+                        + "};\n",
+                    )
+                )
+
+    def _export_config(self):
+        return self._net.export_config()
+
+    def _export_cpp_header_parametric(self, config):
+        if config is not None:
+            raise ValueError("Got non-None parametric config")
+        return ("nlohmann::json PARAMETRIC {};\n",)
+
+    def _export_weights(self) -> np.ndarray:
+        return self._net.export_weights()
+
+    def _forward(self, x):
+        if x.ndim == 2:
+            x = x[:, None, :]
+        y = self._net(x)
+        assert y.shape[1] == 1
+        return y[:, 0, :]
```

### Comparing `neural-amp-modeler-0.5.1/nam/train/colab.py` & `neural-amp-modeler-0.5.2/nam/train/colab.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-# File: colab.py
-# Created Date: Sunday December 4th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Hide the mess in Colab to make things look pretty for users.
-"""
-
-
-from pathlib import Path
-from typing import Optional, Tuple
-
-from ..models.metadata import UserMetadata
-from ._version import Version
-from .core import train
-
-
-_INPUT_BASENAMES = ((Version(1, 1, 1), "v1_1_1.wav"), (Version(1, 0, 0), "v1.wav"))
-_BUGGY_INPUT_BASENAMES = {
-    # 1.1.0 has the spikes at the wrong spots.
-    "v1_1_0.wav"
-}
-_OUTPUT_BASENAME = "output.wav"
-_TRAIN_PATH = "."
-
-
-def _check_for_files() -> Tuple[Version, str]:
-    print("Checking that we have all of the required audio files...")
-    for name in _BUGGY_INPUT_BASENAMES:
-        if Path(name).exists():
-            raise RuntimeError(
-                f"Detected input signal {name} that has known bugs. Please download the latest input signal, {_INPUT_BASENAMES[0][1]}"
-            )
-    for i, (input_version, input_basename) in enumerate(_INPUT_BASENAMES):
-        if Path(input_basename).exists():
-            if i > 0:
-                print(
-                    f"WARNING: Using out-of-date input file {input_basename}. "
-                    "Recommend downloading and using the latest version."
-                )
-            break
-    else:
-        raise FileNotFoundError(
-            f"Didn't find NAM's input audio file. Please upload {_INPUT_BASENAMES[0][1]}"
-        )
-    if not Path(_OUTPUT_BASENAME).exists():
-        raise FileNotFoundError(
-            f"Didn't find your reamped output audio file. Please upload {_OUTPUT_BASENAME}."
-        )
-    return input_version, input_basename
-
-
-def _get_valid_export_directory():
-    def get_path(version):
-        return Path("exported_models", f"version_{version}")
-
-    version = 0
-    while get_path(version).exists():
-        version += 1
-    return get_path(version)
-
-
-def run(
-    epochs: int = 100,
-    delay: Optional[int] = None,
-    architecture: str = "standard",
-    lr: float = 0.004,
-    lr_decay: float = 0.007,
-    seed: Optional[int] = 0,
-    user_metadata: Optional[UserMetadata] = None,
-):
-    """
-    :param epochs: How amny epochs we'll train for.
-    :param delay: How far the output algs the input due to round-trip latency during
-        reamping, in samples.
-    :param stage_1_channels: The number of channels in the WaveNet's first stage.
-    :param stage_2_channels: The number of channels in the WaveNet's second stage.
-    :param lr: The initial learning rate
-    :param lr_decay: The amount by which the learning rate decays each epoch
-    :param seed: RNG seed for reproducibility.
-    """
-
-    input_version, input_basename = _check_for_files()
-
-    model = train(
-        input_basename,
-        _OUTPUT_BASENAME,
-        _TRAIN_PATH,
-        input_version=input_version,
-        epochs=epochs,
-        delay=delay,
-        architecture=architecture,
-        lr=lr,
-        lr_decay=lr_decay,
-        seed=seed,
-    )
-
-    print("Exporting your model...")
-    model_export_outdir = _get_valid_export_directory()
-    model_export_outdir.mkdir(parents=True, exist_ok=False)
-    model.net.export(model_export_outdir, user_metadata=user_metadata)
-    print(f"Model exported to {model_export_outdir}. Enjoy!")
+# File: colab.py
+# Created Date: Sunday December 4th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Hide the mess in Colab to make things look pretty for users.
+"""
+
+
+from pathlib import Path
+from typing import Optional, Tuple
+
+from ..models.metadata import UserMetadata
+from ._version import Version
+from .core import train
+
+
+_INPUT_BASENAMES = ((Version(1, 1, 1), "v1_1_1.wav"), (Version(1, 0, 0), "v1.wav"))
+_BUGGY_INPUT_BASENAMES = {
+    # 1.1.0 has the spikes at the wrong spots.
+    "v1_1_0.wav"
+}
+_OUTPUT_BASENAME = "output.wav"
+_TRAIN_PATH = "."
+
+
+def _check_for_files() -> Tuple[Version, str]:
+    print("Checking that we have all of the required audio files...")
+    for name in _BUGGY_INPUT_BASENAMES:
+        if Path(name).exists():
+            raise RuntimeError(
+                f"Detected input signal {name} that has known bugs. Please download the latest input signal, {_INPUT_BASENAMES[0][1]}"
+            )
+    for i, (input_version, input_basename) in enumerate(_INPUT_BASENAMES):
+        if Path(input_basename).exists():
+            if i > 0:
+                print(
+                    f"WARNING: Using out-of-date input file {input_basename}. "
+                    "Recommend downloading and using the latest version."
+                )
+            break
+    else:
+        raise FileNotFoundError(
+            f"Didn't find NAM's input audio file. Please upload {_INPUT_BASENAMES[0][1]}"
+        )
+    if not Path(_OUTPUT_BASENAME).exists():
+        raise FileNotFoundError(
+            f"Didn't find your reamped output audio file. Please upload {_OUTPUT_BASENAME}."
+        )
+    return input_version, input_basename
+
+
+def _get_valid_export_directory():
+    def get_path(version):
+        return Path("exported_models", f"version_{version}")
+
+    version = 0
+    while get_path(version).exists():
+        version += 1
+    return get_path(version)
+
+
+def run(
+    epochs: int = 100,
+    delay: Optional[int] = None,
+    architecture: str = "standard",
+    lr: float = 0.004,
+    lr_decay: float = 0.007,
+    seed: Optional[int] = 0,
+    user_metadata: Optional[UserMetadata] = None,
+):
+    """
+    :param epochs: How amny epochs we'll train for.
+    :param delay: How far the output algs the input due to round-trip latency during
+        reamping, in samples.
+    :param stage_1_channels: The number of channels in the WaveNet's first stage.
+    :param stage_2_channels: The number of channels in the WaveNet's second stage.
+    :param lr: The initial learning rate
+    :param lr_decay: The amount by which the learning rate decays each epoch
+    :param seed: RNG seed for reproducibility.
+    """
+
+    input_version, input_basename = _check_for_files()
+
+    model = train(
+        input_basename,
+        _OUTPUT_BASENAME,
+        _TRAIN_PATH,
+        input_version=input_version,
+        epochs=epochs,
+        delay=delay,
+        architecture=architecture,
+        lr=lr,
+        lr_decay=lr_decay,
+        seed=seed,
+    )
+
+    print("Exporting your model...")
+    model_export_outdir = _get_valid_export_directory()
+    model_export_outdir.mkdir(parents=True, exist_ok=False)
+    model.net.export(model_export_outdir, user_metadata=user_metadata)
+    print(f"Model exported to {model_export_outdir}. Enjoy!")
```

### Comparing `neural-amp-modeler-0.5.1/nam/train/core.py` & `neural-amp-modeler-0.5.2/nam/train/core.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,435 +1,435 @@
-# File: core.py
-# Created Date: Tuesday December 20th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Functions used by the GUI trainer.
-"""
-
-import hashlib
-from enum import Enum
-from time import time
-from typing import Optional, Union
-
-import matplotlib.pyplot as plt
-import numpy as np
-import pytorch_lightning as pl
-import torch
-from torch.utils.data import DataLoader
-
-from ..data import REQUIRED_RATE, Split, init_dataset, wav_to_np
-from ..models import Model
-from ._version import Version
-
-
-class Architecture(Enum):
-    STANDARD = "standard"
-    LITE = "lite"
-    FEATHER = "feather"
-
-
-def _detect_input_version(input_path) -> Version:
-    """
-    Check to see if the input matches any of the known inputs
-    """
-    md5 = hashlib.md5()
-    buffer_size = 65536
-    with open(input_path, "rb") as f:
-        while True:
-            data = f.read(buffer_size)
-            if not data:
-                break
-            md5.update(data)
-    file_hash = md5.hexdigest()
-
-    version = {
-        "4d54a958861bf720ec4637f43d44a7ef": Version(1, 0, 0),
-        "7c3b6119c74465f79d96c761a0e27370": Version(1, 1, 1),
-    }.get(file_hash)
-    if version is None:
-        raise RuntimeError(
-            f"Provided input file {input_path} does not match any known standard input "
-            "files."
-        )
-    return version
-
-
-_V1_BLIP_LOCATIONS = 12_000, 36_000
-
-
-def _calibrate_delay_v1(input_path, output_path) -> int:
-    lookahead = 1_000
-    lookback = 10_000
-    safety_factor = 4
-
-    # Calibrate the trigger:
-    y = wav_to_np(output_path)[:48_000]
-    background_level = np.max(np.abs(y[:6_000]))
-    trigger_threshold = max(background_level + 0.01, 1.01 * background_level)
-
-    delays = []
-    for blip_index, i in enumerate(_V1_BLIP_LOCATIONS, 1):
-
-        start_looking = i - lookahead
-        stop_looking = i + lookback
-        y_scan = y[start_looking:stop_looking]
-        triggered = np.where(np.abs(y_scan) > trigger_threshold)[0]
-        if len(triggered) == 0:
-            msg = (
-                f"No response activated the trigger in response to blip "
-                f"{blip_index}. Is something wrong with the reamp?"
-            )
-            print(msg)
-            print("SHARE THIS PLOT IF YOU ASK FOR HELP")
-            plt.figure()
-            plt.plot(np.arange(-lookahead, lookback), y_scan, label="Signal")
-            plt.axvline(x=0, color="C1", linestyle="--", label="Trigger")
-            plt.axhline(
-                y=-trigger_threshold, color="k", linestyle="--", label="Threshold"
-            )
-            plt.axhline(y=trigger_threshold, color="k", linestyle="--")
-            plt.xlim((-lookahead, lookback))
-            plt.xlabel("Samples")
-            plt.ylabel("Response")
-            plt.legend()
-            plt.show()
-            raise RuntimeError(msg)
-        else:
-            j = triggered[0]
-            delays.append(j + start_looking - i)
-
-    print("Delays:")
-    for d in delays:
-        print(f" {d}")
-    delay = int(np.min(delays)) - safety_factor
-    print(f"After aplying safety factor, final delay is {delay}")
-    return delay
-
-
-def _plot_delay_v1(delay: int, input_path: str, output_path: str, _nofail=True):
-    print("Plotting the delay for manual inspection...")
-    x = wav_to_np(input_path)[:48_000]
-    y = wav_to_np(output_path)[:48_000]
-    i = np.where(np.abs(x) > 0.5 * np.abs(x).max())[0]  # In case resampled poorly
-    if len(i) == 0:
-        print("Failed to find the spike in the input file.")
-        print(
-            "Plotting the input and output; there should be spikes at around the "
-            "marked locations."
-        )
-        expected_spikes = 12_000, 36_000  # For v1 specifically
-        fig, axs = plt.subplots(2, 1)
-        for ax, curve in zip(axs, (x, y)):
-            ax.plot(curve)
-            [ax.axvline(x=es, color="C1", linestyle="--") for es in expected_spikes]
-        plt.show()
-        if _nofail:
-            raise RuntimeError("Failed to plot delay")
-    else:
-        i = i[0]
-        di = 20
-        plt.figure()
-        # plt.plot(x[i - di : i + di], ".-", label="Input")
-        plt.plot(
-            np.arange(-di, di),
-            y[i - di + delay : i + di + delay],
-            ".-",
-            label="Output",
-        )
-        plt.axvline(x=0, linestyle="--", color="C1")
-        plt.legend()
-        plt.show()  # This doesn't freeze the notebook
-
-
-def _calibrate_delay(
-    delay: Optional[int],
-    input_version: Version,
-    input_path: str,
-    output_path: str,
-    silent: bool=False
-) -> int:
-    if input_version.major == 1:
-        calibrate, plot = _calibrate_delay_v1, _plot_delay_v1
-    else:
-        raise NotImplementedError(
-            f"Input calibration not implemented for input version {input_version}"
-        )
-    if delay is not None:
-        print(f"Delay is specified as {delay}")
-    else:
-        print("Delay wasn't provided; attempting to calibrate automatically...")
-        delay = calibrate(input_path, output_path)
-    if not silent:
-        plot(delay, input_path, output_path)
-    return delay
-
-
-def _get_wavenet_config(architecture):
-    return {
-        Architecture.STANDARD: {
-            "layers_configs": [
-                {
-                    "input_size": 1,
-                    "condition_size": 1,
-                    "channels": 16,
-                    "head_size": 8,
-                    "kernel_size": 3,
-                    "dilations": [1, 2, 4, 8, 16, 32, 64, 128, 256, 512],
-                    "activation": "Tanh",
-                    "gated": False,
-                    "head_bias": False,
-                },
-                {
-                    "condition_size": 1,
-                    "input_size": 16,
-                    "channels": 8,
-                    "head_size": 1,
-                    "kernel_size": 3,
-                    "dilations": [1, 2, 4, 8, 16, 32, 64, 128, 256, 512],
-                    "activation": "Tanh",
-                    "gated": False,
-                    "head_bias": True,
-                },
-            ],
-            "head_scale": 0.02,
-        },
-        Architecture.LITE: {
-            "layers_configs": [
-                {
-                    "input_size": 1,
-                    "condition_size": 1,
-                    "channels": 12,
-                    "head_size": 6,
-                    "kernel_size": 3,
-                    "dilations": [1, 2, 4, 8, 16, 32, 64],
-                    "activation": "Tanh",
-                    "gated": False,
-                    "head_bias": False,
-                },
-                {
-                    "condition_size": 1,
-                    "input_size": 12,
-                    "channels": 6,
-                    "head_size": 1,
-                    "kernel_size": 3,
-                    "dilations": [128, 256, 512, 1, 2, 4, 8, 16, 32, 64, 128, 256, 512],
-                    "activation": "Tanh",
-                    "gated": False,
-                    "head_bias": True,
-                },
-            ],
-            "head_scale": 0.02,
-        },
-        Architecture.FEATHER: {
-            "layers_configs": [
-                {
-                    "input_size": 1,
-                    "condition_size": 1,
-                    "channels": 8,
-                    "head_size": 4,
-                    "kernel_size": 3,
-                    "dilations": [1, 2, 4, 8, 16, 32, 64],
-                    "activation": "Tanh",
-                    "gated": False,
-                    "head_bias": False,
-                },
-                {
-                    "condition_size": 1,
-                    "input_size": 8,
-                    "channels": 4,
-                    "head_size": 1,
-                    "kernel_size": 3,
-                    "dilations": [128, 256, 512, 1, 2, 4, 8, 16, 32, 64, 128, 256, 512],
-                    "activation": "Tanh",
-                    "gated": False,
-                    "head_bias": True,
-                },
-            ],
-            "head_scale": 0.02,
-        },
-    }[architecture]
-
-
-def _get_configs(
-    input_basename: str,
-    output_basename: str,
-    delay: int,
-    epochs: int,
-    architecture: Architecture,
-    lr: float,
-    lr_decay: float,
-):
-    val_seconds = 9
-    train_val_split = -val_seconds * REQUIRED_RATE
-    data_config = {
-        "train": {"ny": 8192, "stop": train_val_split},
-        "validation": {"ny": None, "start": train_val_split},
-        "common": {
-            "x_path": input_basename,
-            "y_path": output_basename,
-            "delay": delay,
-        },
-    }
-    model_config = {
-        "net": {
-            "name": "WaveNet",
-            # This should do decently. If you really want a nice model, try turning up
-            # "channels" in the first block and "input_size" in the second from 12 to 16.
-            "config": _get_wavenet_config(architecture),
-        },
-        "loss": {"val_loss": "esr"},
-        "optimizer": {"lr": lr},
-        "lr_scheduler": {"class": "ExponentialLR", "kwargs": {"gamma": 1.0 - lr_decay}},
-    }
-    if torch.cuda.is_available():
-        device_config = {"accelerator": "gpu", "devices": 1}
-    elif torch.backends.mps.is_available():
-        device_config = {"accelerator": "mps", "devices": 1}
-    else:
-        print("WARNING: No GPU was found. Training will be very slow!")
-        device_config = {}
-    learning_config = {
-        "train_dataloader": {
-            "batch_size": 16,
-            "shuffle": True,
-            "pin_memory": True,
-            "drop_last": True,
-            "num_workers": 0,
-        },
-        "val_dataloader": {},
-        "trainer": {"max_epochs": epochs, **device_config},
-    }
-    return data_config, model_config, learning_config
-
-
-def _esr(pred: torch.Tensor, target: torch.Tensor) -> float:
-    return (
-        torch.mean(torch.square(pred - target)).item()
-        / torch.mean(torch.square(target)).item()
-    )
-
-
-def _plot(
-        model,
-        ds,
-        window_start: Optional[int] = None,
-        window_end: Optional[int] = None,
-        filepath: Optional[str] = None,
-        silent: bool = False
-):
-    print("Plotting a comparison of your model with the target output...")
-    with torch.no_grad():
-        tx = len(ds.x) / 48_000
-        print(f"Run (t={tx:.2f} sec)")
-        t0 = time()
-        output = model(ds.x).flatten().cpu().numpy()
-        t1 = time()
-        print(f"Took {t1 - t0:.2f} sec ({tx / (t1 - t0):.2f}x)")
-
-    esr = _esr(torch.Tensor(output), ds.y)
-    # Trying my best to put numbers to it...
-    if esr < 0.01:
-        esr_comment = "Great!"
-    elif esr < 0.035:
-        esr_comment = "Not bad!"
-    elif esr < 0.1:
-        esr_comment = "...This *might* sound ok!"
-    elif esr < 0.3:
-        esr_comment = "...This probably won't sound great :("
-    else:
-        esr_comment = "...Something seems to have gone wrong."
-    print(f"Error-signal ratio = {esr:.4f}")
-    print(esr_comment)
-
-    plt.figure(figsize=(16, 5))
-    plt.plot(output[window_start:window_end], label="Prediction")
-    plt.plot(ds.y[window_start:window_end], linestyle="--", label="Target")
-    plt.title(f"ESR={esr:.4f}")
-    plt.legend()
-    if filepath is not None:
-        plt.savefig(filepath + ".png")
-    if not silent:
-        plt.show()
-
-def train(
-    input_path: str,
-    output_path: str,
-    train_path: str,
-    input_version: Optional[Version] = None,
-    epochs=100,
-    delay=None,
-    architecture: Union[Architecture, str] = Architecture.STANDARD,
-    lr=0.004,
-    lr_decay=0.007,
-    seed: Optional[int] = 0,
-    save_plot: bool=False,
-    silent: bool=False,
-    modelname: str="model"
-):
-    if seed is not None:
-        torch.manual_seed(seed)
-
-    # This needs more thought...
-    # 1. Does the user want me to calibrate the delay?
-    # 2. Does the user want to see what the chosen (by them or me) delay looks like?
-    if delay is None:
-        if input_version is None:
-            input_version = _detect_input_version(input_path)
-        delay = _calibrate_delay(delay, input_version, input_path, output_path, silent=silent)
-    else:
-        print(f"Delay provided as {delay}; skip calibration")
-
-    data_config, model_config, learning_config = _get_configs(
-        input_path,
-        output_path,
-        delay,
-        epochs,
-        Architecture(architecture),
-        lr,
-        lr_decay,
-    )
-
-    print("Starting training. It's time to kick ass and chew bubblegum!")
-    model = Model.init_from_config(model_config)
-    data_config["common"]["nx"] = model.net.receptive_field
-    dataset_train = init_dataset(data_config, Split.TRAIN)
-    dataset_validation = init_dataset(data_config, Split.VALIDATION)
-    train_dataloader = DataLoader(dataset_train, **learning_config["train_dataloader"])
-    val_dataloader = DataLoader(dataset_validation, **learning_config["val_dataloader"])
-
-    trainer = pl.Trainer(
-        callbacks=[
-            pl.callbacks.model_checkpoint.ModelCheckpoint(
-                filename="checkpoint_best_{epoch:04d}_{step}_{ESR:.4f}_{MSE:.3e}",
-                save_top_k=3,
-                monitor="val_loss",
-                every_n_epochs=1,
-            ),
-            pl.callbacks.model_checkpoint.ModelCheckpoint(
-                filename="checkpoint_last_{epoch:04d}_{step}", every_n_epochs=1
-            ),
-        ],
-        default_root_dir=train_path,
-        **learning_config["trainer"],
-    )
-    trainer.fit(model, train_dataloader, val_dataloader)
-
-    # Go to best checkpoint
-    best_checkpoint = trainer.checkpoint_callback.best_model_path
-    if best_checkpoint != "":
-        model = Model.load_from_checkpoint(
-            trainer.checkpoint_callback.best_model_path,
-            **Model.parse_config(model_config),
-        )
-    model.cpu()
-    model.eval()
-
-    _plot(
-        model,
-        dataset_validation,
-        window_start=100_000,  # Start of the plotting window, in samples
-        window_end=101_000,  # End of the plotting window, in samples
-        filepath=train_path +'/'+ modelname if save_plot else None,
-        silent=silent
-    )
-    return model
+# File: core.py
+# Created Date: Tuesday December 20th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Functions used by the GUI trainer.
+"""
+
+import hashlib
+from enum import Enum
+from time import time
+from typing import Optional, Union
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pytorch_lightning as pl
+import torch
+from torch.utils.data import DataLoader
+
+from ..data import REQUIRED_RATE, Split, init_dataset, wav_to_np
+from ..models import Model
+from ._version import Version
+
+
+class Architecture(Enum):
+    STANDARD = "standard"
+    LITE = "lite"
+    FEATHER = "feather"
+
+
+def _detect_input_version(input_path) -> Version:
+    """
+    Check to see if the input matches any of the known inputs
+    """
+    md5 = hashlib.md5()
+    buffer_size = 65536
+    with open(input_path, "rb") as f:
+        while True:
+            data = f.read(buffer_size)
+            if not data:
+                break
+            md5.update(data)
+    file_hash = md5.hexdigest()
+
+    version = {
+        "4d54a958861bf720ec4637f43d44a7ef": Version(1, 0, 0),
+        "7c3b6119c74465f79d96c761a0e27370": Version(1, 1, 1),
+    }.get(file_hash)
+    if version is None:
+        raise RuntimeError(
+            f"Provided input file {input_path} does not match any known standard input "
+            "files."
+        )
+    return version
+
+
+_V1_BLIP_LOCATIONS = 12_000, 36_000
+
+
+def _calibrate_delay_v1(input_path, output_path) -> int:
+    lookahead = 1_000
+    lookback = 10_000
+    safety_factor = 4
+
+    # Calibrate the trigger:
+    y = wav_to_np(output_path)[:48_000]
+    background_level = np.max(np.abs(y[:6_000]))
+    trigger_threshold = max(background_level + 0.01, 1.01 * background_level)
+
+    delays = []
+    for blip_index, i in enumerate(_V1_BLIP_LOCATIONS, 1):
+
+        start_looking = i - lookahead
+        stop_looking = i + lookback
+        y_scan = y[start_looking:stop_looking]
+        triggered = np.where(np.abs(y_scan) > trigger_threshold)[0]
+        if len(triggered) == 0:
+            msg = (
+                f"No response activated the trigger in response to blip "
+                f"{blip_index}. Is something wrong with the reamp?"
+            )
+            print(msg)
+            print("SHARE THIS PLOT IF YOU ASK FOR HELP")
+            plt.figure()
+            plt.plot(np.arange(-lookahead, lookback), y_scan, label="Signal")
+            plt.axvline(x=0, color="C1", linestyle="--", label="Trigger")
+            plt.axhline(
+                y=-trigger_threshold, color="k", linestyle="--", label="Threshold"
+            )
+            plt.axhline(y=trigger_threshold, color="k", linestyle="--")
+            plt.xlim((-lookahead, lookback))
+            plt.xlabel("Samples")
+            plt.ylabel("Response")
+            plt.legend()
+            plt.show()
+            raise RuntimeError(msg)
+        else:
+            j = triggered[0]
+            delays.append(j + start_looking - i)
+
+    print("Delays:")
+    for d in delays:
+        print(f" {d}")
+    delay = int(np.min(delays)) - safety_factor
+    print(f"After aplying safety factor, final delay is {delay}")
+    return delay
+
+
+def _plot_delay_v1(delay: int, input_path: str, output_path: str, _nofail=True):
+    print("Plotting the delay for manual inspection...")
+    x = wav_to_np(input_path)[:48_000]
+    y = wav_to_np(output_path)[:48_000]
+    i = np.where(np.abs(x) > 0.5 * np.abs(x).max())[0]  # In case resampled poorly
+    if len(i) == 0:
+        print("Failed to find the spike in the input file.")
+        print(
+            "Plotting the input and output; there should be spikes at around the "
+            "marked locations."
+        )
+        expected_spikes = 12_000, 36_000  # For v1 specifically
+        fig, axs = plt.subplots(2, 1)
+        for ax, curve in zip(axs, (x, y)):
+            ax.plot(curve)
+            [ax.axvline(x=es, color="C1", linestyle="--") for es in expected_spikes]
+        plt.show()
+        if _nofail:
+            raise RuntimeError("Failed to plot delay")
+    else:
+        i = i[0]
+        di = 20
+        plt.figure()
+        # plt.plot(x[i - di : i + di], ".-", label="Input")
+        plt.plot(
+            np.arange(-di, di),
+            y[i - di + delay : i + di + delay],
+            ".-",
+            label="Output",
+        )
+        plt.axvline(x=0, linestyle="--", color="C1")
+        plt.legend()
+        plt.show()  # This doesn't freeze the notebook
+
+
+def _calibrate_delay(
+    delay: Optional[int],
+    input_version: Version,
+    input_path: str,
+    output_path: str,
+    silent: bool=False
+) -> int:
+    if input_version.major == 1:
+        calibrate, plot = _calibrate_delay_v1, _plot_delay_v1
+    else:
+        raise NotImplementedError(
+            f"Input calibration not implemented for input version {input_version}"
+        )
+    if delay is not None:
+        print(f"Delay is specified as {delay}")
+    else:
+        print("Delay wasn't provided; attempting to calibrate automatically...")
+        delay = calibrate(input_path, output_path)
+    if not silent:
+        plot(delay, input_path, output_path)
+    return delay
+
+
+def _get_wavenet_config(architecture):
+    return {
+        Architecture.STANDARD: {
+            "layers_configs": [
+                {
+                    "input_size": 1,
+                    "condition_size": 1,
+                    "channels": 16,
+                    "head_size": 8,
+                    "kernel_size": 3,
+                    "dilations": [1, 2, 4, 8, 16, 32, 64, 128, 256, 512],
+                    "activation": "Tanh",
+                    "gated": False,
+                    "head_bias": False,
+                },
+                {
+                    "condition_size": 1,
+                    "input_size": 16,
+                    "channels": 8,
+                    "head_size": 1,
+                    "kernel_size": 3,
+                    "dilations": [1, 2, 4, 8, 16, 32, 64, 128, 256, 512],
+                    "activation": "Tanh",
+                    "gated": False,
+                    "head_bias": True,
+                },
+            ],
+            "head_scale": 0.02,
+        },
+        Architecture.LITE: {
+            "layers_configs": [
+                {
+                    "input_size": 1,
+                    "condition_size": 1,
+                    "channels": 12,
+                    "head_size": 6,
+                    "kernel_size": 3,
+                    "dilations": [1, 2, 4, 8, 16, 32, 64],
+                    "activation": "Tanh",
+                    "gated": False,
+                    "head_bias": False,
+                },
+                {
+                    "condition_size": 1,
+                    "input_size": 12,
+                    "channels": 6,
+                    "head_size": 1,
+                    "kernel_size": 3,
+                    "dilations": [128, 256, 512, 1, 2, 4, 8, 16, 32, 64, 128, 256, 512],
+                    "activation": "Tanh",
+                    "gated": False,
+                    "head_bias": True,
+                },
+            ],
+            "head_scale": 0.02,
+        },
+        Architecture.FEATHER: {
+            "layers_configs": [
+                {
+                    "input_size": 1,
+                    "condition_size": 1,
+                    "channels": 8,
+                    "head_size": 4,
+                    "kernel_size": 3,
+                    "dilations": [1, 2, 4, 8, 16, 32, 64],
+                    "activation": "Tanh",
+                    "gated": False,
+                    "head_bias": False,
+                },
+                {
+                    "condition_size": 1,
+                    "input_size": 8,
+                    "channels": 4,
+                    "head_size": 1,
+                    "kernel_size": 3,
+                    "dilations": [128, 256, 512, 1, 2, 4, 8, 16, 32, 64, 128, 256, 512],
+                    "activation": "Tanh",
+                    "gated": False,
+                    "head_bias": True,
+                },
+            ],
+            "head_scale": 0.02,
+        },
+    }[architecture]
+
+
+def _get_configs(
+    input_basename: str,
+    output_basename: str,
+    delay: int,
+    epochs: int,
+    architecture: Architecture,
+    lr: float,
+    lr_decay: float,
+):
+    val_seconds = 9
+    train_val_split = -val_seconds * REQUIRED_RATE
+    data_config = {
+        "train": {"ny": 8192, "stop": train_val_split},
+        "validation": {"ny": None, "start": train_val_split},
+        "common": {
+            "x_path": input_basename,
+            "y_path": output_basename,
+            "delay": delay,
+        },
+    }
+    model_config = {
+        "net": {
+            "name": "WaveNet",
+            # This should do decently. If you really want a nice model, try turning up
+            # "channels" in the first block and "input_size" in the second from 12 to 16.
+            "config": _get_wavenet_config(architecture),
+        },
+        "loss": {"val_loss": "esr"},
+        "optimizer": {"lr": lr},
+        "lr_scheduler": {"class": "ExponentialLR", "kwargs": {"gamma": 1.0 - lr_decay}},
+    }
+    if torch.cuda.is_available():
+        device_config = {"accelerator": "gpu", "devices": 1}
+    elif torch.backends.mps.is_available():
+        device_config = {"accelerator": "mps", "devices": 1}
+    else:
+        print("WARNING: No GPU was found. Training will be very slow!")
+        device_config = {}
+    learning_config = {
+        "train_dataloader": {
+            "batch_size": 16,
+            "shuffle": True,
+            "pin_memory": True,
+            "drop_last": True,
+            "num_workers": 0,
+        },
+        "val_dataloader": {},
+        "trainer": {"max_epochs": epochs, **device_config},
+    }
+    return data_config, model_config, learning_config
+
+
+def _esr(pred: torch.Tensor, target: torch.Tensor) -> float:
+    return (
+        torch.mean(torch.square(pred - target)).item()
+        / torch.mean(torch.square(target)).item()
+    )
+
+
+def _plot(
+        model,
+        ds,
+        window_start: Optional[int] = None,
+        window_end: Optional[int] = None,
+        filepath: Optional[str] = None,
+        silent: bool = False
+):
+    print("Plotting a comparison of your model with the target output...")
+    with torch.no_grad():
+        tx = len(ds.x) / 48_000
+        print(f"Run (t={tx:.2f} sec)")
+        t0 = time()
+        output = model(ds.x).flatten().cpu().numpy()
+        t1 = time()
+        print(f"Took {t1 - t0:.2f} sec ({tx / (t1 - t0):.2f}x)")
+
+    esr = _esr(torch.Tensor(output), ds.y)
+    # Trying my best to put numbers to it...
+    if esr < 0.01:
+        esr_comment = "Great!"
+    elif esr < 0.035:
+        esr_comment = "Not bad!"
+    elif esr < 0.1:
+        esr_comment = "...This *might* sound ok!"
+    elif esr < 0.3:
+        esr_comment = "...This probably won't sound great :("
+    else:
+        esr_comment = "...Something seems to have gone wrong."
+    print(f"Error-signal ratio = {esr:.4f}")
+    print(esr_comment)
+
+    plt.figure(figsize=(16, 5))
+    plt.plot(output[window_start:window_end], label="Prediction")
+    plt.plot(ds.y[window_start:window_end], linestyle="--", label="Target")
+    plt.title(f"ESR={esr:.4f}")
+    plt.legend()
+    if filepath is not None:
+        plt.savefig(filepath + ".png")
+    if not silent:
+        plt.show()
+
+def train(
+    input_path: str,
+    output_path: str,
+    train_path: str,
+    input_version: Optional[Version] = None,
+    epochs=100,
+    delay=None,
+    architecture: Union[Architecture, str] = Architecture.STANDARD,
+    lr=0.004,
+    lr_decay=0.007,
+    seed: Optional[int] = 0,
+    save_plot: bool=False,
+    silent: bool=False,
+    modelname: str="model"
+):
+    if seed is not None:
+        torch.manual_seed(seed)
+
+    # This needs more thought...
+    # 1. Does the user want me to calibrate the delay?
+    # 2. Does the user want to see what the chosen (by them or me) delay looks like?
+    if delay is None:
+        if input_version is None:
+            input_version = _detect_input_version(input_path)
+        delay = _calibrate_delay(delay, input_version, input_path, output_path, silent=silent)
+    else:
+        print(f"Delay provided as {delay}; skip calibration")
+
+    data_config, model_config, learning_config = _get_configs(
+        input_path,
+        output_path,
+        delay,
+        epochs,
+        Architecture(architecture),
+        lr,
+        lr_decay,
+    )
+
+    print("Starting training. It's time to kick ass and chew bubblegum!")
+    model = Model.init_from_config(model_config)
+    data_config["common"]["nx"] = model.net.receptive_field
+    dataset_train = init_dataset(data_config, Split.TRAIN)
+    dataset_validation = init_dataset(data_config, Split.VALIDATION)
+    train_dataloader = DataLoader(dataset_train, **learning_config["train_dataloader"])
+    val_dataloader = DataLoader(dataset_validation, **learning_config["val_dataloader"])
+
+    trainer = pl.Trainer(
+        callbacks=[
+            pl.callbacks.model_checkpoint.ModelCheckpoint(
+                filename="checkpoint_best_{epoch:04d}_{step}_{ESR:.4f}_{MSE:.3e}",
+                save_top_k=3,
+                monitor="val_loss",
+                every_n_epochs=1,
+            ),
+            pl.callbacks.model_checkpoint.ModelCheckpoint(
+                filename="checkpoint_last_{epoch:04d}_{step}", every_n_epochs=1
+            ),
+        ],
+        default_root_dir=train_path,
+        **learning_config["trainer"],
+    )
+    trainer.fit(model, train_dataloader, val_dataloader)
+
+    # Go to best checkpoint
+    best_checkpoint = trainer.checkpoint_callback.best_model_path
+    if best_checkpoint != "":
+        model = Model.load_from_checkpoint(
+            trainer.checkpoint_callback.best_model_path,
+            **Model.parse_config(model_config),
+        )
+    model.cpu()
+    model.eval()
+
+    _plot(
+        model,
+        dataset_validation,
+        window_start=100_000,  # Start of the plotting window, in samples
+        window_end=101_000,  # End of the plotting window, in samples
+        filepath=train_path +'/'+ modelname if save_plot else None,
+        silent=silent
+    )
+    return model
```

### Comparing `neural-amp-modeler-0.5.1/nam/train/gui.py` & `neural-amp-modeler-0.5.2/nam/train/gui.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,664 +1,664 @@
-# File: gui.py
-# Created Date: Saturday February 25th 2023
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-GUI for training
-
-Usage:
->>> from nam.train.gui import run
->>> run()
-"""
-
-
-# Hack to recover graceful shutdowns in Windows.
-# This has to happen ASAP
-# See:
-# https://github.com/sdatkinson/neural-amp-modeler/issues/105
-# https://stackoverflow.com/a/44822794
-def _ensure_graceful_shutdowns():
-    import os
-
-    if os.name == "nt":  # OS is Windows
-        os.environ["FOR_DISABLE_CONSOLE_CTRL_HANDLER"] = "1"
-
-
-_ensure_graceful_shutdowns()
-
-import re
-import tkinter as tk
-from dataclasses import dataclass
-from enum import Enum
-from functools import partial
-from pathlib import Path
-from tkinter import filedialog
-from typing import Callable, Optional, Sequence
-
-try:
-    from nam import __version__
-    from nam.train import core
-    from nam.models.metadata import GearType, UserMetadata, ToneType
-
-    _install_is_valid = True
-except ImportError:
-    _install_is_valid = False
-_BUTTON_WIDTH = 20
-_BUTTON_HEIGHT = 2
-_TEXT_WIDTH = 70
-
-_DEFAULT_NUM_EPOCHS = 100
-_DEFAULT_DELAY = None
-
-_ADVANCED_OPTIONS_LEFT_WIDTH = 12
-_ADVANCED_OPTIONS_RIGHT_WIDTH = 12
-_METADATA_RIGHT_WIDTH = 60
-
-
-@dataclass
-class _AdvancedOptions(object):
-    architecture: core.Architecture
-    num_epochs: int
-    delay: Optional[int]
-
-
-class _PathType(Enum):
-    FILE = "file"
-    DIRECTORY = "directory"
-    MULTIFILE = "multifile"
-
-
-class _PathButton(object):
-    """
-    Button and the path
-    """
-
-    def __init__(
-        self,
-        frame: tk.Frame,
-        button_text: str,
-        info_str: str,
-        path_type: _PathType,
-        hooks: Optional[Sequence[Callable[[], None]]] = None,
-    ):
-        self._button_text = button_text
-        self._info_str = info_str
-        self._path: Optional[Path] = None
-        self._path_type = path_type
-        self._button = tk.Button(
-            frame,
-            text=button_text,
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._set_val,
-        )
-        self._button.pack(side=tk.LEFT)
-        self._label = tk.Label(
-            frame,
-            width=_TEXT_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            bg=None,
-            anchor="w",
-        )
-        self._label.pack(side=tk.RIGHT)
-        self._hooks = hooks
-        self._set_text()
-
-    @property
-    def val(self) -> Optional[Path]:
-        return self._path
-
-    def _set_text(self):
-        if self._path is None:
-            self._label["fg"] = "red"
-            self._label["text"] = self._info_str
-        else:
-            val = self.val
-            val = val[0] if isinstance(val, tuple) and len(val) == 1 else val
-            self._label["fg"] = "black"
-            self._label["text"] = f"{self._button_text.capitalize()} set to {val}"
-
-    def _set_val(self):
-        res = {
-            _PathType.FILE: filedialog.askopenfilename,
-            _PathType.DIRECTORY: filedialog.askdirectory,
-            _PathType.MULTIFILE: filedialog.askopenfilenames,
-        }[self._path_type]()
-        if res != "":
-            self._path = res
-        self._set_text()
-
-        if self._hooks is not None:
-            for h in self._hooks:
-                h()
-
-
-class _GUI(object):
-    def __init__(self):
-        self._root = tk.Tk()
-        self._root.title(f"NAM Trainer - v{__version__}")
-
-        # Buttons for paths:
-        self._frame_input_path = tk.Frame(self._root)
-        self._frame_input_path.pack()
-        self._path_button_input = _PathButton(
-            self._frame_input_path,
-            "Input Audio",
-            "Select input DI file (eg: v1_1_1.wav)",
-            _PathType.FILE,
-            hooks=[self._check_button_states],
-        )
-
-        self._frame_output_path = tk.Frame(self._root)
-        self._frame_output_path.pack()
-        self._path_button_output = _PathButton(
-            self._frame_output_path,
-            "Output Audio",
-            "Select output (reamped) audio - choose multiple files to enable batch training",
-            _PathType.MULTIFILE,
-            hooks=[self._check_button_states],
-        )
-
-        self._frame_train_destination = tk.Frame(self._root)
-        self._frame_train_destination.pack()
-        self._path_button_train_destination = _PathButton(
-            self._frame_train_destination,
-            "Train Destination",
-            "Select training output directory",
-            _PathType.DIRECTORY,
-            hooks=[self._check_button_states],
-        )
-
-        # Metadata
-        self.user_metadata = UserMetadata()
-        self._frame_metadata = tk.Frame(self._root)
-        self._frame_metadata.pack()
-        self._button_metadata = tk.Button(
-            self._frame_metadata,
-            text="Metadata...",
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._open_metadata,
-        )
-        self._button_metadata.pack()
-        self.user_metadata_flag = False
-
-        # This should probably be to the right somewhere
-        self._get_additional_options_frame()
-
-        # Advanced options for training
-        default_architecture = core.Architecture.STANDARD
-        self.advanced_options = _AdvancedOptions(
-            default_architecture, _DEFAULT_NUM_EPOCHS, _DEFAULT_DELAY
-        )
-        # Window to edit them:
-        self._frame_advanced_options = tk.Frame(self._root)
-        self._frame_advanced_options.pack()
-        self._button_advanced_options = tk.Button(
-            self._frame_advanced_options,
-            text="Advanced options...",
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._open_advanced_options,
-        )
-        self._button_advanced_options.pack()
-
-        # Train button
-        self._frame_train = tk.Frame(self._root)
-        self._frame_train.pack()
-        self._button_train = tk.Button(
-            self._frame_train,
-            text="Train",
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._train,
-        )
-        self._button_train.pack()
-
-        self._check_button_states()
-
-    def _get_additional_options_frame(self):
-        # Checkboxes
-        self._frame_silent = tk.Frame(self._root)
-        self._frame_silent.pack(side=tk.LEFT)
-
-        # Silent run (bypass popups)
-        self._silent = tk.BooleanVar()
-        self._chkbox_silent = tk.Checkbutton(
-            self._frame_silent,
-            text="Silent run (suggested for batch training)",
-            variable=self._silent,
-        )
-        self._chkbox_silent.grid(row=1, column=1, sticky="W")
-
-        # Auto save the end plot
-        self._save_plot = tk.BooleanVar()
-        self._save_plot.set(True)  # default this to true
-        self._chkbox_save_plot = tk.Checkbutton(
-            self._frame_silent,
-            text="Save ESR plot automatically",
-            variable=self._save_plot,
-        )
-        self._chkbox_save_plot.grid(row=2, column=1, sticky="W")
-
-    def mainloop(self):
-        self._root.mainloop()
-
-    def _open_advanced_options(self):
-        """
-        Open advanced options
-        """
-        ao = _AdvancedOptionsGUI(self)
-        # I should probably disable the main GUI...
-        ao.mainloop()
-        # ...and then re-enable it once it gets closed.
-
-    def _open_metadata(self):
-        """
-        Open dialog for metadata
-        """
-        mdata = _UserMetadataGUI(self)
-        # I should probably disable the main GUI...
-        mdata.mainloop()
-
-    def _train(self):
-        # Advanced options:
-        num_epochs = self.advanced_options.num_epochs
-        architecture = self.advanced_options.architecture
-        delay = self.advanced_options.delay
-        file_list = self._path_button_output.val
-
-        # Advanced-er options
-        # If you're poking around looking for these, then maybe it's time to learn to
-        # use the command-line scripts ;)
-        lr = 0.004
-        lr_decay = 0.05
-        seed = 0
-
-        # Run it
-        for file in file_list:
-            print("Now training {}".format(file))
-            basename = re.sub(r"\.wav$", "", file.split("/")[-1])
-
-            trained_model = core.train(
-                self._path_button_input.val,
-                file,
-                self._path_button_train_destination.val,
-                epochs=num_epochs,
-                delay=delay,
-                architecture=architecture,
-                lr=lr,
-                lr_decay=lr_decay,
-                seed=seed,
-                silent=self._silent.get(),
-                save_plot=self._save_plot.get(),
-                modelname=basename,
-            )
-            print("Model training complete!")
-            print("Exporting...")
-            outdir = self._path_button_train_destination.val
-            print(f"Exporting trained model to {outdir}...")
-            trained_model.net.export(
-                outdir,
-                basename=basename,
-                user_metadata=self.user_metadata
-                if self.user_metadata_flag
-                else UserMetadata(),
-            )
-            # Metadata was only valid for 1 run, so make sure it's not used again unless
-            # the user re-visits the window and clicks "ok"
-            self.user_metadata_flag = False
-            print("Done!")
-
-    def _check_button_states(self):
-        """
-        Determine if any buttons should be disabled
-        """
-        # Train button is diabled unless all paths are set
-        if any(
-            pb.val is None
-            for pb in (
-                self._path_button_input,
-                self._path_button_output,
-                self._path_button_train_destination,
-            )
-        ):
-            self._button_train["state"] = tk.DISABLED
-            return
-        self._button_train["state"] = tk.NORMAL
-
-
-# some typing functions
-def _non_negative_int(val):
-    val = int(val)
-    if val < 0:
-        val = 0
-    return val
-
-
-def _int_or_null(val):
-    val = val.rstrip()
-    if val == "null":
-        return val
-    return int(val)
-
-
-def _int_or_null_inv(val):
-    return "null" if val is None else str(val)
-
-
-def _rstripped_str(val):
-    return str(val).rstrip()
-
-
-class _LabeledOptionMenu(object):
-    """
-    Label (left) and radio buttons (right)
-    """
-
-    def __init__(
-        self, frame: tk.Frame, label: str, choices: Enum, default: Optional[Enum] = None
-    ):
-        """
-        :param command: Called to propagate option selection. Is provided with the
-            value corresponding to the radio button selected.
-        """
-        self._frame = frame
-        self._choices = choices
-        height = _BUTTON_HEIGHT
-        bg = None
-        fg = "black"
-        self._label = tk.Label(
-            frame,
-            width=_ADVANCED_OPTIONS_LEFT_WIDTH,
-            height=height,
-            fg=fg,
-            bg=bg,
-            anchor="w",
-            text=label,
-        )
-        self._label.pack(side=tk.LEFT)
-
-        frame_menu = tk.Frame(frame)
-        frame_menu.pack(side=tk.RIGHT)
-
-        self._selected_value = None
-        default = (list(choices)[0] if default is None else default).value
-        self._menu = tk.OptionMenu(
-            frame_menu,
-            tk.StringVar(master=frame, value=default, name=label),
-            # default,
-            *[choice.value for choice in choices],  #  if choice.value!=default],
-            command=self._set,
-        )
-        self._menu.config(width=_ADVANCED_OPTIONS_RIGHT_WIDTH)
-        self._menu.pack(side=tk.RIGHT)
-        # Initialize
-        self._set(default)
-
-    def get(self) -> Enum:
-        return self._selected_value
-
-    def _set(self, val: str):
-        """
-        Set the value selected
-        """
-        self._selected_value = self._choices(val)
-
-
-class _LabeledText(object):
-    """
-    Label (left) and text input (right)
-    """
-
-    def __init__(
-        self,
-        frame: tk.Frame,
-        label: str,
-        default=None,
-        type=None,
-        left_width=_ADVANCED_OPTIONS_LEFT_WIDTH,
-        right_width=_ADVANCED_OPTIONS_RIGHT_WIDTH,
-    ):
-        """
-        :param command: Called to propagate option selection. Is provided with the
-            value corresponding to the radio button selected.
-        :param type: If provided, casts value to given type
-        """
-        self._frame = frame
-        label_height = 2
-        text_height = 1
-        self._label = tk.Label(
-            frame,
-            width=left_width,
-            height=label_height,
-            fg="black",
-            bg=None,
-            anchor="w",
-            text=label,
-        )
-        self._label.pack(side=tk.LEFT)
-
-        self._text = tk.Text(
-            frame,
-            width=right_width,
-            height=text_height,
-            fg="black",
-            bg=None,
-        )
-        self._text.pack(side=tk.RIGHT)
-
-        self._type = type
-
-        if default is not None:
-            self._text.insert("1.0", str(default))
-
-    def get(self):
-        try:
-            val = self._text.get("1.0", tk.END)  # Line 1, character zero (wat)
-            if self._type is not None:
-                val = self._type(val)
-            return val
-        except tk.TclError:
-            return None
-
-
-class _AdvancedOptionsGUI(object):
-    """
-    A window to hold advanced options (Architecture and number of epochs)
-    """
-
-    def __init__(self, parent: _GUI):
-        self._parent = parent
-        self._root = tk.Tk()
-        self._root.title("Advanced Options")
-
-        # Architecture: radio buttons
-        self._frame_architecture = tk.Frame(self._root)
-        self._frame_architecture.pack()
-        self._architecture = _LabeledOptionMenu(
-            self._frame_architecture,
-            "Architecture",
-            core.Architecture,
-            default=self._parent.advanced_options.architecture,
-        )
-
-        # Number of epochs: text box
-        self._frame_epochs = tk.Frame(self._root)
-        self._frame_epochs.pack()
-
-        self._epochs = _LabeledText(
-            self._frame_epochs,
-            "Epochs",
-            default=str(self._parent.advanced_options.num_epochs),
-            type=_non_negative_int,
-        )
-
-        # Delay: text box
-        self._frame_delay = tk.Frame(self._root)
-        self._frame_delay.pack()
-
-        self._delay = _LabeledText(
-            self._frame_delay,
-            "Delay",
-            default=_int_or_null_inv(self._parent.advanced_options.delay),
-            type=_int_or_null,
-        )
-
-        # "Ok": apply and destory
-        self._frame_ok = tk.Frame(self._root)
-        self._frame_ok.pack()
-        self._button_ok = tk.Button(
-            self._frame_ok,
-            text="Ok",
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._apply_and_destroy,
-        )
-        self._button_ok.pack()
-
-    def mainloop(self):
-        self._root.mainloop()
-
-    def _apply_and_destroy(self):
-        """
-        Set values to parent and destroy this object
-        """
-        self._parent.advanced_options.architecture = self._architecture.get()
-        epochs = self._epochs.get()
-        if epochs is not None:
-            self._parent.advanced_options.num_epochs = epochs
-        delay = self._delay.get()
-        # Value None is returned as "null" to disambiguate from non-set.
-        if delay is not None:
-            self._parent.advanced_options.delay = None if delay == "null" else delay
-        self._root.destroy()
-
-
-class _UserMetadataGUI(object):
-    # Things that are auto-filled:
-    # Model date
-    # gain
-    def __init__(self, parent: _GUI):
-        self._parent = parent
-        self._root = tk.Tk()
-        self._root.title("Metadata")
-
-        LabeledText = partial(_LabeledText, right_width=_METADATA_RIGHT_WIDTH)
-
-        # Name
-        self._frame_name = tk.Frame(self._root)
-        self._frame_name.pack()
-        self._name = LabeledText(
-            self._frame_name,
-            "NAM name",
-            default=parent.user_metadata.name,
-            type=_rstripped_str,
-        )
-        # Modeled by
-        self._frame_modeled_by = tk.Frame(self._root)
-        self._frame_modeled_by.pack()
-        self._modeled_by = LabeledText(
-            self._frame_modeled_by,
-            "Modeled by",
-            default=parent.user_metadata.modeled_by,
-            type=_rstripped_str,
-        )
-        # Gear make
-        self._frame_gear_make = tk.Frame(self._root)
-        self._frame_gear_make.pack()
-        self._gear_make = LabeledText(
-            self._frame_gear_make,
-            "Gear make",
-            default=parent.user_metadata.gear_make,
-            type=_rstripped_str,
-        )
-        # Gear model
-        self._frame_gear_model = tk.Frame(self._root)
-        self._frame_gear_model.pack()
-        self._gear_model = LabeledText(
-            self._frame_gear_model,
-            "Gear model",
-            default=parent.user_metadata.gear_model,
-            type=_rstripped_str,
-        )
-        # Gear type
-        self._frame_gear_type = tk.Frame(self._root)
-        self._frame_gear_type.pack()
-        self._gear_type = _LabeledOptionMenu(
-            self._frame_gear_type,
-            "Gear type",
-            GearType,
-            default=parent.user_metadata.gear_type,
-        )
-        # Tone type
-        self._frame_tone_type = tk.Frame(self._root)
-        self._frame_tone_type.pack()
-        self._tone_type = _LabeledOptionMenu(
-            self._frame_tone_type,
-            "Tone type",
-            ToneType,
-            default=parent.user_metadata.tone_type,
-        )
-
-        # "Ok": apply and destory
-        self._frame_ok = tk.Frame(self._root)
-        self._frame_ok.pack()
-        self._button_ok = tk.Button(
-            self._frame_ok,
-            text="Ok",
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._apply_and_destroy,
-        )
-        self._button_ok.pack()
-
-    def mainloop(self):
-        self._root.mainloop()
-
-    def _apply_and_destroy(self):
-        """
-        Set values to parent and destroy this object
-        """
-        self._parent.user_metadata.name = self._name.get()
-        self._parent.user_metadata.modeled_by = self._modeled_by.get()
-        self._parent.user_metadata.gear_make = self._gear_make.get()
-        self._parent.user_metadata.gear_model = self._gear_model.get()
-        self._parent.user_metadata.gear_type = self._gear_type.get()
-        self._parent.user_metadata.tone_type = self._tone_type.get()
-        self._parent.user_metadata_flag = True
-
-        self._root.destroy()
-
-
-def _install_error():
-    window = tk.Tk()
-    window.title("ERROR")
-    label = tk.Label(
-        window,
-        width=45,
-        height=2,
-        text="The NAM training software has not been installed correctly.",
-    )
-    label.pack()
-    button = tk.Button(window, width=10, height=2, text="Quit", command=window.destroy)
-    button.pack()
-    window.mainloop()
-
-
-def run():
-    if _install_is_valid:
-        _gui = _GUI()
-        _gui.mainloop()
-    else:
-        _install_error()
-
-
-if __name__ == "__main__":
-    run()
+# File: gui.py
+# Created Date: Saturday February 25th 2023
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+GUI for training
+
+Usage:
+>>> from nam.train.gui import run
+>>> run()
+"""
+
+
+# Hack to recover graceful shutdowns in Windows.
+# This has to happen ASAP
+# See:
+# https://github.com/sdatkinson/neural-amp-modeler/issues/105
+# https://stackoverflow.com/a/44822794
+def _ensure_graceful_shutdowns():
+    import os
+
+    if os.name == "nt":  # OS is Windows
+        os.environ["FOR_DISABLE_CONSOLE_CTRL_HANDLER"] = "1"
+
+
+_ensure_graceful_shutdowns()
+
+import re
+import tkinter as tk
+from dataclasses import dataclass
+from enum import Enum
+from functools import partial
+from pathlib import Path
+from tkinter import filedialog
+from typing import Callable, Optional, Sequence
+
+try:
+    from nam import __version__
+    from nam.train import core
+    from nam.models.metadata import GearType, UserMetadata, ToneType
+
+    _install_is_valid = True
+except ImportError:
+    _install_is_valid = False
+_BUTTON_WIDTH = 20
+_BUTTON_HEIGHT = 2
+_TEXT_WIDTH = 70
+
+_DEFAULT_NUM_EPOCHS = 100
+_DEFAULT_DELAY = None
+
+_ADVANCED_OPTIONS_LEFT_WIDTH = 12
+_ADVANCED_OPTIONS_RIGHT_WIDTH = 12
+_METADATA_RIGHT_WIDTH = 60
+
+
+@dataclass
+class _AdvancedOptions(object):
+    architecture: core.Architecture
+    num_epochs: int
+    delay: Optional[int]
+
+
+class _PathType(Enum):
+    FILE = "file"
+    DIRECTORY = "directory"
+    MULTIFILE = "multifile"
+
+
+class _PathButton(object):
+    """
+    Button and the path
+    """
+
+    def __init__(
+        self,
+        frame: tk.Frame,
+        button_text: str,
+        info_str: str,
+        path_type: _PathType,
+        hooks: Optional[Sequence[Callable[[], None]]] = None,
+    ):
+        self._button_text = button_text
+        self._info_str = info_str
+        self._path: Optional[Path] = None
+        self._path_type = path_type
+        self._button = tk.Button(
+            frame,
+            text=button_text,
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._set_val,
+        )
+        self._button.pack(side=tk.LEFT)
+        self._label = tk.Label(
+            frame,
+            width=_TEXT_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            bg=None,
+            anchor="w",
+        )
+        self._label.pack(side=tk.RIGHT)
+        self._hooks = hooks
+        self._set_text()
+
+    @property
+    def val(self) -> Optional[Path]:
+        return self._path
+
+    def _set_text(self):
+        if self._path is None:
+            self._label["fg"] = "red"
+            self._label["text"] = self._info_str
+        else:
+            val = self.val
+            val = val[0] if isinstance(val, tuple) and len(val) == 1 else val
+            self._label["fg"] = "black"
+            self._label["text"] = f"{self._button_text.capitalize()} set to {val}"
+
+    def _set_val(self):
+        res = {
+            _PathType.FILE: filedialog.askopenfilename,
+            _PathType.DIRECTORY: filedialog.askdirectory,
+            _PathType.MULTIFILE: filedialog.askopenfilenames,
+        }[self._path_type]()
+        if res != "":
+            self._path = res
+        self._set_text()
+
+        if self._hooks is not None:
+            for h in self._hooks:
+                h()
+
+
+class _GUI(object):
+    def __init__(self):
+        self._root = tk.Tk()
+        self._root.title(f"NAM Trainer - v{__version__}")
+
+        # Buttons for paths:
+        self._frame_input_path = tk.Frame(self._root)
+        self._frame_input_path.pack()
+        self._path_button_input = _PathButton(
+            self._frame_input_path,
+            "Input Audio",
+            "Select input DI file (eg: v1_1_1.wav)",
+            _PathType.FILE,
+            hooks=[self._check_button_states],
+        )
+
+        self._frame_output_path = tk.Frame(self._root)
+        self._frame_output_path.pack()
+        self._path_button_output = _PathButton(
+            self._frame_output_path,
+            "Output Audio",
+            "Select output (reamped) audio - choose multiple files to enable batch training",
+            _PathType.MULTIFILE,
+            hooks=[self._check_button_states],
+        )
+
+        self._frame_train_destination = tk.Frame(self._root)
+        self._frame_train_destination.pack()
+        self._path_button_train_destination = _PathButton(
+            self._frame_train_destination,
+            "Train Destination",
+            "Select training output directory",
+            _PathType.DIRECTORY,
+            hooks=[self._check_button_states],
+        )
+
+        # Metadata
+        self.user_metadata = UserMetadata()
+        self._frame_metadata = tk.Frame(self._root)
+        self._frame_metadata.pack()
+        self._button_metadata = tk.Button(
+            self._frame_metadata,
+            text="Metadata...",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._open_metadata,
+        )
+        self._button_metadata.pack()
+        self.user_metadata_flag = False
+
+        # This should probably be to the right somewhere
+        self._get_additional_options_frame()
+
+        # Advanced options for training
+        default_architecture = core.Architecture.STANDARD
+        self.advanced_options = _AdvancedOptions(
+            default_architecture, _DEFAULT_NUM_EPOCHS, _DEFAULT_DELAY
+        )
+        # Window to edit them:
+        self._frame_advanced_options = tk.Frame(self._root)
+        self._frame_advanced_options.pack()
+        self._button_advanced_options = tk.Button(
+            self._frame_advanced_options,
+            text="Advanced options...",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._open_advanced_options,
+        )
+        self._button_advanced_options.pack()
+
+        # Train button
+        self._frame_train = tk.Frame(self._root)
+        self._frame_train.pack()
+        self._button_train = tk.Button(
+            self._frame_train,
+            text="Train",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._train,
+        )
+        self._button_train.pack()
+
+        self._check_button_states()
+
+    def _get_additional_options_frame(self):
+        # Checkboxes
+        self._frame_silent = tk.Frame(self._root)
+        self._frame_silent.pack(side=tk.LEFT)
+
+        # Silent run (bypass popups)
+        self._silent = tk.BooleanVar()
+        self._chkbox_silent = tk.Checkbutton(
+            self._frame_silent,
+            text="Silent run (suggested for batch training)",
+            variable=self._silent,
+        )
+        self._chkbox_silent.grid(row=1, column=1, sticky="W")
+
+        # Auto save the end plot
+        self._save_plot = tk.BooleanVar()
+        self._save_plot.set(True)  # default this to true
+        self._chkbox_save_plot = tk.Checkbutton(
+            self._frame_silent,
+            text="Save ESR plot automatically",
+            variable=self._save_plot,
+        )
+        self._chkbox_save_plot.grid(row=2, column=1, sticky="W")
+
+    def mainloop(self):
+        self._root.mainloop()
+
+    def _open_advanced_options(self):
+        """
+        Open advanced options
+        """
+        ao = _AdvancedOptionsGUI(self)
+        # I should probably disable the main GUI...
+        ao.mainloop()
+        # ...and then re-enable it once it gets closed.
+
+    def _open_metadata(self):
+        """
+        Open dialog for metadata
+        """
+        mdata = _UserMetadataGUI(self)
+        # I should probably disable the main GUI...
+        mdata.mainloop()
+
+    def _train(self):
+        # Advanced options:
+        num_epochs = self.advanced_options.num_epochs
+        architecture = self.advanced_options.architecture
+        delay = self.advanced_options.delay
+        file_list = self._path_button_output.val
+
+        # Advanced-er options
+        # If you're poking around looking for these, then maybe it's time to learn to
+        # use the command-line scripts ;)
+        lr = 0.004
+        lr_decay = 0.007
+        seed = 0
+
+        # Run it
+        for file in file_list:
+            print("Now training {}".format(file))
+            basename = re.sub(r"\.wav$", "", file.split("/")[-1])
+
+            trained_model = core.train(
+                self._path_button_input.val,
+                file,
+                self._path_button_train_destination.val,
+                epochs=num_epochs,
+                delay=delay,
+                architecture=architecture,
+                lr=lr,
+                lr_decay=lr_decay,
+                seed=seed,
+                silent=self._silent.get(),
+                save_plot=self._save_plot.get(),
+                modelname=basename,
+            )
+            print("Model training complete!")
+            print("Exporting...")
+            outdir = self._path_button_train_destination.val
+            print(f"Exporting trained model to {outdir}...")
+            trained_model.net.export(
+                outdir,
+                basename=basename,
+                user_metadata=self.user_metadata
+                if self.user_metadata_flag
+                else UserMetadata(),
+            )
+            # Metadata was only valid for 1 run, so make sure it's not used again unless
+            # the user re-visits the window and clicks "ok"
+            self.user_metadata_flag = False
+            print("Done!")
+
+    def _check_button_states(self):
+        """
+        Determine if any buttons should be disabled
+        """
+        # Train button is diabled unless all paths are set
+        if any(
+            pb.val is None
+            for pb in (
+                self._path_button_input,
+                self._path_button_output,
+                self._path_button_train_destination,
+            )
+        ):
+            self._button_train["state"] = tk.DISABLED
+            return
+        self._button_train["state"] = tk.NORMAL
+
+
+# some typing functions
+def _non_negative_int(val):
+    val = int(val)
+    if val < 0:
+        val = 0
+    return val
+
+
+def _int_or_null(val):
+    val = val.rstrip()
+    if val == "null":
+        return val
+    return int(val)
+
+
+def _int_or_null_inv(val):
+    return "null" if val is None else str(val)
+
+
+def _rstripped_str(val):
+    return str(val).rstrip()
+
+
+class _LabeledOptionMenu(object):
+    """
+    Label (left) and radio buttons (right)
+    """
+
+    def __init__(
+        self, frame: tk.Frame, label: str, choices: Enum, default: Optional[Enum] = None
+    ):
+        """
+        :param command: Called to propagate option selection. Is provided with the
+            value corresponding to the radio button selected.
+        """
+        self._frame = frame
+        self._choices = choices
+        height = _BUTTON_HEIGHT
+        bg = None
+        fg = "black"
+        self._label = tk.Label(
+            frame,
+            width=_ADVANCED_OPTIONS_LEFT_WIDTH,
+            height=height,
+            fg=fg,
+            bg=bg,
+            anchor="w",
+            text=label,
+        )
+        self._label.pack(side=tk.LEFT)
+
+        frame_menu = tk.Frame(frame)
+        frame_menu.pack(side=tk.RIGHT)
+
+        self._selected_value = None
+        default = (list(choices)[0] if default is None else default).value
+        self._menu = tk.OptionMenu(
+            frame_menu,
+            tk.StringVar(master=frame, value=default, name=label),
+            # default,
+            *[choice.value for choice in choices],  #  if choice.value!=default],
+            command=self._set,
+        )
+        self._menu.config(width=_ADVANCED_OPTIONS_RIGHT_WIDTH)
+        self._menu.pack(side=tk.RIGHT)
+        # Initialize
+        self._set(default)
+
+    def get(self) -> Enum:
+        return self._selected_value
+
+    def _set(self, val: str):
+        """
+        Set the value selected
+        """
+        self._selected_value = self._choices(val)
+
+
+class _LabeledText(object):
+    """
+    Label (left) and text input (right)
+    """
+
+    def __init__(
+        self,
+        frame: tk.Frame,
+        label: str,
+        default=None,
+        type=None,
+        left_width=_ADVANCED_OPTIONS_LEFT_WIDTH,
+        right_width=_ADVANCED_OPTIONS_RIGHT_WIDTH,
+    ):
+        """
+        :param command: Called to propagate option selection. Is provided with the
+            value corresponding to the radio button selected.
+        :param type: If provided, casts value to given type
+        """
+        self._frame = frame
+        label_height = 2
+        text_height = 1
+        self._label = tk.Label(
+            frame,
+            width=left_width,
+            height=label_height,
+            fg="black",
+            bg=None,
+            anchor="w",
+            text=label,
+        )
+        self._label.pack(side=tk.LEFT)
+
+        self._text = tk.Text(
+            frame,
+            width=right_width,
+            height=text_height,
+            fg="black",
+            bg=None,
+        )
+        self._text.pack(side=tk.RIGHT)
+
+        self._type = type
+
+        if default is not None:
+            self._text.insert("1.0", str(default))
+
+    def get(self):
+        try:
+            val = self._text.get("1.0", tk.END)  # Line 1, character zero (wat)
+            if self._type is not None:
+                val = self._type(val)
+            return val
+        except tk.TclError:
+            return None
+
+
+class _AdvancedOptionsGUI(object):
+    """
+    A window to hold advanced options (Architecture and number of epochs)
+    """
+
+    def __init__(self, parent: _GUI):
+        self._parent = parent
+        self._root = tk.Tk()
+        self._root.title("Advanced Options")
+
+        # Architecture: radio buttons
+        self._frame_architecture = tk.Frame(self._root)
+        self._frame_architecture.pack()
+        self._architecture = _LabeledOptionMenu(
+            self._frame_architecture,
+            "Architecture",
+            core.Architecture,
+            default=self._parent.advanced_options.architecture,
+        )
+
+        # Number of epochs: text box
+        self._frame_epochs = tk.Frame(self._root)
+        self._frame_epochs.pack()
+
+        self._epochs = _LabeledText(
+            self._frame_epochs,
+            "Epochs",
+            default=str(self._parent.advanced_options.num_epochs),
+            type=_non_negative_int,
+        )
+
+        # Delay: text box
+        self._frame_delay = tk.Frame(self._root)
+        self._frame_delay.pack()
+
+        self._delay = _LabeledText(
+            self._frame_delay,
+            "Delay",
+            default=_int_or_null_inv(self._parent.advanced_options.delay),
+            type=_int_or_null,
+        )
+
+        # "Ok": apply and destory
+        self._frame_ok = tk.Frame(self._root)
+        self._frame_ok.pack()
+        self._button_ok = tk.Button(
+            self._frame_ok,
+            text="Ok",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._apply_and_destroy,
+        )
+        self._button_ok.pack()
+
+    def mainloop(self):
+        self._root.mainloop()
+
+    def _apply_and_destroy(self):
+        """
+        Set values to parent and destroy this object
+        """
+        self._parent.advanced_options.architecture = self._architecture.get()
+        epochs = self._epochs.get()
+        if epochs is not None:
+            self._parent.advanced_options.num_epochs = epochs
+        delay = self._delay.get()
+        # Value None is returned as "null" to disambiguate from non-set.
+        if delay is not None:
+            self._parent.advanced_options.delay = None if delay == "null" else delay
+        self._root.destroy()
+
+
+class _UserMetadataGUI(object):
+    # Things that are auto-filled:
+    # Model date
+    # gain
+    def __init__(self, parent: _GUI):
+        self._parent = parent
+        self._root = tk.Tk()
+        self._root.title("Metadata")
+
+        LabeledText = partial(_LabeledText, right_width=_METADATA_RIGHT_WIDTH)
+
+        # Name
+        self._frame_name = tk.Frame(self._root)
+        self._frame_name.pack()
+        self._name = LabeledText(
+            self._frame_name,
+            "NAM name",
+            default=parent.user_metadata.name,
+            type=_rstripped_str,
+        )
+        # Modeled by
+        self._frame_modeled_by = tk.Frame(self._root)
+        self._frame_modeled_by.pack()
+        self._modeled_by = LabeledText(
+            self._frame_modeled_by,
+            "Modeled by",
+            default=parent.user_metadata.modeled_by,
+            type=_rstripped_str,
+        )
+        # Gear make
+        self._frame_gear_make = tk.Frame(self._root)
+        self._frame_gear_make.pack()
+        self._gear_make = LabeledText(
+            self._frame_gear_make,
+            "Gear make",
+            default=parent.user_metadata.gear_make,
+            type=_rstripped_str,
+        )
+        # Gear model
+        self._frame_gear_model = tk.Frame(self._root)
+        self._frame_gear_model.pack()
+        self._gear_model = LabeledText(
+            self._frame_gear_model,
+            "Gear model",
+            default=parent.user_metadata.gear_model,
+            type=_rstripped_str,
+        )
+        # Gear type
+        self._frame_gear_type = tk.Frame(self._root)
+        self._frame_gear_type.pack()
+        self._gear_type = _LabeledOptionMenu(
+            self._frame_gear_type,
+            "Gear type",
+            GearType,
+            default=parent.user_metadata.gear_type,
+        )
+        # Tone type
+        self._frame_tone_type = tk.Frame(self._root)
+        self._frame_tone_type.pack()
+        self._tone_type = _LabeledOptionMenu(
+            self._frame_tone_type,
+            "Tone type",
+            ToneType,
+            default=parent.user_metadata.tone_type,
+        )
+
+        # "Ok": apply and destory
+        self._frame_ok = tk.Frame(self._root)
+        self._frame_ok.pack()
+        self._button_ok = tk.Button(
+            self._frame_ok,
+            text="Ok",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._apply_and_destroy,
+        )
+        self._button_ok.pack()
+
+    def mainloop(self):
+        self._root.mainloop()
+
+    def _apply_and_destroy(self):
+        """
+        Set values to parent and destroy this object
+        """
+        self._parent.user_metadata.name = self._name.get()
+        self._parent.user_metadata.modeled_by = self._modeled_by.get()
+        self._parent.user_metadata.gear_make = self._gear_make.get()
+        self._parent.user_metadata.gear_model = self._gear_model.get()
+        self._parent.user_metadata.gear_type = self._gear_type.get()
+        self._parent.user_metadata.tone_type = self._tone_type.get()
+        self._parent.user_metadata_flag = True
+
+        self._root.destroy()
+
+
+def _install_error():
+    window = tk.Tk()
+    window.title("ERROR")
+    label = tk.Label(
+        window,
+        width=45,
+        height=2,
+        text="The NAM training software has not been installed correctly.",
+    )
+    label.pack()
+    button = tk.Button(window, width=10, height=2, text="Quit", command=window.destroy)
+    button.pack()
+    window.mainloop()
+
+
+def run():
+    if _install_is_valid:
+        _gui = _GUI()
+        _gui.mainloop()
+    else:
+        _install_error()
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `neural-amp-modeler-0.5.1/neural_amp_modeler.egg-info/SOURCES.txt` & `neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 nam/models/_names.py
 nam/models/base.py
 nam/models/conv_net.py
 nam/models/linear.py
 nam/models/losses.py
 nam/models/metadata.py
 nam/models/recurrent.py
+nam/models/undersampling.py
 nam/models/wavenet.py
 nam/models/_resources/loudness_input.wav
 nam/models/parametric/__init__.py
 nam/models/parametric/catnets.py
 nam/models/parametric/hyper_net.py
 nam/models/parametric/params.py
 nam/train/__init__.py
 nam/train/_version.py
 nam/train/colab.py
 nam/train/core.py
 nam/train/gui.py
+nam/train/ir.py
 neural_amp_modeler.egg-info/PKG-INFO
 neural_amp_modeler.egg-info/SOURCES.txt
 neural_amp_modeler.egg-info/dependency_links.txt
 neural_amp_modeler.egg-info/entry_points.txt
 neural_amp_modeler.egg-info/requires.txt
 neural_amp_modeler.egg-info/top_level.txt
 tests/test_install.py
```

### Comparing `neural-amp-modeler-0.5.1/setup.py` & `neural-amp-modeler-0.5.2/setup.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# File: setup.py
-# Created Date: 2020-04-08
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-from distutils.util import convert_path
-from setuptools import setup, find_packages
-
-main_ns = {}
-ver_path = convert_path("nam/_version.py")
-with open(ver_path) as ver_file:
-    exec(ver_file.read(), main_ns)
-
-requirements = [
-    "auraloss==0.3.0",
-    "matplotlib",
-    "numpy",
-    "pydantic",
-    "pytorch_lightning",
-    "scipy",
-    "sounddevice",
-    "tensorboard",
-    "torch",
-    "tqdm",
-    "wavio<=0.0.4",  # Breaking change in 0.0.5
-]
-
-setup(
-    name="neural-amp-modeler",
-    version=main_ns["__version__"],
-    description="Neural amp modeler",
-    author="Steven Atkinson",
-    author_email="steven@atkinson.mn",
-    url="https://github.com/sdatkinson/",
-    install_requires=requirements,
-    packages=find_packages(),
-    include_package_data=True,
-    entry_points={
-        "console_scripts": [
-            "nam = nam.train.gui:run",
-        ]
-    },
-)
+# File: setup.py
+# Created Date: 2020-04-08
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+from distutils.util import convert_path
+from setuptools import setup, find_packages
+
+main_ns = {}
+ver_path = convert_path("nam/_version.py")
+with open(ver_path) as ver_file:
+    exec(ver_file.read(), main_ns)
+
+requirements = [
+    "auraloss==0.3.0",
+    "matplotlib",
+    "numpy",
+    "pydantic",
+    "pytorch_lightning",
+    "scipy",
+    "sounddevice",
+    "tensorboard",
+    "torch",
+    "tqdm",
+    "wavio<=0.0.4",  # Breaking change in 0.0.5
+]
+
+setup(
+    name="neural-amp-modeler",
+    version=main_ns["__version__"],
+    description="Neural amp modeler",
+    author="Steven Atkinson",
+    author_email="steven@atkinson.mn",
+    url="https://github.com/sdatkinson/",
+    install_requires=requirements,
+    packages=find_packages(),
+    include_package_data=True,
+    entry_points={
+        "console_scripts": [
+            "nam = nam.train.gui:run",
+        ]
+    },
+)
```


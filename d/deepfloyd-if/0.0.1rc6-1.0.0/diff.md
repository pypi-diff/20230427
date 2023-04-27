# Comparing `tmp/deepfloyd_if-0.0.1rc6.tar.gz` & `tmp/deepfloyd_if-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfloyd_if-0.0.1rc6.tar", last modified: Wed Apr 26 17:13:32 2023, max compression
+gzip compressed data, was "deepfloyd_if-1.0.0.tar", last modified: Wed Apr 26 17:24:25 2023, max compression
```

## Comparing `deepfloyd_if-0.0.1rc6.tar` & `deepfloyd_if-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:13:32.153390 deepfloyd_if-0.0.1rc6/
--rw-r--r--   0 shonenkov   (501) staff       (20)     1504 2023-04-26 14:57:02.000000 deepfloyd_if-0.0.1rc6/LICENSE
--rw-r--r--   0 shonenkov   (501) staff       (20)    11615 2023-04-26 16:50:32.000000 deepfloyd_if-0.0.1rc6/LICENSE-MODEL
--rw-r--r--   0 shonenkov   (501) staff       (20)    14511 2023-04-26 17:13:32.153485 deepfloyd_if-0.0.1rc6/PKG-INFO
--rw-r--r--   0 shonenkov   (501) staff       (20)    14260 2023-04-26 17:02:57.000000 deepfloyd_if-0.0.1rc6/README.md
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:13:32.146526 deepfloyd_if-0.0.1rc6/deepfloyd_if/
--rw-r--r--   0 shonenkov   (501) staff       (20)       51 2023-04-26 17:13:31.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/__init__.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:13:32.148465 deepfloyd_if-0.0.1rc6/deepfloyd_if/model/
--rw-r--r--   0 shonenkov   (501) staff       (20)      118 2022-12-21 22:31:58.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/model/__init__.py
--rw-r--r--   0 shonenkov   (501) staff       (20)    35223 2023-03-09 17:58:29.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/model/gaussian_diffusion.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     2587 2022-12-21 22:31:58.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/model/losses.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     5965 2023-01-10 14:02:27.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/model/nn.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     2001 2022-12-21 22:31:58.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/model/resample.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     6379 2023-01-10 14:02:27.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/model/respace.py
--rw-r--r--   0 shonenkov   (501) staff       (20)    27952 2023-01-28 11:21:37.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/model/unet.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:13:32.150223 deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/
--rw-r--r--   0 shonenkov   (501) staff       (20)      321 2023-04-26 15:11:36.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/__init__.py
--rw-r--r--   0 shonenkov   (501) staff       (20)    15411 2023-04-26 15:11:36.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/base.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1977 2023-04-17 00:13:08.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/stage_I.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1939 2023-04-17 00:13:08.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/stage_II.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1962 2023-04-17 00:13:08.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/stage_III.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     3126 2023-04-26 16:50:32.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/stage_III_sd_x4.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     9421 2022-12-21 22:31:58.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/t5.py
--rw-r--r--   0 shonenkov   (501) staff       (20)      742 2023-04-06 21:54:11.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/utils.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:13:32.151287 deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/
--rw-r--r--   0 shonenkov   (501) staff       (20)      247 2023-03-19 16:24:39.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/__init__.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     5565 2023-04-26 16:50:32.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/dream.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     4522 2023-04-26 16:50:32.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/inpainting.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     4443 2023-04-26 16:50:32.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/style_transfer.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1722 2023-04-26 16:50:32.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/super_resolution.py
--rw-r--r--   0 shonenkov   (501) staff       (20)      709 2023-03-18 20:13:21.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/utils.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:13:32.152058 deepfloyd_if-0.0.1rc6/deepfloyd_if/resources/
--rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/resources/p_head_v1.npz
--rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/resources/w_head_v1.npz
--rw-r--r--   0 shonenkov   (501) staff       (20)      947 2023-01-12 23:07:13.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/resources/wm.png
--rw-r--r--   0 shonenkov   (501) staff       (20)   630912 2022-12-21 22:31:58.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy
--rw-r--r--   0 shonenkov   (501) staff       (20)     2390 2022-12-21 22:31:58.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if/utils.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:13:32.147183 deepfloyd_if-0.0.1rc6/deepfloyd_if.egg-info/
--rw-r--r--   0 shonenkov   (501) staff       (20)    14511 2023-04-26 17:13:32.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if.egg-info/PKG-INFO
--rw-r--r--   0 shonenkov   (501) staff       (20)     1123 2023-04-26 17:13:32.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if.egg-info/SOURCES.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)       39 2023-04-26 17:13:32.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if.egg-info/dependency_links.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)      228 2023-04-26 17:13:32.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if.egg-info/requires.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)       99 2023-04-26 17:13:32.000000 deepfloyd_if-0.0.1rc6/deepfloyd_if.egg-info/top_level.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)      281 2023-04-26 17:13:32.153792 deepfloyd_if-0.0.1rc6/setup.cfg
--rw-r--r--   0 shonenkov   (501) staff       (20)     2018 2023-04-06 21:54:11.000000 deepfloyd_if-0.0.1rc6/setup.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:24:25.269283 deepfloyd_if-1.0.0/
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1504 2023-04-26 14:57:02.000000 deepfloyd_if-1.0.0/LICENSE
+-rw-r--r--   0 shonenkov   (501) staff       (20)    11615 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.0/LICENSE-MODEL
+-rw-r--r--   0 shonenkov   (501) staff       (20)    14569 2023-04-26 17:24:25.269388 deepfloyd_if-1.0.0/PKG-INFO
+-rw-r--r--   0 shonenkov   (501) staff       (20)    14321 2023-04-26 17:23:31.000000 deepfloyd_if-1.0.0/README.md
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:24:25.262367 deepfloyd_if-1.0.0/deepfloyd_if/
+-rw-r--r--   0 shonenkov   (501) staff       (20)       48 2023-04-26 17:22:23.000000 deepfloyd_if-1.0.0/deepfloyd_if/__init__.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:24:25.264229 deepfloyd_if-1.0.0/deepfloyd_if/model/
+-rw-r--r--   0 shonenkov   (501) staff       (20)      118 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.0/deepfloyd_if/model/__init__.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)    35223 2023-03-09 17:58:29.000000 deepfloyd_if-1.0.0/deepfloyd_if/model/gaussian_diffusion.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2587 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.0/deepfloyd_if/model/losses.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     5965 2023-01-10 14:02:27.000000 deepfloyd_if-1.0.0/deepfloyd_if/model/nn.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2001 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.0/deepfloyd_if/model/resample.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     6379 2023-01-10 14:02:27.000000 deepfloyd_if-1.0.0/deepfloyd_if/model/respace.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)    27952 2023-01-28 11:21:37.000000 deepfloyd_if-1.0.0/deepfloyd_if/model/unet.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:24:25.265795 deepfloyd_if-1.0.0/deepfloyd_if/modules/
+-rw-r--r--   0 shonenkov   (501) staff       (20)      321 2023-04-26 15:11:36.000000 deepfloyd_if-1.0.0/deepfloyd_if/modules/__init__.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)    15411 2023-04-26 15:11:36.000000 deepfloyd_if-1.0.0/deepfloyd_if/modules/base.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1977 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.0/deepfloyd_if/modules/stage_I.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1939 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.0/deepfloyd_if/modules/stage_II.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1962 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.0/deepfloyd_if/modules/stage_III.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     3126 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.0/deepfloyd_if/modules/stage_III_sd_x4.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     9421 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.0/deepfloyd_if/modules/t5.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)      742 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.0/deepfloyd_if/modules/utils.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:24:25.266767 deepfloyd_if-1.0.0/deepfloyd_if/pipelines/
+-rw-r--r--   0 shonenkov   (501) staff       (20)      247 2023-03-19 16:24:39.000000 deepfloyd_if-1.0.0/deepfloyd_if/pipelines/__init__.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     5565 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.0/deepfloyd_if/pipelines/dream.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     4522 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.0/deepfloyd_if/pipelines/inpainting.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     4443 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.0/deepfloyd_if/pipelines/style_transfer.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1722 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.0/deepfloyd_if/pipelines/super_resolution.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)      709 2023-03-18 20:13:21.000000 deepfloyd_if-1.0.0/deepfloyd_if/pipelines/utils.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:24:25.267614 deepfloyd_if-1.0.0/deepfloyd_if/resources/
+-rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.0/deepfloyd_if/resources/p_head_v1.npz
+-rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.0/deepfloyd_if/resources/w_head_v1.npz
+-rw-r--r--   0 shonenkov   (501) staff       (20)      947 2023-01-12 23:07:13.000000 deepfloyd_if-1.0.0/deepfloyd_if/resources/wm.png
+-rw-r--r--   0 shonenkov   (501) staff       (20)   630912 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.0/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2390 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.0/deepfloyd_if/utils.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-26 17:24:25.262974 deepfloyd_if-1.0.0/deepfloyd_if.egg-info/
+-rw-r--r--   0 shonenkov   (501) staff       (20)    14569 2023-04-26 17:24:25.000000 deepfloyd_if-1.0.0/deepfloyd_if.egg-info/PKG-INFO
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1123 2023-04-26 17:24:25.000000 deepfloyd_if-1.0.0/deepfloyd_if.egg-info/SOURCES.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)        1 2023-04-26 17:24:25.000000 deepfloyd_if-1.0.0/deepfloyd_if.egg-info/dependency_links.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)      228 2023-04-26 17:24:25.000000 deepfloyd_if-1.0.0/deepfloyd_if.egg-info/requires.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)       99 2023-04-26 17:24:25.000000 deepfloyd_if-1.0.0/deepfloyd_if.egg-info/top_level.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)      281 2023-04-26 17:24:25.269891 deepfloyd_if-1.0.0/setup.cfg
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2018 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.0/setup.py
```

### Comparing `deepfloyd_if-0.0.1rc6/LICENSE` & `deepfloyd_if-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/LICENSE-MODEL` & `deepfloyd_if-1.0.0/LICENSE-MODEL`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/PKG-INFO` & `deepfloyd_if-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfloyd_if
-Version: 0.0.1rc6
+Version: 1.0.0
 Summary: DeepFloyd-IF (Imagen Free)
 Author: DeepFloyd, StabilityAI
 Author-email: shonenkov@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE-MODEL
 
@@ -36,14 +36,15 @@
 ## Quick Start
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1KDOntg5NCnaEocz7et1pudM5zyZBv23o?usp=sharing)
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/DeepFloyd/IF)
 
 ```shell
 pip install deepfloyd_if==1.0.0
 pip install xformers==0.0.16
+pip install git+https://github.com/openai/CLIP.git --no-deps
 ```
 
 ## Local notebook and UI demo
 
 The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable as in a Jupyter Notebook at `IF/notebooks/pipes-DeepFloyd-IF.ipynb` or as Gradio UI demo that you can run locally with
 ```shell
 pip install gradio
```

### Comparing `deepfloyd_if-0.0.1rc6/README.md` & `deepfloyd_if-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ## Quick Start
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1KDOntg5NCnaEocz7et1pudM5zyZBv23o?usp=sharing)
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/DeepFloyd/IF)
 
 ```shell
 pip install deepfloyd_if==1.0.0
 pip install xformers==0.0.16
+pip install git+https://github.com/openai/CLIP.git --no-deps
 ```
 
 ## Local notebook and UI demo
 
 The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable as in a Jupyter Notebook at `IF/notebooks/pipes-DeepFloyd-IF.ipynb` or as Gradio UI demo that you can run locally with
 ```shell
 pip install gradio
```

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/model/gaussian_diffusion.py` & `deepfloyd_if-1.0.0/deepfloyd_if/model/gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/model/losses.py` & `deepfloyd_if-1.0.0/deepfloyd_if/model/losses.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/model/nn.py` & `deepfloyd_if-1.0.0/deepfloyd_if/model/nn.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/model/resample.py` & `deepfloyd_if-1.0.0/deepfloyd_if/model/resample.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/model/respace.py` & `deepfloyd_if-1.0.0/deepfloyd_if/model/respace.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/model/unet.py` & `deepfloyd_if-1.0.0/deepfloyd_if/model/unet.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/base.py` & `deepfloyd_if-1.0.0/deepfloyd_if/modules/base.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/stage_I.py` & `deepfloyd_if-1.0.0/deepfloyd_if/modules/stage_I.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/stage_II.py` & `deepfloyd_if-1.0.0/deepfloyd_if/modules/stage_II.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/stage_III.py` & `deepfloyd_if-1.0.0/deepfloyd_if/modules/stage_III.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/stage_III_sd_x4.py` & `deepfloyd_if-1.0.0/deepfloyd_if/modules/stage_III_sd_x4.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/t5.py` & `deepfloyd_if-1.0.0/deepfloyd_if/modules/t5.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/modules/utils.py` & `deepfloyd_if-1.0.0/deepfloyd_if/modules/utils.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/dream.py` & `deepfloyd_if-1.0.0/deepfloyd_if/pipelines/dream.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/inpainting.py` & `deepfloyd_if-1.0.0/deepfloyd_if/pipelines/inpainting.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/style_transfer.py` & `deepfloyd_if-1.0.0/deepfloyd_if/pipelines/style_transfer.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/super_resolution.py` & `deepfloyd_if-1.0.0/deepfloyd_if/pipelines/super_resolution.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/pipelines/utils.py` & `deepfloyd_if-1.0.0/deepfloyd_if/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/resources/p_head_v1.npz` & `deepfloyd_if-1.0.0/deepfloyd_if/resources/p_head_v1.npz`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/resources/w_head_v1.npz` & `deepfloyd_if-1.0.0/deepfloyd_if/resources/w_head_v1.npz`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/resources/wm.png` & `deepfloyd_if-1.0.0/deepfloyd_if/resources/wm.png`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy` & `deepfloyd_if-1.0.0/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if/utils.py` & `deepfloyd_if-1.0.0/deepfloyd_if/utils.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if.egg-info/PKG-INFO` & `deepfloyd_if-1.0.0/deepfloyd_if.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfloyd-if
-Version: 0.0.1rc6
+Version: 1.0.0
 Summary: DeepFloyd-IF (Imagen Free)
 Author: DeepFloyd, StabilityAI
 Author-email: shonenkov@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE-MODEL
 
@@ -36,14 +36,15 @@
 ## Quick Start
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1KDOntg5NCnaEocz7et1pudM5zyZBv23o?usp=sharing)
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/DeepFloyd/IF)
 
 ```shell
 pip install deepfloyd_if==1.0.0
 pip install xformers==0.0.16
+pip install git+https://github.com/openai/CLIP.git --no-deps
 ```
 
 ## Local notebook and UI demo
 
 The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable as in a Jupyter Notebook at `IF/notebooks/pipes-DeepFloyd-IF.ipynb` or as Gradio UI demo that you can run locally with
 ```shell
 pip install gradio
```

### Comparing `deepfloyd_if-0.0.1rc6/deepfloyd_if.egg-info/SOURCES.txt` & `deepfloyd_if-1.0.0/deepfloyd_if.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-0.0.1rc6/setup.py` & `deepfloyd_if-1.0.0/setup.py`

 * *Files identical despite different names*


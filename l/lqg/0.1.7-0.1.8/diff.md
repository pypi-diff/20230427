# Comparing `tmp/lqg-0.1.7.tar.gz` & `tmp/lqg-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqg-0.1.7.tar", last modified: Mon Aug 22 14:49:28 2022, max compression
+gzip compressed data, was "lqg-0.1.8.tar", last modified: Thu Apr 27 11:21:47 2023, max compression
```

## Comparing `lqg-0.1.7.tar` & `lqg-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-08-22 14:49:28.679106 lqg-0.1.7/
--rw-r--r--   0 dominik   (1000) dominik   (1000)    34523 2022-08-19 15:34:18.000000 lqg-0.1.7/LICENSE
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2837 2022-08-22 14:49:28.679106 lqg-0.1.7/PKG-INFO
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2345 2022-08-22 12:12:18.000000 lqg-0.1.7/README.md
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-08-22 14:49:28.672439 lqg-0.1.7/lqg/
--rw-r--r--   0 dominik   (1000) dominik   (1000)       49 2022-08-22 14:48:52.000000 lqg-0.1.7/lqg/__init__.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2028 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/ccg.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-08-22 14:49:28.675773 lqg-0.1.7/lqg/infer/
--rw-r--r--   0 dominik   (1000) dominik   (1000)      121 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/infer/__init__.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1758 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/infer/map.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1557 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/infer/mle.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     3721 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/infer/models.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2158 2022-08-22 12:26:18.000000 lqg-0.1.7/lqg/infer/prior.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1542 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/infer/utils.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2968 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/io.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     4456 2022-08-22 12:17:15.000000 lqg-0.1.7/lqg/kalman.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     6971 2022-08-22 14:37:15.000000 lqg-0.1.7/lqg/model.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     7607 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/optim.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1644 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/riccati.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-08-22 14:49:28.675773 lqg-0.1.7/lqg/tracking/
--rw-r--r--   0 dominik   (1000) dominik   (1000)      587 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/tracking/__init__.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     4955 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/tracking/basic.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)    11395 2022-08-22 12:15:15.000000 lqg-0.1.7/lqg/tracking/eye.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)      698 2022-08-22 12:19:48.000000 lqg-0.1.7/lqg/tracking/kf.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     5517 2022-08-22 12:23:30.000000 lqg-0.1.7/lqg/tracking/subjective.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     3096 2022-08-19 15:34:18.000000 lqg-0.1.7/lqg/tracking/three_dims.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-08-22 14:49:28.675773 lqg-0.1.7/lqg.egg-info/
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2837 2022-08-22 14:49:28.000000 lqg-0.1.7/lqg.egg-info/PKG-INFO
--rw-r--r--   0 dominik   (1000) dominik   (1000)      506 2022-08-22 14:49:28.000000 lqg-0.1.7/lqg.egg-info/SOURCES.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)        1 2022-08-22 14:49:28.000000 lqg-0.1.7/lqg.egg-info/dependency_links.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)      104 2022-08-22 14:49:28.000000 lqg-0.1.7/lqg.egg-info/requires.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)        4 2022-08-22 14:49:28.000000 lqg-0.1.7/lqg.egg-info/top_level.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)       38 2022-08-22 14:49:28.679106 lqg-0.1.7/setup.cfg
--rw-r--r--   0 dominik   (1000) dominik   (1000)      919 2022-08-22 14:48:27.000000 lqg-0.1.7/setup.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-27 11:21:47.694705 lqg-0.1.8/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)    34523 2023-04-05 08:53:51.000000 lqg-0.1.8/LICENSE
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2876 2023-04-27 11:21:47.694705 lqg-0.1.8/PKG-INFO
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2384 2023-04-27 11:11:09.000000 lqg-0.1.8/README.md
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-27 11:21:47.694705 lqg-0.1.8/lqg/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)       49 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/__init__.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2028 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/ccg.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-27 11:21:47.694705 lqg-0.1.8/lqg/infer/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      121 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/infer/__init__.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     1758 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/infer/map.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     1557 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/infer/mle.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     3721 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/infer/models.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2158 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/infer/prior.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     1542 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/infer/utils.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2968 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/io.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     4456 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/kalman.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     6971 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/model.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     7607 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/optim.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     1644 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/riccati.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-27 11:21:47.694705 lqg-0.1.8/lqg/tracking/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      587 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/__init__.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     4955 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/basic.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)    11395 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/eye.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      698 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/kf.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     5517 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/subjective.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     3096 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/three_dims.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-27 11:21:47.694705 lqg-0.1.8/lqg.egg-info/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2876 2023-04-27 11:21:47.000000 lqg-0.1.8/lqg.egg-info/PKG-INFO
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      506 2023-04-27 11:21:47.000000 lqg-0.1.8/lqg.egg-info/SOURCES.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)        1 2023-04-27 11:21:47.000000 lqg-0.1.8/lqg.egg-info/dependency_links.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      104 2023-04-27 11:21:47.000000 lqg-0.1.8/lqg.egg-info/requires.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)        4 2023-04-27 11:21:47.000000 lqg-0.1.8/lqg.egg-info/top_level.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)       38 2023-04-27 11:21:47.694705 lqg-0.1.8/setup.cfg
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      919 2023-04-27 11:12:46.000000 lqg-0.1.8/setup.py
```

### Comparing `lqg-0.1.7/LICENSE` & `lqg-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/PKG-INFO` & `lqg-0.1.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: lqg
-Version: 0.1.7
+Version: 0.1.8
 Summary: (Inverse) optimal control for linear quadratic Gaussian systems
 Home-page: https://github.com/dominikstrb/lqg
 Author: Dominik Straub
 Author-email: dominik.straub@tu-darmstadt.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Inverse optimal control for continuous psychophysics
 
-![Experimenter-actor-loop](https://raw.githubusercontent.com/RothkopfLab/lqg/main/img/experimenter-actor-loop.png)
+![Experimenter-actor-loop](https://raw.githubusercontent.com/RothkopfLab/lqg/main/docs/source/_static/experimenter-actor-loop.png)
 
 
-This repository contains the official implementation of the inverse optimal control method presented in the paper:
+This repository contains the official [JAX](https://github.com/google/jax) implementation of the inverse optimal control method presented in the paper:
 
-> Straub, D., & Rothkopf, C. A. (2021). Putting perception into action: Inverse optimal control for continuous psychophysics. [bioRxiv.](https://www.biorxiv.org/content/10.1101/2021.12.23.473976v1.abstract)
-
-## CCN 2022 tutorial
-For our [tutorial at CCN 2022](https://2022.ccneuro.org/view_event.php?mid=19), you can follow along in the Jupyter notebook [CCN_2022_Tutorial.ipynb](https://github.com/RothkopfLab/lqg/blob/main/CCN_2022_Tutorial.ipynb). To run the notebook, you can either install the `lqg` package locally (see [below](https://github.com/RothkopfLab/lqg#installation)) or [open it in the browser](https://colab.research.google.com/github/dominikstrb/lqg/blob/main/CCN_2022_Tutorial.ipynb) on Google Colab.
+> [Straub, D., & Rothkopf, C. A. (2022). Putting perception into action with inverse optimal control for continuous psychophysics. eLife, 11, e76635.](https://elifesciences.org/articles/76635)
 
 ## Installation
 The package can be installed via `pip`
 
 ```bash
 python -m pip install lqg
 ```
@@ -43,18 +40,23 @@
 - `main.py` shows how to simulate data and infer parameters using the LQG model of the tracking task.
 
 - [`notebooks/01-HowTo.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/01-HowTo.ipynb) explains the model and its parameters in more detail, including the extension to subjective internal models.
 
 - [`notebooks/02-Data.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/02-Data.ipynb) fits the ideal observer and bounded actor model to the [data](https://github.com/kbonnen/BonnenEtAl2015_KalmanFilterCode) from [Bonnen et al. (2015)](https://jov.arvojournals.org/article.aspx?articleid=2301260) to reproduce Fig. 4A from our paper.
 
 ## Citation
-If you use our method in your research, please cite our preprint:
+If you use our method or code in your research, please cite our paper:
 
 ```
-@article{straub2021putting,
-  title={Putting perception into action: Inverse optimal control for continuous psychophysics},
+@article{straub2022putting,
+  title={Putting perception into action with inverse optimal control for continuous psychophysics},
   author={Straub, Dominik and Rothkopf, Constantin A},
-  journal={bioRxiv},
-  year={2021},
-  publisher={Cold Spring Harbor Laboratory}
+  journal={eLife},
+  volume={11},
+  pages={e76635},
+  year={2022},
+  publisher={eLife Sciences Publications Limited}
 }
 ```
+
+## Signal-dependent noise
+This implementation supports the basic LQG framework. For the extension to signal-dependent noise [(Todorov, 2005)](https://direct.mit.edu/neco/article-abstract/17/5/1084/6949/Stochastic-Optimal-Control-and-Estimation-Methods), please see [our NeurIPS 2021 paper](https://proceedings.neurips.cc/paper/2021/hash/4e55139e019a58e0084f194f758ffdea-Abstract.html) and [its implementation](https://github.com/RothkopfLab/inverse-optimal-control).
```

### Comparing `lqg-0.1.7/README.md` & `lqg-0.1.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 # Inverse optimal control for continuous psychophysics
 
-![Experimenter-actor-loop](https://raw.githubusercontent.com/RothkopfLab/lqg/main/img/experimenter-actor-loop.png)
+![Experimenter-actor-loop](https://raw.githubusercontent.com/RothkopfLab/lqg/main/docs/source/_static/experimenter-actor-loop.png)
 
 
-This repository contains the official implementation of the inverse optimal control method presented in the paper:
+This repository contains the official [JAX](https://github.com/google/jax) implementation of the inverse optimal control method presented in the paper:
 
-> Straub, D., & Rothkopf, C. A. (2021). Putting perception into action: Inverse optimal control for continuous psychophysics. [bioRxiv.](https://www.biorxiv.org/content/10.1101/2021.12.23.473976v1.abstract)
-
-## CCN 2022 tutorial
-For our [tutorial at CCN 2022](https://2022.ccneuro.org/view_event.php?mid=19), you can follow along in the Jupyter notebook [CCN_2022_Tutorial.ipynb](https://github.com/RothkopfLab/lqg/blob/main/CCN_2022_Tutorial.ipynb). To run the notebook, you can either install the `lqg` package locally (see [below](https://github.com/RothkopfLab/lqg#installation)) or [open it in the browser](https://colab.research.google.com/github/dominikstrb/lqg/blob/main/CCN_2022_Tutorial.ipynb) on Google Colab.
+> [Straub, D., & Rothkopf, C. A. (2022). Putting perception into action with inverse optimal control for continuous psychophysics. eLife, 11, e76635.](https://elifesciences.org/articles/76635)
 
 ## Installation
 The package can be installed via `pip`
 
 ```bash
 python -m pip install lqg
 ```
@@ -29,18 +26,23 @@
 - `main.py` shows how to simulate data and infer parameters using the LQG model of the tracking task.
 
 - [`notebooks/01-HowTo.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/01-HowTo.ipynb) explains the model and its parameters in more detail, including the extension to subjective internal models.
 
 - [`notebooks/02-Data.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/02-Data.ipynb) fits the ideal observer and bounded actor model to the [data](https://github.com/kbonnen/BonnenEtAl2015_KalmanFilterCode) from [Bonnen et al. (2015)](https://jov.arvojournals.org/article.aspx?articleid=2301260) to reproduce Fig. 4A from our paper.
 
 ## Citation
-If you use our method in your research, please cite our preprint:
+If you use our method or code in your research, please cite our paper:
 
 ```
-@article{straub2021putting,
-  title={Putting perception into action: Inverse optimal control for continuous psychophysics},
+@article{straub2022putting,
+  title={Putting perception into action with inverse optimal control for continuous psychophysics},
   author={Straub, Dominik and Rothkopf, Constantin A},
-  journal={bioRxiv},
-  year={2021},
-  publisher={Cold Spring Harbor Laboratory}
+  journal={eLife},
+  volume={11},
+  pages={e76635},
+  year={2022},
+  publisher={eLife Sciences Publications Limited}
 }
 ```
+
+## Signal-dependent noise
+This implementation supports the basic LQG framework. For the extension to signal-dependent noise [(Todorov, 2005)](https://direct.mit.edu/neco/article-abstract/17/5/1084/6949/Stochastic-Optimal-Control-and-Estimation-Methods), please see [our NeurIPS 2021 paper](https://proceedings.neurips.cc/paper/2021/hash/4e55139e019a58e0084f194f758ffdea-Abstract.html) and [its implementation](https://github.com/RothkopfLab/inverse-optimal-control).
```

### Comparing `lqg-0.1.7/lqg/ccg.py` & `lqg-0.1.8/lqg/ccg.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/infer/map.py` & `lqg-0.1.8/lqg/infer/map.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/infer/mle.py` & `lqg-0.1.8/lqg/infer/mle.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/infer/models.py` & `lqg-0.1.8/lqg/infer/models.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/infer/prior.py` & `lqg-0.1.8/lqg/infer/prior.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/infer/utils.py` & `lqg-0.1.8/lqg/infer/utils.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/io.py` & `lqg-0.1.8/lqg/io.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/kalman.py` & `lqg-0.1.8/lqg/kalman.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/model.py` & `lqg-0.1.8/lqg/model.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/optim.py` & `lqg-0.1.8/lqg/optim.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/riccati.py` & `lqg-0.1.8/lqg/riccati.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/tracking/__init__.py` & `lqg-0.1.8/lqg/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/tracking/basic.py` & `lqg-0.1.8/lqg/tracking/basic.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/tracking/eye.py` & `lqg-0.1.8/lqg/tracking/eye.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/tracking/kf.py` & `lqg-0.1.8/lqg/tracking/kf.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/tracking/subjective.py` & `lqg-0.1.8/lqg/tracking/subjective.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg/tracking/three_dims.py` & `lqg-0.1.8/lqg/tracking/three_dims.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.7/lqg.egg-info/PKG-INFO` & `lqg-0.1.8/lqg.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: lqg
-Version: 0.1.7
+Version: 0.1.8
 Summary: (Inverse) optimal control for linear quadratic Gaussian systems
 Home-page: https://github.com/dominikstrb/lqg
 Author: Dominik Straub
 Author-email: dominik.straub@tu-darmstadt.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Inverse optimal control for continuous psychophysics
 
-![Experimenter-actor-loop](https://raw.githubusercontent.com/RothkopfLab/lqg/main/img/experimenter-actor-loop.png)
+![Experimenter-actor-loop](https://raw.githubusercontent.com/RothkopfLab/lqg/main/docs/source/_static/experimenter-actor-loop.png)
 
 
-This repository contains the official implementation of the inverse optimal control method presented in the paper:
+This repository contains the official [JAX](https://github.com/google/jax) implementation of the inverse optimal control method presented in the paper:
 
-> Straub, D., & Rothkopf, C. A. (2021). Putting perception into action: Inverse optimal control for continuous psychophysics. [bioRxiv.](https://www.biorxiv.org/content/10.1101/2021.12.23.473976v1.abstract)
-
-## CCN 2022 tutorial
-For our [tutorial at CCN 2022](https://2022.ccneuro.org/view_event.php?mid=19), you can follow along in the Jupyter notebook [CCN_2022_Tutorial.ipynb](https://github.com/RothkopfLab/lqg/blob/main/CCN_2022_Tutorial.ipynb). To run the notebook, you can either install the `lqg` package locally (see [below](https://github.com/RothkopfLab/lqg#installation)) or [open it in the browser](https://colab.research.google.com/github/dominikstrb/lqg/blob/main/CCN_2022_Tutorial.ipynb) on Google Colab.
+> [Straub, D., & Rothkopf, C. A. (2022). Putting perception into action with inverse optimal control for continuous psychophysics. eLife, 11, e76635.](https://elifesciences.org/articles/76635)
 
 ## Installation
 The package can be installed via `pip`
 
 ```bash
 python -m pip install lqg
 ```
@@ -43,18 +40,23 @@
 - `main.py` shows how to simulate data and infer parameters using the LQG model of the tracking task.
 
 - [`notebooks/01-HowTo.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/01-HowTo.ipynb) explains the model and its parameters in more detail, including the extension to subjective internal models.
 
 - [`notebooks/02-Data.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/02-Data.ipynb) fits the ideal observer and bounded actor model to the [data](https://github.com/kbonnen/BonnenEtAl2015_KalmanFilterCode) from [Bonnen et al. (2015)](https://jov.arvojournals.org/article.aspx?articleid=2301260) to reproduce Fig. 4A from our paper.
 
 ## Citation
-If you use our method in your research, please cite our preprint:
+If you use our method or code in your research, please cite our paper:
 
 ```
-@article{straub2021putting,
-  title={Putting perception into action: Inverse optimal control for continuous psychophysics},
+@article{straub2022putting,
+  title={Putting perception into action with inverse optimal control for continuous psychophysics},
   author={Straub, Dominik and Rothkopf, Constantin A},
-  journal={bioRxiv},
-  year={2021},
-  publisher={Cold Spring Harbor Laboratory}
+  journal={eLife},
+  volume={11},
+  pages={e76635},
+  year={2022},
+  publisher={eLife Sciences Publications Limited}
 }
 ```
+
+## Signal-dependent noise
+This implementation supports the basic LQG framework. For the extension to signal-dependent noise [(Todorov, 2005)](https://direct.mit.edu/neco/article-abstract/17/5/1084/6949/Stochastic-Optimal-Control-and-Estimation-Methods), please see [our NeurIPS 2021 paper](https://proceedings.neurips.cc/paper/2021/hash/4e55139e019a58e0084f194f758ffdea-Abstract.html) and [its implementation](https://github.com/RothkopfLab/inverse-optimal-control).
```

### Comparing `lqg-0.1.7/setup.py` & `lqg-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lqg",
-    version="0.1.7",
+    version="0.1.8",
     author="Dominik Straub",
     author_email="dominik.straub@tu-darmstadt.de",
     description="(Inverse) optimal control for linear quadratic Gaussian systems",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dominikstrb/lqg",
     packages=setuptools.find_packages(),
@@ -18,14 +18,14 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
     install_requires=[
         "numpy>=1.20.3",
         "scipy>=1.6.3",
-        "matplotlib==3.2.2",
+        "matplotlib>=3.2.2",
         "ipywidgets==8.0.1",
         "numpyro==0.9.2",
         "jax>=0.3.14",
         "arviz>=0.11.2",
     ],
 )
```


# Comparing `tmp/lovely-jax-0.1.1.dev0.tar.gz` & `tmp/lovely-jax-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovely-jax-0.1.1.dev0.tar", last modified: Wed Jan 11 11:27:19 2023, max compression
+gzip compressed data, was "lovely-jax-0.1.2.tar", last modified: Thu Apr 27 10:38:40 2023, max compression
```

## Comparing `lovely-jax-0.1.1.dev0.tar` & `lovely-jax-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,28 @@
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:27:19.387900 lovely-jax-0.1.1.dev0/
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:27:19.379900 lovely-jax-0.1.1.dev0/.github/
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:27:19.379900 lovely-jax-0.1.1.dev0/.github/workflows/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      194 2022-09-05 16:31:43.000000 lovely-jax-0.1.1.dev0/.github/workflows/deploy.yaml
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      148 2022-09-05 16:31:43.000000 lovely-jax-0.1.1.dev0/.github/workflows/test.yaml
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1799 2022-11-08 08:16:16.000000 lovely-jax-0.1.1.dev0/.gitignore
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1071 2022-11-08 02:17:59.000000 lovely-jax-0.1.1.dev0/LICENSE
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      111 2022-09-05 16:31:43.000000 lovely-jax-0.1.1.dev0/MANIFEST.in
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    11790 2023-01-11 11:27:19.387900 lovely-jax-0.1.1.dev0/PKG-INFO
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    11065 2023-01-11 11:24:37.000000 lovely-jax-0.1.1.dev0/README.md
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:27:19.379900 lovely-jax-0.1.1.dev0/lovely_jax/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      168 2023-01-11 11:24:19.000000 lovely-jax-0.1.1.dev0/lovely_jax/__init__.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     7070 2023-01-11 11:24:19.000000 lovely-jax-0.1.1.dev0/lovely_jax/_modidx.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     2107 2023-01-11 11:24:19.000000 lovely-jax-0.1.1.dev0/lovely_jax/patch.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     3296 2023-01-11 11:24:18.000000 lovely-jax-0.1.1.dev0/lovely_jax/repr_chans.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     2858 2023-01-11 11:24:18.000000 lovely-jax-0.1.1.dev0/lovely_jax/repr_plt.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     3128 2023-01-11 11:24:18.000000 lovely-jax-0.1.1.dev0/lovely_jax/repr_rgb.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     7004 2023-01-11 11:24:18.000000 lovely-jax-0.1.1.dev0/lovely_jax/repr_str.py
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:27:19.383900 lovely-jax-0.1.1.dev0/lovely_jax/utils/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       22 2023-01-11 11:24:19.000000 lovely-jax-0.1.1.dev0/lovely_jax/utils/__init__.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     3588 2023-01-11 11:24:18.000000 lovely-jax-0.1.1.dev0/lovely_jax/utils/config.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1373 2023-01-11 11:24:18.000000 lovely-jax-0.1.1.dev0/lovely_jax/utils/misc.py
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:27:19.379900 lovely-jax-0.1.1.dev0/lovely_jax.egg-info/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    11790 2023-01-11 11:27:19.000000 lovely-jax-0.1.1.dev0/lovely_jax.egg-info/PKG-INFO
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      736 2023-01-11 11:27:19.000000 lovely-jax-0.1.1.dev0/lovely_jax.egg-info/SOURCES.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2023-01-11 11:27:19.000000 lovely-jax-0.1.1.dev0/lovely_jax.egg-info/dependency_links.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       42 2023-01-11 11:27:19.000000 lovely-jax-0.1.1.dev0/lovely_jax.egg-info/entry_points.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2022-11-08 06:49:26.000000 lovely-jax-0.1.1.dev0/lovely_jax.egg-info/not-zip-safe
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       41 2023-01-11 11:27:19.000000 lovely-jax-0.1.1.dev0/lovely_jax.egg-info/requires.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       11 2023-01-11 11:27:19.000000 lovely-jax-0.1.1.dev0/lovely_jax.egg-info/top_level.txt
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:27:19.387900 lovely-jax-0.1.1.dev0/nbs/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    25393 2023-01-11 11:24:33.000000 lovely-jax-0.1.1.dev0/nbs/00_repr_str.ipynb
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   895908 2023-01-01 11:14:19.000000 lovely-jax-0.1.1.dev0/nbs/10_patch.ipynb
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      396 2022-11-08 07:41:11.000000 lovely-jax-0.1.1.dev0/nbs/_quarto.yml
--rw-rw-r--   0 xl0       (1000) xl0       (1000)  2680230 2023-01-11 11:24:33.000000 lovely-jax-0.1.1.dev0/nbs/index.ipynb
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   461120 2022-11-08 02:28:04.000000 lovely-jax-0.1.1.dev0/nbs/mysteryman.npy
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      211 2023-01-11 11:24:33.000000 lovely-jax-0.1.1.dev0/nbs/nbdev.yml
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      523 2022-12-27 07:22:36.000000 lovely-jax-0.1.1.dev0/nbs/sidebar.yml
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      676 2022-11-08 08:07:49.000000 lovely-jax-0.1.1.dev0/nbs/styles.css
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1041 2023-01-11 11:21:21.000000 lovely-jax-0.1.1.dev0/settings.ini
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       38 2023-01-11 11:27:19.387900 lovely-jax-0.1.1.dev0/setup.cfg
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     2541 2022-09-05 16:31:43.000000 lovely-jax-0.1.1.dev0/setup.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-04-27 10:38:40.974894 lovely-jax-0.1.2/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1071 2023-03-12 08:32:48.000000 lovely-jax-0.1.2/LICENSE
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      111 2023-03-12 08:32:48.000000 lovely-jax-0.1.2/MANIFEST.in
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    15461 2023-04-27 10:38:40.974894 lovely-jax-0.1.2/PKG-INFO
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    14741 2023-04-27 10:31:42.000000 lovely-jax-0.1.2/README.md
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-04-27 10:38:40.974894 lovely-jax-0.1.2/lovely_jax/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      163 2023-04-27 10:35:07.000000 lovely-jax-0.1.2/lovely_jax/__init__.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     7070 2023-04-27 10:35:07.000000 lovely-jax-0.1.2/lovely_jax/_modidx.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2271 2023-04-27 10:35:07.000000 lovely-jax-0.1.2/lovely_jax/patch.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     3296 2023-04-27 10:35:07.000000 lovely-jax-0.1.2/lovely_jax/repr_chans.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2898 2023-04-27 10:35:07.000000 lovely-jax-0.1.2/lovely_jax/repr_plt.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     3128 2023-04-27 10:35:07.000000 lovely-jax-0.1.2/lovely_jax/repr_rgb.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     7807 2023-04-27 10:35:07.000000 lovely-jax-0.1.2/lovely_jax/repr_str.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-04-27 10:38:40.974894 lovely-jax-0.1.2/lovely_jax/utils/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       22 2023-04-27 10:35:07.000000 lovely-jax-0.1.2/lovely_jax/utils/__init__.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     3794 2023-04-27 10:35:07.000000 lovely-jax-0.1.2/lovely_jax/utils/config.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1691 2023-04-27 10:35:07.000000 lovely-jax-0.1.2/lovely_jax/utils/misc.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-04-27 10:38:40.974894 lovely-jax-0.1.2/lovely_jax.egg-info/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    15461 2023-04-27 10:38:40.000000 lovely-jax-0.1.2/lovely_jax.egg-info/PKG-INFO
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      530 2023-04-27 10:38:40.000000 lovely-jax-0.1.2/lovely_jax.egg-info/SOURCES.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2023-04-27 10:38:40.000000 lovely-jax-0.1.2/lovely_jax.egg-info/dependency_links.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       42 2023-04-27 10:38:40.000000 lovely-jax-0.1.2/lovely_jax.egg-info/entry_points.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2023-03-13 11:38:21.000000 lovely-jax-0.1.2/lovely_jax.egg-info/not-zip-safe
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       36 2023-04-27 10:38:40.000000 lovely-jax-0.1.2/lovely_jax.egg-info/requires.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       11 2023-04-27 10:38:40.000000 lovely-jax-0.1.2/lovely_jax.egg-info/top_level.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1031 2023-04-27 10:34:43.000000 lovely-jax-0.1.2/settings.ini
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       38 2023-04-27 10:38:40.974894 lovely-jax-0.1.2/setup.cfg
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2541 2023-03-12 08:32:48.000000 lovely-jax-0.1.2/setup.py
```

### Comparing `lovely-jax-0.1.1.dev0/LICENSE` & `lovely-jax-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lovely-jax-0.1.1.dev0/README.md` & `lovely-jax-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: lovely-jax
+Version: 0.1.2
+Summary: 💘 Lovely JAX
+Home-page: https://github.com/xl0/lovely-jax
+Author: Alexey Zaytsev
+Author-email: alexey.zaytsev@gmail.com
+License: MIT License
+Keywords: nbdev jupyter jax
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 💘 Lovely JAX
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 <div>
 
@@ -74,49 +96,49 @@
 
 ## Summary
 
 ``` python
 numbers
 ```
 
-    Array[196, 196, 3] n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073 gpu:0
+    Array[196, 196, 3] n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073 cpu:0
 
 Better, huh?
 
 ``` python
 numbers[1,:6,1] # Still shows values if there are not too many.
 ```
 
-    Array[6] x∈[-0.408, -0.232] μ=-0.340 σ=0.075 gpu:0 [-0.250, -0.232, -0.338, -0.408, -0.408, -0.408]
+    Array[6] x∈[-0.408, -0.232] μ=-0.340 σ=0.075 cpu:0 [-0.250, -0.232, -0.338, -0.408, -0.408, -0.408]
 
 ``` python
 spicy = numbers.flatten()[:12].copy()
 
 spicy = (spicy  .at[0].mul(10000)
                 .at[1].divide(10000)
                 .at[2].set(float('inf'))
                 .at[3].set(float('-inf'))
                 .at[4].set(float('nan'))
                 .reshape((2,6)))
 spicy # Spicy stuff
 ```
 
-    Array[2, 6] n=12 x∈[-3.541e+03, -1.975e-05] μ=-393.848 σ=1.113e+03 +Inf! -Inf! NaN! gpu:0
+    Array[2, 6] n=12 x∈[-3.541e+03, -1.975e-05] μ=-393.848 σ=1.113e+03 +Inf! -Inf! NaN! cpu:0
 
 ``` python
 jnp.zeros((10, 10)) # A zero array - make it obvious
 ```
 
-    Array[10, 10] all_zeros gpu:0
+    Array[10, 10] n=100 all_zeros cpu:0
 
 ``` python
 spicy.v # Verbose
 ```
 
-    Array[2, 6] n=12 x∈[-3.541e+03, -1.975e-05] μ=-393.848 σ=1.113e+03 +Inf! -Inf! NaN! gpu:0
+    Array[2, 6] n=12 x∈[-3.541e+03, -1.975e-05] μ=-393.848 σ=1.113e+03 +Inf! -Inf! NaN! cpu:0
     Array([[-3.541e+03, -1.975e-05,        inf,       -inf,        nan, -9.853e-01],
            [-4.054e-01, -3.025e-01, -8.807e-01, -4.397e-01, -3.025e-01, -7.761e-01]], dtype=float32)
 
 ``` python
 spicy.p # The plain old way
 ```
 
@@ -125,228 +147,266 @@
 
 ## Going `.deeper`
 
 ``` python
 numbers.deeper
 ```
 
-    Array[196, 196, 3] n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073 gpu:0
-      Array[196, 3] n=588 x∈[-1.912, 2.411] μ=-0.728 σ=0.519 gpu:0
-      Array[196, 3] n=588 x∈[-1.861, 2.359] μ=-0.778 σ=0.450 gpu:0
-      Array[196, 3] n=588 x∈[-1.758, 2.379] μ=-0.838 σ=0.437 gpu:0
-      Array[196, 3] n=588 x∈[-1.656, 2.466] μ=-0.878 σ=0.415 gpu:0
-      Array[196, 3] n=588 x∈[-1.717, 2.448] μ=-0.882 σ=0.399 gpu:0
-      Array[196, 3] n=588 x∈[-1.717, 2.431] μ=-0.905 σ=0.408 gpu:0
-      Array[196, 3] n=588 x∈[-1.563, 2.448] μ=-0.859 σ=0.416 gpu:0
-      Array[196, 3] n=588 x∈[-1.475, 2.431] μ=-0.791 σ=0.463 gpu:0
-      Array[196, 3] n=588 x∈[-1.526, 2.429] μ=-0.759 σ=0.499 gpu:0
+    Array[196, 196, 3] n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073 cpu:0
+      Array[196, 3] n=588 x∈[-1.912, 2.411] μ=-0.728 σ=0.519 cpu:0
+      Array[196, 3] n=588 x∈[-1.861, 2.359] μ=-0.778 σ=0.450 cpu:0
+      Array[196, 3] n=588 x∈[-1.758, 2.379] μ=-0.838 σ=0.437 cpu:0
+      Array[196, 3] n=588 x∈[-1.656, 2.466] μ=-0.878 σ=0.415 cpu:0
+      Array[196, 3] n=588 x∈[-1.717, 2.448] μ=-0.882 σ=0.399 cpu:0
+      Array[196, 3] n=588 x∈[-1.717, 2.431] μ=-0.905 σ=0.408 cpu:0
+      Array[196, 3] n=588 x∈[-1.563, 2.448] μ=-0.859 σ=0.416 cpu:0
+      Array[196, 3] n=588 x∈[-1.475, 2.431] μ=-0.791 σ=0.463 cpu:0
+      Array[196, 3] n=588 x∈[-1.526, 2.429] μ=-0.759 σ=0.499 cpu:0
       ...
 
 ``` python
 # You can go deeper if you need to
 numbers[:3,:5,:3].deeper(2)
 ```
 
-    Array[3, 5, 3] n=45 x∈[-1.316, -0.197] μ=-0.593 σ=0.302 gpu:0
-      Array[5, 3] n=15 x∈[-0.985, -0.197] μ=-0.491 σ=0.267 gpu:0
-        Array[3] x∈[-0.672, -0.197] μ=-0.408 σ=0.197 gpu:0 [-0.354, -0.197, -0.672]
-        Array[3] x∈[-0.985, -0.197] μ=-0.507 σ=0.343 gpu:0 [-0.337, -0.197, -0.985]
-        Array[3] x∈[-0.881, -0.303] μ=-0.530 σ=0.252 gpu:0 [-0.405, -0.303, -0.881]
-        Array[3] x∈[-0.776, -0.303] μ=-0.506 σ=0.199 gpu:0 [-0.440, -0.303, -0.776]
-        Array[3] x∈[-0.916, -0.215] μ=-0.506 σ=0.298 gpu:0 [-0.388, -0.215, -0.916]
-      Array[5, 3] n=15 x∈[-1.212, -0.232] μ=-0.609 σ=0.302 gpu:0
-        Array[3] x∈[-0.724, -0.250] μ=-0.460 σ=0.197 gpu:0 [-0.405, -0.250, -0.724]
-        Array[3] x∈[-1.072, -0.232] μ=-0.576 σ=0.360 gpu:0 [-0.423, -0.232, -1.072]
-        Array[3] x∈[-0.968, -0.338] μ=-0.599 σ=0.268 gpu:0 [-0.491, -0.338, -0.968]
-        Array[3] x∈[-0.968, -0.408] μ=-0.651 σ=0.235 gpu:0 [-0.577, -0.408, -0.968]
-        Array[3] x∈[-1.212, -0.408] μ=-0.761 σ=0.336 gpu:0 [-0.662, -0.408, -1.212]
-      Array[5, 3] n=15 x∈[-1.316, -0.285] μ=-0.677 σ=0.306 gpu:0
-        Array[3] x∈[-0.828, -0.303] μ=-0.535 σ=0.219 gpu:0 [-0.474, -0.303, -0.828]
-        Array[3] x∈[-1.125, -0.285] μ=-0.628 σ=0.360 gpu:0 [-0.474, -0.285, -1.125]
-        Array[3] x∈[-1.020, -0.390] μ=-0.651 σ=0.268 gpu:0 [-0.542, -0.390, -1.020]
-        Array[3] x∈[-1.003, -0.478] μ=-0.708 σ=0.219 gpu:0 [-0.645, -0.478, -1.003]
-        Array[3] x∈[-1.316, -0.513] μ=-0.865 σ=0.336 gpu:0 [-0.765, -0.513, -1.316]
+    Array[3, 5, 3] n=45 x∈[-1.316, -0.197] μ=-0.593 σ=0.302 cpu:0
+      Array[5, 3] n=15 x∈[-0.985, -0.197] μ=-0.491 σ=0.267 cpu:0
+        Array[3] x∈[-0.672, -0.197] μ=-0.408 σ=0.197 cpu:0 [-0.354, -0.197, -0.672]
+        Array[3] x∈[-0.985, -0.197] μ=-0.507 σ=0.343 cpu:0 [-0.337, -0.197, -0.985]
+        Array[3] x∈[-0.881, -0.303] μ=-0.530 σ=0.252 cpu:0 [-0.405, -0.303, -0.881]
+        Array[3] x∈[-0.776, -0.303] μ=-0.506 σ=0.199 cpu:0 [-0.440, -0.303, -0.776]
+        Array[3] x∈[-0.916, -0.215] μ=-0.506 σ=0.298 cpu:0 [-0.388, -0.215, -0.916]
+      Array[5, 3] n=15 x∈[-1.212, -0.232] μ=-0.609 σ=0.302 cpu:0
+        Array[3] x∈[-0.724, -0.250] μ=-0.460 σ=0.197 cpu:0 [-0.405, -0.250, -0.724]
+        Array[3] x∈[-1.072, -0.232] μ=-0.576 σ=0.360 cpu:0 [-0.423, -0.232, -1.072]
+        Array[3] x∈[-0.968, -0.338] μ=-0.599 σ=0.268 cpu:0 [-0.491, -0.338, -0.968]
+        Array[3] x∈[-0.968, -0.408] μ=-0.651 σ=0.235 cpu:0 [-0.577, -0.408, -0.968]
+        Array[3] x∈[-1.212, -0.408] μ=-0.761 σ=0.336 cpu:0 [-0.662, -0.408, -1.212]
+      Array[5, 3] n=15 x∈[-1.316, -0.285] μ=-0.677 σ=0.306 cpu:0
+        Array[3] x∈[-0.828, -0.303] μ=-0.535 σ=0.219 cpu:0 [-0.474, -0.303, -0.828]
+        Array[3] x∈[-1.125, -0.285] μ=-0.628 σ=0.360 cpu:0 [-0.474, -0.285, -1.125]
+        Array[3] x∈[-1.020, -0.390] μ=-0.651 σ=0.268 cpu:0 [-0.542, -0.390, -1.020]
+        Array[3] x∈[-1.003, -0.478] μ=-0.708 σ=0.219 cpu:0 [-0.645, -0.478, -1.003]
+        Array[3] x∈[-1.316, -0.513] μ=-0.865 σ=0.336 cpu:0 [-0.765, -0.513, -1.316]
 
 ## Now in `.rgb` color
 
 The important queston - is it our man?
 
 ``` python
 numbers.rgb
 ```
 
-![](index_files/figure-gfm/cell-13-output-1.png)
+![](index_files/figure-commonmark/cell-13-output-1.png)
 
 *Maaaaybe?* Looks like someone normalized him.
 
 ``` python
 in_stats = ( (0.485, 0.456, 0.406),     # mean 
              (0.229, 0.224, 0.225) )    # std
 
 # numbers.rgb(in_stats, cl=True) # For channel-last input format
 numbers.rgb(in_stats)
 ```
 
-![](index_files/figure-gfm/cell-14-output-1.png)
+![](index_files/figure-commonmark/cell-14-output-1.png)
 
 It’s indeed our hero, the Tenchman!
 
 ## `.plt` the statistics
 
 ``` python
 (numbers+3).plt
 ```
 
-![](index_files/figure-gfm/cell-15-output-1.svg)
+![](index_files/figure-commonmark/cell-15-output-1.svg)
 
 ``` python
 (numbers+3).plt(center="mean", max_s=1000)
 ```
 
-![](index_files/figure-gfm/cell-16-output-1.svg)
+![](index_files/figure-commonmark/cell-16-output-1.svg)
 
 ``` python
 (numbers+3).plt(center="range")
 ```
 
-![](index_files/figure-gfm/cell-17-output-1.svg)
+![](index_files/figure-commonmark/cell-17-output-1.svg)
 
 ## See the `.chans`
 
 ``` python
 # .chans will map values betwen [-1,1] to colors.
 # Make our values fit into that range to avoid clipping.
 mean = jnp.array(in_stats[0])
 std = jnp.array(in_stats[1])
 numbers_01 = (numbers*std + mean)
 numbers_01
 ```
 
-    Array[196, 196, 3] n=115248 x∈[0., 1.000] μ=0.361 σ=0.248 gpu:0
+    Array[196, 196, 3] n=115248 (0.4Mb) x∈[0., 1.000] μ=0.361 σ=0.248 cpu:0
 
 ``` python
 numbers_01.chans
 ```
 
-![](index_files/figure-gfm/cell-19-output-1.png)
+![](index_files/figure-commonmark/cell-19-output-1.png)
 
 ## Grouping
 
 ``` python
 # Make 8 images with progressively higher brightness and stack them 2x2x2.
 eight_images = (jnp.stack([numbers]*8) + jnp.linspace(-2, 2, 8)[:,None,None,None])
 eight_images = (eight_images
                      *jnp.array(in_stats[1])
                      +jnp.array(in_stats[0])
                 ).clip(0,1).reshape(2,2,2,196,196,3)
 
 eight_images
 ```
 
-    Array[2, 2, 2, 196, 196, 3] n=921984 x∈[0., 1.000] μ=0.382 σ=0.319 gpu:0
+    Array[2, 2, 2, 196, 196, 3] n=921984 (3.5Mb) x∈[0., 1.000] μ=0.382 σ=0.319 cpu:0
 
 ``` python
 eight_images.rgb
 ```
 
-![](index_files/figure-gfm/cell-21-output-1.png)
+![](index_files/figure-commonmark/cell-21-output-1.png)
+
+## Sharding
+
+``` python
+assert jax.__version_info__[0] == 0
+if jax.__version_info__[1] >= 4:
+    from jax.sharding import PositionalSharding
+    from jax.experimental import mesh_utils
+    sharding = PositionalSharding(mesh_utils.create_device_mesh((4,2)))
+    x = jax.random.normal(jax.random.PRNGKey(0), (8192, 8192))
+    y = jax.device_put(x, sharding)
+
+    jax.debug.visualize_array_sharding(y)
+else:
+    # Note: Looks like ShardedDeviceArray needs an explicit device axis?
+    x = jax.random.normal(jax.random.PRNGKey(0), (8, 1024, 8192))
+    y = jax.device_put_sharded([x for x in x], jax.devices())
+
+print(x)
+print(y)
+```
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace"><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #393b79">            </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #d6616b">            </span>
+<span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #393b79">   CPU 0    </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #d6616b">   CPU 1    </span>
+<span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #393b79">            </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #d6616b">            </span>
+<span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #8ca252">            </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #de9ed6">            </span>
+<span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #8ca252">   CPU 2    </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #de9ed6">   CPU 3    </span>
+<span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #8ca252">            </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #de9ed6">            </span>
+<span style="color: #000000; text-decoration-color: #000000; background-color: #e7cb94">            </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #6b6ecf">            </span>
+<span style="color: #000000; text-decoration-color: #000000; background-color: #e7cb94">   CPU 4    </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #6b6ecf">   CPU 5    </span>
+<span style="color: #000000; text-decoration-color: #000000; background-color: #e7cb94">            </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #6b6ecf">            </span>
+<span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #a55194">            </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #8c6d31">            </span>
+<span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #a55194">   CPU 6    </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #8c6d31">   CPU 7    </span>
+<span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #a55194">            </span><span style="color: #ffffff; text-decoration-color: #ffffff; background-color: #8c6d31">            </span>
+</pre>
+
+    Array[8192, 8192] n=67108864 (0.2Gb) x∈[-5.420, 5.220] μ=-0.000 σ=1.000 cpu:0
+    Array[8192, 8192] n=67108864 (0.2Gb) x∈[-5.420, 5.220] μ=-0.000 σ=1.000 cpu:0,1,2,3,4,5,6,7
 
 ## Options \| [Docs](utils.config.html)
 
 ``` python
 from lovely_jax import set_config, config, lovely, get_config
 ```
 
 ``` python
 set_config(precision=5, sci_mode=True, color=False)
 jnp.array([1., 2, jnp.nan])
 ```
 
-    Array[3] μ=1.50000e+00 σ=5.00000e-01 NaN! gpu:0 [1.00000e+00, 2.00000e+00, nan]
+    Array[3] μ=1.50000e+00 σ=5.00000e-01 NaN! cpu:0 [1.00000e+00, 2.00000e+00, nan]
 
 ``` python
 set_config(precision=None, sci_mode=None, color=None) # None -> Reset to defaults
 ```
 
 ``` python
 print(jnp.array([1., 2]))
 # Or with config context manager.
 with config(sci_mode=True, precision=5):
     print(jnp.array([1., 2]))
 
 print(jnp.array([1., 2]))
 ```
 
-    Array[2] μ=1.500 σ=0.500 gpu:0 [1.000, 2.000]
-    Array[2] μ=1.50000e+00 σ=5.00000e-01 gpu:0 [1.00000e+00, 2.00000e+00]
-    Array[2] μ=1.500 σ=0.500 gpu:0 [1.000, 2.000]
+    Array[2] μ=1.500 σ=0.500 cpu:0 [1.000, 2.000]
+    Array[2] μ=1.50000e+00 σ=5.00000e-01 cpu:0 [1.00000e+00, 2.00000e+00]
+    Array[2] μ=1.500 σ=0.500 cpu:0 [1.000, 2.000]
 
 ## Without `.monkey_patch`
 
 ``` python
 lj.lovely(spicy)
 ```
 
-    Array[2, 6] n=12 x∈[-3.541e+03, -1.975e-05] μ=-393.848 σ=1.113e+03 +Inf! -Inf! NaN! gpu:0
+    Array[2, 6] n=12 x∈[-3.541e+03, -1.975e-05] μ=-393.848 σ=1.113e+03 +Inf! -Inf! NaN! cpu:0
 
 ``` python
 lj.lovely(spicy, verbose=True)
 ```
 
-    Array[2, 6] n=12 x∈[-3.541e+03, -1.975e-05] μ=-393.848 σ=1.113e+03 +Inf! -Inf! NaN! gpu:0
+    Array[2, 6] n=12 x∈[-3.541e+03, -1.975e-05] μ=-393.848 σ=1.113e+03 +Inf! -Inf! NaN! cpu:0
     Array([[-3.541e+03, -1.975e-05,        inf,       -inf,        nan, -9.853e-01],
            [-4.054e-01, -3.025e-01, -8.807e-01, -4.397e-01, -3.025e-01, -7.761e-01]], dtype=float32)
 
 ``` python
 lj.lovely(numbers, depth=1)
 ```
 
-    Array[196, 196, 3] n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073 gpu:0
-      Array[196, 3] n=588 x∈[-1.912, 2.411] μ=-0.728 σ=0.519 gpu:0
-      Array[196, 3] n=588 x∈[-1.861, 2.359] μ=-0.778 σ=0.450 gpu:0
-      Array[196, 3] n=588 x∈[-1.758, 2.379] μ=-0.838 σ=0.437 gpu:0
-      Array[196, 3] n=588 x∈[-1.656, 2.466] μ=-0.878 σ=0.415 gpu:0
-      Array[196, 3] n=588 x∈[-1.717, 2.448] μ=-0.882 σ=0.399 gpu:0
-      Array[196, 3] n=588 x∈[-1.717, 2.431] μ=-0.905 σ=0.408 gpu:0
-      Array[196, 3] n=588 x∈[-1.563, 2.448] μ=-0.859 σ=0.416 gpu:0
-      Array[196, 3] n=588 x∈[-1.475, 2.431] μ=-0.791 σ=0.463 gpu:0
-      Array[196, 3] n=588 x∈[-1.526, 2.429] μ=-0.759 σ=0.499 gpu:0
+    Array[196, 196, 3] n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073 cpu:0
+      Array[196, 3] n=588 x∈[-1.912, 2.411] μ=-0.728 σ=0.519 cpu:0
+      Array[196, 3] n=588 x∈[-1.861, 2.359] μ=-0.778 σ=0.450 cpu:0
+      Array[196, 3] n=588 x∈[-1.758, 2.379] μ=-0.838 σ=0.437 cpu:0
+      Array[196, 3] n=588 x∈[-1.656, 2.466] μ=-0.878 σ=0.415 cpu:0
+      Array[196, 3] n=588 x∈[-1.717, 2.448] μ=-0.882 σ=0.399 cpu:0
+      Array[196, 3] n=588 x∈[-1.717, 2.431] μ=-0.905 σ=0.408 cpu:0
+      Array[196, 3] n=588 x∈[-1.563, 2.448] μ=-0.859 σ=0.416 cpu:0
+      Array[196, 3] n=588 x∈[-1.475, 2.431] μ=-0.791 σ=0.463 cpu:0
+      Array[196, 3] n=588 x∈[-1.526, 2.429] μ=-0.759 σ=0.499 cpu:0
       ...
 
 ``` python
 lj.rgb(numbers, in_stats)
 ```
 
-![](index_files/figure-gfm/cell-29-output-1.png)
+![](index_files/figure-commonmark/cell-30-output-1.png)
 
 ``` python
 lj.plot(numbers, center="mean")
 ```
 
-![](index_files/figure-gfm/cell-30-output-1.svg)
+![](index_files/figure-commonmark/cell-31-output-1.svg)
 
 ``` python
 lj.chans(numbers_01)
 ```
 
-![](index_files/figure-gfm/cell-31-output-1.png)
+![](index_files/figure-commonmark/cell-32-output-1.png)
 
 ## Matplotlib integration \| [Docs](matplotlib.html)
 
 ``` python
 numbers.rgb(in_stats).fig # matplotlib figure
 ```
 
-![](index_files/figure-gfm/cell-32-output-1.svg)
+![](index_files/figure-commonmark/cell-33-output-1.png)
 
 ``` python
 (numbers*0.3+0.5).chans.fig # matplotlib figure
 ```
 
-![](index_files/figure-gfm/cell-33-output-1.svg)
+![](index_files/figure-commonmark/cell-34-output-1.png)
 
 ``` python
 numbers.plt.fig.savefig('pretty.svg') # Save it
 ```
 
 ``` python
 !file pretty.svg; rm pretty.svg
@@ -368,8 +428,8 @@
 ax3.set_axis_off()
 
 numbers_01.plt(ax=ax1)
 numbers_01.rgb(ax=ax2)
 numbers_01.chans(ax=ax3);
 ```
 
-![](index_files/figure-gfm/cell-36-output-1.svg)
+![](index_files/figure-commonmark/cell-37-output-1.png)
```

### Comparing `lovely-jax-0.1.1.dev0/lovely_jax/_modidx.py` & `lovely-jax-0.1.2/lovely_jax/_modidx.py`

 * *Files identical despite different names*

### Comparing `lovely-jax-0.1.1.dev0/lovely_jax/patch.py` & `lovely-jax-0.1.2/lovely_jax/patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/10_patch.ipynb.
 
 # %% auto 0
 __all__ = ['monkey_patch']
 
-# %% ../nbs/10_patch.ipynb 4
+# %% ../nbs/10_patch.ipynb 5
 import numpy as np
 import jax
 import jax.numpy as jnp
 from jax._src import array
 from fastcore.foundation import patch_to
 import matplotlib.pyplot as plt
 
 from .repr_str import StrProxy
 from .repr_rgb import RGBProxy
 from .repr_plt import PlotProxy
 from .repr_chans import ChanProxy
 
-# %% ../nbs/10_patch.ipynb 5
+# %% ../nbs/10_patch.ipynb 6
 def _monkey_patch(cls):
     "Monkey-patch lovely features into `cls`" 
 
     if not hasattr(cls, '_plain_repr'):
         cls._plain_repr = cls.__repr__
         cls._plain_str = cls.__str__
         cls._plain_format = cls.__format__
@@ -68,7 +68,12 @@
     def plt(t: jax.Array):
         return PlotProxy(t)
 
 
 def monkey_patch():
     _monkey_patch(array.ArrayImpl)
     _monkey_patch(array.DeviceArray)
+
+    # This was required for earlied version of jax 0.4.x
+    if hasattr(jax.pxla, '_ShardedDeviceArray'):
+        _monkey_patch(jax.pxla._ShardedDeviceArray)
+
```

### Comparing `lovely-jax-0.1.1.dev0/lovely_jax/repr_chans.py` & `lovely-jax-0.1.2/lovely_jax/repr_chans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/05_repr_chans.ipynb.
 
 # %% auto 0
 __all__ = ['chans']
 
-# %% ../nbs/05_repr_chans.ipynb 5
+# %% ../nbs/05_repr_chans.ipynb 4
 from typing import Any, Optional as O
 
 import jax, jax.numpy as jnp
 from matplotlib import pyplot as plt, axes, figure
 from IPython.core.pylabtools import print_figure
 
 from lovely_numpy.utils.utils import cached_property
```

### Comparing `lovely-jax-0.1.1.dev0/lovely_jax/repr_plt.py` & `lovely-jax-0.1.2/lovely_jax/repr_plt.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 from lovely_numpy.utils.utils import cached_property
 from lovely_numpy.repr_plt import fig_plot
 from lovely_numpy import config as np_config
 
 from .repr_str import to_str, pretty_str
 from .utils.misc import to_numpy
-from .utils.config import get_config
+from .utils.config import get_config, config
 
-# %% ../nbs/02_repr_plt.ipynb 5
+# %% ../nbs/02_repr_plt.ipynb 6
 # This is here for the monkey-patched tensor use case.
 # Gives the ability to call both .plt and .plt(ax=ax).  
 
 class PlotProxy(): 
     """Flexible `PIL.Image.Image` wrapper"""
 
     def __init__(self, x:jax.Array):
@@ -47,15 +47,15 @@
         return self
 
     @cached_property
     def fig(self) -> figure.Figure:
         cfg = get_config()
         with np_config( fig_close=cfg.fig_close,
                         fig_show=cfg.fig_show,
-                        plt_seed=cfg.plt_seed ):
+                        plt_seed=cfg.plt_seed ), config(show_mem_above=jnp.inf):
             return fig_plot( to_numpy(self.x),
                             summary=to_str(self.x, color=False),
                             **self.params)
 
     def _repr_png_(self):
         return print_figure(self.fig, fmt="png",
             metadata={"Software": "Matplotlib, https://matplotlib.org/"})
@@ -67,15 +67,15 @@
             "Creator": "Matplotlib, https://matplotlib.org/",
         }
         with rc_context({"svg.hashsalt": "1"}):
             svg_repr = print_figure(self.fig, fmt="svg", metadata=metadata)
         return svg_repr
 
 
-# %% ../nbs/02_repr_plt.ipynb 6
+# %% ../nbs/02_repr_plt.ipynb 7
 def plot(   x       :jax.Array, # Tensor to explore
             center  :str    ="zero",    # Center plot on  `zero`, `mean`, or `range`
             max_s   :int    =10000,     # Draw up to this many samples. =0 to draw all
             plt0    :Any    =True,      # Take zero values into account
             ax      :O[axes.Axes]=None  # Optionally provide a matplotlib axes.
         ) -> PlotProxy:
```

### Comparing `lovely-jax-0.1.1.dev0/lovely_jax/repr_rgb.py` & `lovely-jax-0.1.2/lovely_jax/repr_rgb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_repr_rgb.ipynb.
 
 # %% auto 0
 __all__ = ['rgb']
 
-# %% ../nbs/01_repr_rgb.ipynb 5
+# %% ../nbs/01_repr_rgb.ipynb 4
 from typing import Any, Optional as O
 
 
 from matplotlib import axes, figure
 from IPython.core.pylabtools import print_figure
 from PIL import Image
 import jax, jax.numpy as jnp
```

### Comparing `lovely-jax-0.1.1.dev0/lovely_jax/repr_str.py` & `lovely-jax-0.1.2/lovely_jax/repr_str.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 # %% ../nbs/00_repr_str.ipynb 5
 import warnings
 from typing import Union, Optional as O
 
 import numpy as np
 import jax, jax.numpy as jnp
 
-from lovely_numpy import np_to_str_common, pretty_str, sparse_join, ansi_color, in_debugger
+from lovely_numpy import np_to_str_common, pretty_str, sparse_join, ansi_color, in_debugger, bytes_to_human
 from lovely_numpy import config as lnp_config
 
-from .utils.config import get_config
+from .utils.config import get_config, config
 from .utils.misc import to_numpy, is_cpu, test_array_repr
 
 # %% ../nbs/00_repr_str.ipynb 8
 dtnames =   {   "float16": "f16",
                 "float32": "", # Default dtype in jax
                 "float64": "f64", 
                 "bfloat16": "bf16",
@@ -34,15 +34,15 @@
 def short_dtype(x: jax.Array) -> str:
     return dtnames.get(x.dtype.name, str(x.dtype))
 
 # %% ../nbs/00_repr_str.ipynb 10
 def plain_repr(x: jax.Array):
     "Pick the right function to get a plain repr"
     # assert isinstance(x, np.ndarray), f"expected np.ndarray but got {type(x)}" # Could be a sub-class.
-    return x._plain_repr() if hasattr(type(x), "_plain_repr") else repr(x)
+    return x._plain_repr() if hasattr(x, "_plain_repr") else repr(x)
 
 # def plain_str(x: torch.Tensor):
 #     "Pick the right function to get a plain str."
 #     # assert isinstance(x, np.ndarray), f"expected np.ndarray but got {type(x)}"
 #     return x._plain_str() if hasattr(type(x), "_plain_str") else str(x)
 
 # %% ../nbs/00_repr_str.ipynb 11
@@ -61,34 +61,28 @@
                         color=True,                     # ANSI color highlighting
                         ddof=0):                        # For "std" unbiasing
 
     if x.size == 0:
         return ansi_color("empty", "grey", color)
 
     zeros = ansi_color("all_zeros", "grey", color) if jnp.equal(x, 0.).all() and x.size > 1 else None
-    pinf = ansi_color("+Inf!", "red", color) if jnp.isposinf(x).any() else None
-    ninf = ansi_color("-Inf!", "red", color) if jnp.isneginf(x).any() else None
-    nan = ansi_color("NaN!", "red", color) if jnp.isnan(x).any() else None
+    # pinf = ansi_color("+Inf!", "red", color) if jnp.isposinf(x).any() else None
+    # ninf = ansi_color("-Inf!", "red", color) if jnp.isneginf(x).any() else None
+    # nan = ansi_color("NaN!", "red", color) if jnp.isnan(x).any() else None
 
-    attention = sparse_join([zeros,pinf,ninf,nan])
-    numel = f"n={x.size}" if x.size > 5 and max(x.shape) != x.size else None
+    # attention = sparse_join([zeros,pinf,ninf,nan])
 
     summary = None
     if not zeros and x.ndim > 0:
-        # Calculate stats on good values only.
-        # This is memory expensive, don't do it on GPU.
-        # We divert to numpy if there are any nasties in the data.
-        # gx = x[ jnp.isfinite(x) ]
-
         minmax = f"x∈[{pretty_str(x.min())}, {pretty_str(x.max())}]" if x.size > 2 else None
         meanstd = f"μ={pretty_str(x.mean())} σ={pretty_str(x.std(ddof=ddof))}" if x.size >= 2 else None
-        summary = sparse_join([numel, minmax, meanstd])
+        summary = sparse_join([minmax, meanstd])
 
 
-    return sparse_join([ summary, attention])
+    return sparse_join([ summary, zeros])
 
 # %% ../nbs/00_repr_str.ipynb 14
 def to_str(x: jax.Array,  # Input
             plain: bool=False,
             verbose: bool=False,
             depth=0,
             lvl=0,
@@ -96,27 +90,38 @@
 
     if plain:
         return plain_repr(x)
 
     conf = get_config()
 
     tname = type(x).__name__.split(".")[-1]
+    if tname in ("ArrayImpl"): tname = "Array"
     shape = str(list(x.shape)) if x.ndim else None
     type_str = sparse_join([tname, shape], sep="")
-    
 
-    dev = f"{x.device().platform}:{x.device().id}"
+    if hasattr(x, "devices"): # Unified Array (jax >= 0.4)
+        int_dev_ids = sorted([d.id for d in x.devices()])
+        ids = ",".join(map(str, int_dev_ids))
+        dev = f"{list(x.devices())[0].platform}:{ids}"
+    elif hasattr(x, "device"): # Old-style DeviceArray
+        dev = f"{x.device().platform}:{x.device().id}"
+    elif hasattr(x, "sharding"):
+        int_dev_ids = sorted([d.id for d in x.sharding.devices])
+        ids = ",".join(map(str, int_dev_ids))
+        dev = f"{x.sharding.devices[0].platform}:{ids}"
+    else:
+        assert 0, f"Weird input type={type(input)}, expecrted Array, DeviceArray, or ShardedDeviceArray"
+
     dtype = short_dtype(x)
     # grad_fn = t.grad_fn.name() if t.grad_fn else None
     # PyTorch does not want you to know, but all `grad_fn``
     # tensors actuall have `requires_grad=True`` too.
     # grad = "grad" if t.requires_grad else None 
     grad = grad_fn = None
 
-
     # For complex tensors, just show the shape / size part for now.
     if not jnp.iscomplexobj(x):
         if color is None: color=conf.color
         if in_debugger(): color = False
         # `lovely-numpy` is used to calculate stats when doing so on GPU would require
         # memory allocation (not float tensors, tensors with bad numbers), or if the
         # data is on CPU (because numpy is faster).
@@ -128,33 +133,40 @@
                         sci_mode=conf.sci_mode):
 
             if is_cpu(x) or is_nasty(x):
                 common = np_to_str_common(np.array(x), color=color)
             else:
                 common = jax_to_str_common(x, color=color)
 
+            numel = None
+            if x.shape and max(x.shape) != x.size:
+                numel = f"n={x.size}"
+                if get_config().show_mem_above <= x.nbytes:
+                    numel = sparse_join([numel, f"({bytes_to_human(x.nbytes)})"])
+            elif get_config().show_mem_above <= x.nbytes:
+                numel = bytes_to_human(x.nbytes)
+
             vals = pretty_str(x) if 0 < x.size <= 10 else None
-            res = sparse_join([type_str, dtype, common, grad, grad_fn, dev, vals])
+            res = sparse_join([type_str, dtype, numel, common, grad, grad_fn, dev, vals])
     else:
         res = plain_repr(x)
 
-
     if verbose:
         res += "\n" + plain_repr(x)
 
     if depth and x.ndim > 1:
+        with config(show_mem_above=jnp.inf):
+            deep_width = min((x.shape[0]), conf.deeper_width) # Print at most this many lines
+            deep_lines = [ " "*conf.indent*(lvl+1) + to_str(x[i,:], depth=depth-1, lvl=lvl+1)
+                                for i in range(deep_width)] 
 
-        deep_width = min((x.shape[0]), conf.deeper_width) # Print at most this many lines
-        deep_lines = [ " "*conf.indent*(lvl+1) + to_str(x[i,:], depth=depth-1, lvl=lvl+1)
-                            for i in range(deep_width)] 
-
-        # If we were limited by width, print ...
-        if deep_width < x.shape[0]: deep_lines.append(" "*conf.indent*(lvl+1) + "...")
+            # If we were limited by width, print ...
+            if deep_width < x.shape[0]: deep_lines.append(" "*conf.indent*(lvl+1) + "...")
 
-        res += "\n" + "\n".join(deep_lines)
+            res += "\n" + "\n".join(deep_lines)
 
     return res
 
 # %% ../nbs/00_repr_str.ipynb 15
 def history_warning():
     "Issue a warning (once) ifw e are running in IPYthon with output cache enabled"
```

### Comparing `lovely-jax-0.1.1.dev0/lovely_jax/utils/config.py` & `lovely-jax-0.1.2/lovely_jax/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/03a_utils.config.ipynb.
 
 # %% auto 0
 __all__ = ['set_config', 'get_config', 'config']
 
-# %% ../../nbs/03a_utils.config.ipynb 4
+# %% ../../nbs/03a_utils.config.ipynb 5
 from copy import copy
 from types import SimpleNamespace
 from typing import Optional, Union, Callable, TypeVar
 from contextlib import contextmanager
 from lovely_numpy import config as np_config
 
-# %% ../../nbs/03a_utils.config.ipynb 5
+# %% ../../nbs/03a_utils.config.ipynb 6
 class Config(SimpleNamespace):
     "Config"
     def __init__(self,
             precision     = 3,    # Digits after `.`
             threshold_max = 3,    # .abs() larger than 1e3 -> Sci mode
             threshold_min = -4,   # .abs() smaller that 1e-4 -> Sci mode
             sci_mode      = None, # Sci mode (2.3e4). None=auto
+            show_mem_above= 1024, # Show memory footprint above this size
             indent        = 2,    # Indent for .deeper()
             color         = True, # ANSI colors in text
             deeper_width  = 9,    # For .deeper, width per level
             plt_seed      = 42,   # Sampling seed for `plot`
             fig_close     = True, # Close matplotlib Figure
             fig_show      = False,# Call `plt.show()` for `.plt`, `.chans` and `.rgb`
 
     ):
         super().__init__(**{k:v for k,v in locals().items() if k not in ["self", "__class__"]})
 
 _defaults = Config()
 _config = copy(_defaults)
 
-# %% ../../nbs/03a_utils.config.ipynb 8
+# %% ../../nbs/03a_utils.config.ipynb 9
 # Allows passing None as an argument to reset the 
 class _Default():
     def __repr__(self):
         return "Ignore"
 D = _Default()
 Default = TypeVar("Default")
 
-# %% ../../nbs/03a_utils.config.ipynb 9
+# %% ../../nbs/03a_utils.config.ipynb 10
 def set_config( precision       :Optional[Union[Default,int]]  =D,
                 threshold_min   :Optional[Union[Default,int]]  =D,
                 threshold_max   :Optional[Union[Default,int]]  =D,
                 sci_mode        :Optional[Union[Default,bool]] =D,
+                show_mem_above  :Optional[Union[Default,int]]  =D,
                 indent          :Optional[Union[Default,bool]] =D,
                 color           :Optional[Union[Default,bool]] =D,
                 deeper_width    :Optional[Union[Default,int]]  =D,
                 plt_seed        :Optional[Union[Default,int]]  =D,
                 fig_close       :Optional[Union[Default,bool]] =D,
                 fig_show        :Optional[Union[Default,bool]] =D
                 ) -> None:
@@ -57,25 +59,26 @@
     for k,v in args.items():
         if v != D:
             if v is None:
                 setattr(_config, k, getattr(_defaults, k))
             else:
                 setattr(_config, k, v)
 
-# %% ../../nbs/03a_utils.config.ipynb 10
+# %% ../../nbs/03a_utils.config.ipynb 11
 def get_config():
     "Get a copy of config variables"
     return copy(_config)
 
-# %% ../../nbs/03a_utils.config.ipynb 11
+# %% ../../nbs/03a_utils.config.ipynb 12
 @contextmanager
 def config( precision       :Optional[Union[Default,int]]   =D,
             threshold_min   :Optional[Union[Default,int]]   =D,
             threshold_max   :Optional[Union[Default,int]]   =D,
             sci_mode        :Optional[Union[Default,bool]]  =D,
+            show_mem_above  :Optional[Union[Default,int]]   =D,
             indent          :Optional[Union[Default,bool]]  =D,
             color           :Optional[Union[Default,bool]]  =D,
             deeper_width    :Optional[Union[Default,int]]   =D,
             plt_seed        :Optional[Union[Default,int]]   =D,
             fig_close       :Optional[Union[Default,bool]]  =D,
             fig_show        :Optional[Union[Default,bool]]  =D
             ):
```

### Comparing `lovely-jax-0.1.1.dev0/settings.ini` & `lovely-jax-0.1.2/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = lovely-jax
 lib_name = %(repo)s
-version = 0.1.1-dev0
+version = 0.1.2
 min_python = 3.7
 license = mit
 
 ### nbdev ###
 doc_path = _docs
 lib_path = lovely_jax
 nbs_path = nbs
@@ -35,11 +35,11 @@
 language = English
 status = 3
 user = xl0
 
 ### Optional ###
 # Note: [cpu] for CI.
 # If you already have the cuda version installed, this will not override it.
-requirements = jax[cpu] lovely-numpy>=0.2.8.dev2
+requirements = jax[cpu] lovely-numpy>=0.2.9
 # pip_requirements =
 # dev_requirements =
 # console_scripts =
```

### Comparing `lovely-jax-0.1.1.dev0/setup.py` & `lovely-jax-0.1.2/setup.py`

 * *Files identical despite different names*


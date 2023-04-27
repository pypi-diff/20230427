# Comparing `tmp/lovely-numpy-0.2.9.tar.gz` & `tmp/lovely-numpy-0.2.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovely-numpy-0.2.9.tar", last modified: Thu Apr 27 10:06:39 2023, max compression
+gzip compressed data, was "lovely-numpy-0.2.9.dev1.tar", last modified: Wed Jan 11 11:14:20 2023, max compression
```

## Comparing `lovely-numpy-0.2.9.tar` & `lovely-numpy-0.2.9.dev1.tar`

### file list

```diff
@@ -1,31 +1,70 @@
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-04-27 10:06:39.640330 lovely-numpy-0.2.9/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1071 2023-03-12 08:33:02.000000 lovely-numpy-0.2.9/LICENSE
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      111 2023-03-12 08:33:02.000000 lovely-numpy-0.2.9/MANIFEST.in
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     9497 2023-04-27 10:06:39.640330 lovely-numpy-0.2.9/PKG-INFO
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     8761 2023-04-27 08:55:32.000000 lovely-numpy-0.2.9/README.md
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-04-27 10:06:39.640330 lovely-numpy-0.2.9/lovely_numpy/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      159 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/__init__.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    12300 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/_modidx.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     2431 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/lo.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     4552 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/repr_chans.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    10843 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/repr_plt.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     4932 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/repr_rgb.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     3271 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/repr_str.py
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-04-27 10:06:39.640330 lovely-numpy-0.2.9/lovely_numpy/utils/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       43 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/utils/__init__.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     2725 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/utils/colormap.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     4891 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/utils/config.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1430 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/utils/pad.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     3830 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/utils/tile2d.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     4925 2023-04-27 10:00:50.000000 lovely-numpy-0.2.9/lovely_numpy/utils/utils.py
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-04-27 10:06:39.640330 lovely-numpy-0.2.9/lovely_numpy.egg-info/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     9497 2023-04-27 10:06:39.000000 lovely-numpy-0.2.9/lovely_numpy.egg-info/PKG-INFO
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      648 2023-04-27 10:06:39.000000 lovely-numpy-0.2.9/lovely_numpy.egg-info/SOURCES.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2023-04-27 10:06:39.000000 lovely-numpy-0.2.9/lovely_numpy.egg-info/dependency_links.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       46 2023-04-27 10:06:39.000000 lovely-numpy-0.2.9/lovely_numpy.egg-info/entry_points.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2023-03-13 11:34:02.000000 lovely-numpy-0.2.9/lovely_numpy.egg-info/not-zip-safe
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       60 2023-04-27 10:06:39.000000 lovely-numpy-0.2.9/lovely_numpy.egg-info/requires.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       13 2023-04-27 10:06:39.000000 lovely-numpy-0.2.9/lovely_numpy.egg-info/top_level.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1095 2023-04-27 10:00:43.000000 lovely-numpy-0.2.9/settings.ini
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       38 2023-04-27 10:06:39.640330 lovely-numpy-0.2.9/setup.cfg
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     2577 2023-03-12 08:33:02.000000 lovely-numpy-0.2.9/setup.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:14:20.121522 lovely-numpy-0.2.9.dev1/
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:14:20.109522 lovely-numpy-0.2.9.dev1/.github/
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:14:20.109522 lovely-numpy-0.2.9.dev1/.github/workflows/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      194 2022-09-05 16:31:43.000000 lovely-numpy-0.2.9.dev1/.github/workflows/deploy.yaml
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      148 2022-09-05 16:31:43.000000 lovely-numpy-0.2.9.dev1/.github/workflows/test.yaml
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1812 2022-11-25 08:41:52.000000 lovely-numpy-0.2.9.dev1/.gitignore
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1071 2022-11-17 12:33:18.000000 lovely-numpy-0.2.9.dev1/LICENSE
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      111 2022-09-05 16:31:43.000000 lovely-numpy-0.2.9.dev1/MANIFEST.in
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     9372 2023-01-11 11:14:20.121522 lovely-numpy-0.2.9.dev1/PKG-INFO
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     8631 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/README.md
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:14:20.109522 lovely-numpy-0.2.9.dev1/index_files/
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:14:20.113522 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    13514 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-11-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    73300 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-12-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   184505 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-14-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   240952 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-16-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    41223 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-17-output-1.svg
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    36401 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-18-output-1.svg
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    51043 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-19-output-1.svg
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    73300 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-28-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   188991 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-29-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    50339 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-30-output-1.svg
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    99518 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-31-output-1.svg
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   390491 2023-01-11 10:47:14.000000 lovely-numpy-0.2.9.dev1/index_files/figure-gfm/cell-34-output-1.svg
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:14:20.113522 lovely-numpy-0.2.9.dev1/lovely_numpy/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      164 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/__init__.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    12059 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/_modidx.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2431 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/lo.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     4552 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/repr_chans.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    10814 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/repr_plt.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     4932 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/repr_rgb.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     3067 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/repr_str.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:14:20.113522 lovely-numpy-0.2.9.dev1/lovely_numpy/utils/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       43 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/utils/__init__.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2725 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/utils/colormap.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     4662 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/utils/config.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1430 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/utils/pad.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     3830 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/utils/tile2d.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     4610 2023-01-11 11:06:51.000000 lovely-numpy-0.2.9.dev1/lovely_numpy/utils/utils.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:14:20.113522 lovely-numpy-0.2.9.dev1/lovely_numpy.egg-info/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     9372 2023-01-11 11:14:19.000000 lovely-numpy-0.2.9.dev1/lovely_numpy.egg-info/PKG-INFO
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1624 2023-01-11 11:14:20.000000 lovely-numpy-0.2.9.dev1/lovely_numpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2023-01-11 11:14:19.000000 lovely-numpy-0.2.9.dev1/lovely_numpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       46 2023-01-11 11:14:19.000000 lovely-numpy-0.2.9.dev1/lovely_numpy.egg-info/entry_points.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2022-12-04 07:37:46.000000 lovely-numpy-0.2.9.dev1/lovely_numpy.egg-info/not-zip-safe
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       60 2023-01-11 11:14:19.000000 lovely-numpy-0.2.9.dev1/lovely_numpy.egg-info/requires.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       13 2023-01-11 11:14:19.000000 lovely-numpy-0.2.9.dev1/lovely_numpy.egg-info/top_level.txt
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:14:20.113522 lovely-numpy-0.2.9.dev1/misc/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1121 2022-12-25 06:33:25.000000 lovely-numpy-0.2.9.dev1/misc/test_matplotlib.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2023-01-11 11:14:20.121522 lovely-numpy-0.2.9.dev1/nbs/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    17231 2023-01-11 11:04:34.000000 lovely-numpy-0.2.9.dev1/nbs/00_repr_str.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   479649 2022-12-27 10:03:07.000000 lovely-numpy-0.2.9.dev1/nbs/01_repr_rgb.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   585392 2022-12-27 09:23:03.000000 lovely-numpy-0.2.9.dev1/nbs/02_repr_plt.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    12746 2023-01-11 11:04:34.000000 lovely-numpy-0.2.9.dev1/nbs/03_utils.utils.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)  1628982 2022-12-27 10:43:28.000000 lovely-numpy-0.2.9.dev1/nbs/03a_utils.colormap.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    94554 2022-12-06 07:51:29.000000 lovely-numpy-0.2.9.dev1/nbs/03b_utils.pad.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   191581 2022-12-07 09:44:30.000000 lovely-numpy-0.2.9.dev1/nbs/03c_utils.tile2d.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   239954 2022-12-27 09:23:03.000000 lovely-numpy-0.2.9.dev1/nbs/03d_utils.config.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)  1428171 2022-12-27 09:23:03.000000 lovely-numpy-0.2.9.dev1/nbs/05_repr_chans.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   243950 2023-01-11 10:47:10.000000 lovely-numpy-0.2.9.dev1/nbs/10_lo.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      556 2022-11-25 11:07:29.000000 lovely-numpy-0.2.9.dev1/nbs/_quarto.yml
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)  2163324 2023-01-11 10:47:10.000000 lovely-numpy-0.2.9.dev1/nbs/index.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)  1453145 2022-12-27 10:15:39.000000 lovely-numpy-0.2.9.dev1/nbs/matplotlib.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   461120 2022-11-17 13:20:47.000000 lovely-numpy-0.2.9.dev1/nbs/mysteryman.npy
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      219 2023-01-11 11:06:55.000000 lovely-numpy-0.2.9.dev1/nbs/nbdev.yml
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      528 2022-12-24 14:25:42.000000 lovely-numpy-0.2.9.dev1/nbs/sidebar.yml
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      612 2022-11-17 13:20:47.000000 lovely-numpy-0.2.9.dev1/nbs/styles.css
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1100 2023-01-11 11:06:08.000000 lovely-numpy-0.2.9.dev1/settings.ini
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       38 2023-01-11 11:14:20.121522 lovely-numpy-0.2.9.dev1/setup.cfg
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2577 2022-12-01 06:17:01.000000 lovely-numpy-0.2.9.dev1/setup.py
```

### Comparing `lovely-numpy-0.2.9/LICENSE` & `lovely-numpy-0.2.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `lovely-numpy-0.2.9/PKG-INFO` & `lovely-numpy-0.2.9.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lovely-numpy
-Version: 0.2.9
+Version: 0.2.9.dev1
 Summary: 💟 Lovely numpy
 Home-page: https://github.com/xl0/lovely-numpy
 Author: Alexey Zaytsev
 Author-email: alexey.zaytsev@gmail.com
 License: MIT License
 Keywords: jupyter numpy visualisation
 Classifier: Development Status :: 4 - Beta
@@ -91,15 +91,15 @@
 
 ## <code>Lo</code> and behold!
 
 ``` python
 lo(numbers)
 ```
 
-    array[196, 196, 3] f32 n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073
+    array[196, 196, 3] f32 n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073
 
 Better, eh?
 
 ``` python
 lo(numbers[1,:6,1]) # Still shows values if there are not too many.
 ```
 
@@ -120,15 +120,15 @@
 
     array[2, 6] f32 n=12 x∈[-3.541e+03, -3.369e-05] μ=-393.776 σ=1.113e+03 +Inf! -Inf! NaN!
 
 ``` python
 lo(np.zeros((10, 10))) # A zero array - make it obvious
 ```
 
-    array[10, 10] n=100 all_zeros
+    array[10, 10] all_zeros
 
 ``` python
 lo(spicy, verbose=True)
 ```
 
     array[2, 6] f32 n=12 x∈[-3.541e+03, -3.369e-05] μ=-393.776 σ=1.113e+03 +Inf! -Inf! NaN!
     array([[-3540.5432,    -0.    , ...,        nan,    -0.4054],
@@ -137,15 +137,15 @@
 
 ## Going `.deeper`
 
 ``` python
 lo(numbers.transpose(2,1,0)).deeper
 ```
 
-    array[3, 196, 196] f32 n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073
+    array[3, 196, 196] f32 n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073
       array[196, 196] f32 n=38416 x∈[-2.118, 2.249] μ=-0.324 σ=1.036
       array[196, 196] f32 n=38416 x∈[-1.966, 2.429] μ=-0.274 σ=0.973
       array[196, 196] f32 n=38416 x∈[-1.804, 2.640] μ=-0.567 σ=1.178
 
 ``` python
 # You can go deeper if you need to
 lo(numbers[:3,:4]).deeper(2)
@@ -172,89 +172,89 @@
 
 The important queston - is it our man?
 
 ``` python
 lo(numbers).rgb
 ```
 
-![](index_files/figure-commonmark/cell-11-output-1.png)
+![](index_files/figure-gfm/cell-11-output-1.png)
 
 *Maaaaybe?* Looks like someone normalized him.
 
 ``` python
 in_stats = ( (0.485, 0.456, 0.406),     # mean 
              (0.229, 0.224, 0.225) )    # std
 
 # numbers.rgb(in_stats, cl=True) # For channel-last input format
 lo(numbers).rgb(denorm=in_stats)
 ```
 
-![](index_files/figure-commonmark/cell-12-output-1.png)
+![](index_files/figure-gfm/cell-12-output-1.png)
 
 It’s indeed our hero, the Tenchman!
 
 ## See the `.chans`
 
 ``` python
 # .chans will map values betwen [-1,1] to colors.
 # Make our values fit into that range to avoid clipping.
 mean = np.array(in_stats[0])
 std = np.array(in_stats[1])
 numbers_01 = (numbers*std + mean).clip(0,1)
 lo(numbers_01)
 ```
 
-    array[196, 196, 3] n=115248 (0.9Mb) x∈[0., 1.000] μ=0.361 σ=0.248
+    array[196, 196, 3] n=115248 x∈[0., 1.000] μ=0.361 σ=0.248
 
 ``` python
 lo(numbers_01).chans
 ```
 
-![](index_files/figure-commonmark/cell-14-output-1.png)
+![](index_files/figure-gfm/cell-14-output-1.png)
 
 ## Grouping
 
 ``` python
 # Make 8 images with progressively higher brightness and stack them 2x2x2.
 eight_images = (np.stack([numbers]*8) + np.linspace(-2, 2, 8)[:,None,None,None])
 eight_images = (eight_images
                      *np.array(in_stats[1])
                      +np.array(in_stats[0])
                 ).clip(0,1).reshape(2,2,2,196,196,3)
             
 lo(eight_images)
 ```
 
-    array[2, 2, 2, 196, 196, 3] n=921984 (7.0Mb) x∈[0., 1.000] μ=0.382 σ=0.319
+    array[2, 2, 2, 196, 196, 3] n=921984 x∈[0., 1.000] μ=0.382 σ=0.319
 
 ``` python
 lo(eight_images).rgb
 ```
 
-![](index_files/figure-commonmark/cell-16-output-1.png)
+![](index_files/figure-gfm/cell-16-output-1.png)
 
 ## Histogram
 
 ``` python
 lo(numbers+3).plt
 ```
 
-![](index_files/figure-commonmark/cell-17-output-1.svg)
+![](index_files/figure-gfm/cell-17-output-1.svg)
 
 ``` python
 lo(numbers+3).plt(center="mean", max_s=1000)
 ```
 
-![](index_files/figure-commonmark/cell-18-output-1.svg)
+![](index_files/figure-gfm/cell-18-output-1.svg)
 
 ``` python
 lo(numbers+3).plt(center="range")
 ```
 
-![](index_files/figure-commonmark/cell-19-output-1.svg)
+![](index_files/figure-gfm/cell-19-output-1.svg)
 
 ## Options \| [Docs](03d_utils.config.html)
 
 ``` python
 from lovely_numpy import set_config, config, lovely
 ```
 
@@ -307,41 +307,41 @@
 ```
 
 ``` python
 lovely(numbers) # Returns `str`, that's why you see ''.
 # Note:  lo(x) returns a wrapper object with a `__repr__` and other methods.
 ```
 
-    'array[196, 196, 3] f32 n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073'
+    'array[196, 196, 3] f32 n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073'
 
 ``` python
 rgb(numbers, denorm=in_stats)
 ```
 
-![](index_files/figure-commonmark/cell-28-output-1.png)
+![](index_files/figure-gfm/cell-28-output-1.png)
 
 ``` python
 chans(numbers*0.3+0.5)
 ```
 
-![](index_files/figure-commonmark/cell-29-output-1.png)
+![](index_files/figure-gfm/cell-29-output-1.png)
 
 ``` python
 plot(numbers)
 ```
 
-![](index_files/figure-commonmark/cell-30-output-1.svg)
+![](index_files/figure-gfm/cell-30-output-1.svg)
 
 ## Matplotlib integration \| [Docs](matplotlib.html)
 
 ``` python
 lo(numbers).rgb(in_stats).fig # matplotlib figure
 ```
 
-![](index_files/figure-commonmark/cell-31-output-1.png)
+![](index_files/figure-gfm/cell-31-output-1.svg)
 
 ``` python
 lo(numbers).plt.fig.savefig('pretty.svg') # Save it
 ```
 
 ``` python
 !file pretty.svg; rm pretty.svg
@@ -361,8 +361,8 @@
 ax3.set_axis_off()
 
 lo(numbers_01).plt(ax=ax1)
 lo(numbers_01).rgb(ax=ax2)
 lo(numbers_01).chans(ax=ax3);
 ```
 
-![](index_files/figure-commonmark/cell-34-output-1.png)
+![](index_files/figure-gfm/cell-34-output-1.svg)
```

### Comparing `lovely-numpy-0.2.9/README.md` & `lovely-numpy-0.2.9.dev1/lovely_numpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: lovely-numpy
+Version: 0.2.9.dev1
+Summary: 💟 Lovely numpy
+Home-page: https://github.com/xl0/lovely-numpy
+Author: Alexey Zaytsev
+Author-email: alexey.zaytsev@gmail.com
+License: MIT License
+Keywords: jupyter numpy visualisation
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
 💟 Lovely NumPy
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 <div>
 
@@ -69,15 +91,15 @@
 
 ## <code>Lo</code> and behold!
 
 ``` python
 lo(numbers)
 ```
 
-    array[196, 196, 3] f32 n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073
+    array[196, 196, 3] f32 n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073
 
 Better, eh?
 
 ``` python
 lo(numbers[1,:6,1]) # Still shows values if there are not too many.
 ```
 
@@ -98,15 +120,15 @@
 
     array[2, 6] f32 n=12 x∈[-3.541e+03, -3.369e-05] μ=-393.776 σ=1.113e+03 +Inf! -Inf! NaN!
 
 ``` python
 lo(np.zeros((10, 10))) # A zero array - make it obvious
 ```
 
-    array[10, 10] n=100 all_zeros
+    array[10, 10] all_zeros
 
 ``` python
 lo(spicy, verbose=True)
 ```
 
     array[2, 6] f32 n=12 x∈[-3.541e+03, -3.369e-05] μ=-393.776 σ=1.113e+03 +Inf! -Inf! NaN!
     array([[-3540.5432,    -0.    , ...,        nan,    -0.4054],
@@ -115,15 +137,15 @@
 
 ## Going `.deeper`
 
 ``` python
 lo(numbers.transpose(2,1,0)).deeper
 ```
 
-    array[3, 196, 196] f32 n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073
+    array[3, 196, 196] f32 n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073
       array[196, 196] f32 n=38416 x∈[-2.118, 2.249] μ=-0.324 σ=1.036
       array[196, 196] f32 n=38416 x∈[-1.966, 2.429] μ=-0.274 σ=0.973
       array[196, 196] f32 n=38416 x∈[-1.804, 2.640] μ=-0.567 σ=1.178
 
 ``` python
 # You can go deeper if you need to
 lo(numbers[:3,:4]).deeper(2)
@@ -150,89 +172,89 @@
 
 The important queston - is it our man?
 
 ``` python
 lo(numbers).rgb
 ```
 
-![](index_files/figure-commonmark/cell-11-output-1.png)
+![](index_files/figure-gfm/cell-11-output-1.png)
 
 *Maaaaybe?* Looks like someone normalized him.
 
 ``` python
 in_stats = ( (0.485, 0.456, 0.406),     # mean 
              (0.229, 0.224, 0.225) )    # std
 
 # numbers.rgb(in_stats, cl=True) # For channel-last input format
 lo(numbers).rgb(denorm=in_stats)
 ```
 
-![](index_files/figure-commonmark/cell-12-output-1.png)
+![](index_files/figure-gfm/cell-12-output-1.png)
 
 It’s indeed our hero, the Tenchman!
 
 ## See the `.chans`
 
 ``` python
 # .chans will map values betwen [-1,1] to colors.
 # Make our values fit into that range to avoid clipping.
 mean = np.array(in_stats[0])
 std = np.array(in_stats[1])
 numbers_01 = (numbers*std + mean).clip(0,1)
 lo(numbers_01)
 ```
 
-    array[196, 196, 3] n=115248 (0.9Mb) x∈[0., 1.000] μ=0.361 σ=0.248
+    array[196, 196, 3] n=115248 x∈[0., 1.000] μ=0.361 σ=0.248
 
 ``` python
 lo(numbers_01).chans
 ```
 
-![](index_files/figure-commonmark/cell-14-output-1.png)
+![](index_files/figure-gfm/cell-14-output-1.png)
 
 ## Grouping
 
 ``` python
 # Make 8 images with progressively higher brightness and stack them 2x2x2.
 eight_images = (np.stack([numbers]*8) + np.linspace(-2, 2, 8)[:,None,None,None])
 eight_images = (eight_images
                      *np.array(in_stats[1])
                      +np.array(in_stats[0])
                 ).clip(0,1).reshape(2,2,2,196,196,3)
             
 lo(eight_images)
 ```
 
-    array[2, 2, 2, 196, 196, 3] n=921984 (7.0Mb) x∈[0., 1.000] μ=0.382 σ=0.319
+    array[2, 2, 2, 196, 196, 3] n=921984 x∈[0., 1.000] μ=0.382 σ=0.319
 
 ``` python
 lo(eight_images).rgb
 ```
 
-![](index_files/figure-commonmark/cell-16-output-1.png)
+![](index_files/figure-gfm/cell-16-output-1.png)
 
 ## Histogram
 
 ``` python
 lo(numbers+3).plt
 ```
 
-![](index_files/figure-commonmark/cell-17-output-1.svg)
+![](index_files/figure-gfm/cell-17-output-1.svg)
 
 ``` python
 lo(numbers+3).plt(center="mean", max_s=1000)
 ```
 
-![](index_files/figure-commonmark/cell-18-output-1.svg)
+![](index_files/figure-gfm/cell-18-output-1.svg)
 
 ``` python
 lo(numbers+3).plt(center="range")
 ```
 
-![](index_files/figure-commonmark/cell-19-output-1.svg)
+![](index_files/figure-gfm/cell-19-output-1.svg)
 
 ## Options \| [Docs](03d_utils.config.html)
 
 ``` python
 from lovely_numpy import set_config, config, lovely
 ```
 
@@ -285,41 +307,41 @@
 ```
 
 ``` python
 lovely(numbers) # Returns `str`, that's why you see ''.
 # Note:  lo(x) returns a wrapper object with a `__repr__` and other methods.
 ```
 
-    'array[196, 196, 3] f32 n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073'
+    'array[196, 196, 3] f32 n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073'
 
 ``` python
 rgb(numbers, denorm=in_stats)
 ```
 
-![](index_files/figure-commonmark/cell-28-output-1.png)
+![](index_files/figure-gfm/cell-28-output-1.png)
 
 ``` python
 chans(numbers*0.3+0.5)
 ```
 
-![](index_files/figure-commonmark/cell-29-output-1.png)
+![](index_files/figure-gfm/cell-29-output-1.png)
 
 ``` python
 plot(numbers)
 ```
 
-![](index_files/figure-commonmark/cell-30-output-1.svg)
+![](index_files/figure-gfm/cell-30-output-1.svg)
 
 ## Matplotlib integration \| [Docs](matplotlib.html)
 
 ``` python
 lo(numbers).rgb(in_stats).fig # matplotlib figure
 ```
 
-![](index_files/figure-commonmark/cell-31-output-1.png)
+![](index_files/figure-gfm/cell-31-output-1.svg)
 
 ``` python
 lo(numbers).plt.fig.savefig('pretty.svg') # Save it
 ```
 
 ``` python
 !file pretty.svg; rm pretty.svg
@@ -339,8 +361,8 @@
 ax3.set_axis_off()
 
 lo(numbers_01).plt(ax=ax1)
 lo(numbers_01).rgb(ax=ax2)
 lo(numbers_01).chans(ax=ax3);
 ```
 
-![](index_files/figure-commonmark/cell-34-output-1.png)
+![](index_files/figure-gfm/cell-34-output-1.svg)
```

### Comparing `lovely-numpy-0.2.9/lovely_numpy/_modidx.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,14 @@
                                                                                       'lovely_numpy/utils/tile2d.py'),
                                            'lovely_numpy.utils.tile2d.hypertile': ( 'utils.tile2d.html#hypertile',
                                                                                     'lovely_numpy/utils/tile2d.py'),
                                            'lovely_numpy.utils.tile2d.tile2d': ( 'utils.tile2d.html#tile2d',
                                                                                  'lovely_numpy/utils/tile2d.py')},
             'lovely_numpy.utils.utils': { 'lovely_numpy.utils.utils.ansi_color': ( 'utils.utils.html#ansi_color',
                                                                                    'lovely_numpy/utils/utils.py'),
-                                          'lovely_numpy.utils.utils.bytes_to_human': ( 'utils.utils.html#bytes_to_human',
-                                                                                       'lovely_numpy/utils/utils.py'),
                                           'lovely_numpy.utils.utils.history_warning': ( 'utils.utils.html#history_warning',
                                                                                         'lovely_numpy/utils/utils.py'),
                                           'lovely_numpy.utils.utils.in_debugger': ( 'utils.utils.html#in_debugger',
                                                                                     'lovely_numpy/utils/utils.py'),
                                           'lovely_numpy.utils.utils.np_to_str_common': ( 'utils.utils.html#np_to_str_common',
                                                                                          'lovely_numpy/utils/utils.py'),
                                           'lovely_numpy.utils.utils.pretty_str': ( 'utils.utils.html#pretty_str',
```

### Comparing `lovely-numpy-0.2.9/lovely_numpy/lo.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/lo.py`

 * *Files identical despite different names*

### Comparing `lovely-numpy-0.2.9/lovely_numpy/repr_chans.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/repr_chans.py`

 * *Files identical despite different names*

### Comparing `lovely-numpy-0.2.9/lovely_numpy/repr_plt.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/repr_plt.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from matplotlib import pyplot as plt, axes, figure, rc_context
 from IPython.core.pylabtools import print_figure
 
 from .repr_str import lovely, pretty_str
 from .utils import get_config, config
 from .utils.utils import cached_property
 
+
 # %% ../nbs/02_repr_plt.ipynb 4
 def normal_pdf( x   :np.ndarray,
                 mean:Union[np.ndarray, float] =0.,
                 std :Union[np.ndarray, float] =1.):
     r"""Probability Distribution Function of Normal Distribution:
         $$f(x, \mu, \sigma)
         = \dfrac{1}
@@ -45,14 +46,15 @@
     # Samples up to max_s elements and returns
     #   - samples from x
     #   - original x min (None = no good numbes in x)
     #   - original x max (None = no good numbes in x)
     
     # Ignore NaN and Inf.
     x = x[ np.isfinite(x) ]
+
     x_min = x_max = None
 
     if x.size: 
         x_min, x_max = x.min(), x.max()
         
         # An option to ignore zeros
         if not plt0: x = x[x != 0.]
@@ -191,15 +193,14 @@
 # %% ../nbs/02_repr_plt.ipynb 12
 def plot_str(t_str, ax):
     xlim = ax.get_xlim()
     ylim = ax.get_ylim()
     ax.text(xlim[0], ylim[1]*1.05, s=t_str)
 
 # %% ../nbs/02_repr_plt.ipynb 13
-@config(show_mem_above=np.inf)
 def fig_plot(   x     :np.ndarray,  # 
                 center  :str    ="zero",        # Center plot on  `zero`, `mean`, or `range`
                 max_s   :int    =10000,         # Draw up to this many samples. =0 to draw all
                 plt0    :Any    =True,          # Take zero values into account
                 ax      :O[axes.Axes]=None,     # Optionally, supply your own matplotlib axes.
                 summary :O[str] =None,          # Summary string (to display on top). None=str(lovely(x))
                 ddof    :int    =0,             # Apply bias correction to std
```

### Comparing `lovely-numpy-0.2.9/lovely_numpy/repr_rgb.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/repr_rgb.py`

 * *Files identical despite different names*

### Comparing `lovely-numpy-0.2.9/lovely_numpy/repr_str.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/repr_str.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # %% ../nbs/00_repr_str.ipynb 4
 from typing import Union, Optional as O
 from collections import defaultdict
 from fastcore.foundation import store_attr
 import warnings
 import numpy as np
 
-from .utils import pretty_str, sparse_join, np_to_str_common, in_debugger, bytes_to_human
+from .utils import pretty_str, sparse_join, np_to_str_common, in_debugger
 from .utils.config import get_config, set_config, config
 
 # %% ../nbs/00_repr_str.ipynb 6
 dtnames =   {   "float16": "f16",
                 "float32": "f32",
                 "float64": "", # Default dtype in numpy
                 "uint8": "u8",
@@ -57,37 +57,32 @@
         tname = "array" if type(x) == np.ndarray else type(x).__name__.split(".")[-1]
 
     shape = str(list(x.shape)) if x.ndim else None
     type_str = sparse_join([tname, shape], sep="")
 
     color = get_config().color if color is None else color
     if in_debugger(): color = False
-
-    numel = None
-    if x.shape and max(x.shape) != x.size:
-        numel = f"n={x.size}"
-        if get_config().show_mem_above <= x.nbytes:
-            numel = sparse_join([numel, f"({bytes_to_human(x.nbytes)})"])
-    elif get_config().show_mem_above <= x.nbytes:
-        numel = bytes_to_human(x.nbytes)
-
     common = np_to_str_common(x, color=color)
     dtype = short_dtype(x)
     
     vals = pretty_str(x) if 0 < x.size <= 10 else None
-    res = sparse_join([type_str, dtype, numel, common, vals])
+    res = sparse_join([type_str, dtype, common, vals])
 
     if verbose:
         res += "\n" + plain_repr(x)
 
     if depth and x.ndim > 1:
         deep_width = min(x.shape[0], conf.deeper_width) # Print at most this many lines
-        with config(show_mem_above=np.inf):
-            deep_lines = [ " "*conf.indent*(lvl+1) + lovely(x[i,:], depth=depth-1, lvl=lvl+1)
-                                for i in range(deep_width)]
+        deep_lines = [ " "*conf.indent*(lvl+1) + lovely(x[i,:], depth=depth-1, lvl=lvl+1)
+                            for i in range(deep_width)]
+
+        # If we were limited by width, print ...
+        if deep_width < x.shape[0]: deep_lines.append(" "*conf.indent*(lvl+1) + "...")
 
-            # If we were limited by width, print ...
-            if deep_width < x.shape[0]: deep_lines.append(" "*conf.indent*(lvl+1) + "...")
+        res += "\n" + "\n".join(deep_lines)
 
-            res += "\n" + "\n".join(deep_lines)
+        # res += "\n" + "\n".join([
+        #     " " * get_config().indent * (lvl+1) +
+        #     str(lovely(x[i,:], depth=depth-1, lvl=lvl+1))
+        #     for i in range(x.shape[0])])
 
     return res
```

### Comparing `lovely-numpy-0.2.9/lovely_numpy/utils/colormap.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `lovely-numpy-0.2.9/lovely_numpy/utils/config.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/utils/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 class Config(SimpleNamespace):
     "Config"
     def __init__(self,
             precision     = 3,    # Digits after `.`
             threshold_max = 3,    # .abs() larger than 1e3 -> Sci mode
             threshold_min = -4,   # .abs() smaller that 1e-4 -> Sci mode
             sci_mode      = None, # Sci mode (2.3e4). None=auto
-            show_mem_above= 1024, # Show memory usage in b/Kb/Mb/Gb if it's larger than this
             indent        = 2,    # Indent for .deeper()
             color         = True, # ANSI colors in text
             deeper_width  =9,     # For .deeper, width per level
             repr          = None, # Use func e.g. `lovely` for `repr(np.ndarray)`
             str           = None, # Use func e.g. `lovely` for `str(np.ndarray)`
             plt_seed      = 42,   # Sampling seed for `plot`
             fig_close     = True, # Close matplotlib Figure
@@ -43,15 +42,14 @@
 Default = TypeVar("Default")
 
 # %% ../../nbs/03d_utils.config.ipynb 9
 def set_config( precision       :Optional[Union[Default,int]]     =D,
                 threshold_min   :Optional[Union[Default,int]]     =D,
                 threshold_max   :Optional[Union[Default,int]]     =D,
                 sci_mode        :Optional[Union[Default,bool]]    =D,
-                show_mem_above  :Optional[Union[Default,bool]]    =D,
                 indent          :Optional[Union[Default,bool]]    =D,
                 color           :Optional[Union[Default,bool]]    =D,
                 deeper_width    :Optional[Union[Default,int]]     =D,
                 repr            :Optional[Union[Default,Callable]]=D,
                 str             :Optional[Union[Default,Callable]]=D,
                 plt_seed        :Optional[Union[Default,int]]     =D,
                 fig_close       :Optional[Union[Default,bool]]    =D,
@@ -88,15 +86,14 @@
 
 # %% ../../nbs/03d_utils.config.ipynb 11
 @contextmanager
 def config( precision       :Optional[Union[Default,int]]     =D,
             threshold_min   :Optional[Union[Default,int]]     =D,
             threshold_max   :Optional[Union[Default,int]]     =D,
             sci_mode        :Optional[Union[Default,bool]]    =D,
-            show_mem_above  :Optional[Union[Default,bool]]    =D,
             indent          :Optional[Union[Default,bool]]    =D,
             color           :Optional[Union[Default,bool]]    =D,
             deeper_width    :Optional[Union[Default,int]]     =D,
             repr            :Optional[Union[Default,Callable]]=D,
             str             :Optional[Union[Default,Callable]]=D,
             plt_seed        :Optional[Union[Default,int]]     =D,
             fig_close       :Optional[Union[Default,bool]]    =D,
```

### Comparing `lovely-numpy-0.2.9/lovely_numpy/utils/pad.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/utils/pad.py`

 * *Files identical despite different names*

### Comparing `lovely-numpy-0.2.9/lovely_numpy/utils/tile2d.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/utils/tile2d.py`

 * *Files identical despite different names*

### Comparing `lovely-numpy-0.2.9/lovely_numpy/utils/utils.py` & `lovely-numpy-0.2.9.dev1/lovely_numpy/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/03_utils.utils.ipynb.
 
 # %% auto 0
-__all__ = ['sci_mode', 'pretty_str', 'sparse_join', 'ansi_color', 'bytes_to_human', 'np_to_str_common', 'history_warning',
-           'in_debugger']
+__all__ = ['sci_mode', 'pretty_str', 'sparse_join', 'ansi_color', 'np_to_str_common', 'history_warning', 'in_debugger']
 
 # %% ../../nbs/03_utils.utils.ipynb 4
 import sys
 from collections import defaultdict
 import warnings
 import numpy as np
 from typing import Optional, Union
@@ -56,61 +55,48 @@
         style["grey"] = "\x1b[38;2;127;127;127m"
         style["red"] = "\x1b[31m"
         end_style = "\x1b[0m"
        
         return style[col]+s+end_style if use_color else s
 
 # %% ../../nbs/03_utils.utils.ipynb 18
-def bytes_to_human(num_bytes):
-    units = ['b', 'Kb', 'Mb', 'Gb']
-
-    value = num_bytes
-    for unit in units:
-        if value < 1024 / 10:
-            break
-        value /= 1024.0
-
-    if value % 1 == 0 or value >= 10:
-        return f"{round(value)}{unit}"
-    else:
-        return f"{value:.1f}{unit}"
-
-# %% ../../nbs/03_utils.utils.ipynb 20
 def np_to_str_common(x: Union[np.ndarray, np.generic],  # Input
                         color=True,                     # ANSI color highlighting
                         ddof=0):                        # For "std" unbiasing
-                        
+
     if x.size == 0:
         return ansi_color("empty", "grey", color)
 
     zeros = ansi_color("all_zeros", "grey", color) if np.equal(x, 0.).all() and x.size > 1 else None
     pinf = ansi_color("+Inf!", "red", color) if np.isposinf(x).any() else None
     ninf = ansi_color("-Inf!", "red", color) if np.isneginf(x).any() else None
     nan = ansi_color("NaN!", "red", color) if np.isnan(x).any() else None
 
     attention = sparse_join([zeros,pinf,ninf,nan])
+    numel = f"n={x.size}" if x.size > 5 and max(x.shape) != x.size else None
 
-    summary=None
+    summary = None
     if not zeros and isinstance(x, np.ndarray):
         # Calculate stats on good values only.
         gx = x[ np.isfinite(x) ]
 
         minmax = f"x∈[{pretty_str(gx.min())}, {pretty_str(gx.max())}]" if gx.size > 2 else None
         meanstd = f"μ={pretty_str(gx.mean())} σ={pretty_str(gx.std(ddof=ddof))}" if gx.size >= 2 else None
-        summary = sparse_join([minmax, meanstd])
+        summary = sparse_join([numel, minmax, meanstd])
+
 
     return sparse_join([ summary, attention])
 
-# %% ../../nbs/03_utils.utils.ipynb 24
+# %% ../../nbs/03_utils.utils.ipynb 22
 def history_warning():
     "Issue a warning (once) ifw e are running in IPYthon with output cache enabled"
     if "get_ipython" in globals() and get_ipython().cache_size > 0:
         warnings.warn("IPYthon has its output cache enabled. See https://xl0.github.io/lovely-tensors/history.html")
 
-# %% ../../nbs/03_utils.utils.ipynb 26
+# %% ../../nbs/03_utils.utils.ipynb 24
 # functools.cached_property is not available in python < 3.8
 
 assert sys.version_info.major == 3 # Python 4 some day?
 
 if sys.version_info.minor < 8:
     class cached_property:
         attrname: str
@@ -127,13 +113,13 @@
                 x = self.func(instance)
                 setattr(instance, "_cache_" + self.attrname, x)
                 return x
 else:
     from functools import cached_property
 
 
-# %% ../../nbs/03_utils.utils.ipynb 29
+# %% ../../nbs/03_utils.utils.ipynb 27
 def in_debugger():
     """Returns True if a debugger was used.
     
     Note: This funciton will keep returning True even after you exit the debugger."""
     return getattr(sys, "gettrace", None) and sys.gettrace() is not None
```

### Comparing `lovely-numpy-0.2.9/lovely_numpy.egg-info/PKG-INFO` & `lovely-numpy-0.2.9.dev1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: lovely-numpy
-Version: 0.2.9
-Summary: 💟 Lovely numpy
-Home-page: https://github.com/xl0/lovely-numpy
-Author: Alexey Zaytsev
-Author-email: alexey.zaytsev@gmail.com
-License: MIT License
-Keywords: jupyter numpy visualisation
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 💟 Lovely NumPy
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 <div>
 
@@ -91,15 +69,15 @@
 
 ## <code>Lo</code> and behold!
 
 ``` python
 lo(numbers)
 ```
 
-    array[196, 196, 3] f32 n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073
+    array[196, 196, 3] f32 n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073
 
 Better, eh?
 
 ``` python
 lo(numbers[1,:6,1]) # Still shows values if there are not too many.
 ```
 
@@ -120,15 +98,15 @@
 
     array[2, 6] f32 n=12 x∈[-3.541e+03, -3.369e-05] μ=-393.776 σ=1.113e+03 +Inf! -Inf! NaN!
 
 ``` python
 lo(np.zeros((10, 10))) # A zero array - make it obvious
 ```
 
-    array[10, 10] n=100 all_zeros
+    array[10, 10] all_zeros
 
 ``` python
 lo(spicy, verbose=True)
 ```
 
     array[2, 6] f32 n=12 x∈[-3.541e+03, -3.369e-05] μ=-393.776 σ=1.113e+03 +Inf! -Inf! NaN!
     array([[-3540.5432,    -0.    , ...,        nan,    -0.4054],
@@ -137,15 +115,15 @@
 
 ## Going `.deeper`
 
 ``` python
 lo(numbers.transpose(2,1,0)).deeper
 ```
 
-    array[3, 196, 196] f32 n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073
+    array[3, 196, 196] f32 n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073
       array[196, 196] f32 n=38416 x∈[-2.118, 2.249] μ=-0.324 σ=1.036
       array[196, 196] f32 n=38416 x∈[-1.966, 2.429] μ=-0.274 σ=0.973
       array[196, 196] f32 n=38416 x∈[-1.804, 2.640] μ=-0.567 σ=1.178
 
 ``` python
 # You can go deeper if you need to
 lo(numbers[:3,:4]).deeper(2)
@@ -172,89 +150,89 @@
 
 The important queston - is it our man?
 
 ``` python
 lo(numbers).rgb
 ```
 
-![](index_files/figure-commonmark/cell-11-output-1.png)
+![](index_files/figure-gfm/cell-11-output-1.png)
 
 *Maaaaybe?* Looks like someone normalized him.
 
 ``` python
 in_stats = ( (0.485, 0.456, 0.406),     # mean 
              (0.229, 0.224, 0.225) )    # std
 
 # numbers.rgb(in_stats, cl=True) # For channel-last input format
 lo(numbers).rgb(denorm=in_stats)
 ```
 
-![](index_files/figure-commonmark/cell-12-output-1.png)
+![](index_files/figure-gfm/cell-12-output-1.png)
 
 It’s indeed our hero, the Tenchman!
 
 ## See the `.chans`
 
 ``` python
 # .chans will map values betwen [-1,1] to colors.
 # Make our values fit into that range to avoid clipping.
 mean = np.array(in_stats[0])
 std = np.array(in_stats[1])
 numbers_01 = (numbers*std + mean).clip(0,1)
 lo(numbers_01)
 ```
 
-    array[196, 196, 3] n=115248 (0.9Mb) x∈[0., 1.000] μ=0.361 σ=0.248
+    array[196, 196, 3] n=115248 x∈[0., 1.000] μ=0.361 σ=0.248
 
 ``` python
 lo(numbers_01).chans
 ```
 
-![](index_files/figure-commonmark/cell-14-output-1.png)
+![](index_files/figure-gfm/cell-14-output-1.png)
 
 ## Grouping
 
 ``` python
 # Make 8 images with progressively higher brightness and stack them 2x2x2.
 eight_images = (np.stack([numbers]*8) + np.linspace(-2, 2, 8)[:,None,None,None])
 eight_images = (eight_images
                      *np.array(in_stats[1])
                      +np.array(in_stats[0])
                 ).clip(0,1).reshape(2,2,2,196,196,3)
             
 lo(eight_images)
 ```
 
-    array[2, 2, 2, 196, 196, 3] n=921984 (7.0Mb) x∈[0., 1.000] μ=0.382 σ=0.319
+    array[2, 2, 2, 196, 196, 3] n=921984 x∈[0., 1.000] μ=0.382 σ=0.319
 
 ``` python
 lo(eight_images).rgb
 ```
 
-![](index_files/figure-commonmark/cell-16-output-1.png)
+![](index_files/figure-gfm/cell-16-output-1.png)
 
 ## Histogram
 
 ``` python
 lo(numbers+3).plt
 ```
 
-![](index_files/figure-commonmark/cell-17-output-1.svg)
+![](index_files/figure-gfm/cell-17-output-1.svg)
 
 ``` python
 lo(numbers+3).plt(center="mean", max_s=1000)
 ```
 
-![](index_files/figure-commonmark/cell-18-output-1.svg)
+![](index_files/figure-gfm/cell-18-output-1.svg)
 
 ``` python
 lo(numbers+3).plt(center="range")
 ```
 
-![](index_files/figure-commonmark/cell-19-output-1.svg)
+![](index_files/figure-gfm/cell-19-output-1.svg)
 
 ## Options \| [Docs](03d_utils.config.html)
 
 ``` python
 from lovely_numpy import set_config, config, lovely
 ```
 
@@ -307,41 +285,41 @@
 ```
 
 ``` python
 lovely(numbers) # Returns `str`, that's why you see ''.
 # Note:  lo(x) returns a wrapper object with a `__repr__` and other methods.
 ```
 
-    'array[196, 196, 3] f32 n=115248 (0.4Mb) x∈[-2.118, 2.640] μ=-0.388 σ=1.073'
+    'array[196, 196, 3] f32 n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073'
 
 ``` python
 rgb(numbers, denorm=in_stats)
 ```
 
-![](index_files/figure-commonmark/cell-28-output-1.png)
+![](index_files/figure-gfm/cell-28-output-1.png)
 
 ``` python
 chans(numbers*0.3+0.5)
 ```
 
-![](index_files/figure-commonmark/cell-29-output-1.png)
+![](index_files/figure-gfm/cell-29-output-1.png)
 
 ``` python
 plot(numbers)
 ```
 
-![](index_files/figure-commonmark/cell-30-output-1.svg)
+![](index_files/figure-gfm/cell-30-output-1.svg)
 
 ## Matplotlib integration \| [Docs](matplotlib.html)
 
 ``` python
 lo(numbers).rgb(in_stats).fig # matplotlib figure
 ```
 
-![](index_files/figure-commonmark/cell-31-output-1.png)
+![](index_files/figure-gfm/cell-31-output-1.svg)
 
 ``` python
 lo(numbers).plt.fig.savefig('pretty.svg') # Save it
 ```
 
 ``` python
 !file pretty.svg; rm pretty.svg
@@ -361,8 +339,8 @@
 ax3.set_axis_off()
 
 lo(numbers_01).plt(ax=ax1)
 lo(numbers_01).rgb(ax=ax2)
 lo(numbers_01).chans(ax=ax3);
 ```
 
-![](index_files/figure-commonmark/cell-34-output-1.png)
+![](index_files/figure-gfm/cell-34-output-1.svg)
```

### Comparing `lovely-numpy-0.2.9/settings.ini` & `lovely-numpy-0.2.9.dev1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = lovely-numpy
 lib_name = lovely-numpy
-version = 0.2.9
+version = 0.2.9-dev1
 min_python = 3.7
 license = MIT
 
 ### nbdev ###
 doc_path = _docs
 lib_path = lovely_numpy
 nbs_path = nbs
```

### Comparing `lovely-numpy-0.2.9/setup.py` & `lovely-numpy-0.2.9.dev1/setup.py`

 * *Files identical despite different names*


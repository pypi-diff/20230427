# Comparing `tmp/lovely-tensors-0.1.8.tar.gz` & `tmp/lovely-tensors-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovely-tensors-0.1.8.tar", last modified: Fri Nov 25 11:19:56 2022, max compression
+gzip compressed data, was "lovely-tensors-0.1.9.tar", last modified: Sat Dec  3 02:46:34 2022, max compression
```

## Comparing `lovely-tensors-0.1.8.tar` & `lovely-tensors-0.1.9.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-11-25 11:19:56.935738 lovely-tensors-0.1.8/
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-11-25 11:19:56.919738 lovely-tensors-0.1.8/.github/
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-11-25 11:19:56.923738 lovely-tensors-0.1.8/.github/workflows/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      236 2022-10-23 06:08:14.000000 lovely-tensors-0.1.8/.github/workflows/deploy.yaml
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      148 2022-10-23 06:08:14.000000 lovely-tensors-0.1.8/.github/workflows/test.yaml
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1608 2022-10-23 06:08:14.000000 lovely-tensors-0.1.8/.gitignore
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1070 2022-11-12 13:14:09.000000 lovely-tensors-0.1.8/LICENSE
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      111 2022-10-23 06:08:14.000000 lovely-tensors-0.1.8/MANIFEST.in
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    10190 2022-11-25 11:19:56.935738 lovely-tensors-0.1.8/PKG-INFO
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     9437 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/README.md
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   304095 2022-11-05 11:00:36.000000 lovely-tensors-0.1.8/features.pt
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-11-25 11:19:56.919738 lovely-tensors-0.1.8/index_files/
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-11-25 11:19:56.927739 lovely-tensors-0.1.8/index_files/figure-gfm/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    78953 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-13-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    64824 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-14-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    25052 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-15-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    25818 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-16-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    24672 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-17-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   188168 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-19-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   659338 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-23-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   215482 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-25-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    26561 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-27-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   236049 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-28-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    14841 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-29-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    64824 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-33-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    25417 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-34-output-1.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   188168 2022-11-25 11:12:33.000000 lovely-tensors-0.1.8/index_files/figure-gfm/cell-35-output-1.png
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-11-25 11:19:56.927739 lovely-tensors-0.1.8/lovely_tensors/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      212 2022-11-25 11:11:35.000000 lovely-tensors-0.1.8/lovely_tensors/__init__.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     5810 2022-11-25 11:11:35.000000 lovely-tensors-0.1.8/lovely_tensors/_modidx.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1555 2022-11-25 11:11:35.000000 lovely-tensors-0.1.8/lovely_tensors/patch.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     2392 2022-11-25 11:11:35.000000 lovely-tensors-0.1.8/lovely_tensors/repr_chans.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     8000 2022-11-25 11:11:35.000000 lovely-tensors-0.1.8/lovely_tensors/repr_plt.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     2181 2022-11-25 11:11:35.000000 lovely-tensors-0.1.8/lovely_tensors/repr_rgb.py
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     3935 2022-11-25 11:11:35.000000 lovely-tensors-0.1.8/lovely_tensors/repr_str.py
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-11-25 11:19:56.927739 lovely-tensors-0.1.8/lovely_tensors/utils/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)        0 2022-11-25 11:11:35.000000 lovely-tensors-0.1.8/lovely_tensors/utils/__init__.py
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-11-25 11:19:56.927739 lovely-tensors-0.1.8/lovely_tensors.egg-info/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    10190 2022-11-25 11:19:56.000000 lovely-tensors-0.1.8/lovely_tensors.egg-info/PKG-INFO
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1497 2022-11-25 11:19:56.000000 lovely-tensors-0.1.8/lovely_tensors.egg-info/SOURCES.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2022-11-25 11:19:56.000000 lovely-tensors-0.1.8/lovely_tensors.egg-info/dependency_links.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       50 2022-11-25 11:19:56.000000 lovely-tensors-0.1.8/lovely_tensors.egg-info/entry_points.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2022-10-26 05:06:18.000000 lovely-tensors-0.1.8/lovely_tensors.egg-info/not-zip-safe
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       80 2022-11-25 11:19:56.000000 lovely-tensors-0.1.8/lovely_tensors.egg-info/requires.txt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       15 2022-11-25 11:19:56.000000 lovely-tensors-0.1.8/lovely_tensors.egg-info/top_level.txt
-drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-11-25 11:19:56.935738 lovely-tensors-0.1.8/nbs/
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    17033 2022-11-25 09:42:43.000000 lovely-tensors-0.1.8/nbs/00_repr_str.ipynb
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   735770 2022-11-25 09:42:43.000000 lovely-tensors-0.1.8/nbs/01_repr_rgb.ipynb
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   303581 2022-11-25 08:33:41.000000 lovely-tensors-0.1.8/nbs/02_repr_plt.ipynb
--rw-rw-r--   0 xl0       (1000) xl0       (1000)  1531278 2022-11-25 09:24:23.000000 lovely-tensors-0.1.8/nbs/05_repr_chans.ipynb
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   865116 2022-11-25 08:33:41.000000 lovely-tensors-0.1.8/nbs/10_patch.ipynb
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      578 2022-11-25 10:56:09.000000 lovely-tensors-0.1.8/nbs/_quarto.yml
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     4267 2022-11-16 08:19:01.000000 lovely-tensors-0.1.8/nbs/history.ipynb
--rw-rw-r--   0 xl0       (1000) xl0       (1000)  2474774 2022-11-25 11:09:49.000000 lovely-tensors-0.1.8/nbs/index.ipynb
--rw-rw-r--   0 xl0       (1000) xl0       (1000)   461739 2022-10-23 06:08:14.000000 lovely-tensors-0.1.8/nbs/mysteryman.pt
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      229 2022-11-25 11:11:39.000000 lovely-tensors-0.1.8/nbs/nbdev.yml
--rw-rw-r--   0 xl0       (1000) xl0       (1000)      335 2022-11-25 09:38:43.000000 lovely-tensors-0.1.8/nbs/sidebar.yml
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1506 2022-11-25 10:02:47.000000 lovely-tensors-0.1.8/nbs/styles.css
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    13697 2022-10-23 06:08:14.000000 lovely-tensors-0.1.8/nbs/tenchman.jpg
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    78953 2022-10-23 06:08:14.000000 lovely-tensors-0.1.8/normalized.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)    63926 2022-10-23 06:08:14.000000 lovely-tensors-0.1.8/rgb.png
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     1057 2022-11-25 09:36:21.000000 lovely-tensors-0.1.8/settings.ini
--rw-rw-r--   0 xl0       (1000) xl0       (1000)       38 2022-11-25 11:19:56.935738 lovely-tensors-0.1.8/setup.cfg
--rw-rw-r--   0 xl0       (1000) xl0       (1000)     2541 2022-10-23 06:08:14.000000 lovely-tensors-0.1.8/setup.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-12-03 02:46:34.290240 lovely-tensors-0.1.9/
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-12-03 02:46:34.278240 lovely-tensors-0.1.9/.github/
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-12-03 02:46:34.282240 lovely-tensors-0.1.9/.github/workflows/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      236 2022-10-23 06:08:14.000000 lovely-tensors-0.1.9/.github/workflows/deploy.yaml
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      148 2022-10-23 06:08:14.000000 lovely-tensors-0.1.9/.github/workflows/test.yaml
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1608 2022-10-23 06:08:14.000000 lovely-tensors-0.1.9/.gitignore
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1070 2022-11-12 13:14:09.000000 lovely-tensors-0.1.9/LICENSE
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      111 2022-11-26 10:31:22.000000 lovely-tensors-0.1.9/MANIFEST.in
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    10187 2022-12-03 02:46:34.290240 lovely-tensors-0.1.9/PKG-INFO
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     9434 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/README.md
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   304095 2022-11-05 11:00:36.000000 lovely-tensors-0.1.9/features.pt
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-12-03 02:46:34.278240 lovely-tensors-0.1.9/index_files/
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-12-03 02:46:34.282240 lovely-tensors-0.1.9/index_files/figure-gfm/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    78953 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-13-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    64824 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-14-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    25052 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-15-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    25818 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-16-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    24672 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-17-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   188168 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-19-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   659338 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-23-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   215482 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-25-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    26561 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-27-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   236049 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-28-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    14841 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-29-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    64824 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-33-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    25417 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-34-output-1.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   188168 2022-12-03 02:41:21.000000 lovely-tensors-0.1.9/index_files/figure-gfm/cell-35-output-1.png
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-12-03 02:46:34.286240 lovely-tensors-0.1.9/lovely_tensors/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      162 2022-12-03 02:41:12.000000 lovely-tensors-0.1.9/lovely_tensors/__init__.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     7324 2022-12-03 02:41:12.000000 lovely-tensors-0.1.9/lovely_tensors/_modidx.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1555 2022-12-03 02:41:12.000000 lovely-tensors-0.1.9/lovely_tensors/patch.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2419 2022-12-03 02:41:12.000000 lovely-tensors-0.1.9/lovely_tensors/repr_chans.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     8000 2022-12-03 02:41:12.000000 lovely-tensors-0.1.9/lovely_tensors/repr_plt.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2119 2022-12-03 02:41:12.000000 lovely-tensors-0.1.9/lovely_tensors/repr_rgb.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     6773 2022-12-03 02:41:12.000000 lovely-tensors-0.1.9/lovely_tensors/repr_str.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-12-03 02:46:34.286240 lovely-tensors-0.1.9/lovely_tensors/utils/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       22 2022-12-03 02:41:12.000000 lovely-tensors-0.1.9/lovely_tensors/utils/__init__.py
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2168 2022-12-03 02:41:12.000000 lovely-tensors-0.1.9/lovely_tensors/utils/config.py
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-12-03 02:46:34.286240 lovely-tensors-0.1.9/lovely_tensors.egg-info/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    10187 2022-12-03 02:46:34.000000 lovely-tensors-0.1.9/lovely_tensors.egg-info/PKG-INFO
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1554 2022-12-03 02:46:34.000000 lovely-tensors-0.1.9/lovely_tensors.egg-info/SOURCES.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2022-12-03 02:46:34.000000 lovely-tensors-0.1.9/lovely_tensors.egg-info/dependency_links.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       50 2022-12-03 02:46:34.000000 lovely-tensors-0.1.9/lovely_tensors.egg-info/entry_points.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)        1 2022-11-25 13:00:39.000000 lovely-tensors-0.1.9/lovely_tensors.egg-info/not-zip-safe
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       78 2022-12-03 02:46:34.000000 lovely-tensors-0.1.9/lovely_tensors.egg-info/requires.txt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       15 2022-12-03 02:46:34.000000 lovely-tensors-0.1.9/lovely_tensors.egg-info/top_level.txt
+drwxrwxr-x   0 xl0       (1000) xl0       (1000)        0 2022-12-03 02:46:34.290240 lovely-tensors-0.1.9/nbs/
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    22548 2022-12-03 02:41:16.000000 lovely-tensors-0.1.9/nbs/00_repr_str.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   735690 2022-12-01 13:47:01.000000 lovely-tensors-0.1.9/nbs/01_repr_rgb.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   303581 2022-11-25 08:33:41.000000 lovely-tensors-0.1.9/nbs/02_repr_plt.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     5462 2022-12-02 05:31:41.000000 lovely-tensors-0.1.9/nbs/03_utils.config.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)  1531314 2022-12-01 13:47:01.000000 lovely-tensors-0.1.9/nbs/05_repr_chans.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   865116 2022-12-03 02:42:06.000000 lovely-tensors-0.1.9/nbs/10_patch.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      578 2022-11-30 02:56:50.000000 lovely-tensors-0.1.9/nbs/_quarto.yml
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     4267 2022-11-16 08:19:01.000000 lovely-tensors-0.1.9/nbs/history.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)  2474771 2022-12-03 02:41:16.000000 lovely-tensors-0.1.9/nbs/index.ipynb
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)   461739 2022-10-23 06:08:14.000000 lovely-tensors-0.1.9/nbs/mysteryman.pt
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      229 2022-12-03 02:41:16.000000 lovely-tensors-0.1.9/nbs/nbdev.yml
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)      369 2022-12-02 05:13:07.000000 lovely-tensors-0.1.9/nbs/sidebar.yml
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1506 2022-11-30 02:56:50.000000 lovely-tensors-0.1.9/nbs/styles.css
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    13697 2022-10-23 06:08:14.000000 lovely-tensors-0.1.9/nbs/tenchman.jpg
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    78953 2022-10-23 06:08:14.000000 lovely-tensors-0.1.9/normalized.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)    63926 2022-10-23 06:08:14.000000 lovely-tensors-0.1.9/rgb.png
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     1055 2022-12-03 02:24:42.000000 lovely-tensors-0.1.9/settings.ini
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)       38 2022-12-03 02:46:34.290240 lovely-tensors-0.1.9/setup.cfg
+-rw-rw-r--   0 xl0       (1000) xl0       (1000)     2577 2022-12-01 11:21:10.000000 lovely-tensors-0.1.9/setup.py
```

### Comparing `lovely-tensors-0.1.8/.gitignore` & `lovely-tensors-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/LICENSE` & `lovely-tensors-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/PKG-INFO` & `lovely-tensors-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lovely-tensors
-Version: 0.1.8
+Version: 0.1.9
 Summary: ❤️ Lovely Tensors
 Home-page: https://github.com/xl0/lovely-tensors
 Author: Alexey Zaytsev
 Author-email: alexey.zaytsev@gmail.com
 License: MIT License
 Keywords: jupyter pytorch tensor visualisation
 Classifier: Development Status :: 4 - Beta
@@ -81,15 +81,15 @@
 import lovely_tensors as lt
 ```
 
 ``` python
 lt.monkey_patch()
 ```
 
-## `__repr__`
+## Summary
 
 ``` python
 numbers # torch.Tensor
 ```
 
     tensor[3, 196, 196] n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073
```

### Comparing `lovely-tensors-0.1.8/README.md` & `lovely-tensors-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 import lovely_tensors as lt
 ```
 
 ``` python
 lt.monkey_patch()
 ```
 
-## `__repr__`
+## Summary
 
 ``` python
 numbers # torch.Tensor
 ```
 
     tensor[3, 196, 196] n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073
```

### Comparing `lovely-tensors-0.1.8/features.pt` & `lovely-tensors-0.1.9/features.pt`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-13-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-13-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-14-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-14-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-15-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-15-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-16-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-16-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-17-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-17-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-19-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-19-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-23-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-23-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-25-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-25-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-27-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-27-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-28-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-28-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-29-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-29-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-33-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-33-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-34-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-34-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/index_files/figure-gfm/cell-35-output-1.png` & `lovely-tensors-0.1.9/index_files/figure-gfm/cell-35-output-1.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/lovely_tensors/_modidx.py` & `lovely-tensors-0.1.9/lovely_tensors/_modidx.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,12 +40,24 @@
                                                                                         'lovely_tensors/repr_str.py'),
                                          'lovely_tensors.repr_str.StrProxy.__init__': ( 'repr_str.html#strproxy.__init__',
                                                                                         'lovely_tensors/repr_str.py'),
                                          'lovely_tensors.repr_str.StrProxy.__repr__': ( 'repr_str.html#strproxy.__repr__',
                                                                                         'lovely_tensors/repr_str.py'),
                                          'lovely_tensors.repr_str.history_warning': ( 'repr_str.html#history_warning',
                                                                                       'lovely_tensors/repr_str.py'),
+                                         'lovely_tensors.repr_str.is_cpu': ('repr_str.html#is_cpu', 'lovely_tensors/repr_str.py'),
+                                         'lovely_tensors.repr_str.is_nasty': ('repr_str.html#is_nasty', 'lovely_tensors/repr_str.py'),
                                          'lovely_tensors.repr_str.lovely': ('repr_str.html#lovely', 'lovely_tensors/repr_str.py'),
+                                         'lovely_tensors.repr_str.plain_repr': ('repr_str.html#plain_repr', 'lovely_tensors/repr_str.py'),
+                                         'lovely_tensors.repr_str.plain_str': ('repr_str.html#plain_str', 'lovely_tensors/repr_str.py'),
                                          'lovely_tensors.repr_str.short_dtype': ('repr_str.html#short_dtype', 'lovely_tensors/repr_str.py'),
                                          'lovely_tensors.repr_str.to_str': ('repr_str.html#to_str', 'lovely_tensors/repr_str.py'),
+                                         'lovely_tensors.repr_str.torch_to_str_common': ( 'repr_str.html#torch_to_str_common',
+                                                                                          'lovely_tensors/repr_str.py'),
                                          'lovely_tensors.repr_str.type_to_dtype': ( 'repr_str.html#type_to_dtype',
-                                                                                    'lovely_tensors/repr_str.py')}}}
+                                                                                    'lovely_tensors/repr_str.py')},
+            'lovely_tensors.utils.config': { 'lovely_tensors.utils.config.config': ( 'utils.config.html#config',
+                                                                                     'lovely_tensors/utils/config.py'),
+                                             'lovely_tensors.utils.config.get_config': ( 'utils.config.html#get_config',
+                                                                                         'lovely_tensors/utils/config.py'),
+                                             'lovely_tensors.utils.config.set_config': ( 'utils.config.html#set_config',
+                                                                                         'lovely_tensors/utils/config.py')}}}
```

### Comparing `lovely-tensors-0.1.8/lovely_tensors/patch.py` & `lovely-tensors-0.1.9/lovely_tensors/patch.py`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/lovely_tensors/repr_chans.py` & `lovely-tensors-0.1.9/lovely_tensors/repr_chans.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,17 @@
                     cm_below=cm_below,
                     cm_above=cm_above,
                     cm_ninf=cm_ninf,
                     cm_pinf=cm_pinf,
                     cm_nan=cm_nan,
                     view_width=view_width,
                     gutter_px=gutter_px,
+                    frame_px=frame_px,
                     scale=scale,
-                    frame_px=frame_px)
+                    cl=cl)
 
 
 # %% ../nbs/05_repr_chans.ipynb 6
 class ChanProxy():
     def __init__(self, t: torch.Tensor):
         self.t = t
```

### Comparing `lovely-tensors-0.1.8/lovely_tensors/repr_plt.py` & `lovely-tensors-0.1.9/lovely_tensors/repr_plt.py`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/lovely_tensors/repr_rgb.py` & `lovely-tensors-0.1.9/lovely_tensors/repr_rgb.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,28 +32,26 @@
 # first case, the class defines `_repr_png_` to send the image to Jupyter. For
 # the later case, it defines __call__, which accps the argument.
 
 class RGBProxy():
     """Flexible `PIL.Image.Image` wrapper"""
     
     def __init__(self, t:torch.Tensor):
-        # super().__init__()
         assert t.ndim >= 3, f"Expecting at least 3 dimensions, got shape{t.shape}={t.dim()}"
-        self.t = t #.detach().cpu().numpy()
+        self.t = t
 
     def __call__(   self,
                     denorm=None,
                     cl=False,
                     gutter_px=3, frame_px=1,
                     scale=1,
                     view_width=966):
 
         return rgb(self.t, denorm=denorm, cl=cl, gutter_px=gutter_px,
-                frame_px=frame_px, view_width=view_width)
+                frame_px=frame_px, view_width=view_width, scale=scale)
     
-    @torch.no_grad()
     def _repr_png_(self):
         # Note: In order to prevernt IPYthon from hogging memory, we
         # delete the reference to the tensor after the first call to
         # `_repr_png_`. This is fine for Jupyter use.
         return self.__call__()._repr_png_()
```

### Comparing `lovely-tensors-0.1.8/lovely_tensors.egg-info/PKG-INFO` & `lovely-tensors-0.1.9/lovely_tensors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lovely-tensors
-Version: 0.1.8
+Version: 0.1.9
 Summary: ❤️ Lovely Tensors
 Home-page: https://github.com/xl0/lovely-tensors
 Author: Alexey Zaytsev
 Author-email: alexey.zaytsev@gmail.com
 License: MIT License
 Keywords: jupyter pytorch tensor visualisation
 Classifier: Development Status :: 4 - Beta
@@ -81,15 +81,15 @@
 import lovely_tensors as lt
 ```
 
 ``` python
 lt.monkey_patch()
 ```
 
-## `__repr__`
+## Summary
 
 ``` python
 numbers # torch.Tensor
 ```
 
     tensor[3, 196, 196] n=115248 x∈[-2.118, 2.640] μ=-0.388 σ=1.073
```

### Comparing `lovely-tensors-0.1.8/lovely_tensors.egg-info/SOURCES.txt` & `lovely-tensors-0.1.9/lovely_tensors.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,17 +34,19 @@
 lovely_tensors.egg-info/SOURCES.txt
 lovely_tensors.egg-info/dependency_links.txt
 lovely_tensors.egg-info/entry_points.txt
 lovely_tensors.egg-info/not-zip-safe
 lovely_tensors.egg-info/requires.txt
 lovely_tensors.egg-info/top_level.txt
 lovely_tensors/utils/__init__.py
+lovely_tensors/utils/config.py
 nbs/00_repr_str.ipynb
 nbs/01_repr_rgb.ipynb
 nbs/02_repr_plt.ipynb
+nbs/03_utils.config.ipynb
 nbs/05_repr_chans.ipynb
 nbs/10_patch.ipynb
 nbs/_quarto.yml
 nbs/history.ipynb
 nbs/index.ipynb
 nbs/mysteryman.pt
 nbs/nbdev.yml
```

### Comparing `lovely-tensors-0.1.8/nbs/00_repr_str.ipynb` & `lovely-tensors-0.1.9/nbs/00_repr_str.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722098808958246%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(3, '\\n'), (5, '\\n'), (6, '\\n'), (7, 'from lovely_numpy "*

 * *            "import np_to_str_common, pretty_str, sparse_join, ansi_color\\n'), (8, 'from "*

 * *            "lovely_numpy import config as lnp_config\\n'), (9, '\\n'), (10, 'from "*

 * *            "lovely_tensors.utils.config import get_config\\n')], delete: [6, 3, 2]}}, 6: "*

 * *            "{'source': {insert: [(6, '    return dtp')], delete: [6]}}, 15: {'source': {insert: "*

 * *            "[(12, '\\n'), (13, '    conf = g […]*

```diff
@@ -31,19 +31,23 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#| hide\n",
                 "#| export\n",
-                "from typing import Optional, Union\n",
-                "from collections import defaultdict\n",
                 "import warnings\n",
+                "\n",
                 "import torch\n",
-                "from lovely_numpy.utils import np_to_str_common, pretty_str, sparse_join, plain_repr, PRINT_OPTS"
+                "\n",
+                "\n",
+                "from lovely_numpy import np_to_str_common, pretty_str, sparse_join, ansi_color\n",
+                "from lovely_numpy import config as lnp_config\n",
+                "\n",
+                "from lovely_tensors.utils.config import get_config\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -77,15 +81,15 @@
             "source": [
                 "# |exporti\n",
                 "def type_to_dtype(t: str) -> torch.dtype:\n",
                 "    \"Convert str, e.g. 'float32' to torch.dtype e.g torch.float32\"\n",
                 "    \n",
                 "    dtp = vars(torch)[t]\n",
                 "    assert isinstance(dtp, torch.dtype)\n",
-                "    return dtp\n"
+                "    return dtp"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -129,55 +133,165 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# | exporti\n",
+                "def plain_repr(x: torch.Tensor):\n",
+                "    \"Pick the right function to get a plain repr\"\n",
+                "    # assert isinstance(x, np.ndarray), f\"expected np.ndarray but got {type(x)}\" # Could be a sub-class.\n",
+                "    return x._plain_repr() if hasattr(type(x), \"_plain_repr\") else repr(x)\n",
+                "\n",
+                "def plain_str(x: torch.Tensor):\n",
+                "    \"Pick the right function to get a plain str.\"\n",
+                "    # assert isinstance(x, np.ndarray), f\"expected np.ndarray but got {type(x)}\"\n",
+                "    return x._plain_str() if hasattr(type(x), \"_plain_str\") else str(x)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# | exporti\n",
+                "def is_nasty(t: torch.Tensor):\n",
+                "    \"\"\"Return true of any `t` values are inf or nan\"\"\"\n",
+                "    \n",
+                "    # Unlike .min()/.max(), amin/amax do not allocate extra GPU memory.\n",
+                "    t_min = t.amin()\n",
+                "    t_max = t.amax()\n",
+                "\n",
+                "    return (t_min.isnan() or t_min.isinf() or t_max.isinf()).item()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "#| hide\n",
+                "\n",
+                "test_eq(is_nasty(torch.tensor([1, 2, float(\"nan\")])), True)\n",
+                "test_eq(is_nasty(torch.tensor([1, 2, float(\"inf\")])), True)\n",
+                "test_eq(is_nasty(torch.tensor([1, 2, 3])), False)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# |exporti\n",
+                "\n",
+                "def torch_to_str_common(t: torch.Tensor,  # Input\n",
+                "                        color=True,       # ANSI color highlighting\n",
+                "                        ) -> str:\n",
+                "    \n",
+                "    amin, amax = t.amin(), t.amax()\n",
+                "\n",
+                "    zeros = ansi_color(\"all_zeros\", \"grey\", color) if amin.eq(0) and amax.eq(0) and t.numel() > 1 else None\n",
+                "    pinf = ansi_color(\"+Inf!\", \"red\", color) if amax.isposinf() else None\n",
+                "    ninf = ansi_color(\"-Inf!\", \"red\", color) if amin.isneginf() else None\n",
+                "    nan = ansi_color(\"NaN!\", \"red\", color) if amin.isnan() else None\n",
+                "\n",
+                "    attention = sparse_join([zeros,pinf,ninf,nan])\n",
+                "    numel = f\"n={t.numel()}\" if t.numel() > 5 and max(t.shape) != t.numel() else None\n",
+                "\n",
+                "    summary = None\n",
+                "    if not zeros:\n",
+                "        minmax = f\"x\u2208[{pretty_str(amin)}, {pretty_str(amax)}]\" if t.numel() > 2 else None\n",
+                "        meanstd = f\"\u03bc={pretty_str(t.mean())} \u03c3={pretty_str(t.std())}\" if t.numel() >= 2 else None\n",
+                "        summary = sparse_join([numel, minmax, meanstd])\n",
+                "\n",
+                "\n",
+                "    return sparse_join([ summary, attention])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# |exporti\n",
+                "# tensor.is_cpu was only introduced in 1.13.\n",
+                "def is_cpu(t: torch.Tensor):\n",
+                "    return t.device == torch.device(\"cpu\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "# |exporti\n",
                 "\n",
                 "@torch.no_grad()\n",
                 "def to_str(t: torch.Tensor,\n",
                 "            plain: bool=False,\n",
                 "            verbose: bool=False,\n",
                 "            depth=0,\n",
                 "            lvl=0,\n",
                 "            color=None) -> str:\n",
                 "\n",
                 "    if plain:\n",
                 "        return plain_repr(t)\n",
                 "\n",
+                "    conf = get_config()\n",
+                "\n",
                 "    tname = \"tensor\" if type(t) is torch.Tensor else type(t).__name__.split(\".\")[-1]\n",
                 "    shape = str(list(t.shape)) if t.ndim else None\n",
                 "    type_str = sparse_join([tname, shape], sep=\"\")\n",
                 "    \n",
                 "    dev = str(t.device) if t.device.type != \"cpu\" else None\n",
                 "    dtype = short_dtype(t)\n",
                 "    grad_fn = t.grad_fn.name() if t.grad_fn else None\n",
                 "    # PyTorch does not want you to know, but all `grad_fn``\n",
                 "    # tensors actuall have `requires_grad=True`` too.\n",
                 "    grad = \"grad\" if t.requires_grad else None \n",
                 "    \n",
                 "\n",
-                "    # Done with collecting torch-specific info. Pass it to Lovely-Numpy\n",
-                "    common=None\n",
-                "    vals=None\n",
+                "    # For complex tensors, just show the shape / size part for now.\n",
                 "    if not t.is_complex():\n",
-                "        common = np_to_str_common(t.cpu().numpy(), color=color, ddof=1)\n",
-                "        vals = pretty_str(t.cpu().numpy()) if t.numel() <= 10 else None\n",
+                "        color = conf.color if color is None else color\n",
+                "        # `lovely-numpy` is used to calculate stats when doing so on GPU would require\n",
+                "        # memory allocation (not float tensors, tensors with bad numbers), or if the\n",
+                "        # data is on CPU (because numpy is faster).\n",
+                "        #\n",
+                "        # Temporarily set the numpy config to match our config for consistency.\n",
+                "        with lnp_config(precision=conf.precision,\n",
+                "                        threshold_min=conf.threshold_min,\n",
+                "                        threshold_max=conf.threshold_max,\n",
+                "                        sci_mode=conf.sci_mode,\n",
+                "                        color=color):\n",
+                "\n",
+                "            if is_cpu(t) or is_nasty(t) or not t.is_floating_point():\n",
+                "                common = np_to_str_common(t.detach().cpu().numpy(), color=color, ddof=1)\n",
+                "            else:\n",
+                "                common = torch_to_str_common(t, color=color)\n",
+                "\n",
+                "            vals = pretty_str(t.cpu().numpy()) if t.numel() <= 10 else None\n",
+                "            res = sparse_join([type_str, dtype, common, grad, grad_fn, dev, vals])\n",
+                "    else:\n",
+                "        res = plain_repr(t)\n",
                 "\n",
-                "    res = sparse_join([type_str, dtype, common, grad, grad_fn, dev, vals])\n",
                 "\n",
-                "    if verbose or t.is_complex():\n",
+                "    if verbose:\n",
                 "        res += \"\\n\" + plain_repr(t)\n",
                 "\n",
                 "    if depth and t.dim() > 1:\n",
                 "        res += \"\\n\" + \"\\n\".join([\n",
-                "            \" \"*PRINT_OPTS.indent*(lvl+1) +\n",
-                "            str(StrProxy(t[i,:], depth=depth-1, lvl=lvl+1))\n",
+                "            \" \"*conf.indent*(lvl+1) +\n",
+                "            str(StrProxy(t[i,:], depth=depth-1, lvl=lvl+1)) # XXX use to_str\n",
                 "            for i in range(t.shape[0])])\n",
                 "\n",
                 "    return res"
             ]
         },
         {
             "cell_type": "code",
@@ -198,15 +312,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/tmp/ipykernel_751009/3648473780.py:6: UserWarning: IPYthon has its output cache enabled. See https://xl0.github.io/lovely-tensors/history.html\n",
+                        "/tmp/ipykernel_1413323/3648473780.py:6: UserWarning: IPYthon has its output cache enabled. See https://xl0.github.io/lovely-tensors/history.html\n",
                         "  warnings.warn(\"IPYthon has its output cache enabled. See https://xl0.github.io/lovely-tensors/history.html\")\n"
                     ]
                 }
             ],
             "source": [
                 "# |hide\n",
                 "get_ipython().cache_size=1000\n",
@@ -263,14 +377,21 @@
                 "            plain=False,    # Just print if exactly as before\n",
                 "            depth=0,        # Show stats in depth\n",
                 "            color=None):    # Force color (True/False) or auto.\n",
                 "    return StrProxy(t, verbose=verbose, plain=plain, depth=depth, color=color)"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Examples"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -282,28 +403,28 @@
                     ]
                 }
             ],
             "source": [
                 "print(lovely(randoms[0]))\n",
                 "print(lovely(randoms[:2]))\n",
                 "print(lovely(randoms[:6].view(2, 3))) # More than 2 elements -> show statistics\n",
-                "print(lovely(randoms[:11])) # More than 10 -> suppress data output\n"
+                "print(lovely(randoms[:11]))           # More than 10 -> suppress data output\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# |hide\n",
-                "test_eq(str(lovely(randoms[0])), \"tensor 1.927\")\n",
-                "test_eq(str(lovely(randoms[:2])), \"tensor[2] \u03bc=1.707 \u03c3=0.311 [1.927, 1.487]\")\n",
+                "test_eq(str(lovely(randoms[0])),             \"tensor 1.927\")\n",
+                "test_eq(str(lovely(randoms[:2])),            \"tensor[2] \u03bc=1.707 \u03c3=0.311 [1.927, 1.487]\")\n",
                 "test_eq(str(lovely(randoms[:6].view(2, 3))), \"tensor[2, 3] n=6 x\u2208[-2.106, 1.927] \u03bc=0.276 \u03c3=1.594 [[1.927, 1.487, 0.901], [-2.106, 0.678, -1.235]]\")\n",
-                "test_eq(str(lovely(randoms[:11])), \"tensor[11] x\u2208[-2.106, 1.927] \u03bc=0.046 \u03c3=1.384\")"
+                "test_eq(str(lovely(randoms[:11])),           \"tensor[11] x\u2208[-2.106, 1.927] \u03bc=0.046 \u03c3=1.384\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
@@ -439,14 +560,34 @@
                 "lovely(torch.zeros(12))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "tensor[2, 6] n=12 x\u2208[-1.605, 1.927e+04] \u03bc=2.141e+03 \u03c3=6.423e+03 \u001b[31m+Inf!\u001b[0m \u001b[31m-Inf!\u001b[0m \u001b[31mNaN!\u001b[0m"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "lovely(nasties)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
                 "test_eq(str(lovely(nasties)),\n",
                 "    'tensor[2, 6] n=12 x\u2208[-1.605, 1.927e+04] \u03bc=2.141e+03 \u03c3=6.423e+03 \\x1b[31m+Inf!\\x1b[0m \\x1b[31m-Inf!\\x1b[0m \\x1b[31mNaN!\\x1b[0m')\n",
                 "test_eq(str(lovely(torch.tensor([float(\"nan\")]*11))), 'tensor[11] \\x1b[31mNaN!\\x1b[0m')\n",
                 "test_eq(str(lovely(torch.zeros(12))), 'tensor[12] \\x1b[38;2;127;127;127mall_zeros\\x1b[0m')"
             ]
@@ -455,14 +596,34 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
+                            "tensor[3] i32 x\u2208[1, 3] \u03bc=2.000 \u03c3=1.000 [1, 2, 3]"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "lovely(torch.tensor([1,2,3], dtype=torch.int32))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
                             "tensor[2, 6] n=12 x\u2208[-1.605, 1.927e+04] \u03bc=2.141e+03 \u03c3=6.423e+03 \u001b[31m+Inf!\u001b[0m \u001b[31m-Inf!\u001b[0m \u001b[31mNaN!\u001b[0m\n",
                             "tensor([[ 1.9269e+04,  1.4873e-04,  9.0072e-01,         inf,        -inf,         nan],\n",
                             "        [-4.3067e-02, -1.6047e+00, -7.5214e-01,  1.6487e+00, -3.9248e-01, -1.4036e+00]])"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
@@ -518,24 +679,31 @@
                 "image = torch.load(\"mysteryman.pt\")\n",
                 "image[1,100,100] = float('nan')\n",
                 "\n",
                 "lovely(image, depth=1)"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "#### CUDA memory is not leaked"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "before allocation: torch.cuda.memory_allocated()=0\n",
-                        "after allocation: torch.cuda.memory_allocated()=12582912\n"
+                        "before allocation: Allocated: 0 MB, Max: 0 Mb\n",
+                        "after allocation: Allocated: 12 MB, Max: 12 Mb\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "tensor[3, 1024, 1024] n=3145728 x\u2208[-5.325, 5.150] \u03bc=-0.000 \u03c3=0.999 cuda:0"
                         ]
@@ -543,51 +711,55 @@
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "after repr: torch.cuda.memory_allocated()=12582912\n",
-                        "after cleanup: torch.cuda.memory_allocated()=0\n"
+                        "after repr: Allocated: 12 MB, Max: 12 Mb\n",
+                        "after cleanup: Allocated: 0 MB, Max: 12 Mb\n"
                     ]
                 }
             ],
             "source": [
                 "# |eval: false\n",
+                "def memstats():\n",
+                "    allocated = int(torch.cuda.memory_allocated() // (1024*1024))\n",
+                "    max_allocated = int(torch.cuda.max_memory_allocated() // (1024*1024))\n",
+                "    return f\"Allocated: {allocated} MB, Max: {max_allocated} Mb\"\n",
                 "\n",
                 "if torch.cuda.is_available():\n",
                 "    cudamem = torch.cuda.memory_allocated()\n",
-                "    print(f\"before allocation: {torch.cuda.memory_allocated()=}\")\n",
+                "    print(f\"before allocation: {memstats()}\")\n",
                 "    numbers = torch.randn((3, 1024, 1024), device=\"cuda\") # 12Mb image\n",
                 "    torch.cuda.synchronize()\n",
                 "\n",
-                "    print(f\"after allocation: {torch.cuda.memory_allocated()=}\")\n",
+                "    print(f\"after allocation: {memstats()}\")\n",
                 "    # Note, the return value of lovely() is not a string, but a\n",
                 "    # StrProxy that holds reference to 'numbers'. You have to del\n",
-                "    # any references to it.\n",
+                "    # the references to it, but once it's gone, the reference to\n",
+                "    # the tensor is gone too.\n",
                 "    display(lovely(numbers) )\n",
-                "    print(f\"after repr: {torch.cuda.memory_allocated()=}\")\n",
+                "    print(f\"after repr: {memstats()}\")\n",
                 "    \n",
                 "    del numbers\n",
                 "    # torch.cuda.memory.empty_cache()\n",
                 "\n",
-                "    print(f\"after cleanup: {torch.cuda.memory_allocated()=}\")\n",
+                "    print(f\"after cleanup: {memstats()}\")\n",
                 "    test_eq(cudamem >= torch.cuda.memory_allocated(), True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "tensor[5] complex64\n",
                             "tensor([-0.4011-0.4035j,  1.1300+0.0788j, -0.0277+0.9978j, -0.4636+0.6064j, -1.1505-0.9865j])"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
```

### Comparing `lovely-tensors-0.1.8/nbs/01_repr_rgb.ipynb` & `lovely-tensors-0.1.9/nbs/01_repr_rgb.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998702422145329%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(13, '        self.t = t\\n'), (23, '                "*

 * *            "frame_px=frame_px, view_width=view_width, scale=scale)\\n')], delete: [26, 24, 14, "*

 * *            '12]}}}'}*

```diff
@@ -89,29 +89,27 @@
                 "# first case, the class defines `_repr_png_` to send the image to Jupyter. For\n",
                 "# the later case, it defines __call__, which accps the argument.\n",
                 "\n",
                 "class RGBProxy():\n",
                 "    \"\"\"Flexible `PIL.Image.Image` wrapper\"\"\"\n",
                 "    \n",
                 "    def __init__(self, t:torch.Tensor):\n",
-                "        # super().__init__()\n",
                 "        assert t.ndim >= 3, f\"Expecting at least 3 dimensions, got shape{t.shape}={t.dim()}\"\n",
-                "        self.t = t #.detach().cpu().numpy()\n",
+                "        self.t = t\n",
                 "\n",
                 "    def __call__(   self,\n",
                 "                    denorm=None,\n",
                 "                    cl=False,\n",
                 "                    gutter_px=3, frame_px=1,\n",
                 "                    scale=1,\n",
                 "                    view_width=966):\n",
                 "\n",
                 "        return rgb(self.t, denorm=denorm, cl=cl, gutter_px=gutter_px,\n",
-                "                frame_px=frame_px, view_width=view_width)\n",
+                "                frame_px=frame_px, view_width=view_width, scale=scale)\n",
                 "    \n",
-                "    @torch.no_grad()\n",
                 "    def _repr_png_(self):\n",
                 "        # Note: In order to prevernt IPYthon from hogging memory, we\n",
                 "        # delete the reference to the tensor after the first call to\n",
                 "        # `_repr_png_`. This is fine for Jupyter use.\n",
                 "        return self.__call__()._repr_png_()\n"
             ]
         },
```

### Comparing `lovely-tensors-0.1.8/nbs/02_repr_plt.ipynb` & `lovely-tensors-0.1.9/nbs/02_repr_plt.ipynb`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/nbs/05_repr_chans.ipynb` & `lovely-tensors-0.1.9/nbs/05_repr_chans.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998883928571429%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(24, '                    frame_px=frame_px,\\n'), (26, "*

 * *            "'                    cl=cl)\\n')], delete: [25]}}}"}*

```diff
@@ -75,16 +75,17 @@
                 "                    cm_below=cm_below,\n",
                 "                    cm_above=cm_above,\n",
                 "                    cm_ninf=cm_ninf,\n",
                 "                    cm_pinf=cm_pinf,\n",
                 "                    cm_nan=cm_nan,\n",
                 "                    view_width=view_width,\n",
                 "                    gutter_px=gutter_px,\n",
+                "                    frame_px=frame_px,\n",
                 "                    scale=scale,\n",
-                "                    frame_px=frame_px)\n"
+                "                    cl=cl)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `lovely-tensors-0.1.8/nbs/10_patch.ipynb` & `lovely-tensors-0.1.9/nbs/10_patch.ipynb`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/nbs/_quarto.yml` & `lovely-tensors-0.1.9/nbs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/nbs/history.ipynb` & `lovely-tensors-0.1.9/nbs/history.ipynb`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/nbs/index.ipynb` & `lovely-tensors-0.1.9/nbs/index.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996639784946236%*

 * *Differences: {"'cells'": "{15: {'source': ['## Summary']}}"}*

```diff
@@ -187,15 +187,15 @@
                 "lt.monkey_patch()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## `__repr__`"
+                "## Summary"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
```

### Comparing `lovely-tensors-0.1.8/nbs/mysteryman.pt` & `lovely-tensors-0.1.9/nbs/mysteryman.pt`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/nbs/styles.css` & `lovely-tensors-0.1.9/nbs/styles.css`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/nbs/tenchman.jpg` & `lovely-tensors-0.1.9/nbs/tenchman.jpg`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/normalized.png` & `lovely-tensors-0.1.9/normalized.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/rgb.png` & `lovely-tensors-0.1.9/rgb.png`

 * *Files identical despite different names*

### Comparing `lovely-tensors-0.1.8/settings.ini` & `lovely-tensors-0.1.9/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = lovely-tensors
 lib_name = lovely-tensors
-version = 0.1.8
+version = 0.1.9
 min_python = 3.7
 license = mit
 
 ### nbdev ###
 doc_path = _docs
 lib_path = lovely_tensors
 nbs_path = nbs
@@ -33,12 +33,12 @@
 description = ❤️ Lovely Tensors
 keywords = jupyter pytorch tensor visualisation
 language = English
 status = 3
 user = xl0
 
 ### Optional ###
-requirements = pillow fastcore numpy ipython lovely-numpy>=0.1.2
+requirements = pillow fastcore numpy ipython lovely-numpy>=0.2
 pip_requirements = torch matplotlib
 conda_requirements = pytorch matplotlib-base
 dev_requirements = scipy
 # console_scripts =
```

### Comparing `lovely-tensors-0.1.8/setup.py` & `lovely-tensors-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pkg_resources import parse_version
 from configparser import ConfigParser
 import setuptools
 assert parse_version(setuptools.__version__)>=parse_version('36.2')
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
-config.read('settings.ini')
+config.read('settings.ini', encoding="utf-8")
 cfg = config['DEFAULT']
 
 cfg_keys = 'version description keywords author author_email'.split()
 expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
 for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
 setup_cfg = {o:cfg[o] for o in cfg_keys}
 
@@ -41,15 +41,15 @@
     url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
     extras_require={ 'dev': dev_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md').read(),
+    long_description = open('README.md', encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
     entry_points = {
         'console_scripts': cfg.get('console_scripts','').split(),
         'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
     },
     **setup_cfg)
```


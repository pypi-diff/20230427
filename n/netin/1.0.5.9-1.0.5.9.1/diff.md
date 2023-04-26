# Comparing `tmp/netin-1.0.5.9.tar.gz` & `tmp/netin-1.0.5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.9.tar", last modified: Wed Apr 26 21:43:46 2023, max compression
+gzip compressed data, was "netin-1.0.5.9.1.tar", last modified: Wed Apr 26 22:57:57 2023, max compression
```

## Comparing `netin-1.0.5.9.tar` & `netin-1.0.5.9.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.9/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.9/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3926 2023-04-26 21:43:46.498003 netin-1.0.5.9/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.5.9/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.9/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.9/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.9/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/examples/notebooks/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.5.9/examples/notebooks/deleteme.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.9/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.9/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.9/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.9/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      477 2023-04-26 21:37:21.000000 netin-1.0.5.9/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.5.9/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/netin/algorithms/sampling/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.5.9/netin/algorithms/sampling/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.5.9/netin/algorithms/sampling/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.5.9/netin/algorithms/sampling/degree_group_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.5.9/netin/algorithms/sampling/degree_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.5.9/netin/algorithms/sampling/partial_crawls.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.5.9/netin/algorithms/sampling/random_edges.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.5.9/netin/algorithms/sampling/random_neighbor.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.5.9/netin/algorithms/sampling/random_nodes.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6171 2023-04-26 21:06:58.000000 netin-1.0.5.9/netin/algorithms/sampling/sampling.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      524 2023-04-26 20:32:15.000000 netin-1.0.5.9/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5521 2023-04-24 18:03:30.000000 netin-1.0.5.9/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    14272 2023-04-26 19:47:38.000000 netin-1.0.5.9/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3434 2023-04-26 19:47:38.000000 netin-1.0.5.9/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5388 2023-04-26 19:47:38.000000 netin-1.0.5.9/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    28889 2023-04-26 21:31:14.000000 netin-1.0.5.9/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8253 2023-04-26 21:06:58.000000 netin-1.0.5.9/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3565 2023-04-26 21:42:50.000000 netin-1.0.5.9/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7286 2023-04-26 21:43:01.000000 netin-1.0.5.9/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7758 2023-04-26 21:42:54.000000 netin-1.0.5.9/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6216 2023-04-26 19:47:38.000000 netin-1.0.5.9/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.9/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.9/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.9/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.9/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.9/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.9/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9948 2023-04-26 20:38:34.000000 netin-1.0.5.9/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      574 2023-04-26 19:48:59.000000 netin-1.0.5.9/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.5.9/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5990 2023-04-26 20:37:47.000000 netin-1.0.5.9/netin/stats/networks.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.5.9/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.9/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1447 2023-04-26 18:57:24.000000 netin-1.0.5.9/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.5.9/netin/utils/io.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2184 2023-04-25 17:56:25.000000 netin-1.0.5.9/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.5.9/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.5.9/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    27179 2023-04-26 01:45:19.000000 netin-1.0.5.9/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3926 2023-04-26 21:43:46.000000 netin-1.0.5.9/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1708 2023-04-26 21:43:46.000000 netin-1.0.5.9/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-26 21:43:46.000000 netin-1.0.5.9/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.9/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-26 21:43:46.000000 netin-1.0.5.9/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-26 21:43:46.000000 netin-1.0.5.9/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.9/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.9/requirements/docs.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.9/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-26 21:43:46.498003 netin-1.0.5.9/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4291 2023-04-26 19:17:45.000000 netin-1.0.5.9/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.9.1/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.9.1/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.5.9.1/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.9.1/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.9.1/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.9.1/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/examples/notebooks/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.5.9.1/examples/notebooks/deleteme.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.9.1/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.9.1/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.9.1/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.9.1/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      479 2023-04-26 22:56:37.000000 netin-1.0.5.9.1/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.5.9.1/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/algorithms/sampling/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.5.9.1/netin/algorithms/sampling/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.5.9.1/netin/algorithms/sampling/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.5.9.1/netin/algorithms/sampling/degree_group_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.5.9.1/netin/algorithms/sampling/degree_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.5.9.1/netin/algorithms/sampling/partial_crawls.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.5.9.1/netin/algorithms/sampling/random_edges.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.5.9.1/netin/algorithms/sampling/random_neighbor.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.5.9.1/netin/algorithms/sampling/random_nodes.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6171 2023-04-26 21:06:58.000000 netin-1.0.5.9.1/netin/algorithms/sampling/sampling.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      524 2023-04-26 20:32:15.000000 netin-1.0.5.9.1/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5521 2023-04-24 18:03:30.000000 netin-1.0.5.9.1/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    14272 2023-04-26 19:47:38.000000 netin-1.0.5.9.1/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3434 2023-04-26 19:47:38.000000 netin-1.0.5.9.1/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5388 2023-04-26 19:47:38.000000 netin-1.0.5.9.1/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    29353 2023-04-26 22:52:24.000000 netin-1.0.5.9.1/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8253 2023-04-26 21:06:58.000000 netin-1.0.5.9.1/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3619 2023-04-26 22:55:17.000000 netin-1.0.5.9.1/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7340 2023-04-26 22:55:39.000000 netin-1.0.5.9.1/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7812 2023-04-26 22:56:19.000000 netin-1.0.5.9.1/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6216 2023-04-26 19:47:38.000000 netin-1.0.5.9.1/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.9.1/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.9.1/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.9.1/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.9.1/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.9.1/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.9.1/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9948 2023-04-26 20:38:34.000000 netin-1.0.5.9.1/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      574 2023-04-26 19:48:59.000000 netin-1.0.5.9.1/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.5.9.1/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5990 2023-04-26 20:37:47.000000 netin-1.0.5.9.1/netin/stats/networks.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.5.9.1/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.9.1/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1447 2023-04-26 18:57:24.000000 netin-1.0.5.9.1/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.5.9.1/netin/utils/io.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2184 2023-04-25 17:56:25.000000 netin-1.0.5.9.1/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.5.9.1/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.5.9.1/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    27317 2023-04-26 22:50:16.000000 netin-1.0.5.9.1/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.674023 netin-1.0.5.9.1/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 22:57:57.000000 netin-1.0.5.9.1/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1708 2023-04-26 22:57:57.000000 netin-1.0.5.9.1/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-26 22:57:57.000000 netin-1.0.5.9.1/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.9.1/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-26 22:57:57.000000 netin-1.0.5.9.1/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-26 22:57:57.000000 netin-1.0.5.9.1/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.9.1/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.9.1/requirements/docs.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.9.1/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-26 22:57:57.678023 netin-1.0.5.9.1/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4291 2023-04-26 19:17:45.000000 netin-1.0.5.9.1/setup.py
```

### Comparing `netin-1.0.5.9/LICENSE` & `netin-1.0.5.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/PKG-INFO` & `netin-1.0.5.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.9
+Version: 1.0.5.9.1
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.9/README.rst` & `netin-1.0.5.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/examples/notebooks/deleteme.py` & `netin-1.0.5.9.1/examples/notebooks/deleteme.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/algorithms/sampling/degree_group_rank.py` & `netin-1.0.5.9.1/netin/algorithms/sampling/degree_group_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/algorithms/sampling/degree_rank.py` & `netin-1.0.5.9.1/netin/algorithms/sampling/degree_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/algorithms/sampling/partial_crawls.py` & `netin-1.0.5.9.1/netin/algorithms/sampling/partial_crawls.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/algorithms/sampling/random_edges.py` & `netin-1.0.5.9.1/netin/algorithms/sampling/random_edges.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/algorithms/sampling/random_neighbor.py` & `netin-1.0.5.9.1/netin/algorithms/sampling/random_neighbor.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/algorithms/sampling/random_nodes.py` & `netin-1.0.5.9.1/netin/algorithms/sampling/random_nodes.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/algorithms/sampling/sampling.py` & `netin-1.0.5.9.1/netin/algorithms/sampling/sampling.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/__init__.py` & `netin-1.0.5.9.1/netin/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/dh.py` & `netin-1.0.5.9.1/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/directed.py` & `netin-1.0.5.9.1/netin/generators/directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/dpa.py` & `netin-1.0.5.9.1/netin/generators/dpa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/dpah.py` & `netin-1.0.5.9.1/netin/generators/dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/graph.py` & `netin-1.0.5.9.1/netin/generators/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -750,23 +750,31 @@
         n_jobs: int
             number of parallel jobs
 
         Returns
         -------
         pd.DataFrame
             dataframe with the metadata of the nodes
+
+        Notes
+        -----
+        Column `class_label` is a binary column indicating whether the node belongs to the minority class.
         """
-        cols = ['node', 'class_label']
+        cols = ['node', 'class_label', 'real_label', 'source']
+
         obj = {'node': self.node_list,
-               'class_label': [self.get_class_label(n) for n in self.node_list]}
+               'class_label': [const.MAJORITY_LABEL if self.get_class_label(n) == self.get_majority_label() else const.MINORITY_LABEL for n in self.node_list],
+               'real_label': [self.get_class_label(n) for n in self.node_list],
+               'source': 'model' if 'empirical' not in self.graph else 'data'}
 
         # include graph metadata
         if include_graph_metadata:
             n = self.number_of_nodes()
-            newcols = [c for c in self.graph.keys() if c not in ['class_attribute', 'class_values', 'class_labels']]
+            newcols = [c for c in self.graph.keys() if c not in ['class_attribute', 'class_values',
+                                                                 'class_labels']]
             obj.update({c: self.graph[c] for c in newcols})
             cols.extend(newcols)
 
         # include metrics
         column_values = pqdm(const.VALID_METRICS, self.compute_node_stats, n_jobs=n_jobs)
         obj.update({col: values for col, values in zip(const.VALID_METRICS, column_values)})
         cols.extend(const.VALID_METRICS)
```

### Comparing `netin-1.0.5.9/netin/generators/h.py` & `netin-1.0.5.9.1/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/pa.py` & `netin-1.0.5.9.1/netin/generators/pa.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,15 +101,17 @@
             graph to fit the model to
 
         n: int
             number of nodes to override (e.g., to generate a smaller network)
 
         k: int
             minimum node degree to override (e.g., to generate a denser network ``k>1``)
-        seed
+
+        seed: object
+            seed for random number generator
 
         Returns
         -------
         netin.PA
             fitted model
         """
         n = n or g.number_of_nodes()
```

### Comparing `netin-1.0.5.9/netin/generators/pah.py` & `netin-1.0.5.9.1/netin/generators/pah.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,17 @@
             graph to fit the model to
 
         n: int
             number of nodes to override (e.g., to generate a smaller network)
 
         k: int
             minimum node degree to override (e.g., to generate a denser network ``k>1``)
-        seed
+
+        seed: object
+            seed for random number generator
 
         Returns
         -------
         netin.PAH
             fitted model
         """
         n = n or g.number_of_nodes()
```

### Comparing `netin-1.0.5.9/netin/generators/patc.py` & `netin-1.0.5.9.1/netin/generators/patc.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,17 @@
             graph to fit the model to
 
         n: int
             number of nodes to override (e.g., to generate a smaller network)
 
         k: int
             minimum node degree to override (e.g., to generate a denser network ``k>1``)
-        seed
+
+        seed: object
+            seed for random number generator
 
         Returns
         -------
         netin.PATC
             fitted model
         """
         n = n or g.number_of_nodes()
```

### Comparing `netin-1.0.5.9/netin/generators/patch.py` & `netin-1.0.5.9.1/netin/generators/patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/tc.py` & `netin-1.0.5.9.1/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/tests/test_directed.py` & `netin-1.0.5.9.1/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/tests/test_dpah.py` & `netin-1.0.5.9.1/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/tests/test_patch.py` & `netin-1.0.5.9.1/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/tests/test_undirected.py` & `netin-1.0.5.9.1/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/generators/undirected.py` & `netin-1.0.5.9.1/netin/generators/undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/stats/__init__.py` & `netin-1.0.5.9.1/netin/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/stats/distributions.py` & `netin-1.0.5.9.1/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/stats/networks.py` & `netin-1.0.5.9.1/netin/stats/networks.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/stats/ranking.py` & `netin-1.0.5.9.1/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/utils/constants.py` & `netin-1.0.5.9.1/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/utils/io.py` & `netin-1.0.5.9.1/netin/utils/io.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/utils/validator.py` & `netin-1.0.5.9.1/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/netin/viz/handlers.py` & `netin-1.0.5.9.1/netin/viz/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from matplotlib import rc
+from collections import Counter
 
 from netin.generators.graph import Graph
 from netin.stats.distributions import fit_power_law
 from netin.stats.distributions import get_disparity
 from netin.stats.distributions import get_fraction_of_minority
 from netin.stats.distributions import get_gini_coefficient
 from netin.utils import constants as const
@@ -97,15 +98,17 @@
         If it is a curve for the minority class, the color is the color of the minority class.
         Otherwise, the color for the class label.
 
     Returns
     -------
     color: str
         color for the class label
+
     """
+
     if ylabel in MINORITY_CURVE and class_label is None:
         return COLOR_MINORITY
 
     return COLOR_MINORITY if class_label == const.MINORITY_LABEL \
         else COLOR_MAJORITY if class_label == const.MAJORITY_LABEL \
         else COLOR_BLACK
 
@@ -454,15 +457,16 @@
         class_label: str
         iter_groups = df.groupby(hue) if hue is not None else [(None, df)]
         f_m = df.query("class_label == @const.MINORITY_LABEL").shape[0] / df.shape[0]
         for class_label, group in iter_groups:
             total = df[_col_name].sum() if common_norm else group[_col_name].sum()
             xs, ys = get_x_y_from_df_fnc(group, _col_name, total)
             plot = ax.scatter if scatter else ax.plot
-            plot(xs, ys, label=class_label, color=_get_class_label_color(class_label, xy_fnc_name), **kwargs)
+            plot(xs, ys, label=class_label, color=_get_class_label_color(class_label=class_label,
+                                                                         ylabel=xy_fnc_name), **kwargs)
 
             if hline_fnc:
                 hline_fnc(ax.axhline, group)
             if vline_fnc:
                 vline_fnc(ax.axvline, group)
             if me_fnc:
                 me_fnc(ax, f_m, ys, beta)
@@ -785,15 +789,15 @@
             if group_nonzero[_col_name].nunique() == 1:
                 # not enough data to fit the powerlaw
                 continue
 
             discrete = group_nonzero[_col_name].dtype == np.int64
             fit = fit_power_law(group_nonzero.loc[:, _col_name].values, discrete=discrete, verbose=verbose)
 
-            color = _get_class_label_color(class_label)
+            color = _get_class_label_color(class_label=class_label)
 
             efnc = fit.plot_ccdf if kind == "ccdf" else fit.plot_cdf if kind == 'cdf' else fit.plot_pdf
             fnc = fit.power_law.plot_ccdf if kind == "ccdf" else fit.power_law.plot_cdf if kind == 'cdf' \
                 else fit.power_law.plot_pdf
 
             try:
                 ax = efnc(label=r"Empirical", ax=ax, color=color, **kwargs)
```

### Comparing `netin-1.0.5.9/netin.egg-info/PKG-INFO` & `netin-1.0.5.9.1/netin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.9
+Version: 1.0.5.9.1
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.9/netin.egg-info/SOURCES.txt` & `netin-1.0.5.9.1/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.9/setup.py` & `netin-1.0.5.9.1/setup.py`

 * *Files identical despite different names*


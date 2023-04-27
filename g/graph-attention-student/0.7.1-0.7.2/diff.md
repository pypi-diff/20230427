# Comparing `tmp/graph_attention_student-0.7.1.tar.gz` & `tmp/graph_attention_student-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_attention_student-0.7.1.tar", max compression
+gzip compressed data, was "graph_attention_student-0.7.2.tar", max compression
```

## Comparing `graph_attention_student-0.7.1.tar` & `graph_attention_student-0.7.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rwxr-xr-x   0        0        0     8961 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/README.rst
--rwxr-xr-x   0        0        0        5 2023-04-19 13:30:28.447135 graph_attention_student-0.7.1/graph_attention_student/VERSION
--rwxr-xr-x   0        0        0       90 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/__init__.py
--rwxr-xr-x   0        0        0    84242 2023-03-19 09:18:21.518826 graph_attention_student-0.7.1/graph_attention_student/_models.py
--rwxr-xr-x   0        0        0     1131 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/cli.py
--rwxr-xr-x   0        0        0    54483 2023-01-17 14:13:51.169936 graph_attention_student-0.7.1/graph_attention_student/data.py
--rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/examples/__init__.py
--rw-r--r--   0        0        0     9670 2023-01-20 11:45:50.758439 graph_attention_student-0.7.1/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc
--rw-r--r--   0        0        0    12164 2023-01-20 09:12:31.703590 graph_attention_student-0.7.1/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc
--rwxr-xr-x   0        0        0    11582 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/examples/gnes_example.py
--rwxr-xr-x   0        0        0    11569 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/examples/gnnx_example.py
--rwxr-xr-x   0        0        0    18745 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/examples/smiles_example.py
--rw-r--r--   0        0        0    14585 2023-01-20 12:59:31.279402 graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn.py
--rw-r--r--   0        0        0     5503 2023-01-20 11:59:55.452453 graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py
--rw-r--r--   0        0        0     4809 2023-01-20 11:39:35.159855 graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn_gin.py
--rwxr-xr-x   0        0        0    20103 2023-01-20 10:32:00.863590 graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_megan.py
--rw-r--r--   0        0        0     1272 2023-01-20 09:42:42.629614 graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_megan_tadf.py
--rwxr-xr-x   0        0        0      726 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/experiments/README.rst
--rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/experiments/__init__.py
--rw-r--r--   0        0        0    10604 2023-03-28 09:55:24.672691 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_classification.cpython-310.pyc
--rw-r--r--   0        0        0    15106 2023-03-20 09:39:48.984068 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc
--rw-r--r--   0        0        0    10324 2023-04-19 12:44:07.919515 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc
--rw-r--r--   0        0        0     6258 2023-01-24 12:19:49.929234 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc
--rw-r--r--   0        0        0     1373 2023-01-24 14:25:26.991807 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc
--rw-r--r--   0        0        0     4729 2023-04-19 12:44:06.195491 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc
--rw-r--r--   0        0        0     1345 2023-01-24 12:56:57.478326 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc
--rwxr-xr-x   0        0        0     9205 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/experiments/process_aqsoldb.py
--rwxr-xr-x   0        0        0    31932 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/experiments/rb_motifs_multi.py
--rwxr-xr-x   0        0        0    34843 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/experiments/rb_motifs_single.py
--rw-r--r--   0        0        0      459 2023-01-24 12:36:03.337029 graph_attention_student-0.7.1/graph_attention_student/experiments/template_sub_experiment.py
--rw-r--r--   0        0        0    18495 2023-03-28 09:55:23.204678 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_classification.py
--rw-r--r--   0        0        0     5029 2023-03-29 07:00:40.799553 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_classification_megan.py
--rw-r--r--   0        0        0    18717 2023-03-19 08:35:02.980618 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_posthoc.py
--rw-r--r--   0        0        0    24342 2023-03-20 09:39:47.552048 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised.py
--rw-r--r--   0        0        0     5567 2023-03-20 09:39:47.564048 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised_multi.py
--rw-r--r--   0        0        0     5788 2023-03-20 07:08:16.190877 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised_single.py
--rw-r--r--   0        0        0    17117 2023-04-19 12:42:45.170288 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single.py
--rw-r--r--   0        0        0     8128 2023-01-24 12:19:49.761232 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx.py
--rw-r--r--   0        0        0     1038 2023-01-24 14:25:25.831799 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py
--rw-r--r--   0        0        0     5506 2023-01-24 13:54:11.870993 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py
--rw-r--r--   0        0        0     3581 2023-01-24 14:26:38.996305 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py
--rw-r--r--   0        0        0     5234 2023-01-24 13:19:46.309473 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py
--rw-r--r--   0        0        0     7948 2023-04-19 12:44:06.007488 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_megan.py
--rw-r--r--   0        0        0     1034 2023-04-19 12:46:43.177610 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py
--rw-r--r--   0        0        0      695 2023-02-27 13:28:58.309313 graph_attention_student-0.7.1/graph_attention_student/keras.py
--rwxr-xr-x   0        0        0    20274 2023-02-23 19:42:55.562555 graph_attention_student-0.7.1/graph_attention_student/layers.py
--rw-r--r--   0        0        0      205 2023-03-19 09:12:41.525356 graph_attention_student-0.7.1/graph_attention_student/models/__init__.py
--rw-r--r--   0        0        0      380 2023-03-19 09:15:50.038102 graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3314 2023-04-01 14:29:59.234990 graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc
--rw-r--r--   0        0        0     1950 2023-03-19 09:15:50.054102 graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc
--rw-r--r--   0        0        0     9247 2023-04-01 10:01:31.663992 graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc
--rw-r--r--   0        0        0    15003 2023-03-28 11:59:53.838597 graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/megan.cpython-310.pyc
--rw-r--r--   0        0        0     3406 2023-04-01 14:29:47.290900 graph_attention_student-0.7.1/graph_attention_student/models/gnes.py
--rw-r--r--   0        0        0     2590 2023-03-19 09:15:48.990097 graph_attention_student-0.7.1/graph_attention_student/models/gnnx.py
--rw-r--r--   0        0        0    12361 2023-04-01 10:01:20.259917 graph_attention_student-0.7.1/graph_attention_student/models/gradient.py
--rw-r--r--   0        0        0    28462 2023-03-28 11:59:52.766589 graph_attention_student-0.7.1/graph_attention_student/models/megan.py
--rwxr-xr-x   0        0        0     1040 2023-01-18 09:06:23.993806 graph_attention_student-0.7.1/graph_attention_student/templates/article.tex.j2
--rw-r--r--   0        0        0      375 2023-01-24 12:08:49.160527 graph_attention_student-0.7.1/graph_attention_student/templates/table.tex.j2
--rw-r--r--   0        0        0      151 2023-01-17 16:58:58.659355 graph_attention_student-0.7.1/graph_attention_student/templates/table_content.tex.j2
--rw-r--r--   0        0        0       76 2023-01-17 17:10:30.475776 graph_attention_student-0.7.1/graph_attention_student/templates/table_element_mean.tex.j2
--rwxr-xr-x   0        0        0    13166 2023-04-01 11:27:51.694228 graph_attention_student-0.7.1/graph_attention_student/training.py
--rwxr-xr-x   0        0        0     3753 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/typing.py
--rwxr-xr-x   0        0        0    15021 2023-01-18 08:39:58.301379 graph_attention_student-0.7.1/graph_attention_student/util.py
--rwxr-xr-x   0        0        0    16147 2023-03-27 10:44:14.975799 graph_attention_student-0.7.1/graph_attention_student/visualization.py
--rwxr-xr-x   0        0        0     1397 2023-04-19 13:30:28.439135 graph_attention_student-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    10441 1970-01-01 00:00:00.000000 graph_attention_student-0.7.1/setup.py
--rw-r--r--   0        0        0    10052 1970-01-01 00:00:00.000000 graph_attention_student-0.7.1/PKG-INFO
+-rwxr-xr-x   0        0        0     8961 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/README.rst
+-rwxr-xr-x   0        0        0        5 2023-04-27 12:35:16.036165 graph_attention_student-0.7.2/graph_attention_student/VERSION
+-rwxr-xr-x   0        0        0       90 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/__init__.py
+-rwxr-xr-x   0        0        0    84242 2023-03-19 09:18:21.518826 graph_attention_student-0.7.2/graph_attention_student/_models.py
+-rwxr-xr-x   0        0        0     1131 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/cli.py
+-rwxr-xr-x   0        0        0    54483 2023-01-17 14:13:51.169936 graph_attention_student-0.7.2/graph_attention_student/data.py
+-rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/examples/__init__.py
+-rw-r--r--   0        0        0     9670 2023-01-20 11:45:50.758439 graph_attention_student-0.7.2/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc
+-rw-r--r--   0        0        0    12164 2023-01-20 09:12:31.703590 graph_attention_student-0.7.2/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc
+-rwxr-xr-x   0        0        0    11582 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/examples/gnes_example.py
+-rwxr-xr-x   0        0        0    11569 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/examples/gnnx_example.py
+-rwxr-xr-x   0        0        0    18745 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/examples/smiles_example.py
+-rw-r--r--   0        0        0    14585 2023-01-20 12:59:31.279402 graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn.py
+-rw-r--r--   0        0        0     5503 2023-01-20 11:59:55.452453 graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py
+-rw-r--r--   0        0        0     4809 2023-01-20 11:39:35.159855 graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn_gin.py
+-rwxr-xr-x   0        0        0    20103 2023-01-20 10:32:00.863590 graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_megan.py
+-rw-r--r--   0        0        0     1272 2023-01-20 09:42:42.629614 graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_megan_tadf.py
+-rwxr-xr-x   0        0        0      726 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/experiments/README.rst
+-rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/experiments/__init__.py
+-rw-r--r--   0        0        0    10604 2023-03-28 09:55:24.672691 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_classification.cpython-310.pyc
+-rw-r--r--   0        0        0    15106 2023-03-20 09:39:48.984068 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc
+-rw-r--r--   0        0        0    10324 2023-04-19 12:44:07.919515 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc
+-rw-r--r--   0        0        0     6258 2023-01-24 12:19:49.929234 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc
+-rw-r--r--   0        0        0     1373 2023-01-24 14:25:26.991807 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc
+-rw-r--r--   0        0        0     4798 2023-04-27 11:59:03.979768 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc
+-rw-r--r--   0        0        0     1345 2023-01-24 12:56:57.478326 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc
+-rwxr-xr-x   0        0        0     9205 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/experiments/process_aqsoldb.py
+-rwxr-xr-x   0        0        0    31932 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/experiments/rb_motifs_multi.py
+-rwxr-xr-x   0        0        0    34843 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/experiments/rb_motifs_single.py
+-rw-r--r--   0        0        0      459 2023-01-24 12:36:03.337029 graph_attention_student-0.7.2/graph_attention_student/experiments/template_sub_experiment.py
+-rw-r--r--   0        0        0    18495 2023-03-28 09:55:23.204678 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_classification.py
+-rw-r--r--   0        0        0     5029 2023-03-29 07:00:40.799553 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_classification_megan.py
+-rw-r--r--   0        0        0    18717 2023-03-19 08:35:02.980618 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_posthoc.py
+-rw-r--r--   0        0        0    24342 2023-03-20 09:39:47.552048 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised.py
+-rw-r--r--   0        0        0     5567 2023-03-20 09:39:47.564048 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised_multi.py
+-rw-r--r--   0        0        0     5788 2023-03-20 07:08:16.190877 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised_single.py
+-rw-r--r--   0        0        0    17117 2023-04-19 12:42:45.170288 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single.py
+-rw-r--r--   0        0        0     8128 2023-01-24 12:19:49.761232 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx.py
+-rw-r--r--   0        0        0     1038 2023-01-24 14:25:25.831799 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py
+-rw-r--r--   0        0        0     5506 2023-01-24 13:54:11.870993 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py
+-rw-r--r--   0        0        0     3581 2023-01-24 14:26:38.996305 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py
+-rw-r--r--   0        0        0     5234 2023-01-24 13:19:46.309473 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py
+-rw-r--r--   0        0        0     8048 2023-04-27 11:58:55.515701 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_megan.py
+-rw-r--r--   0        0        0     1218 2023-04-27 12:34:08.343622 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py
+-rw-r--r--   0        0        0      695 2023-02-27 13:28:58.309313 graph_attention_student-0.7.2/graph_attention_student/keras.py
+-rwxr-xr-x   0        0        0    20274 2023-02-23 19:42:55.562555 graph_attention_student-0.7.2/graph_attention_student/layers.py
+-rw-r--r--   0        0        0      205 2023-03-19 09:12:41.525356 graph_attention_student-0.7.2/graph_attention_student/models/__init__.py
+-rw-r--r--   0        0        0      380 2023-03-19 09:15:50.038102 graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3314 2023-04-01 14:29:59.234990 graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc
+-rw-r--r--   0        0        0     1950 2023-03-19 09:15:50.054102 graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc
+-rw-r--r--   0        0        0     9247 2023-04-01 10:01:31.663992 graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc
+-rw-r--r--   0        0        0    15515 2023-04-27 12:08:11.991926 graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/megan.cpython-310.pyc
+-rw-r--r--   0        0        0     3406 2023-04-01 14:29:47.290900 graph_attention_student-0.7.2/graph_attention_student/models/gnes.py
+-rw-r--r--   0        0        0     2590 2023-03-19 09:15:48.990097 graph_attention_student-0.7.2/graph_attention_student/models/gnnx.py
+-rw-r--r--   0        0        0    12361 2023-04-01 10:01:20.259917 graph_attention_student-0.7.2/graph_attention_student/models/gradient.py
+-rw-r--r--   0        0        0    29552 2023-04-27 12:08:10.919918 graph_attention_student-0.7.2/graph_attention_student/models/megan.py
+-rwxr-xr-x   0        0        0     1040 2023-01-18 09:06:23.993806 graph_attention_student-0.7.2/graph_attention_student/templates/article.tex.j2
+-rw-r--r--   0        0        0      375 2023-01-24 12:08:49.160527 graph_attention_student-0.7.2/graph_attention_student/templates/table.tex.j2
+-rw-r--r--   0        0        0      151 2023-01-17 16:58:58.659355 graph_attention_student-0.7.2/graph_attention_student/templates/table_content.tex.j2
+-rw-r--r--   0        0        0       76 2023-01-17 17:10:30.475776 graph_attention_student-0.7.2/graph_attention_student/templates/table_element_mean.tex.j2
+-rwxr-xr-x   0        0        0    13166 2023-04-01 11:27:51.694228 graph_attention_student-0.7.2/graph_attention_student/training.py
+-rwxr-xr-x   0        0        0     3753 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/typing.py
+-rwxr-xr-x   0        0        0    15021 2023-01-18 08:39:58.301379 graph_attention_student-0.7.2/graph_attention_student/util.py
+-rwxr-xr-x   0        0        0    16147 2023-03-27 10:44:14.975799 graph_attention_student-0.7.2/graph_attention_student/visualization.py
+-rwxr-xr-x   0        0        0     1397 2023-04-27 12:35:16.028165 graph_attention_student-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    10441 1970-01-01 00:00:00.000000 graph_attention_student-0.7.2/setup.py
+-rw-r--r--   0        0        0    10052 1970-01-01 00:00:00.000000 graph_attention_student-0.7.2/PKG-INFO
```

### Comparing `graph_attention_student-0.7.1/README.rst` & `graph_attention_student-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/_models.py` & `graph_attention_student-0.7.2/graph_attention_student/_models.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/cli.py` & `graph_attention_student-0.7.2/graph_attention_student/cli.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/data.py` & `graph_attention_student-0.7.2/graph_attention_student/data.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/examples/gnes_example.py` & `graph_attention_student-0.7.2/graph_attention_student/examples/gnes_example.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/examples/gnnx_example.py` & `graph_attention_student-0.7.2/graph_attention_student/examples/gnnx_example.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/examples/smiles_example.py` & `graph_attention_student-0.7.2/graph_attention_student/examples/smiles_example.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn.py` & `graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py` & `graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn_gin.py` & `graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn_gin.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_megan.py` & `graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_megan.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_megan_tadf.py` & `graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_megan_tadf.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/README.rst` & `graph_attention_student-0.7.2/graph_attention_student/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_classification.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_classification.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 19 12:44:06 2023 UTC, .py size: 7948 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 16e2 3f64 0c1f 0000  o.........?d....
+00000000: 6f0d 0d0a 0000 0000 7f63 4a64 701f 0000  o........cJdp...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 4c02 0000 5500  .....@...sL...U.
+00000020: 0009 0000 0040 0000 0073 5802 0000 5500  .....@...sX...U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6401 6402 6c03 5a04 6401 6402  l.Z.d.d.l.Z.d.d.
 00000050: 6c05 5a06 6401 6402 6c07 6d08 5a09 0100  l.Z.d.d.l.m.Z...
 00000060: 6401 6402 6c0a 5a0b 6401 6403 6c0c 6d0d  d.d.l.Z.d.d.l.m.
 00000070: 5a0d 0100 6401 6404 6c0e 6d0f 5a0f 0100  Z...d.d.l.m.Z...
 00000080: 6401 6405 6c10 6d11 5a11 0100 6401 6406  d.d.l.m.Z...d.d.
 00000090: 6c12 6d13 5a13 0100 6401 6407 6c14 6d15  l.m.Z...d.d.l.m.
@@ -14,283 +14,287 @@
 000000d0: 1900 651b 640c 3c00 640d 5a1d 651a 651b  ..e.d.<.d.Z.e.e.
 000000e0: 640e 3c00 6700 640f a201 5a1e 6504 6a1f  d.<.g.d...Z.e.j.
 000000f0: 6520 1900 651b 6410 3c00 6411 5a21 6522  e ..e.d.<.d.Z!e"
 00000100: 651b 6412 3c00 6413 5a23 6522 651b 6414  e.d.<.d.Z#e"e.d.
 00000110: 3c00 6415 5a24 6522 651b 6416 3c00 6417  <.d.Z$e"e.d.<.d.
 00000120: 5a25 6520 651b 6418 3c00 6419 5a26 6522  Z%e e.d.<.d.Z&e"
 00000130: 651b 641a 3c00 641b 5a27 6528 651b 641c  e.d.<.d.Z'e(e.d.
-00000140: 3c00 6401 5a29 641d 641e 6702 6701 5a2a  <.d.Z)d.d.g.g.Z*
-00000150: 641f 6420 6421 9c02 5a2b 6700 6422 a201  d.d d!..Z+g.d"..
-00000160: 5a2c 6411 5a2d 6423 5a2e 6424 6425 8400  Z,d.Z-d#Z.d$d%..
-00000170: 5a2f 6426 6427 6702 5a30 6502 a031 6532  Z/d&d'g.Z0e..1e2
-00000180: a101 6a33 a034 a100 5a35 6501 6a36 a037  ..j3.4..Z5e.j6.7
-00000190: 6535 6428 a102 5a38 6535 5a39 6429 5a3a  e5d(..Z8e5Z9d)Z:
-000001a0: 642a 5a3b 650d 8300 8f5d 0100 650f 6538  d*Z;e....]..e.e8
-000001b0: 6539 653a 653c 8300 8304 0400 5a3d 8f39  e9e:e<......Z=.9
-000001c0: 0100 653d a03e 642b a101 642c 642b 8400  ..e=.>d+..d,d+..
-000001d0: 8301 5a3f 653d a03e 642d a101 642e 642d  ..Z?e=.>d-..d.d-
-000001e0: 8400 8301 5a40 653d a03e 642f a101 6436  ....Z@e=.>d/..d6
-000001f0: 6430 6528 6602 6431 642f 8405 8301 5a41  d0e(f.d1d/....ZA
-00000200: 653d a03e 6432 a101 6433 6432 8400 8301  e=.>d2..d3d2....
-00000210: 5a42 653d a03e 6434 a101 6435 6434 8400  ZBe=.>d4..d5d4..
-00000220: 8301 5a43 5700 6402 0400 0400 8303 0100  ..ZCW.d.........
-00000230: 6e11 3100 9001 7306 7701 0100 0100 0100  n.1...s.w.......
-00000240: 5900 0100 5700 6402 0400 0400 8303 0100  Y...W.d.........
-00000250: 6402 5300 5700 6402 0400 0400 8303 0100  d.S.W.d.........
-00000260: 6402 5300 3100 9001 731f 7701 0100 0100  d.S.1...s.w.....
-00000270: 0100 5900 0100 6402 5300 2937 7a13 0a0a  ..Y...d.S.)7z...
-00000280: 4348 414e 4745 4c4f 470a 0a30 2e31 2e30  CHANGELOG..0.1.0
-00000290: 0ae9 0000 0000 4e29 01da 0953 6b69 7070  ......N)...Skipp
-000002a0: 6162 6c65 2901 da0d 5375 6245 7870 6572  able)...SubExper
-000002b0: 696d 656e 7429 01da 1f72 6167 6765 645f  iment)...ragged_
-000002c0: 7465 6e73 6f72 5f66 726f 6d5f 6e65 7374  tensor_from_nest
-000002d0: 6564 5f6e 756d 7079 2901 da05 4d65 6761  ed_numpy)...Mega
-000002e0: 6e29 02da 064e 6f4c 6f73 73da 036d 7365  n)...NoLoss..mse
-000002f0: 2901 da13 4c6f 6750 726f 6772 6573 7343  )...LogProgressC
-00000300: 616c 6c62 6163 6bda 126e 6f64 655f 696d  allback..node_im
-00000310: 706f 7274 616e 6365 735f 32da 144e 4f44  portances_2..NOD
-00000320: 455f 494d 504f 5254 414e 4345 535f 4b45  E_IMPORTANCES_KE
-00000330: 59da 1265 6467 655f 696d 706f 7274 616e  Y..edge_importan
-00000340: 6365 735f 32da 1445 4447 455f 494d 504f  ces_2..EDGE_IMPO
-00000350: 5254 414e 4345 535f 4b45 59da 054d 4547  RTANCES_KEY..MEG
-00000360: 414e da0a 4d4f 4445 4c5f 4e41 4d45 2903  AN..MODEL_NAME).
-00000370: e920 0000 0072 0f00 0000 720f 0000 00da  . ...r....r.....
-00000380: 0555 4e49 5453 6700 0000 0000 0000 00da  .UNITSg.........
-00000390: 0c44 524f 504f 5554 5f52 4154 4567 0000  .DROPOUT_RATEg..
-000003a0: 0000 0000 f03f da11 494d 504f 5254 414e  .....?..IMPORTAN
-000003b0: 4345 5f46 4143 544f 52e9 0500 0000 da15  CE_FACTOR.......
-000003c0: 494d 504f 5254 414e 4345 5f4d 554c 5449  IMPORTANCE_MULTI
-000003d0: 504c 4945 52e9 0200 0000 da13 494d 504f  PLIER.......IMPO
-000003e0: 5254 414e 4345 5f43 4841 4e4e 454c 5367  RTANCE_CHANNELSg
-000003f0: 0000 0000 0000 1440 da0f 5350 4152 5349  .......@..SPARSI
-00000400: 5459 5f46 4143 544f 5246 da0c 434f 4e43  TY_FACTORF..CONC
-00000410: 4154 5f48 4541 4453 e9fd ffff ffe9 0300  AT_HEADS........
-00000420: 0000 e9ff ffff ffe9 0100 0000 2902 7201  ............).r.
-00000430: 0000 0072 1c00 0000 2903 e93c 0000 00e9  ...r....)..<....
-00000440: 1400 0000 721c 0000 00e9 fa00 0000 6300  ....r.........c.
-00000450: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000460: 0000 0043 0000 0073 0e00 0000 7400 6a01  ...C...s....t.j.
-00000470: 6a02 6401 6402 8d01 5300 2903 4e67 7b14  j.d.d...S.).Ng{.
-00000480: ae47 e17a 843f 2901 da0d 6c65 6172 6e69  .G.z.?)...learni
-00000490: 6e67 5f72 6174 6529 03da 026b 73da 0a6f  ng_rate)...ks..o
-000004a0: 7074 696d 697a 6572 73da 054e 6164 616d  ptimizers..Nadam
-000004b0: a900 7224 0000 0072 2400 0000 fa66 2f6d  ..r$...r$....f/m
-000004c0: 6564 6961 2f73 7364 2f50 726f 6772 616d  edia/ssd/Program
-000004d0: 6d69 6e67 2f67 7261 7068 5f61 7474 656e  ming/graph_atten
-000004e0: 7469 6f6e 5f73 7475 6465 6e74 2f67 7261  tion_student/gra
-000004f0: 7068 5f61 7474 656e 7469 6f6e 5f73 7475  ph_attention_stu
-00000500: 6465 6e74 2f65 7870 6572 696d 656e 7473  dent/experiments
-00000510: 2f76 6764 5f73 696e 676c 655f 6d65 6761  /vgd_single_mega
-00000520: 6e2e 7079 da08 3c6c 616d 6264 613e 5800  n.py..<lambda>X.
-00000530: 0000 7302 0000 000e 0072 2600 0000 da08  ..s......r&.....
-00000540: 6e65 6761 7469 7665 da08 706f 7369 7469  negative..positi
-00000550: 7665 7a0d 7667 645f 7369 6e67 6c65 2e70  vez.vgd_single.p
-00000560: 797a 1872 6573 756c 7473 2f76 6764 5f73  yz.results/vgd_s
-00000570: 696e 676c 655f 6d65 6761 6e54 da0c 6372  ingle_meganT..cr
-00000580: 6561 7465 5f6d 6f64 656c 6301 0000 0000  eate_modelc.....
-00000590: 0000 0000 0000 0002 0000 000f 0000 0043  ...............C
-000005a0: 0000 0073 b400 0000 7c00 a000 6401 a101  ...s....|...d...
-000005b0: 0100 7c00 a000 6402 7c00 6a01 6403 1900  ..|...d.|.j.d...
-000005c0: 9b00 9d02 a101 0100 7402 7c00 6a01 6404  ........t.|.j.d.
-000005d0: 1900 7c00 6a01 6405 1900 7c00 6a01 6406  ..|.j.d...|.j.d.
-000005e0: 1900 7c00 6a01 6407 1900 7c00 6a01 6408  ..|.j.d...|.j.d.
-000005f0: 1900 7c00 6a01 6403 1900 7c00 6a01 6409  ..|.j.d...|.j.d.
-00000600: 1900 7c00 6a01 640a 1900 7c00 6a01 640b  ..|.j.d...|.j.d.
-00000610: 1900 7c00 6a01 640c 1900 640d 640e 7c00  ..|.j.d...d.d.|.
-00000620: 6a01 640f 1900 6410 8d0d 7d01 7c01 6a03  j.d...d...}.|.j.
-00000630: 7404 7405 8300 7405 8300 6703 6700 6411  t.t...t...g.g.d.
-00000640: a201 7404 6701 7c00 6a01 6412 1900 8300  ..t.g.|.j.d.....
-00000650: 640d 6413 8d05 0100 7c01 5300 2914 4e72  d.d.....|.S.).Nr
-00000660: 0d00 0000 7a14 202a 2053 5041 5253 4954  ....z. * SPARSIT
-00000670: 595f 4641 4354 4f52 3a20 7217 0000 0072  Y_FACTOR: r....r
-00000680: 1000 0000 7211 0000 0072 1200 0000 7214  ....r....r....r.
-00000690: 0000 0072 1600 0000 da14 5245 4752 4553  ...r......REGRES
-000006a0: 5349 4f4e 5f52 4546 4552 454e 4345 da11  SION_REFERENCE..
-000006b0: 5245 4752 4553 5349 4f4e 5f4c 494d 4954  REGRESSION_LIMIT
-000006c0: 53da 0b46 494e 414c 5f55 4e49 5453 da0d  S..FINAL_UNITS..
-000006d0: 4649 4e41 4c5f 4452 4f50 4f55 5446 5472  FINAL_DROPOUTFTr
-000006e0: 1800 0000 290d da05 756e 6974 73da 0c64  ....)...units..d
-000006f0: 726f 706f 7574 5f72 6174 65da 1169 6d70  ropout_rate..imp
-00000700: 6f72 7461 6e63 655f 6661 6374 6f72 da15  ortance_factor..
-00000710: 696d 706f 7274 616e 6365 5f6d 756c 7469  importance_multi
-00000720: 706c 6965 72da 1369 6d70 6f72 7461 6e63  plier..importanc
-00000730: 655f 6368 616e 6e65 6c73 da0f 7370 6172  e_channels..spar
-00000740: 7369 7479 5f66 6163 746f 72da 1472 6567  sity_factor..reg
-00000750: 7265 7373 696f 6e5f 7265 6665 7265 6e63  ression_referenc
-00000760: 65da 1172 6567 7265 7373 696f 6e5f 6c69  e..regression_li
-00000770: 6d69 7473 da0b 6669 6e61 6c5f 756e 6974  mits..final_unit
-00000780: 73da 1266 696e 616c 5f64 726f 706f 7574  s..final_dropout
-00000790: 5f72 6174 65da 1475 7365 5f67 7261 7068  _rate..use_graph
-000007a0: 5f61 7474 7269 6275 7465 73da 1175 7365  _attributes..use
-000007b0: 5f65 6467 655f 6665 6174 7572 6573 da0c  _edge_features..
-000007c0: 636f 6e63 6174 5f68 6561 6473 2903 721c  concat_heads).r.
-000007d0: 0000 0072 0100 0000 7201 0000 00da 0c4f  ...r....r......O
-000007e0: 5054 494d 495a 4552 5f43 4229 05da 046c  PTIMIZER_CB)...l
-000007f0: 6f73 73da 0c6c 6f73 735f 7765 6967 6874  oss..loss_weight
-00000800: 73da 076d 6574 7269 6373 da09 6f70 7469  s..metrics..opti
-00000810: 6d69 7a65 72da 0b72 756e 5f65 6167 6572  mizer..run_eager
-00000820: 6c79 2906 da04 696e 666f da0a 7061 7261  ly)...info..para
-00000830: 6d65 7465 7273 7205 0000 00da 0763 6f6d  metersr......com
-00000840: 7069 6c65 7207 0000 0072 0600 0000 2902  piler....r....).
-00000850: da01 65da 056d 6f64 656c 7224 0000 0072  ..e..modelr$...r
-00000860: 2400 0000 7225 0000 0072 2900 0000 6700  $...r%...r)...g.
-00000870: 0000 7338 0000 000a 0216 0102 0108 0108  ..s8............
-00000880: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00000890: 0102 0102 0108 0106 f304 0f02 0204 0104  ................
-000008a0: 0102 fd06 0504 030a 0102 0106 f504 0dda  ................
-000008b0: 0966 6974 5f6d 6f64 656c 6306 0000 0000  .fit_modelc.....
-000008c0: 0000 0000 0000 0007 0000 000c 0000 0043  ...............C
-000008d0: 0000 0073 3e00 0000 7c01 6a00 7c02 7c03  ...s>...|.j.|.|.
-000008e0: 7c00 6a01 6401 1900 7c00 6a01 6402 1900  |.j.d...|.j.d...
-000008f0: 7c04 7c05 6602 6403 7402 7c00 6a03 6404  |.|.f.d.t.|.j.d.
-00000900: 6405 6406 8d03 6701 6407 6408 8d08 7d06  d.d...g.d.d...}.
-00000910: 7c06 6a04 5300 2909 4eda 0a42 4154 4348  |.j.S.).N..BATCH
-00000920: 5f53 495a 45da 0645 504f 4348 5372 1c00  _SIZE..EPOCHSr..
-00000930: 0000 7213 0000 00da 1f76 616c 5f6f 7574  ..r......val_out
-00000940: 7075 745f 315f 6d65 616e 5f73 7175 6172  put_1_mean_squar
-00000950: 6564 5f65 7272 6f72 2903 da06 6c6f 6767  ed_error)...logg
-00000960: 6572 da0a 6570 6f63 685f 7374 6570 da0a  er..epoch_step..
-00000970: 6964 656e 7469 6669 6572 7201 0000 0029  identifierr....)
-00000980: 06da 0a62 6174 6368 5f73 697a 65da 0665  ...batch_size..e
-00000990: 706f 6368 73da 0f76 616c 6964 6174 696f  pochs..validatio
-000009a0: 6e5f 6461 7461 da0f 7661 6c69 6461 7469  n_data..validati
-000009b0: 6f6e 5f66 7265 71da 0963 616c 6c62 6163  on_freq..callbac
-000009c0: 6b73 da07 7665 7262 6f73 6529 05da 0366  ks..verbose)...f
-000009d0: 6974 7242 0000 0072 0800 0000 724a 0000  itrB...r....rJ..
-000009e0: 00da 0768 6973 746f 7279 2907 7244 0000  ...history).rD..
-000009f0: 0072 4500 0000 da07 785f 7472 6169 6eda  .rE.....x_train.
-00000a00: 0779 5f74 7261 696e da06 785f 7465 7374  .y_train..x_test
-00000a10: da06 795f 7465 7374 7254 0000 0072 2400  ..y_testrT...r$.
-00000a20: 0000 7224 0000 0072 2500 0000 7246 0000  ..r$...r%...rF..
-00000a30: 0089 0000 0073 2000 0000 0402 0201 0201  .....s .........
-00000a40: 0801 0801 0601 0201 0202 0401 0201 0201  ................
-00000a50: 04fd 02ff 0207 06f2 0610 da0b 7175 6572  ............quer
-00000a60: 795f 6d6f 6465 6cda 1369 6e63 6c75 6465  y_model..include
-00000a70: 5f69 6d70 6f72 7461 6e63 6573 6305 0000  _importancesc...
-00000a80: 0000 0000 0000 0000 0008 0000 0003 0000  ................
-00000a90: 0043 0000 0073 2a00 0000 7c00 a000 6401  .C...s*...|...d.
-00000aa0: a101 0100 7c01 7c02 8301 5c03 7d05 7d06  ....|.|...\.}.}.
-00000ab0: 7d07 7c04 7213 7c05 7c06 7c07 6603 5300  }.|.r.|.|.|.f.S.
-00000ac0: 7c05 5300 2902 4e7a 1571 7565 7279 696e  |.S.).Nz.queryin
-00000ad0: 6720 7468 6520 6d6f 6465 6c2e 2e2e 2901  g the model...).
-00000ae0: 7241 0000 0029 0872 4400 0000 7245 0000  rA...).rD...rE..
-00000af0: 00da 0178 da01 7972 5a00 0000 da08 6f75  ...x..yrZ.....ou
-00000b00: 745f 7072 6564 da07 6e69 5f70 7265 64da  t_pred..ni_pred.
-00000b10: 0765 695f 7072 6564 7224 0000 0072 2400  .ei_predr$...r$.
-00000b20: 0000 7225 0000 0072 5900 0000 9e00 0000  ..r%...rY.......
-00000b30: 730a 0000 000a 020e 0104 020a 0104 02da  s...............
-00000b40: 1263 616c 6375 6c61 7465 5f66 6964 656c  .calculate_fidel
-00000b50: 6974 7963 0800 0000 0000 0000 0000 0000  ityc............
-00000b60: 1500 0000 0a00 0000 4300 0000 7358 0100  ........C...sX..
-00000b70: 007c 0064 0119 007d 087c 006a 0064 0219  .|.d...}.|.j.d..
-00000b80: 0074 017c 006a 0064 0319 0083 016b 0372  .t.|.j.d.....k.r
-00000b90: 1364 0467 0153 0074 0274 0383 0144 005d  .d.g.S.t.t...D.]
-00000ba0: 597d 0967 007d 0a7c 0644 005d 147d 0b74  Y}.g.}.|.D.].}.t
-00000bb0: 04a0 057c 0ba1 017d 0c64 047c 0c64 0064  ...|...}.d.|.d.d
-00000bc0: 0085 027c 0966 023c 007c 0aa0 067c 0ca1  ...|.f.<.|...|..
-00000bd0: 0101 0071 1d74 077c 0a83 017d 0d64 0564  ...q.t.|...}.d.d
-00000be0: 0684 007c 017c 037c 0d64 078d 0244 0083  ...|.|.|.d...D..
-00000bf0: 015c 037d 0e7d 0f7d 0f74 087c 0283 0144  .\.}.}.}.t.|...D
-00000c00: 005d 275c 027d 107d 1174 097c 057c 1019  .]'\.}.}.t.|.|..
-00000c10: 0064 0419 0083 017c 0064 087c 089b 0064  .d.....|.d.|...d
-00000c20: 097c 119b 009d 043c 0074 097c 0e7c 1019  .|.....<.t.|.|..
-00000c30: 0064 0419 0083 017c 0064 0a7c 089b 0064  .d.....|.d.|...d
-00000c40: 097c 119b 0064 097c 099b 009d 063c 0071  .|...d.|.....<.q
-00000c50: 4871 1767 007d 127c 0244 005d 347d 1164  Hq.g.}.|.D.]4}.d
-00000c60: 047d 1374 0274 0383 0144 005d 267d 097c  .}.t.t...D.]&}.|
-00000c70: 0064 087c 089b 0064 097c 119b 009d 0419  .d.|...d.|......
-00000c80: 007d 147c 0064 0a7c 089b 0064 097c 119b  .}.|.d.|...d.|..
-00000c90: 0064 097c 099b 009d 0619 007d 0e7c 137c  .d.|.......}.|.|
-00000ca0: 006a 0a64 0319 007c 0919 007c 147c 0e18  .j.d...|...|.|..
-00000cb0: 0014 0037 007d 1371 7d7c 12a0 067c 13a1  ...7.}.q}|...|..
-00000cc0: 0101 0071 757c 1253 0029 0b4e da03 7265  ...qu|.S.).N..re
-00000cd0: 7072 1600 0000 da12 4348 414e 4e45 4c5f  pr......CHANNEL_
-00000ce0: 4449 5245 4354 494f 4e53 7201 0000 0063  DIRECTIONSr....c
-00000cf0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000d00: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00000d10: 005d 067d 017c 01a0 00a1 0091 0271 0253  .].}.|.......q.S
-00000d20: 0072 2400 0000 2901 da05 6e75 6d70 7929  .r$...)...numpy)
-00000d30: 02da 022e 30da 0176 7224 0000 0072 2400  ....0..vr$...r$.
-00000d40: 0000 7225 0000 00da 0a3c 6c69 7374 636f  ..r%.....<listco
-00000d50: 6d70 3ebe 0000 0073 0200 0000 1400 7a26  mp>....s......z&
-00000d60: 6361 6c63 756c 6174 655f 6669 6465 6c69  calculate_fideli
-00000d70: 7479 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ty.<locals>.<lis
-00000d80: 7463 6f6d 703e 2901 da15 6e6f 6465 5f69  tcomp>)...node_i
-00000d90: 6d70 6f72 7461 6e63 6573 5f6d 6173 6b7a  mportances_maskz
-00000da0: 096f 7574 2f70 7265 642f fa01 2f7a 0b6f  .out/pred/../z.o
-00000db0: 7574 2f6d 6173 6b65 642f 290b da01 70da  ut/masked/)...p.
-00000dc0: 036c 656e da05 7261 6e67 6572 1600 0000  .len..ranger....
-00000dd0: da02 6e70 da09 6f6e 6573 5f6c 696b 65da  ..np..ones_like.
-00000de0: 0661 7070 656e 6472 0400 0000 da09 656e  .appendr......en
-00000df0: 756d 6572 6174 65da 0566 6c6f 6174 7242  umerate..floatrB
-00000e00: 0000 0029 1572 4400 0000 7245 0000 00da  ...).rD...rE....
-00000e10: 0c69 6e64 6963 6573 5f74 7275 65da 0678  .indices_true..x
-00000e20: 5f74 7275 65da 0679 5f74 7275 6572 5d00  _true..y_truer].
-00000e30: 0000 725e 0000 0072 5f00 0000 7261 0000  ..r^...r_...ra..
-00000e40: 00da 016b da05 6d61 736b 73da 026e 69da  ...k..masks..ni.
-00000e50: 046d 6173 6bda 0c6d 6173 6b73 5f74 656e  .mask..masks_ten
-00000e60: 736f 72da 0a6f 7574 5f6d 6173 6b65 64da  sor..out_masked.
-00000e70: 015f da01 63da 0569 6e64 6578 da0a 6669  ._..c..index..fi
-00000e80: 6465 6c69 7469 6573 da08 6669 6465 6c69  delities..fideli
-00000e90: 7479 da03 6f75 7472 2400 0000 7224 0000  ty..outr$...r$..
-00000ea0: 0072 2500 0000 7260 0000 00a9 0000 0073  .r%...r`.......s
-00000eb0: 3400 0000 0802 1802 0601 0c07 0402 0801  4...............
-00000ec0: 0a01 1001 0c01 0802 0601 0a01 0cff 1003  ................
-00000ed0: 2001 2801 02fe 0404 0801 0402 0c01 1401   .(.............
-00000ee0: 1a01 1c01 0c02 0402 da0a 7361 7665 5f6d  ..........save_m
-00000ef0: 6f64 656c 6302 0000 0000 0000 0000 0000  odelc...........
-00000f00: 0003 0000 0004 0000 0043 0000 0073 3000  .........C...s0.
-00000f10: 0000 7c00 a000 6401 a101 0100 7401 6a02  ..|...d.....t.j.
-00000f20: a003 7c00 6a02 6402 a102 7d02 7c02 7c00  ..|.j.d...}.|.|.
-00000f30: 6403 3c00 7c01 a004 7c02 a101 0100 6400  d.<.|...|.....d.
-00000f40: 5300 2904 4e7a 1973 6176 696e 6720 7468  S.).Nz.saving th
-00000f50: 6520 4d45 4741 4e20 6d6f 6465 6c2e 2e2e  e MEGAN model...
-00000f60: 7245 0000 00da 0a6d 6f64 656c 5f70 6174  rE.....model_pat
-00000f70: 6829 0572 4100 0000 da02 6f73 da04 7061  h).rA.....os..pa
-00000f80: 7468 da04 6a6f 696e da04 7361 7665 2903  th..join..save).
-00000f90: 7244 0000 0072 4500 0000 7281 0000 0072  rD...rE...r....r
-00000fa0: 2400 0000 7224 0000 0072 2500 0000 7280  $...r$...r%...r.
-00000fb0: 0000 00d2 0000 0073 0800 0000 0a02 1001  .......s........
-00000fc0: 0801 0e01 2901 5429 44da 075f 5f64 6f63  ....).T)D..__doc
-00000fd0: 5f5f 7282 0000 00da 0770 6174 686c 6962  __r......pathlib
-00000fe0: da06 7479 7069 6e67 da01 74da 0a74 656e  ..typing..t..ten
-00000ff0: 736f 7266 6c6f 77da 0274 66da 1074 656e  sorflow..tf..ten
-00001000: 736f 7266 6c6f 772e 6b65 7261 73da 056b  sorflow.keras..k
-00001010: 6572 6173 7221 0000 0072 6300 0000 726c  erasr!...rc...rl
-00001020: 0000 00da 0c70 7963 6f6d 6578 2e75 7469  .....pycomex.uti
-00001030: 6c72 0200 0000 da12 7079 636f 6d65 782e  lr......pycomex.
-00001040: 6578 7065 7269 6d65 6e74 7203 0000 00da  experimentr.....
-00001050: 106b 6763 6e6e 2e64 6174 612e 7574 696c  .kgcnn.data.util
-00001060: 7372 0400 0000 da1e 6772 6170 685f 6174  sr......graph_at
-00001070: 7465 6e74 696f 6e5f 7374 7564 656e 742e  tention_student.
-00001080: 6d6f 6465 6c73 7205 0000 00da 2067 7261  modelsr..... gra
-00001090: 7068 5f61 7474 656e 7469 6f6e 5f73 7475  ph_attention_stu
-000010a0: 6465 6e74 2e74 7261 696e 696e 6772 0600  dent.trainingr..
-000010b0: 0000 7207 0000 0072 0800 0000 720a 0000  ..r....r....r...
-000010c0: 00da 084f 7074 696f 6e61 6cda 0373 7472  ...Optional..str
-000010d0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-000010e0: 5f72 0c00 0000 720e 0000 0072 1000 0000  _r....r....r....
-000010f0: da04 4c69 7374 da03 696e 7472 1100 0000  ..List..intr....
-00001100: 7270 0000 0072 1200 0000 7214 0000 0072  rp...r....r....r
-00001110: 1600 0000 7217 0000 0072 1800 0000 da04  ....r....r......
-00001120: 626f 6f6c 722a 0000 0072 2b00 0000 7262  boolr*...r+...rb
-00001130: 0000 0072 2c00 0000 722d 0000 0072 4800  ...r,...r-...rH.
-00001140: 0000 723b 0000 00da 1949 4d50 4f52 5441  ..r;.....IMPORTA
-00001150: 4e43 455f 4348 414e 4e45 4c5f 4c41 4245  NCE_CHANNEL_LABE
-00001160: 4c53 da04 5061 7468 da08 5f5f 6669 6c65  LS..Path..__file
-00001170: 5f5f da06 7061 7265 6e74 da08 6162 736f  __..parent..abso
-00001180: 6c75 7465 da04 5041 5448 7283 0000 0072  lute..PATHr....r
-00001190: 8400 0000 da0f 4558 5045 5249 4d45 4e54  ......EXPERIMENT
-000011a0: 5f50 4154 48da 0942 4153 455f 5041 5448  _PATH..BASE_PATH
-000011b0: da09 4e41 4d45 5350 4143 45da 0544 4542  ..NAMESPACE..DEB
-000011c0: 5547 da07 676c 6f62 616c 73da 0273 65da  UG..globals..se.
-000011d0: 0468 6f6f 6b72 2900 0000 7246 0000 0072  .hookr)...rF...r
-000011e0: 5900 0000 7260 0000 0072 8000 0000 7224  Y...r`...r....r$
-000011f0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
-00001200: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001210: 7364 0000 0006 0008 0608 0108 0108 020c  sd..............
-00001220: 0108 010c 010c 010c 010c 0210 010c 0112  ................
-00001230: 0612 010c 0616 040c 040c 050c 030c 060c  ................
-00001240: 040c 0404 060a 0102 0302 0106 fe08 0904  ................
-00001250: 0304 0308 0108 0410 040e 0104 0104 0104  ................
-00001260: 011e 0108 020a 0108 210a 0108 1412 0108  ........!.......
-00001270: 0a0a 0108 280c 0154 92                   ....(..T.
+00000140: 3c00 6401 6701 5a29 641d 641e 6702 6701  <.d.g.Z)d.d.g.g.
+00000150: 5a2a 641f 641f 6702 6701 5a2b 6420 641f  Z*d.d.g.g.Z+d d.
+00000160: 6421 9c02 5a2c 6700 6422 a201 5a2d 6411  d!..Z,g.d"..Z-d.
+00000170: 5a2e 6423 5a2f 6424 6425 8400 5a30 6426  Z.d#Z/d$d%..Z0d&
+00000180: 6427 6702 5a31 6502 a032 6533 a101 6a34  d'g.Z1e..2e3..j4
+00000190: a035 a100 5a36 6501 6a37 a038 6536 6428  .5..Z6e.j7.8e6d(
+000001a0: a102 5a39 6536 5a3a 6429 5a3b 642a 5a3c  ..Z9e6Z:d)Z;d*Z<
+000001b0: 650d 8300 8f5d 0100 650f 6539 653a 653b  e....]..e.e9e:e;
+000001c0: 653d 8300 8304 0400 5a3e 8f39 0100 653e  e=......Z>.9..e>
+000001d0: a03f 642b a101 642c 642b 8400 8301 5a40  .?d+..d,d+....Z@
+000001e0: 653e a03f 642d a101 642e 642d 8400 8301  e>.?d-..d.d-....
+000001f0: 5a41 653e a03f 642f a101 6436 6430 6528  ZAe>.?d/..d6d0e(
+00000200: 6602 6431 642f 8405 8301 5a42 653e a03f  f.d1d/....ZBe>.?
+00000210: 6432 a101 6433 6432 8400 8301 5a43 653e  d2..d3d2....ZCe>
+00000220: a03f 6434 a101 6435 6434 8400 8301 5a44  .?d4..d5d4....ZD
+00000230: 5700 6402 0400 0400 8303 0100 6e11 3100  W.d.........n.1.
+00000240: 9001 730c 7701 0100 0100 0100 5900 0100  ..s.w.......Y...
+00000250: 5700 6402 0400 0400 8303 0100 6402 5300  W.d.........d.S.
+00000260: 5700 6402 0400 0400 8303 0100 6402 5300  W.d.........d.S.
+00000270: 3100 9001 7325 7701 0100 0100 0100 5900  1...s%w.......Y.
+00000280: 0100 6402 5300 2937 7a13 0a0a 4348 414e  ..d.S.)7z...CHAN
+00000290: 4745 4c4f 470a 0a30 2e31 2e30 0ae9 0000  GELOG..0.1.0....
+000002a0: 0000 4e29 01da 0953 6b69 7070 6162 6c65  ..N)...Skippable
+000002b0: 2901 da0d 5375 6245 7870 6572 696d 656e  )...SubExperimen
+000002c0: 7429 01da 1f72 6167 6765 645f 7465 6e73  t)...ragged_tens
+000002d0: 6f72 5f66 726f 6d5f 6e65 7374 6564 5f6e  or_from_nested_n
+000002e0: 756d 7079 2901 da05 4d65 6761 6e29 02da  umpy)...Megan)..
+000002f0: 064e 6f4c 6f73 73da 036d 7365 2901 da13  .NoLoss..mse)...
+00000300: 4c6f 6750 726f 6772 6573 7343 616c 6c62  LogProgressCallb
+00000310: 6163 6bda 126e 6f64 655f 696d 706f 7274  ack..node_import
+00000320: 616e 6365 735f 32da 144e 4f44 455f 494d  ances_2..NODE_IM
+00000330: 504f 5254 414e 4345 535f 4b45 59da 1265  PORTANCES_KEY..e
+00000340: 6467 655f 696d 706f 7274 616e 6365 735f  dge_importances_
+00000350: 32da 1445 4447 455f 494d 504f 5254 414e  2..EDGE_IMPORTAN
+00000360: 4345 535f 4b45 59da 054d 4547 414e da0a  CES_KEY..MEGAN..
+00000370: 4d4f 4445 4c5f 4e41 4d45 2903 e920 0000  MODEL_NAME).. ..
+00000380: 0072 0f00 0000 720f 0000 00da 0555 4e49  .r....r......UNI
+00000390: 5453 6700 0000 0000 0000 00da 0c44 524f  TSg..........DRO
+000003a0: 504f 5554 5f52 4154 4567 0000 0000 0000  POUT_RATEg......
+000003b0: f03f da11 494d 504f 5254 414e 4345 5f46  .?..IMPORTANCE_F
+000003c0: 4143 544f 52e9 0500 0000 da15 494d 504f  ACTOR.......IMPO
+000003d0: 5254 414e 4345 5f4d 554c 5449 504c 4945  RTANCE_MULTIPLIE
+000003e0: 52e9 0200 0000 da13 494d 504f 5254 414e  R.......IMPORTAN
+000003f0: 4345 5f43 4841 4e4e 454c 5367 0000 0000  CE_CHANNELSg....
+00000400: 0000 1440 da0f 5350 4152 5349 5459 5f46  ...@..SPARSITY_F
+00000410: 4143 544f 5246 da0c 434f 4e43 4154 5f48  ACTORF..CONCAT_H
+00000420: 4541 4453 e9fd ffff ffe9 0300 0000 e901  EADS............
+00000430: 0000 00e9 ffff ffff 2902 7201 0000 0072  ........).r....r
+00000440: 1b00 0000 2903 e93c 0000 00e9 1400 0000  ....)..<........
+00000450: 721b 0000 00e9 fa00 0000 6300 0000 0000  r.........c.....
+00000460: 0000 0000 0000 0000 0000 0003 0000 0043  ...............C
+00000470: 0000 0073 0e00 0000 7400 6a01 6a02 6401  ...s....t.j.j.d.
+00000480: 6402 8d01 5300 2903 4e67 fca9 f1d2 4d62  d...S.).Ng....Mb
+00000490: 503f 2901 da0d 6c65 6172 6e69 6e67 5f72  P?)...learning_r
+000004a0: 6174 6529 03da 026b 73da 0a6f 7074 696d  ate)...ks..optim
+000004b0: 697a 6572 73da 054e 6164 616d a900 7224  izers..Nadam..r$
+000004c0: 0000 0072 2400 0000 fa66 2f6d 6564 6961  ...r$....f/media
+000004d0: 2f73 7364 2f50 726f 6772 616d 6d69 6e67  /ssd/Programming
+000004e0: 2f67 7261 7068 5f61 7474 656e 7469 6f6e  /graph_attention
+000004f0: 5f73 7475 6465 6e74 2f67 7261 7068 5f61  _student/graph_a
+00000500: 7474 656e 7469 6f6e 5f73 7475 6465 6e74  ttention_student
+00000510: 2f65 7870 6572 696d 656e 7473 2f76 6764  /experiments/vgd
+00000520: 5f73 696e 676c 655f 6d65 6761 6e2e 7079  _single_megan.py
+00000530: da08 3c6c 616d 6264 613e 5900 0000 7302  ..<lambda>Y...s.
+00000540: 0000 000e 0072 2600 0000 da08 6e65 6761  .....r&.....nega
+00000550: 7469 7665 da08 706f 7369 7469 7665 7a0d  tive..positivez.
+00000560: 7667 645f 7369 6e67 6c65 2e70 797a 1872  vgd_single.pyz.r
+00000570: 6573 756c 7473 2f76 6764 5f73 696e 676c  esults/vgd_singl
+00000580: 655f 6d65 6761 6e54 da0c 6372 6561 7465  e_meganT..create
+00000590: 5f6d 6f64 656c 6301 0000 0000 0000 0000  _modelc.........
+000005a0: 0000 0002 0000 0010 0000 0043 0000 0073  ...........C...s
+000005b0: bc00 0000 7c00 a000 6401 a101 0100 7c00  ....|...d.....|.
+000005c0: a000 6402 7c00 6a01 6403 1900 9b00 9d02  ..d.|.j.d.......
+000005d0: a101 0100 7402 7c00 6a01 6404 1900 7c00  ....t.|.j.d...|.
+000005e0: 6a01 6405 1900 7c00 6a01 6406 1900 7c00  j.d...|.j.d...|.
+000005f0: 6a01 6407 1900 7c00 6a01 6408 1900 7c00  j.d...|.j.d...|.
+00000600: 6a01 6403 1900 7c00 6a01 6409 1900 7c00  j.d...|.j.d...|.
+00000610: 6a01 640a 1900 7c00 6a01 640b 1900 7c00  j.d...|.j.d...|.
+00000620: 6a01 640c 1900 7c00 6a01 640d 1900 640e  j.d...|.j.d...d.
+00000630: 640f 7c00 6a01 6410 1900 6411 8d0e 7d01  d.|.j.d...d...}.
+00000640: 7c01 6a03 7404 7405 8300 7405 8300 6703  |.j.t.t...t...g.
+00000650: 6700 6412 a201 7404 6701 7c00 6a01 6413  g.d...t.g.|.j.d.
+00000660: 1900 8300 640e 6414 8d05 0100 7c01 5300  ....d.d.....|.S.
+00000670: 2915 4e72 0d00 0000 7a14 202a 2053 5041  ).Nr....z. * SPA
+00000680: 5253 4954 595f 4641 4354 4f52 3a20 7217  RSITY_FACTOR: r.
+00000690: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
+000006a0: 0000 7214 0000 0072 1600 0000 da14 5245  ..r....r......RE
+000006b0: 4752 4553 5349 4f4e 5f52 4546 4552 454e  GRESSION_REFEREN
+000006c0: 4345 da11 5245 4752 4553 5349 4f4e 5f4c  CE..REGRESSION_L
+000006d0: 494d 4954 53da 1252 4547 5245 5353 494f  IMITS..REGRESSIO
+000006e0: 4e5f 5745 4947 4854 53da 0b46 494e 414c  N_WEIGHTS..FINAL
+000006f0: 5f55 4e49 5453 da0d 4649 4e41 4c5f 4452  _UNITS..FINAL_DR
+00000700: 4f50 4f55 5446 5472 1800 0000 290e da05  OPOUTFTr....)...
+00000710: 756e 6974 73da 0c64 726f 706f 7574 5f72  units..dropout_r
+00000720: 6174 65da 1169 6d70 6f72 7461 6e63 655f  ate..importance_
+00000730: 6661 6374 6f72 da15 696d 706f 7274 616e  factor..importan
+00000740: 6365 5f6d 756c 7469 706c 6965 72da 1369  ce_multiplier..i
+00000750: 6d70 6f72 7461 6e63 655f 6368 616e 6e65  mportance_channe
+00000760: 6c73 da0f 7370 6172 7369 7479 5f66 6163  ls..sparsity_fac
+00000770: 746f 72da 1472 6567 7265 7373 696f 6e5f  tor..regression_
+00000780: 7265 6665 7265 6e63 65da 1172 6567 7265  reference..regre
+00000790: 7373 696f 6e5f 6c69 6d69 7473 da12 7265  ssion_limits..re
+000007a0: 6772 6573 7369 6f6e 5f77 6569 6768 7473  gression_weights
+000007b0: da0b 6669 6e61 6c5f 756e 6974 73da 1266  ..final_units..f
+000007c0: 696e 616c 5f64 726f 706f 7574 5f72 6174  inal_dropout_rat
+000007d0: 65da 1475 7365 5f67 7261 7068 5f61 7474  e..use_graph_att
+000007e0: 7269 6275 7465 73da 1175 7365 5f65 6467  ributes..use_edg
+000007f0: 655f 6665 6174 7572 6573 da0c 636f 6e63  e_features..conc
+00000800: 6174 5f68 6561 6473 2903 721b 0000 0072  at_heads).r....r
+00000810: 0100 0000 7201 0000 00da 0c4f 5054 494d  ....r......OPTIM
+00000820: 495a 4552 5f43 4229 05da 046c 6f73 73da  IZER_CB)...loss.
+00000830: 0c6c 6f73 735f 7765 6967 6874 73da 076d  .loss_weights..m
+00000840: 6574 7269 6373 da09 6f70 7469 6d69 7a65  etrics..optimize
+00000850: 72da 0b72 756e 5f65 6167 6572 6c79 2906  r..run_eagerly).
+00000860: da04 696e 666f da0a 7061 7261 6d65 7465  ..info..paramete
+00000870: 7273 7205 0000 00da 0763 6f6d 7069 6c65  rsr......compile
+00000880: 7207 0000 0072 0600 0000 2902 da01 65da  r....r....)...e.
+00000890: 056d 6f64 656c 7224 0000 0072 2400 0000  .modelr$...r$...
+000008a0: 7225 0000 0072 2900 0000 6800 0000 733a  r%...r)...h...s:
+000008b0: 0000 000a 0216 0102 0108 0108 0108 0108  ................
+000008c0: 0108 0108 0108 0108 0108 0108 0108 0102  ................
+000008d0: 0102 0108 0106 f204 1002 0204 0104 0102  ................
+000008e0: fd06 0504 030a 0102 0106 f504 0dda 0966  ...............f
+000008f0: 6974 5f6d 6f64 656c 6306 0000 0000 0000  it_modelc.......
+00000900: 0000 0000 0007 0000 000c 0000 0043 0000  .............C..
+00000910: 0073 3e00 0000 7c01 6a00 7c02 7c03 7c00  .s>...|.j.|.|.|.
+00000920: 6a01 6401 1900 7c00 6a01 6402 1900 7c04  j.d...|.j.d...|.
+00000930: 7c05 6602 6403 7402 7c00 6a03 6404 6405  |.f.d.t.|.j.d.d.
+00000940: 6406 8d03 6701 6407 6408 8d08 7d06 7c06  d...g.d.d...}.|.
+00000950: 6a04 5300 2909 4eda 0a42 4154 4348 5f53  j.S.).N..BATCH_S
+00000960: 495a 45da 0645 504f 4348 5372 1b00 0000  IZE..EPOCHSr....
+00000970: 7213 0000 00da 1f76 616c 5f6f 7574 7075  r......val_outpu
+00000980: 745f 315f 6d65 616e 5f73 7175 6172 6564  t_1_mean_squared
+00000990: 5f65 7272 6f72 2903 da06 6c6f 6767 6572  _error)...logger
+000009a0: da0a 6570 6f63 685f 7374 6570 da0a 6964  ..epoch_step..id
+000009b0: 656e 7469 6669 6572 7201 0000 0029 06da  entifierr....)..
+000009c0: 0a62 6174 6368 5f73 697a 65da 0665 706f  .batch_size..epo
+000009d0: 6368 73da 0f76 616c 6964 6174 696f 6e5f  chs..validation_
+000009e0: 6461 7461 da0f 7661 6c69 6461 7469 6f6e  data..validation
+000009f0: 5f66 7265 71da 0963 616c 6c62 6163 6b73  _freq..callbacks
+00000a00: da07 7665 7262 6f73 6529 05da 0366 6974  ..verbose)...fit
+00000a10: 7244 0000 0072 0800 0000 724c 0000 00da  rD...r....rL....
+00000a20: 0768 6973 746f 7279 2907 7246 0000 0072  .history).rF...r
+00000a30: 4700 0000 da07 785f 7472 6169 6eda 0779  G.....x_train..y
+00000a40: 5f74 7261 696e da06 785f 7465 7374 da06  _train..x_test..
+00000a50: 795f 7465 7374 7256 0000 0072 2400 0000  y_testrV...r$...
+00000a60: 7224 0000 0072 2500 0000 7248 0000 008b  r$...r%...rH....
+00000a70: 0000 0073 2000 0000 0402 0201 0201 0801  ...s ...........
+00000a80: 0801 0601 0201 0202 0401 0201 0201 04fd  ................
+00000a90: 02ff 0207 06f2 0610 da0b 7175 6572 795f  ..........query_
+00000aa0: 6d6f 6465 6cda 1369 6e63 6c75 6465 5f69  model..include_i
+00000ab0: 6d70 6f72 7461 6e63 6573 6305 0000 0000  mportancesc.....
+00000ac0: 0000 0000 0000 0008 0000 0003 0000 0043  ...............C
+00000ad0: 0000 0073 2a00 0000 7c00 a000 6401 a101  ...s*...|...d...
+00000ae0: 0100 7c01 7c02 8301 5c03 7d05 7d06 7d07  ..|.|...\.}.}.}.
+00000af0: 7c04 7213 7c05 7c06 7c07 6603 5300 7c05  |.r.|.|.|.f.S.|.
+00000b00: 5300 2902 4e7a 1571 7565 7279 696e 6720  S.).Nz.querying 
+00000b10: 7468 6520 6d6f 6465 6c2e 2e2e 2901 7243  the model...).rC
+00000b20: 0000 0029 0872 4600 0000 7247 0000 00da  ...).rF...rG....
+00000b30: 0178 da01 7972 5c00 0000 da08 6f75 745f  .x..yr\.....out_
+00000b40: 7072 6564 da07 6e69 5f70 7265 64da 0765  pred..ni_pred..e
+00000b50: 695f 7072 6564 7224 0000 0072 2400 0000  i_predr$...r$...
+00000b60: 7225 0000 0072 5b00 0000 a000 0000 730a  r%...r[.......s.
+00000b70: 0000 000a 020e 0104 020a 0104 02da 1263  ...............c
+00000b80: 616c 6375 6c61 7465 5f66 6964 656c 6974  alculate_fidelit
+00000b90: 7963 0800 0000 0000 0000 0000 0000 1500  yc..............
+00000ba0: 0000 0a00 0000 4300 0000 7358 0100 007c  ......C...sX...|
+00000bb0: 0064 0119 007d 087c 006a 0064 0219 0074  .d...}.|.j.d...t
+00000bc0: 017c 006a 0064 0319 0083 016b 0372 1364  .|.j.d.....k.r.d
+00000bd0: 0467 0153 0074 0274 0383 0144 005d 597d  .g.S.t.t...D.]Y}
+00000be0: 0967 007d 0a7c 0644 005d 147d 0b74 04a0  .g.}.|.D.].}.t..
+00000bf0: 057c 0ba1 017d 0c64 047c 0c64 0064 0085  .|...}.d.|.d.d..
+00000c00: 027c 0966 023c 007c 0aa0 067c 0ca1 0101  .|.f.<.|...|....
+00000c10: 0071 1d74 077c 0a83 017d 0d64 0564 0684  .q.t.|...}.d.d..
+00000c20: 007c 017c 037c 0d64 078d 0244 0083 015c  .|.|.|.d...D...\
+00000c30: 037d 0e7d 0f7d 0f74 087c 0283 0144 005d  .}.}.}.t.|...D.]
+00000c40: 275c 027d 107d 1174 097c 057c 1019 0064  '\.}.}.t.|.|...d
+00000c50: 0419 0083 017c 0064 087c 089b 0064 097c  .....|.d.|...d.|
+00000c60: 119b 009d 043c 0074 097c 0e7c 1019 0064  .....<.t.|.|...d
+00000c70: 0419 0083 017c 0064 0a7c 089b 0064 097c  .....|.d.|...d.|
+00000c80: 119b 0064 097c 099b 009d 063c 0071 4871  ...d.|.....<.qHq
+00000c90: 1767 007d 127c 0244 005d 347d 1164 047d  .g.}.|.D.]4}.d.}
+00000ca0: 1374 0274 0383 0144 005d 267d 097c 0064  .t.t...D.]&}.|.d
+00000cb0: 087c 089b 0064 097c 119b 009d 0419 007d  .|...d.|.......}
+00000cc0: 147c 0064 0a7c 089b 0064 097c 119b 0064  .|.d.|...d.|...d
+00000cd0: 097c 099b 009d 0619 007d 0e7c 137c 006a  .|.......}.|.|.j
+00000ce0: 0a64 0319 007c 0919 007c 147c 0e18 0014  .d...|...|.|....
+00000cf0: 0037 007d 1371 7d7c 12a0 067c 13a1 0101  .7.}.q}|...|....
+00000d00: 0071 757c 1253 0029 0b4e da03 7265 7072  .qu|.S.).N..repr
+00000d10: 1600 0000 da12 4348 414e 4e45 4c5f 4449  ......CHANNEL_DI
+00000d20: 5245 4354 494f 4e53 7201 0000 0063 0100  RECTIONSr....c..
+00000d30: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000d40: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
+00000d50: 067d 017c 01a0 00a1 0091 0271 0253 0072  .}.|.......q.S.r
+00000d60: 2400 0000 2901 da05 6e75 6d70 7929 02da  $...)...numpy)..
+00000d70: 022e 30da 0176 7224 0000 0072 2400 0000  ..0..vr$...r$...
+00000d80: 7225 0000 00da 0a3c 6c69 7374 636f 6d70  r%.....<listcomp
+00000d90: 3ec0 0000 0073 0200 0000 1400 7a26 6361  >....s......z&ca
+00000da0: 6c63 756c 6174 655f 6669 6465 6c69 7479  lculate_fidelity
+00000db0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000dc0: 6f6d 703e 2901 da15 6e6f 6465 5f69 6d70  omp>)...node_imp
+00000dd0: 6f72 7461 6e63 6573 5f6d 6173 6b7a 096f  ortances_maskz.o
+00000de0: 7574 2f70 7265 642f fa01 2f7a 0b6f 7574  ut/pred/../z.out
+00000df0: 2f6d 6173 6b65 642f 290b da01 70da 036c  /masked/)...p..l
+00000e00: 656e da05 7261 6e67 6572 1600 0000 da02  en..ranger......
+00000e10: 6e70 da09 6f6e 6573 5f6c 696b 65da 0661  np..ones_like..a
+00000e20: 7070 656e 6472 0400 0000 da09 656e 756d  ppendr......enum
+00000e30: 6572 6174 65da 0566 6c6f 6174 7244 0000  erate..floatrD..
+00000e40: 0029 1572 4600 0000 7247 0000 00da 0c69  .).rF...rG.....i
+00000e50: 6e64 6963 6573 5f74 7275 65da 0678 5f74  ndices_true..x_t
+00000e60: 7275 65da 0679 5f74 7275 6572 5f00 0000  rue..y_truer_...
+00000e70: 7260 0000 0072 6100 0000 7263 0000 00da  r`...ra...rc....
+00000e80: 016b da05 6d61 736b 73da 026e 69da 046d  .k..masks..ni..m
+00000e90: 6173 6bda 0c6d 6173 6b73 5f74 656e 736f  ask..masks_tenso
+00000ea0: 72da 0a6f 7574 5f6d 6173 6b65 64da 015f  r..out_masked.._
+00000eb0: da01 63da 0569 6e64 6578 da0a 6669 6465  ..c..index..fide
+00000ec0: 6c69 7469 6573 da08 6669 6465 6c69 7479  lities..fidelity
+00000ed0: da03 6f75 7472 2400 0000 7224 0000 0072  ..outr$...r$...r
+00000ee0: 2500 0000 7262 0000 00ab 0000 0073 3400  %...rb.......s4.
+00000ef0: 0000 0802 1802 0601 0c07 0402 0801 0a01  ................
+00000f00: 1001 0c01 0802 0601 0a01 0cff 1003 2001  .............. .
+00000f10: 2801 02fe 0404 0801 0402 0c01 1401 1a01  (...............
+00000f20: 1c01 0c02 0402 da0a 7361 7665 5f6d 6f64  ........save_mod
+00000f30: 656c 6302 0000 0000 0000 0000 0000 0003  elc.............
+00000f40: 0000 0004 0000 0043 0000 0073 3000 0000  .......C...s0...
+00000f50: 7c00 a000 6401 a101 0100 7401 6a02 a003  |...d.....t.j...
+00000f60: 7c00 6a02 6402 a102 7d02 7c02 7c00 6403  |.j.d...}.|.|.d.
+00000f70: 3c00 7c01 a004 7c02 a101 0100 6400 5300  <.|...|.....d.S.
+00000f80: 2904 4e7a 1973 6176 696e 6720 7468 6520  ).Nz.saving the 
+00000f90: 4d45 4741 4e20 6d6f 6465 6c2e 2e2e 7247  MEGAN model...rG
+00000fa0: 0000 00da 0a6d 6f64 656c 5f70 6174 6829  .....model_path)
+00000fb0: 0572 4300 0000 da02 6f73 da04 7061 7468  .rC.....os..path
+00000fc0: da04 6a6f 696e da04 7361 7665 2903 7246  ..join..save).rF
+00000fd0: 0000 0072 4700 0000 7283 0000 0072 2400  ...rG...r....r$.
+00000fe0: 0000 7224 0000 0072 2500 0000 7282 0000  ..r$...r%...r...
+00000ff0: 00d4 0000 0073 0800 0000 0a02 1001 0801  .....s..........
+00001000: 0e01 2901 5429 45da 075f 5f64 6f63 5f5f  ..).T)E..__doc__
+00001010: 7284 0000 00da 0770 6174 686c 6962 da06  r......pathlib..
+00001020: 7479 7069 6e67 da01 74da 0a74 656e 736f  typing..t..tenso
+00001030: 7266 6c6f 77da 0274 66da 1074 656e 736f  rflow..tf..tenso
+00001040: 7266 6c6f 772e 6b65 7261 73da 056b 6572  rflow.keras..ker
+00001050: 6173 7221 0000 0072 6500 0000 726e 0000  asr!...re...rn..
+00001060: 00da 0c70 7963 6f6d 6578 2e75 7469 6c72  ...pycomex.utilr
+00001070: 0200 0000 da12 7079 636f 6d65 782e 6578  ......pycomex.ex
+00001080: 7065 7269 6d65 6e74 7203 0000 00da 106b  perimentr......k
+00001090: 6763 6e6e 2e64 6174 612e 7574 696c 7372  gcnn.data.utilsr
+000010a0: 0400 0000 da1e 6772 6170 685f 6174 7465  ......graph_atte
+000010b0: 6e74 696f 6e5f 7374 7564 656e 742e 6d6f  ntion_student.mo
+000010c0: 6465 6c73 7205 0000 00da 2067 7261 7068  delsr..... graph
+000010d0: 5f61 7474 656e 7469 6f6e 5f73 7475 6465  _attention_stude
+000010e0: 6e74 2e74 7261 696e 696e 6772 0600 0000  nt.trainingr....
+000010f0: 7207 0000 0072 0800 0000 720a 0000 00da  r....r....r.....
+00001100: 084f 7074 696f 6e61 6cda 0373 7472 da0f  .Optional..str..
+00001110: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
+00001120: 0c00 0000 720e 0000 0072 1000 0000 da04  ....r....r......
+00001130: 4c69 7374 da03 696e 7472 1100 0000 7272  List..intr....rr
+00001140: 0000 0072 1200 0000 7214 0000 0072 1600  ...r....r....r..
+00001150: 0000 7217 0000 0072 1800 0000 da04 626f  ..r....r......bo
+00001160: 6f6c 722a 0000 0072 2b00 0000 722c 0000  olr*...r+...r,..
+00001170: 0072 6400 0000 722d 0000 0072 2e00 0000  .rd...r-...r....
+00001180: 724a 0000 0072 3d00 0000 da19 494d 504f  rJ...r=.....IMPO
+00001190: 5254 414e 4345 5f43 4841 4e4e 454c 5f4c  RTANCE_CHANNEL_L
+000011a0: 4142 454c 53da 0450 6174 68da 085f 5f66  ABELS..Path..__f
+000011b0: 696c 655f 5fda 0670 6172 656e 74da 0861  ile__..parent..a
+000011c0: 6273 6f6c 7574 65da 0450 4154 4872 8500  bsolute..PATHr..
+000011d0: 0000 7286 0000 00da 0f45 5850 4552 494d  ..r......EXPERIM
+000011e0: 454e 545f 5041 5448 da09 4241 5345 5f50  ENT_PATH..BASE_P
+000011f0: 4154 48da 094e 414d 4553 5041 4345 da05  ATH..NAMESPACE..
+00001200: 4445 4255 47da 0767 6c6f 6261 6c73 da02  DEBUG..globals..
+00001210: 7365 da04 686f 6f6b 7229 0000 0072 4800  se..hookr)...rH.
+00001220: 0000 725b 0000 0072 6200 0000 7282 0000  ..r[...rb...r...
+00001230: 0072 2400 0000 7224 0000 0072 2400 0000  .r$...r$...r$...
+00001240: 7225 0000 00da 083c 6d6f 6475 6c65 3e01  r%.....<module>.
+00001250: 0000 0073 6600 0000 0600 0806 0801 0801  ...sf...........
+00001260: 0802 0c01 0801 0c01 0c01 0c01 0c02 1001  ................
+00001270: 0c01 1206 1201 0c06 1604 0c04 0c05 0c03  ................
+00001280: 0c06 0c04 0c04 0606 0a01 0a01 0203 0201  ................
+00001290: 06fe 0809 0403 0403 0801 0804 1004 0e01  ................
+000012a0: 0401 0401 0401 1e01 0802 0a01 0822 0a01  ............."..
+000012b0: 0814 1201 080a 0a01 0828 0c01 5491       .........(..T.
```

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/process_aqsoldb.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/process_aqsoldb.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/rb_motifs_multi.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/rb_motifs_multi.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/rb_motifs_single.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/rb_motifs_single.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_classification.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_classification.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_classification_megan.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_classification_megan.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_posthoc.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_posthoc.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised_multi.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised_multi.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised_single.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised_single.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_megan.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_megan.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,17 @@
 # average will be used to combine the results.
 CONCAT_HEADS: bool = False
 
 # We need to supply the range of possible target values and a reference target value a priori to the
 # network for the regression case. The regression limits should be as complete as possible. The reference
 # does not have to be in the middle, changing it will influence the development of the explanations quite
 # a bit.
-REGRESSION_REFERENCE = 0
+REGRESSION_REFERENCE = [0]
 REGRESSION_LIMITS = [[-3, 3]]
+REGRESSION_WEIGHTS = [[1, 1]]
 
 CHANNEL_DIRECTIONS = {
     0: -1,
     1: +1,
 }
 
 # At the tail end of the network there is a MLP, which does the final prediction. This list defines the
@@ -81,15 +82,15 @@
 FINAL_UNITS = [60, 20, 1]
 
 # This dropout is applied after EVERY layer in the final MLP. Using this should not be necessary
 FINAL_DROPOUT = 0.0
 
 # == TRAINING PARAMETERS ==
 EPOCHS = 250
-OPTIMIZER_CB = lambda: ks.optimizers.Nadam(learning_rate=0.01)
+OPTIMIZER_CB = lambda: ks.optimizers.Nadam(learning_rate=0.001)
 
 
 # == EVALUATION PARAMETERS ==
 IMPORTANCE_CHANNEL_LABELS = ['negative', 'positive']
 
 
 # == EXPERIMENT PARAMETERS ==
@@ -109,14 +110,15 @@
             dropout_rate=e.parameters['DROPOUT_RATE'],
             importance_factor=e.parameters['IMPORTANCE_FACTOR'],
             importance_multiplier=e.parameters['IMPORTANCE_MULTIPLIER'],
             importance_channels=e.parameters['IMPORTANCE_CHANNELS'],
             sparsity_factor=e.parameters['SPARSITY_FACTOR'],
             regression_reference=e.parameters['REGRESSION_REFERENCE'],
             regression_limits=e.parameters['REGRESSION_LIMITS'],
+            regression_weights=e.parameters['REGRESSION_WEIGHTS'],
             final_units=e.parameters['FINAL_UNITS'],
             final_dropout_rate=e.parameters['FINAL_DROPOUT'],
             use_graph_attributes=False,
             use_edge_features=True,
             concat_heads=e.parameters['CONCAT_HEADS']
         )
         model.compile(
```

### Comparing `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py` & `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 import pathlib
 import typing as t
 
 from pycomex.util import Skippable
 from pycomex.experiment import SubExperiment
 
 # == DATASET PARAMETERS ==
-VISUAL_GRAPH_DATASET_PATH: str = os.path.expanduser('~/.visual_graph_datasets/datasets/aqsoldb')
+VISUAL_GRAPH_DATASET_PATH: str = os.path.expanduser('/media/ssd/.visual_graph_datasets/datasets/aqsoldb')
 USE_DATASET_SPLIT: t.Optional[int] = 0
 TRAIN_RATIO: float = 0.8
 NUM_EXAMPLES: int = 100
 
 NODE_IMPORTANCES_KEY: t.Optional[str] = None
 EDGE_IMPORTANCES_KEY: t.Optional[str] = None
 
 USE_NODE_COORDINATES: bool = False
 USE_EDGE_ATTRIBUTES: bool = True
 USE_EDGE_LENGTHS: bool = False
 
 # == MODEL PARAMETERS ==
-UNITS = [32, 32, 32]
+UNITS = [64, 64, 64]
+DROPOUT_RATE = 0.3
 FINAL_UNITS = [64, 32, 1]
-REGRESSION_REFERENCE = -3
-REGRESSION_LIMITS = [[-12, 3]]
+REGRESSION_LIMITS = None
+REGRESSION_REFERENCE = [-1.0]
+REGRESSION_WEIGHTS = [[1.0, 1.0]]
+IMPORTANCE_CHANNELS: int = 2
+IMPORTANCE_FACTOR = 1.0
+IMPORTANCE_MULTIPLIER = 1.0
+SPARSITY_FACTOR = 3.0
+CONCAT_HEADS = False
 
 # == TRAINING PARAMETERS ==
 BATCH_SIZE = 32
 EPOCHS = 50
 REPETITIONS = 1
 
 # == EXPERIMENT PARAMETERS ==
```

### Comparing `graph_attention_student-0.7.1/graph_attention_student/keras.py` & `graph_attention_student-0.7.2/graph_attention_student/keras.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/layers.py` & `graph_attention_student-0.7.2/graph_attention_student/layers.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/megan.cpython-310.pyc` & `graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/megan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 28 11:59:52 2023 UTC, .py size: 28462 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b8d6 2264 2e6f 0000  o........."d.o..
+00000000: 6f0d 0d0a 0000 0000 aa65 4a64 7073 0000  o........eJdps..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 6d05 5a06 0100 6400 6402 6c07  d.l.m.Z...d.d.l.
 00000050: 6d08 5a08 0100 6400 6403 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0b 6d0d 5a0d 6d0e 5a0e 0100 6400  d.l.m.Z.m.Z...d.
@@ -31,908 +31,940 @@
 000001e0: 6757 6569 6768 7465 644e 6f64 6573 2901  gWeightedNodes).
 000001f0: da21 4578 706c 616e 6174 696f 6e53 7061  .!ExplanationSpa
 00000200: 7273 6974 7952 6567 756c 6172 697a 6174  rsityRegularizat
 00000210: 696f 6e29 01da 134d 756c 7469 4865 6164  ion)...MultiHead
 00000220: 4741 5456 324c 6179 6572 2901 da03 6d61  GATV2Layer)...ma
 00000230: 6529 01da 0362 6365 2901 da0f 7368 6966  e)...bce)...shif
 00000240: 7465 645f 7369 676d 6f69 6463 0000 0000  ted_sigmoidc....
-00000250: 0000 0000 0000 0000 0000 0000 3100 0000  ............1...
-00000260: 0000 0000 7364 0100 0065 005a 0164 005a  ....sd...e.Z.d.Z
+00000250: 0000 0000 0000 0000 0000 0000 3300 0000  ............3...
+00000260: 0000 0000 7388 0100 0065 005a 0164 005a  ....s....e.Z.d.Z
 00000270: 0264 015a 0364 0264 0364 0464 0367 0064  .d.Z.d.d.d.d.g.d
 00000280: 0564 0664 0464 0464 0764 0864 0464 0364  .d.d.d.d.d.d.d.d
 00000290: 0964 0a67 0164 0464 0b64 0c64 0864 0864  .d.g.d.d.d.d.d.d
-000002a0: 0864 0364 0966 1764 0d65 046a 0565 0619  .d.d.f.d.e.j.e..
-000002b0: 0064 0e65 0764 0f65 0864 1065 0964 1165  .d.e.d.e.d.e.d.e
-000002c0: 0864 1265 046a 0565 0619 0064 1365 0664  .d.e.j.e...d.e.d
-000002d0: 1465 0764 1565 0964 1665 0964 1765 0964  .e.d.e.d.e.d.e.d
-000002e0: 1865 046a 0a65 046a 0565 0b6a 0c6a 0d19  .e.j.e.j.e.j.j..
-000002f0: 0019 0064 1965 0964 1a65 0864 1b65 0864  ...d.e.d.e.d.e.d
-00000300: 1c65 046a 0565 0619 0064 1d65 0964 1e65  .e.j.e...d.e.d.e
-00000310: 0764 1f65 0764 2065 046a 0a65 046a 0e65  .d.e.d e.j.e.j.e
-00000320: 0965 0966 0219 0019 0064 2165 046a 0a65  .e.f.....d!e.j.e
-00000330: 046a 0565 046a 0e65 0965 0966 0219 0019  .j.e.j.e.e.f....
-00000340: 0019 0064 2265 046a 0a65 0919 0064 2365  ...d"e.j.e...d#e
-00000350: 0864 2465 0866 3064 2564 2684 055a 0f87  .d$e.f0d%d&..Z..
-00000360: 0066 0164 2764 2884 085a 1065 1164 2965  .f.d'd(..Z.e.d)e
-00000370: 0866 0264 2a64 2b84 0483 015a 1209 0909  .f.d*d+....Z....
-00000380: 0909 0864 3764 2c65 0864 2365 0864 2d65  ...d7d,e.d#e.d-e
-00000390: 046a 0a65 136a 1419 0066 0664 2e64 2f84  .j.e.j...f.d.d/.
-000003a0: 055a 1564 3064 3184 005a 1609 0364 3864  .Z.d0d1..Z...d8d
-000003b0: 3265 0866 0264 3364 3484 055a 1764 3564  2e.f.d3d4..Z.d5d
-000003c0: 3684 005a 1887 0004 005a 1953 0029 39da  6..Z.....Z.S.)9.
-000003d0: 054d 6567 616e 613c 0200 000a 2020 2020  .Megana<....    
-000003e0: 4d45 4741 4e3a 204d 756c 7469 2045 7870  MEGAN: Multi Exp
-000003f0: 6c61 6e61 7469 6f6e 2047 7261 7068 2041  lanation Graph A
-00000400: 7474 656e 7469 6f6e 204e 6574 776f 726b  ttention Network
-00000410: 0a20 2020 2054 6869 7320 6d6f 6465 6c20  .    This model 
-00000420: 6375 7272 656e 746c 7920 7375 7070 6f72  currently suppor
-00000430: 7473 2067 7261 7068 2072 6567 7265 7373  ts graph regress
-00000440: 696f 6e20 616e 6420 6772 6170 6820 636c  ion and graph cl
-00000450: 6173 7369 6669 6361 7469 6f6e 2070 726f  assification pro
-00000460: 626c 656d 732e 2049 7420 7761 7320 6d61  blems. It was ma
-00000470: 696e 6c79 2064 6573 6967 6e65 640a 2020  inly designed.  
-00000480: 2020 7769 7468 2061 2066 6f63 7573 206f    with a focus o
-00000490: 6e20 6578 706c 6169 6e61 626c 6520 4149  n explainable AI
-000004a0: 2028 5841 4929 2e20 416c 6f6e 6720 7468   (XAI). Along th
-000004b0: 6520 6d61 696e 2070 7265 6469 6374 696f  e main predictio
-000004c0: 6e2c 2074 6869 7320 6d6f 6465 6c20 6973  n, this model is
-000004d0: 2061 626c 6520 746f 206f 7574 7075 7420   able to output 
-000004e0: 6d75 6c74 6970 6c65 0a20 2020 2061 7474  multiple.    att
-000004f0: 656e 7469 6f6e 2d62 6173 6564 2065 7870  ention-based exp
-00000500: 6c61 6e61 7469 6f6e 7320 666f 7220 7468  lanations for th
-00000510: 6174 2070 7265 6469 6374 696f 6e2e 204d  at prediction. M
-00000520: 6f72 6520 7370 6563 6966 6963 616c 6c79  ore specifically
-00000530: 2c20 7468 6520 6d6f 6465 6c20 6f75 7470  , the model outp
-00000540: 7574 7320 6e6f 6465 2061 6e64 2065 6467  uts node and edg
-00000550: 650a 2020 2020 6174 7472 6962 7574 696f  e.    attributio
-00000560: 6e61 6c20 6578 706c 616e 6174 696f 6e73  nal explanations
-00000570: 2028 6173 7369 676e 696e 6720 5b30 2c20   (assigning [0, 
-00000580: 315d 2076 616c 7565 7320 746f 2065 7665  1] values to eve
-00000590: 7220 6e6f 6465 202f 2065 6467 6520 6f66  r node / edge of
-000005a0: 2074 6865 2069 6e70 7574 2067 7261 7068   the input graph
-000005b0: 2920 696e 204b 0a20 2020 2073 6570 6172  ) in K.    separ
-000005c0: 6174 6520 6578 706c 616e 6174 696f 6e20  ate explanation 
-000005d0: 6368 616e 6e65 6c73 2c20 7768 6572 6520  channels, where 
-000005e0: 4b20 6361 6e20 6265 2063 686f 7365 6e20  K can be chosen 
-000005f0: 6173 2061 6e20 696e 6465 7065 6e64 656e  as an independen
-00000600: 7420 6d6f 6465 6c20 7061 7261 6d65 7465  t model paramete
-00000610: 722e 0a20 2020 20fa 106b 6763 6e6e 3e6c  r..    ..kgcnn>l
-00000620: 6561 6b79 5f72 656c 7554 e700 0000 0000  eaky_reluT......
-00000630: 0000 00e9 0200 0000 da07 7369 676d 6f69  ..........sigmoi
-00000640: 6467 0000 0000 0000 2440 4e46 e901 0000  dg......$@NF....
-00000650: 00da 066c 696e 6561 72da 0373 756d da05  ...linear..sum..
-00000660: 756e 6974 73da 0a61 6374 6976 6174 696f  units..activatio
-00000670: 6eda 0875 7365 5f62 6961 73da 0c64 726f  n..use_bias..dro
-00000680: 706f 7574 5f72 6174 65da 1175 7365 5f65  pout_rate..use_e
-00000690: 6467 655f 6665 6174 7572 6573 da10 696d  dge_features..im
-000006a0: 706f 7274 616e 6365 5f75 6e69 7473 da13  portance_units..
-000006b0: 696d 706f 7274 616e 6365 5f63 6861 6e6e  importance_chann
-000006c0: 656c 73da 1569 6d70 6f72 7461 6e63 655f  els..importance_
-000006d0: 6163 7469 7661 7469 6f6e da17 696d 706f  activation..impo
-000006e0: 7274 616e 6365 5f64 726f 706f 7574 5f72  rtance_dropout_r
-000006f0: 6174 65da 1169 6d70 6f72 7461 6e63 655f  ate..importance_
-00000700: 6661 6374 6f72 da15 696d 706f 7274 616e  factor..importan
-00000710: 6365 5f6d 756c 7469 706c 6965 72da 1a69  ce_multiplier..i
-00000720: 6d70 6f72 7461 6e63 655f 7472 616e 7366  mportance_transf
-00000730: 6f72 6d61 7469 6f6e 73da 0f73 7061 7273  ormations..spars
-00000740: 6974 795f 6661 6374 6f72 da0c 636f 6e63  ity_factor..conc
-00000750: 6174 5f68 6561 6473 da19 7365 7061 7261  at_heads..separa
-00000760: 7465 5f65 7870 6c61 6e61 7469 6f6e 5f73  te_explanation_s
-00000770: 7465 70da 0b66 696e 616c 5f75 6e69 7473  tep..final_units
-00000780: da12 6669 6e61 6c5f 6472 6f70 6f75 745f  ..final_dropout_
-00000790: 7261 7465 da10 6669 6e61 6c5f 6163 7469  rate..final_acti
-000007a0: 7661 7469 6f6e da0d 6669 6e61 6c5f 706f  vation..final_po
-000007b0: 6f6c 696e 67da 1172 6567 7265 7373 696f  oling..regressio
-000007c0: 6e5f 6c69 6d69 7473 da0f 7265 6772 6573  n_limits..regres
-000007d0: 7369 6f6e 5f62 696e 73da 1472 6567 7265  sion_bins..regre
-000007e0: 7373 696f 6e5f 7265 6665 7265 6e63 65da  ssion_reference.
-000007f0: 1272 6574 7572 6e5f 696d 706f 7274 616e  .return_importan
-00000800: 6365 73da 1475 7365 5f67 7261 7068 5f61  ces..use_graph_a
-00000810: 7474 7269 6275 7465 7363 1900 0000 0000  ttributesc......
-00000820: 0000 0000 0000 2000 0000 0a00 0000 4b00  ...... .......K.
-00000830: 0000 7336 0300 0074 006a 016a 026a 037c  ..s6...t.j.j.j.|
-00000840: 0066 0169 007c 19a4 018e 0101 007c 017c  .f.i.|.......|.|
-00000850: 005f 047c 027c 005f 057c 037c 005f 067c  ._.|.|._.|.|._.|
-00000860: 047c 005f 077c 057c 005f 087c 067c 005f  .|._.|.|._.|.|._
-00000870: 097c 077c 005f 0a7c 087c 005f 0b7c 097c  .|.|._.|.|._.|.|
-00000880: 005f 0c7c 0a7c 005f 0d7c 0b7c 005f 0e7c  ._.|.|._.|.|._.|
-00000890: 0c7c 005f 0f7c 0d7c 005f 107c 0e7c 005f  .|._.|.|._.|.|._
-000008a0: 117c 107c 005f 127c 117c 005f 137c 127c  .|.|._.|.|._.|.|
-000008b0: 005f 147c 137c 005f 157c 147c 005f 167c  ._.|.|._.|.|._.|
-000008c0: 167c 005f 177c 157c 005f 187c 177c 005f  .|._.|.|._.|.|._
-000008d0: 197c 0f7c 005f 1a7c 187c 005f 1b67 007c  .|.|._.|.|._.g.|
-000008e0: 005f 1c7c 006a 0444 005d 187d 1a74 1d7c  ._.|.j.D.].}.t.|
-000008f0: 1a7c 006a 0a7c 006a 087c 006a 057c 006a  .|.j.|.j.|.j.|.j
-00000900: 0664 017c 006a 1164 028d 077d 1b7c 006a  .d.|.j.d...}.|.j
-00000910: 1ca0 1e7c 1ba1 0101 0071 5974 1f7c 006a  ...|.....qYt.|.j
-00000920: 0764 038d 017c 005f 2074 217c 006a 1064  .d...|._ t!|.j.d
-00000930: 048d 017c 005f 2274 237c 006a 0b64 058d  ...|._"t#|.j.d..
-00000940: 017c 005f 2474 2564 0664 078d 017c 005f  .|._$t%d.d...|._
-00000950: 2674 2764 0864 0964 0a8d 027c 005f 2874  &t'd.d.d...|._(t
-00000960: 2764 0864 0b64 0a8d 027c 005f 2974 2a83  'd.d.d...|._)t*.
-00000970: 007c 005f 2b7c 067c 006a 0a67 0117 007c  .|._+|.|.j.g...|
-00000980: 005f 2c64 0c64 0d84 007c 0644 0083 0164  ._,d.d...|.D...d
-00000990: 0e67 0117 007c 005f 2d67 007c 005f 2e74  .g...|._-g.|._.t
-000009a0: 2f7c 006a 2c7c 006a 2d83 0244 005d 115c  /|.j,|.j-..D.].\
-000009b0: 027d 1a7d 1c74 307c 1a7c 1c7c 0364 0f8d  .}.}.t0|.|.|.d..
-000009c0: 037d 1b7c 006a 2ea0 1e7c 1ba1 0101 0071  .}.|.j...|.....q
-000009d0: bb74 317c 006a 1564 108d 017c 005f 3274  .t1|.j.d...|._2t
-000009e0: 2564 0664 078d 017c 005f 3374 1f7c 006a  %d.d...|._3t.|.j
-000009f0: 1364 038d 017c 005f 3464 1164 0d84 007c  .d...|._4d.d...|
-00000a00: 006a 1244 0083 017c 005f 357c 006a 147c  .j.D...|._5|.j.|
-00000a10: 006a 3564 063c 0064 1264 0d84 007c 006a  .j5d.<.d.d...|.j
-00000a20: 1244 0083 017c 005f 3664 017c 006a 3664  .D...|._6d.|.j6d
-00000a30: 063c 0067 007c 005f 3774 2f7c 006a 127c  .<.g.|._7t/|.j.|
-00000a40: 006a 357c 006a 3683 0344 005d 135c 037d  .j5|.j6..D.].\.}
-00000a50: 1a7d 1c7d 1d74 307c 1a7c 1c7c 0364 0f8d  .}.}.t0|.|.|.d..
-00000a60: 037d 1b7c 006a 37a0 1e7c 1ba1 0101 0090  .}.|.j7..|......
-00000a70: 0171 0a74 006a 38a0 39a1 007c 005f 3a74  .q.t.j8.9..|._:t
-00000a80: 3ba0 3c74 3da1 017c 005f 3e74 006a 38a0  ;.<t=..|._>t.j8.
-00000a90: 3fa1 007c 005f 4074 006a 38a0 41a1 007c  ?..|._@t.j8.A..|
-00000aa0: 005f 4274 3ba0 3c74 43a1 017c 005f 447c  ._Bt;.<tC..|._D|
-00000ab0: 006a 1664 1375 0190 0172 977c 1664 1375  .j.d.u...r.|.d.u
-00000ac0: 0190 0173 4b4a 0064 1483 0182 0174 457c  ...sKJ.d.....tE|
-00000ad0: 1674 4674 4766 0283 0290 0172 577c 1667  .tFtGf.....rW|.g
-00000ae0: 017c 005f 1774 487c 006a 1783 017d 1e74  .|._.tH|.j...}.t
-00000af0: 487c 006a 1683 017d 1f7c 1e64 1514 007c  H|.j...}.|.d...|
-00000b00: 076b 0290 0173 734a 0064 167c 1e9b 0064  .k...ssJ.d.|...d
-00000b10: 177c 079b 0064 189d 0583 0182 017c 1e7c  .|...d.......|.|
-00000b20: 1064 0619 006b 0290 0173 874a 0064 197c  .d...k...s.J.d.|
-00000b30: 1e9b 0064 1a7c 1064 0619 009b 0064 1b9d  ...d.|.d.....d..
-00000b40: 0583 0182 017c 1e7c 1f6b 0290 0173 994a  .....|.|.k...s.J
-00000b50: 0064 197c 1e9b 0064 1c7c 1f9b 0064 1b9d  .d.|...d.|...d..
-00000b60: 0583 0182 0164 1353 0064 1353 0029 1d61  .....d.S.d.S.).a
-00000b70: 250f 0000 0a20 2020 2020 2020 2041 7267  %....        Arg
-00000b80: 733a 0a20 2020 2020 2020 2020 2020 2075  s:.            u
-00000b90: 6e69 7473 3a20 4120 6c69 7374 206f 6620  nits: A list of 
-00000ba0: 696e 7473 2077 6865 7265 2065 6163 6820  ints where each 
-00000bb0: 656c 656d 656e 7420 636f 6e66 6967 7572  element configur
-00000bc0: 6573 2061 6e20 6164 6469 7469 6f6e 616c  es an additional
-00000bd0: 2061 7474 656e 7469 6f6e 206c 6179 6572   attention layer
-00000be0: 2e20 5468 6520 6e75 6d65 7269 630a 2020  . The numeric.  
-00000bf0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00000c00: 6c75 6520 6465 7465 726d 696e 6573 2074  lue determines t
-00000c10: 6865 206e 756d 6265 7220 6f66 2068 6964  he number of hid
-00000c20: 6465 6e20 756e 6974 7320 746f 2062 6520  den units to be 
-00000c30: 7573 6564 2069 6e20 7468 6520 6174 7465  used in the atte
-00000c40: 6e74 696f 6e20 6865 6164 7320 6f66 2074  ntion heads of t
-00000c50: 6861 7420 6c61 7965 720a 2020 2020 2020  hat layer.      
-00000c60: 2020 2020 2020 6163 7469 7661 7469 6f6e        activation
-00000c70: 3a20 5468 6520 6163 7469 7661 7469 6f6e  : The activation
-00000c80: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-00000c90: 7573 6564 2077 6974 6869 6e20 7468 6520  used within the 
-00000ca0: 6174 7465 6e74 696f 6e20 6c61 7965 7273  attention layers
-00000cb0: 206f 6620 7468 6520 6e65 7477 6f72 6b0a   of the network.
-00000cc0: 2020 2020 2020 2020 2020 2020 7573 655f              use_
-00000cd0: 6269 6173 3a20 5768 6574 6865 7220 7468  bias: Whether th
-00000ce0: 6520 6c61 7965 7273 206f 6620 7468 6520  e layers of the 
-00000cf0: 6e65 7477 6f72 6b20 7368 6f75 6c64 2075  network should u
-00000d00: 7365 2062 6961 7320 7765 6967 6874 7320  se bias weights 
-00000d10: 6174 2061 6c6c 0a20 2020 2020 2020 2020  at all.         
-00000d20: 2020 2064 726f 706f 7574 5f72 6174 653a     dropout_rate:
-00000d30: 2054 6865 2064 726f 706f 7574 2072 6174   The dropout rat
-00000d40: 6520 746f 2062 6520 6170 706c 6965 6420  e to be applied 
-00000d50: 6166 7465 7220 2a65 6163 682a 206f 6620  after *each* of 
-00000d60: 7468 6520 6174 7465 6e74 696f 6e20 6c61  the attention la
-00000d70: 7965 7273 206f 6620 7468 6520 6e65 7477  yers of the netw
-00000d80: 6f72 6b2e 0a20 2020 2020 2020 2020 2020  ork..           
-00000d90: 2075 7365 5f65 6467 655f 6665 6174 7572   use_edge_featur
-00000da0: 6573 3a20 5768 6574 6865 7220 6564 6765  es: Whether edge
-00000db0: 2066 6561 7475 7265 7320 7368 6f75 6c64   features should
-00000dc0: 2062 6520 7573 6564 2e20 4765 6e65 7261   be used. Genera
-00000dd0: 6c6c 7920 7468 6520 6e65 7477 6f72 6b20  lly the network 
-00000de0: 7375 7070 6f72 7473 2074 6865 0a20 2020  supports the.   
-00000df0: 2020 2020 2020 2020 2020 2020 2075 7361               usa
-00000e00: 6765 206f 6620 6564 6765 2066 6561 7475  ge of edge featu
-00000e10: 7265 732c 2062 7574 2069 6620 7468 6520  res, but if the 
-00000e20: 696e 7075 7420 6461 7461 2064 6f65 7320  input data does 
-00000e30: 6e6f 7420 636f 6e74 6169 6e20 6564 6765  not contain edge
-00000e40: 2066 6561 7475 7265 732c 2074 6869 7320   features, this 
-00000e50: 7368 6f75 6c64 2062 650a 2020 2020 2020  should be.      
-00000e60: 2020 2020 2020 2020 2020 7365 7420 746f            set to
-00000e70: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-00000e80: 2020 2020 696d 706f 7274 616e 6365 5f75      importance_u
-00000e90: 6e69 7473 3a20 4120 6c69 7374 206f 6620  nits: A list of 
-00000ea0: 696e 7473 2077 6865 7265 2065 6163 6820  ints where each 
-00000eb0: 656c 656d 656e 7420 636f 6e66 6967 7572  element configur
-00000ec0: 6573 2061 6e6f 7468 6572 2064 656e 7365  es another dense
-00000ed0: 206c 6179 6572 2069 6e20 7468 650a 2020   layer in the.  
-00000ee0: 2020 2020 2020 2020 2020 2020 2020 7375                su
-00000ef0: 626e 6574 776f 726b 2074 6861 7420 7072  bnetwork that pr
-00000f00: 6f64 7563 6573 2074 6865 206e 6f64 6520  oduces the node 
-00000f10: 696d 706f 7274 616e 6365 2074 656e 736f  importance tenso
-00000f20: 7220 6672 6f6d 2074 6865 206d 6169 6e20  r from the main 
-00000f30: 6e6f 6465 2065 6d62 6564 6469 6e67 732e  node embeddings.
-00000f40: 2054 6865 0a20 2020 2020 2020 2020 2020   The.           
-00000f50: 2020 2020 206e 756d 6572 6963 2076 616c       numeric val
-00000f60: 7565 2064 6574 6572 6d69 6e65 7320 7468  ue determines th
-00000f70: 6520 6e75 6d62 6572 206f 6620 6869 6464  e number of hidd
-00000f80: 656e 2075 6e69 7473 2069 6e20 7468 6174  en units in that
-00000f90: 206c 6179 6572 2e0a 2020 2020 2020 2020   layer..        
-00000fa0: 2020 2020 696d 706f 7274 616e 6365 5f63      importance_c
-00000fb0: 6861 6e6e 656c 733a 2054 6865 2069 6e74  hannels: The int
-00000fc0: 206e 756d 6265 7220 6f66 2065 7870 6c61   number of expla
-00000fd0: 6e61 7469 6f6e 2063 6861 6e6e 656c 7320  nation channels 
-00000fe0: 746f 2062 6520 7072 6f64 7563 6564 2062  to be produced b
-00000ff0: 7920 7468 6520 6e65 7477 6f72 6b2e 2054  y the network. T
-00001000: 6869 730a 2020 2020 2020 2020 2020 2020  his.            
-00001010: 2020 2020 6973 2074 6865 2076 616c 7565      is the value
-00001020: 2072 6566 6572 7265 6420 746f 2061 7320   referred to as 
-00001030: 224b 222e 204e 6f74 6520 7468 6174 2074  "K". Note that t
-00001040: 6869 7320 7769 6c6c 2061 6c73 6f20 6465  his will also de
-00001050: 7465 726d 696e 6520 7468 6520 6e75 6d62  termine the numb
-00001060: 6572 206f 6620 6174 7465 6e74 696f 6e0a  er of attention.
-00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001080: 6865 6164 7320 7573 6564 2077 6974 6869  heads used withi
-00001090: 6e20 7468 6520 6174 7465 6e74 696f 6e20  n the attention 
-000010a0: 7375 626e 6574 776f 726b 2e0a 2020 2020  subnetwork..    
-000010b0: 2020 2020 2020 2020 696d 706f 7274 616e          importan
-000010c0: 6365 5f66 6163 746f 723a 2054 6865 2077  ce_factor: The w
-000010d0: 6569 6768 7420 6f66 2074 6865 2065 7870  eight of the exp
-000010e0: 6c61 6e61 7469 6f6e 2d6f 6e6c 7920 7472  lanation-only tr
-000010f0: 6169 6e20 7374 6570 2e20 4966 2074 6869  ain step. If thi
-00001100: 7320 6973 2073 6574 2074 6f20 6578 6163  s is set to exac
-00001110: 746c 790a 2020 2020 2020 2020 2020 2020  tly.            
-00001120: 2020 2020 7a65 726f 2074 6865 6e20 7468      zero then th
-00001130: 6520 6578 706c 616e 6174 696f 6e20 7472  e explanation tr
-00001140: 6169 6e20 7374 6570 2077 696c 6c20 6e6f  ain step will no
-00001150: 7420 6265 2065 7865 6375 7465 6420 6174  t be executed at
-00001160: 2061 6c6c 2028 6c65 7373 2063 6f6d 7075   all (less compu
-00001170: 7461 7469 6f6e 616c 6c79 0a20 2020 2020  tationally.     
-00001180: 2020 2020 2020 2020 2020 2065 7870 656e             expen
-00001190: 7369 7665 290a 2020 2020 2020 2020 2020  sive).          
-000011a0: 2020 696d 706f 7274 616e 6365 5f6d 756c    importance_mul
-000011b0: 7469 706c 6965 723a 2041 6e20 6164 6469  tiplier: An addi
-000011c0: 7469 6f6e 616c 2068 7970 6572 7061 7261  tional hyperpara
-000011d0: 6d65 7465 7220 6f66 2074 6865 2065 7870  meter of the exp
-000011e0: 6c61 6e61 7469 6f6e 2d6f 6e6c 7920 7472  lanation-only tr
-000011f0: 6169 6e20 7374 6570 2e20 5468 6973 0a20  ain step. This. 
-00001200: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001210: 7320 6573 7365 6e74 6961 6c6c 7920 7468  s essentially th
-00001220: 6520 7363 616c 696e 6720 6661 6374 6f72  e scaling factor
-00001230: 2074 6861 7420 6973 2061 7070 6c69 6564   that is applied
-00001240: 2074 6f20 7468 6520 7661 6c75 6573 206f   to the values o
-00001250: 6620 7468 6520 6461 7461 7365 7420 7375  f the dataset su
-00001260: 6368 2074 6861 740a 2020 2020 2020 2020  ch that.        
-00001270: 2020 2020 2020 2020 7468 6520 7461 7267          the targ
-00001280: 6574 2076 616c 7565 7320 6361 6e20 7265  et values can re
-00001290: 6173 6f6e 6162 6c79 2062 6520 6170 7072  asonably be appr
-000012a0: 6f78 696d 6174 6564 2062 7920 6120 7375  oximated by a su
-000012b0: 6d20 6f66 205b 302c 2031 5d20 696d 706f  m of [0, 1] impo
-000012c0: 7274 616e 6365 2076 616c 7565 732e 0a20  rtance values.. 
-000012d0: 2020 2020 2020 2020 2020 2073 7061 7273             spars
-000012e0: 6974 795f 6661 6374 6f72 3a20 5468 6520  ity_factor: The 
-000012f0: 636f 6566 6669 6369 656e 7420 666f 7220  coefficient for 
-00001300: 7468 6520 7370 6172 7369 7479 2072 6567  the sparsity reg
-00001310: 756c 6172 697a 6174 696f 6e20 6f66 2074  ularization of t
-00001320: 6865 206e 6f64 6520 696d 706f 7274 616e  he node importan
-00001330: 6365 0a20 2020 2020 2020 2020 2020 2020  ce.             
-00001340: 2020 2074 656e 736f 722e 0a20 2020 2020     tensor..     
-00001350: 2020 2020 2020 2063 6f6e 6361 745f 6865         concat_he
-00001360: 6164 733a 2057 6865 7468 6572 2074 6f20  ads: Whether to 
-00001370: 636f 6e63 6174 2074 6865 2068 6561 6473  concat the heads
-00001380: 206f 6620 7468 6520 6174 7465 6e74 696f   of the attentio
-00001390: 6e20 7375 626e 6574 776f 726b 2e20 5468  n subnetwork. Th
-000013a0: 6520 6465 6661 756c 7420 6973 2054 7275  e default is Tru
-000013b0: 652e 2049 6e0a 2020 2020 2020 2020 2020  e. In.          
-000013c0: 2020 2020 2020 7468 6174 2063 6173 6520        that case 
-000013d0: 7468 6520 6f75 7470 7574 206f 6620 6561  the output of ea
-000013e0: 6368 2069 6e64 6976 6964 7561 6c20 6174  ch individual at
-000013f0: 7465 6e74 696f 6e20 6865 6164 2069 7320  tention head is 
-00001400: 636f 6e63 6174 656e 6174 6564 2061 6e64  concatenated and
-00001410: 2074 6865 2063 6f6e 6361 7465 6e61 7465   the concatenate
-00001420: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00001430: 2020 7665 6374 6f72 2069 7320 7468 656e    vector is then
-00001440: 2075 7365 6420 6173 2074 6865 2069 6e70   used as the inp
-00001450: 7574 206f 6620 7468 6520 6e65 7874 2061  ut of the next a
-00001460: 7474 656e 7469 6f6e 206c 6179 6572 2773  ttention layer's
-00001470: 2068 6561 6473 2e20 4966 2074 6869 7320   heads. If this 
-00001480: 6973 2046 616c 7365 2c20 7468 650a 2020  is False, the.  
-00001490: 2020 2020 2020 2020 2020 2020 2020 7665                ve
-000014a0: 6374 6f72 7320 6172 6520 6176 6572 6167  ctors are averag
-000014b0: 6520 706f 6f6c 6564 2069 6e73 7465 6164  e pooled instead
-000014c0: 2e0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
-000014d0: 6e61 6c5f 756e 6974 733a 2041 206c 6973  nal_units: A lis
-000014e0: 7420 6f66 2069 6e74 7320 7768 6572 6520  t of ints where 
-000014f0: 6561 6368 2065 6c65 6d65 6e74 2063 6f6e  each element con
-00001500: 6669 6775 7265 7320 616e 6f74 6865 7220  figures another 
-00001510: 6465 6e73 6520 6c61 7965 7220 696e 2074  dense layer in t
-00001520: 6865 204d 4c50 0a20 2020 2020 2020 2020  he MLP.         
-00001530: 2020 2020 2020 2061 7420 7468 6520 7461         at the ta
-00001540: 696c 2065 6e64 206f 6620 7468 6520 6e65  il end of the ne
-00001550: 7477 6f72 6b2e 2054 6865 206e 756d 6572  twork. The numer
-00001560: 6963 2076 616c 7565 2064 6574 6572 6d69  ic value determi
-00001570: 6e65 7320 7468 6520 6e75 6d62 6572 206f  nes the number o
-00001580: 6620 7468 6520 6869 6464 656e 2075 6e69  f the hidden uni
-00001590: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
-000015a0: 2020 2069 6e20 7468 6174 206c 6179 6572     in that layer
-000015b0: 2e20 4e6f 7465 2074 6861 7420 7468 6520  . Note that the 
-000015c0: 6669 6e61 6c20 656c 656d 656e 7420 696e  final element in
-000015d0: 2074 6869 7320 6c69 7374 2068 6173 2074   this list has t
-000015e0: 6f20 6265 2074 6865 2073 616d 6520 6173  o be the same as
-000015f0: 2074 6865 2064 696d 656e 7369 6f6e 0a20   the dimension. 
-00001600: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001610: 6f20 6265 2065 7870 6563 7465 6420 666f  o be expected fo
-00001620: 7220 7468 6520 7361 6d70 6c65 7320 6f66  r the samples of
-00001630: 2074 6865 2074 7261 696e 696e 6720 6461   the training da
-00001640: 7461 7365 7421 0a20 2020 2020 2020 2020  taset!.         
-00001650: 2020 2066 696e 616c 5f64 726f 706f 7574     final_dropout
-00001660: 5f72 6174 653a 2054 6865 2064 726f 706f  _rate: The dropo
-00001670: 7574 2072 6174 6520 746f 2062 6520 6170  ut rate to be ap
-00001680: 706c 6965 6420 6166 7465 7220 2a65 7665  plied after *eve
-00001690: 7279 2a20 6c61 7965 7220 6f66 2074 6865  ry* layer of the
-000016a0: 2066 696e 616c 204d 4c50 2e0a 2020 2020   final MLP..    
-000016b0: 2020 2020 2020 2020 6669 6e61 6c5f 6163          final_ac
-000016c0: 7469 7661 7469 6f6e 3a20 5468 6520 6163  tivation: The ac
-000016d0: 7469 7661 7469 6f6e 2074 6f20 6265 2061  tivation to be a
-000016e0: 7070 6c69 6564 2061 7420 7468 6520 7665  pplied at the ve
-000016f0: 7279 206c 6173 7420 6c61 7965 7220 6f66  ry last layer of
-00001700: 2074 6865 204d 4c50 2074 6f20 7072 6f64   the MLP to prod
-00001710: 7563 6520 7468 650a 2020 2020 2020 2020  uce the.        
-00001720: 2020 2020 2020 2020 6163 7475 616c 206f          actual o
-00001730: 7574 7075 7420 6f66 2074 6865 206e 6574  utput of the net
-00001740: 776f 726b 2e0a 2020 2020 2020 2020 2020  work..          
-00001750: 2020 6669 6e61 6c5f 706f 6f6c 696e 673a    final_pooling:
-00001760: 2054 6865 2070 6f6f 6c69 6e67 206d 6574   The pooling met
-00001770: 686f 6420 746f 2062 6520 7573 6564 2064  hod to be used d
-00001780: 7572 696e 6720 7468 6520 676c 6f62 616c  uring the global
-00001790: 2070 6f6f 6c69 6e67 2070 6861 7365 2069   pooling phase i
-000017a0: 6e20 7468 6520 6e65 7477 6f72 6b2e 0a20  n the network.. 
-000017b0: 2020 2020 2020 2020 2020 2072 6567 7265             regre
-000017c0: 7373 696f 6e5f 6c69 6d69 7473 3a20 4120  ssion_limits: A 
-000017d0: 7475 706c 6520 7768 6572 6520 7468 6520  tuple where the 
-000017e0: 6669 7273 7420 7661 6c75 6520 6973 2074  first value is t
-000017f0: 6865 206c 6f77 6572 206c 696d 6974 2066  he lower limit f
-00001800: 6f72 2074 6865 2065 7870 6563 7465 6420  or the expected 
-00001810: 7661 6c75 6520 7261 6e67 650a 2020 2020  value range.    
-00001820: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
-00001830: 6865 2072 6567 7265 7373 696f 6e20 7461  he regression ta
-00001840: 736b 2061 6e64 2074 6568 2073 6563 6f6e  sk and teh secon
-00001850: 6420 7661 6c75 6520 7468 6520 7570 7065  d value the uppe
-00001860: 7220 6c69 6d69 742e 0a20 2020 2020 2020  r limit..       
-00001870: 2020 2020 2072 6567 7265 7373 696f 6e5f       regression_
-00001880: 7265 6665 7265 6e63 653a 2041 2072 6566  reference: A ref
-00001890: 6572 656e 6365 2076 616c 7565 2077 6869  erence value whi
-000018a0: 6368 2069 7320 696e 7369 6465 2074 6865  ch is inside the
-000018b0: 2072 616e 6765 206f 6620 6578 7065 6374   range of expect
-000018c0: 6564 2076 616c 7565 7320 2862 6573 7420  ed values (best 
-000018d0: 6966 0a20 2020 2020 2020 2020 2020 2020  if.             
-000018e0: 2020 2069 7420 7761 7320 696e 2074 6865     it was in the
-000018f0: 206d 6964 646c 652c 2062 7574 2064 6f65   middle, but doe
-00001900: 7320 6e6f 7420 6861 7665 2074 6f29 2e20  s not have to). 
-00001910: 4368 6f6f 7369 6e67 2064 6966 6665 7265  Choosing differe
-00001920: 6e74 2072 6566 6572 656e 6365 7320 7769  nt references wi
-00001930: 6c6c 2072 6573 756c 740a 2020 2020 2020  ll result.      
-00001940: 2020 2020 2020 2020 2020 696e 2064 6966            in dif
-00001950: 6665 7265 6e74 2065 7870 6c61 6e61 7469  ferent explanati
-00001960: 6f6e 732e 0a20 2020 2020 2020 2020 2020  ons..           
-00001970: 2072 6574 7572 6e5f 696d 706f 7274 616e   return_importan
-00001980: 6365 733a 2057 6865 7468 6572 2074 6865  ces: Whether the
-00001990: 2069 6d70 6f72 7461 6e63 6520 2f20 6578   importance / ex
-000019a0: 706c 616e 6174 696f 6e20 7465 6e73 6f72  planation tensor
-000019b0: 7320 7368 6f75 6c64 2062 6520 7265 7475  s should be retu
-000019c0: 726e 6564 2061 7320 616e 206f 7574 7075  rned as an outpu
-000019d0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000019e0: 2020 6f66 2074 6865 206d 6f64 656c 2e20    of the model. 
-000019f0: 4966 2074 6869 7320 6973 2054 7275 652c  If this is True,
-00001a00: 2074 6865 206f 7574 7075 7420 6f66 2074   the output of t
-00001a10: 6865 206d 6f64 656c 2077 696c 6c20 6265  he model will be
-00001a20: 2061 2033 2d74 7570 6c65 3a0a 2020 2020   a 3-tuple:.    
-00001a30: 2020 2020 2020 2020 2020 2020 286f 7574              (out
-00001a40: 7075 742c 206e 6f64 6520 696d 706f 7274  put, node import
-00001a50: 616e 6365 732c 2065 6467 6520 696d 706f  ances, edge impo
-00001a60: 7274 616e 6365 7329 2c20 6f74 6865 7277  rtances), otherw
-00001a70: 6973 6520 6974 2069 7320 6a75 7374 2074  ise it is just t
-00001a80: 6865 206f 7574 7075 7420 6974 7365 6c66  he output itself
-00001a90: 0a20 2020 2020 2020 2054 2907 721a 0000  .        T).r...
-00001aa0: 00da 096e 756d 5f68 6561 6473 721e 0000  ...num_headsr...
-00001ab0: 0072 1b00 0000 721c 0000 00da 0e68 6173  .r....r......has
-00001ac0: 5f73 656c 665f 6c6f 6f70 7372 2700 0000  _self_loopsr'...
-00001ad0: 2901 da04 7261 7465 2901 da06 6661 6374  )...rate)...fact
-00001ae0: 6f72 2901 721b 0000 00e9 ffff ffff a901  or).r...........
-00001af0: da04 6178 6973 da04 6d65 616e 7201 0000  ..axis..meanr...
-00001b00: 0029 02da 0e70 6f6f 6c69 6e67 5f6d 6574  .)...pooling_met
-00001b10: 686f 64da 0d70 6f6f 6c69 6e67 5f69 6e64  hod..pooling_ind
-00001b20: 6578 7217 0000 0063 0100 0000 0000 0000  exr....c........
-00001b30: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
-00001b40: f310 0000 0067 007c 005d 047d 0164 0091  .....g.|.].}.d..
-00001b50: 0271 0253 00a9 0172 1300 0000 a900 a902  .q.S...r........
-00001b60: da02 2e30 da01 5f72 3e00 0000 723e 0000  ...0.._r>...r>..
-00001b70: 00fa 562f 6d65 6469 612f 7373 642f 5072  ..V/media/ssd/Pr
-00001b80: 6f67 7261 6d6d 696e 672f 6772 6170 685f  ogramming/graph_
-00001b90: 6174 7465 6e74 696f 6e5f 7374 7564 656e  attention_studen
-00001ba0: 742f 6772 6170 685f 6174 7465 6e74 696f  t/graph_attentio
-00001bb0: 6e5f 7374 7564 656e 742f 6d6f 6465 6c73  n_student/models
-00001bc0: 2f6d 6567 616e 2e70 79da 0a3c 6c69 7374  /megan.py..<list
-00001bd0: 636f 6d70 3e9d 0000 00f3 0200 0000 1000  comp>...........
-00001be0: 7a22 4d65 6761 6e2e 5f5f 696e 6974 5f5f  z"Megan.__init__
-00001bf0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00001c00: 6f6d 703e 7218 0000 0029 0372 1a00 0000  omp>r....).r....
-00001c10: 721b 0000 0072 1c00 0000 2901 723a 0000  r....r....).r:..
-00001c20: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00001c30: 0000 0300 0000 5300 0000 723c 0000 0072  ......S...r<...r
-00001c40: 3d00 0000 723e 0000 0072 3f00 0000 723e  =...r>...r?...r>
-00001c50: 0000 0072 3e00 0000 7242 0000 0072 4300  ...r>...rB...rC.
-00001c60: 0000 ac00 0000 7244 0000 0063 0100 0000  ......rD...c....
-00001c70: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00001c80: 5300 0000 723c 0000 00a9 0154 723e 0000  S...r<.....Tr>..
-00001c90: 0072 3f00 0000 723e 0000 0072 3e00 0000  .r?...r>...r>...
-00001ca0: 7242 0000 0072 4300 0000 ae00 0000 7244  rB...rC.......rD
-00001cb0: 0000 004e 7a4e 596f 7520 6861 7665 2074  ...NzNYou have t
-00001cc0: 6f20 7375 7070 6c79 2061 2022 7265 6772  o supply a "regr
-00001cd0: 6573 7369 6f6e 5f72 6566 6572 656e 6365  ession_reference
-00001ce0: 2220 7661 6c75 6520 666f 7220 6578 706c  " value for expl
-00001cf0: 616e 6174 696f 6e20 636f 2d74 7261 696e  anation co-train
-00001d00: 696e 6721 7215 0000 007a 4c66 6f72 2065  ing!r....zLfor e
-00001d10: 7870 6c61 6e61 7469 6f6e 2063 6f2d 7472  xplanation co-tr
-00001d20: 6169 6e69 6e67 2c20 7468 6520 6e75 6d62  aining, the numb
-00001d30: 6572 206f 6620 7265 6772 6573 7369 6f6e  er of regression
-00001d40: 5f72 6566 6572 656e 6365 7320 2863 7572  _references (cur
-00001d50: 7265 6e74 6c79 207a 4629 2068 6173 2074  rently zF) has t
-00001d60: 6f20 6265 2065 7861 6374 6c79 2068 616c  o be exactly hal
-00001d70: 6620 7468 6520 6e75 6d62 6572 206f 6620  f the number of 
-00001d80: 696d 706f 7274 616e 6365 2063 6861 6e6e  importance chann
-00001d90: 656c 7320 2863 7572 7265 6e74 6c79 207a  els (currently z
-00001da0: 0229 217a 4c46 6f72 2065 7870 6c61 6e61  .)!zLFor explana
-00001db0: 7469 6f6e 2063 6f2d 7472 6169 6e69 6e67  tion co-training
-00001dc0: 2c20 7468 6520 6e75 6d62 6572 206f 6620  , the number of 
-00001dd0: 7265 6772 6573 7369 6f6e 5f72 6566 6572  regression_refer
-00001de0: 656e 6365 7320 2863 7572 7265 6e74 6c79  ences (currently
-00001df0: 207a 5429 2068 6173 2074 6f20 6265 2065   zT) has to be e
-00001e00: 7861 6374 6c79 2074 6865 2073 616d 6520  xactly the same 
-00001e10: 6173 2074 6865 2066 696e 616c 2075 6e69  as the final uni
-00001e20: 7420 636f 756e 7420 696e 2074 6865 204d  t count in the M
-00001e30: 4c50 2074 6169 6c20 656e 6420 2863 7572  LP tail end (cur
-00001e40: 7265 6e74 6c79 20fa 0129 7a55 2920 6861  rently ..)zU) ha
-00001e50: 7320 746f 2062 6520 6578 6163 746c 7920  s to be exactly 
-00001e60: 7468 6520 7361 6d65 2061 7320 7468 6520  the same as the 
-00001e70: 6e75 6d62 6572 206f 6620 7265 6772 6573  number of regres
-00001e80: 7369 6f6e 5f6c 696d 6974 7320 696e 7465  sion_limits inte
-00001e90: 7276 616c 7320 2863 7572 7265 6e74 6c79  rvals (currently
-00001ea0: 2029 49da 026b 73da 066d 6f64 656c 73da   )I..ks..models.
-00001eb0: 054d 6f64 656c da08 5f5f 696e 6974 5f5f  .Model..__init__
-00001ec0: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
-00001ed0: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
-00001ee0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
-00001ef0: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
-00001f00: 0072 2700 0000 7229 0000 0072 2a00 0000  .r'...r)...r*...
-00001f10: 722b 0000 0072 2c00 0000 722d 0000 0072  r+...r,...r-...r
-00001f20: 2f00 0000 722e 0000 0072 3000 0000 7228  /...r....r0...r(
-00001f30: 0000 0072 3100 0000 da10 6174 7465 6e74  ...r1.....attent
-00001f40: 696f 6e5f 6c61 7965 7273 720e 0000 00da  ion_layersr.....
-00001f50: 0661 7070 656e 6472 0900 0000 da0b 6c61  .appendr......la
-00001f60: 795f 6472 6f70 6f75 7472 0d00 0000 da0c  y_dropoutr......
-00001f70: 6c61 795f 7370 6172 7369 7479 7208 0000  lay_sparsityr...
-00001f80: 00da 126c 6179 5f61 6374 5f69 6d70 6f72  ...lay_act_impor
-00001f90: 7461 6e63 6572 0500 0000 da11 6c61 795f  tancer......lay_
-00001fa0: 636f 6e63 6174 5f61 6c70 6861 7372 0a00  concat_alphasr..
-00001fb0: 0000 da11 6c61 795f 706f 6f6c 5f65 6467  ....lay_pool_edg
-00001fc0: 6573 5f69 6eda 126c 6179 5f70 6f6f 6c5f  es_in..lay_pool_
-00001fd0: 6564 6765 735f 6f75 7472 0600 0000 da0b  edges_outr......
-00001fe0: 6c61 795f 6176 6572 6167 65da 156e 6f64  lay_average..nod
-00001ff0: 655f 696d 706f 7274 616e 6365 5f75 6e69  e_importance_uni
-00002000: 7473 da14 6e6f 6465 5f69 6d70 6f72 7461  ts..node_importa
-00002010: 6e63 655f 6163 7473 da16 6e6f 6465 5f69  nce_acts..node_i
-00002020: 6d70 6f72 7461 6e63 655f 6c61 7965 7273  mportance_layers
-00002030: da03 7a69 7072 0700 0000 720b 0000 00da  ..zipr....r.....
-00002040: 0c6c 6179 5f70 6f6f 6c5f 6f75 74da 0e6c  .lay_pool_out..l
-00002050: 6179 5f63 6f6e 6361 745f 6f75 74da 116c  ay_concat_out..l
-00002060: 6179 5f66 696e 616c 5f64 726f 706f 7574  ay_final_dropout
-00002070: da0a 6669 6e61 6c5f 6163 7473 da0c 6669  ..final_acts..fi
-00002080: 6e61 6c5f 6269 6173 6573 da0c 6669 6e61  nal_biases..fina
-00002090: 6c5f 6c61 7965 7273 da06 6c6f 7373 6573  l_layers..losses
-000020a0: da12 4269 6e61 7279 4372 6f73 7365 6e74  ..BinaryCrossent
-000020b0: 726f 7079 da08 6263 655f 6c6f 7373 7202  ropy..bce_lossr.
-000020c0: 0000 00da 0f4c 6f73 7365 7343 6f6e 7461  .....LossesConta
-000020d0: 696e 6572 7210 0000 00da 1c63 6f6d 7069  inerr......compi
-000020e0: 6c65 645f 636c 6173 7369 6669 6361 7469  led_classificati
-000020f0: 6f6e 5f6c 6f73 73da 104d 6561 6e53 7175  on_loss..MeanSqu
-00002100: 6172 6564 4572 726f 72da 086d 7365 5f6c  aredError..mse_l
-00002110: 6f73 73da 114d 6561 6e41 6273 6f6c 7574  oss..MeanAbsolut
-00002120: 6545 7272 6f72 da08 6d61 655f 6c6f 7373  eError..mae_loss
-00002130: 720f 0000 00da 1863 6f6d 7069 6c65 645f  r......compiled_
-00002140: 7265 6772 6573 7369 6f6e 5f6c 6f73 73da  regression_loss.
-00002150: 0a69 7369 6e73 7461 6e63 65da 0369 6e74  .isinstance..int
-00002160: da05 666c 6f61 74da 036c 656e 2920 da04  ..float..len) ..
-00002170: 7365 6c66 721a 0000 0072 1b00 0000 721c  selfr....r....r.
-00002180: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
-00002190: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
-000021a0: 0072 2300 0000 7224 0000 0072 2500 0000  .r#...r$...r%...
-000021b0: 7226 0000 0072 2700 0000 7228 0000 0072  r&...r'...r(...r
-000021c0: 2900 0000 722a 0000 0072 2b00 0000 722c  )...r*...r+...r,
-000021d0: 0000 0072 2d00 0000 722e 0000 0072 2f00  ...r-...r....r/.
-000021e0: 0000 7230 0000 0072 3100 0000 da06 6b77  ..r0...r1.....kw
-000021f0: 6172 6773 da01 75da 036c 6179 da03 6163  args..u..lay..ac
-00002200: 74da 0462 6961 73da 0e6e 756d 5f72 6566  t..bias..num_ref
-00002210: 6572 656e 6365 73da 0a6e 756d 5f6c 696d  erences..num_lim
-00002220: 6974 7372 3e00 0000 723e 0000 0072 4200  itsr>...r>...rB.
-00002230: 0000 724a 0000 001e 0000 0073 c200 0000  ..rJ.......s....
-00002240: 164a 0601 0601 0601 0601 0601 0601 0601  .J..............
-00002250: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00002260: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00002270: 0601 0603 0a01 0201 0201 0401 0401 0401  ................
-00002280: 0401 0201 0401 06f9 0e09 0e02 0e01 0e03  ................
-00002290: 0c01 0e02 0e01 0801 0e03 1601 0601 1601  ................
-000022a0: 0201 0201 0201 0201 06fd 0e05 0e03 0c01  ................
-000022b0: 0e01 1202 0c01 1201 0a01 0601 1c01 0201  ................
-000022c0: 0201 0201 0201 06fd 1005 0c03 0c01 0c02  ................
-000022d0: 0c01 0c01 0c06 1202 1009 0801 0a02 0a01  ................
-000022e0: 1001 0801 0201 06ff 04ff 1004 0801 0601  ................
-000022f0: 06ff 04ff 0c04 0801 0201 06ff 04ff 04e8  ................
-00002300: 0418 7a0e 4d65 6761 6e2e 5f5f 696e 6974  ..z.Megan.__init
-00002310: 5f5f 6301 0000 0000 0000 0000 0000 0002  __c.............
-00002320: 0000 0007 0000 0003 0000 0073 b600 0000  ...........s....
-00002330: 7400 7401 7c00 8302 a002 a100 7d01 7c01  t.t.|.......}.|.
-00002340: a003 6900 6401 7c00 6a04 9301 6402 7c00  ..i.d.|.j...d.|.
-00002350: 6a05 9301 6403 7c00 6a06 9301 6404 7c00  j...d.|.j...d.|.
-00002360: 6a07 9301 6405 7c00 6a08 9301 6406 7c00  j...d.|.j...d.|.
-00002370: 6a09 9301 6407 7c00 6a0a 9301 6408 7c00  j...d.|.j...d.|.
-00002380: 6a0b 9301 6409 7c00 6a0c 9301 640a 7c00  j...d.|.j...d.|.
-00002390: 6a0d 9301 640b 7c00 6a0e 9301 640c 7c00  j...d.|.j...d.|.
-000023a0: 6a0f 9301 640d 7c00 6a10 9301 640e 7c00  j...d.|.j...d.|.
-000023b0: 6a11 9301 640f 7c00 6a12 9301 6410 7c00  j...d.|.j...d.|.
-000023c0: 6a13 9301 6411 7c00 6a14 9301 7c00 6a15  j...d.|.j...|.j.
-000023d0: 7c00 6a16 7c00 6a17 6412 9c03 a501 a101  |.j.|.j.d.......
-000023e0: 0100 7c01 5300 2913 4e72 1a00 0000 721b  ..|.S.).Nr....r.
-000023f0: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
-00002400: 0000 721f 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-00002410: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
-00002420: 7226 0000 0072 2700 0000 7229 0000 0072  r&...r'...r)...r
-00002430: 2a00 0000 722b 0000 0072 2c00 0000 2903  *...r+...r,...).
-00002440: 722d 0000 0072 2f00 0000 7230 0000 0029  r-...r/...r0...)
-00002450: 18da 0573 7570 6572 7212 0000 00da 0a67  ...superr......g
-00002460: 6574 5f63 6f6e 6669 67da 0675 7064 6174  et_config..updat
-00002470: 6572 1a00 0000 721b 0000 0072 1c00 0000  er....r....r....
-00002480: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00002490: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
-000024a0: 0000 0072 2400 0000 7226 0000 0072 2700  ...r$...r&...r'.
-000024b0: 0000 7229 0000 0072 2a00 0000 722b 0000  ..r)...r*...r+..
-000024c0: 0072 2c00 0000 722d 0000 0072 2f00 0000  .r,...r-...r/...
-000024d0: 7230 0000 0029 0272 6c00 0000 da06 636f  r0...).rl.....co
-000024e0: 6e66 6967 a901 da09 5f5f 636c 6173 735f  nfig....__class_
-000024f0: 5f72 3e00 0000 7242 0000 0072 7500 0000  _r>...rB...ru...
-00002500: e200 0000 7352 0000 000e 0106 0106 0102  ....sR..........
-00002510: ff06 0202 fe06 0302 fd06 0402 fc06 0502  ................
-00002520: fb06 0602 fa06 0702 f906 0802 f806 0902  ................
-00002530: f706 0a02 f606 0b02 f506 0c02 f406 0d02  ................
-00002540: f306 0e02 f206 0f02 f106 1002 f006 1102  ................
-00002550: ef04 1204 0104 010a ec04 177a 104d 6567  ...........z.Meg
-00002560: 616e 2e67 6574 5f63 6f6e 6669 67da 0672  an.get_config..r
-00002570: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
-00002580: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
-00002590: 0000 007c 006a 0064 0075 0153 0029 014e  ...|.j.d.u.S.).N
-000025a0: 2901 722d 0000 0029 0172 6c00 0000 723e  ).r-...).rl...r>
-000025b0: 0000 0072 3e00 0000 7242 0000 00da 1064  ...r>...rB.....d
-000025c0: 6f69 6e67 5f72 6567 7265 7373 696f 6efc  oing_regression.
-000025d0: 0000 0073 0200 0000 0a02 7a16 4d65 6761  ...s......z.Mega
-000025e0: 6e2e 646f 696e 675f 7265 6772 6573 7369  n.doing_regressi
-000025f0: 6f6e da08 7472 6169 6e69 6e67 da15 6e6f  on..training..no
-00002600: 6465 5f69 6d70 6f72 7461 6e63 6573 5f6d  de_importances_m
-00002610: 6173 6b63 0500 0000 0000 0000 0000 0000  askc............
-00002620: 1e00 0000 0600 0000 4b00 0000 7328 0200  ........K...s(..
-00002630: 007c 006a 0072 0a7c 015c 047d 067d 077d  .|.j.r.|.\.}.}.}
-00002640: 087d 096e 077c 015c 037d 067d 077d 0864  .}.n.|.\.}.}.}.d
-00002650: 017d 0967 007d 0a7c 067d 0b7c 006a 0144  .}.g.}.|.}.|.j.D
-00002660: 005d 197d 0c7c 0c7c 0b7c 077c 0867 0383  .].}.|.|.|.|.g..
-00002670: 015c 027d 0b7d 0d7c 0272 2c7c 006a 027c  .\.}.}.|.r,|.j.|
-00002680: 0b7c 0264 028d 027d 0b7c 0aa0 037c 0da1  .|.d...}.|...|..
-00002690: 0101 0071 187c 00a0 047c 0aa1 017d 0a74  ...q.|...|...}.t
-000026a0: 056a 067c 0a64 0364 0464 058d 037d 0e7c  .j.|.d.d.d...}.|
-000026b0: 00a0 077c 0ea1 017d 0e7c 00a0 087c 067c  ...|...}.|...|.|
-000026c0: 0e7c 0867 03a1 017d 0f7c 00a0 097c 067c  .|.g...}.|...|.|
-000026d0: 0e7c 0867 03a1 017d 107c 00a0 0a7c 107c  .|.g...}.|...|.|
-000026e0: 0f67 02a1 017d 117c 0b7d 127c 006a 0b44  .g...}.|.}.|.j.D
-000026f0: 005d 067d 0c7c 0c7c 1283 017d 1271 607c  .].}.|.|...}.q`|
-00002700: 00a0 077c 12a1 017d 127c 127c 1114 007d  ...|...}.|.|...}
-00002710: 137c 00a0 0c7c 13a1 0101 007c 0464 0175  .|...|.....|.d.u
-00002720: 0172 8474 05a0 0d7c 0474 056a 0ea1 027d  .r.t...|.t.j...}
-00002730: 047c 137c 0414 007d 1367 007d 147c 006a  .|.|...}.g.}.|.j
-00002740: 0f64 0319 007d 1574 107c 006a 1183 0144  .d...}.t.|.j...D
-00002750: 005d 2e7d 1674 056a 127c 1364 0164 0185  .].}.t.j.|.d.d..
-00002760: 0264 0164 0185 027c 1666 0319 0064 0364  .d.d...|.f...d.d
-00002770: 068d 027d 177c 0b7c 1714 007d 187c 006a  ...}.|.|...}.|.j
-00002780: 1364 0175 0172 b47c 006a 137c 1619 007d  .d.u.r.|.j.|...}
-00002790: 197c 197c 1883 017d 187c 00a0 147c 18a1  .|.|...}.|...|..
-000027a0: 017d 1a7c 14a0 037c 1aa1 0101 0071 907c  .}.|...|.....q.|
-000027b0: 00a0 157c 14a1 017d 1a7c 006a 0072 ce7c  ...|...}.|.j.r.|
-000027c0: 00a0 157c 1a7c 0967 02a1 017d 1a74 167c  ...|.|.g...}.t.|
-000027d0: 006a 1783 017d 1b74 187c 006a 1783 0144  .j...}.t.|.j...D
-000027e0: 005d 175c 027d 1c7d 0c7c 0c7c 1a83 017d  .].\.}.}.|.|...}
-000027f0: 1a7c 0272 ef7c 1c7c 1b64 0718 006b 0072  .|.r.|.|.d...k.r
-00002800: ef7c 006a 197c 1a7c 0264 028d 027d 1a71  .|.j.|.|.d...}.q
-00002810: d87c 006a 1a90 0172 0674 05a0 1b7c 1aa1  .|.j...r.t...|..
-00002820: 0174 056a 1c7c 006a 1d74 056a 0e64 088d  .t.j.|.j.t.j.d..
-00002830: 0214 007d 1d7c 1a7c 1d17 007d 1a7c 006a  ...}.|.|...}.|.j
-00002840: 1e90 0173 0d7c 0390 0172 127c 1a7c 137c  ...s.|...r.|.|.|
-00002850: 0e66 0353 007c 1a53 0029 0961 b701 0000  .f.S.|.S.).a....
-00002860: 0a20 2020 2020 2020 2046 6f72 7761 7264  .        Forward
-00002870: 2070 6173 7320 6f66 2074 6865 206d 6f64   pass of the mod
-00002880: 656c 2e0a 0a20 2020 2020 2020 202a 2a53  el...        **S
-00002890: 6861 7065 2045 7870 6c61 6e61 7469 6f6e  hape Explanation
-000028a0: 733a 2a2a 2041 6c6c 2073 6861 7065 7320  s:** All shapes 
-000028b0: 696e 2062 7261 636b 6574 7320 5b5d 2061  in brackets [] a
-000028c0: 7265 2072 6167 6765 6420 6469 6d65 6e73  re ragged dimens
-000028d0: 696f 6e73 210a 0a20 2020 2020 2020 202d  ions!..        -
-000028e0: 2056 3a20 4e75 6d20 6e6f 6465 7320 696e   V: Num nodes in
-000028f0: 2074 6865 2067 7261 7068 0a20 2020 2020   the graph.     
-00002900: 2020 202d 2045 3a20 4e75 6d20 6564 6765     - E: Num edge
-00002910: 7320 696e 2074 6865 2067 7261 7068 0a20  s in the graph. 
-00002920: 2020 2020 2020 202d 204e 3a20 4e75 6d20         - N: Num 
-00002930: 6665 6174 7572 6520 7661 6c75 6573 2070  feature values p
-00002940: 6572 206e 6f64 650a 2020 2020 2020 2020  er node.        
-00002950: 2d20 4d3a 204e 556d 2066 6561 7475 7265  - M: NUm feature
-00002960: 2076 616c 7565 7320 7065 7220 6564 6765   values per edge
-00002970: 0a20 2020 2020 2020 202d 2048 3a20 4e75  .        - H: Nu
-00002980: 6d20 6665 6174 7572 6520 7661 6c75 6573  m feature values
-00002990: 2070 6572 2067 7261 7068 0a20 2020 2020   per graph.     
-000029a0: 2020 202d 2042 3a20 4e75 6d20 6772 6170     - B: Num grap
-000029b0: 6873 2069 6e20 6120 6261 7463 680a 2020  hs in a batch.  
-000029c0: 2020 2020 2020 2d20 4b3a 204e 756d 2069        - K: Num i
-000029d0: 6d70 6f72 7461 6e63 6520 2865 7870 6c61  mportance (expla
-000029e0: 6e61 7469 6f6e 2920 6368 616e 6e65 6c73  nation) channels
-000029f0: 2063 6f6e 6669 6775 7265 6420 696e 2074   configured in t
-00002a00: 6865 2063 6f6e 7374 7275 6374 6f72 0a20  he constructor. 
-00002a10: 2020 2020 2020 204e 2901 727c 0000 0072         N).r|...r
-00002a20: 3600 0000 4629 0272 3800 0000 da08 6b65  6...F).r8.....ke
-00002a30: 6570 6469 6d73 7237 0000 0072 1500 0000  epdimsr7...r....
-00002a40: 2901 da05 6474 7970 6529 1f72 3100 0000  )...dtype).r1...
-00002a50: 724b 0000 0072 4d00 0000 724c 0000 0072  rK...rM...rL...r
-00002a60: 5000 0000 da02 7466 da0a 7265 6475 6365  P.....tf..reduce
-00002a70: 5f73 756d 724f 0000 0072 5100 0000 7252  _sumrO...rQ...rR
-00002a80: 0000 0072 5300 0000 7256 0000 0072 4e00  ...rS...rV...rN.
-00002a90: 0000 da04 6361 7374 da07 666c 6f61 7433  ....cast..float3
-00002aa0: 3272 2900 0000 da05 7261 6e67 6572 2000  2r).....ranger .
-00002ab0: 0000 da0b 6578 7061 6e64 5f64 696d 7372  ....expand_dimsr
-00002ac0: 2500 0000 7258 0000 0072 5900 0000 726b  %...rX...rY...rk
-00002ad0: 0000 0072 5d00 0000 da09 656e 756d 6572  ...r].....enumer
-00002ae0: 6174 6572 5a00 0000 727b 0000 00da 096f  aterZ...r{.....o
-00002af0: 6e65 735f 6c69 6b65 da08 636f 6e73 7461  nes_like..consta
-00002b00: 6e74 722f 0000 0072 3000 0000 291e 726c  ntr/...r0...).rl
-00002b10: 0000 00da 0669 6e70 7574 7372 7c00 0000  .....inputsr|...
-00002b20: 7230 0000 0072 7d00 0000 726d 0000 00da  r0...r}...rm....
-00002b30: 0a6e 6f64 655f 696e 7075 74da 0a65 6467  .node_input..edg
-00002b40: 655f 696e 7075 74da 1065 6467 655f 696e  e_input..edge_in
-00002b50: 6465 785f 696e 7075 74da 0b67 7261 7068  dex_input..graph
-00002b60: 5f69 6e70 7574 da06 616c 7068 6173 da01  _input..alphas..
-00002b70: 7872 6f00 0000 da05 616c 7068 61da 1065  xro.....alpha..e
-00002b80: 6467 655f 696d 706f 7274 616e 6365 73da  dge_importances.
-00002b90: 0f70 6f6f 6c65 645f 6564 6765 735f 696e  .pooled_edges_in
-00002ba0: da10 706f 6f6c 6564 5f65 6467 6573 5f6f  ..pooled_edges_o
-00002bb0: 7574 da0c 706f 6f6c 6564 5f65 6467 6573  ut..pooled_edges
-00002bc0: da16 6e6f 6465 5f69 6d70 6f72 7461 6e63  ..node_importanc
-00002bd0: 6573 5f74 696c 6465 da10 6e6f 6465 5f69  es_tilde..node_i
-00002be0: 6d70 6f72 7461 6e63 6573 da04 6f75 7473  mportances..outs
-00002bf0: da01 6eda 016b da15 6e6f 6465 5f69 6d70  ..n..k..node_imp
-00002c00: 6f72 7461 6e63 655f 736c 6963 65da 116d  ortance_slice..m
-00002c10: 6173 6b65 645f 656d 6265 6464 696e 6773  asked_embeddings
-00002c20: da0d 6c61 795f 7472 616e 7366 6f72 6dda  ..lay_transform.
-00002c30: 036f 7574 da10 6e75 6d5f 6669 6e61 6c5f  .out..num_final_
-00002c40: 6c61 7965 7273 da01 63da 0972 6566 6572  layers..c..refer
-00002c50: 656e 6365 723e 0000 0072 3e00 0000 7242  encer>...r>...rB
-00002c60: 0000 00da 0463 616c 6c00 0100 0073 6600  .....call....sf.
-00002c70: 0000 061f 0e01 0a02 0401 0405 0401 0a01  ................
-00002c80: 1203 0401 0e01 0c02 0a04 1001 0a01 1006  ................
-00002c90: 1001 0e01 0402 0a01 0a01 0a02 0802 0a01  ................
-00002ca0: 0809 0e01 0801 0405 0a01 0e01 2001 0801  ............ ...
-00002cb0: 0a05 0a01 0801 0a02 0c03 0a03 0604 0e01  ................
-00002cc0: 0a04 1201 0801 1001 0e01 0280 0802 1c01  ................
-00002cd0: 0801 0e05 0a01 0402 7a0a 4d65 6761 6e2e  ........z.Megan.
-00002ce0: 6361 6c6c 6302 0000 0000 0000 0000 0000  callc...........
-00002cf0: 000c 0000 0006 0000 0043 0000 0073 ce00  .........C...s..
-00002d00: 0000 6700 7d02 6700 7d03 7400 7401 7c00  ..g.}.g.}.t.t.|.
-00002d10: 6a02 7c00 6a03 8302 8301 4400 5d4b 5c02  j.|.j.....D.]K\.
-00002d20: 7d04 5c02 7d05 7d06 7404 7c06 6401 1900  }.\.}.}.t.|.d...
-00002d30: 7c06 6402 1900 1800 8301 7d07 7405 6a06  |.d.......}.t.j.
-00002d40: 7c01 6400 6400 8502 7c04 6602 1900 6403  |.d.d...|.f...d.
-00002d50: 6404 8d02 7d08 7405 a004 7c08 7c05 1800  d...}.t...|.|...
-00002d60: a101 7d09 7c09 7c00 6a07 1400 6405 7c07  ..}.|.|.j...d.|.
-00002d70: 1400 1b00 7d09 7405 a008 7c08 7c05 6b00  ....}.t...|.|.k.
-00002d80: 6406 6407 a103 7d0a 7405 a008 7c08 7c05  d.d...}.t...|.|.
-00002d90: 6b04 6406 6407 a103 7d0b 7c02 7c09 7c09  k.d.d...}.|.|.|.
-00002da0: 6702 3700 7d02 7c03 7c0a 7c0b 6702 3700  g.7.}.|.|.|.g.7.
-00002db0: 7d03 710d 7405 6a09 7c02 6403 6404 8d02  }.q.t.j.|.d.d...
-00002dc0: 7405 6a09 7c03 6403 6404 8d02 6602 5300  t.j.|.d.d...f.S.
-00002dd0: 2908 4e72 1700 0000 7201 0000 0072 3600  ).Nr....r....r6.
-00002de0: 0000 7237 0000 0067 0000 0000 0000 e03f  ..r7...g.......?
-00002df0: 6700 0000 0000 00f0 3f72 1400 0000 290a  g.......?r....).
-00002e00: 7286 0000 0072 5700 0000 722f 0000 0072  r....rW...r/...r
-00002e10: 2d00 0000 da03 6162 7372 8000 0000 7285  -.....absr....r.
-00002e20: 0000 0072 2400 0000 da05 7768 6572 65da  ...r$.....where.
-00002e30: 0663 6f6e 6361 7429 0c72 6c00 0000 da08  .concat).rl.....
-00002e40: 6f75 745f 7472 7565 da07 7361 6d70 6c65  out_true..sample
-00002e50: 73da 056d 6173 6b73 da01 6972 2f00 0000  s..masks..ir/...
-00002e60: 722d 0000 00da 1072 6567 7265 7373 696f  r-.....regressio
-00002e70: 6e5f 7769 6474 68da 0676 616c 7565 73da  n_width..values.
-00002e80: 1063 656e 7465 725f 6469 7374 616e 6365  .center_distance
-00002e90: 73da 076c 6f5f 6d61 736b da07 6869 5f6d  s..lo_mask..hi_m
-00002ea0: 6173 6b72 3e00 0000 723e 0000 0072 4200  askr>...r>...rB.
-00002eb0: 0000 da17 7265 6772 6573 7369 6f6e 5f61  ....regression_a
-00002ec0: 7567 6d65 6e74 6174 696f 6e86 0100 0073  ugmentation....s
-00002ed0: 2000 0000 0402 0401 0801 0401 12ff 1403   ...............
-00002ee0: 1a01 0e01 1201 1208 1202 0c02 0e01 0c03  ................
-00002ef0: 0c01 04fe 7a1d 4d65 6761 6e2e 7265 6772  ....z.Megan.regr
-00002f00: 6573 7369 6f6e 5f61 7567 6d65 6e74 6174  ession_augmentat
-00002f10: 696f 6eda 0e75 7064 6174 655f 7765 6967  ion..update_weig
-00002f20: 6874 7363 0400 0000 0000 0000 0000 0000  htsc............
-00002f30: 1300 0000 0800 0000 4300 0000 733a 0100  ........C...s:..
-00002f40: 007c 006a 0072 097c 025c 037d 047d 057d  .|.j.r.|.\.}.}.}
-00002f50: 056e 027c 027d 0464 017d 0674 01a0 02a1  .n.|.}.d.}.t....
-00002f60: 008f 6c7d 077c 007c 0164 0264 0264 038d  ..l}.|.|.d.d.d..
-00002f70: 037d 087c 085c 037d 097d 0a7d 0b67 007d  .}.|.\.}.}.}.g.}
-00002f80: 0c74 037c 006a 0483 0144 005d 1c7d 0d74  .t.|.j...D.].}.t
-00002f90: 016a 057c 0a64 0064 0085 0264 0064 0085  .j.|.d.d...d.d..
-00002fa0: 027c 0d66 0319 0064 0464 058d 027d 0e7c  .|.f...d.d...}.|
-00002fb0: 00a0 067c 0ea1 017d 0f7c 0ca0 077c 0fa1  ...|...}.|...|..
-00002fc0: 0101 0071 257c 00a0 087c 0ca1 017d 0c7c  ...q%|...|...}.|
-00002fd0: 006a 0972 617c 00a0 0a7c 04a1 015c 027d  .j.ra|...|...\.}
-00002fe0: 047d 107c 0c7d 097c 006a 047c 00a0 0b7c  .}.|.}.|.j.|...|
-00002ff0: 047c 1014 007c 097c 1014 00a1 0214 007d  .|...|.|.......}
-00003000: 066e 1074 0c7c 0c7c 006a 0d64 0664 078d  .n.t.|.|.j.d.d..
-00003010: 037d 097c 00a0 0e7c 047c 097c 0414 00a1  .}.|...|.|.|....
-00003020: 027d 067c 067c 006a 0f39 007d 0657 0064  .}.|.|.j.9.}.W.d
-00003030: 0004 0004 0083 0301 006e 0831 0073 8077  .........n.1.s.w
-00003040: 0101 0001 0001 0059 0001 007c 006a 107d  .......Y...|.j.}
-00003050: 117c 07a0 117c 067c 11a1 027d 127c 0372  .|...|.|...}.|.r
-00003060: 997c 006a 12a0 1374 147c 127c 1183 02a1  .|.j...t.|.|....
-00003070: 0101 0064 087c 0669 0153 0029 094e 7201  ...d.|.i.S.).Nr.
-00003080: 0000 0054 a902 727c 0000 0072 3000 0000  ...T..r|...r0...
-00003090: 7236 0000 0072 3700 0000 7215 0000 00a9  r6...r7...r.....
-000030a0: 02da 0573 6869 6674 da0a 6d75 6c74 6970  ...shift..multip
-000030b0: 6c69 6572 da08 6578 705f 6c6f 7373 2915  lier..exp_loss).
-000030c0: 7230 0000 0072 8000 0000 da0c 4772 6164  r0...r......Grad
-000030d0: 6965 6e74 5461 7065 7284 0000 0072 2000  ientTaper....r .
-000030e0: 0000 7285 0000 0072 5800 0000 724c 0000  ..r....rX...rL..
-000030f0: 0072 5900 0000 727b 0000 0072 ae00 0000  .rY...r{...r....
-00003100: 7267 0000 0072 1100 0000 7224 0000 0072  rg...r....r$...r
-00003110: 6200 0000 7223 0000 00da 1374 7261 696e  b...r#.....train
-00003120: 6162 6c65 5f76 6172 6961 626c 6573 da08  able_variables..
-00003130: 6772 6164 6965 6e74 da09 6f70 7469 6d69  gradient..optimi
-00003140: 7a65 72da 0f61 7070 6c79 5f67 7261 6469  zer..apply_gradi
-00003150: 656e 7473 7257 0000 0029 1372 6c00 0000  entsrW...).rl...
-00003160: 728f 0000 00da 0179 72af 0000 0072 a500  r......yr....r..
-00003170: 0000 7241 0000 0072 b400 0000 da04 7461  ..rA...r......ta
-00003180: 7065 da06 795f 7072 6564 da08 6f75 745f  pe..y_pred..out_
-00003190: 7072 6564 da07 6e69 5f70 7265 64da 0765  pred..ni_pred..e
-000031a0: 695f 7072 6564 7297 0000 0072 9900 0000  i_predr....r....
-000031b0: da16 6e6f 6465 5f69 6d70 6f72 7461 6e63  ..node_importanc
-000031c0: 6573 5f73 6c69 6365 729d 0000 00da 046d  es_slicer......m
-000031d0: 6173 6bda 0e74 7261 696e 6162 6c65 5f76  ask..trainable_v
-000031e0: 6172 73da 0d65 7870 5f67 7261 6469 656e  ars..exp_gradien
-000031f0: 7473 723e 0000 0072 3e00 0000 7242 0000  tsr>...r>...rB..
-00003200: 00da 1674 7261 696e 5f73 7465 705f 6578  ...train_step_ex
-00003210: 706c 616e 6174 696f 6ea4 0100 0073 3800  planation....s8.
-00003220: 0000 0603 0c01 0402 0402 0a01 0e02 0a01  ................
-00003230: 0407 0e01 2001 0a01 0c02 0a03 0602 0e01  .... ...........
-00003240: 0401 0e01 0601 08ff 1005 1001 0c02 1ce1  ................
-00003250: 0622 0c01 0403 1201 0802 7a1c 4d65 6761  ."........z.Mega
-00003260: 6e2e 7472 6169 6e5f 7374 6570 5f65 7870  n.train_step_exp
-00003270: 6c61 6e61 7469 6f6e 6302 0000 0000 0000  lanationc.......
-00003280: 0000 0000 0018 0000 0008 0000 0043 0000  .............C..
-00003290: 0073 d801 0000 7400 7c01 8301 6401 6b02  .s....t.|...d.k.
-000032a0: 720c 7c01 5c03 7d02 7d03 7d04 6e06 6400  r.|.\.}.}.}.n.d.
-000032b0: 7d04 7c01 5c02 7d02 7d03 7c00 6a01 6402  }.|.\.}.}.|.j.d.
-000032c0: 6b03 7221 7c00 6a02 7221 7c00 a003 7c02  k.r!|.j.r!|...|.
-000032d0: 7c03 a102 7d05 6e02 6900 7d05 6402 7d06  |...}.n.i.}.d.}.
-000032e0: 7404 a005 a100 8f8c 7d07 7c03 5c03 7d08  t.......}.|.\.}.
-000032f0: 7d09 7d0a 7c00 7c02 6403 6403 6404 8d03  }.}.|.|.d.d.d...
-00003300: 5c03 7d0b 7d0c 7d0d 7c00 6a06 7c08 7c09  \.}.}.}.|.j.|.|.
-00003310: 7c0a 6703 7c0b 7c0c 7c0d 6703 7c04 7c00  |.g.|.|.|.g.|.|.
-00003320: 6a07 6405 8d04 7d0e 7c00 6a01 6402 6b03  j.d...}.|.j.d.k.
-00003330: 72ae 7c00 6a02 73ae 6700 7d0f 7408 7c00  r.|.j.s.g.}.t.|.
-00003340: 6a09 8301 4400 5d1c 7d10 7404 6a0a 7c0c  j...D.].}.t.j.|.
-00003350: 6400 6400 8502 6400 6400 8502 7c10 6603  d.d...d.d...|.f.
-00003360: 1900 6406 6407 8d02 7d11 7c00 a00b 7c11  ..d.d...}.|...|.
-00003370: a101 7d12 7c0f a00c 7c12 a101 0100 7158  ..}.|...|.....qX
-00003380: 7c00 a00d 7c0f a101 7d0f 7c00 6a0e 7291  |...|...}.|.j.r.
-00003390: 7c00 a00f 7c08 a101 5c02 7d13 7d14 7c0f  |...|...\.}.}.|.
-000033a0: 7d15 7c00 a010 7c13 7c14 1400 7c15 7c14  }.|...|.|...|.|.
-000033b0: 1400 a102 7d06 6e10 7411 7c0f 7c00 6a12  ....}.n.t.|.|.j.
-000033c0: 6408 6409 8d03 7c08 1400 7d15 7c00 a013  d.d...|...}.|...
-000033d0: 7c08 7c15 a102 7d06 7c06 7c00 6a01 3900  |.|...}.|.|.j.9.
-000033e0: 7d06 7c06 7c05 640a 3c00 7c0e 7c06 3700  }.|.|.d.<.|.|.7.
-000033f0: 7d0e 5700 6400 0400 0400 8303 0100 6e08  }.W.d.........n.
-00003400: 3100 73b8 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
-00003410: 7c00 6a14 7d16 7c07 a015 7c0e 7c16 a102  |.j.}.|...|.|...
-00003420: 7d17 7c00 6a16 a017 7418 7c17 7c16 8302  }.|.j...t.|.|...
-00003430: a101 0100 7c00 6a19 6a1a 7c03 7c00 6a1b  ....|.j.j.|.|.j.
-00003440: 73d8 7c0b 6e04 7c0b 7c0c 7c0d 6703 7c04  s.|.n.|.|.|.g.|.
-00003450: 640b 8d03 0100 6900 640c 640d 8400 7c00  d.....i.d.d...|.
-00003460: 6a1c 4400 8301 a501 7c05 a501 5300 290e  j.D.....|...S.).
-00003470: 4ee9 0300 0000 7201 0000 0054 72b0 0000  N.....r....Tr...
-00003480: 0029 02da 0d73 616d 706c 655f 7765 6967  .)...sample_weig
-00003490: 6874 da15 7265 6775 6c61 7269 7a61 7469  ht..regularizati
-000034a0: 6f6e 5f6c 6f73 7365 7372 3600 0000 7237  on_lossesr6...r7
-000034b0: 0000 0072 1700 0000 72b1 0000 0072 b400  ...r....r....r..
-000034c0: 0000 2901 72c6 0000 0063 0100 0000 0000  ..).r....c......
-000034d0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
-000034e0: 0000 7318 0000 0069 007c 005d 087d 017c  ..s....i.|.].}.|
-000034f0: 016a 007c 01a0 01a1 0093 0271 0253 0072  .j.|.......q.S.r
-00003500: 3e00 0000 2902 da04 6e61 6d65 da06 7265  >...)...name..re
-00003510: 7375 6c74 2902 7240 0000 00da 016d 723e  sult).r@.....mr>
-00003520: 0000 0072 3e00 0000 7242 0000 00da 0a3c  ...r>...rB.....<
-00003530: 6469 6374 636f 6d70 3e26 0200 0073 0200  dictcomp>&...s..
-00003540: 0000 1800 7a24 4d65 6761 6e2e 7472 6169  ....z$Megan.trai
-00003550: 6e5f 7374 6570 2e3c 6c6f 6361 6c73 3e2e  n_step.<locals>.
-00003560: 3c64 6963 7463 6f6d 703e 291d 726b 0000  <dictcomp>).rk..
-00003570: 0072 2300 0000 7228 0000 0072 c400 0000  .r#...r(...r....
-00003580: 7280 0000 0072 b500 0000 da0d 636f 6d70  r....r......comp
-00003590: 696c 6564 5f6c 6f73 7372 5e00 0000 7284  iled_lossr^...r.
-000035a0: 0000 0072 2000 0000 7285 0000 0072 5800  ...r ...r....rX.
-000035b0: 0000 724c 0000 0072 5900 0000 727b 0000  ..rL...rY...r{..
-000035c0: 0072 ae00 0000 7267 0000 0072 1100 0000  .r....rg...r....
-000035d0: 7224 0000 0072 6200 0000 72b6 0000 0072  r$...rb...r....r
-000035e0: b700 0000 72b8 0000 0072 b900 0000 7257  ....r....r....rW
-000035f0: 0000 00da 1063 6f6d 7069 6c65 645f 6d65  .....compiled_me
-00003600: 7472 6963 73da 0c75 7064 6174 655f 7374  trics..update_st
-00003610: 6174 6572 3000 0000 da07 6d65 7472 6963  ater0.....metric
-00003620: 7329 1872 6c00 0000 da04 6461 7461 728f  s).rl.....datar.
-00003630: 0000 0072 ba00 0000 72c6 0000 00da 0b65  ...r....r......e
-00003640: 7870 5f6d 6574 7269 6373 72b4 0000 0072  xp_metricsr....r
-00003650: bb00 0000 72a5 0000 00da 076e 695f 7472  ....r......ni_tr
-00003660: 7565 da07 6569 5f74 7275 6572 bd00 0000  ue..ei_truer....
-00003670: 72be 0000 0072 bf00 0000 da04 6c6f 7373  r....r......loss
-00003680: 7297 0000 0072 9900 0000 72c0 0000 0072  r....r....r....r
-00003690: 9d00 0000 da09 5f6f 7574 5f74 7275 6572  ......_out_truer
-000036a0: c100 0000 da09 5f6f 7574 5f70 7265 6472  ......_out_predr
-000036b0: c200 0000 da09 6772 6164 6965 6e74 7372  ......gradientsr
-000036c0: 3e00 0000 723e 0000 0072 4200 0000 da0a  >...r>...rB.....
-000036d0: 7472 6169 6e5f 7374 6570 d801 0000 7370  train_step....sp
-000036e0: 0000 000c 010c 0104 0208 0110 060e 0104  ................
-000036f0: 0204 020a 010a 0214 0104 0108 0108 0102  ................
-00003700: 0104 0106 fc10 0704 060e 0120 010a 010c  ........... ....
-00003710: 020a 0306 020e 0104 010a 0106 0106 ff02  ................
-00003720: 0602 0104 0102 0104 fd02 0404 fc0c 050a  ................
-00003730: 0208 0108 0102 801c d306 2f0c 0112 0206  ........../.....
-00003740: 0202 0112 0102 0106 fd02 080e 0102 ff02  ................
-00003750: 0204 fe7a 104d 6567 616e 2e74 7261 696e  ...z.Megan.train
-00003760: 5f73 7465 7029 0346 464e 7245 0000 0029  _step).FFNrE...)
-00003770: 1ada 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00003780: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00003790: 616d 655f 5fda 075f 5f64 6f63 5f5f da01  ame__..__doc__..
-000037a0: 74da 044c 6973 7472 6900 0000 da03 7374  t..Listri.....st
-000037b0: 72da 0462 6f6f 6c72 6a00 0000 da08 4f70  r..boolrj.....Op
-000037c0: 7469 6f6e 616c 7247 0000 00da 066c 6179  tionalrG.....lay
-000037d0: 6572 73da 054c 6179 6572 da05 5475 706c  ers..Layer..Tupl
-000037e0: 6572 4a00 0000 7275 0000 00da 0870 726f  erJ...ru.....pro
-000037f0: 7065 7274 7972 7b00 0000 7280 0000 00da  pertyr{...r.....
-00003800: 0c52 6167 6765 6454 656e 736f 7272 a100  .RaggedTensorr..
-00003810: 0000 72ae 0000 0072 c400 0000 72d8 0000  ..r....r....r...
-00003820: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00003830: 723e 0000 0072 3e00 0000 7278 0000 0072  r>...r>...rx...r
-00003840: 4200 0000 7212 0000 0014 0000 0073 be00  B...r........s..
-00003850: 0000 0800 0401 020c 0201 0201 0201 0202  ................
-00003860: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00003870: 0201 0402 0201 0201 0201 0201 0201 0201  ................
-00003880: 0201 0201 04e5 0802 02fe 0203 02fd 0204  ................
-00003890: 02fc 0205 02fb 0206 02fa 0808 02f8 0209  ................
-000038a0: 02f7 020a 02f6 020b 02f5 020c 02f4 020d  ................
-000038b0: 02f3 120e 02f2 020f 02f1 0210 02f0 0211  ................
-000038c0: 02ef 0813 02ed 0214 02ec 0215 02eb 0216  ................
-000038d0: 02ea 1217 02e9 1818 02e8 0819 02e7 021a  ................
-000038e0: 02e6 021b 0ae5 007f 0c45 021a 1001 0205  .........E......
-000038f0: 0201 0201 04fc 0202 02fe 0203 02fd 0a04  ................
-00003900: 0afc 007f 0807 021f 04ff 0201 0aff 1034  ...............4
-00003910: 7212 0000 0029 20da 0674 7970 696e 6772  r....) ..typingr
-00003920: dd00 0000 da0a 7465 6e73 6f72 666c 6f77  ......tensorflow
-00003930: 7280 0000 00da 1074 656e 736f 7266 6c6f  r......tensorflo
-00003940: 772e 6b65 7261 73da 056b 6572 6173 7247  w.keras..kerasrG
-00003950: 0000 00da 1e74 656e 736f 7266 6c6f 772e  .....tensorflow.
-00003960: 7079 7468 6f6e 2e6b 6572 6173 2e65 6e67  python.keras.eng
-00003970: 696e 6572 0200 0000 da10 6b67 636e 6e2e  iner......kgcnn.
-00003980: 6461 7461 2e75 7469 6c73 7203 0000 00da  data.utilsr.....
-00003990: 146b 6763 6e6e 2e6c 6179 6572 732e 6d6f  .kgcnn.layers.mo
-000039a0: 6475 6c65 7372 0400 0000 7205 0000 0072  dulesr....r....r
-000039b0: 0600 0000 7207 0000 0072 0800 0000 7209  ....r....r....r.
-000039c0: 0000 00da 146b 6763 6e6e 2e6c 6179 6572  .....kgcnn.layer
-000039d0: 732e 706f 6f6c 696e 6772 0a00 0000 720b  s.poolingr....r.
-000039e0: 0000 0072 0c00 0000 da1e 6772 6170 685f  ...r......graph_
-000039f0: 6174 7465 6e74 696f 6e5f 7374 7564 656e  attention_studen
-00003a00: 742e 6c61 7965 7273 720d 0000 0072 0e00  t.layersr....r..
-00003a10: 0000 da20 6772 6170 685f 6174 7465 6e74  ... graph_attent
-00003a20: 696f 6e5f 7374 7564 656e 742e 7472 6169  ion_student.trai
-00003a30: 6e69 6e67 720f 0000 0072 1000 0000 7211  ningr....r....r.
-00003a40: 0000 0072 4800 0000 7249 0000 0072 1200  ...rH...rI...r..
-00003a50: 0000 723e 0000 0072 3e00 0000 723e 0000  ..r>...r>...r>..
-00003a60: 0072 4200 0000 da08 3c6d 6f64 756c 653e  .rB.....<module>
-00003a70: 0100 0000 7322 0000 0008 0008 020c 010c  ....s"..........
-00003a80: 010c 010c 0110 0114 010c 010c 010c 010c  ................
-00003a90: 010c 010c 010c 010c 0118 03              ...........
+000002a0: 0864 0864 0364 0966 1864 0d65 046a 0565  .d.d.d.f.d.e.j.e
+000002b0: 0619 0064 0e65 0764 0f65 0864 1065 0964  ...d.e.d.e.d.e.d
+000002c0: 1165 0864 1265 046a 0565 0619 0064 1365  .e.d.e.j.e...d.e
+000002d0: 0664 1465 0764 1565 0964 1665 0964 1765  .d.e.d.e.d.e.d.e
+000002e0: 0964 1865 046a 0a65 046a 0565 0b6a 0c6a  .d.e.j.e.j.e.j.j
+000002f0: 0d19 0019 0064 1965 0964 1a65 0864 1b65  .....d.e.d.e.d.e
+00000300: 0864 1c65 046a 0565 0619 0064 1d65 0964  .d.e.j.e...d.e.d
+00000310: 1e65 0764 1f65 0764 2065 046a 0a65 046a  .e.d.e.d e.j.e.j
+00000320: 0e65 0965 0966 0219 0019 0064 2165 046a  .e.e.f.....d!e.j
+00000330: 0a65 046a 0e65 0965 0966 0219 0019 0064  .e.j.e.e.f.....d
+00000340: 2265 046a 0a65 046a 0565 046a 0e65 0965  "e.j.e.j.e.j.e.e
+00000350: 0966 0219 0019 0019 0064 2365 046a 0a65  .f.......d#e.j.e
+00000360: 0919 0064 2465 0864 2565 0866 3264 2664  ...d$e.d%e.f2d&d
+00000370: 2784 055a 0f87 0066 0164 2864 2984 085a  '..Z...f.d(d)..Z
+00000380: 1065 1164 2a65 0866 0264 2b64 2c84 0483  .e.d*e.f.d+d,...
+00000390: 015a 1264 2a65 0866 0264 2d64 2e84 045a  .Z.d*e.f.d-d...Z
+000003a0: 1309 0909 0909 0864 3a64 2f65 0864 2465  .......d:d/e.d$e
+000003b0: 0864 3065 046a 0a65 146a 1519 0066 0664  .d0e.j.e.j...f.d
+000003c0: 3164 3284 055a 1664 3364 3484 005a 1709  1d2..Z.d3d4..Z..
+000003d0: 0364 3b64 3565 0866 0264 3664 3784 055a  .d;d5e.f.d6d7..Z
+000003e0: 1864 3864 3984 005a 1987 0004 005a 1a53  .d8d9..Z.....Z.S
+000003f0: 0029 3cda 054d 6567 616e 613c 0200 000a  .)<..Megana<....
+00000400: 2020 2020 4d45 4741 4e3a 204d 756c 7469      MEGAN: Multi
+00000410: 2045 7870 6c61 6e61 7469 6f6e 2047 7261   Explanation Gra
+00000420: 7068 2041 7474 656e 7469 6f6e 204e 6574  ph Attention Net
+00000430: 776f 726b 0a20 2020 2054 6869 7320 6d6f  work.    This mo
+00000440: 6465 6c20 6375 7272 656e 746c 7920 7375  del currently su
+00000450: 7070 6f72 7473 2067 7261 7068 2072 6567  pports graph reg
+00000460: 7265 7373 696f 6e20 616e 6420 6772 6170  ression and grap
+00000470: 6820 636c 6173 7369 6669 6361 7469 6f6e  h classification
+00000480: 2070 726f 626c 656d 732e 2049 7420 7761   problems. It wa
+00000490: 7320 6d61 696e 6c79 2064 6573 6967 6e65  s mainly designe
+000004a0: 640a 2020 2020 7769 7468 2061 2066 6f63  d.    with a foc
+000004b0: 7573 206f 6e20 6578 706c 6169 6e61 626c  us on explainabl
+000004c0: 6520 4149 2028 5841 4929 2e20 416c 6f6e  e AI (XAI). Alon
+000004d0: 6720 7468 6520 6d61 696e 2070 7265 6469  g the main predi
+000004e0: 6374 696f 6e2c 2074 6869 7320 6d6f 6465  ction, this mode
+000004f0: 6c20 6973 2061 626c 6520 746f 206f 7574  l is able to out
+00000500: 7075 7420 6d75 6c74 6970 6c65 0a20 2020  put multiple.   
+00000510: 2061 7474 656e 7469 6f6e 2d62 6173 6564   attention-based
+00000520: 2065 7870 6c61 6e61 7469 6f6e 7320 666f   explanations fo
+00000530: 7220 7468 6174 2070 7265 6469 6374 696f  r that predictio
+00000540: 6e2e 204d 6f72 6520 7370 6563 6966 6963  n. More specific
+00000550: 616c 6c79 2c20 7468 6520 6d6f 6465 6c20  ally, the model 
+00000560: 6f75 7470 7574 7320 6e6f 6465 2061 6e64  outputs node and
+00000570: 2065 6467 650a 2020 2020 6174 7472 6962   edge.    attrib
+00000580: 7574 696f 6e61 6c20 6578 706c 616e 6174  utional explanat
+00000590: 696f 6e73 2028 6173 7369 676e 696e 6720  ions (assigning 
+000005a0: 5b30 2c20 315d 2076 616c 7565 7320 746f  [0, 1] values to
+000005b0: 2065 7665 7220 6e6f 6465 202f 2065 6467   ever node / edg
+000005c0: 6520 6f66 2074 6865 2069 6e70 7574 2067  e of the input g
+000005d0: 7261 7068 2920 696e 204b 0a20 2020 2073  raph) in K.    s
+000005e0: 6570 6172 6174 6520 6578 706c 616e 6174  eparate explanat
+000005f0: 696f 6e20 6368 616e 6e65 6c73 2c20 7768  ion channels, wh
+00000600: 6572 6520 4b20 6361 6e20 6265 2063 686f  ere K can be cho
+00000610: 7365 6e20 6173 2061 6e20 696e 6465 7065  sen as an indepe
+00000620: 6e64 656e 7420 6d6f 6465 6c20 7061 7261  ndent model para
+00000630: 6d65 7465 722e 0a20 2020 20fa 106b 6763  meter..    ..kgc
+00000640: 6e6e 3e6c 6561 6b79 5f72 656c 7554 e700  nn>leaky_reluT..
+00000650: 0000 0000 0000 00e9 0200 0000 da07 7369  ..............si
+00000660: 676d 6f69 6467 0000 0000 0000 2440 4e46  gmoidg......$@NF
+00000670: e901 0000 00da 066c 696e 6561 72da 0373  .......linear..s
+00000680: 756d da05 756e 6974 73da 0a61 6374 6976  um..units..activ
+00000690: 6174 696f 6eda 0875 7365 5f62 6961 73da  ation..use_bias.
+000006a0: 0c64 726f 706f 7574 5f72 6174 65da 1175  .dropout_rate..u
+000006b0: 7365 5f65 6467 655f 6665 6174 7572 6573  se_edge_features
+000006c0: da10 696d 706f 7274 616e 6365 5f75 6e69  ..importance_uni
+000006d0: 7473 da13 696d 706f 7274 616e 6365 5f63  ts..importance_c
+000006e0: 6861 6e6e 656c 73da 1569 6d70 6f72 7461  hannels..importa
+000006f0: 6e63 655f 6163 7469 7661 7469 6f6e da17  nce_activation..
+00000700: 696d 706f 7274 616e 6365 5f64 726f 706f  importance_dropo
+00000710: 7574 5f72 6174 65da 1169 6d70 6f72 7461  ut_rate..importa
+00000720: 6e63 655f 6661 6374 6f72 da15 696d 706f  nce_factor..impo
+00000730: 7274 616e 6365 5f6d 756c 7469 706c 6965  rtance_multiplie
+00000740: 72da 1a69 6d70 6f72 7461 6e63 655f 7472  r..importance_tr
+00000750: 616e 7366 6f72 6d61 7469 6f6e 73da 0f73  ansformations..s
+00000760: 7061 7273 6974 795f 6661 6374 6f72 da0c  parsity_factor..
+00000770: 636f 6e63 6174 5f68 6561 6473 da19 7365  concat_heads..se
+00000780: 7061 7261 7465 5f65 7870 6c61 6e61 7469  parate_explanati
+00000790: 6f6e 5f73 7465 70da 0b66 696e 616c 5f75  on_step..final_u
+000007a0: 6e69 7473 da12 6669 6e61 6c5f 6472 6f70  nits..final_drop
+000007b0: 6f75 745f 7261 7465 da10 6669 6e61 6c5f  out_rate..final_
+000007c0: 6163 7469 7661 7469 6f6e da0d 6669 6e61  activation..fina
+000007d0: 6c5f 706f 6f6c 696e 67da 1172 6567 7265  l_pooling..regre
+000007e0: 7373 696f 6e5f 6c69 6d69 7473 da12 7265  ssion_limits..re
+000007f0: 6772 6573 7369 6f6e 5f77 6569 6768 7473  gression_weights
+00000800: da0f 7265 6772 6573 7369 6f6e 5f62 696e  ..regression_bin
+00000810: 73da 1472 6567 7265 7373 696f 6e5f 7265  s..regression_re
+00000820: 6665 7265 6e63 65da 1272 6574 7572 6e5f  ference..return_
+00000830: 696d 706f 7274 616e 6365 73da 1475 7365  importances..use
+00000840: 5f67 7261 7068 5f61 7474 7269 6275 7465  _graph_attribute
+00000850: 7363 1a00 0000 0000 0000 0000 0000 2100  sc............!.
+00000860: 0000 0a00 0000 4b00 0000 7362 0300 0074  ......K...sb...t
+00000870: 006a 016a 026a 037c 0066 0169 007c 1aa4  .j.j.j.|.f.i.|..
+00000880: 018e 0101 007c 017c 005f 047c 027c 005f  .....|.|._.|.|._
+00000890: 057c 037c 005f 067c 047c 005f 077c 057c  .|.|._.|.|._.|.|
+000008a0: 005f 087c 067c 005f 097c 077c 005f 0a7c  ._.|.|._.|.|._.|
+000008b0: 087c 005f 0b7c 097c 005f 0c7c 0a7c 005f  .|._.|.|._.|.|._
+000008c0: 0d7c 0b7c 005f 0e7c 0c7c 005f 0f7c 0d7c  .|.|._.|.|._.|.|
+000008d0: 005f 107c 0e7c 005f 117c 107c 005f 127c  ._.|.|._.|.|._.|
+000008e0: 117c 005f 137c 127c 005f 147c 137c 005f  .|._.|.|._.|.|._
+000008f0: 157c 147c 005f 167c 157c 005f 177c 177c  .|.|._.|.|._.|.|
+00000900: 005f 187c 167c 005f 197c 187c 005f 1a7c  ._.|.|._.|.|._.|
+00000910: 0f7c 005f 1b7c 197c 005f 1c67 007c 005f  .|._.|.|._.g.|._
+00000920: 1d7c 006a 0444 005d 187d 1b74 1e7c 1b7c  .|.j.D.].}.t.|.|
+00000930: 006a 0a7c 006a 087c 006a 057c 006a 0664  .j.|.j.|.j.|.j.d
+00000940: 017c 006a 1164 028d 077d 1c7c 006a 1da0  .|.j.d...}.|.j..
+00000950: 1f7c 1ca1 0101 0071 5c74 207c 006a 0764  .|.....q\t |.j.d
+00000960: 038d 017c 005f 2174 227c 006a 1064 048d  ...|._!t"|.j.d..
+00000970: 017c 005f 2374 247c 006a 0b64 058d 017c  .|._#t$|.j.d...|
+00000980: 005f 2574 2664 0664 078d 017c 005f 2774  ._%t&d.d...|._'t
+00000990: 2864 0864 0964 0a8d 027c 005f 2974 2864  (d.d.d...|._)t(d
+000009a0: 0864 0b64 0a8d 027c 005f 2a74 2b83 007c  .d.d...|._*t+..|
+000009b0: 005f 2c7c 067c 006a 0a67 0117 007c 005f  ._,|.|.j.g...|._
+000009c0: 2d64 0c64 0d84 007c 0644 0083 0164 0e67  -d.d...|.D...d.g
+000009d0: 0117 007c 005f 2e67 007c 005f 2f74 307c  ...|._.g.|._/t0|
+000009e0: 006a 2d7c 006a 2e83 0244 005d 115c 027d  .j-|.j...D.].\.}
+000009f0: 1b7d 1d74 317c 1b7c 1d7c 0364 0f8d 037d  .}.t1|.|.|.d...}
+00000a00: 1c7c 006a 2fa0 1f7c 1ca1 0101 0071 be74  .|.j/..|.....q.t
+00000a10: 327c 006a 1564 108d 017c 005f 3374 2664  2|.j.d...|._3t&d
+00000a20: 0664 078d 017c 005f 3474 207c 006a 1364  .d...|._4t |.j.d
+00000a30: 038d 017c 005f 3564 1164 0d84 007c 006a  ...|._5d.d...|.j
+00000a40: 1244 0083 017c 005f 367c 006a 147c 006a  .D...|._6|.j.|.j
+00000a50: 3664 063c 0064 1264 0d84 007c 006a 1244  6d.<.d.d...|.j.D
+00000a60: 0083 017c 005f 3764 017c 006a 3764 063c  ...|._7d.|.j7d.<
+00000a70: 0067 007c 005f 3874 307c 006a 127c 006a  .g.|._8t0|.j.|.j
+00000a80: 367c 006a 3783 0344 005d 135c 037d 1b7d  6|.j7..D.].\.}.}
+00000a90: 1d7d 1e74 317c 1b7c 1d7c 0364 0f8d 037d  .}.t1|.|.|.d...}
+00000aa0: 1c7c 006a 38a0 1f7c 1ca1 0101 0090 0171  .|.j8..|.......q
+00000ab0: 0d74 006a 39a0 3aa1 007c 005f 3b74 3ca0  .t.j9.:..|._;t<.
+00000ac0: 3d74 3ea1 017c 005f 3f74 006a 39a0 40a1  =t>..|._?t.j9.@.
+00000ad0: 007c 005f 4174 006a 39a0 42a1 007c 005f  .|._At.j9.B..|._
+00000ae0: 4374 3ca0 3d74 44a1 017c 005f 457c 006a  Ct<.=tD..|._E|.j
+00000af0: 1864 1375 0190 0172 ad74 467c 1774 4774  .d.u...r.tF|.tGt
+00000b00: 4866 0283 0290 0172 517c 1767 017c 005f  Hf.....rQ|.g.|._
+00000b10: 1874 497c 006a 1883 017d 1f7c 006a 1764  .tI|.j...}.|.j.d
+00000b20: 1375 0190 0172 6274 497c 006a 1783 017d  .u...rbtI|.j...}
+00000b30: 206e 157c 006a 1664 1375 0190 0172 6e74   n.|.j.d.u...rnt
+00000b40: 497c 006a 1683 017d 206e 0974 4a64 147c  I|.j...} n.tJd.|
+00000b50: 006a 189b 0064 159d 0383 0182 017c 1f64  .j...d.......|.d
+00000b60: 1614 007c 076b 0290 0173 894a 0064 177c  ...|.k...s.J.d.|
+00000b70: 1f9b 0064 187c 079b 0064 199d 0583 0182  ...d.|...d......
+00000b80: 017c 1f7c 1064 0619 006b 0290 0173 9d4a  .|.|.d...k...s.J
+00000b90: 0064 1a7c 1f9b 0064 1b7c 1064 0619 009b  .d.|...d.|.d....
+00000ba0: 0064 1c9d 0583 0182 017c 1f7c 206b 0290  .d.......|.| k..
+00000bb0: 0173 af4a 0064 1a7c 1f9b 0064 1d7c 209b  .s.J.d.|...d.| .
+00000bc0: 0064 1c9d 0583 0182 0164 1353 0064 1353  .d.......d.S.d.S
+00000bd0: 0029 1e61 250f 0000 0a20 2020 2020 2020  .).a%....       
+00000be0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00000bf0: 2020 2075 6e69 7473 3a20 4120 6c69 7374     units: A list
+00000c00: 206f 6620 696e 7473 2077 6865 7265 2065   of ints where e
+00000c10: 6163 6820 656c 656d 656e 7420 636f 6e66  ach element conf
+00000c20: 6967 7572 6573 2061 6e20 6164 6469 7469  igures an additi
+00000c30: 6f6e 616c 2061 7474 656e 7469 6f6e 206c  onal attention l
+00000c40: 6179 6572 2e20 5468 6520 6e75 6d65 7269  ayer. The numeri
+00000c50: 630a 2020 2020 2020 2020 2020 2020 2020  c.              
+00000c60: 2020 7661 6c75 6520 6465 7465 726d 696e    value determin
+00000c70: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
+00000c80: 2068 6964 6465 6e20 756e 6974 7320 746f   hidden units to
+00000c90: 2062 6520 7573 6564 2069 6e20 7468 6520   be used in the 
+00000ca0: 6174 7465 6e74 696f 6e20 6865 6164 7320  attention heads 
+00000cb0: 6f66 2074 6861 7420 6c61 7965 720a 2020  of that layer.  
+00000cc0: 2020 2020 2020 2020 2020 6163 7469 7661            activa
+00000cd0: 7469 6f6e 3a20 5468 6520 6163 7469 7661  tion: The activa
+00000ce0: 7469 6f6e 2066 756e 6374 696f 6e20 746f  tion function to
+00000cf0: 2062 6520 7573 6564 2077 6974 6869 6e20   be used within 
+00000d00: 7468 6520 6174 7465 6e74 696f 6e20 6c61  the attention la
+00000d10: 7965 7273 206f 6620 7468 6520 6e65 7477  yers of the netw
+00000d20: 6f72 6b0a 2020 2020 2020 2020 2020 2020  ork.            
+00000d30: 7573 655f 6269 6173 3a20 5768 6574 6865  use_bias: Whethe
+00000d40: 7220 7468 6520 6c61 7965 7273 206f 6620  r the layers of 
+00000d50: 7468 6520 6e65 7477 6f72 6b20 7368 6f75  the network shou
+00000d60: 6c64 2075 7365 2062 6961 7320 7765 6967  ld use bias weig
+00000d70: 6874 7320 6174 2061 6c6c 0a20 2020 2020  hts at all.     
+00000d80: 2020 2020 2020 2064 726f 706f 7574 5f72         dropout_r
+00000d90: 6174 653a 2054 6865 2064 726f 706f 7574  ate: The dropout
+00000da0: 2072 6174 6520 746f 2062 6520 6170 706c   rate to be appl
+00000db0: 6965 6420 6166 7465 7220 2a65 6163 682a  ied after *each*
+00000dc0: 206f 6620 7468 6520 6174 7465 6e74 696f   of the attentio
+00000dd0: 6e20 6c61 7965 7273 206f 6620 7468 6520  n layers of the 
+00000de0: 6e65 7477 6f72 6b2e 0a20 2020 2020 2020  network..       
+00000df0: 2020 2020 2075 7365 5f65 6467 655f 6665       use_edge_fe
+00000e00: 6174 7572 6573 3a20 5768 6574 6865 7220  atures: Whether 
+00000e10: 6564 6765 2066 6561 7475 7265 7320 7368  edge features sh
+00000e20: 6f75 6c64 2062 6520 7573 6564 2e20 4765  ould be used. Ge
+00000e30: 6e65 7261 6c6c 7920 7468 6520 6e65 7477  nerally the netw
+00000e40: 6f72 6b20 7375 7070 6f72 7473 2074 6865  ork supports the
+00000e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e60: 2075 7361 6765 206f 6620 6564 6765 2066   usage of edge f
+00000e70: 6561 7475 7265 732c 2062 7574 2069 6620  eatures, but if 
+00000e80: 7468 6520 696e 7075 7420 6461 7461 2064  the input data d
+00000e90: 6f65 7320 6e6f 7420 636f 6e74 6169 6e20  oes not contain 
+00000ea0: 6564 6765 2066 6561 7475 7265 732c 2074  edge features, t
+00000eb0: 6869 7320 7368 6f75 6c64 2062 650a 2020  his should be.  
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00000ed0: 7420 746f 2046 616c 7365 2e0a 2020 2020  t to False..    
+00000ee0: 2020 2020 2020 2020 696d 706f 7274 616e          importan
+00000ef0: 6365 5f75 6e69 7473 3a20 4120 6c69 7374  ce_units: A list
+00000f00: 206f 6620 696e 7473 2077 6865 7265 2065   of ints where e
+00000f10: 6163 6820 656c 656d 656e 7420 636f 6e66  ach element conf
+00000f20: 6967 7572 6573 2061 6e6f 7468 6572 2064  igures another d
+00000f30: 656e 7365 206c 6179 6572 2069 6e20 7468  ense layer in th
+00000f40: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00000f50: 2020 7375 626e 6574 776f 726b 2074 6861    subnetwork tha
+00000f60: 7420 7072 6f64 7563 6573 2074 6865 206e  t produces the n
+00000f70: 6f64 6520 696d 706f 7274 616e 6365 2074  ode importance t
+00000f80: 656e 736f 7220 6672 6f6d 2074 6865 206d  ensor from the m
+00000f90: 6169 6e20 6e6f 6465 2065 6d62 6564 6469  ain node embeddi
+00000fa0: 6e67 732e 2054 6865 0a20 2020 2020 2020  ngs. The.       
+00000fb0: 2020 2020 2020 2020 206e 756d 6572 6963           numeric
+00000fc0: 2076 616c 7565 2064 6574 6572 6d69 6e65   value determine
+00000fd0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
+00000fe0: 6869 6464 656e 2075 6e69 7473 2069 6e20  hidden units in 
+00000ff0: 7468 6174 206c 6179 6572 2e0a 2020 2020  that layer..    
+00001000: 2020 2020 2020 2020 696d 706f 7274 616e          importan
+00001010: 6365 5f63 6861 6e6e 656c 733a 2054 6865  ce_channels: The
+00001020: 2069 6e74 206e 756d 6265 7220 6f66 2065   int number of e
+00001030: 7870 6c61 6e61 7469 6f6e 2063 6861 6e6e  xplanation chann
+00001040: 656c 7320 746f 2062 6520 7072 6f64 7563  els to be produc
+00001050: 6564 2062 7920 7468 6520 6e65 7477 6f72  ed by the networ
+00001060: 6b2e 2054 6869 730a 2020 2020 2020 2020  k. This.        
+00001070: 2020 2020 2020 2020 6973 2074 6865 2076          is the v
+00001080: 616c 7565 2072 6566 6572 7265 6420 746f  alue referred to
+00001090: 2061 7320 224b 222e 204e 6f74 6520 7468   as "K". Note th
+000010a0: 6174 2074 6869 7320 7769 6c6c 2061 6c73  at this will als
+000010b0: 6f20 6465 7465 726d 696e 6520 7468 6520  o determine the 
+000010c0: 6e75 6d62 6572 206f 6620 6174 7465 6e74  number of attent
+000010d0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000010e0: 2020 2020 6865 6164 7320 7573 6564 2077      heads used w
+000010f0: 6974 6869 6e20 7468 6520 6174 7465 6e74  ithin the attent
+00001100: 696f 6e20 7375 626e 6574 776f 726b 2e0a  ion subnetwork..
+00001110: 2020 2020 2020 2020 2020 2020 696d 706f              impo
+00001120: 7274 616e 6365 5f66 6163 746f 723a 2054  rtance_factor: T
+00001130: 6865 2077 6569 6768 7420 6f66 2074 6865  he weight of the
+00001140: 2065 7870 6c61 6e61 7469 6f6e 2d6f 6e6c   explanation-onl
+00001150: 7920 7472 6169 6e20 7374 6570 2e20 4966  y train step. If
+00001160: 2074 6869 7320 6973 2073 6574 2074 6f20   this is set to 
+00001170: 6578 6163 746c 790a 2020 2020 2020 2020  exactly.        
+00001180: 2020 2020 2020 2020 7a65 726f 2074 6865          zero the
+00001190: 6e20 7468 6520 6578 706c 616e 6174 696f  n the explanatio
+000011a0: 6e20 7472 6169 6e20 7374 6570 2077 696c  n train step wil
+000011b0: 6c20 6e6f 7420 6265 2065 7865 6375 7465  l not be execute
+000011c0: 6420 6174 2061 6c6c 2028 6c65 7373 2063  d at all (less c
+000011d0: 6f6d 7075 7461 7469 6f6e 616c 6c79 0a20  omputationally. 
+000011e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000011f0: 7870 656e 7369 7665 290a 2020 2020 2020  xpensive).      
+00001200: 2020 2020 2020 696d 706f 7274 616e 6365        importance
+00001210: 5f6d 756c 7469 706c 6965 723a 2041 6e20  _multiplier: An 
+00001220: 6164 6469 7469 6f6e 616c 2068 7970 6572  additional hyper
+00001230: 7061 7261 6d65 7465 7220 6f66 2074 6865  parameter of the
+00001240: 2065 7870 6c61 6e61 7469 6f6e 2d6f 6e6c   explanation-onl
+00001250: 7920 7472 6169 6e20 7374 6570 2e20 5468  y train step. Th
+00001260: 6973 0a20 2020 2020 2020 2020 2020 2020  is.             
+00001270: 2020 2069 7320 6573 7365 6e74 6961 6c6c     is essentiall
+00001280: 7920 7468 6520 7363 616c 696e 6720 6661  y the scaling fa
+00001290: 6374 6f72 2074 6861 7420 6973 2061 7070  ctor that is app
+000012a0: 6c69 6564 2074 6f20 7468 6520 7661 6c75  lied to the valu
+000012b0: 6573 206f 6620 7468 6520 6461 7461 7365  es of the datase
+000012c0: 7420 7375 6368 2074 6861 740a 2020 2020  t such that.    
+000012d0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+000012e0: 7461 7267 6574 2076 616c 7565 7320 6361  target values ca
+000012f0: 6e20 7265 6173 6f6e 6162 6c79 2062 6520  n reasonably be 
+00001300: 6170 7072 6f78 696d 6174 6564 2062 7920  approximated by 
+00001310: 6120 7375 6d20 6f66 205b 302c 2031 5d20  a sum of [0, 1] 
+00001320: 696d 706f 7274 616e 6365 2076 616c 7565  importance value
+00001330: 732e 0a20 2020 2020 2020 2020 2020 2073  s..            s
+00001340: 7061 7273 6974 795f 6661 6374 6f72 3a20  parsity_factor: 
+00001350: 5468 6520 636f 6566 6669 6369 656e 7420  The coefficient 
+00001360: 666f 7220 7468 6520 7370 6172 7369 7479  for the sparsity
+00001370: 2072 6567 756c 6172 697a 6174 696f 6e20   regularization 
+00001380: 6f66 2074 6865 206e 6f64 6520 696d 706f  of the node impo
+00001390: 7274 616e 6365 0a20 2020 2020 2020 2020  rtance.         
+000013a0: 2020 2020 2020 2074 656e 736f 722e 0a20         tensor.. 
+000013b0: 2020 2020 2020 2020 2020 2063 6f6e 6361             conca
+000013c0: 745f 6865 6164 733a 2057 6865 7468 6572  t_heads: Whether
+000013d0: 2074 6f20 636f 6e63 6174 2074 6865 2068   to concat the h
+000013e0: 6561 6473 206f 6620 7468 6520 6174 7465  eads of the atte
+000013f0: 6e74 696f 6e20 7375 626e 6574 776f 726b  ntion subnetwork
+00001400: 2e20 5468 6520 6465 6661 756c 7420 6973  . The default is
+00001410: 2054 7275 652e 2049 6e0a 2020 2020 2020   True. In.      
+00001420: 2020 2020 2020 2020 2020 7468 6174 2063            that c
+00001430: 6173 6520 7468 6520 6f75 7470 7574 206f  ase the output o
+00001440: 6620 6561 6368 2069 6e64 6976 6964 7561  f each individua
+00001450: 6c20 6174 7465 6e74 696f 6e20 6865 6164  l attention head
+00001460: 2069 7320 636f 6e63 6174 656e 6174 6564   is concatenated
+00001470: 2061 6e64 2074 6865 2063 6f6e 6361 7465   and the concate
+00001480: 6e61 7465 640a 2020 2020 2020 2020 2020  nated.          
+00001490: 2020 2020 2020 7665 6374 6f72 2069 7320        vector is 
+000014a0: 7468 656e 2075 7365 6420 6173 2074 6865  then used as the
+000014b0: 2069 6e70 7574 206f 6620 7468 6520 6e65   input of the ne
+000014c0: 7874 2061 7474 656e 7469 6f6e 206c 6179  xt attention lay
+000014d0: 6572 2773 2068 6561 6473 2e20 4966 2074  er's heads. If t
+000014e0: 6869 7320 6973 2046 616c 7365 2c20 7468  his is False, th
+000014f0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00001500: 2020 7665 6374 6f72 7320 6172 6520 6176    vectors are av
+00001510: 6572 6167 6520 706f 6f6c 6564 2069 6e73  erage pooled ins
+00001520: 7465 6164 2e0a 2020 2020 2020 2020 2020  tead..          
+00001530: 2020 6669 6e61 6c5f 756e 6974 733a 2041    final_units: A
+00001540: 206c 6973 7420 6f66 2069 6e74 7320 7768   list of ints wh
+00001550: 6572 6520 6561 6368 2065 6c65 6d65 6e74  ere each element
+00001560: 2063 6f6e 6669 6775 7265 7320 616e 6f74   configures anot
+00001570: 6865 7220 6465 6e73 6520 6c61 7965 7220  her dense layer 
+00001580: 696e 2074 6865 204d 4c50 0a20 2020 2020  in the MLP.     
+00001590: 2020 2020 2020 2020 2020 2061 7420 7468             at th
+000015a0: 6520 7461 696c 2065 6e64 206f 6620 7468  e tail end of th
+000015b0: 6520 6e65 7477 6f72 6b2e 2054 6865 206e  e network. The n
+000015c0: 756d 6572 6963 2076 616c 7565 2064 6574  umeric value det
+000015d0: 6572 6d69 6e65 7320 7468 6520 6e75 6d62  ermines the numb
+000015e0: 6572 206f 6620 7468 6520 6869 6464 656e  er of the hidden
+000015f0: 2075 6e69 7473 0a20 2020 2020 2020 2020   units.         
+00001600: 2020 2020 2020 2069 6e20 7468 6174 206c         in that l
+00001610: 6179 6572 2e20 4e6f 7465 2074 6861 7420  ayer. Note that 
+00001620: 7468 6520 6669 6e61 6c20 656c 656d 656e  the final elemen
+00001630: 7420 696e 2074 6869 7320 6c69 7374 2068  t in this list h
+00001640: 6173 2074 6f20 6265 2074 6865 2073 616d  as to be the sam
+00001650: 6520 6173 2074 6865 2064 696d 656e 7369  e as the dimensi
+00001660: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+00001670: 2020 2074 6f20 6265 2065 7870 6563 7465     to be expecte
+00001680: 6420 666f 7220 7468 6520 7361 6d70 6c65  d for the sample
+00001690: 7320 6f66 2074 6865 2074 7261 696e 696e  s of the trainin
+000016a0: 6720 6461 7461 7365 7421 0a20 2020 2020  g dataset!.     
+000016b0: 2020 2020 2020 2066 696e 616c 5f64 726f         final_dro
+000016c0: 706f 7574 5f72 6174 653a 2054 6865 2064  pout_rate: The d
+000016d0: 726f 706f 7574 2072 6174 6520 746f 2062  ropout rate to b
+000016e0: 6520 6170 706c 6965 6420 6166 7465 7220  e applied after 
+000016f0: 2a65 7665 7279 2a20 6c61 7965 7220 6f66  *every* layer of
+00001700: 2074 6865 2066 696e 616c 204d 4c50 2e0a   the final MLP..
+00001710: 2020 2020 2020 2020 2020 2020 6669 6e61              fina
+00001720: 6c5f 6163 7469 7661 7469 6f6e 3a20 5468  l_activation: Th
+00001730: 6520 6163 7469 7661 7469 6f6e 2074 6f20  e activation to 
+00001740: 6265 2061 7070 6c69 6564 2061 7420 7468  be applied at th
+00001750: 6520 7665 7279 206c 6173 7420 6c61 7965  e very last laye
+00001760: 7220 6f66 2074 6865 204d 4c50 2074 6f20  r of the MLP to 
+00001770: 7072 6f64 7563 6520 7468 650a 2020 2020  produce the.    
+00001780: 2020 2020 2020 2020 2020 2020 6163 7475              actu
+00001790: 616c 206f 7574 7075 7420 6f66 2074 6865  al output of the
+000017a0: 206e 6574 776f 726b 2e0a 2020 2020 2020   network..      
+000017b0: 2020 2020 2020 6669 6e61 6c5f 706f 6f6c        final_pool
+000017c0: 696e 673a 2054 6865 2070 6f6f 6c69 6e67  ing: The pooling
+000017d0: 206d 6574 686f 6420 746f 2062 6520 7573   method to be us
+000017e0: 6564 2064 7572 696e 6720 7468 6520 676c  ed during the gl
+000017f0: 6f62 616c 2070 6f6f 6c69 6e67 2070 6861  obal pooling pha
+00001800: 7365 2069 6e20 7468 6520 6e65 7477 6f72  se in the networ
+00001810: 6b2e 0a20 2020 2020 2020 2020 2020 2072  k..            r
+00001820: 6567 7265 7373 696f 6e5f 6c69 6d69 7473  egression_limits
+00001830: 3a20 4120 7475 706c 6520 7768 6572 6520  : A tuple where 
+00001840: 7468 6520 6669 7273 7420 7661 6c75 6520  the first value 
+00001850: 6973 2074 6865 206c 6f77 6572 206c 696d  is the lower lim
+00001860: 6974 2066 6f72 2074 6865 2065 7870 6563  it for the expec
+00001870: 7465 6420 7661 6c75 6520 7261 6e67 650a  ted value range.
+00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001890: 6f66 2074 6865 2072 6567 7265 7373 696f  of the regressio
+000018a0: 6e20 7461 736b 2061 6e64 2074 6568 2073  n task and teh s
+000018b0: 6563 6f6e 6420 7661 6c75 6520 7468 6520  econd value the 
+000018c0: 7570 7065 7220 6c69 6d69 742e 0a20 2020  upper limit..   
+000018d0: 2020 2020 2020 2020 2072 6567 7265 7373           regress
+000018e0: 696f 6e5f 7265 6665 7265 6e63 653a 2041  ion_reference: A
+000018f0: 2072 6566 6572 656e 6365 2076 616c 7565   reference value
+00001900: 2077 6869 6368 2069 7320 696e 7369 6465   which is inside
+00001910: 2074 6865 2072 616e 6765 206f 6620 6578   the range of ex
+00001920: 7065 6374 6564 2076 616c 7565 7320 2862  pected values (b
+00001930: 6573 7420 6966 0a20 2020 2020 2020 2020  est if.         
+00001940: 2020 2020 2020 2069 7420 7761 7320 696e         it was in
+00001950: 2074 6865 206d 6964 646c 652c 2062 7574   the middle, but
+00001960: 2064 6f65 7320 6e6f 7420 6861 7665 2074   does not have t
+00001970: 6f29 2e20 4368 6f6f 7369 6e67 2064 6966  o). Choosing dif
+00001980: 6665 7265 6e74 2072 6566 6572 656e 6365  ferent reference
+00001990: 7320 7769 6c6c 2072 6573 756c 740a 2020  s will result.  
+000019a0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+000019b0: 2064 6966 6665 7265 6e74 2065 7870 6c61   different expla
+000019c0: 6e61 7469 6f6e 732e 0a20 2020 2020 2020  nations..       
+000019d0: 2020 2020 2072 6574 7572 6e5f 696d 706f       return_impo
+000019e0: 7274 616e 6365 733a 2057 6865 7468 6572  rtances: Whether
+000019f0: 2074 6865 2069 6d70 6f72 7461 6e63 6520   the importance 
+00001a00: 2f20 6578 706c 616e 6174 696f 6e20 7465  / explanation te
+00001a10: 6e73 6f72 7320 7368 6f75 6c64 2062 6520  nsors should be 
+00001a20: 7265 7475 726e 6564 2061 7320 616e 206f  returned as an o
+00001a30: 7574 7075 740a 2020 2020 2020 2020 2020  utput.          
+00001a40: 2020 2020 2020 6f66 2074 6865 206d 6f64        of the mod
+00001a50: 656c 2e20 4966 2074 6869 7320 6973 2054  el. If this is T
+00001a60: 7275 652c 2074 6865 206f 7574 7075 7420  rue, the output 
+00001a70: 6f66 2074 6865 206d 6f64 656c 2077 696c  of the model wil
+00001a80: 6c20 6265 2061 2033 2d74 7570 6c65 3a0a  l be a 3-tuple:.
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 286f 7574 7075 742c 206e 6f64 6520 696d  (output, node im
+00001ab0: 706f 7274 616e 6365 732c 2065 6467 6520  portances, edge 
+00001ac0: 696d 706f 7274 616e 6365 7329 2c20 6f74  importances), ot
+00001ad0: 6865 7277 6973 6520 6974 2069 7320 6a75  herwise it is ju
+00001ae0: 7374 2074 6865 206f 7574 7075 7420 6974  st the output it
+00001af0: 7365 6c66 0a20 2020 2020 2020 2054 2907  self.        T).
+00001b00: 721a 0000 00da 096e 756d 5f68 6561 6473  r......num_heads
+00001b10: 721e 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00001b20: 0e68 6173 5f73 656c 665f 6c6f 6f70 7372  .has_self_loopsr
+00001b30: 2700 0000 2901 da04 7261 7465 2901 da06  '...)...rate)...
+00001b40: 6661 6374 6f72 2901 721b 0000 00e9 ffff  factor).r.......
+00001b50: ffff a901 da04 6178 6973 da04 6d65 616e  ......axis..mean
+00001b60: 7201 0000 0029 02da 0e70 6f6f 6c69 6e67  r....)...pooling
+00001b70: 5f6d 6574 686f 64da 0d70 6f6f 6c69 6e67  _method..pooling
+00001b80: 5f69 6e64 6578 7217 0000 0063 0100 0000  _indexr....c....
+00001b90: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001ba0: 5300 0000 f310 0000 0067 007c 005d 047d  S........g.|.].}
+00001bb0: 0164 0091 0271 0253 00a9 0172 1300 0000  .d...q.S...r....
+00001bc0: a900 a902 da02 2e30 da01 5f72 3f00 0000  .......0.._r?...
+00001bd0: 723f 0000 00fa 562f 6d65 6469 612f 7373  r?....V/media/ss
+00001be0: 642f 5072 6f67 7261 6d6d 696e 672f 6772  d/Programming/gr
+00001bf0: 6170 685f 6174 7465 6e74 696f 6e5f 7374  aph_attention_st
+00001c00: 7564 656e 742f 6772 6170 685f 6174 7465  udent/graph_atte
+00001c10: 6e74 696f 6e5f 7374 7564 656e 742f 6d6f  ntion_student/mo
+00001c20: 6465 6c73 2f6d 6567 616e 2e70 79da 0a3c  dels/megan.py..<
+00001c30: 6c69 7374 636f 6d70 3e9f 0000 00f3 0200  listcomp>.......
+00001c40: 0000 1000 7a22 4d65 6761 6e2e 5f5f 696e  ....z"Megan.__in
+00001c50: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c  it__.<locals>.<l
+00001c60: 6973 7463 6f6d 703e 7218 0000 0029 0372  istcomp>r....).r
+00001c70: 1a00 0000 721b 0000 0072 1c00 0000 2901  ....r....r....).
+00001c80: 723b 0000 0063 0100 0000 0000 0000 0000  r;...c..........
+00001c90: 0000 0200 0000 0300 0000 5300 0000 723d  ..........S...r=
+00001ca0: 0000 0072 3e00 0000 723f 0000 0072 4000  ...r>...r?...r@.
+00001cb0: 0000 723f 0000 0072 3f00 0000 7243 0000  ..r?...r?...rC..
+00001cc0: 0072 4400 0000 ae00 0000 7245 0000 0063  .rD.......rE...c
+00001cd0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001ce0: 0300 0000 5300 0000 723d 0000 00a9 0154  ....S...r=.....T
+00001cf0: 723f 0000 0072 4000 0000 723f 0000 0072  r?...r@...r?...r
+00001d00: 3f00 0000 7243 0000 0072 4400 0000 b000  ?...rC...rD.....
+00001d10: 0000 7245 0000 004e 7a3d 596f 7520 6861  ..rE...Nz=You ha
+00001d20: 7665 2073 7570 706c 6965 6420 6120 6e6f  ve supplied a no
+00001d30: 6e2d 6e75 6c6c 2076 616c 7565 2066 6f72  n-null value for
+00001d40: 2072 6567 7265 7373 696f 6e5f 7265 6665   regression_refe
+00001d50: 7265 6e63 653a 207a 682e 2054 6861 7420  rence: zh. That 
+00001d60: 6d65 616e 7320 796f 7520 6e65 6564 2074  means you need t
+00001d70: 6f20 6569 7468 6572 2073 7570 706c 7920  o either supply 
+00001d80: 6120 7661 6c69 6420 7661 6c75 6520 666f  a valid value fo
+00001d90: 7220 7265 6772 6573 7369 6f6e 5f6c 696d  r regression_lim
+00001da0: 6974 7320 6f72 2072 6567 7265 7373 696f  its or regressio
+00001db0: 6e5f 7765 6967 6874 7320 6173 2077 656c  n_weights as wel
+00001dc0: 6c72 1500 0000 7a4c 666f 7220 6578 706c  lr....zLfor expl
+00001dd0: 616e 6174 696f 6e20 636f 2d74 7261 696e  anation co-train
+00001de0: 696e 672c 2074 6865 206e 756d 6265 7220  ing, the number 
+00001df0: 6f66 2072 6567 7265 7373 696f 6e5f 7265  of regression_re
+00001e00: 6665 7265 6e63 6573 2028 6375 7272 656e  ferences (curren
+00001e10: 746c 7920 7a46 2920 6861 7320 746f 2062  tly zF) has to b
+00001e20: 6520 6578 6163 746c 7920 6861 6c66 2074  e exactly half t
+00001e30: 6865 206e 756d 6265 7220 6f66 2069 6d70  he number of imp
+00001e40: 6f72 7461 6e63 6520 6368 616e 6e65 6c73  ortance channels
+00001e50: 2028 6375 7272 656e 746c 7920 7a02 2921   (currently z.)!
+00001e60: 7a4c 466f 7220 6578 706c 616e 6174 696f  zLFor explanatio
+00001e70: 6e20 636f 2d74 7261 696e 696e 672c 2074  n co-training, t
+00001e80: 6865 206e 756d 6265 7220 6f66 2072 6567  he number of reg
+00001e90: 7265 7373 696f 6e5f 7265 6665 7265 6e63  ression_referenc
+00001ea0: 6573 2028 6375 7272 656e 746c 7920 7a54  es (currently zT
+00001eb0: 2920 6861 7320 746f 2062 6520 6578 6163  ) has to be exac
+00001ec0: 746c 7920 7468 6520 7361 6d65 2061 7320  tly the same as 
+00001ed0: 7468 6520 6669 6e61 6c20 756e 6974 2063  the final unit c
+00001ee0: 6f75 6e74 2069 6e20 7468 6520 4d4c 5020  ount in the MLP 
+00001ef0: 7461 696c 2065 6e64 2028 6375 7272 656e  tail end (curren
+00001f00: 746c 7920 fa01 297a 5529 2068 6173 2074  tly ..)zU) has t
+00001f10: 6f20 6265 2065 7861 6374 6c79 2074 6865  o be exactly the
+00001f20: 2073 616d 6520 6173 2074 6865 206e 756d   same as the num
+00001f30: 6265 7220 6f66 2072 6567 7265 7373 696f  ber of regressio
+00001f40: 6e5f 6c69 6d69 7473 2069 6e74 6572 7661  n_limits interva
+00001f50: 6c73 2028 6375 7272 656e 746c 7920 294b  ls (currently )K
+00001f60: da02 6b73 da06 6d6f 6465 6c73 da05 4d6f  ..ks..models..Mo
+00001f70: 6465 6cda 085f 5f69 6e69 745f 5f72 1a00  del..__init__r..
+00001f80: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00001f90: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00001fa0: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
+00001fb0: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
+00001fc0: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
+00001fd0: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
+00001fe0: 0072 3000 0000 722f 0000 0072 3100 0000  .r0...r/...r1...
+00001ff0: 7228 0000 0072 3200 0000 da10 6174 7465  r(...r2.....atte
+00002000: 6e74 696f 6e5f 6c61 7965 7273 720e 0000  ntion_layersr...
+00002010: 00da 0661 7070 656e 6472 0900 0000 da0b  ...appendr......
+00002020: 6c61 795f 6472 6f70 6f75 7472 0d00 0000  lay_dropoutr....
+00002030: da0c 6c61 795f 7370 6172 7369 7479 7208  ..lay_sparsityr.
+00002040: 0000 00da 126c 6179 5f61 6374 5f69 6d70  .....lay_act_imp
+00002050: 6f72 7461 6e63 6572 0500 0000 da11 6c61  ortancer......la
+00002060: 795f 636f 6e63 6174 5f61 6c70 6861 7372  y_concat_alphasr
+00002070: 0a00 0000 da11 6c61 795f 706f 6f6c 5f65  ......lay_pool_e
+00002080: 6467 6573 5f69 6eda 126c 6179 5f70 6f6f  dges_in..lay_poo
+00002090: 6c5f 6564 6765 735f 6f75 7472 0600 0000  l_edges_outr....
+000020a0: da0b 6c61 795f 6176 6572 6167 65da 156e  ..lay_average..n
+000020b0: 6f64 655f 696d 706f 7274 616e 6365 5f75  ode_importance_u
+000020c0: 6e69 7473 da14 6e6f 6465 5f69 6d70 6f72  nits..node_impor
+000020d0: 7461 6e63 655f 6163 7473 da16 6e6f 6465  tance_acts..node
+000020e0: 5f69 6d70 6f72 7461 6e63 655f 6c61 7965  _importance_laye
+000020f0: 7273 da03 7a69 7072 0700 0000 720b 0000  rs..zipr....r...
+00002100: 00da 0c6c 6179 5f70 6f6f 6c5f 6f75 74da  ...lay_pool_out.
+00002110: 0e6c 6179 5f63 6f6e 6361 745f 6f75 74da  .lay_concat_out.
+00002120: 116c 6179 5f66 696e 616c 5f64 726f 706f  .lay_final_dropo
+00002130: 7574 da0a 6669 6e61 6c5f 6163 7473 da0c  ut..final_acts..
+00002140: 6669 6e61 6c5f 6269 6173 6573 da0c 6669  final_biases..fi
+00002150: 6e61 6c5f 6c61 7965 7273 da06 6c6f 7373  nal_layers..loss
+00002160: 6573 da12 4269 6e61 7279 4372 6f73 7365  es..BinaryCrosse
+00002170: 6e74 726f 7079 da08 6263 655f 6c6f 7373  ntropy..bce_loss
+00002180: 7202 0000 00da 0f4c 6f73 7365 7343 6f6e  r......LossesCon
+00002190: 7461 696e 6572 7210 0000 00da 1c63 6f6d  tainerr......com
+000021a0: 7069 6c65 645f 636c 6173 7369 6669 6361  piled_classifica
+000021b0: 7469 6f6e 5f6c 6f73 73da 104d 6561 6e53  tion_loss..MeanS
+000021c0: 7175 6172 6564 4572 726f 72da 086d 7365  quaredError..mse
+000021d0: 5f6c 6f73 73da 114d 6561 6e41 6273 6f6c  _loss..MeanAbsol
+000021e0: 7574 6545 7272 6f72 da08 6d61 655f 6c6f  uteError..mae_lo
+000021f0: 7373 720f 0000 00da 1863 6f6d 7069 6c65  ssr......compile
+00002200: 645f 7265 6772 6573 7369 6f6e 5f6c 6f73  d_regression_los
+00002210: 73da 0a69 7369 6e73 7461 6e63 65da 0369  s..isinstance..i
+00002220: 6e74 da05 666c 6f61 74da 036c 656e da0e  nt..float..len..
+00002230: 4173 7365 7274 696f 6e45 7272 6f72 2921  AssertionError)!
+00002240: da04 7365 6c66 721a 0000 0072 1b00 0000  ..selfr....r....
+00002250: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00002260: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
+00002270: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
+00002280: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
+00002290: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
+000022a0: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
+000022b0: 2f00 0000 7230 0000 0072 3100 0000 7232  /...r0...r1...r2
+000022c0: 0000 00da 066b 7761 7267 73da 0175 da03  .....kwargs..u..
+000022d0: 6c61 79da 0361 6374 da04 6269 6173 da0e  lay..act..bias..
+000022e0: 6e75 6d5f 7265 6665 7265 6e63 6573 da0a  num_references..
+000022f0: 6e75 6d5f 7661 6c75 6573 723f 0000 0072  num_valuesr?...r
+00002300: 3f00 0000 7243 0000 0072 4b00 0000 1e00  ?...rC...rK.....
+00002310: 0000 73ce 0000 0016 4b06 0106 0106 0106  ..s.....K.......
+00002320: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00002330: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00002340: 0106 0106 0106 0106 0106 0106 030a 0102  ................
+00002350: 0102 0104 0104 0104 0104 0102 0104 0106  ................
+00002360: f90e 090e 020e 010e 030c 010e 020e 0108  ................
+00002370: 010e 0316 0106 0116 0102 0102 0102 0102  ................
+00002380: 0106 fd0e 050e 030c 010e 0112 020c 0112  ................
+00002390: 010a 0106 011c 0102 0102 0102 0102 0106  ................
+000023a0: fd10 050c 030c 010c 020c 010c 010c 0710  ................
+000023b0: 0808 010a 020c 020c 010c 010c 0104 0204  ................
+000023c0: 010a ff10 0408 0102 0106 ff04 ff10 0408  ................
+000023d0: 0106 0106 ff04 ff0c 0408 0102 0106 ff04  ................
+000023e0: ff04 e204 1e7a 0e4d 6567 616e 2e5f 5f69  .....z.Megan.__i
+000023f0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00002400: 0000 0200 0000 0900 0000 0300 0000 73be  ..............s.
+00002410: 0000 0074 0074 017c 0083 02a0 02a1 007d  ...t.t.|.......}
+00002420: 017c 01a0 0369 0064 017c 006a 0493 0164  .|...i.d.|.j...d
+00002430: 027c 006a 0593 0164 037c 006a 0693 0164  .|.j...d.|.j...d
+00002440: 047c 006a 0793 0164 057c 006a 0893 0164  .|.j...d.|.j...d
+00002450: 067c 006a 0993 0164 077c 006a 0a93 0164  .|.j...d.|.j...d
+00002460: 087c 006a 0b93 0164 097c 006a 0c93 0164  .|.j...d.|.j...d
+00002470: 0a7c 006a 0d93 0164 0b7c 006a 0e93 0164  .|.j...d.|.j...d
+00002480: 0c7c 006a 0f93 0164 0d7c 006a 1093 0164  .|.j...d.|.j...d
+00002490: 0e7c 006a 1193 0164 0f7c 006a 1293 0164  .|.j...d.|.j...d
+000024a0: 107c 006a 1393 0164 117c 006a 1493 017c  .|.j...d.|.j...|
+000024b0: 006a 157c 006a 167c 006a 177c 006a 187c  .j.|.j.|.j.|.j.|
+000024c0: 006a 1964 129c 05a5 01a1 0101 007c 0153  .j.d.........|.S
+000024d0: 0029 134e 721a 0000 0072 1b00 0000 721c  .).Nr....r....r.
+000024e0: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
+000024f0: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
+00002500: 0072 2300 0000 7224 0000 0072 2600 0000  .r#...r$...r&...
+00002510: 7227 0000 0072 2900 0000 722a 0000 0072  r'...r)...r*...r
+00002520: 2b00 0000 722c 0000 0029 0572 2d00 0000  +...r,...).r-...
+00002530: 722e 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
+00002540: 3200 0000 291a da05 7375 7065 7272 1200  2...)...superr..
+00002550: 0000 da0a 6765 745f 636f 6e66 6967 da06  ....get_config..
+00002560: 7570 6461 7465 721a 0000 0072 1b00 0000  updater....r....
+00002570: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00002580: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
+00002590: 0000 0072 2300 0000 7224 0000 0072 2600  ...r#...r$...r&.
+000025a0: 0000 7227 0000 0072 2900 0000 722a 0000  ..r'...r)...r*..
+000025b0: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+000025c0: 722e 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
+000025d0: 3200 0000 2902 726e 0000 00da 0663 6f6e  2...).rn.....con
+000025e0: 6669 67a9 01da 095f 5f63 6c61 7373 5f5f  fig....__class__
+000025f0: 723f 0000 0072 4300 0000 7277 0000 00eb  r?...rC...rw....
+00002600: 0000 0073 5600 0000 0e01 0601 0601 02ff  ...sV...........
+00002610: 0602 02fe 0603 02fd 0604 02fc 0605 02fb  ................
+00002620: 0606 02fa 0607 02f9 0608 02f8 0609 02f7  ................
+00002630: 060a 02f6 060b 02f5 060c 02f4 060d 02f3  ................
+00002640: 060e 02f2 060f 02f1 0610 02f0 0611 02ef  ................
+00002650: 0412 0401 0401 0401 0401 0aea 0419 7a10  ..............z.
+00002660: 4d65 6761 6e2e 6765 745f 636f 6e66 6967  Megan.get_config
+00002670: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
+00002680: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00002690: 0073 1400 0000 7c00 6a00 6400 7501 7009  .s....|.j.d.u.p.
+000026a0: 7c00 6a01 6400 7501 5300 a901 4e29 0272  |.j.d.u.S...N).r
+000026b0: 2d00 0000 722e 0000 00a9 0172 6e00 0000  -...r......rn...
+000026c0: 723f 0000 0072 3f00 0000 7243 0000 00da  r?...r?...rC....
+000026d0: 1064 6f69 6e67 5f72 6567 7265 7373 696f  .doing_regressio
+000026e0: 6e0a 0100 0073 0200 0000 1402 7a16 4d65  n....s......z.Me
+000026f0: 6761 6e2e 646f 696e 675f 7265 6772 6573  gan.doing_regres
+00002700: 7369 6f6e 6301 0000 0000 0000 0000 0000  sionc...........
+00002710: 0001 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00002720: 0000 7c00 6a00 6400 7501 5300 727d 0000  ..|.j.d.u.S.r}..
+00002730: 0029 0172 2e00 0000 727e 0000 0072 3f00  .).r....r~...r?.
+00002740: 0000 723f 0000 0072 4300 0000 da18 646f  ..r?...rC.....do
+00002750: 696e 675f 7265 6772 6573 7369 6f6e 5f77  ing_regression_w
+00002760: 6569 6768 7473 0e01 0000 7302 0000 000a  eights....s.....
+00002770: 017a 1e4d 6567 616e 2e64 6f69 6e67 5f72  .z.Megan.doing_r
+00002780: 6567 7265 7373 696f 6e5f 7765 6967 6874  egression_weight
+00002790: 73da 0874 7261 696e 696e 67da 156e 6f64  s..training..nod
+000027a0: 655f 696d 706f 7274 616e 6365 735f 6d61  e_importances_ma
+000027b0: 736b 6305 0000 0000 0000 0000 0000 001e  skc.............
+000027c0: 0000 0006 0000 004b 0000 0073 2802 0000  .......K...s(...
+000027d0: 7c00 6a00 720a 7c01 5c04 7d06 7d07 7d08  |.j.r.|.\.}.}.}.
+000027e0: 7d09 6e07 7c01 5c03 7d06 7d07 7d08 6401  }.n.|.\.}.}.}.d.
+000027f0: 7d09 6700 7d0a 7c06 7d0b 7c00 6a01 4400  }.g.}.|.}.|.j.D.
+00002800: 5d19 7d0c 7c0c 7c0b 7c07 7c08 6703 8301  ].}.|.|.|.|.g...
+00002810: 5c02 7d0b 7d0d 7c02 722c 7c00 6a02 7c0b  \.}.}.|.r,|.j.|.
+00002820: 7c02 6402 8d02 7d0b 7c0a a003 7c0d a101  |.d...}.|...|...
+00002830: 0100 7118 7c00 a004 7c0a a101 7d0a 7405  ..q.|...|...}.t.
+00002840: 6a06 7c0a 6403 6404 6405 8d03 7d0e 7c00  j.|.d.d.d...}.|.
+00002850: a007 7c0e a101 7d0e 7c00 a008 7c06 7c0e  ..|...}.|...|.|.
+00002860: 7c08 6703 a101 7d0f 7c00 a009 7c06 7c0e  |.g...}.|...|.|.
+00002870: 7c08 6703 a101 7d10 7c00 a00a 7c10 7c0f  |.g...}.|...|.|.
+00002880: 6702 a101 7d11 7c0b 7d12 7c00 6a0b 4400  g...}.|.}.|.j.D.
+00002890: 5d06 7d0c 7c0c 7c12 8301 7d12 7160 7c00  ].}.|.|...}.q`|.
+000028a0: a007 7c12 a101 7d12 7c12 7c11 1400 7d13  ..|...}.|.|...}.
+000028b0: 7c00 a00c 7c13 a101 0100 7c04 6401 7501  |...|.....|.d.u.
+000028c0: 7284 7405 a00d 7c04 7405 6a0e a102 7d04  r.t...|.t.j...}.
+000028d0: 7c13 7c04 1400 7d13 6700 7d14 7c00 6a0f  |.|...}.g.}.|.j.
+000028e0: 6403 1900 7d15 7410 7c00 6a11 8301 4400  d...}.t.|.j...D.
+000028f0: 5d2e 7d16 7405 6a12 7c13 6401 6401 8502  ].}.t.j.|.d.d...
+00002900: 6401 6401 8502 7c16 6603 1900 6403 6406  d.d...|.f...d.d.
+00002910: 8d02 7d17 7c0b 7c17 1400 7d18 7c00 6a13  ..}.|.|...}.|.j.
+00002920: 6401 7501 72b4 7c00 6a13 7c16 1900 7d19  d.u.r.|.j.|...}.
+00002930: 7c19 7c18 8301 7d18 7c00 a014 7c18 a101  |.|...}.|...|...
+00002940: 7d1a 7c14 a003 7c1a a101 0100 7190 7c00  }.|...|.....q.|.
+00002950: a015 7c14 a101 7d1a 7c00 6a00 72ce 7c00  ..|...}.|.j.r.|.
+00002960: a015 7c1a 7c09 6702 a101 7d1a 7416 7c00  ..|.|.g...}.t.|.
+00002970: 6a17 8301 7d1b 7418 7c00 6a17 8301 4400  j...}.t.|.j...D.
+00002980: 5d17 5c02 7d1c 7d0c 7c0c 7c1a 8301 7d1a  ].\.}.}.|.|...}.
+00002990: 7c02 72ef 7c1c 7c1b 6407 1800 6b00 72ef  |.r.|.|.d...k.r.
+000029a0: 7c00 6a19 7c1a 7c02 6402 8d02 7d1a 71d8  |.j.|.|.d...}.q.
+000029b0: 7c00 6a1a 9001 7206 7405 a01b 7c1a a101  |.j...r.t...|...
+000029c0: 7405 6a1c 7c00 6a1d 7405 6a0e 6408 8d02  t.j.|.j.t.j.d...
+000029d0: 1400 7d1d 7c1a 7c1d 1700 7d1a 7c00 6a1e  ..}.|.|...}.|.j.
+000029e0: 9001 730d 7c03 9001 7212 7c1a 7c13 7c0e  ..s.|...r.|.|.|.
+000029f0: 6603 5300 7c1a 5300 2909 61b7 0100 000a  f.S.|.S.).a.....
+00002a00: 2020 2020 2020 2020 466f 7277 6172 6420          Forward 
+00002a10: 7061 7373 206f 6620 7468 6520 6d6f 6465  pass of the mode
+00002a20: 6c2e 0a0a 2020 2020 2020 2020 2a2a 5368  l...        **Sh
+00002a30: 6170 6520 4578 706c 616e 6174 696f 6e73  ape Explanations
+00002a40: 3a2a 2a20 416c 6c20 7368 6170 6573 2069  :** All shapes i
+00002a50: 6e20 6272 6163 6b65 7473 205b 5d20 6172  n brackets [] ar
+00002a60: 6520 7261 6767 6564 2064 696d 656e 7369  e ragged dimensi
+00002a70: 6f6e 7321 0a0a 2020 2020 2020 2020 2d20  ons!..        - 
+00002a80: 563a 204e 756d 206e 6f64 6573 2069 6e20  V: Num nodes in 
+00002a90: 7468 6520 6772 6170 680a 2020 2020 2020  the graph.      
+00002aa0: 2020 2d20 453a 204e 756d 2065 6467 6573    - E: Num edges
+00002ab0: 2069 6e20 7468 6520 6772 6170 680a 2020   in the graph.  
+00002ac0: 2020 2020 2020 2d20 4e3a 204e 756d 2066        - N: Num f
+00002ad0: 6561 7475 7265 2076 616c 7565 7320 7065  eature values pe
+00002ae0: 7220 6e6f 6465 0a20 2020 2020 2020 202d  r node.        -
+00002af0: 204d 3a20 4e55 6d20 6665 6174 7572 6520   M: NUm feature 
+00002b00: 7661 6c75 6573 2070 6572 2065 6467 650a  values per edge.
+00002b10: 2020 2020 2020 2020 2d20 483a 204e 756d          - H: Num
+00002b20: 2066 6561 7475 7265 2076 616c 7565 7320   feature values 
+00002b30: 7065 7220 6772 6170 680a 2020 2020 2020  per graph.      
+00002b40: 2020 2d20 423a 204e 756d 2067 7261 7068    - B: Num graph
+00002b50: 7320 696e 2061 2062 6174 6368 0a20 2020  s in a batch.   
+00002b60: 2020 2020 202d 204b 3a20 4e75 6d20 696d       - K: Num im
+00002b70: 706f 7274 616e 6365 2028 6578 706c 616e  portance (explan
+00002b80: 6174 696f 6e29 2063 6861 6e6e 656c 7320  ation) channels 
+00002b90: 636f 6e66 6967 7572 6564 2069 6e20 7468  configured in th
+00002ba0: 6520 636f 6e73 7472 7563 746f 720a 2020  e constructor.  
+00002bb0: 2020 2020 2020 4e29 0172 8100 0000 7237        N).r....r7
+00002bc0: 0000 0046 2902 7239 0000 00da 086b 6565  ...F).r9.....kee
+00002bd0: 7064 696d 7372 3800 0000 7215 0000 0029  pdimsr8...r....)
+00002be0: 01da 0564 7479 7065 291f 7232 0000 0072  ...dtype).r2...r
+00002bf0: 4c00 0000 724e 0000 0072 4d00 0000 7251  L...rN...rM...rQ
+00002c00: 0000 00da 0274 66da 0a72 6564 7563 655f  .....tf..reduce_
+00002c10: 7375 6d72 5000 0000 7252 0000 0072 5300  sumrP...rR...rS.
+00002c20: 0000 7254 0000 0072 5700 0000 724f 0000  ..rT...rW...rO..
+00002c30: 00da 0463 6173 74da 0766 6c6f 6174 3332  ...cast..float32
+00002c40: 7229 0000 00da 0572 616e 6765 7220 0000  r).....ranger ..
+00002c50: 00da 0b65 7870 616e 645f 6469 6d73 7225  ...expand_dimsr%
+00002c60: 0000 0072 5900 0000 725a 0000 0072 6c00  ...rY...rZ...rl.
+00002c70: 0000 725e 0000 00da 0965 6e75 6d65 7261  ..r^.....enumera
+00002c80: 7465 725b 0000 0072 7f00 0000 da09 6f6e  ter[...r......on
+00002c90: 6573 5f6c 696b 65da 0863 6f6e 7374 616e  es_like..constan
+00002ca0: 7472 3000 0000 7231 0000 0029 1e72 6e00  tr0...r1...).rn.
+00002cb0: 0000 da06 696e 7075 7473 7281 0000 0072  ....inputsr....r
+00002cc0: 3100 0000 7282 0000 0072 6f00 0000 da0a  1...r....ro.....
+00002cd0: 6e6f 6465 5f69 6e70 7574 da0a 6564 6765  node_input..edge
+00002ce0: 5f69 6e70 7574 da10 6564 6765 5f69 6e64  _input..edge_ind
+00002cf0: 6578 5f69 6e70 7574 da0b 6772 6170 685f  ex_input..graph_
+00002d00: 696e 7075 74da 0661 6c70 6861 73da 0178  input..alphas..x
+00002d10: 7271 0000 00da 0561 6c70 6861 da10 6564  rq.....alpha..ed
+00002d20: 6765 5f69 6d70 6f72 7461 6e63 6573 da0f  ge_importances..
+00002d30: 706f 6f6c 6564 5f65 6467 6573 5f69 6eda  pooled_edges_in.
+00002d40: 1070 6f6f 6c65 645f 6564 6765 735f 6f75  .pooled_edges_ou
+00002d50: 74da 0c70 6f6f 6c65 645f 6564 6765 73da  t..pooled_edges.
+00002d60: 166e 6f64 655f 696d 706f 7274 616e 6365  .node_importance
+00002d70: 735f 7469 6c64 65da 106e 6f64 655f 696d  s_tilde..node_im
+00002d80: 706f 7274 616e 6365 73da 046f 7574 73da  portances..outs.
+00002d90: 016e da01 6bda 156e 6f64 655f 696d 706f  .n..k..node_impo
+00002da0: 7274 616e 6365 5f73 6c69 6365 da11 6d61  rtance_slice..ma
+00002db0: 736b 6564 5f65 6d62 6564 6469 6e67 73da  sked_embeddings.
+00002dc0: 0d6c 6179 5f74 7261 6e73 666f 726d da03  .lay_transform..
+00002dd0: 6f75 74da 106e 756d 5f66 696e 616c 5f6c  out..num_final_l
+00002de0: 6179 6572 73da 0163 da09 7265 6665 7265  ayers..c..refere
+00002df0: 6e63 6572 3f00 0000 723f 0000 0072 4300  ncer?...r?...rC.
+00002e00: 0000 da04 6361 6c6c 1301 0000 7366 0000  ....call....sf..
+00002e10: 0006 1f0e 010a 0204 0104 0504 010a 0112  ................
+00002e20: 0304 010e 010c 020a 0410 010a 0110 0610  ................
+00002e30: 010e 0104 020a 010a 010a 0208 020a 0108  ................
+00002e40: 090e 0108 0104 050a 010e 0120 0108 010a  ........... ....
+00002e50: 050a 0108 010a 020c 030a 0306 040e 010a  ................
+00002e60: 0412 0108 0110 010e 0102 8008 021c 0108  ................
+00002e70: 010e 050a 0104 027a 0a4d 6567 616e 2e63  .......z.Megan.c
+00002e80: 616c 6c63 0200 0000 0000 0000 0000 0000  allc............
+00002e90: 0d00 0000 0900 0000 4300 0000 730c 0100  ........C...s...
+00002ea0: 0067 007d 0267 007d 0374 007c 006a 0183  .g.}.g.}.t.|.j..
+00002eb0: 0144 005d 6e5c 027d 047d 0574 026a 037c  .D.]n\.}.}.t.j.|
+00002ec0: 0164 0064 0085 027c 0466 0219 0064 0164  .d.d...|.f...d.d
+00002ed0: 028d 027d 0674 02a0 047c 067c 0518 00a1  ...}.t...|.|....
+00002ee0: 017d 077c 006a 0572 417c 006a 067c 0419  .}.|.j.rA|.j.|..
+00002ef0: 007d 0874 02a0 077c 067c 056b 007c 077c  .}.t...|.|.k.|.|
+00002f00: 006a 087c 0864 0319 0014 0014 007c 077c  .j.|.d.......|.|
+00002f10: 006a 087c 0864 0419 0014 0014 00a1 037d  .j.|.d.........}
+00002f20: 076e 187c 006a 097c 0419 007d 0974 047c  .n.|.j.|...}.t.|
+00002f30: 0964 0419 007c 0964 0319 0018 0083 017d  .d...|.d.......}
+00002f40: 0a7c 077c 006a 0814 0064 057c 0a14 001b  .|.|.j...d.|....
+00002f50: 007d 0774 02a0 077c 067c 056b 0064 0664  .}.t...|.|.k.d.d
+00002f60: 07a1 037d 0b74 02a0 077c 067c 056b 0464  ...}.t...|.|.k.d
+00002f70: 0664 07a1 037d 0c7c 027c 077c 0767 0237  .d...}.|.|.|.g.7
+00002f80: 007d 027c 037c 0b7c 0c67 0237 007d 0371  .}.|.|.|.g.7.}.q
+00002f90: 0974 026a 0a7c 0264 0164 028d 0274 026a  .t.j.|.d.d...t.j
+00002fa0: 0a7c 0364 0164 028d 0266 0253 0029 084e  .|.d.d...f.S.).N
+00002fb0: 7237 0000 0072 3800 0000 7201 0000 0072  r7...r8...r....r
+00002fc0: 1700 0000 6700 0000 0000 00e0 3f67 0000  ....g.......?g..
+00002fd0: 0000 0000 f03f 7214 0000 0029 0b72 8b00  .....?r....).r..
+00002fe0: 0000 7230 0000 0072 8500 0000 728a 0000  ..r0...r....r...
+00002ff0: 00da 0361 6273 7280 0000 0072 2e00 0000  ...absr....r....
+00003000: da05 7768 6572 6572 2400 0000 722d 0000  ..wherer$...r-..
+00003010: 00da 0663 6f6e 6361 7429 0d72 6e00 0000  ...concat).rn...
+00003020: da08 6f75 745f 7472 7565 da07 7361 6d70  ..out_true..samp
+00003030: 6c65 73da 056d 6173 6b73 da01 6972 3000  les..masks..ir0.
+00003040: 0000 da06 7661 6c75 6573 da10 6365 6e74  ....values..cent
+00003050: 6572 5f64 6973 7461 6e63 6573 722e 0000  er_distancesr...
+00003060: 0072 2d00 0000 da10 7265 6772 6573 7369  .r-.....regressi
+00003070: 6f6e 5f77 6964 7468 da07 6c6f 5f6d 6173  on_width..lo_mas
+00003080: 6bda 0768 695f 6d61 736b 723f 0000 0072  k..hi_maskr?...r
+00003090: 3f00 0000 7243 0000 00da 1772 6567 7265  ?...rC.....regre
+000030a0: 7373 696f 6e5f 6175 676d 656e 7461 7469  ssion_augmentati
+000030b0: 6f6e 9901 0000 732c 0000 0004 0204 0112  on....s,........
+000030c0: 021a 010e 0106 020a 0104 0106 0110 0110  ................
+000030d0: 0106 fd0a 0714 0112 0112 0812 020c 020e  ................
+000030e0: 010c 030c 0104 fe7a 1d4d 6567 616e 2e72  .......z.Megan.r
+000030f0: 6567 7265 7373 696f 6e5f 6175 676d 656e  egression_augmen
+00003100: 7461 7469 6f6e da0e 7570 6461 7465 5f77  tation..update_w
+00003110: 6569 6768 7473 6304 0000 0000 0000 0000  eightsc.........
+00003120: 0000 0013 0000 0008 0000 0043 0000 0073  ...........C...s
+00003130: 3a01 0000 7c00 6a00 7209 7c02 5c03 7d04  :...|.j.r.|.\.}.
+00003140: 7d05 7d05 6e02 7c02 7d04 6401 7d06 7401  }.}.n.|.}.d.}.t.
+00003150: a002 a100 8f6c 7d07 7c00 7c01 6402 6402  .....l}.|.|.d.d.
+00003160: 6403 8d03 7d08 7c08 5c03 7d09 7d0a 7d0b  d...}.|.\.}.}.}.
+00003170: 6700 7d0c 7403 7c00 6a04 8301 4400 5d1c  g.}.t.|.j...D.].
+00003180: 7d0d 7401 6a05 7c0a 6400 6400 8502 6400  }.t.j.|.d.d...d.
+00003190: 6400 8502 7c0d 6603 1900 6404 6405 8d02  d...|.f...d.d...
+000031a0: 7d0e 7c00 a006 7c0e a101 7d0f 7c0c a007  }.|...|...}.|...
+000031b0: 7c0f a101 0100 7125 7c00 a008 7c0c a101  |.....q%|...|...
+000031c0: 7d0c 7c00 6a09 7261 7c00 a00a 7c04 a101  }.|.j.ra|...|...
+000031d0: 5c02 7d04 7d10 7c0c 7d09 7c00 6a04 7c00  \.}.}.|.}.|.j.|.
+000031e0: a00b 7c04 7c10 1400 7c09 7c10 1400 a102  ..|.|...|.|.....
+000031f0: 1400 7d06 6e10 740c 7c0c 7c00 6a0d 6406  ..}.n.t.|.|.j.d.
+00003200: 6407 8d03 7d09 7c00 a00e 7c04 7c09 7c04  d...}.|...|.|.|.
+00003210: 1400 a102 7d06 7c06 7c00 6a0f 3900 7d06  ....}.|.|.j.9.}.
+00003220: 5700 6400 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
+00003230: 7380 7701 0100 0100 0100 5900 0100 7c00  s.w.......Y...|.
+00003240: 6a10 7d11 7c07 a011 7c06 7c11 a102 7d12  j.}.|...|.|...}.
+00003250: 7c03 7299 7c00 6a12 a013 7414 7c12 7c11  |.r.|.j...t.|.|.
+00003260: 8302 a101 0100 6408 7c06 6901 5300 2909  ......d.|.i.S.).
+00003270: 4e72 0100 0000 54a9 0272 8100 0000 7231  Nr....T..r....r1
+00003280: 0000 0072 3700 0000 7238 0000 0072 1500  ...r7...r8...r..
+00003290: 0000 a902 da05 7368 6966 74da 0a6d 756c  ......shift..mul
+000032a0: 7469 706c 6965 72da 0865 7870 5f6c 6f73  tiplier..exp_los
+000032b0: 7329 1572 3100 0000 7285 0000 00da 0c47  s).r1...r......G
+000032c0: 7261 6469 656e 7454 6170 6572 8900 0000  radientTaper....
+000032d0: 7220 0000 0072 8a00 0000 7259 0000 0072  r ...r....rY...r
+000032e0: 4d00 0000 725a 0000 0072 7f00 0000 72b3  M...rZ...r....r.
+000032f0: 0000 0072 6800 0000 7211 0000 0072 2400  ...rh...r....r$.
+00003300: 0000 7263 0000 0072 2300 0000 da13 7472  ..rc...r#.....tr
+00003310: 6169 6e61 626c 655f 7661 7269 6162 6c65  ainable_variable
+00003320: 73da 0867 7261 6469 656e 74da 096f 7074  s..gradient..opt
+00003330: 696d 697a 6572 da0f 6170 706c 795f 6772  imizer..apply_gr
+00003340: 6164 6965 6e74 7372 5800 0000 2913 726e  adientsrX...).rn
+00003350: 0000 0072 9400 0000 da01 7972 b400 0000  ...r......yr....
+00003360: 72aa 0000 0072 4200 0000 72b9 0000 00da  r....rB...r.....
+00003370: 0474 6170 65da 0679 5f70 7265 64da 086f  .tape..y_pred..o
+00003380: 7574 5f70 7265 64da 076e 695f 7072 6564  ut_pred..ni_pred
+00003390: da07 6569 5f70 7265 6472 9c00 0000 729e  ..ei_predr....r.
+000033a0: 0000 00da 166e 6f64 655f 696d 706f 7274  .....node_import
+000033b0: 616e 6365 735f 736c 6963 6572 a200 0000  ances_slicer....
+000033c0: da04 6d61 736b da0e 7472 6169 6e61 626c  ..mask..trainabl
+000033d0: 655f 7661 7273 da0d 6578 705f 6772 6164  e_vars..exp_grad
+000033e0: 6965 6e74 7372 3f00 0000 723f 0000 0072  ientsr?...r?...r
+000033f0: 4300 0000 da16 7472 6169 6e5f 7374 6570  C.....train_step
+00003400: 5f65 7870 6c61 6e61 7469 6f6e c101 0000  _explanation....
+00003410: 7338 0000 0006 030c 0104 0204 020a 010e  s8..............
+00003420: 020a 0104 070e 0120 010a 010c 020a 0306  ....... ........
+00003430: 020e 0104 010e 0106 0108 ff10 0510 010c  ................
+00003440: 021c e106 220c 0104 0312 0108 027a 1c4d  ...."........z.M
+00003450: 6567 616e 2e74 7261 696e 5f73 7465 705f  egan.train_step_
+00003460: 6578 706c 616e 6174 696f 6e63 0200 0000  explanationc....
+00003470: 0000 0000 0000 0000 1800 0000 0800 0000  ................
+00003480: 4300 0000 73d8 0100 0074 007c 0183 0164  C...s....t.|...d
+00003490: 016b 0272 0c7c 015c 037d 027d 037d 046e  .k.r.|.\.}.}.}.n
+000034a0: 0664 007d 047c 015c 027d 027d 037c 006a  .d.}.|.\.}.}.|.j
+000034b0: 0164 026b 0372 217c 006a 0272 217c 00a0  .d.k.r!|.j.r!|..
+000034c0: 037c 027c 03a1 027d 056e 0269 007d 0564  .|.|...}.n.i.}.d
+000034d0: 027d 0674 04a0 05a1 008f 8c7d 077c 035c  .}.t.......}.|.\
+000034e0: 037d 087d 097d 0a7c 007c 0264 0364 0364  .}.}.}.|.|.d.d.d
+000034f0: 048d 035c 037d 0b7d 0c7d 0d7c 006a 067c  ...\.}.}.}.|.j.|
+00003500: 087c 097c 0a67 037c 0b7c 0c7c 0d67 037c  .|.|.g.|.|.|.g.|
+00003510: 047c 006a 0764 058d 047d 0e7c 006a 0164  .|.j.d...}.|.j.d
+00003520: 026b 0372 ae7c 006a 0273 ae67 007d 0f74  .k.r.|.j.s.g.}.t
+00003530: 087c 006a 0983 0144 005d 1c7d 1074 046a  .|.j...D.].}.t.j
+00003540: 0a7c 0c64 0064 0085 0264 0064 0085 027c  .|.d.d...d.d...|
+00003550: 1066 0319 0064 0664 078d 027d 117c 00a0  .f...d.d...}.|..
+00003560: 0b7c 11a1 017d 127c 0fa0 0c7c 12a1 0101  .|...}.|...|....
+00003570: 0071 587c 00a0 0d7c 0fa1 017d 0f7c 006a  .qX|...|...}.|.j
+00003580: 0e72 917c 00a0 0f7c 08a1 015c 027d 137d  .r.|...|...\.}.}
+00003590: 147c 0f7d 157c 00a0 107c 137c 1414 007c  .|.}.|...|.|...|
+000035a0: 157c 1414 00a1 027d 066e 1074 117c 0f7c  .|.....}.n.t.|.|
+000035b0: 006a 1264 0864 098d 037c 0814 007d 157c  .j.d.d...|...}.|
+000035c0: 00a0 137c 087c 15a1 027d 067c 067c 006a  ...|.|...}.|.|.j
+000035d0: 0139 007d 067c 067c 0564 0a3c 007c 0e7c  .9.}.|.|.d.<.|.|
+000035e0: 0637 007d 0e57 0064 0004 0004 0083 0301  .7.}.W.d........
+000035f0: 006e 0831 0073 b877 0101 0001 0001 0059  .n.1.s.w.......Y
+00003600: 0001 007c 006a 147d 167c 07a0 157c 0e7c  ...|.j.}.|...|.|
+00003610: 16a1 027d 177c 006a 16a0 1774 187c 177c  ...}.|.j...t.|.|
+00003620: 1683 02a1 0101 007c 006a 196a 1a7c 037c  .......|.j.j.|.|
+00003630: 006a 1b73 d87c 0b6e 047c 0b7c 0c7c 0d67  .j.s.|.n.|.|.|.g
+00003640: 037c 0464 0b8d 0301 0069 0064 0c64 0d84  .|.d.....i.d.d..
+00003650: 007c 006a 1c44 0083 01a5 017c 05a5 0153  .|.j.D.....|...S
+00003660: 0029 0e4e e903 0000 0072 0100 0000 5472  .).N.....r....Tr
+00003670: b500 0000 2902 da0d 7361 6d70 6c65 5f77  ....)...sample_w
+00003680: 6569 6768 74da 1572 6567 756c 6172 697a  eight..regulariz
+00003690: 6174 696f 6e5f 6c6f 7373 6573 7237 0000  ation_lossesr7..
+000036a0: 0072 3800 0000 7217 0000 0072 b600 0000  .r8...r....r....
+000036b0: 72b9 0000 0029 0172 cb00 0000 6301 0000  r....).r....c...
+000036c0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+000036d0: 0053 0000 0073 1800 0000 6900 7c00 5d08  .S...s....i.|.].
+000036e0: 7d01 7c01 6a00 7c01 a001 a100 9302 7102  }.|.j.|.......q.
+000036f0: 5300 723f 0000 0029 02da 046e 616d 65da  S.r?...)...name.
+00003700: 0672 6573 756c 7429 0272 4100 0000 da01  .result).rA.....
+00003710: 6d72 3f00 0000 723f 0000 0072 4300 0000  mr?...r?...rC...
+00003720: da0a 3c64 6963 7463 6f6d 703e 4302 0000  ..<dictcomp>C...
+00003730: 7302 0000 0018 007a 244d 6567 616e 2e74  s......z$Megan.t
+00003740: 7261 696e 5f73 7465 702e 3c6c 6f63 616c  rain_step.<local
+00003750: 733e 2e3c 6469 6374 636f 6d70 3e29 1d72  s>.<dictcomp>).r
+00003760: 6c00 0000 7223 0000 0072 2800 0000 72c9  l...r#...r(...r.
+00003770: 0000 0072 8500 0000 72ba 0000 00da 0d63  ...r....r......c
+00003780: 6f6d 7069 6c65 645f 6c6f 7373 725f 0000  ompiled_lossr_..
+00003790: 0072 8900 0000 7220 0000 0072 8a00 0000  .r....r ...r....
+000037a0: 7259 0000 0072 4d00 0000 725a 0000 0072  rY...rM...rZ...r
+000037b0: 7f00 0000 72b3 0000 0072 6800 0000 7211  ....r....rh...r.
+000037c0: 0000 0072 2400 0000 7263 0000 0072 bb00  ...r$...rc...r..
+000037d0: 0000 72bc 0000 0072 bd00 0000 72be 0000  ..r....r....r...
+000037e0: 0072 5800 0000 da10 636f 6d70 696c 6564  .rX.....compiled
+000037f0: 5f6d 6574 7269 6373 da0c 7570 6461 7465  _metrics..update
+00003800: 5f73 7461 7465 7231 0000 00da 076d 6574  _stater1.....met
+00003810: 7269 6373 2918 726e 0000 00da 0464 6174  rics).rn.....dat
+00003820: 6172 9400 0000 72bf 0000 0072 cb00 0000  ar....r....r....
+00003830: da0b 6578 705f 6d65 7472 6963 7372 b900  ..exp_metricsr..
+00003840: 0000 72c0 0000 0072 aa00 0000 da07 6e69  ..r....r......ni
+00003850: 5f74 7275 65da 0765 695f 7472 7565 72c2  _true..ei_truer.
+00003860: 0000 0072 c300 0000 72c4 0000 00da 046c  ...r....r......l
+00003870: 6f73 7372 9c00 0000 729e 0000 0072 c500  ossr....r....r..
+00003880: 0000 72a2 0000 00da 095f 6f75 745f 7472  ..r......_out_tr
+00003890: 7565 72c6 0000 00da 095f 6f75 745f 7072  uer......_out_pr
+000038a0: 6564 72c7 0000 00da 0967 7261 6469 656e  edr......gradien
+000038b0: 7473 723f 0000 0072 3f00 0000 7243 0000  tsr?...r?...rC..
+000038c0: 00da 0a74 7261 696e 5f73 7465 70f5 0100  ...train_step...
+000038d0: 0073 7000 0000 0c01 0c01 0402 0801 1006  .sp.............
+000038e0: 0e01 0402 0402 0a01 0a02 1401 0401 0801  ................
+000038f0: 0801 0201 0401 06fc 1007 0406 0e01 2001  .............. .
+00003900: 0a01 0c02 0a03 0602 0e01 0401 0a01 0601  ................
+00003910: 06ff 0206 0201 0401 0201 04fd 0204 04fc  ................
+00003920: 0c05 0a02 0801 0801 0280 1cd3 062f 0c01  ............./..
+00003930: 1202 0602 0201 1201 0201 06fd 0208 0e01  ................
+00003940: 02ff 0202 04fe 7a10 4d65 6761 6e2e 7472  ......z.Megan.tr
+00003950: 6169 6e5f 7374 6570 2903 4646 4e72 4600  ain_step).FFNrF.
+00003960: 0000 291b da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00003970: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00003980: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00003990: 5fda 0174 da04 4c69 7374 726a 0000 00da  _..t..Listrj....
+000039a0: 0373 7472 da04 626f 6f6c 726b 0000 00da  .str..boolrk....
+000039b0: 084f 7074 696f 6e61 6c72 4800 0000 da06  .OptionalrH.....
+000039c0: 6c61 7965 7273 da05 4c61 7965 72da 0554  layers..Layer..T
+000039d0: 7570 6c65 724b 0000 0072 7700 0000 da08  uplerK...rw.....
+000039e0: 7072 6f70 6572 7479 727f 0000 0072 8000  propertyr....r..
+000039f0: 0000 7285 0000 00da 0c52 6167 6765 6454  ..r......RaggedT
+00003a00: 656e 736f 7272 a600 0000 72b3 0000 0072  ensorr....r....r
+00003a10: c900 0000 72dd 0000 00da 0d5f 5f63 6c61  ....r......__cla
+00003a20: 7373 6365 6c6c 5f5f 723f 0000 0072 3f00  sscell__r?...r?.
+00003a30: 0000 727a 0000 0072 4300 0000 7212 0000  ..rz...rC...r...
+00003a40: 0014 0000 0073 c600 0000 0800 0401 020c  .....s..........
+00003a50: 0201 0201 0201 0202 0201 0201 0201 0201  ................
+00003a60: 0201 0201 0201 0201 0201 0402 0201 0201  ................
+00003a70: 0201 0201 0201 0201 0201 0201 0201 04e4  ................
+00003a80: 0802 02fe 0203 02fd 0204 02fc 0205 02fb  ................
+00003a90: 0206 02fa 0808 02f8 0209 02f7 020a 02f6  ................
+00003aa0: 020b 02f5 020c 02f4 020d 02f3 120e 02f2  ................
+00003ab0: 020f 02f1 0210 02f0 0211 02ef 0813 02ed  ................
+00003ac0: 0214 02ec 0215 02eb 0216 02ea 1217 02e9  ................
+00003ad0: 1218 02e8 1819 02e7 081a 02e6 021b 02e5  ................
+00003ae0: 021c 0ae4 007f 0c4e 021f 1001 0e03 0207  .......N........
+00003af0: 0201 0201 04fc 0202 02fe 0203 02fd 0a04  ................
+00003b00: 0afc 007f 0807 0229 04ff 0201 0aff 1034  .......).......4
+00003b10: 7212 0000 0029 20da 0674 7970 696e 6772  r....) ..typingr
+00003b20: e200 0000 da0a 7465 6e73 6f72 666c 6f77  ......tensorflow
+00003b30: 7285 0000 00da 1074 656e 736f 7266 6c6f  r......tensorflo
+00003b40: 772e 6b65 7261 73da 056b 6572 6173 7248  w.keras..kerasrH
+00003b50: 0000 00da 1e74 656e 736f 7266 6c6f 772e  .....tensorflow.
+00003b60: 7079 7468 6f6e 2e6b 6572 6173 2e65 6e67  python.keras.eng
+00003b70: 696e 6572 0200 0000 da10 6b67 636e 6e2e  iner......kgcnn.
+00003b80: 6461 7461 2e75 7469 6c73 7203 0000 00da  data.utilsr.....
+00003b90: 146b 6763 6e6e 2e6c 6179 6572 732e 6d6f  .kgcnn.layers.mo
+00003ba0: 6475 6c65 7372 0400 0000 7205 0000 0072  dulesr....r....r
+00003bb0: 0600 0000 7207 0000 0072 0800 0000 7209  ....r....r....r.
+00003bc0: 0000 00da 146b 6763 6e6e 2e6c 6179 6572  .....kgcnn.layer
+00003bd0: 732e 706f 6f6c 696e 6772 0a00 0000 720b  s.poolingr....r.
+00003be0: 0000 0072 0c00 0000 da1e 6772 6170 685f  ...r......graph_
+00003bf0: 6174 7465 6e74 696f 6e5f 7374 7564 656e  attention_studen
+00003c00: 742e 6c61 7965 7273 720d 0000 0072 0e00  t.layersr....r..
+00003c10: 0000 da20 6772 6170 685f 6174 7465 6e74  ... graph_attent
+00003c20: 696f 6e5f 7374 7564 656e 742e 7472 6169  ion_student.trai
+00003c30: 6e69 6e67 720f 0000 0072 1000 0000 7211  ningr....r....r.
+00003c40: 0000 0072 4900 0000 724a 0000 0072 1200  ...rI...rJ...r..
+00003c50: 0000 723f 0000 0072 3f00 0000 723f 0000  ..r?...r?...r?..
+00003c60: 0072 4300 0000 da08 3c6d 6f64 756c 653e  .rC.....<module>
+00003c70: 0100 0000 7322 0000 0008 0008 020c 010c  ....s"..........
+00003c80: 010c 010c 0110 0114 010c 010c 010c 010c  ................
+00003c90: 010c 010c 010c 010c 0118 03              ...........
```

### Comparing `graph_attention_student-0.7.1/graph_attention_student/models/gnes.py` & `graph_attention_student-0.7.2/graph_attention_student/models/gnes.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/models/gnnx.py` & `graph_attention_student-0.7.2/graph_attention_student/models/gnnx.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/models/gradient.py` & `graph_attention_student-0.7.2/graph_attention_student/models/gradient.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/models/megan.py` & `graph_attention_student-0.7.2/graph_attention_student/models/megan.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
                  separate_explanation_step: bool = False,
                  # mlp tail end related arguments
                  final_units: t.List[int] = [1],
                  final_dropout_rate: float = 0.0,
                  final_activation: str = 'linear',
                  final_pooling: str = 'sum',
                  regression_limits: t.Optional[t.Tuple[float, float]] = None,
+                 regression_weights: t.Optional[t.Tuple[float, float]] = None,
                  regression_bins: t.Optional[t.List[t.Tuple[float, float]]] = None,
                  regression_reference: t.Optional[float] = None,
                  return_importances: bool = True,
                  use_graph_attributes: bool = False,
                  **kwargs):
         """
         Args:
@@ -117,14 +118,15 @@
         self.sparsity_factor = sparsity_factor
         self.concat_heads = concat_heads
         self.final_units = final_units
         self.final_dropout_rate = final_dropout_rate
         self.final_activation = final_activation
         self.final_pooling = final_pooling
         self.regression_limits = regression_limits
+        self.regression_weights = regression_weights
         self.regression_reference = regression_reference
         self.regression_bins = regression_bins
         self.return_importances = return_importances
         self.separate_explanation_step = separate_explanation_step
         self.use_graph_attributes = use_graph_attributes
 
         # ~ MAIN CONVOLUTIONAL / ATTENTION LAYERS
@@ -186,45 +188,52 @@
         self.bce_loss = ks.losses.BinaryCrossentropy()
         self.compiled_classification_loss = compile_utils.LossesContainer(bce)
 
         self.mse_loss = ks.losses.MeanSquaredError()
         self.mae_loss = ks.losses.MeanAbsoluteError()
         self.compiled_regression_loss = compile_utils.LossesContainer(mae)
 
+        # TODO: Clean up this mess
         # If regression_limits have been supplied, we interprete this as the intent to perform explanation
         # co-training for a regression dataset.
         # So the content of this if condition makes sure to perform the necessary pre-processing steps
         # for this case.
-        if self.regression_limits is not None:
-            # first of all we do some simple assertions to handle some common error cases
-            assert regression_reference is not None, ('You have to supply a "regression_reference" value for '
-                                                      'explanation co-training!')
+        if self.regression_reference is not None:
 
             # This is the first and simpler case for regression explanation co-training: In this case the
             # regression reference value is only a single value. In that case, there is only one target
             # value that is supposed to be regressed. The alternative would be that it is a list in which
             # case it would have to have as many elements as target values to be predicted.
             # However in this case we convert it into a list as well to be able to treat everything from
             # this point on as the multi-value case guaranteed.
             if isinstance(regression_reference, (int, float)):
                 self.regression_reference = [regression_reference]
 
             num_references = len(self.regression_reference)
-            num_limits = len(self.regression_limits)
+
+            if self.regression_weights is not None:
+                num_values = len(self.regression_weights)
+            elif self.regression_limits is not None:
+                num_values = len(self.regression_limits)
+            else:
+                raise AssertionError(f'You have supplied a non-null value for regression_reference: '
+                                     f'{self.regression_reference}. That means you need to either supply '
+                                     f'a valid value for regression_limits or regression_weights as well')
+
             assert num_references * 2 == importance_channels, (
                 f'for explanation co-training, the number of regression_references (currently {num_references}) has '
                 f'to be exactly half the number of importance channels (currently {importance_channels})!'
             )
             assert num_references == final_units[-1], (
                 f'For explanation co-training, the number of regression_references (currently {num_references}) has '
                 f'to be exactly the same as the final unit count in the MLP tail end (currently {final_units[-1]})'
             )
-            assert num_references == num_limits, (
+            assert num_references == num_values, (
                 f'For explanation co-training, the number of regression_references (currently {num_references}) has '
-                f'to be exactly the same as the number of regression_limits intervals (currently {num_limits})'
+                f'to be exactly the same as the number of regression_limits intervals (currently {num_values})'
             )
 
     def get_config(self):
         config = super(Megan, self).get_config()
         config.update({
             "units": self.units,
             "activation": self.activation,
@@ -240,22 +249,32 @@
             "sparsity_factor": self.sparsity_factor,
             "concat_heads": self.concat_heads,
             "final_units": self.final_units,
             "final_dropout_rate": self.final_dropout_rate,
             "final_activation": self.final_activation,
             "final_pooling": self.final_pooling,
             "regression_limits": self.regression_limits,
+            "regression_weights": self.regression_weights,
             "regression_reference": self.regression_reference,
-            "return_importances": self.return_importances
+            "return_importances": self.return_importances,
+            "use_graph_attributes": self.use_graph_attributes,
         })
 
         return config
+
+    # ~ Properties
+
     @property
     def doing_regression(self) -> bool:
-        return self.regression_limits is not None
+        return (self.regression_limits is not None) or (self.regression_weights is not None)
+
+    def doing_regression_weights(self) -> bool:
+        return self.regression_weights is not None
+
+    # ~ Forward Pass Implementation
 
     def call(self,
              inputs,
              training: bool = False,
              return_importances: bool = False,
              node_importances_mask: t.Optional[tf.RaggedTensor] = None,
              **kwargs):
@@ -387,21 +406,31 @@
         else:
             return out
 
     def regression_augmentation(self,
                                 out_true):
         samples = []
         masks = []
-        for i, (regression_reference, regression_limits) in enumerate(zip(self.regression_reference,
-                                                                          self.regression_limits)):
 
-            regression_width = abs(regression_limits[1] - regression_limits[0])
+        for i, regression_reference in enumerate(self.regression_reference):
             values = tf.expand_dims(out_true[:, i], axis=-1)
             center_distances = tf.abs(values - regression_reference)
-            center_distances = (center_distances * self.importance_multiplier) / (0.5 * regression_width)
+
+            if self.doing_regression_weights:
+                regression_weights = self.regression_weights[i]
+                center_distances = tf.where(
+                    values < regression_reference,
+                    center_distances * (self.importance_multiplier * regression_weights[0]),
+                    center_distances * (self.importance_multiplier * regression_weights[1]),
+                )
+
+            else:
+                regression_limits = self.regression_limits[i]
+                regression_width = abs(regression_limits[1] - regression_limits[0])
+                center_distances = (center_distances * self.importance_multiplier) / (0.5 * regression_width)
 
             # So we need two things: a "samples" tensor and a "mask" tensor. We are going to use the samples
             # tensor as the actual ground truth which acts as the regression target during the explanation
             # train step. The binary values of the mask will determine at which positions a loss should
             # actually be calculated for both of the channels
 
             # The "lower" part is all the samples which have a target value below the reference value.
```

### Comparing `graph_attention_student-0.7.1/graph_attention_student/templates/article.tex.j2` & `graph_attention_student-0.7.2/graph_attention_student/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/training.py` & `graph_attention_student-0.7.2/graph_attention_student/training.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/typing.py` & `graph_attention_student-0.7.2/graph_attention_student/typing.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/util.py` & `graph_attention_student-0.7.2/graph_attention_student/util.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/graph_attention_student/visualization.py` & `graph_attention_student-0.7.2/graph_attention_student/visualization.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.1/pyproject.toml` & `graph_attention_student-0.7.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "graph_attention_student"
-version = "0.7.1"
+version = "0.7.2"
 description = "MEGAN: Multi Explanation Graph Attention Network"
 license = "MIT"
 authors = ["xxx <jonseb1998@gmail.com>"]
 maintainers = ["xxx <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural network", "attention", "kgcnn"]
 packages = [
```

### Comparing `graph_attention_student-0.7.1/setup.py` & `graph_attention_student-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 entry_points = \
 {'console_scripts': ['graph_attention_student = '
                      'graph_attention_student.cli:cli']}
 
 setup_kwargs = {
     'name': 'graph-attention-student',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': 'MEGAN: Multi Explanation Graph Attention Network',
     'long_description': '|made-with-python| |made-with-kgcnn| |python-version| |os-linux|\n\n.. |os-linux| image:: https://img.shields.io/badge/os-linux-orange.svg\n   :target: https://www.python.org/\n\n.. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg\n   :target: https://www.python.org/\n\n.. |made-with-kgcnn| image:: https://img.shields.io/badge/Made%20with-KGCNN-blue.svg\n   :target: https://github.com/aimat-lab/gcnn_keras\n\n.. |made-with-python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg\n   :target: https://www.python.org/\n\n.. image:: architecture.png\n    :width: 800\n    :alt: Architecture Overview\n\n================================================\nMEGAN: Multi Explanation Graph Attention Student\n================================================\n\nExplainable artificial intelligence (XAI) methods are expected to improve trust during human-AI interactions,\nprovide tools for model analysis and extend human understanding of complex problems. Attention-based models\nare an important subclass of XAI methods, partly due to their full differentiability and the potential to\nimprove explanations by means of explanation-supervised training. We propose the novel multi-explanation\ngraph attention network (MEGAN). Our graph regression and classification model features multiple explanation\nchannels, which can be chosen independently of the task specifications. We first validate our model on a\nsynthetic graph regression dataset, where our model produces single-channel explanations with quality\nsimilar to GNNExplainer. Furthermore, we demonstrate the advantages of multi-channel explanations on one\nsynthetic and two real-world datasets: The prediction of water solubility of molecular graphs and\nsentiment classification of movie reviews. We find that our model produces explanations consistent\nwith human intuition, opening the way to learning from our model in less well-understood tasks.\n\nInstallation\n============\n\nMain Installation\n-----------------\n\nClone the repository from github:\n\n.. code-block:: shell\n\n    git clone https://github.com/awa59kst120df/graph_attention_student.git\n\nThen in the main folder run a ``pip install``:\n\n.. code-block:: shell\n\n    cd graph_attention_student\n    pip3 install -e .\n\nAfterwards, you can check the install by invoking the CLI:\n\n.. code-block:: shell\n\n    python3 -m graph_attention_student.cli --version\n    python3 -m graph_attention_student.cli --help\n\nUsage\n=====\n\nComputational Experiments\n-------------------------\n\nIt is possible to list, show and execute all the computational experiments using a command line interface\nCLI.\n\n    *NOTE* Most of the experiments have a long runtime, ranging from ~2hrs to ~2days.\n    Furthermore, all of the experiments which do model training are currently configured to run on a GPU\n    and might crash if the GPU can either not be detected or does not have enough VRAM. This setting can\n    be changed in the corresponding experiment scripts\n\nAll the available experiments can be listed like this:\n\n.. code-block:: shell\n\n    python3 -m graph_attention_student.cli list\n\nThe details for a specific experiment can be viewed like this:\n\n.. code-block:: shell\n\n    python3 -m graph_attention_student.cli info [experiment_name]\n\nA new run of an experiment can be started like this. However, be aware that this might take some time.\n\n.. code-block::\n\n    python3 -m graph_attention_student.cli run [experiment_name]\n\nEach experiment will create a new archive folder, which will contain all the artifacts (such as visual\nexamples and the raw data) created during the runtime. The location of this archive folder can be found\nfrom the output generated by the experiment execution.\n\nArchived Experiments\n--------------------\n\nTo view the detailed data which was used in the making of the paper, go to\n``graph_attention_student/experiments``. The subfolders in that folder contain the archived experiments.\nThese contain extensive examples for each repetition of the various experiments as well as all of the raw\ndata collected during the execution of the experiments.\n\nMEGAN in code\n-------------\n\nThe MEGAN model is implemented as the ``MultiAttentionStudent`` class, which implements ``keras.Model``.\nThe implementation is based on the `kgcnn`_ library for graph convolutional networks for keras. For further\ninformation on loading graph structured data with `kgcnn`_ visit:\nhttps://github.com/aimat-lab/gcnn_keras\n\nThis is a simple example of how to use the model in the regression case:\n\n.. code-block:: python\n\n    import tensorflow as tf\n    import tensorflow.keras as ks\n    from graph_attention_student.training import NoLoss\n    from graph_attention_student.models import Megan\n\n    model = Megan(\n        # These lists define the number of layers and the number of hidden units in each layer for the\n        # various parts of the architecture\n        units=[9, 9, 9],  # The main convolutional layers\n        importance_units=[],  # The MLP that creates the node importances\n        final_units=[5, 1],  # The final MLP for graph embeddings\n        # Example for a regression problem. We need the prior knowledge about what range the values of the\n        # dataset will be expected to fall into...\n        regression_limits=(-3, +3),\n        # ... as well as a reference value.\n        regression_reference=0,\n        # This controls the weight of the explanation-only train step (gamma)\n        importance_factor=1.0,\n        importance_multiplier=5,\n        # This is the weight of the sparsity regularization\n        sparsity_factor=0.1,\n    )\n\n    # The model output is actually a three tuple: (prediction, node_importances, edge_importances).\n    # This allows the importances to be trained in a supervised fashion. If we don\'t want that,\n    # we can simply supply the NoLoss function instead.\n    model.compile(\n        loss=[ks.losses.MeanSquaredError(), NoLoss(), NoLoss()],\n        loss_weights=[1, 1, 1],\n        optimizer=ks.optimizers.Adam(0.001)\n    )\n\n    # model.fit() ...\n\n\n.. _kgcnn: https://github.com/aimat-lab/gcnn_keras\n.. _examples/solubility_regression.py: https://github.com/aimat-lab/graph_attention_student/tree/master/graph_attention_student/examples/solubility_regression.py\n.. _`GATv2`: https://github.com/tech-srl/how_attentive_are_gats\n\n---\n\nExamples\n========\n\nThe following examples show some of the *cherry picked* examples that show the explanatory capabilities of\nthe model.\n\nRB-Motifs Dataset\n-----------------\n\nThis is a synthetic dataset, which basically consists of randomly generated graphs with nodes of different\ncolors. Some of the graphs contain special sub-graph motifs, which are either blue-heavy or red-heavy\nstructures. The blue-heavy sub-graphs contribute a certain negative value to the overall value of the graph,\nwhile red-heavy structures contain a certain positive value.\n\nThis way, every graph has a certain value associated with it, which is between -3 and 3. The network was\ntrained to predict this value for each graph.\n\n.. image:: rb_motifs_example.png\n    :width: 800\n    :alt: Rb-Motifs Example\n\nThe examples shows from left to right: (1) The ground truth explanations, (2) a baseline MEGAN model trained\nonly on the prediction task, (3) explanation-supervised MEGAN model and (4) GNNExplainer explanations for a\nbasic GCN network. While the baseline MEGAN and GNNExplainer focus only on one of the ground truth motifs,\nthe explanation-supervised MEGAN model correctly finds both.\n\nWater Solubility Dataset\n------------------------\n\nThis is the `AqSolDB`_ dataset, which consists of ~10000 molecules and measured values for the solubility in\nwater (logS value).\n\nThe network was trained to predict the solubility value for each molecule.\n\n.. image:: solubility_example.png\n    :width: 800\n    :alt: Solubility Example.png\n\n.. _`AqSolDB`: https://www.nature.com/articles/s41597-019-0151-1\n\nMovie Reviews\n-------------\n\nOriginally the *MovieReviews* dataset is a natural language processing dataset from the `ERASER`_ benchmark.\nThe task is to classify the sentiment of ~2000 movie reviews collected from the IMDB database into the\nclasses "positive" and "negative". This dataset was converted into a graph dataset by considering all words\nas nodes of a graph and then connecting adjacent words by undirected edges with a sliding window of size 2.\nWords were converted into numeric feature vectors by using a pre-trained `GLOVE`_ model.\n\nExample for a positive review:\n\n.. image:: movie_reviews_pos.png\n    :width: 800\n    :alt: Positive Movie Review\n\nExample for a negative review:\n\n.. image:: movie_reviews_neg.png\n    :width: 800\n    :alt: Negative Movie Review\n\nExamples show the explanation channel for the "negative" class left and the "positive" class right.\nSentences with negative / positive adjectives are appropriately attributed to the corresponding channels.\n\n.. _`ERASER`: https://www.eraserbenchmark.com/\n.. _`GLOVE`: https://nlp.stanford.edu/projects/glove/\n\n',
     'author': 'xxx',
     'author_email': 'jonseb1998@gmail.com',
     'maintainer': 'xxx',
     'maintainer_email': 'jonseb1998@gmail.com',
     'url': 'None',
```

### Comparing `graph_attention_student-0.7.1/PKG-INFO` & `graph_attention_student-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-attention-student
-Version: 0.7.1
+Version: 0.7.2
 Summary: MEGAN: Multi Explanation Graph Attention Network
 License: MIT
 Keywords: graph neural network,attention,kgcnn
 Author: xxx
 Author-email: jonseb1998@gmail.com
 Maintainer: xxx
 Maintainer-email: jonseb1998@gmail.com
```


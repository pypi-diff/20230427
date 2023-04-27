# Comparing `tmp/troubleshooter-1.0.6.tar.gz` & `tmp/troubleshooter-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/troubleshooter-1.0.6.tar", last modified: Sat Jan 28 12:54:46 2023, max compression
+gzip compressed data, was "dist/troubleshooter-1.0.7.tar", last modified: Thu Apr 27 11:50:31 2023, max compression
```

## Comparing `troubleshooter-1.0.6.tar` & `troubleshooter-1.0.7.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/
--rwxrwxrwx   0 root         (0) root         (0)    11357 2022-12-08 02:13:00.000000 troubleshooter-1.0.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      334 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    22712 2023-01-05 00:42:27.000000 troubleshooter-1.0.6/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3833 2023-01-28 12:52:40.000000 troubleshooter-1.0.6/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/tests/
--rwxrwxrwx   0 root         (0) root         (0)      668 2022-12-08 02:13:06.000000 troubleshooter-1.0.6/tests/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/tests/diff_handler/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-15 13:01:34.000000 troubleshooter-1.0.6/tests/diff_handler/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      454 2022-12-15 08:42:12.000000 troubleshooter-1.0.6/tests/diff_handler/test_compare.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/tests/proposer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/tests/proposer/1_9/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/1_9/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3088 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/1_9/test_compile.py
--rwxrwxrwx   0 root         (0) root         (0)      482 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/1_9/test_ops.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/tests/proposer/master/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/master/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5112 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/master/test_ascend_vm.py
--rwxrwxrwx   0 root         (0) root         (0)    12255 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/master/test_compile.py
--rwxrwxrwx   0 root         (0) root         (0)     9667 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/master/test_dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     3163 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/master/test_me_front.py
--rwxrwxrwx   0 root         (0) root         (0)     4310 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/master/test_ops.py
--rwxrwxrwx   0 root         (0) root         (0)     2572 2022-12-08 02:13:04.000000 troubleshooter-1.0.6/tests/proposer/master/test_st_output.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/tests/tracker/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-08 02:13:05.000000 troubleshooter-1.0.6/tests/tracker/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10544 2022-12-08 02:13:05.000000 troubleshooter-1.0.6/tests/tracker/test_tracking.py
--rwxrwxrwx   0 root         (0) root         (0)     1435 2022-12-08 02:13:06.000000 troubleshooter-1.0.6/tests/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/troubleshooter/
--rwxrwxrwx   0 root         (0) root         (0)     1415 2023-01-20 07:49:08.000000 troubleshooter-1.0.6/troubleshooter/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/troubleshooter/common/
--rwxrwxrwx   0 root         (0) root         (0)      668 2022-12-08 02:13:06.000000 troubleshooter-1.0.6/troubleshooter/common/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    12251 2023-01-28 11:45:28.000000 troubleshooter-1.0.6/troubleshooter/common/format_msg.py
--rwxrwxrwx   0 root         (0) root         (0)     1543 2023-01-20 09:55:57.000000 troubleshooter-1.0.6/troubleshooter/common/ms_callback.py
--rwxrwxrwx   0 root         (0) root         (0)     3880 2023-01-20 09:55:39.000000 troubleshooter-1.0.6/troubleshooter/common/ms_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     4083 2023-01-28 01:51:13.000000 troubleshooter-1.0.6/troubleshooter/common/util.py
--rwxrwxrwx   0 root         (0) root         (0)     3255 2023-01-19 01:16:30.000000 troubleshooter-1.0.6/troubleshooter/log.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/troubleshooter/migrator/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-15 06:34:30.000000 troubleshooter-1.0.6/troubleshooter/migrator/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    12191 2023-01-28 12:46:44.000000 troubleshooter-1.0.6/troubleshooter/migrator/diff_handler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/troubleshooter/migrator/mapping_relation/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-15 06:34:30.000000 troubleshooter-1.0.6/troubleshooter/migrator/mapping_relation/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      819 2023-01-28 10:38:58.000000 troubleshooter-1.0.6/troubleshooter/migrator/mapping_relation/weight_adapter.py
--rwxrwxrwx   0 root         (0) root         (0)     1483 2023-01-28 11:03:41.000000 troubleshooter-1.0.6/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/troubleshooter/proposer/
--rwxrwxrwx   0 root         (0) root         (0)      793 2022-12-08 02:13:06.000000 troubleshooter-1.0.6/troubleshooter/proposer/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/
--rwxrwxrwx   0 root         (0) root         (0)     1834 2022-12-08 02:13:06.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3238 2022-12-08 02:13:06.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/base_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1572 2022-12-08 02:13:06.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/compiler_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1586 2022-12-08 02:13:06.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/compiler_scene_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1517 2022-12-08 02:13:06.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/dataset_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1474 2022-12-08 02:13:06.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/dataset_scene_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1239 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/default_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1678 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/front_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1513 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/operators_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1606 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/operators_scene_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     2624 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/allproposers/vm_proposer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/
--rwxrwxrwx   0 root         (0) root         (0)      669 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1787 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/common_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    31271 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    16904 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/dataset_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)     6740 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/front_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    28881 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/operators_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    13146 2022-12-23 01:48:02.000000 troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/vm_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)     3425 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/proposal_action.py
--rwxrwxrwx   0 root         (0) root         (0)     2233 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/proposer/proposer_factory.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/troubleshooter/tracker/
--rwxrwxrwx   0 root         (0) root         (0)      770 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/tracker/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6795 2022-12-08 02:13:07.000000 troubleshooter-1.0.6/troubleshooter/tracker/tracker.py
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/troubleshooter/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 12:54:43.000000 troubleshooter-1.0.6/troubleshooter.egg-info/
--r-xr-xr-x   0 root         (0) root         (0)      334 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/troubleshooter.egg-info/PKG-INFO
--r-xr-xr-x   0 root         (0) root         (0)     2473 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/troubleshooter.egg-info/SOURCES.txt
--r-xr-xr-x   0 root         (0) root         (0)        1 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/troubleshooter.egg-info/dependency_links.txt
--r-xr-xr-x   0 root         (0) root         (0)       36 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/troubleshooter.egg-info/requires.txt
--r-xr-xr-x   0 root         (0) root         (0)       21 2023-01-28 12:54:42.000000 troubleshooter-1.0.6/troubleshooter.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/
+-rwxrwxrwx   0 root         (0) root         (0)    11357 2023-04-19 06:32:30.000000 troubleshooter-1.0.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      472 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    24285 2023-04-25 02:43:53.000000 troubleshooter-1.0.7/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3997 2023-04-27 11:38:56.000000 troubleshooter-1.0.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      668 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/tests/diff_handler/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/diff_handler/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      440 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/diff_handler/test_compare.py
+-rwxrwxrwx   0 root         (0) root         (0)    12415 2023-04-27 09:26:12.000000 troubleshooter-1.0.7/tests/diff_handler/test_migrator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/tests/proposer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/tests/proposer/1_9/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/1_9/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3537 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/1_9/test_compile.py
+-rwxrwxrwx   0 root         (0) root         (0)      482 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/1_9/test_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/tests/proposer/master/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7485 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_ascend_vm.py
+-rwxrwxrwx   0 root         (0) root         (0)    14663 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_compile.py
+-rwxrwxrwx   0 root         (0) root         (0)     9667 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     3163 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_me_front.py
+-rwxrwxrwx   0 root         (0) root         (0)     4310 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)     2572 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_st_output.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/tests/tracker/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/tracker/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10544 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/tracker/test_tracking.py
+-rwxrwxrwx   0 root         (0) root         (0)     1395 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/
+-rwxrwxrwx   0 root         (0) root         (0)     1415 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/common/
+-rwxrwxrwx   0 root         (0) root         (0)      668 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/common/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11931 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/common/format_msg.py
+-rwxrwxrwx   0 root         (0) root         (0)     1511 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/common/ms_callback.py
+-rwxrwxrwx   0 root         (0) root         (0)     3785 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/common/ms_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     3958 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/common/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     3255 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/log.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/migrator/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/migrator/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14445 2023-04-27 03:46:52.000000 troubleshooter-1.0.7/troubleshooter/migrator/diff_handler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      801 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/weight_adapter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1457 2023-04-20 12:28:36.000000 troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/proposer/
+-rwxrwxrwx   0 root         (0) root         (0)      793 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/
+-rwxrwxrwx   0 root         (0) root         (0)     1834 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3238 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/base_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1529 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/compiler_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1544 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/compiler_scene_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/dataset_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1434 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/dataset_scene_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1239 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/default_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1678 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/front_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1472 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/operators_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1566 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/operators_scene_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     2561 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/vm_proposer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/
+-rwxrwxrwx   0 root         (0) root         (0)      669 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1747 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/common_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    36584 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    16638 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/dataset_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)     6740 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/front_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    28384 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/operators_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    19783 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/vm_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)     3425 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/proposal_action.py
+-rwxrwxrwx   0 root         (0) root         (0)     2233 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/proposer_factory.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/tracker/
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/tracker/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6630 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/tracker/tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter.egg-info/
+-r-xr-xr-x   0 root         (0) root         (0)      472 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter.egg-info/PKG-INFO
+-r-xr-xr-x   0 root         (0) root         (0)     2509 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter.egg-info/SOURCES.txt
+-r-xr-xr-x   0 root         (0) root         (0)        1 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter.egg-info/dependency_links.txt
+-r-xr-xr-x   0 root         (0) root         (0)       36 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter.egg-info/requires.txt
+-r-xr-xr-x   0 root         (0) root         (0)       21 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter.egg-info/top_level.txt
```

### Comparing `troubleshooter-1.0.6/LICENSE` & `troubleshooter-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/setup.py` & `troubleshooter-1.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import shutil
 import subprocess
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.egg_info import egg_info
 from setuptools.command.build_py import build_py
 
-version = '1.0.6'
+version = '1.0.7'
 cur_dir = os.path.dirname(os.path.realpath(__file__))
 pkg_dir = os.path.join(cur_dir, 'build')
 
 
 def clean():
     """clean"""
     def readonly_handler(func, path, execinfo):
@@ -109,17 +109,21 @@
         troubleshooter_dir = os.path.join(pkg_dir, 'lib', 'troubleshooter')
         update_permissions(troubleshooter_dir)
 
 
 setup(
     name='troubleshooter',
     version=version,
-    author='Tiger Miao and collaborators.',
-    author_email='asktiger@yeah.net',
-    url='https://gitee.com/askmiao/troubleshooter',
+    author='The MindSpore Authors',
+    author_email='contact@mindspore.cn',
+    url='https://www.mindspore.cn/',
+    project_urls={
+        'Sources': 'https://gitee.com/mindspore/toolkits/tree/master/troubleshooter',
+        'Issue Tracker': 'https://gitee.com/mindspore/toolkits/issues',
+    },
     description=get_description(),
     license='Apache 2.0',
     packages=find_packages(),
     include_package_data=True,
     cmdclass={
         'egg_info': EggInfo,
         'build_py': BuildPy,
```

### Comparing `troubleshooter-1.0.6/tests/__init__.py` & `troubleshooter-1.0.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/tests/proposer/1_9/test_compile.py` & `troubleshooter-1.0.7/tests/proposer/1_9/test_compile.py`

 * *Files 10% similar despite different names*

```diff
@@ -109,7 +109,26 @@
         net = Net_MoreInput()
         out = net(1, 2)
         print(out)
 
     delete_file("/tmp/")
     more_input_case()
     assert file_and_key_match("/tmp/", "compiler_id_4")
+
+
+def test_compiler_staticmap_3():
+    x = (Tensor(4), Tensor(5), Tensor(6))
+    # 'jit' need that mindspore version 2.0.0-alpha or later
+
+    @mindspore.ms_function
+    def index_get(y):
+        return x[y]
+
+    @ts.proposal(write_file_path="/tmp/")
+    def staticmap_case():
+        y = Tensor(2)
+        out = index_get(y)
+        print(out)
+
+    delete_file("/tmp/")
+    staticmap_case()
+    assert file_and_key_match("/tmp/", "compiler_id_22")
```

### Comparing `troubleshooter-1.0.6/tests/proposer/master/test_ascend_vm.py` & `troubleshooter-1.0.7/tests/proposer/master/test_ascend_vm.py`

 * *Files 22% similar despite different names*

```diff
@@ -151,7 +151,79 @@
     @ts.proposal(write_file_path="/tmp/")
     def main():
         raise ValueError("Single op compile failed")
 
     delete_file("/tmp/")
     main()
     assert file_and_key_match("/tmp/", "vm_id_9")
+
+
+def test_version_not_match():
+    @ts.proposal(write_file_path="/tmp/")
+    def main():
+        raise ValueError("""errNo[0x0000000005010001]
+                            hcom_ops_kernel_info_store.cc""")
+
+    delete_file("/tmp/")
+    main()
+    assert file_and_key_match("/tmp/", "vm_id_12")
+
+
+def test_broadcast_op_distribute_failed():
+    @ts.proposal(write_file_path="/tmp/")
+    def main():
+        raise ValueError("mindspore\ccsrc\plugin\device\ascend\hal\device\ge_runtime\task\hccl_task.cc]"
+                         " davinci_model: load task fail, return ret: 1343225860")
+
+    delete_file("/tmp/")
+    main()
+    assert file_and_key_match("/tmp/", "vm_id_13")
+
+
+def test_stream_exceeds():
+    @ts.proposal(write_file_path="/tmp/")
+    def main():
+        raise ValueError("AssignAllNodesStream] Total stream number xxx exceeds the limit of 1024, "
+                         "secrch details information in mindspore's FAQ.")
+
+    delete_file("/tmp/")
+    main()
+    assert file_and_key_match("/tmp/", "vm_id_14")
+
+
+def test_response_is_empty():
+    @ts.proposal(write_file_path="/tmp/")
+    def main():
+        raise ValueError("""
+        Traceback (most recent call last):
+            ...
+        RuntimeError: mindspore/ccsrc/backend/common/session/kernel_build_client.h:107 Response] Response is empty
+        """)
+
+    delete_file("/tmp/")
+    main()
+    assert file_and_key_match("/tmp/", "vm_id_15")
+
+
+def test_memasycpy_failed():
+    # 'Key Log Information' is not in Traceback information
+    @ts.proposal(write_file_path="/tmp/")
+    def main():
+        raise ValueError("Memory async copy failed, device_id=0, stream_id=102, task_id=171, flip_num=0, "
+                         "copy_type=10, memcpy_type=0, copy_data_type=0, length=896[FUNC:GetError]"
+                         "[FILE:stream.cc][LINE:741]")
+
+    delete_file("/tmp/")
+    main()
+    assert file_and_key_match("/tmp/", "vm_id_16")
+
+
+def data_format_not_match():
+    @ts.proposal(write_file_path="/tmp/")
+    def main():
+        raise ValueError("[mindspore/ccsrc/backend/optimizer/ascend/format_type/check_consistency.cc:64] "
+                         "CheckFormatForConsistency] Found inconsistent format! input format 0: FracZ, "
+                         "selected input format: DefaultFormat")
+
+    delete_file("/tmp/")
+    main()
+    assert file_and_key_match("/tmp/", "vm_id_17  ")
```

### Comparing `troubleshooter-1.0.6/tests/proposer/master/test_compile.py` & `troubleshooter-1.0.7/tests/proposer/master/test_compile.py`

 * *Files 10% similar despite different names*

```diff
@@ -435,7 +435,98 @@
         net = Net_MoreInput()
         out = net(1, 2)
         print(out)
 
     delete_file("/tmp/")
     more_input_case()
     assert file_and_key_match("/tmp/", "compiler_id_5")
+
+
+def test_compiler_staticmap_1():
+    # 'jit_class' need that mindspore version 2.0.0-alpha or later
+    @mindspore.jit_class
+    class InnerNet:
+        def __init__(self, val):
+            self.number = val + 3
+
+    class Net(nn.Cell):
+        def __init__(self, val):
+            super(Net, self).__init__()
+            self.inner = InnerNet(val)
+
+        def construct(self, x):
+            net = InnerNet(x)
+            return net.number
+
+    @ts.proposal(write_file_path="/tmp/")
+    def staticmap_case():
+        mindspore.set_context(mode=mindspore.GRAPH_MODE)
+        x = mindspore.Tensor(2, dtype=mindspore.int32)
+        net = Net(x)
+        out = net(x)
+        print(out)
+
+    delete_file("/tmp/")
+    staticmap_case()
+    assert file_and_key_match("/tmp/", "compiler_id_20")
+
+
+def test_compiler_staticmap_2():
+    class Net(nn.Cell):
+        def __init__(self, mode):
+            super(Net, self).__init__()
+            self.mode = mode
+
+        def construct(self):
+            if self.mode == "print_var":
+                var = (1, 2, 3)
+            for i in var:
+                print(1)
+            return True
+
+    @ts.proposal(write_file_path="/tmp/")
+    def staticmap_case():
+        mindspore.set_context(mode=mindspore.GRAPH_MODE)
+        net = Net("not_print_var")
+        out = net()
+        print(out)
+
+    delete_file("/tmp/")
+    staticmap_case()
+    assert file_and_key_match("/tmp/", "compiler_id_21")
+
+
+def test_compiler_staticmap_3():
+    x = (Tensor(4), Tensor(5), Tensor(6))
+    # 'jit' need that mindspore version 2.0.0-alpha or later
+
+    @mindspore.common.jit
+    def index_get(y):
+        return x[y]
+
+    @ts.proposal(write_file_path="/tmp/")
+    def staticmap_case():
+        y = Tensor(2)
+        out = index_get(y)
+        print(out)
+
+    delete_file("/tmp/")
+    staticmap_case()
+    assert file_and_key_match("/tmp/", "compiler_id_22")
+
+
+def test_compiler_staticmap_4():
+    x = (Tensor(4), Tensor(5), Tensor(6))
+
+    class IndexGet(nn.Cell):
+        def construct(self, x, y):
+            return x[y]
+
+    @ts.proposal(write_file_path="/tmp/")
+    def staticmap_case():
+        context.set_context(mode=context.GRAPH_MODE, save_graphs=True, save_graphs_path="../ir/tupleindextensor/1")
+        y = Tensor(2, mindspore.int32)
+        print(IndexGet()(x, y))
+
+    delete_file("/tmp/")
+    staticmap_case()
+    assert file_and_key_match("/tmp/", "compiler_id_23")
```

### Comparing `troubleshooter-1.0.6/tests/proposer/master/test_dataset.py` & `troubleshooter-1.0.7/tests/proposer/master/test_dataset.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/tests/proposer/master/test_me_front.py` & `troubleshooter-1.0.7/tests/proposer/master/test_me_front.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/tests/proposer/master/test_ops.py` & `troubleshooter-1.0.7/tests/proposer/master/test_ops.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/tests/proposer/master/test_st_output.py` & `troubleshooter-1.0.7/tests/proposer/master/test_st_output.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/tests/tracker/test_tracking.py` & `troubleshooter-1.0.7/tests/tracker/test_tracking.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/tests/util.py` & `troubleshooter-1.0.7/tests/util.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""util functions"""
-import re
-import os
-import stat
-from troubleshooter.common.util import validate_and_normalize_path
-
-
-def delete_file(path, file_name="mindspore_failure_analysis_report.log"):
-    path = validate_and_normalize_path(path)
-    file = os.path.join(path, file_name)
-    if os.path.exists(file):
-        # 删除文件，可使用以下两种方法。
-        os.remove(file)
-
-
-def file_and_key_match(path, key, file_name="mindspore_failure_analysis_report.log"):
-    path = validate_and_normalize_path(path)
-    file = os.path.join(path, file_name)
-    with open(file, "r") as f:
-        result = f.read()
-    if result.find(key) == -1:
-        result = False
-    else:
-        result = True
-    return result
-
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""util functions"""
+import re
+import os
+import stat
+from troubleshooter.common.util import validate_and_normalize_path
+
+
+def delete_file(path, file_name="mindspore_failure_analysis_report.log"):
+    path = validate_and_normalize_path(path)
+    file = os.path.join(path, file_name)
+    if os.path.exists(file):
+        # 删除文件，可使用以下两种方法。
+        os.remove(file)
+
+
+def file_and_key_match(path, key, file_name="mindspore_failure_analysis_report.log"):
+    path = validate_and_normalize_path(path)
+    file = os.path.join(path, file_name)
+    with open(file, "r") as f:
+        result = f.read()
+    if result.find(key) == -1:
+        result = False
+    else:
+        result = True
+    return result
+
```

### Comparing `troubleshooter-1.0.6/troubleshooter/__init__.py` & `troubleshooter-1.0.7/troubleshooter/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/common/__init__.py` & `troubleshooter-1.0.7/troubleshooter/common/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/common/format_msg.py` & `troubleshooter-1.0.7/troubleshooter/common/format_msg.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,320 +1,320 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""format output"""
-
-import os
-import re
-from textwrap import fill
-import traceback
-from prettytable import PrettyTable
-from troubleshooter.common.util import print_line
-from troubleshooter.common.ms_utils import get_errmsg_dict
-
-TABLE_WIDTH = 50
-DELIMITER_LEN = 100
-
-# GLog level and level name
-_item_to_cn = {
-    'item': '项目',
-    'desc': '描述',
-    'ms_version': '版本信息:',
-    'ms_mode': '执行模式:',
-    'ms_device': '配置设备:',  # GPU, CPU, Ascend
-    'ms_status': '执行阶段:',
-    'code_line': '代码行:',
-    'cause': '可能原因:',
-    'err_code': '示例错误代码：',
-    'fixed_code': '示例正确代码：',
-    'proposal': '处理建议:',
-    'case': '相关案例:',
-    'sink_mode': '下沉模式:',  # 图下沉，数据下沉，非下沉
-    'case_id': 'ID:',
-}
-
-
-def _add_row(x, item, message, width=TABLE_WIDTH, break_long_words=False, break_on_hyphens=False):
-    if message is None:
-        return
-    item_cn = _item_to_cn.get(item)
-    format_message = _format_str_length(message) if os.linesep in message else message
-    x.add_row([item_cn, fill(format_message, width=width, break_long_words=break_long_words,
-                             break_on_hyphens=break_on_hyphens)])
-
-
-def print_weight_compare_result(result_list, print_type=1):
-    x = PrettyTable()
-    x.title = 'The list of comparison results'
-    x.field_names = ["Parameter name of input ckpt", "Parameter name of converted ckpt", "Whether shape are equal", "Parameter shape of input ckpt", "Parameter shape of converted ckpt"]
-    for result in result_list:
-        if print_type == 1:
-            x.add_row([result[0],result[1],result[2],result[3],result[4]])
-        elif result[2] is not True:
-            x.add_row([result[0], result[1], result[2], result[3], result[4]])
-    print(x.get_string())
-
-
-def print_convert_result(result_list):
-    x = PrettyTable()
-    x.title = 'The list of conversion result'
-    x.field_names = ["Parameter name of pth", "Parameter name of converted ckpt", "Whether the name is converted",
-                     "Whether the weight value is converted","Parameter shape of pth","Parameter shape of ckpt"]
-    for result in result_list:
-        x.add_row([result[0],result[1],result[2],result[3],result[4],result[5]])
-    print(x.get_string())
-
-def print_diff_result(result_list):
-    x = PrettyTable()
-    x.title = 'The list of comparison results'
-    x.field_names = ["orig array name", "target array name", "Results of comparison", "(mean,max,min)"]
-    for result in result_list:
-        x.add_row([result[0],result[1],result[2],result[3]])
-    print(x.get_string())
-
-def print_result(expert_experience, write_file_path):
-    """
-    print MindSpore FAR
-    """
-    x = PrettyTable()
-    item_desc = _item_to_cn
-    x.title = 'MindSpore FAR(Failure Analysis Report)'
-    x.field_names = [item_desc.get("item"), item_desc.get("desc")]
-    x.align[item_desc.get("desc")] = 'l'
-    mindspore_version = expert_experience.get("mindspore_version")
-    mindspore_mode = expert_experience.get("mindspore_mode")
-    mindspore_device = expert_experience.get("Device Type")
-    x.add_row([item_desc.get("ms_version"), fill(mindspore_version, width=TABLE_WIDTH)])
-    x.add_row([item_desc.get("ms_mode"), fill(mindspore_mode, width=TABLE_WIDTH)])
-    if mindspore_device:
-        x.add_row([item_desc.get("ms_device"), fill(mindspore_device, width=TABLE_WIDTH)])
-    ms_status = expert_experience.get("ms_status")
-    code_line = expert_experience.get("code_line")
-    sink_mode = expert_experience.get("Sink Mode")
-    if ms_status:
-        x.add_row([item_desc.get("ms_status"), fill(ms_status, width=TABLE_WIDTH)])
-    if code_line:
-        x.add_row([item_desc.get("code_line"), fill(code_line, width=TABLE_WIDTH)])
-    if sink_mode:
-        x.add_row([item_desc.get("sink_mode"), fill(sink_mode, width=TABLE_WIDTH)])
-
-    # 可能原因
-    fault_cause = expert_experience.get('Fault Cause')
-    _add_row(x, "cause", fault_cause)
-
-    # 错误代码
-    err_code = expert_experience.get("Error Case")
-    err_code = _format_code_str(err_code)
-
-    _add_row(x, "err_code", err_code)
-    # 处理建议
-    suggestion = expert_experience.get("Modification Suggestion")
-    _add_row(x, "proposal", suggestion)
-    # 正确代码
-    fixed_code = expert_experience.get("Fixed Case")
-    fixed_code = _format_code_str(fixed_code)
-    _add_row(x, "fixed_code", fixed_code)
-    # 相关案例
-    fault_case = expert_experience.get("Fault Case")
-    fault_case = _format_case_str(fault_case, mindspore_version)
-    _add_row(x, "case", fault_case)
-    if write_file_path:
-        case_id = expert_experience.get("ID")
-        _add_row(x, "case_id", case_id)
-        file = os.path.join(write_file_path, "mindspore_failure_analysis_report.log")
-        with open(file, "w") as f:
-            f.write(x.get_string() + os.linesep)
-    print(x.get_string())
-
-
-def _print_msg(title, msg=None, print_msg=True):
-    if msg:
-        print_line("-", DELIMITER_LEN)
-        print("-  " + title)
-        print_line("-", DELIMITER_LEN)
-        if print_msg:
-            print(msg.rstrip(os.linesep) + os.linesep)
-
-
-def _print_stack(exc_traceback_obj):
-    if exc_traceback_obj:
-        _print_msg("Python Traceback (most recent call last):", "NULL", False)
-        traceback.print_tb(exc_traceback_obj)
-        print("")
-
-
-def _format_str_length(string):
-    str_list = string.split(os.linesep)
-    result_str = ""
-    for str_tmp in str_list:
-        result_str = result_str + str_tmp.ljust(TABLE_WIDTH) + os.linesep
-    return result_str
-
-
-def _format_code_str(content, width=50):
-    """
-    format code str
-    """
-    if content:
-        lines = content.split("\n")
-        result = '+'.ljust(width - 2, '-') + '+' + os.linesep
-        line = lines[1]
-        if line == '':
-            return content
-        j = 0
-        while line[j] == ' ':
-            j = j + 1
-        for line in lines:
-            if line == lines[0]:
-                continue
-            line = line[j:]
-            pre_line = "> " + line + os.linesep
-            result += pre_line
-        result += '+'.ljust(width - 2, '-') + '+'
-        content = result
-    return content
-
-
-# replace the case link mindspore version to match with current mindspore version
-
-
-# replace mindspore version in link
-def _replace(link, keys, target):
-    """
-    :param link: str, the case web page's link
-    :param keys: list[str], regular expressions for different web page, like note, api and faq.
-    :param target: list[str], the link keywords of web pages of note, api and faq, corresponding to current
-                   mindspore version
-    :return: link: replaced web page's link, corresponding to current mindspore version
-    """
-    for i, key in enumerate(keys):
-        match = re.search(key, link)
-        if match:
-            link = link[:match.start()] + target[i] + link[match.end():]
-            break
-    return link
-
-
-def _replace_link_version(link, link_version, mindspore_version):
-    """
-    replace url link version for diff version
-    """
-    if mindspore_version < link_version:
-        return link
-    if mindspore_version < "r1.7" or link_version >= "r1.7":
-        match = re.search(link_version, link)
-        link = link[:match.start()] + mindspore_version + link[match.end():]
-        return link
-    if link_version < "r1.7" <= mindspore_version:
-        keys = [r"note/zh-CN/{}".format(link_version),
-                r"api/zh-CN/{}".format(link_version),
-                r"faq/zh-CN/{}".format(link_version)]
-        target = ["zh-CN/{}/note".format(mindspore_version),
-                  "zh-CN/{}".format(mindspore_version),
-                  "zh-CN/{}/faq".format(mindspore_version)]
-        link = _replace(link, keys, target)
-    return link
-
-
-def _format_case_str(content, mindspore_version):
-    """
-    format case string
-    """
-    if content:
-        # match, no replace
-        lines = content.split(os.linesep)
-        result = ""
-        for line in lines:
-            line = line.lstrip()
-            match = re.search(mindspore_version, line)
-            if not match:
-                key = r"(r1.[6-9])|(r2.[0-9])"
-                match = re.search(key, line)
-                # no mindspore link, return
-                if match:
-                    link_version = line[match.start():match.end()]
-                    line = _replace_link_version(line, link_version, mindspore_version)
-                result += line + os.linesep
-            else:  # link version same with mindspore version, no replace
-                return content
-        content = result
-    return content
-
-
-def _filter_stack(stack):
-    result = True
-    black_stack_list = ["mindspore/nn/cell.py.*in __call__",
-                        "mindspore/nn/cell.py.*in run_construct",
-                        "mindspore/nn/layer/basic.py.*in proposal_wrapper",
-                        "mindspore/common/api.py.*in wrapper",
-                        "mindspore/common/api.py.*in real_run_op",
-                        "mindspore/ops/primitive.py.*in __call__",
-                        "proposal_action.py.*in proposal_wrapper",
-                        "mindspore/nn/cell.py.*in _run_construct",
-                        "mindspore/ops/primitive.py.*in __check__"]
-    for black_stack in black_stack_list:
-        if re.search(black_stack, stack):
-            result = False
-            break
-    return result
-
-
-def print_clear_exception(exc_type, exc_value, exc_traceback_obj):
-    if exc_traceback_obj:
-        _print_msg("[TroubleShooter-Clear Stack] Python Traceback (most recent call last):", "NULL", False)
-        org_err_stack = traceback.format_exception(exc_type, exc_value, exc_traceback_obj)
-        for stack in org_err_stack:
-            if _filter_stack(stack):
-                print(stack.rstrip(os.linesep))
-
-
-def print_format_exception(exc_type, exc_value, exc_traceback_obj):
-    """
-    print format exception, for old mindspore version
-    """
-    import mindspore
-    ms_version = mindspore.__version__[:3]
-    if ms_version >= '1.8':
-        traceback.print_exc()
-        return
-
-    msg_dict = get_errmsg_dict(exc_type, exc_value)
-    _print_stack(exc_traceback_obj)
-    _print_msg("Error Message:", msg_dict.get("err_msg"))
-
-    if msg_dict.get("construct_stack_msg"):
-        _print_msg("The Traceback of Net Construct Code:", msg_dict.get("construct_stack_msg"))
-    else:
-        _print_msg("The Traceback of Net Construct Code:", msg_dict.get("construct_stack_in_file_msg"))
-    _print_msg("C++ Function:", msg_dict.get("cpp_fun_msg"))
-    _print_msg("Inner Message:", msg_dict.get("abstract_inner_msg"))
-
-
-def format_error_message(error_message):
-    """
-    format error message, from string to dict
-    """
-    msg_list = error_message.split('----------------------------------------------------')
-    format_msg_dict = {}
-    current_key = None
-    for msg in msg_list:
-        if msg_list.index(msg) == 0:
-            format_msg_dict["error_message"] = msg
-            continue
-        msg = msg.strip().strip(os.linesep)
-        if msg.startswith("- "):
-            current_key = msg[2:]
-            continue
-        if current_key:
-            format_msg_dict[current_key] = msg
-    return format_msg_dict
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""format output"""
+
+import os
+import re
+from textwrap import fill
+import traceback
+from prettytable import PrettyTable
+from troubleshooter.common.util import print_line
+from troubleshooter.common.ms_utils import get_errmsg_dict
+
+TABLE_WIDTH = 50
+DELIMITER_LEN = 100
+
+# GLog level and level name
+_item_to_cn = {
+    'item': '项目',
+    'desc': '描述',
+    'ms_version': '版本信息:',
+    'ms_mode': '执行模式:',
+    'ms_device': '配置设备:',  # GPU, CPU, Ascend
+    'ms_status': '执行阶段:',
+    'code_line': '代码行:',
+    'cause': '可能原因:',
+    'err_code': '示例错误代码：',
+    'fixed_code': '示例正确代码：',
+    'proposal': '处理建议:',
+    'case': '相关案例:',
+    'sink_mode': '下沉模式:',  # 图下沉，数据下沉，非下沉
+    'case_id': 'ID:',
+}
+
+
+def _add_row(x, item, message, width=TABLE_WIDTH, break_long_words=False, break_on_hyphens=False):
+    if message is None:
+        return
+    item_cn = _item_to_cn.get(item)
+    format_message = _format_str_length(message) if os.linesep in message else message
+    x.add_row([item_cn, fill(format_message, width=width, break_long_words=break_long_words,
+                             break_on_hyphens=break_on_hyphens)])
+
+
+def print_weight_compare_result(result_list, print_type=1):
+    x = PrettyTable()
+    x.title = 'The list of comparison results'
+    x.field_names = ["Parameter name of input ckpt", "Parameter name of converted ckpt", "Whether shape are equal", "Parameter shape of input ckpt", "Parameter shape of converted ckpt"]
+    for result in result_list:
+        if print_type == 1:
+            x.add_row([result[0],result[1],result[2],result[3],result[4]])
+        elif result[2] is not True:
+            x.add_row([result[0], result[1], result[2], result[3], result[4]])
+    print(x.get_string())
+
+
+def print_convert_result(result_list):
+    x = PrettyTable()
+    x.title = 'The list of conversion result'
+    x.field_names = ["Parameter name of pth", "Parameter name of converted ckpt", "Whether the name is converted",
+                     "Whether the weight value is converted","Parameter shape of pth","Parameter shape of ckpt"]
+    for result in result_list:
+        x.add_row([result[0],result[1],result[2],result[3],result[4],result[5]])
+    print(x.get_string())
+
+def print_diff_result(result_list):
+    x = PrettyTable()
+    x.title = 'The list of comparison results'
+    x.field_names = ["orig array name", "target array name", "Results of comparison", "(mean,max,min)"]
+    for result in result_list:
+        x.add_row([result[0],result[1],result[2],result[3]])
+    print(x.get_string())
+
+def print_result(expert_experience, write_file_path):
+    """
+    print MindSpore FAR
+    """
+    x = PrettyTable()
+    item_desc = _item_to_cn
+    x.title = 'MindSpore FAR(Failure Analysis Report)'
+    x.field_names = [item_desc.get("item"), item_desc.get("desc")]
+    x.align[item_desc.get("desc")] = 'l'
+    mindspore_version = expert_experience.get("mindspore_version")
+    mindspore_mode = expert_experience.get("mindspore_mode")
+    mindspore_device = expert_experience.get("Device Type")
+    x.add_row([item_desc.get("ms_version"), fill(mindspore_version, width=TABLE_WIDTH)])
+    x.add_row([item_desc.get("ms_mode"), fill(mindspore_mode, width=TABLE_WIDTH)])
+    if mindspore_device:
+        x.add_row([item_desc.get("ms_device"), fill(mindspore_device, width=TABLE_WIDTH)])
+    ms_status = expert_experience.get("ms_status")
+    code_line = expert_experience.get("code_line")
+    sink_mode = expert_experience.get("Sink Mode")
+    if ms_status:
+        x.add_row([item_desc.get("ms_status"), fill(ms_status, width=TABLE_WIDTH)])
+    if code_line:
+        x.add_row([item_desc.get("code_line"), fill(code_line, width=TABLE_WIDTH)])
+    if sink_mode:
+        x.add_row([item_desc.get("sink_mode"), fill(sink_mode, width=TABLE_WIDTH)])
+
+    # 可能原因
+    fault_cause = expert_experience.get('Fault Cause')
+    _add_row(x, "cause", fault_cause)
+
+    # 错误代码
+    err_code = expert_experience.get("Error Case")
+    err_code = _format_code_str(err_code)
+
+    _add_row(x, "err_code", err_code)
+    # 处理建议
+    suggestion = expert_experience.get("Modification Suggestion")
+    _add_row(x, "proposal", suggestion)
+    # 正确代码
+    fixed_code = expert_experience.get("Fixed Case")
+    fixed_code = _format_code_str(fixed_code)
+    _add_row(x, "fixed_code", fixed_code)
+    # 相关案例
+    fault_case = expert_experience.get("Fault Case")
+    fault_case = _format_case_str(fault_case, mindspore_version)
+    _add_row(x, "case", fault_case)
+    if write_file_path:
+        case_id = expert_experience.get("ID")
+        _add_row(x, "case_id", case_id)
+        file = os.path.join(write_file_path, "mindspore_failure_analysis_report.log")
+        with open(file, "w") as f:
+            f.write(x.get_string() + os.linesep)
+    print(x.get_string())
+
+
+def _print_msg(title, msg=None, print_msg=True):
+    if msg:
+        print_line("-", DELIMITER_LEN)
+        print("-  " + title)
+        print_line("-", DELIMITER_LEN)
+        if print_msg:
+            print(msg.rstrip(os.linesep) + os.linesep)
+
+
+def _print_stack(exc_traceback_obj):
+    if exc_traceback_obj:
+        _print_msg("Python Traceback (most recent call last):", "NULL", False)
+        traceback.print_tb(exc_traceback_obj)
+        print("")
+
+
+def _format_str_length(string):
+    str_list = string.split(os.linesep)
+    result_str = ""
+    for str_tmp in str_list:
+        result_str = result_str + str_tmp.ljust(TABLE_WIDTH) + os.linesep
+    return result_str
+
+
+def _format_code_str(content, width=50):
+    """
+    format code str
+    """
+    if content:
+        lines = content.split("\n")
+        result = '+'.ljust(width - 2, '-') + '+' + os.linesep
+        line = lines[1]
+        if line == '':
+            return content
+        j = 0
+        while line[j] == ' ':
+            j = j + 1
+        for line in lines:
+            if line == lines[0]:
+                continue
+            line = line[j:]
+            pre_line = "> " + line + os.linesep
+            result += pre_line
+        result += '+'.ljust(width - 2, '-') + '+'
+        content = result
+    return content
+
+
+# replace the case link mindspore version to match with current mindspore version
+
+
+# replace mindspore version in link
+def _replace(link, keys, target):
+    """
+    :param link: str, the case web page's link
+    :param keys: list[str], regular expressions for different web page, like note, api and faq.
+    :param target: list[str], the link keywords of web pages of note, api and faq, corresponding to current
+                   mindspore version
+    :return: link: replaced web page's link, corresponding to current mindspore version
+    """
+    for i, key in enumerate(keys):
+        match = re.search(key, link)
+        if match:
+            link = link[:match.start()] + target[i] + link[match.end():]
+            break
+    return link
+
+
+def _replace_link_version(link, link_version, mindspore_version):
+    """
+    replace url link version for diff version
+    """
+    if mindspore_version < link_version:
+        return link
+    if mindspore_version < "r1.7" or link_version >= "r1.7":
+        match = re.search(link_version, link)
+        link = link[:match.start()] + mindspore_version + link[match.end():]
+        return link
+    if link_version < "r1.7" <= mindspore_version:
+        keys = [r"note/zh-CN/{}".format(link_version),
+                r"api/zh-CN/{}".format(link_version),
+                r"faq/zh-CN/{}".format(link_version)]
+        target = ["zh-CN/{}/note".format(mindspore_version),
+                  "zh-CN/{}".format(mindspore_version),
+                  "zh-CN/{}/faq".format(mindspore_version)]
+        link = _replace(link, keys, target)
+    return link
+
+
+def _format_case_str(content, mindspore_version):
+    """
+    format case string
+    """
+    if content:
+        # match, no replace
+        lines = content.split(os.linesep)
+        result = ""
+        for line in lines:
+            line = line.lstrip()
+            match = re.search(mindspore_version, line)
+            if not match:
+                key = r"(r1.[6-9])|(r2.[0-9])"
+                match = re.search(key, line)
+                # no mindspore link, return
+                if match:
+                    link_version = line[match.start():match.end()]
+                    line = _replace_link_version(line, link_version, mindspore_version)
+                result += line + os.linesep
+            else:  # link version same with mindspore version, no replace
+                return content
+        content = result
+    return content
+
+
+def _filter_stack(stack):
+    result = True
+    black_stack_list = ["mindspore/nn/cell.py.*in __call__",
+                        "mindspore/nn/cell.py.*in run_construct",
+                        "mindspore/nn/layer/basic.py.*in proposal_wrapper",
+                        "mindspore/common/api.py.*in wrapper",
+                        "mindspore/common/api.py.*in real_run_op",
+                        "mindspore/ops/primitive.py.*in __call__",
+                        "proposal_action.py.*in proposal_wrapper",
+                        "mindspore/nn/cell.py.*in _run_construct",
+                        "mindspore/ops/primitive.py.*in __check__"]
+    for black_stack in black_stack_list:
+        if re.search(black_stack, stack):
+            result = False
+            break
+    return result
+
+
+def print_clear_exception(exc_type, exc_value, exc_traceback_obj):
+    if exc_traceback_obj:
+        _print_msg("[TroubleShooter-Clear Stack] Python Traceback (most recent call last):", "NULL", False)
+        org_err_stack = traceback.format_exception(exc_type, exc_value, exc_traceback_obj)
+        for stack in org_err_stack:
+            if _filter_stack(stack):
+                print(stack.rstrip(os.linesep))
+
+
+def print_format_exception(exc_type, exc_value, exc_traceback_obj):
+    """
+    print format exception, for old mindspore version
+    """
+    import mindspore
+    ms_version = mindspore.__version__[:3]
+    if ms_version >= '1.8':
+        traceback.print_exc()
+        return
+
+    msg_dict = get_errmsg_dict(exc_type, exc_value)
+    _print_stack(exc_traceback_obj)
+    _print_msg("Error Message:", msg_dict.get("err_msg"))
+
+    if msg_dict.get("construct_stack_msg"):
+        _print_msg("The Traceback of Net Construct Code:", msg_dict.get("construct_stack_msg"))
+    else:
+        _print_msg("The Traceback of Net Construct Code:", msg_dict.get("construct_stack_in_file_msg"))
+    _print_msg("C++ Function:", msg_dict.get("cpp_fun_msg"))
+    _print_msg("Inner Message:", msg_dict.get("abstract_inner_msg"))
+
+
+def format_error_message(error_message):
+    """
+    format error message, from string to dict
+    """
+    msg_list = error_message.split('----------------------------------------------------')
+    format_msg_dict = {}
+    current_key = None
+    for msg in msg_list:
+        if msg_list.index(msg) == 0:
+            format_msg_dict["error_message"] = msg
+            continue
+        msg = msg.strip().strip(os.linesep)
+        if msg.startswith("- "):
+            current_key = msg[2:]
+            continue
+        if current_key:
+            format_msg_dict[current_key] = msg
+    return format_msg_dict
```

### Comparing `troubleshooter-1.0.6/troubleshooter/common/ms_callback.py` & `troubleshooter-1.0.7/troubleshooter/common/ms_callback.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-
-import mindspore
-class StopMonitor(mindspore.train.callback.Callback):
-    def __init__(self, stop_epoch=1, stop_step=1):
-        """定义初始化过程"""
-        super(StopMonitor, self).__init__()
-        self.stop_epoch = stop_epoch  # 定义step
-        self.stop_step = stop_step  # 定义step
-
-    def on_train_step_end(self, run_context):
-        """每个step结束后执行的操作"""
-        cb_params = run_context.original_args()
-        epoch_num = cb_params.cur_epoch_num  # 获取epoch值
-        step_num = cb_params.cur_step_num  # 获取step值
-        cur_step_in_epoch = (cb_params.cur_step_num - 1) % cb_params.batch_num + 1
-        if step_num == 1875:
-            print(step_num)
-        if epoch_num == self.stop_epoch and cur_step_in_epoch == self.stop_step:
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+
+import mindspore
+class StopMonitor(mindspore.train.callback.Callback):
+    def __init__(self, stop_epoch=1, stop_step=1):
+        """定义初始化过程"""
+        super(StopMonitor, self).__init__()
+        self.stop_epoch = stop_epoch  # 定义step
+        self.stop_step = stop_step  # 定义step
+
+    def on_train_step_end(self, run_context):
+        """每个step结束后执行的操作"""
+        cb_params = run_context.original_args()
+        epoch_num = cb_params.cur_epoch_num  # 获取epoch值
+        step_num = cb_params.cur_step_num  # 获取step值
+        cur_step_in_epoch = (cb_params.cur_step_num - 1) % cb_params.batch_num + 1
+        if step_num == 1875:
+            print(step_num)
+        if epoch_num == self.stop_epoch and cur_step_in_epoch == self.stop_step:
             run_context.request_stop()  # 停止训练
```

### Comparing `troubleshooter-1.0.6/troubleshooter/common/ms_utils.py` & `troubleshooter-1.0.7/troubleshooter/common/ms_utils.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""build information"""
-
-OUT_OF_INDEX = -1
-CPP_FUN_INDEX_EXTEND = 1
-
-
-def _get_ms_information(result):
-    """
-    get mindspore information
-    """
-    import mindspore
-    from mindspore import context
-
-    ms_version = "r" + mindspore.__version__[:3]
-    result["mindspore_version"] = ms_version
-    mode = context.get_context("mode")
-    device = context.get_context("device_target")
-    if mode == 0:
-        result["mindspore_mode"] = "Graph Mode"
-    else:
-        result["mindspore_mode"] = "PyNative Mode"
-    result["Device Type"] = device
-    return result
-
-
-# this code will be discarded
-# pylint: disable=R1714
-def get_errmsg_dict(exc_type, exc_value):
-    """
-    format error message, from string to dict
-    """
-    error_type = str(exc_type.__name__)
-    org_err_msg = str(exc_value)
-    cpp_fun_msg = None
-    construct_stack_msg = None
-    abstract_inner_msg = None
-    construct_stack_in_file_msg = None
-    err_msg = org_err_msg
-    construct_stack_index = org_err_msg.find("The function call stack")
-    construct_stack_in_file_index = org_err_msg.find("# In file /")
-    cpp_fun_index = -1
-    abstract_inner_msg_index = org_err_msg.find("The abstract type of the return value")
-
-    cpp_fun_flag_index = org_err_msg.find("]")
-    if cpp_fun_flag_index != OUT_OF_INDEX:
-        cpp_flag_index = org_err_msg[0:cpp_fun_flag_index].find(".cc:")
-        if cpp_flag_index != OUT_OF_INDEX:
-            cpp_fun_index = cpp_fun_flag_index + CPP_FUN_INDEX_EXTEND
-    if construct_stack_index != OUT_OF_INDEX and cpp_fun_index != OUT_OF_INDEX:
-        cpp_fun_msg = org_err_msg[0:cpp_fun_index - CPP_FUN_INDEX_EXTEND]
-        construct_stack_msg = org_err_msg[construct_stack_index:len(org_err_msg)]
-        if abstract_inner_msg_index != OUT_OF_INDEX:
-            err_msg = org_err_msg[cpp_fun_index:abstract_inner_msg_index]
-            abstract_inner_msg = org_err_msg[abstract_inner_msg_index:construct_stack_index]
-        else:
-            err_msg = org_err_msg[cpp_fun_index:construct_stack_index]
-    elif construct_stack_index == OUT_OF_INDEX and cpp_fun_index != OUT_OF_INDEX:
-        if construct_stack_in_file_index != OUT_OF_INDEX:
-            cpp_fun_msg = org_err_msg[0:cpp_fun_index - CPP_FUN_INDEX_EXTEND]
-            err_msg = org_err_msg[cpp_fun_index:construct_stack_in_file_index]
-            construct_stack_in_file_msg = org_err_msg[construct_stack_in_file_index:len(org_err_msg)]
-        else:
-            cpp_fun_msg = org_err_msg[0:cpp_fun_index - CPP_FUN_INDEX_EXTEND]
-            err_msg = org_err_msg[cpp_fun_index:len(org_err_msg)]
-
-    err_msg = error_type + ":" + err_msg
-    errmsg_dict = {"cpp_fun_msg": cpp_fun_msg, "construct_stack_msg": construct_stack_msg, "err_msg": err_msg,
-                   "abstract_inner_msg": abstract_inner_msg,
-                   "construct_stack_in_file_msg": construct_stack_in_file_msg}
-    return errmsg_dict
-
-
-def base_information_build(result):
-    ret_result = _get_ms_information(result)
-    device_type = ret_result.get("Device Type")
-    if not device_type:
-        ret_result["Device Type"] = "Unknow"
-    return ret_result
-
-
-
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""build information"""
+
+OUT_OF_INDEX = -1
+CPP_FUN_INDEX_EXTEND = 1
+
+
+def _get_ms_information(result):
+    """
+    get mindspore information
+    """
+    import mindspore
+    from mindspore import context
+
+    ms_version = "r" + mindspore.__version__[:3]
+    result["mindspore_version"] = ms_version
+    mode = context.get_context("mode")
+    device = context.get_context("device_target")
+    if mode == 0:
+        result["mindspore_mode"] = "Graph Mode"
+    else:
+        result["mindspore_mode"] = "PyNative Mode"
+    result["Device Type"] = device
+    return result
+
+
+# this code will be discarded
+# pylint: disable=R1714
+def get_errmsg_dict(exc_type, exc_value):
+    """
+    format error message, from string to dict
+    """
+    error_type = str(exc_type.__name__)
+    org_err_msg = str(exc_value)
+    cpp_fun_msg = None
+    construct_stack_msg = None
+    abstract_inner_msg = None
+    construct_stack_in_file_msg = None
+    err_msg = org_err_msg
+    construct_stack_index = org_err_msg.find("The function call stack")
+    construct_stack_in_file_index = org_err_msg.find("# In file /")
+    cpp_fun_index = -1
+    abstract_inner_msg_index = org_err_msg.find("The abstract type of the return value")
+
+    cpp_fun_flag_index = org_err_msg.find("]")
+    if cpp_fun_flag_index != OUT_OF_INDEX:
+        cpp_flag_index = org_err_msg[0:cpp_fun_flag_index].find(".cc:")
+        if cpp_flag_index != OUT_OF_INDEX:
+            cpp_fun_index = cpp_fun_flag_index + CPP_FUN_INDEX_EXTEND
+    if construct_stack_index != OUT_OF_INDEX and cpp_fun_index != OUT_OF_INDEX:
+        cpp_fun_msg = org_err_msg[0:cpp_fun_index - CPP_FUN_INDEX_EXTEND]
+        construct_stack_msg = org_err_msg[construct_stack_index:len(org_err_msg)]
+        if abstract_inner_msg_index != OUT_OF_INDEX:
+            err_msg = org_err_msg[cpp_fun_index:abstract_inner_msg_index]
+            abstract_inner_msg = org_err_msg[abstract_inner_msg_index:construct_stack_index]
+        else:
+            err_msg = org_err_msg[cpp_fun_index:construct_stack_index]
+    elif construct_stack_index == OUT_OF_INDEX and cpp_fun_index != OUT_OF_INDEX:
+        if construct_stack_in_file_index != OUT_OF_INDEX:
+            cpp_fun_msg = org_err_msg[0:cpp_fun_index - CPP_FUN_INDEX_EXTEND]
+            err_msg = org_err_msg[cpp_fun_index:construct_stack_in_file_index]
+            construct_stack_in_file_msg = org_err_msg[construct_stack_in_file_index:len(org_err_msg)]
+        else:
+            cpp_fun_msg = org_err_msg[0:cpp_fun_index - CPP_FUN_INDEX_EXTEND]
+            err_msg = org_err_msg[cpp_fun_index:len(org_err_msg)]
+
+    err_msg = error_type + ":" + err_msg
+    errmsg_dict = {"cpp_fun_msg": cpp_fun_msg, "construct_stack_msg": construct_stack_msg, "err_msg": err_msg,
+                   "abstract_inner_msg": abstract_inner_msg,
+                   "construct_stack_in_file_msg": construct_stack_in_file_msg}
+    return errmsg_dict
+
+
+def base_information_build(result):
+    ret_result = _get_ms_information(result)
+    device_type = ret_result.get("Device Type")
+    if not device_type:
+        ret_result["Device Type"] = "Unknow"
+    return ret_result
+
+
+
```

### Comparing `troubleshooter-1.0.6/troubleshooter/common/util.py` & `troubleshooter-1.0.7/troubleshooter/common/util.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""util functions"""
-import re
-import os
-import stat
-
-
-def print_line(char, times):
-    print(char * times)
-
-
-def get_ms_log_path():
-    log_path = os.environ.get('GLOG_log_dir')
-    return log_path
-
-
-def create_save_path(data_save_path):
-    """Get output path of data."""
-    data_save_path = validate_and_normalize_path(data_save_path)
-    if not os.path.exists(data_save_path):
-        os.makedirs(data_save_path, exist_ok=True)
-        os.chmod(data_save_path, stat.S_IRUSR | stat.S_IWUSR | stat.S_IXUSR)
-    return data_save_path
-
-
-def validate_and_normalize_path(
-        path,
-        check_absolute_path=False,
-        allow_parent_dir=False,
-):
-    """
-    Validates path and returns its normalized form.
-
-    If path has a valid scheme, treat path as url, otherwise consider path a
-    unix local path.
-
-    Note:
-        File scheme (rfc8089) is currently not supported.
-
-    Args:
-        path (str): Path to be normalized.
-        check_absolute_path (bool): Whether check path scheme is supported.
-        allow_parent_dir (bool): Whether allow parent dir in path.
-
-    Returns:
-        str, normalized path.
-    """
-    if not path:
-        raise ValueError("The path is invalid!")
-
-    path_str = str(path)
-    if not allow_parent_dir:
-        path_components = path_str.split("/")
-        if ".." in path_components:
-            raise ValueError("The path is invalid!")
-
-    # path does not have valid schema, treat it as unix local path.
-    if check_absolute_path:
-        if not path_str.startswith("/"):
-            raise ValueError("The path is invalid!")
-    try:
-        # most unix systems allow
-        normalized_path = os.path.realpath(path)
-    except ValueError:
-        raise ValueError("The path is invalid!")
-
-    return normalized_path
-
-
-def compare_key_words(err_msg, key_word):
-    """Find out whether the key log information is in the exception or not."""
-    return key_word and err_msg and re.search(key_word, err_msg)
-
-
-def compare_stack_words(err_msg, key_word):
-    """Find out whether the key log information is in the exception or not."""
-    if key_word and err_msg and not re.search(key_word, err_msg):
-        return False
-    return True
-
-
-def find_file(dir, suffix=".npy"):
-    file_list = []
-    normal_dir = validate_and_normalize_path(dir)
-    walk_generator = os.walk(normal_dir)
-    for root_path, dirs, files in walk_generator:
-        if len(files) < 1:
-            continue
-        for file in files:
-            file_name, suffix_name = os.path.splitext(file)
-            if suffix_name == suffix:
-                file_list.append(file)
-    return file_list
-
-def make_directory(path: str):
-    """Make directory."""
-    if path is None or not isinstance(path, str) or path.strip() == "":
-        raise TypeError("Input path '{}' is invalid type".format(path))
-
-    path = os.path.realpath(path)
-
-    if os.path.exists(path):
-        real_path = path
-    else:
-        try:
-            permissions = os.R_OK | os.W_OK | os.X_OK
-            os.umask(permissions << 3 | permissions)
-            mode = permissions << 6
-            os.makedirs(path, mode=mode, exist_ok=True)
-            real_path = path
-        except PermissionError:
-            raise TypeError("No write permission on the directory `{path}`.")
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""util functions"""
+import re
+import os
+import stat
+
+
+def print_line(char, times):
+    print(char * times)
+
+
+def get_ms_log_path():
+    log_path = os.environ.get('GLOG_log_dir')
+    return log_path
+
+
+def create_save_path(data_save_path):
+    """Get output path of data."""
+    data_save_path = validate_and_normalize_path(data_save_path)
+    if not os.path.exists(data_save_path):
+        os.makedirs(data_save_path, exist_ok=True)
+        os.chmod(data_save_path, stat.S_IRUSR | stat.S_IWUSR | stat.S_IXUSR)
+    return data_save_path
+
+
+def validate_and_normalize_path(
+        path,
+        check_absolute_path=False,
+        allow_parent_dir=False,
+):
+    """
+    Validates path and returns its normalized form.
+
+    If path has a valid scheme, treat path as url, otherwise consider path a
+    unix local path.
+
+    Note:
+        File scheme (rfc8089) is currently not supported.
+
+    Args:
+        path (str): Path to be normalized.
+        check_absolute_path (bool): Whether check path scheme is supported.
+        allow_parent_dir (bool): Whether allow parent dir in path.
+
+    Returns:
+        str, normalized path.
+    """
+    if not path:
+        raise ValueError("The path is invalid!")
+
+    path_str = str(path)
+    if not allow_parent_dir:
+        path_components = path_str.split("/")
+        if ".." in path_components:
+            raise ValueError("The path is invalid!")
+
+    # path does not have valid schema, treat it as unix local path.
+    if check_absolute_path:
+        if not path_str.startswith("/"):
+            raise ValueError("The path is invalid!")
+    try:
+        # most unix systems allow
+        normalized_path = os.path.realpath(path)
+    except ValueError:
+        raise ValueError("The path is invalid!")
+
+    return normalized_path
+
+
+def compare_key_words(err_msg, key_word):
+    """Find out whether the key log information is in the exception or not."""
+    return key_word and err_msg and re.search(key_word, err_msg)
+
+
+def compare_stack_words(err_msg, key_word):
+    """Find out whether the key log information is in the exception or not."""
+    if key_word and err_msg and not re.search(key_word, err_msg):
+        return False
+    return True
+
+
+def find_file(dir, suffix=".npy"):
+    file_list = []
+    normal_dir = validate_and_normalize_path(dir)
+    walk_generator = os.walk(normal_dir)
+    for root_path, dirs, files in walk_generator:
+        if len(files) < 1:
+            continue
+        for file in files:
+            file_name, suffix_name = os.path.splitext(file)
+            if suffix_name == suffix:
+                file_list.append(file)
+    return file_list
+
+def make_directory(path: str):
+    """Make directory."""
+    if path is None or not isinstance(path, str) or path.strip() == "":
+        raise TypeError("Input path '{}' is invalid type".format(path))
+
+    path = os.path.realpath(path)
+
+    if os.path.exists(path):
+        real_path = path
+    else:
+        try:
+            permissions = os.R_OK | os.W_OK | os.X_OK
+            os.umask(permissions << 3 | permissions)
+            mode = permissions << 6
+            os.makedirs(path, mode=mode, exist_ok=True)
+            real_path = path
+        except PermissionError:
+            raise TypeError("No write permission on the directory `{path}`.")
     return real_path
```

### Comparing `troubleshooter-1.0.6/troubleshooter/log.py` & `troubleshooter-1.0.7/troubleshooter/log.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/migrator/diff_handler.py` & `troubleshooter-1.0.7/troubleshooter/migrator/diff_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,301 +1,356 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""compare tools"""
-import os
-import torch
-import numpy as np
-from pprint import pprint
-from troubleshooter import log as logger
-from troubleshooter.common.util import validate_and_normalize_path, find_file, make_directory
-from troubleshooter.migrator.mapping_relation.weight_mapping_lib import weight_name_map, weight_value_map
-from troubleshooter.common.format_msg import print_diff_result, print_weight_compare_result, print_convert_result
-
-FRAMEWORK_TYPE = "ms"
-
-try:
-    import mindspore as ms
-except ModuleNotFoundError as e:
-    e_msg = e.msg
-    no_module_msg = "No module named 'mindspore'"
-    if e_msg == no_module_msg:
-        FRAMEWORK_TYPE = 'pt'
-    else:
-        raise e
-
-class TensorRecorder:
-    def __init__(self):
-        self.summary_record = None
-        self.count = 1
-
-    def init_tensor_summary(self, record_path=None, record_mode=None):
-        if record_mode is None:
-            record_mode = ms.get_context("mode")
-
-        if record_mode == 0:
-            self.summary_record = ms.SummaryRecord(record_path, export_options={'tensor_format': 'npy'})
-
-    def record(self):
-        if not self.summary_record:
-            self.summary_record.record()
-            self.summary_record.flush()
-
-    @staticmethod
-    def record_op(record_dir=None, record_mode=None, framework=None):
-        normal_dir = None
-
-        if framework is None:
-            framework = FRAMEWORK_TYPE
-
-        if record_dir is not None:
-            normal_dir = validate_and_normalize_path(record_dir)
-            make_directory(normal_dir)
-
-        if framework=="ms":
-            if record_mode is None:
-                record_mode = ms.get_context("mode")
-            if record_mode == 0:
-                if record_dir is not None:
-                    logger.user_warning("In MindSpore graph mode, only TensorSummary can be used to record data. "
-                                        "In this mode, The parameter 'record_dir' is not valid")
-                save_op = ms.ops.TensorSummary()
-            else:
-                def save_t2n(name, value):
-                    if normal_dir is not None:
-                        name = os.path.join(normal_dir, name)
-                    np.save(name+".npy", value.asnumpy())
-                save_op = save_t2n
-        else:
-            def save_t2n(name, value):
-                if normal_dir is not None:
-                    name = os.path.join(normal_dir, name)
-                np.save(name + ".npy", value.detach().numpy())
-            save_op = save_t2n
-
-        return save_op
-
-class DifferenceFinder:
-
-    def __init__(self, orig_dir, target_dir):
-        self.orig_dir = orig_dir
-        self.target_dir = target_dir
-    def get_filename_map_list(self):
-        name_map_list = []
-        orig_name_list = find_file(self.orig_dir)
-        orig_name_list.sort()
-        target_name_list = find_file(self.target_dir)
-        none_flag = False
-
-        if not (orig_name_list and target_name_list):
-            logger.user_error("The comparison file is not found in the directory. Please check whether the directory is correct")
-            exit(1)
-
-        for name in orig_name_list:
-            if name in target_name_list:
-                name_map_list.append((name, name))
-                target_name_list.remove(name)
-            else:
-                name_map_list.append((name, None))
-                none_flag = True
-
-        if target_name_list:
-            target_name_list.sort()
-            for name in target_name_list:
-                name_map_list.append((None, name))
-            none_flag = True
-
-        if none_flag:
-            logger.user_warning("The files in the original directory and the target directory cannot be fully mapped. "
-                                "Please manually complete the mapping of file names")
-            print("filename mapping list:" + str(name_map_list))
-        return name_map_list
-
-
-    def compare_npy_dir(self, name_map_list=None, **kwargs):
-        """
-        """
-        if name_map_list is None:
-            name_map_list = self.get_filename_map_list()
-
-        rtol = kwargs.get('rtol', 1e-05)
-        atol = kwargs.get('atol', 1e-08)
-        equal_nan = kwargs.get('equal_nan', False)
-
-        result_list = []
-        normal_orig_dir = validate_and_normalize_path(self.orig_dir)
-        normal_target_dir = validate_and_normalize_path(self.target_dir)
-        for name_map in name_map_list:
-            orig_name = name_map[0]
-            target_name = name_map[1]
-
-            if orig_name is None or target_name is None:
-                result = False
-                diff_detail = ()
-                result_list.append((orig_name, target_name, result, diff_detail))
-                continue
-
-            orig_file = os.path.join(normal_orig_dir, orig_name)
-            target_file = os.path.join(normal_target_dir, target_name)
-
-            if not os.path.isfile(orig_file) or not os.path.isfile(target_file):
-                continue
-
-            orig_value = np.load(orig_file)
-            target_value = np.load(target_file)
-            if orig_value.shape == target_value.shape:
-                result = np.allclose(orig_value, target_value, rtol=rtol, atol=atol, equal_nan=equal_nan)
-
-                if not result:
-                    value_diff = np.abs(orig_value - target_value)
-                    value_mean = value_diff.mean()
-                    value_max = value_diff.max()
-                    value_min = value_diff.min()
-                    diff_detail = value_mean, value_max, value_min
-                else:
-                    diff_detail = ()
-            else:
-                result = False
-                diff_detail = ("Shape is inconsistent", orig_value.shape, target_value.shape)
-
-            result_list.append((orig_name, target_name, result, diff_detail))
-        logger.user_attention("The compare directory information:\n The orig dir: %s \n The target dir: %s", self.orig_dir, self.target_dir)
-        print_diff_result(result_list)
-
-class WeightMigrator:
-
-    def __init__(self, pt_model=None, pth_file_path=None, ckpt_save_path=None):
-        self.weight_map = weight_name_map
-        self.ckpt_path = ckpt_save_path
-        self.pt_model = pt_model
-        self.pt_para_dict = torch.load(pth_file_path, map_location='cpu')
-        self.print_params_list = []
-
-
-    def _get_object(self, name):
-        object_res = None
-        index = name.rfind(".")
-        if index:
-            module_name = name[:index]
-            class_name = name[index + 1:]
-            import importlib
-            imp_module = importlib.import_module(module_name)
-            object_res = getattr(imp_module, class_name)
-        return object_res
-
-
-    def _get_trans_map(self, weight_name, module, weight_map, igone_name=False):
-        res_weight_map = {}
-        for api_name in weight_map:
-            obj = self._get_object(api_name)
-            if isinstance(module, obj):
-                para_map = weight_map.get(api_name)
-                for pt_para_name, ms_para_name in para_map.items():
-                    pt_para_item = weight_name + "." + pt_para_name
-                    if igone_name:
-                        ms_para_item = ms_para_name
-                    else:
-                        ms_para_item = weight_name + "." + ms_para_name
-                    res_weight_map[pt_para_item] = ms_para_item
-                break
-
-        return res_weight_map
-
-
-    def get_weight_map(self, print_map=False):
-        res_weight_name_map = {}
-        res_weight_value_map = {}
-        for name, module in self.pt_model.named_modules():
-            tmp_name_map = self._get_trans_map(name, module, weight_name_map)
-            if tmp_name_map:
-                res_weight_name_map.update(tmp_name_map)
-            tmp_value_map = self._get_trans_map(name, module, weight_value_map, igone_name=True)
-            if tmp_value_map:
-                res_weight_value_map.update(tmp_value_map)
-        if print_map:
-            pprint(res_weight_name_map)
-            pprint(res_weight_value_map)
-        return res_weight_name_map, res_weight_value_map
-
-
-    def _get_name_and_value(self, pth_param_name, name_map, value_map):
-        new_name = pth_param_name
-        parameter = self.pt_para_dict[pth_param_name]
-        ms_tensor = ms.Tensor(parameter.numpy())
-
-        # Update name based on name mapping
-        ms_para_item = name_map.get(pth_param_name)
-        if ms_para_item:
-            new_name = ms_para_item
-
-        # Update values based on parameter value mapping
-        if value_map is not None:
-            fun = value_map.get(pth_param_name)
-
-        if fun:
-            def_get_value = self._get_object(fun)
-            ms_tensor = def_get_value(ms_tensor)
-
-        self.print_params_list.append((pth_param_name, new_name, bool(ms_para_item), bool(fun) , parameter.size(),
-                                       ms_tensor.shape))
-        return new_name, ms_tensor
-
-
-    def convert(self, weight_name_map=None, weight_value_map=None ,print_conv_info=True):
-        name_map, value_map  = self.get_weight_map()
-        if weight_name_map is not None:
-            name_map =  weight_name_map
-        if weight_value_map is not None:
-            value_map =  weight_value_map
-
-        new_params_list = []
-
-        for pth_param_name in self.pt_para_dict:
-            # get ckpt name and value
-            new_name, ms_tensor = self._get_name_and_value(pth_param_name,name_map,value_map)
-            # add name and value to list
-            new_params_list.append({"name": new_name, "data": ms_tensor})
-
-        if new_params_list:
-            ms.save_checkpoint(new_params_list , self.ckpt_path)
-        else:
-            logger.user_warning("There are no parameters to be converted. Parameter conversion failed. "
-                                "Please check whether the configuration is correct")
-
-        if print_conv_info:
-             print_convert_result(self.print_params_list)
-
-        logger.user_attention("The PTH has been converted to the checkpoint of MindSpore. "
-                              "Please check whether the conversion result is correct. "
-                              "The saved path is: %s",self.ckpt_path)
-
-
-    def compare_ckpt(self, ckpt_path=None, converted_ckpt_path=None, print_result=1):
-        name_map_list = []
-        if converted_ckpt_path is None:
-            ckpt_after_convert_path = self.ckpt_path
-        ckpt_dict = ms.load_checkpoint(ckpt_path)
-        ckpt_after_conv_dict = ms.load_checkpoint(ckpt_after_convert_path)
-
-        for ms_para_name, ms_para in ckpt_dict.items():
-            ms_para_after_conv = ckpt_after_conv_dict.get(ms_para_name)
-
-            if ms_para_after_conv is not None:
-                name_map_list.append((ms_para_name, ms_para_name, (ms_para.shape == ms_para_after_conv.shape), ms_para.shape, ms_para_after_conv.shape))
-                ckpt_after_conv_dict.pop(ms_para_name)
-            else:
-                name_map_list.append((ms_para_name, None, None, ms_para.shape, None))
-
-        for name in ckpt_after_conv_dict:
-            name_map_list.append((None, name, None, None, ms_para_after_conv.shape))
-        print_weight_compare_result(name_map_list, print_type=print_result)
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""compare tools"""
+import os
+import torch
+import numpy as np
+from collections import OrderedDict
+from pprint import pprint
+from troubleshooter import log as logger
+from troubleshooter.common.util import validate_and_normalize_path, find_file, make_directory
+from troubleshooter.migrator.mapping_relation.weight_mapping_lib import weight_name_map, weight_value_map
+from troubleshooter.common.format_msg import print_diff_result, print_weight_compare_result, print_convert_result
+
+FRAMEWORK_TYPE = "ms"
+
+try:
+    import mindspore as ms
+except ModuleNotFoundError as e:
+    e_msg = e.msg
+    no_module_msg = "No module named 'mindspore'"
+    if e_msg == no_module_msg:
+        FRAMEWORK_TYPE = 'pt'
+    else:
+        raise e
+
+class TensorRecorder:
+    def __init__(self):
+        self.summary_record = None
+        self.count = 1
+
+    def init_tensor_summary(self, record_path=None, record_mode=None):
+        if record_mode is None:
+            record_mode = ms.get_context("mode")
+
+        if record_mode == 0:
+            self.summary_record = ms.SummaryRecord(record_path, export_options={'tensor_format': 'npy'})
+
+    def record(self):
+        if not self.summary_record:
+            self.summary_record.record()
+            self.summary_record.flush()
+
+    @staticmethod
+    def record_op(record_dir=None, record_mode=None, framework=None):
+        normal_dir = None
+
+        if framework is None:
+            framework = FRAMEWORK_TYPE
+
+        if record_dir is not None:
+            normal_dir = validate_and_normalize_path(record_dir)
+            make_directory(normal_dir)
+
+        if framework=="ms":
+            if record_mode is None:
+                record_mode = ms.get_context("mode")
+            if record_mode == 0:
+                if record_dir is not None:
+                    logger.user_warning("In MindSpore graph mode, only TensorSummary can be used to record data. "
+                                        "In this mode, The parameter 'record_dir' is not valid")
+                save_op = ms.ops.TensorSummary()
+            else:
+                def save_t2n(name, value):
+                    if normal_dir is not None:
+                        name = os.path.join(normal_dir, name)
+                    np.save(name+".npy", value.asnumpy())
+                save_op = save_t2n
+        else:
+            def save_t2n(name, value):
+                if normal_dir is not None:
+                    name = os.path.join(normal_dir, name)
+                np.save(name + ".npy", value.detach().numpy())
+            save_op = save_t2n
+
+        return save_op
+
+class DifferenceFinder:
+
+    def __init__(self, orig_dir, target_dir):
+        self.orig_dir = orig_dir
+        self.target_dir = target_dir
+    def get_filename_map_list(self):
+        name_map_list = []
+        orig_name_list = find_file(self.orig_dir)
+        orig_name_list.sort()
+        target_name_list = find_file(self.target_dir)
+        none_flag = False
+
+        if not (orig_name_list and target_name_list):
+            logger.user_error("The comparison file is not found in the directory. "
+                              "Please check whether the directory is correct")
+            exit(1)
+
+        for name in orig_name_list:
+            if name in target_name_list:
+                name_map_list.append((name, name))
+                target_name_list.remove(name)
+            else:
+                name_map_list.append((name, None))
+                none_flag = True
+
+        if target_name_list:
+            target_name_list.sort()
+            for name in target_name_list:
+                name_map_list.append((None, name))
+            none_flag = True
+
+        if none_flag:
+            logger.user_warning("The files in the original directory and the target directory cannot be fully mapped. "
+                                "Please manually complete the mapping of file names")
+            print("filename mapping list:" + str(name_map_list))
+        return name_map_list
+
+
+    def compare_npy_dir(self, name_map_list=None, **kwargs):
+        """
+        """
+        if name_map_list is None:
+            name_map_list = self.get_filename_map_list()
+
+        rtol = kwargs.get('rtol', 1e-05)
+        atol = kwargs.get('atol', 1e-08)
+        equal_nan = kwargs.get('equal_nan', False)
+
+        result_list = []
+        normal_orig_dir = validate_and_normalize_path(self.orig_dir)
+        normal_target_dir = validate_and_normalize_path(self.target_dir)
+        for name_map in name_map_list:
+            orig_name = name_map[0]
+            target_name = name_map[1]
+
+            if orig_name is None or target_name is None:
+                result = False
+                diff_detail = ()
+                result_list.append((orig_name, target_name, result, diff_detail))
+                continue
+
+            orig_file = os.path.join(normal_orig_dir, orig_name)
+            target_file = os.path.join(normal_target_dir, target_name)
+
+            if not os.path.isfile(orig_file) or not os.path.isfile(target_file):
+                continue
+
+            orig_value = np.load(orig_file)
+            target_value = np.load(target_file)
+            if orig_value.shape == target_value.shape:
+                result = np.allclose(orig_value, target_value, rtol=rtol, atol=atol, equal_nan=equal_nan)
+
+                if not result:
+                    value_diff = np.abs(orig_value - target_value)
+                    value_mean = value_diff.mean()
+                    value_max = value_diff.max()
+                    value_min = value_diff.min()
+                    diff_detail = value_mean, value_max, value_min
+                else:
+                    diff_detail = ()
+            else:
+                result = False
+                diff_detail = ("Shape is inconsistent", orig_value.shape, target_value.shape)
+
+            result_list.append((orig_name, target_name, result, diff_detail))
+        logger.user_attention("The compare directory information:\n The orig dir: %s \n The target dir: %s",
+                              self.orig_dir, self.target_dir)
+        print_diff_result(result_list)
+
+class WeightMigrator:
+
+    def __init__(self, pt_model=None, pth_file_path=None, pth_para_dict=None, ckpt_save_path=None):
+        self.weight_map = weight_name_map
+        self.ckpt_path = ckpt_save_path
+        self.pt_model = pt_model
+        self.pt_para_dict = self._get_para_dict(pth_file_path, pth_para_dict)
+        self.print_params_list = []
+
+
+    def _get_para_dict(self, pth_file_path, pth_para_dict):
+        if pth_para_dict:
+            return pth_para_dict
+
+        pt_para_dict = {}
+        pt_object = torch.load(pth_file_path, map_location='cpu')
+        if isinstance(pt_object, OrderedDict):
+            pt_para_dict = pt_object
+        elif isinstance(pt_object, torch.nn.Module):
+            pt_para_dict = pt_object.state_dict()
+        else:
+            raise ValueError("PTH file parsing failed, possible reasons: "
+                             "1) If using a custom method to save parameter files, please load and set "
+                             "the 'pth_para_dict' parameter yourself to use the conversion tool."
+                             "2) If the input is an optimizer parameter, this tool does not support "
+                             "the conversion of optimizer parameters.")
+
+        values = list(pt_para_dict.values())
+        if values and not isinstance(values[0], torch.Tensor):
+            raise ValueError("PTH file parsing failed, possible reasons: "
+                             "1) If using a custom method to save parameter files, please load and set "
+                             "the 'pth_para_dict' parameter yourself to use the conversion tool."
+                             "2) If the input is an optimizer parameter, this tool does not support "
+                             "the conversion of optimizer parameters.")
+        return pt_para_dict
+
+    def _get_object(self, name):
+        object_res = None
+        index = name.rfind(".")
+        if index:
+            module_name = name[:index]
+            class_name = name[index + 1:]
+            import importlib
+            imp_module = importlib.import_module(module_name)
+            object_res = getattr(imp_module, class_name)
+        return object_res
+
+
+    def _get_trans_map(self, weight_name, module, weight_map, igone_name=False):
+        res_weight_map = {}
+        for api_name in weight_map:
+            obj = self._get_object(api_name)
+            if isinstance(module, obj):
+                para_map = weight_map.get(api_name)
+                for pt_para_name, ms_para_name in para_map.items():
+                    pt_para_item = weight_name + "." + pt_para_name
+                    if igone_name:
+                        ms_para_item = ms_para_name
+                    else:
+                        ms_para_item = weight_name + "." + ms_para_name
+                    res_weight_map[pt_para_item] = ms_para_item
+                break
+
+        return res_weight_map
+
+
+    def _custorm_weight_name_prefix(self, weight_name_map, prefix=None):
+        if prefix:
+            custorm_name_map = {}
+            for key, value in weight_name_map.items():
+                # print(key, ":", prefix + '.' + value)
+                custorm_name_map[key] = str(prefix) + '.' + str(value)
+            return custorm_name_map
+        else:
+            return weight_name_map
+
+
+    def get_weight_map(self, print_map=False, full_name_map=False):
+        res_weight_name_map = {}
+        res_weight_value_map = {}
+        full_weight_name_map = {}
+
+        for name, module in self.pt_model.named_modules():
+            tmp_name_map = self._get_trans_map(name, module, weight_name_map)
+            if tmp_name_map:
+                res_weight_name_map.update(tmp_name_map)
+            tmp_value_map = self._get_trans_map(name, module, weight_value_map, igone_name=True)
+            if tmp_value_map:
+                res_weight_value_map.update(tmp_value_map)
+        if full_name_map:
+            for key, value in self.pt_para_dict.items():
+                full_weight_name_map[key]=key
+            full_weight_name_map.update(res_weight_name_map)
+            res_weight_name_map =  full_weight_name_map
+
+        if print_map:
+            pprint(res_weight_name_map)
+            pprint(res_weight_value_map)
+        return res_weight_name_map, res_weight_value_map
+
+
+    def _get_name_and_value(self, pth_param_name, name_map, value_map):
+        new_name = pth_param_name
+        parameter = self.pt_para_dict[pth_param_name]
+        ms_tensor = ms.Tensor(parameter.numpy())
+
+        # Update name based on name mapping
+        ms_para_item = name_map.get(pth_param_name)
+        if ms_para_item:
+            new_name = ms_para_item
+
+        # Update values based on parameter value mapping
+        if value_map is not None:
+            fun = value_map.get(pth_param_name)
+
+        if fun:
+            def_get_value = self._get_object(fun)
+            ms_tensor = def_get_value(ms_tensor)
+
+        self.print_params_list.append((pth_param_name, new_name, bool(ms_para_item), bool(fun) , parameter.size(),
+                                       ms_tensor.shape))
+        return new_name, ms_tensor
+
+
+    def convert(self, weight_name_map=None, weight_value_map=None ,weight_name_prefix=None, print_conv_info=True):
+
+        if weight_name_prefix:
+            name_map, value_map = self.get_weight_map(full_name_map=True)
+            name_map = self._custorm_weight_name_prefix(name_map, weight_name_prefix)
+        else:
+            name_map, value_map = self.get_weight_map()
+
+        if weight_name_map is not None:
+            name_map =  weight_name_map
+        if weight_value_map is not None:
+            value_map =  weight_value_map
+
+        new_params_list = []
+
+        for pth_param_name in self.pt_para_dict:
+            # get ckpt name and value
+            new_name, ms_tensor = self._get_name_and_value(pth_param_name,name_map,value_map)
+            # add name and value to list
+            new_params_list.append({"name": new_name, "data": ms_tensor})
+
+        if new_params_list:
+            ms.save_checkpoint(new_params_list , self.ckpt_path)
+        else:
+            logger.user_warning("There are no parameters to be converted. Parameter conversion failed. "
+                                "Please check whether the configuration is correct")
+
+        if print_conv_info:
+             print_convert_result(self.print_params_list)
+
+        logger.user_attention("The PTH has been converted to the checkpoint of MindSpore. "
+                              "Please check whether the conversion result is correct. "
+                              "The saved path is: %s",self.ckpt_path)
+
+
+    def compare_ckpt(self, ckpt_path=None, converted_ckpt_path=None, print_result=1):
+        name_map_list = []
+        if converted_ckpt_path is None:
+            ckpt_after_convert_path = self.ckpt_path
+        ckpt_dict = ms.load_checkpoint(ckpt_path)
+        ckpt_after_conv_dict = ms.load_checkpoint(ckpt_after_convert_path)
+
+        for ms_para_name, ms_para in ckpt_dict.items():
+            ms_para_after_conv = ckpt_after_conv_dict.get(ms_para_name)
+
+            if ms_para_after_conv is not None:
+                name_map_list.append((ms_para_name, ms_para_name, (ms_para.shape == ms_para_after_conv.shape),
+                                      ms_para.shape, ms_para_after_conv.shape))
+                ckpt_after_conv_dict.pop(ms_para_name)
+            else:
+                name_map_list.append((ms_para_name, None, None, ms_para.shape, None))
+
+        for name, ms_para in ckpt_after_conv_dict.items():
+            name_map_list.append((None, name, None, None, ms_para.shape))
+        print_weight_compare_result(name_map_list, print_type=print_result)
```

### Comparing `troubleshooter-1.0.6/troubleshooter/migrator/mapping_relation/weight_adapter.py` & `troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/weight_adapter.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-
-def trans_conv1d_weight_value(ms_tensor):
-    import mindspore as ms
-    result = ms.ops.expand_dims(ms_tensor, 2)
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+
+def trans_conv1d_weight_value(ms_tensor):
+    import mindspore as ms
+    result = ms.ops.expand_dims(ms_tensor, 2)
     return result
```

### Comparing `troubleshooter-1.0.6/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py` & `troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-
-
-weight_name_map = {"torch.nn.BatchNorm1d":{'weight': 'gamma', 'bias': 'beta', 'running_mean': 'moving_mean' , 'running_var': 'moving_variance'},
-    "torch.nn.BatchNorm2d":{'weight':'gamma', 'bias':'beta', 'running_mean':'moving_mean' ,'running_var':'moving_variance'},
-    "torch.nn.BatchNorm3d":{'weight':'gamma', 'bias':'beta', 'running_mean':'moving_mean' ,'running_var':'moving_variance'},
-    "torch.nn.Embedding":{'weight':'embedding_table'},
-    "torch.nn.GroupNorm":{'weight':'gamma', 'bias': 'beta'},
-    "torch.nn.LayerNorm":{'weight': 'gamma', 'bias': 'beta'},
-    "torch.nn.PReLU":{'weight':'a'},
-                   }
-
-weight_value_map = {"torch.nn.Conv1d":{'weight': 'troubleshooter.migrator.mapping_relation.weight_adapter.trans_conv1d_weight_value'}
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+
+
+weight_name_map = {"torch.nn.BatchNorm1d":{'weight': 'gamma', 'bias': 'beta', 'running_mean': 'moving_mean' , 'running_var': 'moving_variance'},
+    "torch.nn.BatchNorm2d":{'weight':'gamma', 'bias':'beta', 'running_mean':'moving_mean' ,'running_var':'moving_variance'},
+    "torch.nn.BatchNorm3d":{'weight':'gamma', 'bias':'beta', 'running_mean':'moving_mean' ,'running_var':'moving_variance'},
+    "torch.nn.Embedding":{'weight':'embedding_table'},
+    "torch.nn.GroupNorm":{'weight':'gamma', 'bias': 'beta'},
+    "torch.nn.LayerNorm":{'weight': 'gamma', 'bias': 'beta'},
+    "torch.nn.PReLU":{'weight':'a'},
+                   }
+
+weight_value_map = {"torch.nn.Conv1d":{'weight': 'troubleshooter.migrator.mapping_relation.weight_adapter.trans_conv1d_weight_value'}
                     }
```

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/__init__.py` & `troubleshooter-1.0.7/troubleshooter/proposer/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/allproposers/__init__.py` & `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/allproposers/base_proposer.py` & `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/base_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/allproposers/compiler_scene_proposer.py` & `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/compiler_proposer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""Compiler Proposer"""
-import traceback
-from troubleshooter.proposer.allproposers.base_proposer import Proposer
-from troubleshooter.proposer.knowledge_base.compiler_exp_lib import compiler_general_experience_list_cn
-
-
-class CompilerSceneProposer(Proposer):
-    """The default proposer."""
-
-    def __init__(self):
-        super().__init__()
-        self.experience_list = compiler_general_experience_list_cn
-
-    def analyze(self, exc_type, exc_value, traceback_obj):
-        """
-        Get the proposal from proposer.
-
-        Args:
-            traceback_obj:
-            exc_value:
-            exc_type:
-
-        Returns:
-            dict, the proposal from proposer instance.
-        """
-        error_message = str(exc_value) if exc_value else traceback.format_exc()
-        result = super().base_scene_analyze(error_message, self.experience_list)
-        return result
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+
+"""The compiler proposer."""
+import traceback
+from troubleshooter.proposer.allproposers.base_proposer import Proposer
+from troubleshooter.proposer.knowledge_base.compiler_exp_lib import compiler_experience_list_cn
+
+
+class CompilerProposer(Proposer):
+    """The Compiler proposer."""
+
+    def __init__(self):
+        super().__init__()
+        self.experience_list = compiler_experience_list_cn
+
+    def analyze(self, exc_type, exc_value, traceback_obj):
+        """
+        Get the proposal from proposer.
+
+        Args:
+            traceback_obj:
+            exc_value:
+            exc_type:
+
+        Returns:
+            dict, the proposal from proposer instance.
+        """
+        error_message = str(exc_value) if exc_value else traceback.format_exc()
+        result = super().base_case_analyze(error_message, self.experience_list)
+        return result
```

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/allproposers/dataset_proposer.py` & `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/dataset_proposer.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""Dataset Proposer"""
-import traceback
-from troubleshooter.proposer.allproposers.base_proposer import Proposer
-from troubleshooter.proposer.knowledge_base.dataset_exp_lib import dataset_experience_list_cn
-
-
-class DatasetProposer(Proposer):
-    """The Dataset proposer."""
-
-    def __init__(self):
-        super().__init__()
-        self.experience_list = dataset_experience_list_cn
-
-    def analyze(self, exc_type, exc_value, traceback_obj):
-        """
-        Get the proposal from proposer.
-
-        Args:
-            exc_type:
-            exc_value:
-            traceback_obj:
-
-        Returns:
-
-        """
-        error_message = str(exc_value) if exc_value is not None else traceback.format_exc()
-        result = super().base_case_analyze(error_message, self.experience_list)
-        return result
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""Dataset Proposer"""
+import traceback
+from troubleshooter.proposer.allproposers.base_proposer import Proposer
+from troubleshooter.proposer.knowledge_base.dataset_exp_lib import dataset_experience_list_cn
+
+
+class DatasetProposer(Proposer):
+    """The Dataset proposer."""
+
+    def __init__(self):
+        super().__init__()
+        self.experience_list = dataset_experience_list_cn
+
+    def analyze(self, exc_type, exc_value, traceback_obj):
+        """
+        Get the proposal from proposer.
+
+        Args:
+            exc_type:
+            exc_value:
+            traceback_obj:
+
+        Returns:
+
+        """
+        error_message = str(exc_value) if exc_value is not None else traceback.format_exc()
+        result = super().base_case_analyze(error_message, self.experience_list)
+        return result
```

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/allproposers/dataset_scene_proposer.py` & `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/compiler_scene_proposer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""Dataset scene Proposer"""
-from troubleshooter.proposer.allproposers.base_proposer import Proposer
-from troubleshooter.proposer.knowledge_base.dataset_exp_lib import data_general_experience_list_cn
-
-
-class DatasetSceneProposer(Proposer):
-    """The Dataset scene proposer."""
-
-    def __init__(self):
-        super().__init__()
-        self.experience_list = data_general_experience_list_cn
-
-    def analyze(self, exc_type, exc_value, traceback_obj):
-        """
-
-        Args:
-            exc_type:
-            exc_value:
-            traceback_obj:
-
-        Returns:
-
-        """
-        error_message = str(exc_value) if exc_value else traceback.format_exc()
-        result = super().base_scene_analyze(error_message, self.experience_list)
-        return result
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""Compiler Proposer"""
+import traceback
+from troubleshooter.proposer.allproposers.base_proposer import Proposer
+from troubleshooter.proposer.knowledge_base.compiler_exp_lib import compiler_general_experience_list_cn
+
+
+class CompilerSceneProposer(Proposer):
+    """The default proposer."""
+
+    def __init__(self):
+        super().__init__()
+        self.experience_list = compiler_general_experience_list_cn
+
+    def analyze(self, exc_type, exc_value, traceback_obj):
+        """
+        Get the proposal from proposer.
+
+        Args:
+            traceback_obj:
+            exc_value:
+            exc_type:
+
+        Returns:
+            dict, the proposal from proposer instance.
+        """
+        error_message = str(exc_value) if exc_value else traceback.format_exc()
+        result = super().base_scene_analyze(error_message, self.experience_list)
+        return result
```

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/allproposers/default_proposer.py` & `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/default_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/allproposers/front_proposer.py` & `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/front_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/allproposers/operators_proposer.py` & `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/operators_proposer.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""Operators Proposer"""
-import traceback
-from troubleshooter.proposer.allproposers.base_proposer import Proposer
-from troubleshooter.proposer.knowledge_base.operators_exp_lib import operators_experience_list_cn
-
-
-class OperatorsProposer(Proposer):
-    """The Operators proposer."""
-
-    def __init__(self):
-        super().__init__()
-        self.experience_list = operators_experience_list_cn
-
-    def analyze(self, exc_type, exc_value, traceback_obj):
-        """
-        Operators analyze
-        Args:
-            exc_type:
-            exc_value:
-            traceback_obj:
-
-        Returns:
-
-        """
-        error_message = str(exc_value) if exc_value is not None else traceback.format_exc()
-        result = super().base_case_analyze(error_message, self.experience_list)
-        return result
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""Operators Proposer"""
+import traceback
+from troubleshooter.proposer.allproposers.base_proposer import Proposer
+from troubleshooter.proposer.knowledge_base.operators_exp_lib import operators_experience_list_cn
+
+
+class OperatorsProposer(Proposer):
+    """The Operators proposer."""
+
+    def __init__(self):
+        super().__init__()
+        self.experience_list = operators_experience_list_cn
+
+    def analyze(self, exc_type, exc_value, traceback_obj):
+        """
+        Operators analyze
+        Args:
+            exc_type:
+            exc_value:
+            traceback_obj:
+
+        Returns:
+
+        """
+        error_message = str(exc_value) if exc_value is not None else traceback.format_exc()
+        result = super().base_case_analyze(error_message, self.experience_list)
+        return result
```

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/allproposers/operators_scene_proposer.py` & `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/operators_scene_proposer.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""Operators scene Proposer"""
-from troubleshooter.proposer.allproposers.base_proposer import Proposer
-from troubleshooter.proposer.knowledge_base.operators_exp_lib import operators_general_experience_list_cn
-
-
-class OperatorsSceneProposer(Proposer):
-    """The Operators scene proposer."""
-
-    def __init__(self):
-        super().__init__()
-        self.experience_list = operators_general_experience_list_cn
-
-    def analyze(self, exc_type, exc_value, traceback_obj):
-        """
-        Get the proposal from proposer.
-
-        Args:
-            options: options for proposer analysis
-
-        Returns:
-            dict, the proposal from proposer instance.
-        """
-        error_message = str(exc_value) if exc_value else traceback.format_exc()
-        req_condition = 1
-        result = super().base_scene_analyze(error_message, self.experience_list, req_condition)
-        return result
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""Operators scene Proposer"""
+from troubleshooter.proposer.allproposers.base_proposer import Proposer
+from troubleshooter.proposer.knowledge_base.operators_exp_lib import operators_general_experience_list_cn
+
+
+class OperatorsSceneProposer(Proposer):
+    """The Operators scene proposer."""
+
+    def __init__(self):
+        super().__init__()
+        self.experience_list = operators_general_experience_list_cn
+
+    def analyze(self, exc_type, exc_value, traceback_obj):
+        """
+        Get the proposal from proposer.
+
+        Args:
+            options: options for proposer analysis
+
+        Returns:
+            dict, the proposal from proposer instance.
+        """
+        error_message = str(exc_value) if exc_value else traceback.format_exc()
+        req_condition = 1
+        result = super().base_scene_analyze(error_message, self.experience_list, req_condition)
+        return result
```

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/allproposers/vm_proposer.py` & `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/vm_proposer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""VM Proposer"""
-import traceback
-from troubleshooter.common.util import compare_key_words, compare_stack_words
-from troubleshooter.common.format_msg import format_error_message
-from troubleshooter.proposer.allproposers.base_proposer import Proposer
-from troubleshooter.proposer.knowledge_base.vm_exp_lib import vm_experience_list_cn, vm_general_experience_list_cn
-
-
-class VmProposer(Proposer):
-    """The VM proposer."""
-
-    def __init__(self):
-        super().__init__()
-        self.experience_list = vm_experience_list_cn
-        self.general_experience_list = vm_general_experience_list_cn
-
-    def analyze(self, exc_type, exc_value, traceback_obj):
-        """
-        Vm analyze
-        Args:
-            exc_type:
-            exc_value:
-            traceback_obj:
-
-        Returns:
-
-        """
-        error_message = str(exc_value) if exc_value else traceback.format_exc()
-        msg_dict = format_error_message(error_message)
-        result = None
-
-        for experience in self.experience_list:
-            key_words = experience.get('Key Log Information')
-            python_stack_info = experience.get('Key Python Stack Information')
-            cplusplus_stack_info = experience.get('Key C++ Stack Information')
-            err_msg = msg_dict.get('error_message')
-            cpp_stack = msg_dict.get('C++ Call Stack: (For framework developers)')
-            ascend_err_msg = msg_dict.get('Ascend Error Message:')
-
-            if (compare_key_words(err_msg, key_words) or compare_key_words(ascend_err_msg, key_words)) and \
-                    compare_stack_words(err_msg, python_stack_info) and \
-                    compare_stack_words(cpp_stack, cplusplus_stack_info):
-                result = experience
-                break
-
-        if result is None:
-            result = super().base_scene_analyze(error_message, self.general_experience_list)
-
-        return result
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""VM Proposer"""
+import traceback
+from troubleshooter.common.util import compare_key_words, compare_stack_words
+from troubleshooter.common.format_msg import format_error_message
+from troubleshooter.proposer.allproposers.base_proposer import Proposer
+from troubleshooter.proposer.knowledge_base.vm_exp_lib import vm_experience_list_cn, vm_general_experience_list_cn
+
+
+class VmProposer(Proposer):
+    """The VM proposer."""
+
+    def __init__(self):
+        super().__init__()
+        self.experience_list = vm_experience_list_cn
+        self.general_experience_list = vm_general_experience_list_cn
+
+    def analyze(self, exc_type, exc_value, traceback_obj):
+        """
+        Vm analyze
+        Args:
+            exc_type:
+            exc_value:
+            traceback_obj:
+
+        Returns:
+
+        """
+        error_message = str(exc_value) if exc_value else traceback.format_exc()
+        msg_dict = format_error_message(error_message)
+        result = None
+
+        for experience in self.experience_list:
+            key_words = experience.get('Key Log Information')
+            python_stack_info = experience.get('Key Python Stack Information')
+            cplusplus_stack_info = experience.get('Key C++ Stack Information')
+            err_msg = msg_dict.get('error_message')
+            cpp_stack = msg_dict.get('C++ Call Stack: (For framework developers)')
+            ascend_err_msg = msg_dict.get('Ascend Error Message:')
+
+            if (compare_key_words(err_msg, key_words) or compare_key_words(ascend_err_msg, key_words)) and \
+                    compare_stack_words(err_msg, python_stack_info) and \
+                    compare_stack_words(cpp_stack, cplusplus_stack_info):
+                result = experience
+                break
+
+        if result is None:
+            result = super().base_scene_analyze(error_message, self.general_experience_list)
+
+        return result
```

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/__init__.py` & `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py` & `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,548 +1,654 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-
-compiler_experience_list_cn = [
-    {
-        "ID": "compiler_id_1",
-        "Fault Name": "construct 参数错误 <2.0",
-        "Key Log Information": "For 'Cell', the function construct .* 0 positional argument and 0 default argument",
-        "Key Python Stack Information": "",
-        "Key C++ Stack Information": "",
-        "Fault Cause": "继承nn.Cell类，重定义construct函数时，缺少self参数报错",
-        "Error Case": """
-                      def construct(a,b):
-                                    ^~~~~~~ 此处缺少了self""",
-        "Modification Suggestion": "修改construct定义,添加self参数.",
-        "Fixed Case": """
-                      def construct(self,a,b):
-                                      ^~~~~~~ 添加self""",
-        "Fault Case": """1.nn.Cell 官方文档:
-                   https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
-                   2.缺少self参数报错案例:
-                   https://bbs.huaweicloud.com/forum/thread-178902-1-1.html""",
-        "Test Case": "test_compiler_no_self.py"},
-    # Different versions have different error descriptions, and the ID is used repeatedly
-    {
-        "ID": "compiler_id_1",
-        "Fault Name": "construct 参数错误 >2.0",
-        "Key Log Information": "For 'Cell', the method 'construct' must have parameter 'self'",
-        "Key Python Stack Information": "",
-        "Key C++ Stack Information": "",
-        "Fault Cause": "继承nn.Cell类，重定义construct函数时，缺少self参数报错",
-        "Error Case": """
-                  def construct(a,b):
-                                ^~~~~~~ 此处缺少了self""",
-        "Modification Suggestion": "修改construct定义,添加self参数.",
-        "Fixed Case": """
-                  def construct(self,a,b):
-                                  ^~~~~~~ 添加self""",
-        "Fault Case": """1.nn.Cell 官方文档:
-               https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
-               2.缺少self参数报错案例:
-               https://bbs.huaweicloud.com/forum/thread-178902-1-1.html""",
-        "Test Case": "test_compiler_no_self.py"},
-
-    {
-         "ID": "compiler_id_2",
-         "Fault Name":"construct 参数错误",
-         "Key Log Information":"For 'Cell', the function construct .* positional argument, but got .*",
-         "Key Python Stack Information":"",
-         "Key C++ Stack Information":"",
-         "Fault Cause":"继承nn.Cell类，重定义construct函数时，定义参数个数与调用时输入参数不匹配报错",
-         "Error Case":"""
-                         class Net_LessInput(Cell):
-                           def construct(self,x,y):
-                              return x + y
-                         net = Net_LessInput()
-                         out = net(1)
-                                   ^~~~~~~ 此处缺少1个输入参数""",
-         "Modification Suggestion":"检查construct函数定义参数与调用输入参数，如果参数不匹配，"
-                                   "请根据情况修改参数定义或输入参数。",
-         "Fixed Case":"""
-                        class Net_LessInput(Cell):
-                         def construct(self,x,y):
-                             return x + y
-                        net = Net_LessInput()
-                        out = net(1,2)
-                                   ^~~~~~~ 此处增加1个输入参数""",
-         "Fault Case":"""1.nn.Cell官方文档：
-                      https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
-                      2.参考缺少self参数报错案例：
-                      https://bbs.huaweicloud.com/forum/thread-178902-1-1.html"""},
-    {
-        "ID": "compiler_id_3",
-        "Fault Name":"construct 参数错误",
-        "Key Log Information":"construct\(\) missing [1-9] required positional argument.*",
-        "Key Python Stack Information":"",
-        "Key C++ Stack Information":"",
-        "Fault Cause":"继承nn.Cell类，重定义construct函数时，定义参数个数与调用时输入参数不匹配报错",
-        "Error Case":"""
-                     class Net_LessInput(Cell):
-                       def construct(self,x,y):
-                          return x + y
-                     net = Net_LessInput()
-                     out = net(1)
-                               ^~~~~~~ 此处缺少1个输入参数""",
-        "Modification Suggestion":"检查construct函数定义参数与调用输入参数，如果参数不匹配，"
-                                  "请根据情况修改参数定义或输入参数。",
-        "Fixed Case":"""
-                    class Net_LessInput(Cell):
-                     def construct(self,x,y):
-                         return x + y
-                    net = Net_LessInput()
-                    out = net(1,2)
-                               ^~~~~~~ 此处增加1个输入参数""",
-        "Fault Case":"""1.nn.Cell官方文档：
-                  https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
-                  2.参考缺少self参数报错案例：
-                  https://bbs.huaweicloud.com/forum/thread-178902-1-1.html"""},
-    {
-         "ID": "compiler_id_4",
-         "Fault Name":"construct 参数错误",
-         "Key Log Information":"For 'Cell', the function construct .* [1-9] positional argument and "
-                             "[0-9] default argument, total .*",
-         "Key Python Stack Information":"",
-         "Key C++ Stack Information":"",
-         "Fault Cause":"继承nn.Cell类，重定义construct函数时，定义参数个数与调用时输入参数不匹配报错",
-         "Error Case":"""
-                    class Net_MoreInput(Cell):
-                       def construct(self,x):
-                           return x
-                     net = Net_MoreInput()
-                     out = net(1, 2)
-                                  ^~~~~~~ 此处多1个输入参数""",
-         "Modification Suggestion":"检查construct函数定义参数与调用输入参数，如果参数不匹配，请根据情况修改参数定义或输入参数。",
-         "Fixed Case":"""
-                     class Net_MoreInput(Cell):
-                       def construct(self,x):
-                           return x
-                     net = Net_MoreInput()
-                     out = net(1)
-                               ^~~~~~~ 此处去掉1个输入参数""",
-         "Fault Case":"""1.nn.Cell官方文档:
-                  https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
-                  2.参考缺少self参数报错案例:
-                  https://bbs.huaweicloud.com/forum/thread-178902-1-1.html"""},
-    {
-        "ID": "compiler_id_5",
-        "Fault Name":"construct 参数错误",
-        "Key Log Information":"construct\(\) takes [1-9] positional arguments but [0-9] were given",
-        "Key Python Stack Information":"",
-        "Key C++ Stack Information":"",
-        "Fault Cause":"继承nn.Cell类，重定义construct函数时，定义参数个数与调用时输入参数不匹配报错",
-        "Error Case":"""
-                class Net_MoreInput(Cell):
-                   def construct(self,x):
-                       return x
-                 net = Net_MoreInput()
-                 out = net(1, 2)
-                              ^~~~~~~ 此处多1个输入参数""",
-        "Modification Suggestion":"检查construct函数定义参数与调用输入参数，如果参数不匹配，请根据情况修改参数定义或输入参数。",
-        "Fixed Case":"""
-                 class Net_MoreInput(Cell):
-                   def construct(self,x):
-                       return x
-                 net = Net_MoreInput()
-                 out = net(1)
-                           ^~~~~~~ 此处去掉1个输入参数""",
-        "Fault Case":"""1.nn.Cell官方文档:
-              https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
-              2.参考缺少self参数报错案例:
-              https://bbs.huaweicloud.com/forum/thread-178902-1-1.html"""},
-    {
-     "ID": "compiler_id_6",
-     "Fault Name": "自定义接口参数错误",
-     "Key Log Information": ".* parameters number of the function is .*but .*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "自定义函数参数定义列表，与函数输入参数列表不匹配引起报错",
-     "Error Case": """
-                    class Net(nn.Cell):
-                        ...
-                        def func(x, y):
-                            return self.div(x, y)
-                        def construct(self, x, y):
-                            a=self.sub(x, 1)
-                            b=self.add(a, y)
-                            c=self.mul(self.func(a,a,b),b)
-                                            ^~~~~~~~~~参数与函数定义不匹配
-                            return c""",
-     "Modification Suggestion": "参考函数定义，修改自定义函数调用参数",
-     "Fixed Case": """
-                    class Net(nn.Cell):
-                        ...
-                        def func(x, y):
-                            return self.div(x, y)
-                        def construct(self, x, y):
-                            a=self.sub(x, 1)
-                            b=self.add(a, y)
-                            c=self.mul(self.func(a,b),b)
-                                            ^~~~~~~~~~修改参数与函数定义匹配
-                            return c""",
-     "Fault Case": """1.使用analyze_fail.dat分析函数参数错误案例:
-                     https://www.mindspore.cn/docs/programming_guide/zh-CN/r1.6/read_ir_files.html#analyze-fail-dat"""},
-    {
-        "ID": "compiler_id_7",
-        "Fault Name": "自定义接口参数错误",
-        "Key Log Information": ".* takes . positional arguments but . were given",
-        "Key Python Stack Information": "",
-        "Key C++ Stack Information": "",
-        "Fault Cause": "自定义函数参数定义列表，与函数输入参数列表不匹配引起报错",
-        "Error Case": """
-                    class Net(nn.Cell):
-                        ...
-                        def func(x, y):
-                            return self.div(x, y)
-                        def construct(self, x, y):
-                            a=self.sub(x, 1)
-                            b=self.add(a, y)
-                            c=self.mul(b,self.func(a,a,b))
-                                            ^~~~~~~~~~参数与函数定义不匹配
-                            return c""",
-        "Modification Suggestion": "参考函数定义，修改自定义函数调用参数.",
-        "Fixed Case": """
-                    class Net(nn.Cell):
-                        ...
-                        def func(x, y):
-                            return self.div(x, y)
-                        def construct(self, x, y):
-                            a=self.sub(x, 1)
-                            b=self.add(a, y)
-                            c=self.mul(b, self.func(a,b))
-                                            ^~~~~~~~~~修改参数与函数定义匹配
-                            return c""",
-        "Fault Case":"1.使用analyze_fail.dat分析函数参数错误案例: "
-                     "https://www.mindspore.cn/docs/programming_guide/zh-CN/r1.6/read_ir_files.html#analyze-fail-dat"},
-    {
-     "ID": "compiler_id_8",
-     "Fault Name": "抽象类型合并失败",
-     "Key Log Information": "Type Join Failed: dtype1 = .*, dtype2 = .*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "静态图的控制流(例如:if...else...)语法要求不同分支返回值的类型必须相同，不相同时(例如：Float32与Float16)会报错。",
-     "Error Case" : """
-                       def construct(self, x, a, b):
-                         if a > b:
-                           return self.relu(x)
-                         else:
-                           # dtype:Float32 -> Float16
-                         return self.cast(self.relu(x), ms.float16)
-                             ^~~~~~~ 返回值类型与if分支不一致""",
-     "Modification Suggestion": "检查不同分支的返回结果的类型，如果类型不相同，请修改至相同类型。",
-     "Fault Case": """1.编译时报错Type Join Failed案例:
-                   https://www.mindspore.cn/docs/faq/zh-CN/r1.6/network_compilation.html"""},
-    {
-     "ID": "compiler_id_9",
-     "Fault Name": "抽象类型合并失败",
-     "Key Log Information": "Shape Join Failed: shape1 = .*, shape2 = .*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "静态图的控制流(例如:if...else...)语法要求不同分支返回值的shape相同，不相同时会报错。",
-     "Error Case": """
-                     def construct(self, x, a, b):
-                         if a > b:
-                             return self.relu(x)
-                         else:
-                             # shape: (*)->()
-                             return self.reducesum(x)
-                                 ^~~~~~~返回值shape与if分支不一致 """,
-     "Modification Suggestion": "检查不同分支的返回结果的shape，如果不相同，请修改至相同shape",
-     "Fault Case": """1.编译时报错Shape Join Failed案例:
-                   https://www.mindspore.cn/docs/faq/zh-CN/r1.6/network_compilation.html
-                   2.静态图语法：
-                   https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html"""},
-    {
-     "ID": "compiler_id_10",
-     "Fault Name": "抽象类型合并失败",
-     "Key Log Information": "Abstract type .* cannot join with .*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "对函数输出求梯度时，抽象类型不匹配，导致抽象类型合并失败",
-     "Error Case": """
-                    grad = ops.GradOperation(sens_param=True)
-                    # test_net输出类型为tuple(Tensor, Tensor)
-                    def test_net(a, b):
-                      return a, b
-                    _type=ops.DType()
-                    _shape=ops.Shape()
-                    @ms_function()
-                    def join_fail(x, y):
-                      sens_i=ops.Fill()(_type(x),_shape(x),1.0)
-                      a=grad(test_net)(x,y,sens_i)
-                                           ^~~~sens_i类型为Tensor
-                      return a
-
-                    x = Tensor([1.0])
-                    y = Tensor([2.0])
-                    join_fail(x,y)""",
-     "Modification Suggestion": "检查求梯度的函数的输出类型与sens_param的类型是否相同，如果不相同，修改为相同类型.",
-     "Fixed Case":"""
-                  grad = ops.GradOperation(sens_param=True)
-                  # test_net输出类型为tuple(Tensor, Tensor)
-                  def test_net(a, b):
-                    return a, b
-                  _type=ops.DType()
-                  _shape=ops.Shape()
-                  @ms_function()
-                  def join_fail(x, y):
-                    sens_i=ops.Fill()(_type(x),_shape(x),1.0)
-                    sens=(sens_i, sens_i) #
-                    a=grad(test_net)(x,y,sens)
-                                         ^~~~sens类型为tuple
-                    return a
-                  x = Tensor([1.0])
-                  y = Tensor([2.0])
-                  join_fail(x,y)""",
-     "Fault Case": """1.自动求导报错Type Join Failed案例:
-               https://www.mindspore.cn/docs/faq/zh-CN/r1.6/network_compilation.html""" },
-    {
-     "ID": "compiler_id_11",
-     "Fault Name": "静态图找不到属性-1.8.1",
-     "Key Log Information": "operation does not support the type",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "GenerateFromTypes",
-     "Fault Cause": "静态图语法使用未定义的变量报错",
-     "Error Case": """
-                      class Net(nn.Cell):
-                        def construct(self, x):
-                          return x + self.y
-                                        ^~~~~~~ self.y未定义""",
-     "Modification Suggestion": "定位到报错代码行，如果变量未定义，可以在__init__方法中初始化。",
-     "Fixed Case": """
-                      class Net(nn.Cell):
-                        def __init__(self):
-                          super(Net, self).__init__()
-                          self.y = 1.0
-                             ^~~~~~~ 对self.y初始化
-                        def construct(self, x):
-                          return x + self.y""",
-     "Fault Case": "1.静态图语法： "
-                   "https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html "
-                   "2.使用未定义变量报错案例： "
-                   "https://bbs.huaweicloud.com/forum/thread-180857-1-1.html",
-     "Test Case": "test_compiler_kmetatypenone.py"},
-    {
-        "ID": "compiler_id_12",
-        "Fault Name": "静态图找不到属性-1.9",
-        "Key Log Information": "External object has no attribute",
-        "Key Python Stack Information": "",
-        "Key C++ Stack Information": "GetEvaluatedValueForNameSpaceString",
-        "Fault Cause": "静态图语法使用未定义的变量报错",
-        "Error Case": """
-                  class Net(nn.Cell):
-                    def construct(self, x):
-                      return x + self.y
-                                    ^~~~~~~ self.y未定义""",
-        "Modification Suggestion": "定位到报错代码行，如果变量未定义，可以在__init__方法中初始化。",
-        "Fixed Case": """
-                  class Net(nn.Cell):
-                    def __init__(self):
-                      super(Net, self).__init__()
-                      self.y = 1.0
-                         ^~~~~~~ 对self.y初始化
-                    def construct(self, x):
-                      return x + self.y""",
-        "Fault Case": "1.静态图语法： "
-                      "https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html "
-                      "2.使用未定义变量报错案例： "
-                      "https://bbs.huaweicloud.com/forum/thread-180857-1-1.html",
-        "Test Case": "test_compiler_kmetatypenone.py"},
-    {
-     "ID": "compiler_id_13",
-     "Fault Name": "函数调用栈超限",
-     "Key Log Information": "Exceed function call depth limit",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "函数嵌套调用存在死循环或者嵌套调用深度超过限制而引起报错",
-     "Modification Suggestion": "1.检查代码中是否存在无穷递归或死循环，简化代码逻辑减少函数循环嵌套调用 "
-                                "2.使用context.set_context(max_call_depth=value)方法，修改函数调用栈最大深度限制。",
-     "Fault Case": "1.GRU算子参数过大引起栈超限制案例: "
-                   "https://bbs.huaweicloud.com/forum/thread-182256-1-1.html"},
-    {
-     "ID": "compiler_id_14",
-     "Fault Name": "JIT Fallback 使用错误",
-     "Key Log Information": "not use Python object in runtime",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "JIT Fallback暂不支持Runtime阶段解析执行代码",
-     "Error Case": """
-                    @ms_function
-                    def test_np_add():
-                        x = np.array([1, 2, 3, 4, 5])
-                        y = np.array([1, 2, 3, 4, 5])
-                        return np.add(x, y)
-                                    ^~~~~~不支持的语法作为函数返回值报错""",
-     "Modification Suggestion": "静态图模式下不支持的语法，将会生成解释节点，避免将解释节点传递到运行时。",
-     "Fixed Case":"""
-                    @ms_function
-                    def test_np_add():
-                        x = np.array([1, 2, 3, 4, 5])
-                        y = np.array([1, 2, 3, 4, 5])
-                        z = Tensor(np.add(x, y))
-                                      ^~~~不支持的语法，在编译期执行。
-                        return z""",
-     "Fault Case": "1.JIT Fallback使用说明： "
-                   "https://www.mindspore.cn/docs/programming_guide/zh-CN/r1.6/jit_fallback.html"},
-    {
-     "ID": "compiler_id_15",
-     "Fault Name": "使用自定义class的属性与方法-1.8",
-     "Key Log Information": "Not supported to get attribute for InterpretedObject.*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "静态图语法不支持自定义class的属性与方法， 在construct函数中使用出现报错",
-     "Error Case":"""
-                    class LayerParams:
-                        def get_weights(self, shape):
-                            ...
-                            nn_param=mindspore.Parameter(nn_param)
-                            return nn_param
-                    class MyCell(nn.Cell):
-                        def __init__(self):
-                            super().__init__()
-                            self._params=LayerParams(...)
-                        def _fc(self, inputs, output_size):
-                            width=inputs.shape[-1]
-                            weight=self._params.get_weights(...)
-                                                ^~~~~~~~~~~不支持
-                            return weight
-                    def construct(self, x, output_size):
-                        weight = self._fc(x, output_size)
-                        ...""",
-     "Modification Suggestion": "当前版本不支持使用自定义类的属性与方法，请修改自定义类方法，或尝试使用最新版本。",
-     "Fault Case": "1.静态图语法支持： "
-                   "https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html"},
-    {
-        "ID": "compiler_id_16",
-        "Fault Name": "使用自定义class的属性与方法-1.9",
-        "Key Log Information": "Do not support to get attribute from .* object .*",
-        "Key Python Stack Information": "",
-        "Key C++ Stack Information": "StaticGetter",
-        "Fault Cause": "静态图语法不支持调用自定义class的属性与方法， 在construct函数中使用出现报错",
-        "Error Case": """
-                class LayerParams:
-                    def get_weights(self, shape):
-                        ...
-                        nn_param=mindspore.Parameter(nn_param)
-                        return nn_param
-                class MyCell(nn.Cell):
-                    def __init__(self):
-                        super().__init__()
-                        self._params=LayerParams(...)
-                    def _fc(self, inputs, output_size):
-                        width=inputs.shape[-1]
-                        weight=self._params.get_weights(...)
-                                            ^~~~~~~~~~~不支持
-                        return weight
-                def construct(self, x, output_size):
-                    weight = self._fc(x, output_size)
-                    ...""",
-        "Modification Suggestion": "当前版本不支持使用自定义类的属性与方法，请修改自定义类方法，或尝试使用最新版本。",
-        "Fault Case": "1.静态图语法支持： "
-                      "https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html"},
-    {
-     "ID": "compiler_id_17",
-     "Fault Name": "静态图代码缩进错误",
-     "Key Log Information": "incorrect indentations in definition or comment",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "可能是静态图语法中代码行或者注释的缩进没有对齐，引起报错",
-     "Error Case":"""
-                class Net(nn.Cell):
-                    def __init__(self):
-                        super(Net, self).__init__()
-                        self.y = 2.0
-                    def construct(self, x):
-                #       x + 2.0
-                ^~~~~~~~~~~~~~注释行没有对齐
-                        return x + self.y""",
-     "Modification Suggestion": "修改缩进没有对齐的代码行或者注释行，使对齐。",
-     "Fixed Case":"""
-                class Net(nn.Cell):
-                    def __init__(self):
-                        super(Net, self).__init__()
-                        self.y = 2.0
-                    def construct(self, x):
-                        # x + 2.0
-                        ^~~~~~~~~~~~~~修改注释行对齐
-                        return x + self.y""",
-     "Fault Case": """1.静态图语法： 
-                   https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html"""},
-    {
-     "ID": "compiler_id_18",
-     "Fault Name": "Parameter重名报错",
-     "Key Log Information":"value.* Parameter (.*) , its name .* already exists.",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "在一个神经网络内，Parameter出现了重名参数而引起报错，需要修改参数名称。",
-     "Modification Suggestion":"1.如果是一个网络有多个参数Parameter对象，需要修改重名的Parameter的名称； "
-                               "2.如果是一个网络使用PrameterTuple时，需要指定其内部的Parameter为不同名称； "
-                               "3.如果是2个或以上的网络使用了PrameterTuple, 需要使用CellList来避免重名; "
-                               "4.如果存在多个Cell，可以使用Cell.update_parameters_name()增加参数名称前缀，避免重名。",
-      "Fault Case":"1. mindspore.Parameter接口: "
-                   "https://www.mindspore.cn/docs/zh-CN/r1.8/api_python/mindspore/mindspore.Parameter.html "
-                   "2. mindspore.PrameterTuple接口： "
-                   "https://www.mindspore.cn/docs/zh-CN/r1.8/api_python/mindspore/mindspore.ParameterTuple.html "},
-    {
-        "ID": "compiler_id_19",
-        "Fault Name": "静态图模式下使用了错误的框架API",
-        "Key Log Information": "Unsupported statement \'Try\'",
-        "Key Python Stack Information": "",
-        "Key C++ Stack Information": "ParseStatement",
-        "Fault Cause": "静态图模式下网络的construct函数、@ms_function修饰的函数或@ms.jit修饰的函数中出现如下问题： "
-                       "1）直接或者间接使用了try语法，此语法静态图模式不支持; "
-                       "2）直接或间接的调用了MindSpore的get_context接口（get_context接口会使用try语法），此接口不能在construct "
-                       "等函数中调用; ",
-        "Modification Suggestion": "1）找到函数中直接或者间接使用了try语法, 将try语法在函数中移除; "
-                                   "2）函数中调用的get_context()接口，迁移到函数外调用; "
-                                   "3）如果没发现调用函数位置，则可能为函数多级调用或者框架内部多级调用，可去社区提单求助",
-        "Fault Case": "1.静态图语法支持： "
-                      "https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html "}
-]
-
-compiler_general_experience_list_cn = [
-    {
-     "ID": "compiler_g_id_1",
-     "Fault Name": "静态图类型推导问题",
-     "Key Log Information": "Get instructions about .analyze_fail.dat.",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Code Path":"",
-     "Fault Cause": "可能为静态图的语法编译错误，包括数据类型、原型操作、运算符、复合语句、函数等使用的问题。",
-     "Modification Suggestion": "1.根据报错信息，分析编译报错的类型； "
-                                "2.针对报错的类型，查看官网静态图语法支持介绍，分析报错的原因; "
-                                "3.使用analyze_fail.dat文件分析静态图编译结果，定位报错的代码行，分析报错原因。 ",
-     "Fault Case": "1.图编译语法支持： "
-                   " https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html "
-                   "2.错误分析方法： "
-                   "https://www.mindspore.cn/tutorials/experts/zh-CN/r1.8/debug/error_analyze.html "
-                   "3.analyze_fail.dat文件分析网络编译失败原因： "
-                   "https://www.mindspore.cn/tutorials/experts/zh-CN/r1.8/debug/mindir.html"
-                   "4.中间表达MindIR "
-                   "https://www.mindspore.cn/docs/zh-CN/r1.8/design/mindir.html"
-                   "5.社区论坛-功能调试案例集： "
-                   "https://bbs.huaweicloud.com/forum/forum-1076-2704-1.html "},
-    {
-     "ID": "compiler_g_id_2",
-     "Fault Name": "静态图编译问题",
-     "Key Log Information": "",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "mindspore.*\.cc",
-     "Code Path": "mindspore.core.abstract;mindspore.ccsrc.pipeline.jit",
-     "Fault Cause": "可能为静态图的语法编译错误，包括数据类型、原型操作、运算符、复合语句、函数等使用的问题。",
-     "Modification Suggestion": "1.根据报错信息，分析编译报错的类型； "
-                                "2.针对报错的类型，查看官网静态图语法支持介绍，分析报错的原因; ",
-     "Fault Case": "1.图编译语法支持： "
-                   " https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html "}
-]
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+
+compiler_experience_list_cn = [
+    {
+        "ID": "compiler_id_1",
+        "Fault Name": "construct 参数错误 <2.0",
+        "Key Log Information": "For 'Cell', the function construct .* 0 positional argument and 0 default argument",
+        "Key Python Stack Information": "",
+        "Key C++ Stack Information": "",
+        "Fault Cause": "继承nn.Cell类，重定义construct函数时，缺少self参数报错",
+        "Error Case": """
+                      def construct(a,b):
+                                    ^~~~~~~ 此处缺少了self""",
+        "Modification Suggestion": "修改construct定义,添加self参数.",
+        "Fixed Case": """
+                      def construct(self,a,b):
+                                      ^~~~~~~ 添加self""",
+        "Fault Case": """1.nn.Cell 官方文档:
+                   https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
+                   2.缺少self参数报错案例:
+                   https://bbs.huaweicloud.com/forum/thread-178902-1-1.html""",
+        "Test Case": "test_compiler_no_self.py"},
+    # Different versions have different error descriptions, and the ID is used repeatedly
+    {
+        "ID": "compiler_id_1",
+        "Fault Name": "construct 参数错误 >2.0",
+        "Key Log Information": "For 'Cell', the method 'construct' must have parameter 'self'",
+        "Key Python Stack Information": "",
+        "Key C++ Stack Information": "",
+        "Fault Cause": "继承nn.Cell类，重定义construct函数时，缺少self参数报错",
+        "Error Case": """
+                  def construct(a,b):
+                                ^~~~~~~ 此处缺少了self""",
+        "Modification Suggestion": "修改construct定义,添加self参数.",
+        "Fixed Case": """
+                  def construct(self,a,b):
+                                  ^~~~~~~ 添加self""",
+        "Fault Case": """1.nn.Cell 官方文档:
+               https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
+               2.缺少self参数报错案例:
+               https://bbs.huaweicloud.com/forum/thread-178902-1-1.html""",
+        "Test Case": "test_compiler_no_self.py"},
+
+    {
+         "ID": "compiler_id_2",
+         "Fault Name":"construct 参数错误",
+         "Key Log Information":"For 'Cell', the function construct .* positional argument, but got .*",
+         "Key Python Stack Information":"",
+         "Key C++ Stack Information":"",
+         "Fault Cause":"继承nn.Cell类，重定义construct函数时，定义参数个数与调用时输入参数不匹配报错",
+         "Error Case":"""
+                         class Net_LessInput(Cell):
+                           def construct(self,x,y):
+                              return x + y
+                         net = Net_LessInput()
+                         out = net(1)
+                                   ^~~~~~~ 此处缺少1个输入参数""",
+         "Modification Suggestion":"检查construct函数定义参数与调用输入参数，如果参数不匹配，"
+                                   "请根据情况修改参数定义或输入参数。",
+         "Fixed Case":"""
+                        class Net_LessInput(Cell):
+                         def construct(self,x,y):
+                             return x + y
+                        net = Net_LessInput()
+                        out = net(1,2)
+                                   ^~~~~~~ 此处增加1个输入参数""",
+         "Fault Case":"""1.nn.Cell官方文档：
+                      https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
+                      2.参考缺少self参数报错案例：
+                      https://bbs.huaweicloud.com/forum/thread-178902-1-1.html"""},
+    {
+        "ID": "compiler_id_3",
+        "Fault Name":"construct 参数错误",
+        "Key Log Information":"construct\(\) missing [1-9] required positional argument.*",
+        "Key Python Stack Information":"",
+        "Key C++ Stack Information":"",
+        "Fault Cause":"继承nn.Cell类，重定义construct函数时，定义参数个数与调用时输入参数不匹配报错",
+        "Error Case":"""
+                     class Net_LessInput(Cell):
+                       def construct(self,x,y):
+                          return x + y
+                     net = Net_LessInput()
+                     out = net(1)
+                               ^~~~~~~ 此处缺少1个输入参数""",
+        "Modification Suggestion":"检查construct函数定义参数与调用输入参数，如果参数不匹配，"
+                                  "请根据情况修改参数定义或输入参数。",
+        "Fixed Case":"""
+                    class Net_LessInput(Cell):
+                     def construct(self,x,y):
+                         return x + y
+                    net = Net_LessInput()
+                    out = net(1,2)
+                               ^~~~~~~ 此处增加1个输入参数""",
+        "Fault Case":"""1.nn.Cell官方文档：
+                  https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
+                  2.参考缺少self参数报错案例：
+                  https://bbs.huaweicloud.com/forum/thread-178902-1-1.html"""},
+    {
+         "ID": "compiler_id_4",
+         "Fault Name":"construct 参数错误",
+         "Key Log Information":"For 'Cell', the function construct .* [1-9] positional argument and "
+                             "[0-9] default argument, total .*",
+         "Key Python Stack Information":"",
+         "Key C++ Stack Information":"",
+         "Fault Cause":"继承nn.Cell类，重定义construct函数时，定义参数个数与调用时输入参数不匹配报错",
+         "Error Case":"""
+                    class Net_MoreInput(Cell):
+                       def construct(self,x):
+                           return x
+                     net = Net_MoreInput()
+                     out = net(1, 2)
+                                  ^~~~~~~ 此处多1个输入参数""",
+         "Modification Suggestion":"检查construct函数定义参数与调用输入参数，如果参数不匹配，请根据情况修改参数定义或输入参数。",
+         "Fixed Case":"""
+                     class Net_MoreInput(Cell):
+                       def construct(self,x):
+                           return x
+                     net = Net_MoreInput()
+                     out = net(1)
+                               ^~~~~~~ 此处去掉1个输入参数""",
+         "Fault Case":"""1.nn.Cell官方文档:
+                  https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
+                  2.参考缺少self参数报错案例:
+                  https://bbs.huaweicloud.com/forum/thread-178902-1-1.html"""},
+    {
+        "ID": "compiler_id_5",
+        "Fault Name":"construct 参数错误",
+        "Key Log Information":"construct\(\) takes [1-9] positional arguments but [0-9] were given",
+        "Key Python Stack Information":"",
+        "Key C++ Stack Information":"",
+        "Fault Cause":"继承nn.Cell类，重定义construct函数时，定义参数个数与调用时输入参数不匹配报错",
+        "Error Case":"""
+                class Net_MoreInput(Cell):
+                   def construct(self,x):
+                       return x
+                 net = Net_MoreInput()
+                 out = net(1, 2)
+                              ^~~~~~~ 此处多1个输入参数""",
+        "Modification Suggestion":"检查construct函数定义参数与调用输入参数，如果参数不匹配，请根据情况修改参数定义或输入参数。",
+        "Fixed Case":"""
+                 class Net_MoreInput(Cell):
+                   def construct(self,x):
+                       return x
+                 net = Net_MoreInput()
+                 out = net(1)
+                           ^~~~~~~ 此处去掉1个输入参数""",
+        "Fault Case":"""1.nn.Cell官方文档:
+              https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Cell.html
+              2.参考缺少self参数报错案例:
+              https://bbs.huaweicloud.com/forum/thread-178902-1-1.html"""},
+    {
+     "ID": "compiler_id_6",
+     "Fault Name": "自定义接口参数错误",
+     "Key Log Information": ".* parameters number of the function is .*but .*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "自定义函数参数定义列表，与函数输入参数列表不匹配引起报错",
+     "Error Case": """
+                    class Net(nn.Cell):
+                        ...
+                        def func(x, y):
+                            return self.div(x, y)
+                        def construct(self, x, y):
+                            a=self.sub(x, 1)
+                            b=self.add(a, y)
+                            c=self.mul(self.func(a,a,b),b)
+                                            ^~~~~~~~~~参数与函数定义不匹配
+                            return c""",
+     "Modification Suggestion": "参考函数定义，修改自定义函数调用参数",
+     "Fixed Case": """
+                    class Net(nn.Cell):
+                        ...
+                        def func(x, y):
+                            return self.div(x, y)
+                        def construct(self, x, y):
+                            a=self.sub(x, 1)
+                            b=self.add(a, y)
+                            c=self.mul(self.func(a,b),b)
+                                            ^~~~~~~~~~修改参数与函数定义匹配
+                            return c""",
+     "Fault Case": """1.使用analyze_fail.dat分析函数参数错误案例:
+                     https://www.mindspore.cn/docs/programming_guide/zh-CN/r1.6/read_ir_files.html#analyze-fail-dat"""},
+    {
+        "ID": "compiler_id_7",
+        "Fault Name": "自定义接口参数错误",
+        "Key Log Information": ".* takes . positional arguments but . were given",
+        "Key Python Stack Information": "",
+        "Key C++ Stack Information": "",
+        "Fault Cause": "自定义函数参数定义列表，与函数输入参数列表不匹配引起报错",
+        "Error Case": """
+                    class Net(nn.Cell):
+                        ...
+                        def func(x, y):
+                            return self.div(x, y)
+                        def construct(self, x, y):
+                            a=self.sub(x, 1)
+                            b=self.add(a, y)
+                            c=self.mul(b,self.func(a,a,b))
+                                            ^~~~~~~~~~参数与函数定义不匹配
+                            return c""",
+        "Modification Suggestion": "参考函数定义，修改自定义函数调用参数.",
+        "Fixed Case": """
+                    class Net(nn.Cell):
+                        ...
+                        def func(x, y):
+                            return self.div(x, y)
+                        def construct(self, x, y):
+                            a=self.sub(x, 1)
+                            b=self.add(a, y)
+                            c=self.mul(b, self.func(a,b))
+                                            ^~~~~~~~~~修改参数与函数定义匹配
+                            return c""",
+        "Fault Case":"1.使用analyze_fail.dat分析函数参数错误案例: "
+                     "https://www.mindspore.cn/docs/programming_guide/zh-CN/r1.6/read_ir_files.html#analyze-fail-dat"},
+    {
+     "ID": "compiler_id_8",
+     "Fault Name": "抽象类型合并失败",
+     "Key Log Information": "Type Join Failed: dtype1 = .*, dtype2 = .*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "静态图的控制流(例如:if...else...)语法要求不同分支返回值的类型必须相同，不相同时(例如：Float32与Float16)会报错。",
+     "Error Case" : """
+                       def construct(self, x, a, b):
+                         if a > b:
+                           return self.relu(x)
+                         else:
+                           # dtype:Float32 -> Float16
+                         return self.cast(self.relu(x), ms.float16)
+                             ^~~~~~~ 返回值类型与if分支不一致""",
+     "Modification Suggestion": "检查不同分支的返回结果的类型，如果类型不相同，请修改至相同类型。",
+     "Fault Case": """1.编译时报错Type Join Failed案例:
+                   https://www.mindspore.cn/docs/faq/zh-CN/r1.6/network_compilation.html"""},
+    {
+     "ID": "compiler_id_9",
+     "Fault Name": "抽象类型合并失败",
+     "Key Log Information": "Shape Join Failed: shape1 = .*, shape2 = .*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "静态图的控制流(例如:if...else...)语法要求不同分支返回值的shape相同，不相同时会报错。",
+     "Error Case": """
+                     def construct(self, x, a, b):
+                         if a > b:
+                             return self.relu(x)
+                         else:
+                             # shape: (*)->()
+                             return self.reducesum(x)
+                                 ^~~~~~~返回值shape与if分支不一致 """,
+     "Modification Suggestion": "检查不同分支的返回结果的shape，如果不相同，请修改至相同shape",
+     "Fault Case": """1.编译时报错Shape Join Failed案例:
+                   https://www.mindspore.cn/docs/faq/zh-CN/r1.6/network_compilation.html
+                   2.静态图语法：
+                   https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html"""},
+    {
+     "ID": "compiler_id_10",
+     "Fault Name": "抽象类型合并失败",
+     "Key Log Information": "Abstract type .* cannot join with .*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "对函数输出求梯度时，抽象类型不匹配，导致抽象类型合并失败",
+     "Error Case": """
+                    grad = ops.GradOperation(sens_param=True)
+                    # test_net输出类型为tuple(Tensor, Tensor)
+                    def test_net(a, b):
+                      return a, b
+                    _type=ops.DType()
+                    _shape=ops.Shape()
+                    @ms_function()
+                    def join_fail(x, y):
+                      sens_i=ops.Fill()(_type(x),_shape(x),1.0)
+                      a=grad(test_net)(x,y,sens_i)
+                                           ^~~~sens_i类型为Tensor
+                      return a
+
+                    x = Tensor([1.0])
+                    y = Tensor([2.0])
+                    join_fail(x,y)""",
+     "Modification Suggestion": "检查求梯度的函数的输出类型与sens_param的类型是否相同，如果不相同，修改为相同类型.",
+     "Fixed Case":"""
+                  grad = ops.GradOperation(sens_param=True)
+                  # test_net输出类型为tuple(Tensor, Tensor)
+                  def test_net(a, b):
+                    return a, b
+                  _type=ops.DType()
+                  _shape=ops.Shape()
+                  @ms_function()
+                  def join_fail(x, y):
+                    sens_i=ops.Fill()(_type(x),_shape(x),1.0)
+                    sens=(sens_i, sens_i) #
+                    a=grad(test_net)(x,y,sens)
+                                         ^~~~sens类型为tuple
+                    return a
+                  x = Tensor([1.0])
+                  y = Tensor([2.0])
+                  join_fail(x,y)""",
+     "Fault Case": """1.自动求导报错Type Join Failed案例:
+               https://www.mindspore.cn/docs/faq/zh-CN/r1.6/network_compilation.html""" },
+    {
+     "ID": "compiler_id_11",
+     "Fault Name": "静态图找不到属性-1.8.1",
+     "Key Log Information": "operation does not support the type",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "GenerateFromTypes",
+     "Fault Cause": "静态图语法使用未定义的变量报错",
+     "Error Case": """
+                      class Net(nn.Cell):
+                        def construct(self, x):
+                          return x + self.y
+                                        ^~~~~~~ self.y未定义""",
+     "Modification Suggestion": "定位到报错代码行，如果变量未定义，可以在__init__方法中初始化。",
+     "Fixed Case": """
+                      class Net(nn.Cell):
+                        def __init__(self):
+                          super(Net, self).__init__()
+                          self.y = 1.0
+                             ^~~~~~~ 对self.y初始化
+                        def construct(self, x):
+                          return x + self.y""",
+     "Fault Case": "1.静态图语法： "
+                   "https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html "
+                   "2.使用未定义变量报错案例： "
+                   "https://bbs.huaweicloud.com/forum/thread-180857-1-1.html",
+     "Test Case": "test_compiler_kmetatypenone.py"},
+    {
+        "ID": "compiler_id_12",
+        "Fault Name": "静态图找不到属性-1.9",
+        "Key Log Information": "External object has no attribute",
+        "Key Python Stack Information": "",
+        "Key C++ Stack Information": "GetEvaluatedValueForNameSpaceString",
+        "Fault Cause": "静态图语法使用未定义的变量报错",
+        "Error Case": """
+                  class Net(nn.Cell):
+                    def construct(self, x):
+                      return x + self.y
+                                    ^~~~~~~ self.y未定义""",
+        "Modification Suggestion": "定位到报错代码行，如果变量未定义，可以在__init__方法中初始化。",
+        "Fixed Case": """
+                  class Net(nn.Cell):
+                    def __init__(self):
+                      super(Net, self).__init__()
+                      self.y = 1.0
+                         ^~~~~~~ 对self.y初始化
+                    def construct(self, x):
+                      return x + self.y""",
+        "Fault Case": "1.静态图语法： "
+                      "https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html "
+                      "2.使用未定义变量报错案例： "
+                      "https://bbs.huaweicloud.com/forum/thread-180857-1-1.html",
+        "Test Case": "test_compiler_kmetatypenone.py"},
+    {
+     "ID": "compiler_id_13",
+     "Fault Name": "函数调用栈超限",
+     "Key Log Information": "Exceed function call depth limit",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "函数嵌套调用存在死循环或者嵌套调用深度超过限制而引起报错",
+     "Modification Suggestion": "1.检查代码中是否存在无穷递归或死循环，简化代码逻辑减少函数循环嵌套调用 "
+                                "2.使用context.set_context(max_call_depth=value)方法，修改函数调用栈最大深度限制。",
+     "Fault Case": "1.GRU算子参数过大引起栈超限制案例: "
+                   "https://bbs.huaweicloud.com/forum/thread-182256-1-1.html"},
+    {
+     "ID": "compiler_id_14",
+     "Fault Name": "JIT Fallback 使用错误",
+     "Key Log Information": "not use Python object in runtime",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "JIT Fallback暂不支持Runtime阶段解析执行代码",
+     "Error Case": """
+                    @ms_function
+                    def test_np_add():
+                        x = np.array([1, 2, 3, 4, 5])
+                        y = np.array([1, 2, 3, 4, 5])
+                        return np.add(x, y)
+                                    ^~~~~~不支持的语法作为函数返回值报错""",
+     "Modification Suggestion": "静态图模式下不支持的语法，将会生成解释节点，避免将解释节点传递到运行时。",
+     "Fixed Case":"""
+                    @ms_function
+                    def test_np_add():
+                        x = np.array([1, 2, 3, 4, 5])
+                        y = np.array([1, 2, 3, 4, 5])
+                        z = Tensor(np.add(x, y))
+                                      ^~~~不支持的语法，在编译期执行。
+                        return z""",
+     "Fault Case": "1.JIT Fallback使用说明： "
+                   "https://www.mindspore.cn/docs/programming_guide/zh-CN/r1.6/jit_fallback.html"},
+    {
+     "ID": "compiler_id_15",
+     "Fault Name": "使用自定义class的属性与方法-1.8",
+     "Key Log Information": "Not supported to get attribute for InterpretedObject.*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "静态图语法不支持自定义class的属性与方法， 在construct函数中使用出现报错",
+     "Error Case":"""
+                    class LayerParams:
+                        def get_weights(self, shape):
+                            ...
+                            nn_param=mindspore.Parameter(nn_param)
+                            return nn_param
+                    class MyCell(nn.Cell):
+                        def __init__(self):
+                            super().__init__()
+                            self._params=LayerParams(...)
+                        def _fc(self, inputs, output_size):
+                            width=inputs.shape[-1]
+                            weight=self._params.get_weights(...)
+                                                ^~~~~~~~~~~不支持
+                            return weight
+                    def construct(self, x, output_size):
+                        weight = self._fc(x, output_size)
+                        ...""",
+     "Modification Suggestion": "当前版本不支持使用自定义类的属性与方法，请修改自定义类方法，或尝试使用最新版本。",
+     "Fault Case": "1.静态图语法支持： "
+                   "https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html"},
+    {
+        "ID": "compiler_id_16",
+        "Fault Name": "使用自定义class的属性与方法-1.9",
+        "Key Log Information": "Do not support to get attribute from .* object .*",
+        "Key Python Stack Information": "",
+        "Key C++ Stack Information": "StaticGetter",
+        "Fault Cause": "静态图语法不支持调用自定义class的属性与方法， 在construct函数中使用出现报错",
+        "Error Case": """
+                class LayerParams:
+                    def get_weights(self, shape):
+                        ...
+                        nn_param=mindspore.Parameter(nn_param)
+                        return nn_param
+                class MyCell(nn.Cell):
+                    def __init__(self):
+                        super().__init__()
+                        self._params=LayerParams(...)
+                    def _fc(self, inputs, output_size):
+                        width=inputs.shape[-1]
+                        weight=self._params.get_weights(...)
+                                            ^~~~~~~~~~~不支持
+                        return weight
+                def construct(self, x, output_size):
+                    weight = self._fc(x, output_size)
+                    ...""",
+        "Modification Suggestion": "当前版本不支持使用自定义类的属性与方法，请修改自定义类方法，或尝试使用最新版本。",
+        "Fault Case": "1.静态图语法支持： "
+                      "https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html"},
+    {
+     "ID": "compiler_id_17",
+     "Fault Name": "静态图代码缩进错误",
+     "Key Log Information": "incorrect indentations in definition or comment",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "可能是静态图语法中代码行或者注释的缩进没有对齐，引起报错",
+     "Error Case":"""
+                class Net(nn.Cell):
+                    def __init__(self):
+                        super(Net, self).__init__()
+                        self.y = 2.0
+                    def construct(self, x):
+                #       x + 2.0
+                ^~~~~~~~~~~~~~注释行没有对齐
+                        return x + self.y""",
+     "Modification Suggestion": "修改缩进没有对齐的代码行或者注释行，使对齐。",
+     "Fixed Case":"""
+                class Net(nn.Cell):
+                    def __init__(self):
+                        super(Net, self).__init__()
+                        self.y = 2.0
+                    def construct(self, x):
+                        # x + 2.0
+                        ^~~~~~~~~~~~~~修改注释行对齐
+                        return x + self.y""",
+     "Fault Case": """1.静态图语法： 
+                   https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html"""},
+    {
+     "ID": "compiler_id_18",
+     "Fault Name": "Parameter重名报错",
+     "Key Log Information":"value.* Parameter (.*) , its name .* already exists.",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "在一个神经网络内，Parameter出现了重名参数而引起报错，需要修改参数名称。",
+     "Modification Suggestion":"1.如果是一个网络有多个参数Parameter对象，需要修改重名的Parameter的名称； "
+                               "2.如果是一个网络使用PrameterTuple时，需要指定其内部的Parameter为不同名称； "
+                               "3.如果是2个或以上的网络使用了PrameterTuple, 需要使用CellList来避免重名; "
+                               "4.如果存在多个Cell，可以使用Cell.update_parameters_name()增加参数名称前缀，避免重名。",
+      "Fault Case":"1. mindspore.Parameter接口: "
+                   "https://www.mindspore.cn/docs/zh-CN/r1.8/api_python/mindspore/mindspore.Parameter.html "
+                   "2. mindspore.PrameterTuple接口： "
+                   "https://www.mindspore.cn/docs/zh-CN/r1.8/api_python/mindspore/mindspore.ParameterTuple.html "},
+    {
+        "ID": "compiler_id_19",
+        "Fault Name": "静态图模式下使用了错误的框架API",
+        "Key Log Information": "Unsupported statement \'Try\'",
+        "Key Python Stack Information": "",
+        "Key C++ Stack Information": "ParseStatement",
+        "Fault Cause": "静态图模式下网络的construct函数、@ms_function修饰的函数或@ms.jit修饰的函数中出现如下问题： "
+                       "1）直接或者间接使用了try语法，此语法静态图模式不支持; "
+                       "2）直接或间接的调用了MindSpore的get_context接口（get_context接口会使用try语法），此接口不能在construct "
+                       "等函数中调用; ",
+        "Modification Suggestion": "1）找到函数中直接或者间接使用了try语法, 将try语法在函数中移除; "
+                                   "2）函数中调用的get_context()接口，迁移到函数外调用; "
+                                   "3）如果没发现调用函数位置，则可能为函数多级调用或者框架内部多级调用，可去社区提单求助",
+        "Fault Case": "1.静态图语法支持： "
+                      "https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html "},
+    {
+         "ID": "compiler_id_20",
+         "Fault Name": "静态图自定义类语法",
+         "Key Log Information": "initializing input to create instance for MsClassObject.*?should be a constant",
+         "Key Python Stack Information": "",
+         "Key C++ Stack Information": "",
+         "Fault Cause": "静态图模式下，不支持在construct中用动态输入去初始化自定义类，创建自定义类的实例时，参数必须是常量。",
+         "Error Case": """
+                    class Net(nn.Cell):
+                        def construct(self, x):
+                            net = InnerNet(x)
+                                           ^~~~~~~~~~~~~~不支持
+                            return net.number""",
+         "Modification Suggestion": "在__init__中创建自定义类的实例",
+         "Fixed Case": """
+                    class Net(nn.Cell):
+                        def __init__(self):
+                            super(Net, self).__init__()
+                            self.inner = InnerNet(val)
+                              ^~~~~~~~~~~~~~在__init__中创建实例
+                        def construct(self, x):
+                            return self.inner.number""",
+         "Fault Case": """1.静态图语法： 
+                       https://www.mindspore.cn/tutorials/experts/zh-CN/r2.0.0-alpha/network/jit_class.html#%E5%88%9B%E5%BB%BA%E8%87%AA%E5%AE%9A%E4%B9%89%E7%B1%BB%E7%9A%84%E5%AE%9E%E4%BE%8B"""},
+    {
+         "ID": "compiler_id_21",
+         "Fault Name": "静态图变量未赋初值报错",
+         "Key Log Information": "The name.*?is not defined, or not supported in graph mode",
+         "Key Python Stack Information": "",
+         "Key C++ Stack Information": "",
+         "Fault Cause": "静态图模式下，需要保证变量在每一个分支都有定义，因此建议在if判断前给变量赋一个初始值。",
+         "Error Case": """
+                    class Net(nn.Cell):
+                        def construct(self, x):
+                            if condition:
+                                var = (1, 2, 3)
+                            for i in var:
+                                      ^~~~~~~~~~~~~~未给变量var赋一个初始值
+                                print(i)
+                            return True""",
+         "Modification Suggestion": "在if判断条件前给变量赋一个初始值。",
+         "Fixed Case": """
+                    class Net(nn.Cell):
+                        def construct(self, x):
+                            var = ()
+                            ^~~~~~~~~~~~~~在if判断前给变量var赋一个初值
+                            if condition:
+                                var = (1, 2, 3)  
+                            for i in var:
+                                print(i)
+                            return True""",
+         "Fault Case": """1.静态图语法： 
+                       https://www.mindspore.cn/tutorials/experts/zh-CN/r2.0.0-alpha/network/jit_class.html#%E5%88%9B%E5%BB%BA%E8%87%AA%E5%AE%9A%E4%B9%89%E7%B1%BB%E7%9A%84%E5%AE%9E%E4%BE%8B"""},
+    {
+         "ID": "compiler_id_22",
+         "Fault Name": "静态图Tensor索引报错",
+         "Key Log Information": "switch_layer index must be an int32, but got Int64",
+         "Key Python Stack Information": "",
+         "Key C++ Stack Information": "",
+         "Fault Cause": "静态图模式下，索引值为Tensor有限制。索引Tensor是一个dtype为int32的标量",
+         "Error Case": """
+                    @jit
+                    def index_get(y):
+                        return x[y]
+                                 ^~~~~~~~~~~~~~索引值为int32的标量Tensor
+                    x = (Tensor(4), Tensor(5), Tensor(6))
+                    y = Tensor(2)
+                    out = index_get(y)""",
+         "Modification Suggestion": "改用索引值为scalar。",
+         "Fixed Case": """
+                   @jit
+                    def index_get(y):
+                        return x[y]
+                                 ^~~~~~~~~~~~~~改用索引值为scalar。
+                    x = (Tensor(4), Tensor(5), Tensor(6))
+                    y = 2
+                    out = index_get(y)""",
+         "Fault Case": """1.静态图Tensor索引语法支持： 
+                       https://www.mindspore.cn/docs/zh-CN/master/note/static_graph_syntax_support.html#tuple"""},
+    {
+         "ID": "compiler_id_23",
+         "Fault Name": "静态图Tensor索引报错",
+         "Key Log Information": "switch_layer requires that the 2th arg be tuple of functions, but got AbstractTensor",
+         "Key Python Stack Information": "",
+         "Key C++ Stack Information": "",
+         "Fault Cause": "静态图模式下，索引值为Tensor有限制。索引Tensor是一个dtype为int32的标量",
+         "Error Case": """
+                    @jit
+                    def index_get(y):
+                        return x[y]
+                                 ^~~~~~~~~~~~~~静态图中，索引值为Tensor有限制。
+                                               tuple里存放的必须是Cell。
+                    x = (Tensor(4), Tensor(5), Tensor(6))
+                    y = Tensor(2, mindspore.int32)
+                    out = index_get(y)""",
+         "Modification Suggestion": "改用索引值为scalar。",
+         "Fixed Case": """
+                   @jit
+                    def index_get(y):
+                        return x[y]
+                                 ^~~~~~~~~~~~~~改用索引值为scalar。
+                    x = (Tensor(4), Tensor(5), Tensor(6))
+                    y = 2
+                    out = index_get(y)""",
+         "Fault Case": """1.静态图Tensor索引语法支持： 
+                       https://www.mindspore.cn/docs/zh-CN/master/note/static_graph_syntax_support.html#tuple"""},
+]
+
+compiler_general_experience_list_cn = [
+    {
+     "ID": "compiler_g_id_1",
+     "Fault Name": "静态图类型推导问题",
+     "Key Log Information": "Get instructions about .analyze_fail.dat.",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Code Path":"",
+     "Fault Cause": "可能为静态图的语法编译错误，包括数据类型、原型操作、运算符、复合语句、函数等使用的问题。",
+     "Modification Suggestion": "1.根据报错信息，分析编译报错的类型； "
+                                "2.针对报错的类型，查看官网静态图语法支持介绍，分析报错的原因; "
+                                "3.使用analyze_fail.dat文件分析静态图编译结果，定位报错的代码行，分析报错原因。 ",
+     "Fault Case": "1.图编译语法支持： "
+                   " https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html "
+                   "2.错误分析方法： "
+                   "https://www.mindspore.cn/tutorials/experts/zh-CN/r1.8/debug/error_analyze.html "
+                   "3.analyze_fail.dat文件分析网络编译失败原因： "
+                   "https://www.mindspore.cn/tutorials/experts/zh-CN/r1.8/debug/mindir.html"
+                   "4.中间表达MindIR "
+                   "https://www.mindspore.cn/docs/zh-CN/r1.8/design/mindir.html"
+                   "5.社区论坛-功能调试案例集： "
+                   "https://bbs.huaweicloud.com/forum/forum-1076-2704-1.html "},
+    {
+     "ID": "compiler_g_id_2",
+     "Fault Name": "静态图编译问题",
+     "Key Log Information": "",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "mindspore.*\.cc",
+     "Code Path": "mindspore.core.abstract;mindspore.ccsrc.pipeline.jit",
+     "Fault Cause": "可能为静态图的语法编译错误，包括数据类型、原型操作、运算符、复合语句、函数等使用的问题。",
+     "Modification Suggestion": "1.根据报错信息，分析编译报错的类型； "
+                                "2.针对报错的类型，查看官网静态图语法支持介绍，分析报错的原因; ",
+     "Fault Case": "1.图编译语法支持： "
+                   " https://www.mindspore.cn/docs/note/zh-CN/r1.6/static_graph_syntax_support.html "}
+]
```

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/front_exp_lib.py` & `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/front_exp_lib.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/knowledge_base/operators_exp_lib.py` & `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/operators_exp_lib.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,498 +1,498 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-
-operators_experience_list_cn = [
-    {
-     "ID": "operator_id_1",
-     "Fault Name": "Conv2D算子参数错误",
-     "Key Log Information": "For primitive.*, the x shape size must be equal to .*, but got .*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "weight_init参数与Conv2D算子输入参数shape不匹配引起报错.",
-     "Error Case": """
-                    net = nn.Conv2d(120, 240, 4)                           
-                    x=Tensor(np.ones([120,480,640]),ms.float32)
-                    output=net(x)
-                               ^~~~~~ 输入参数的Shape不是NCHW和NHWC""",
-     "Modification Suggestion": "检查Conv2D算子输入参数x的shape，保证参数shape满足NHWC或者NCHW格式.",
-     "Fixed Case": """
-                    net = nn.Conv2d(120, 240, 4)                              
-                    x=Tensor(np.ones([1,120,480,640]),ms.float32)
-                    output = net(x)
-                                 ^~~~~~ 输入参数的Shape符合NCHW格式""",
-     "Fault Case": "1. Conv2d API: "
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Conv2d.html "
-                   "2. Conv2d算子报错案例： "
-                   "https://bbs.huaweicloud.com/forum/thread-182006-1-1.html"},
-    {
-     "ID": "operator_id_2",
-     "Fault Name": "Pad算子参数错误",
-     "Key Log Information": "all elements of .*paddings.* must be >= 0.*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "Pad算子参数paddings不支持负数",
-     "Error Case": """
-                    paddings=((1, 1), (-1, 2))
-                                        ^~~~~~~~ nn.Pad不支持负数索引
-                    net = nn.Pad(paddings, mode="SYMMETRIC")
-                    data = np.array([[1, 2, 3], [4, 5, 6]])
-                    x = Tensor(data, mindspore.float32)
-                    print("x=",x.shape)
-                    y = net(x)
-                    print(y.shape)""",
-     "Modification Suggestion": "修改Pad算子的参数paddings，避免使用负数",
-     "Fixed Case": """
-                    paddings=((1, 1), (2, 2))
-                                       ^~~~~~~~使用正整数索引
-                    net = nn.Pad(paddings, mode="SYMMETRIC")
-                    data = np.array([[1, 2, 3], [4, 5, 6]])
-                    x = Tensor(data, mindspore.float32)
-                    print("x=",x.shape)
-                    y = net(x)
-                    print(y.shape)""",
-     "Fault Case": "1. nn.Pad API: " 
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Pad.html "
-                   "2. nn.Pad 报错案例： "
-                   "https://bbs.huaweicloud.com/forum/thread-182187-1-1.html"},
-    {
-     "ID": "operator_id_3",
-     "Fault Name": "Pad算子参数错误-1.8",
-     "Key Log Information": "the .paddings.shape. must be int and must =",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "Pad算子的参数paddings的维度与输入x的维度不一致。",
-     "Error Case": """
-                    paddings=((1, 1), (2, 2))
-                    pad = nn.Pad(paddings, mode="SYMMETRIC")
-                    data = np.array([[[[1, 2, 3], [4, 5, 6]]]])
-                    print(data.shape)
-                    x = Tensor(data, mindspore.float32)
-                    print("x=",x.shape)
-                    y = pad(x)
-                            ^~~~~~~~~~~~~paddings的维度与输入x的维度不匹配
-                    print(y.shape)""",
-     "Modification Suggestion": "修改Pad算子的参数paddings或者输入参数x，保证shape与输入参数x一致。",
-     "Fixed Case":"""
-                    paddings=((0,0),(0,0),(1,1),(2,2))
-                               ^~~~~~^~~~~~表示前两个维度不进行pad
-                    pad = nn.Pad(paddings, mode="SYMMETRIC")
-                    data = np.array([[[[1, 2, 3], [4, 5, 6]]]])
-                    x = Tensor(data, mindspore.float32)
-                    x = x.squeeze()
-                    print("x=",x.shape)
-                    y = pad(x)
-                    print(y.shape)""",
-     "Fault Case": "1. nn.Pad API: "
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Pad.html "},
-    # Different versions have different error descriptions, and the ID is used repeatedly operator_id_3
-    {
-     "ID": "operator_id_3",
-     "Fault Name": "Pad算子参数错误 > 1.8",
-     "Key Log Information": "paddings.shape.* must equal to input",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "Pad算子的参数paddings的维度与输入x的维度不一致。",
-     "Error Case": """
-                paddings=((1, 1), (2, 2))
-                pad = nn.Pad(paddings, mode="SYMMETRIC")
-                data = np.array([[[[1, 2, 3], [4, 5, 6]]]])
-                print(data.shape)
-                x = Tensor(data, mindspore.float32)
-                print("x=",x.shape)
-                y = pad(x)
-                        ^~~~~~~~~~~~~paddings的维度与输入x的维度不匹配
-                print(y.shape)""",
-     "Modification Suggestion": "修改Pad算子的参数paddings或者输入参数x，保证shape与输入参数x一致。",
-     "Fixed Case": """
-                paddings=((0,0),(0,0),(1,1),(2,2))
-                           ^~~~~~^~~~~~表示前两个维度不进行pad
-                pad = nn.Pad(paddings, mode="SYMMETRIC")
-                data = np.array([[[[1, 2, 3], [4, 5, 6]]]])
-                x = Tensor(data, mindspore.float32)
-                x = x.squeeze()
-                print("x=",x.shape)
-                y = pad(x)
-                print(y.shape)""",
-     "Fault Case": "1. nn.Pad API: "
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Pad.html "},
-    # only 'paddings' up to 4 dims is supported
-    {
-     "ID": "operator_id_5",
-     "Fault Name": "Pad算子参数错误",
-     "Key Log Information": "only 'paddings' up to 4 dims is supported",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "Pad算子的参数paddings的维度超过4维报错。",
-     "Error Case": """
-                    paddings=((0,0),(0,0),(0,0),(1,1),(2,2))
-                    pad = nn.Pad(paddings, mode="SYMMETRIC")
-                                    ^~~~~~~paddings维度超过4维
-                    data = np.array([[[[[1, 2, 3], [4, 5, 6]]]]])
-                    x = Tensor(data, mindspore.float32)
-                    print("x=",x.shape)
-                    y = pad(x)
-                    print(y.shape)""",
-     "Modification Suggestion": "修改Pad算子的参数paddings与输入参数x，保证shape不超过4维且保持一致。",
-     "Fixed Case":"""
-                    paddings=((1,1),(2,2))
-                    pad = nn.Pad(paddings, mode="SYMMETRIC")
-                                    ^~~~~~~paddings维度为2
-                    data = np.array([[1, 2, 3], [4, 5, 6]]])
-                    x = Tensor(data, mindspore.float32)
-                    print("x=",x.shape)
-                    y = pad(x)
-                            ^~~~~~~x维度也为2 
-                    print(y.shape)""",
-     "Fault Case": "1. nn.Pad API: "
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Pad.html "},
-    {
-     "ID": "operator_id_6",
-     "Fault Name": "ReduceSum 算子编译报错",
-     "Key Log Information": "the num of dimensions of input.* should be .* range of .0, 8., but .*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "算子输入参数的维度超过了限制，最大值支持维度8，实际维度超过8报错.",
-     "Error Case": """
-                    reducesum = ops.ReduceSum(keep_dims=True)
-                    data = np.random.randn(1,1,4,4,4,4,4,4,4,4)
-                    x = Tensor(data, mindspore.float32)
-                                ^~~~~~~~输入x维度大于8
-                    out = reducesum(x, (1,))""",
-     "Modification Suggestion": "检查ReduceSum算子输入参数x的维度，保证维度不超过8",
-     "Fixed Case": """
-                    reducesum = ops.ReduceSum(keep_dims=True)
-                    data = np.random.randn(4, 4, 4, 4, 4, 4, 4, 4)
-                    x = Tensor(data, mindspore.float32)
-                                ^~~~~~~~输入x维度为8
-                    out = reducesum(x, (1,))""",
-     "Fault Case": "1. ReduceSum API： "
-                   "https://www.mindspore.cn/docs/zh-CN/master/api_python/ops/mindspore.ops.ReduceSum.html "
-                   "2. ReduceSum算子参数错误案例： "
-                   "https://bbs.huaweicloud.com/forum/thread-182168-1-1.html"},
-    {
-     "ID": "operator_id_7",
-     "Fault Name": "损失函数的输入参数不匹配报错",
-     "Key Log Information": "For primitive\[.*Entropy.*\], the x shape.* must be equal to.*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "损失函数要求logits和labels的shape必须一样，不一样时报错",
-     "Modification Suggestion": "修改损失函数的输入，保证输入参数的shape一致。",
-     "Fault Case": "1. 损失函数 API:  "
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/mindspore.ops.html "
-                   "2. 损失函数报错案例:  "
-                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182186"},
-    {
-     "ID": "operator_id_8",
-     "Fault Name": "损失函数的输入参数不匹配报错",
-     "Key Log Information": "For '.*Loss', the 'logits_shape' should be .*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "损失函数要求logits和labels的shape必须一样，不一样时报错",
-     "Modification Suggestion": "修改损失函数的输入，保证输入参数的shape一致。",
-     "Fault Case": "1. 损失函数 API:  "
-                   "https://www.mindspore.cn/docs/en/r1.7/acatpi_python/mindspore.nn.html#loss-function "
-                   "2. 损失函数报错案例:  "
-                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182186"},
-    {
-     "ID": "operator_id_9",
-     "Fault Name": "算子输入参数不匹配报错",
-     "Key Log Information": "x.shape and y.shape need to broadcast",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "算子输入参数的shape不同且不包含1或者-1，broadcast报错",
-     "Error Case":"""
-                    x = Tensor(np.array([2, 3]), mindspore.int32)
-                    y = Tensor(np.array([4, 5, 6]), mindspore.int32)
-                    output = x - y
-                    #          ^~~~~~~减法解析为ops.Sub算子，输入x、y的shape不一致且不能broadcast
-                    print(output)""",
-     "Modification Suggestion": "1.  检查输入参数shape错误的原因，修改至符合要求. ",
-     "Fixed Case":"""
-                    x = Tensor(np.array([0，2, 3]), mindspore.int32)
-                    y = Tensor(np.array([4, 5, 6]), mindspore.int32)
-                    output = x - y
-                    #          ^~~~~~~减法解析为ops.Sub算子，输入x、y的shape一致
-                    print(output)""",
-     "Fault Case": "1. ops.Sub API: "
-                   "https://www.mindspore.cn/docs/zh-CN/master/api_python/ops/mindspore.ops.Sub.html "
-                   "2. Sub算子broadcast报错: "
-                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182004"},
-    {
-     "ID": "operator_id_10",
-     "Fault Name": "view/Reshape算子参数不匹配报错",
-     "Key Log Information": "product of the shape of 'input_x' should be equal to",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "调用Reshape算子，或者使用其他API间接调用Reshape算子。如果reshape后Tensor元素总数量与原Tensor的不匹配，则报错。",
-     "Error Case": """
-                    data = np.random.randint(100, size=(20, 4))
-                    x = mindspore.Tensor(data,mindspore.float32)
-                    x = x.view((-1,3))
-                    #              ^~~~~~~~输入参数x的元素数量并不能被3整除
-                    print(x.shape)""",
-     "Modification Suggestion": "检查Tensor.view或者ops.Reshape算子的输入参数shape与原Tensor的shape的差异，找出元素总量不匹配的原因，修正至符合要求。",
-     "Fixed Case": """
-                    data = np.random.randint(100, size=(20, 4))
-                    x = mindspore.Tensor(data,mindspore.float32)
-                    x = x.view((-1,8))
-                    #              ^~~~~~~~输入参数x的元素数量能被8整除
-                    print(x.shape)""",
-     "Fault Case": "1. Tensor.view API： "
-                   "https://www.mindspore.cn/docs/zh-CN/master/api_python/mindspore/mindspore.Tensor.html#mindspore.Tensor.view  "
-                   "2. Tensor.view 使用错误案例： "
-                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=181982"},
-    {
-     "ID": "operator_id_11",
-     "Fault Name": "view/Reshape算子参数不匹配报错-1.9",
-     "Key Log Information": "For .*Reshape.* the product of the 'input_x' shape should be equal to",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "调用Reshape算子，或者使用其他接口（如view）间接调用Reshape算子。如果reshape后Tensor元素总数量与原Tensor的不匹配，则报错。",
-     "Error Case": """
-                    data = np.random.randint(100, size=(20, 4))
-                    x = mindspore.Tensor(data,mindspore.float32)
-                    x = x.view((-1,3))
-                    #              ^~~~~~~~输入参数x的元素数量并不能被3整除
-                    print(x.shape)""",
-     "Modification Suggestion": "检查Tensor.view或者ops.Reshape算子的输入参数shape与原Tensor的shape的差异，找出元素总量不匹配的原因，修正至符合要求。",
-     "Fixed Case": """
-                    data = np.random.randint(100, size=(20, 4))
-                    x = mindspore.Tensor(data,mindspore.float32)
-                    x = x.view((-1,8))
-                    #              ^~~~~~~~输入参数x的元素数量能被8整除
-                    print(x.shape)""",
-     "Fault Case": "1. Tensor.view API： "
-                   "https://www.mindspore.cn/docs/zh-CN/master/api_python/mindspore/mindspore.Tensor.html#mindspore.Tensor.view  "
-                   "2. Tensor.view 使用错误案例： "
-                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=181982"},
-    {
-     "ID": "operator_id_12",
-     "Fault Name": "view/Reshape算子参数不匹配报错-2.0",
-     "Key Log Information": "For .*Reshape.* the product of the 'input_x' shape should be equal to",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "调用Reshape算子，或者使用其他接口（如view）间接调用Reshape算子。如果reshape后Tensor元素总数量与原Tensor的不匹配，则报错。",
-     "Error Case": """
-                data = np.random.randint(100, size=(20, 4))
-                x = mindspore.Tensor(data,mindspore.float32)
-                x = x.view((-1,3))
-                #              ^~~~~~~~输入参数x的元素数量并不能被3整除
-                print(x.shape)""",
-     "Modification Suggestion": "检查Tensor.view或者ops.Reshape算子的输入参数shape与原Tensor的shape的差异，找出元素总量不匹配的原因，修正至符合要求。",
-     "Fixed Case": """
-                data = np.random.randint(100, size=(20, 4))
-                x = mindspore.Tensor(data,mindspore.float32)
-                x = x.view((-1,8))
-                #              ^~~~~~~~输入参数x的元素数量能被8整除
-                print(x.shape)""",
-     "Fault Case": "1. Tensor.view API： "
-                   "https://www.mindspore.cn/docs/zh-CN/master/api_python/mindspore/Tensor/mindspore.Tensor.view.html  "
-                   "2. Tensor.view 使用错误案例： "
-                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=181982"},
-    {
-     "ID": "operator_id_13",
-     "Fault Name": "算子不支持参数类型报错",
-     "Key Log Information": "Unsupported parameter type for python primitive, the parameter value is KeywordArg",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "ConvertAbstractToPython",
-     "Fault Cause": "算子不支持键值对参数而报错",
-     "Error Case": """
-                    reduce_mean = ops.ReduceMean(keep_dims=True)
-                    data = np.ones((3, 4, 5, 6), dtype=np.float32) 
-                    x = Tensor(data, mindspore.float32)
-                    out = reduce_mean(x, axis=(2, 3)) 
-                    #                    ^~~~~~~~~~输入参数不支持键值对""",
-     "Modification Suggestion": "查询算子API接口说明，确认输入参数类型，修改至符合要求. ",
-     "Fixed Case": """
-                    reduce_mean = ops.ReduceMean(keep_dims=True)
-                    data = np.ones((3, 4, 5, 6), dtype=np.float32) 
-                    x = Tensor(data, mindspore.float32)
-                    out = reduce_mean(x, (2, 3)) 
-                    #                    ^~~~~~~~~~输入参数支持tuple类型""",
-     "Fault Case": "1.ReduceMean算子输入键值对参数报错： "
-                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182167 "
-                   "2.ReduceMean API: "
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/ops/mindspore.ops.ReduceMean.html"},
-    {
-     "ID": "operator_id_14",
-     "Fault Name": "SoftmaxCrossEntropyWithLogits接口使用报错",
-     "Key Log Information": "For primitive\[SoftmaxCrossEntropyWithLogits\], the dimension of logits must be equal to ., but got .",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "SoftmaxCrossEntropyWithLogits 只支持2维的输入",
-     "Error Case":"""
-                    loss=nn.SoftmaxCrossEntropyWithLogits()
-                    x = np.array([[2,4,1,4,5],[2,1,2,4,3]])
-                    y = np.array([[0,0,0,0,1],[0,0,0,1,0]])
-                    logits = Tensor(x, mindspore.float32)
-                    labels = Tensor(y.astype(np.float32))
-                    print(logits.shape, labels.shape)
-                    out = loss(logits, labels)
-                    #             ^~~~~~~~^~~~~~~~输入入参数维度，只支持（N,C）格式""",
-     "Modification Suggestion": "检查SoftmaxCrossEntropyWithLogits输入参数维度，只支持（N,C）两维输入，可使用Reshape算子进行降维. ",
-     "Fixed Case":"""
-                    loss=nn.SoftmaxCrossEntropyWithLogits()
-                    x = np.array([[2,4,1,4,5],[2,1,2,4,3]])
-                    y = np.array([[0,0,0,0,1],[0,0,0,1,0]])
-                    logits = Tensor(x, mindspore.float32)
-                    labels = Tensor(y.astype(np.float32))
-                    print(logits.shape, labels.shape)
-                    out = loss(logits, labels)
-                    #             ^~~~~~~~^~~~~~~~输入入参数维度，符合（N,C）格式""",
-     "Fault Case": "1. SoftmaxCrossEntropyWithLogits API: "
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.SoftmaxCrossEntropyWithLogits.html"},
-    {
-     "ID": "operator_id_15",
-     "Fault Name": "算子选择类型不支持报错",
-     "Key Log Information": "Can not select a valid kernel info for .* in .*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "算子选择因输入参数类型不支持，引起报错",
-     "Error Case": """
-                    data = np.array([[1.0], [2.0], [4.0]])
-                    input_x = Tensor(data, mindspore.float64)
-                    input_y = 3.0
-                    _pow = ops.Pow()
-                    out = _pow(input_x, input_y)
-                    #            ^~~~~~~~~~~~~ops.Pow不支持float64类型
-                    print(out)""",
-     "Modification Suggestion": "找到报错算子，查询算子API说明， 修改算子输入参数类型至符合要求. ",
-     "Fixed Case": """
-                    data = np.array([[1.0], [2.0], [4.0]])
-                    input_x = Tensor(data, mindspore.float32)
-                    input_y = 3.0
-                    _pow = ops.Pow()
-                    out = _pow(input_x, input_y)
-                    #            ^~~~~~~~~~~~~ops.Pow支持float32类型
-                    print(out)""",
-     "Fault Case": "1.ops.Pow API: "
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/ops/mindspore.ops.Pow.html"
-                   "2.ops.Pow算子报错案例: "
-                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182027"},
-    {
-     "ID": "operator_id_16",
-     "Fault Name": "算子参数不支持报错",
-     "Key Log Information": "Unsupported input type for .*",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "算子不支持当前输入参数类型报错",
-     "Error Case": """
-                    x = False
-                    y = True
-                    output = ops.scalar_add(x, y)
-                    #                       ^~~~~~~不支持输入参数类型BOOL
-                    print('output', output)""",
-     "Modification Suggestion": "参考算子接口官方文档，修改输入参数类型",
-     "Fixed Case": """
-                    x = 0
-                    y = 1
-                    output = ops.scalar_add(x, y)
-                    #                       ^~~~~~~不支持输入参数类型BOOL
-                    print('output', output)""",
-     "Fault Case": "1.ops.scalar_add API: "
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/mindspore.ops.html?highlight=scalar_add "
-                   "2.ops.scalar_add()算子报错案例: "
-                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182173"},
-    {
-     "ID": "operator_id_17",
-     "Fault Name": "算子参数不支持报错-r1.6",
-     "Key Log Information": "input var is a not support implicit conversion",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "算子输入参数的类型不匹配，且不支持隐式转换报错。",
-     "Error Case": """
-                    x=Tensor(np.array([1.0,2.0,3.0]), ms.float32)
-                    y = np.array([4.0,5.0,6.0])
-                    output = x * y
-                    #            ^~~~~~乘法解释为ops.Mul算子
-                    #            ops.Mul算子不支持np.array
-                    print(output)""",
-     "Modification Suggestion": "修改算子输入参数类型，通常支持Tensor或Scale",
-     "Fixed Case":"""
-                    x=Tensor(np.array([1.0,2.0,3.0]), ms.float32)
-                    y=Tensor(np.array([4.0,5.0,6.0]), ms.float32)
-                    #   ^~~~~~修改参数类型为Tensor
-                    output = x * y
-                    print(output)""",
-     "Fault Case": "1. ops.Mul API: "
-                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/ops/mindspore.ops.Mul.html "},
-    {
-     "ID": "operator_id_18",
-     "Fault Name": "算子参数不支持报错-r1.8",
-     "Key Log Information": "input var can not be implicitly converted",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "算子输入参数的类型不匹配，且不支持隐式转换报错。",
-     "Error Case": """
-                    x=Tensor(np.array([1.0,2.0,3.0]), ms.float32)
-                    y = np.array([4.0,5.0,6.0])
-                    output = x * y
-                    #            ^~~~~~乘法解释为ops.Mul算子
-                    #            ops.Mul算子不支持np.array
-                    print(output)""",
-     "Modification Suggestion": "修改算子输入参数类型，通常支持Tensor或Scale",
-     "Fixed Case":"""
-                    x=Tensor(np.array([1.0,2.0,3.0]), ms.float32)
-                    y=Tensor(np.array([4.0,5.0,6.0]), ms.float32)
-                    #   ^~~~~~修改参数类型为Tensor
-                    output = x * y
-                    print(output)""",
-     "Fault Case": "1. ops.Mul API: "
-                   "https://www.mindspore.cn/docs/zh-CN/r1.7/api_python/ops/mindspore.ops.Mul.html "},
-    {
-     "ID": "operator_id_19",
-     "Fault Name": "算子反向未定义错误",
-     "Key Log Information": "Illegal primitive: Primitive .* bprop not defined",
-     "Key Python Stack Information": "",
-     "Key C++ Stack Information": "",
-     "Fault Cause": "该算子反向可能没有定义，反向求导时报错",
-     "Modification Suggestion": "建议自定义算子反向或者替换为其他算子",
-     "Fault Case": "1. 算子自定义反向示例： "
-                   "https://www.mindspore.cn/tutorials/experts/zh-CN/r1.7/operation/op_cpu.html#"
-                   "2. 算子反向未定义案例： "
-                   "https://bbs.huaweicloud.com/forum/thread-182166-1-1.html"}
-]
-operators_general_experience_list_cn = [
- {
-  "ID": "operator_g_id_1",
-  "Fault Name": "算子选择错误",
-  "Key Log Information": "Can not find any available kernel info;Can not select a valid kernel info",
-  "Key Python Stack Information": "",
-  "Key C++ Stack Information": "",
-  "Code Path":"",
-  "Fault Cause": "Ascend设备算子选择出现错误，可能原因是使用的算子不存在或者算子参数/输入配置错误。",
-  "Modification Suggestion": "1. 检查报错算子API定义，确认使用方式，输入参数类型及shape格式是否支持;"
-                             "2. 对比算子使用示例与自身代码的差异，从不同点查找报错原因.",
-  "Fault Case": "1.API接口文档： "
-                "https://www.mindspore.cn/docs/zh-CN/r1.8/api_python/mindspore.html "
-                "2.算子编译问题 FAQ： "
-                "https://www.mindspore.cn/docs/zh-CN/r1.8/faq/operators_compile.html "
- },
- {
-  "ID": "operator_g_id_2",
-  "Fault Name": "算子使用错误",
-  "Key Log Information": "For primitive\[.*\], the .* must be .*;For primitive\[.*\], the .* should be .*;"
-                         "For '.*', the .* must be;For '.*', the .* should be",
-  "Key Python Stack Information": "mindspore.python.mindspore.ops",
-  "Key C++ Stack Information": "mindspore.core.ops",
-  "Code Path":"mindspore.core.ops;mindspore.python.mindspore.ops",
-  "Fault Cause": "识别当前报错为算子使用错误",
-  "Modification Suggestion": "1.  确认报错算子，检查算子使用方式是否正确;  #                 "
-                             "2. 检查算子是否支持当前执行模式，如图模式、并行模式等. #              ",
-  "Fault Case": "1.MindSpore接口文档： "
-                "https://www.mindspore.cn/docs/zh-CN/r1.8/api_python/mindspore.nn.html "
-                "2.常见报错案例汇总： "
-                "https://bbs.huaweicloud.com/forum/thread-194053-1-1.html "}
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+
+operators_experience_list_cn = [
+    {
+     "ID": "operator_id_1",
+     "Fault Name": "Conv2D算子参数错误",
+     "Key Log Information": "For primitive.*, the x shape size must be equal to .*, but got .*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "weight_init参数与Conv2D算子输入参数shape不匹配引起报错.",
+     "Error Case": """
+                    net = nn.Conv2d(120, 240, 4)                           
+                    x=Tensor(np.ones([120,480,640]),ms.float32)
+                    output=net(x)
+                               ^~~~~~ 输入参数的Shape不是NCHW和NHWC""",
+     "Modification Suggestion": "检查Conv2D算子输入参数x的shape，保证参数shape满足NHWC或者NCHW格式.",
+     "Fixed Case": """
+                    net = nn.Conv2d(120, 240, 4)                              
+                    x=Tensor(np.ones([1,120,480,640]),ms.float32)
+                    output = net(x)
+                                 ^~~~~~ 输入参数的Shape符合NCHW格式""",
+     "Fault Case": "1. Conv2d API: "
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Conv2d.html "
+                   "2. Conv2d算子报错案例： "
+                   "https://bbs.huaweicloud.com/forum/thread-182006-1-1.html"},
+    {
+     "ID": "operator_id_2",
+     "Fault Name": "Pad算子参数错误",
+     "Key Log Information": "all elements of .*paddings.* must be >= 0.*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "Pad算子参数paddings不支持负数",
+     "Error Case": """
+                    paddings=((1, 1), (-1, 2))
+                                        ^~~~~~~~ nn.Pad不支持负数索引
+                    net = nn.Pad(paddings, mode="SYMMETRIC")
+                    data = np.array([[1, 2, 3], [4, 5, 6]])
+                    x = Tensor(data, mindspore.float32)
+                    print("x=",x.shape)
+                    y = net(x)
+                    print(y.shape)""",
+     "Modification Suggestion": "修改Pad算子的参数paddings，避免使用负数",
+     "Fixed Case": """
+                    paddings=((1, 1), (2, 2))
+                                       ^~~~~~~~使用正整数索引
+                    net = nn.Pad(paddings, mode="SYMMETRIC")
+                    data = np.array([[1, 2, 3], [4, 5, 6]])
+                    x = Tensor(data, mindspore.float32)
+                    print("x=",x.shape)
+                    y = net(x)
+                    print(y.shape)""",
+     "Fault Case": "1. nn.Pad API: " 
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Pad.html "
+                   "2. nn.Pad 报错案例： "
+                   "https://bbs.huaweicloud.com/forum/thread-182187-1-1.html"},
+    {
+     "ID": "operator_id_3",
+     "Fault Name": "Pad算子参数错误-1.8",
+     "Key Log Information": "the .paddings.shape. must be int and must =",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "Pad算子的参数paddings的维度与输入x的维度不一致。",
+     "Error Case": """
+                    paddings=((1, 1), (2, 2))
+                    pad = nn.Pad(paddings, mode="SYMMETRIC")
+                    data = np.array([[[[1, 2, 3], [4, 5, 6]]]])
+                    print(data.shape)
+                    x = Tensor(data, mindspore.float32)
+                    print("x=",x.shape)
+                    y = pad(x)
+                            ^~~~~~~~~~~~~paddings的维度与输入x的维度不匹配
+                    print(y.shape)""",
+     "Modification Suggestion": "修改Pad算子的参数paddings或者输入参数x，保证shape与输入参数x一致。",
+     "Fixed Case":"""
+                    paddings=((0,0),(0,0),(1,1),(2,2))
+                               ^~~~~~^~~~~~表示前两个维度不进行pad
+                    pad = nn.Pad(paddings, mode="SYMMETRIC")
+                    data = np.array([[[[1, 2, 3], [4, 5, 6]]]])
+                    x = Tensor(data, mindspore.float32)
+                    x = x.squeeze()
+                    print("x=",x.shape)
+                    y = pad(x)
+                    print(y.shape)""",
+     "Fault Case": "1. nn.Pad API: "
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Pad.html "},
+    # Different versions have different error descriptions, and the ID is used repeatedly operator_id_3
+    {
+     "ID": "operator_id_3",
+     "Fault Name": "Pad算子参数错误 > 1.8",
+     "Key Log Information": "paddings.shape.* must equal to input",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "Pad算子的参数paddings的维度与输入x的维度不一致。",
+     "Error Case": """
+                paddings=((1, 1), (2, 2))
+                pad = nn.Pad(paddings, mode="SYMMETRIC")
+                data = np.array([[[[1, 2, 3], [4, 5, 6]]]])
+                print(data.shape)
+                x = Tensor(data, mindspore.float32)
+                print("x=",x.shape)
+                y = pad(x)
+                        ^~~~~~~~~~~~~paddings的维度与输入x的维度不匹配
+                print(y.shape)""",
+     "Modification Suggestion": "修改Pad算子的参数paddings或者输入参数x，保证shape与输入参数x一致。",
+     "Fixed Case": """
+                paddings=((0,0),(0,0),(1,1),(2,2))
+                           ^~~~~~^~~~~~表示前两个维度不进行pad
+                pad = nn.Pad(paddings, mode="SYMMETRIC")
+                data = np.array([[[[1, 2, 3], [4, 5, 6]]]])
+                x = Tensor(data, mindspore.float32)
+                x = x.squeeze()
+                print("x=",x.shape)
+                y = pad(x)
+                print(y.shape)""",
+     "Fault Case": "1. nn.Pad API: "
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Pad.html "},
+    # only 'paddings' up to 4 dims is supported
+    {
+     "ID": "operator_id_5",
+     "Fault Name": "Pad算子参数错误",
+     "Key Log Information": "only 'paddings' up to 4 dims is supported",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "Pad算子的参数paddings的维度超过4维报错。",
+     "Error Case": """
+                    paddings=((0,0),(0,0),(0,0),(1,1),(2,2))
+                    pad = nn.Pad(paddings, mode="SYMMETRIC")
+                                    ^~~~~~~paddings维度超过4维
+                    data = np.array([[[[[1, 2, 3], [4, 5, 6]]]]])
+                    x = Tensor(data, mindspore.float32)
+                    print("x=",x.shape)
+                    y = pad(x)
+                    print(y.shape)""",
+     "Modification Suggestion": "修改Pad算子的参数paddings与输入参数x，保证shape不超过4维且保持一致。",
+     "Fixed Case":"""
+                    paddings=((1,1),(2,2))
+                    pad = nn.Pad(paddings, mode="SYMMETRIC")
+                                    ^~~~~~~paddings维度为2
+                    data = np.array([[1, 2, 3], [4, 5, 6]]])
+                    x = Tensor(data, mindspore.float32)
+                    print("x=",x.shape)
+                    y = pad(x)
+                            ^~~~~~~x维度也为2 
+                    print(y.shape)""",
+     "Fault Case": "1. nn.Pad API: "
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.Pad.html "},
+    {
+     "ID": "operator_id_6",
+     "Fault Name": "ReduceSum 算子编译报错",
+     "Key Log Information": "the num of dimensions of input.* should be .* range of .0, 8., but .*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "算子输入参数的维度超过了限制，最大值支持维度8，实际维度超过8报错.",
+     "Error Case": """
+                    reducesum = ops.ReduceSum(keep_dims=True)
+                    data = np.random.randn(1,1,4,4,4,4,4,4,4,4)
+                    x = Tensor(data, mindspore.float32)
+                                ^~~~~~~~输入x维度大于8
+                    out = reducesum(x, (1,))""",
+     "Modification Suggestion": "检查ReduceSum算子输入参数x的维度，保证维度不超过8",
+     "Fixed Case": """
+                    reducesum = ops.ReduceSum(keep_dims=True)
+                    data = np.random.randn(4, 4, 4, 4, 4, 4, 4, 4)
+                    x = Tensor(data, mindspore.float32)
+                                ^~~~~~~~输入x维度为8
+                    out = reducesum(x, (1,))""",
+     "Fault Case": "1. ReduceSum API： "
+                   "https://www.mindspore.cn/docs/zh-CN/master/api_python/ops/mindspore.ops.ReduceSum.html "
+                   "2. ReduceSum算子参数错误案例： "
+                   "https://bbs.huaweicloud.com/forum/thread-182168-1-1.html"},
+    {
+     "ID": "operator_id_7",
+     "Fault Name": "损失函数的输入参数不匹配报错",
+     "Key Log Information": "For primitive\[.*Entropy.*\], the x shape.* must be equal to.*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "损失函数要求logits和labels的shape必须一样，不一样时报错",
+     "Modification Suggestion": "修改损失函数的输入，保证输入参数的shape一致。",
+     "Fault Case": "1. 损失函数 API:  "
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/mindspore.ops.html "
+                   "2. 损失函数报错案例:  "
+                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182186"},
+    {
+     "ID": "operator_id_8",
+     "Fault Name": "损失函数的输入参数不匹配报错",
+     "Key Log Information": "For '.*Loss', the 'logits_shape' should be .*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "损失函数要求logits和labels的shape必须一样，不一样时报错",
+     "Modification Suggestion": "修改损失函数的输入，保证输入参数的shape一致。",
+     "Fault Case": "1. 损失函数 API:  "
+                   "https://www.mindspore.cn/docs/en/r1.7/acatpi_python/mindspore.nn.html#loss-function "
+                   "2. 损失函数报错案例:  "
+                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182186"},
+    {
+     "ID": "operator_id_9",
+     "Fault Name": "算子输入参数不匹配报错",
+     "Key Log Information": "x.shape and y.shape need to broadcast",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "算子输入参数的shape不同且不包含1或者-1，broadcast报错",
+     "Error Case":"""
+                    x = Tensor(np.array([2, 3]), mindspore.int32)
+                    y = Tensor(np.array([4, 5, 6]), mindspore.int32)
+                    output = x - y
+                    #          ^~~~~~~减法解析为ops.Sub算子，输入x、y的shape不一致且不能broadcast
+                    print(output)""",
+     "Modification Suggestion": "1.  检查输入参数shape错误的原因，修改至符合要求. ",
+     "Fixed Case":"""
+                    x = Tensor(np.array([0，2, 3]), mindspore.int32)
+                    y = Tensor(np.array([4, 5, 6]), mindspore.int32)
+                    output = x - y
+                    #          ^~~~~~~减法解析为ops.Sub算子，输入x、y的shape一致
+                    print(output)""",
+     "Fault Case": "1. ops.Sub API: "
+                   "https://www.mindspore.cn/docs/zh-CN/master/api_python/ops/mindspore.ops.Sub.html "
+                   "2. Sub算子broadcast报错: "
+                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182004"},
+    {
+     "ID": "operator_id_10",
+     "Fault Name": "view/Reshape算子参数不匹配报错",
+     "Key Log Information": "product of the shape of 'input_x' should be equal to",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "调用Reshape算子，或者使用其他API间接调用Reshape算子。如果reshape后Tensor元素总数量与原Tensor的不匹配，则报错。",
+     "Error Case": """
+                    data = np.random.randint(100, size=(20, 4))
+                    x = mindspore.Tensor(data,mindspore.float32)
+                    x = x.view((-1,3))
+                    #              ^~~~~~~~输入参数x的元素数量并不能被3整除
+                    print(x.shape)""",
+     "Modification Suggestion": "检查Tensor.view或者ops.Reshape算子的输入参数shape与原Tensor的shape的差异，找出元素总量不匹配的原因，修正至符合要求。",
+     "Fixed Case": """
+                    data = np.random.randint(100, size=(20, 4))
+                    x = mindspore.Tensor(data,mindspore.float32)
+                    x = x.view((-1,8))
+                    #              ^~~~~~~~输入参数x的元素数量能被8整除
+                    print(x.shape)""",
+     "Fault Case": "1. Tensor.view API： "
+                   "https://www.mindspore.cn/docs/zh-CN/master/api_python/mindspore/mindspore.Tensor.html#mindspore.Tensor.view  "
+                   "2. Tensor.view 使用错误案例： "
+                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=181982"},
+    {
+     "ID": "operator_id_11",
+     "Fault Name": "view/Reshape算子参数不匹配报错-1.9",
+     "Key Log Information": "For .*Reshape.* the product of the 'input_x' shape should be equal to",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "调用Reshape算子，或者使用其他接口（如view）间接调用Reshape算子。如果reshape后Tensor元素总数量与原Tensor的不匹配，则报错。",
+     "Error Case": """
+                    data = np.random.randint(100, size=(20, 4))
+                    x = mindspore.Tensor(data,mindspore.float32)
+                    x = x.view((-1,3))
+                    #              ^~~~~~~~输入参数x的元素数量并不能被3整除
+                    print(x.shape)""",
+     "Modification Suggestion": "检查Tensor.view或者ops.Reshape算子的输入参数shape与原Tensor的shape的差异，找出元素总量不匹配的原因，修正至符合要求。",
+     "Fixed Case": """
+                    data = np.random.randint(100, size=(20, 4))
+                    x = mindspore.Tensor(data,mindspore.float32)
+                    x = x.view((-1,8))
+                    #              ^~~~~~~~输入参数x的元素数量能被8整除
+                    print(x.shape)""",
+     "Fault Case": "1. Tensor.view API： "
+                   "https://www.mindspore.cn/docs/zh-CN/master/api_python/mindspore/mindspore.Tensor.html#mindspore.Tensor.view  "
+                   "2. Tensor.view 使用错误案例： "
+                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=181982"},
+    {
+     "ID": "operator_id_12",
+     "Fault Name": "view/Reshape算子参数不匹配报错-2.0",
+     "Key Log Information": "For .*Reshape.* the product of the 'input_x' shape should be equal to",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "调用Reshape算子，或者使用其他接口（如view）间接调用Reshape算子。如果reshape后Tensor元素总数量与原Tensor的不匹配，则报错。",
+     "Error Case": """
+                data = np.random.randint(100, size=(20, 4))
+                x = mindspore.Tensor(data,mindspore.float32)
+                x = x.view((-1,3))
+                #              ^~~~~~~~输入参数x的元素数量并不能被3整除
+                print(x.shape)""",
+     "Modification Suggestion": "检查Tensor.view或者ops.Reshape算子的输入参数shape与原Tensor的shape的差异，找出元素总量不匹配的原因，修正至符合要求。",
+     "Fixed Case": """
+                data = np.random.randint(100, size=(20, 4))
+                x = mindspore.Tensor(data,mindspore.float32)
+                x = x.view((-1,8))
+                #              ^~~~~~~~输入参数x的元素数量能被8整除
+                print(x.shape)""",
+     "Fault Case": "1. Tensor.view API： "
+                   "https://www.mindspore.cn/docs/zh-CN/master/api_python/mindspore/Tensor/mindspore.Tensor.view.html  "
+                   "2. Tensor.view 使用错误案例： "
+                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=181982"},
+    {
+     "ID": "operator_id_13",
+     "Fault Name": "算子不支持参数类型报错",
+     "Key Log Information": "Unsupported parameter type for python primitive, the parameter value is KeywordArg",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "ConvertAbstractToPython",
+     "Fault Cause": "算子不支持键值对参数而报错",
+     "Error Case": """
+                    reduce_mean = ops.ReduceMean(keep_dims=True)
+                    data = np.ones((3, 4, 5, 6), dtype=np.float32) 
+                    x = Tensor(data, mindspore.float32)
+                    out = reduce_mean(x, axis=(2, 3)) 
+                    #                    ^~~~~~~~~~输入参数不支持键值对""",
+     "Modification Suggestion": "查询算子API接口说明，确认输入参数类型，修改至符合要求. ",
+     "Fixed Case": """
+                    reduce_mean = ops.ReduceMean(keep_dims=True)
+                    data = np.ones((3, 4, 5, 6), dtype=np.float32) 
+                    x = Tensor(data, mindspore.float32)
+                    out = reduce_mean(x, (2, 3)) 
+                    #                    ^~~~~~~~~~输入参数支持tuple类型""",
+     "Fault Case": "1.ReduceMean算子输入键值对参数报错： "
+                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182167 "
+                   "2.ReduceMean API: "
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/ops/mindspore.ops.ReduceMean.html"},
+    {
+     "ID": "operator_id_14",
+     "Fault Name": "SoftmaxCrossEntropyWithLogits接口使用报错",
+     "Key Log Information": "For primitive\[SoftmaxCrossEntropyWithLogits\], the dimension of logits must be equal to ., but got .",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "SoftmaxCrossEntropyWithLogits 只支持2维的输入",
+     "Error Case":"""
+                    loss=nn.SoftmaxCrossEntropyWithLogits()
+                    x = np.array([[2,4,1,4,5],[2,1,2,4,3]])
+                    y = np.array([[0,0,0,0,1],[0,0,0,1,0]])
+                    logits = Tensor(x, mindspore.float32)
+                    labels = Tensor(y.astype(np.float32))
+                    print(logits.shape, labels.shape)
+                    out = loss(logits, labels)
+                    #             ^~~~~~~~^~~~~~~~输入入参数维度，只支持（N,C）格式""",
+     "Modification Suggestion": "检查SoftmaxCrossEntropyWithLogits输入参数维度，只支持（N,C）两维输入，可使用Reshape算子进行降维. ",
+     "Fixed Case":"""
+                    loss=nn.SoftmaxCrossEntropyWithLogits()
+                    x = np.array([[2,4,1,4,5],[2,1,2,4,3]])
+                    y = np.array([[0,0,0,0,1],[0,0,0,1,0]])
+                    logits = Tensor(x, mindspore.float32)
+                    labels = Tensor(y.astype(np.float32))
+                    print(logits.shape, labels.shape)
+                    out = loss(logits, labels)
+                    #             ^~~~~~~~^~~~~~~~输入入参数维度，符合（N,C）格式""",
+     "Fault Case": "1. SoftmaxCrossEntropyWithLogits API: "
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/nn/mindspore.nn.SoftmaxCrossEntropyWithLogits.html"},
+    {
+     "ID": "operator_id_15",
+     "Fault Name": "算子选择类型不支持报错",
+     "Key Log Information": "Can not select a valid kernel info for .* in .*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "算子选择因输入参数类型不支持，引起报错",
+     "Error Case": """
+                    data = np.array([[1.0], [2.0], [4.0]])
+                    input_x = Tensor(data, mindspore.float64)
+                    input_y = 3.0
+                    _pow = ops.Pow()
+                    out = _pow(input_x, input_y)
+                    #            ^~~~~~~~~~~~~ops.Pow不支持float64类型
+                    print(out)""",
+     "Modification Suggestion": "找到报错算子，查询算子API说明， 修改算子输入参数类型至符合要求. ",
+     "Fixed Case": """
+                    data = np.array([[1.0], [2.0], [4.0]])
+                    input_x = Tensor(data, mindspore.float32)
+                    input_y = 3.0
+                    _pow = ops.Pow()
+                    out = _pow(input_x, input_y)
+                    #            ^~~~~~~~~~~~~ops.Pow支持float32类型
+                    print(out)""",
+     "Fault Case": "1.ops.Pow API: "
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/ops/mindspore.ops.Pow.html"
+                   "2.ops.Pow算子报错案例: "
+                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182027"},
+    {
+     "ID": "operator_id_16",
+     "Fault Name": "算子参数不支持报错",
+     "Key Log Information": "Unsupported input type for .*",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "算子不支持当前输入参数类型报错",
+     "Error Case": """
+                    x = False
+                    y = True
+                    output = ops.scalar_add(x, y)
+                    #                       ^~~~~~~不支持输入参数类型BOOL
+                    print('output', output)""",
+     "Modification Suggestion": "参考算子接口官方文档，修改输入参数类型",
+     "Fixed Case": """
+                    x = 0
+                    y = 1
+                    output = ops.scalar_add(x, y)
+                    #                       ^~~~~~~不支持输入参数类型BOOL
+                    print('output', output)""",
+     "Fault Case": "1.ops.scalar_add API: "
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/mindspore.ops.html?highlight=scalar_add "
+                   "2.ops.scalar_add()算子报错案例: "
+                   "https://bbs.huaweicloud.com/forum/forum.php?mod=viewthread&tid=182173"},
+    {
+     "ID": "operator_id_17",
+     "Fault Name": "算子参数不支持报错-r1.6",
+     "Key Log Information": "input var is a not support implicit conversion",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "算子输入参数的类型不匹配，且不支持隐式转换报错。",
+     "Error Case": """
+                    x=Tensor(np.array([1.0,2.0,3.0]), ms.float32)
+                    y = np.array([4.0,5.0,6.0])
+                    output = x * y
+                    #            ^~~~~~乘法解释为ops.Mul算子
+                    #            ops.Mul算子不支持np.array
+                    print(output)""",
+     "Modification Suggestion": "修改算子输入参数类型，通常支持Tensor或Scale",
+     "Fixed Case":"""
+                    x=Tensor(np.array([1.0,2.0,3.0]), ms.float32)
+                    y=Tensor(np.array([4.0,5.0,6.0]), ms.float32)
+                    #   ^~~~~~修改参数类型为Tensor
+                    output = x * y
+                    print(output)""",
+     "Fault Case": "1. ops.Mul API: "
+                   "https://www.mindspore.cn/docs/api/zh-CN/r1.6/api_python/ops/mindspore.ops.Mul.html "},
+    {
+     "ID": "operator_id_18",
+     "Fault Name": "算子参数不支持报错-r1.8",
+     "Key Log Information": "input var can not be implicitly converted",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "算子输入参数的类型不匹配，且不支持隐式转换报错。",
+     "Error Case": """
+                    x=Tensor(np.array([1.0,2.0,3.0]), ms.float32)
+                    y = np.array([4.0,5.0,6.0])
+                    output = x * y
+                    #            ^~~~~~乘法解释为ops.Mul算子
+                    #            ops.Mul算子不支持np.array
+                    print(output)""",
+     "Modification Suggestion": "修改算子输入参数类型，通常支持Tensor或Scale",
+     "Fixed Case":"""
+                    x=Tensor(np.array([1.0,2.0,3.0]), ms.float32)
+                    y=Tensor(np.array([4.0,5.0,6.0]), ms.float32)
+                    #   ^~~~~~修改参数类型为Tensor
+                    output = x * y
+                    print(output)""",
+     "Fault Case": "1. ops.Mul API: "
+                   "https://www.mindspore.cn/docs/zh-CN/r1.7/api_python/ops/mindspore.ops.Mul.html "},
+    {
+     "ID": "operator_id_19",
+     "Fault Name": "算子反向未定义错误",
+     "Key Log Information": "Illegal primitive: Primitive .* bprop not defined",
+     "Key Python Stack Information": "",
+     "Key C++ Stack Information": "",
+     "Fault Cause": "该算子反向可能没有定义，反向求导时报错",
+     "Modification Suggestion": "建议自定义算子反向或者替换为其他算子",
+     "Fault Case": "1. 算子自定义反向示例： "
+                   "https://www.mindspore.cn/tutorials/experts/zh-CN/r1.7/operation/op_cpu.html#"
+                   "2. 算子反向未定义案例： "
+                   "https://bbs.huaweicloud.com/forum/thread-182166-1-1.html"}
+]
+operators_general_experience_list_cn = [
+ {
+  "ID": "operator_g_id_1",
+  "Fault Name": "算子选择错误",
+  "Key Log Information": "Can not find any available kernel info;Can not select a valid kernel info",
+  "Key Python Stack Information": "",
+  "Key C++ Stack Information": "",
+  "Code Path":"",
+  "Fault Cause": "Ascend设备算子选择出现错误，可能原因是使用的算子不存在或者算子参数/输入配置错误。",
+  "Modification Suggestion": "1. 检查报错算子API定义，确认使用方式，输入参数类型及shape格式是否支持;"
+                             "2. 对比算子使用示例与自身代码的差异，从不同点查找报错原因.",
+  "Fault Case": "1.API接口文档： "
+                "https://www.mindspore.cn/docs/zh-CN/r1.8/api_python/mindspore.html "
+                "2.算子编译问题 FAQ： "
+                "https://www.mindspore.cn/docs/zh-CN/r1.8/faq/operators_compile.html "
+ },
+ {
+  "ID": "operator_g_id_2",
+  "Fault Name": "算子使用错误",
+  "Key Log Information": "For primitive\[.*\], the .* must be .*;For primitive\[.*\], the .* should be .*;"
+                         "For '.*', the .* must be;For '.*', the .* should be",
+  "Key Python Stack Information": "mindspore.python.mindspore.ops",
+  "Key C++ Stack Information": "mindspore.core.ops",
+  "Code Path":"mindspore.core.ops;mindspore.python.mindspore.ops",
+  "Fault Cause": "识别当前报错为算子使用错误",
+  "Modification Suggestion": "1.  确认报错算子，检查算子使用方式是否正确;  #                 "
+                             "2. 检查算子是否支持当前执行模式，如图模式、并行模式等. #              ",
+  "Fault Case": "1.MindSpore接口文档： "
+                "https://www.mindspore.cn/docs/zh-CN/r1.8/api_python/mindspore.nn.html "
+                "2.常见报错案例汇总： "
+                "https://bbs.huaweicloud.com/forum/thread-194053-1-1.html "}
 ]
```

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/proposal_action.py` & `troubleshooter-1.0.7/troubleshooter/proposer/proposal_action.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/proposer/proposer_factory.py` & `troubleshooter-1.0.7/troubleshooter/proposer/proposer_factory.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/tracker/__init__.py` & `troubleshooter-1.0.7/troubleshooter/tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.6/troubleshooter/tracker/tracker.py` & `troubleshooter-1.0.7/troubleshooter/tracker/tracker.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-# Copyright 2022 Tiger Miao and collaborators.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""Tracker"""
-import os
-from pysnooper.tracer import Tracer
-from pysnooper.tracer import get_path_and_source_from_frame
-from pysnooper.utils import get_repr_function
-from troubleshooter import log as logger
-
-_NO_RESULT = -1
-_FRAMEWORK_MS = 1
-
-
-# pylint: disable=W0703
-def get_local_reprs(frame, check_keyword):
-    """
-    get local reprs
-    Args:
-        check_keyword: check keyword
-        frame: python frame
-    """
-    for key, value in frame.f_locals.items():
-        repr_function = get_repr_function(value, custom_repr=())
-        try:
-            r = repr_function(value)
-        except Exception:
-            r = 'REPR FAILED'
-        r = r.replace('\r', '').replace('\n', '')
-        if r.find(check_keyword) != _NO_RESULT and r.find('value=') != _NO_RESULT:
-            logger.user_warning("'{}' is detected, Key is {}, Value is {}".format(check_keyword, key, r))
-            return True
-    return False
-
-
-class Tracker(Tracer):
-    """
-    Framework Code Execution Tracking
-    Args:
-        framework (bool): Framework type
-        filter (dict): Tracking filtering
-        *args: Tracer args
-        **kwargs: Tracer args
-    """
-
-    def __init__(self, level=1, **kwargs):
-        self.root_file = ""
-        self.root_path = ""
-        self.level = level
-        self.ms_func_blacklist = {"deco": ["ops/primitive.py"], "__init__": ["ops/primitive.py", "common/tensor.py"],
-                                  "__new__": ["common/parameter.py"], "__setattr__": ["nn/cell.py"],
-                                  "__getattr__": ["nn/cell.py"],
-                                  "_get_cache_prim_for_pynative": ["ops/_primitive_cache.py"]}
-        self.func_whitelist = kwargs.get('func_wl', None)
-        self.path_whitelist = kwargs.get('path_wl', [])
-        self.path_blacklist = kwargs.get('path_bl', [])
-        self.check_keyword = kwargs.get('check_keyword', None)
-        self.check_mode = kwargs.get('check_mode', 1)
-        self.framework = kwargs.get('framework', 1)
-        self.event_list = kwargs.get('event_list', [])
-        self.depth = kwargs.get('depth', 15)
-        self.max_variable_length = kwargs.get('max_variable_length', 150)
-        if self.event_list and 'call' in self.event_list and 'return' not in self.event_list:
-            self.event_list.append('return')
-        if self.level == 2:
-            blacklist = {"__setattr__": "nn/cell.py", "__getattr__": "nn/cell.py"}
-            self.ms_func_blacklist.update(blacklist)
-
-        self.pop_key_list = ['event_list', 'func_wl', 'path_wl', 'depth', 'max_variable_length', 'check_keyword',
-                             'path_bl', 'check_mode']
-        for key in self.pop_key_list:
-            if kwargs.get(key):
-                kwargs.pop(key)
-        super(Tracker, self).__init__(depth=self.depth, max_variable_length=self.max_variable_length, **kwargs)
-
-    def _frame_filter(self, frame, event):
-        if self.framework == _FRAMEWORK_MS:
-            return self._frame_filter_ms(frame, event)
-        return True
-
-    def _frame_filter_ms(self, frame, event):
-        """
-        Filter the frame information of
-        Args:
-            frame: The python frame
-            event: Reserved Fields
-            arg: Reserved Fields
-
-        Returns (bool): frame information
-        """
-        result = True
-
-        # line_no = frame.f_lineno
-        func_name = frame.f_code.co_name
-        source_path = get_path_and_source_from_frame(frame)
-        source_path = source_path if not self.normalize else os.path.basename(source_path)
-
-        if self.root_file == "":
-            self.root_file = source_path[0]
-            self.root_func = func_name
-            self.root_path = os.path.abspath(os.path.dirname(self.root_file))
-            logger.info("the root_file is {}".format(self.root_file))
-            logger.info("the root_func is {}".format(self.root_func))
-            logger.info("the root_path is {}".format(self.root_path))
-            return result
-
-        logger.info("the path_name is {}".format(source_path[0]))
-        logger.info("the func_name is {}".format(func_name))
-
-        # ignore the MindSpore backlist function
-        ignore_path_list = self.ms_func_blacklist.get(func_name)
-        if ignore_path_list:
-            for ignore_path in ignore_path_list:
-                logger.debug("the source_path[0] is {},ignore_path is {}".format(source_path[0], ignore_path))
-                if source_path[0].find(ignore_path) != _NO_RESULT:
-                    return False
-
-        if self.path_blacklist:
-            for path in self.path_blacklist:
-                if source_path[0].find(path) != _NO_RESULT:
-                    return False
-
-        if self.path_whitelist:
-            for path in self.path_whitelist:
-                return source_path[0].find(path) != _NO_RESULT
-
-        if self.level == 1 and (func_name not in ["construct"] or
-                                (source_path[0].find(self.root_path) == _NO_RESULT and
-                                 source_path[0].find("container.py") == _NO_RESULT)):
-            return False
-
-        if self.level == 2 and (func_name not in ["construct", "_convert_python_data"]):
-            return False
-
-        if self.level == 3 and source_path[0].find("site-packages/mindspore") == _NO_RESULT and \
-                source_path[0].find(self.root_path) == _NO_RESULT:
-            return False
-
-        if self.check_keyword and self.check_mode == 1:
-            check_result = get_local_reprs(frame, self.check_keyword)
-            if check_result:
-                exit(0)
-        elif self.check_keyword and self.check_mode == 2:
-            get_local_reprs(frame, self.check_keyword)
-
-        if self.event_list and event not in self.event_list:
-            return False
-
-        return result
-
-    def trace(self, frame, event, arg):
-        if not self._frame_filter(frame, event):
-            return None
-        return super(Tracker, self).trace(frame, event, arg)
+# Copyright 2022 Tiger Miao and collaborators.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""Tracker"""
+import os
+from pysnooper.tracer import Tracer
+from pysnooper.tracer import get_path_and_source_from_frame
+from pysnooper.utils import get_repr_function
+from troubleshooter import log as logger
+
+_NO_RESULT = -1
+_FRAMEWORK_MS = 1
+
+
+# pylint: disable=W0703
+def get_local_reprs(frame, check_keyword):
+    """
+    get local reprs
+    Args:
+        check_keyword: check keyword
+        frame: python frame
+    """
+    for key, value in frame.f_locals.items():
+        repr_function = get_repr_function(value, custom_repr=())
+        try:
+            r = repr_function(value)
+        except Exception:
+            r = 'REPR FAILED'
+        r = r.replace('\r', '').replace('\n', '')
+        if r.find(check_keyword) != _NO_RESULT and r.find('value=') != _NO_RESULT:
+            logger.user_warning("'{}' is detected, Key is {}, Value is {}".format(check_keyword, key, r))
+            return True
+    return False
+
+
+class Tracker(Tracer):
+    """
+    Framework Code Execution Tracking
+    Args:
+        framework (bool): Framework type
+        filter (dict): Tracking filtering
+        *args: Tracer args
+        **kwargs: Tracer args
+    """
+
+    def __init__(self, level=1, **kwargs):
+        self.root_file = ""
+        self.root_path = ""
+        self.level = level
+        self.ms_func_blacklist = {"deco": ["ops/primitive.py"], "__init__": ["ops/primitive.py", "common/tensor.py"],
+                                  "__new__": ["common/parameter.py"], "__setattr__": ["nn/cell.py"],
+                                  "__getattr__": ["nn/cell.py"],
+                                  "_get_cache_prim_for_pynative": ["ops/_primitive_cache.py"]}
+        self.func_whitelist = kwargs.get('func_wl', None)
+        self.path_whitelist = kwargs.get('path_wl', [])
+        self.path_blacklist = kwargs.get('path_bl', [])
+        self.check_keyword = kwargs.get('check_keyword', None)
+        self.check_mode = kwargs.get('check_mode', 1)
+        self.framework = kwargs.get('framework', 1)
+        self.event_list = kwargs.get('event_list', [])
+        self.depth = kwargs.get('depth', 15)
+        self.max_variable_length = kwargs.get('max_variable_length', 150)
+        if self.event_list and 'call' in self.event_list and 'return' not in self.event_list:
+            self.event_list.append('return')
+        if self.level == 2:
+            blacklist = {"__setattr__": "nn/cell.py", "__getattr__": "nn/cell.py"}
+            self.ms_func_blacklist.update(blacklist)
+
+        self.pop_key_list = ['event_list', 'func_wl', 'path_wl', 'depth', 'max_variable_length', 'check_keyword',
+                             'path_bl', 'check_mode']
+        for key in self.pop_key_list:
+            if kwargs.get(key):
+                kwargs.pop(key)
+        super(Tracker, self).__init__(depth=self.depth, max_variable_length=self.max_variable_length, **kwargs)
+
+    def _frame_filter(self, frame, event):
+        if self.framework == _FRAMEWORK_MS:
+            return self._frame_filter_ms(frame, event)
+        return True
+
+    def _frame_filter_ms(self, frame, event):
+        """
+        Filter the frame information of
+        Args:
+            frame: The python frame
+            event: Reserved Fields
+            arg: Reserved Fields
+
+        Returns (bool): frame information
+        """
+        result = True
+
+        # line_no = frame.f_lineno
+        func_name = frame.f_code.co_name
+        source_path = get_path_and_source_from_frame(frame)
+        source_path = source_path if not self.normalize else os.path.basename(source_path)
+
+        if self.root_file == "":
+            self.root_file = source_path[0]
+            self.root_func = func_name
+            self.root_path = os.path.abspath(os.path.dirname(self.root_file))
+            logger.info("the root_file is {}".format(self.root_file))
+            logger.info("the root_func is {}".format(self.root_func))
+            logger.info("the root_path is {}".format(self.root_path))
+            return result
+
+        logger.info("the path_name is {}".format(source_path[0]))
+        logger.info("the func_name is {}".format(func_name))
+
+        # ignore the MindSpore backlist function
+        ignore_path_list = self.ms_func_blacklist.get(func_name)
+        if ignore_path_list:
+            for ignore_path in ignore_path_list:
+                logger.debug("the source_path[0] is {},ignore_path is {}".format(source_path[0], ignore_path))
+                if source_path[0].find(ignore_path) != _NO_RESULT:
+                    return False
+
+        if self.path_blacklist:
+            for path in self.path_blacklist:
+                if source_path[0].find(path) != _NO_RESULT:
+                    return False
+
+        if self.path_whitelist:
+            for path in self.path_whitelist:
+                return source_path[0].find(path) != _NO_RESULT
+
+        if self.level == 1 and (func_name not in ["construct"] or
+                                (source_path[0].find(self.root_path) == _NO_RESULT and
+                                 source_path[0].find("container.py") == _NO_RESULT)):
+            return False
+
+        if self.level == 2 and (func_name not in ["construct", "_convert_python_data"]):
+            return False
+
+        if self.level == 3 and source_path[0].find("site-packages/mindspore") == _NO_RESULT and \
+                source_path[0].find(self.root_path) == _NO_RESULT:
+            return False
+
+        if self.check_keyword and self.check_mode == 1:
+            check_result = get_local_reprs(frame, self.check_keyword)
+            if check_result:
+                exit(0)
+        elif self.check_keyword and self.check_mode == 2:
+            get_local_reprs(frame, self.check_keyword)
+
+        if self.event_list and event not in self.event_list:
+            return False
+
+        return result
+
+    def trace(self, frame, event, arg):
+        if not self._frame_filter(frame, event):
+            return None
+        return super(Tracker, self).trace(frame, event, arg)
```

### Comparing `troubleshooter-1.0.6/troubleshooter.egg-info/SOURCES.txt` & `troubleshooter-1.0.7/troubleshooter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/util.py
 tests/diff_handler/__init__.py
 tests/diff_handler/test_compare.py
+tests/diff_handler/test_migrator.py
 tests/proposer/__init__.py
 tests/proposer/1_9/__init__.py
 tests/proposer/1_9/test_compile.py
 tests/proposer/1_9/test_ops.py
 tests/proposer/master/__init__.py
 tests/proposer/master/test_ascend_vm.py
 tests/proposer/master/test_compile.py
```


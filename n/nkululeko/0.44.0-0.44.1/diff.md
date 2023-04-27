# Comparing `tmp/nkululeko-0.44.0.tar.gz` & `tmp/nkululeko-0.44.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.44.0.tar", last modified: Thu Apr 20 16:55:45 2023, max compression
+gzip compressed data, was "nkululeko-0.44.1.tar", last modified: Thu Apr 27 09:30:21 2023, max compression
```

## Comparing `nkululeko-0.44.0.tar` & `nkululeko-0.44.1.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-20 16:55:45.507060 nkululeko-0.44.0/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5286 2023-04-20 15:52:33.000000 nkululeko-0.44.0/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.44.0/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16010 2023-04-20 16:55:45.507060 nkululeko-0.44.0/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10171 2023-04-04 08:11:52.000000 nkululeko-0.44.0/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-20 16:55:45.507060 nkululeko-0.44.0/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.44.0/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.44.0/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.44.0/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.44.0/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.44.0/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-04-20 15:51:53.000000 nkululeko-0.44.0/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-03-23 14:59:33.000000 nkululeko-0.44.0/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1820 2023-03-23 14:42:03.000000 nkululeko-0.44.0/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.44.0/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.44.0/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.44.0/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20413 2023-04-20 16:45:58.000000 nkululeko-0.44.0/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1692 2023-04-20 13:43:01.000000 nkululeko-0.44.0/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3726 2023-04-18 13:35:09.000000 nkululeko-0.44.0/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2536 2023-02-20 12:40:05.000000 nkululeko-0.44.0/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3117 2023-04-19 15:46:17.000000 nkululeko-0.44.0/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-02-09 11:59:30.000000 nkululeko-0.44.0/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.44.0/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.44.0/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.44.0/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1699 2023-02-15 16:11:36.000000 nkululeko-0.44.0/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.44.0/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.44.0/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3174 2023-04-19 15:22:07.000000 nkululeko-0.44.0/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.44.0/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.44.0/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.44.0/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.44.0/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.44.0/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.44.0/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.44.0/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.44.0/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.44.0/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.44.0/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.44.0/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.44.0/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.44.0/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.44.0/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.44.0/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.44.0/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.44.0/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.44.0/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.44.0/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.44.0/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.44.0/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.44.0/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.44.0/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.44.0/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.44.0/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10638 2023-02-16 12:26:38.000000 nkululeko-0.44.0/nkululeko/runmanager copy.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.44.0/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.44.0/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.44.0/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.44.0/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7661 2023-02-20 11:54:33.000000 nkululeko-0.44.0/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-20 16:55:45.507060 nkululeko-0.44.0/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16010 2023-04-20 16:55:45.000000 nkululeko-0.44.0/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1562 2023-04-20 16:55:45.000000 nkululeko-0.44.0/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-04-20 16:55:45.000000 nkululeko-0.44.0/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-04-20 16:55:45.000000 nkululeko-0.44.0/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-04-20 16:55:45.000000 nkululeko-0.44.0/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.44.0/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      938 2023-04-20 16:55:45.507060 nkululeko-0.44.0/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.44.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-27 09:30:21.173899 nkululeko-0.44.1/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5501 2023-04-27 09:02:47.000000 nkululeko-0.44.1/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.44.1/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16530 2023-04-27 09:30:21.173899 nkululeko-0.44.1/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10476 2023-04-21 08:51:24.000000 nkululeko-0.44.1/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-27 09:30:21.173899 nkululeko-0.44.1/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.44.1/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.44.1/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.44.1/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.44.1/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.44.1/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-04-27 08:44:51.000000 nkululeko-0.44.1/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-03-23 14:59:33.000000 nkululeko-0.44.1/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1908 2023-04-27 08:57:05.000000 nkululeko-0.44.1/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.44.1/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.44.1/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.44.1/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20413 2023-04-20 16:45:58.000000 nkululeko-0.44.1/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1873 2023-04-27 09:18:23.000000 nkululeko-0.44.1/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3726 2023-04-18 13:35:09.000000 nkululeko-0.44.1/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2536 2023-02-20 12:40:05.000000 nkululeko-0.44.1/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3117 2023-04-19 15:46:17.000000 nkululeko-0.44.1/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-02-09 11:59:30.000000 nkululeko-0.44.1/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.44.1/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.44.1/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.44.1/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1699 2023-02-15 16:11:36.000000 nkululeko-0.44.1/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.44.1/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.44.1/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3174 2023-04-19 15:22:07.000000 nkululeko-0.44.1/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.44.1/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.44.1/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.44.1/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.44.1/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.44.1/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.44.1/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.44.1/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.44.1/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.44.1/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.44.1/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.44.1/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.44.1/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.44.1/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.44.1/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.44.1/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.44.1/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.44.1/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.44.1/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.44.1/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.44.1/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.44.1/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.44.1/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.44.1/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.44.1/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.44.1/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.44.1/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.44.1/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.44.1/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.44.1/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7661 2023-02-20 11:54:33.000000 nkululeko-0.44.1/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-04-27 09:30:21.173899 nkululeko-0.44.1/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16530 2023-04-27 09:30:21.000000 nkululeko-0.44.1/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1533 2023-04-27 09:30:21.000000 nkululeko-0.44.1/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-04-27 09:30:21.000000 nkululeko-0.44.1/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-04-27 09:30:21.000000 nkululeko-0.44.1/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-04-27 09:30:21.000000 nkululeko-0.44.1/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.44.1/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      938 2023-04-27 09:30:21.173899 nkululeko-0.44.1/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.44.1/setup.py
```

### Comparing `nkululeko-0.44.0/CHANGELOG.md` & `nkululeko-0.44.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 0.44.1
+--------------
+* bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
+* bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
+
 Version 0.44.0
 --------------
 * added scatter functions: tsne, pca, umap
 
 Version 0.43.7
 --------------
 * added clap features
```

### Comparing `nkululeko-0.44.0/LICENSE` & `nkululeko-0.44.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/PKG-INFO` & `nkululeko-0.44.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.44.0
+Version: 0.44.1
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,29 +18,29 @@
 * [Overview](#overview)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Hello World](#hello-world-example)
 * [Licence](#licence)
 
 ## Overview
-A project to detect speaker characteristics by machine learning experiments with a high level interface.
+A project to detect speaker characteristics by machine learning experiments with a high-level interface.
 
 The idea is to have a framework (based on e.g. sklearn and torch) that can be used by people not being experienced programmers as they mainly have to adapt an initialization parameter file per experiment.
 
-* The latest features can be seen at [the ini-file options](./ini_file.md) that are used to control Nkululeko
+* The latest features can be seen in [the ini-file](./ini_file.md) options](./ini_file.md) that are used to control Nkululeko
 * Below is a [Hello World example](#helloworld) that should set you up fastly.
 * [Here's a blog post on how to set up nkululeko on your computer.](http://blog.syntheticspeech.de/2021/08/30/how-to-set-up-your-first-nkululeko-project/)
 * [Here's a slide presentation about nkululeko](docs/nkululeko.pdf)
 * [Here's a video presentation about nkululeko](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * [Here's the 2022 LREC article on nkululeko](http://felix.syntheticspeech.de/publications/Nkululeko_LREC.pdf)
 
 Here are some examples of typical output:
 
 ### Confusion matrix
-Per default, Nkululeko displays results as a  confusion matrix, using binning with regression.
+Per default, Nkululeko displays results as a confusion matrix using binning with regression.
 
 <img src="images/conf_mat.png" width="500px"/>
 
 ### Epoch progression
 The point when overfitting starts can sometimes be seen by looking at the results per epoch:
 
 <img src="images/epoch_progression.png" width="500px"/>
@@ -63,15 +63,15 @@
 ### Data distribution
 Sometimes you only want to take a look at your data:
 
 <img src="images/data_plot.png" width="500px"/>
 
 ## Installation
 
-Create and activate a virtual python environment and simply run
+Create and activate a virtual Python environment and simply run
 ```
 pip install nkululeko
 ```
 
 Some examples for *ini*-files (which you use to control nkululeko) are in the [tests folder](https://github.com/felixbur/nkululeko/tree/main/tests).
 
 
@@ -95,20 +95,21 @@
 type = ['praat']
 [MODEL]
 type = svm
 [EXPL]
 model = tree
 plot_tree = True
 [PLOT]
-combine_per_speaker = True
+combine_per_speaker = mode
 ```
+Read the [Hello World example](#hello-world-example) for initial usage with Emo-DB dataset.
 
 Here is an overview of the interfaces:
 * **nkululeko.nkululeko**: doing experiments
-* **nkululeko.demo**: demo the current best model on commandline
+* **nkululeko.demo**: demo the current best model on command line
 * **nkululeko.test**: predict a series of files with the current best model
 * **nkululeko.explore**: perform data exploration
 * **nkululeko.augment**: augment the current training data
 
 Alternatively, there is a central "experiment" class that can be used by own experiments
 
 There's my [blog](http://blog.syntheticspeech.de/?s=nkululeko) with tutorials:
@@ -136,58 +137,59 @@
 * [Run multiple experiments in one go](http://blog.syntheticspeech.de/2022/03/28/how-to-run-multiple-experiments-in-one-go-with-nkululeko/)
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
+ * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework.
 ![sketch](images/class_diagram.png)
 
-Currently the following linear classifiers are implemented (integrated from sklearn):
+Currently, the following linear classifiers are implemented (integrated from sklearn):
 * SVM, SVR, XGB, XGR, Tree, Tree_regressor, KNN, KNN_regressor, NaiveBayes, GMM
   and the following ANNs
 * MLP, CNN (tbd)
 
 Here's [an animation that shows the progress of classification done with nkululeko](https://youtu.be/6Y0M382GjvM)
 
 ### Initialization file
 You could 
 * use a generic main python file (like my_experiment.py), 
 * adapt the path to your nkululeko src 
 * and then adapt an .ini file (again fitting at least the paths to src and data)
   
-Here's [an overview on the ini-file options](./ini_file.md)
+Here's [an overview of the ini-file options](./ini_file.md)
 
 ### <a name="helloworld">Hello World example</a>
-* NEW [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
+* NEW: [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * Set up Python on your computer, version >= 3.6
 * Open a terminal/commandline/console window
 * Test python by typing ```python```, python should start with version >3 (NOT 2!). You can leave the Python Interpreter by typing *exit()*
-* Create a folder on your computer for this example, let's call it *nkulu_work*
-* Get a copy of the [Berlin emodb in audformat](https://tubcloud.tu-berlin.de/s/LfkysdXJfiobiEG) and unpack the same folder (*nkulu_work*)
+* Create a folder on your computer for this example, let's call it `nkulu_work`
+* Get a copy of the [Berlin emodb in audformat](https://tubcloud.tu-berlin.de/s/LfkysdXJfiobiEG) and unpack the same folder (`nkulu_work`)
 * Make sure the folder is called "emodb" and does contain the database files directly (not box-in-a-box)
-* Also, in the *nkulu_work* folder: 
-  * Create a python environment
+* Also, in the `nkulu_work` folder: 
+  * Create a Python environment
     * ```python -m venv venv```
   * Then, activate it:
-    * under linux / mac
+    * under Linux / mac
       * ```source venv/bin/activate```
     * under Windows
       * ```venv\Scripts\activate.bat```
     * if that worked, you should see a ```(venv)``` in front of your prompt
   * Install the required packages in your environment
     * ```pip install nkululeko```
     * Repeat until all error messages vanished (or fix them, or try to ignore them)...
 * Now you should have two folders in your *nkulu_work* folder:
   * *emodb* and *venv*
-* Download a copy of the file [exp_emodb.ini](demos/exp_emodb.ini)
+* Download a copy of the file [exp_emodb.ini](demos/exp_emodb.ini) to the current working directory (```nkulu_work```)
 * Run the demo
   * ```python -m nkululeko.nkululeko --config exp_emodb.ini```
 * Find the results in the newly created folder exp_emodb 
   * Inspect ```exp_emodb/images/run_0/emodb_xgb_os_0_000_cnf.png```
   * This is the main result of you experiment: a confusion matrix for the emodb emotional categories
 * Inspect and play around with the [demo configuration file](demos/exp_emodb.ini) that defined your experiment, then re-run.
 * There are many ways to experiment with different classifiers and acoustic features sets, [all described here](https://github.com/felixbur/nkululeko/blob/main/ini_file.md)
@@ -198,22 +200,27 @@
 * Feature scaling
 * Label encoding
 * Binning (continuous to categorical)
 * Online demo interface for trained models 
 
 ### Outlook
 * Classifiers: CNN
-* Feature extractors: mid level descriptors, Mel-spectra
+* Feature extractors: mid-level descriptors, Mel-spectra
 
-## Licence
+## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.44.1
+--------------
+* bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
+* bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
+
 Version 0.44.0
 --------------
 * added scatter functions: tsne, pca, umap
 
 Version 0.43.7
 --------------
 * added clap features
```

### Comparing `nkululeko-0.44.0/README.md` & `nkululeko-0.44.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 * [Overview](#overview)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Hello World](#hello-world-example)
 * [Licence](#licence)
 
 ## Overview
-A project to detect speaker characteristics by machine learning experiments with a high level interface.
+A project to detect speaker characteristics by machine learning experiments with a high-level interface.
 
 The idea is to have a framework (based on e.g. sklearn and torch) that can be used by people not being experienced programmers as they mainly have to adapt an initialization parameter file per experiment.
 
-* The latest features can be seen at [the ini-file options](./ini_file.md) that are used to control Nkululeko
+* The latest features can be seen in [the ini-file](./ini_file.md) options](./ini_file.md) that are used to control Nkululeko
 * Below is a [Hello World example](#helloworld) that should set you up fastly.
 * [Here's a blog post on how to set up nkululeko on your computer.](http://blog.syntheticspeech.de/2021/08/30/how-to-set-up-your-first-nkululeko-project/)
 * [Here's a slide presentation about nkululeko](docs/nkululeko.pdf)
 * [Here's a video presentation about nkululeko](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * [Here's the 2022 LREC article on nkululeko](http://felix.syntheticspeech.de/publications/Nkululeko_LREC.pdf)
 
 Here are some examples of typical output:
 
 ### Confusion matrix
-Per default, Nkululeko displays results as a  confusion matrix, using binning with regression.
+Per default, Nkululeko displays results as a confusion matrix using binning with regression.
 
 <img src="images/conf_mat.png" width="500px"/>
 
 ### Epoch progression
 The point when overfitting starts can sometimes be seen by looking at the results per epoch:
 
 <img src="images/epoch_progression.png" width="500px"/>
@@ -47,15 +47,15 @@
 ### Data distribution
 Sometimes you only want to take a look at your data:
 
 <img src="images/data_plot.png" width="500px"/>
 
 ## Installation
 
-Create and activate a virtual python environment and simply run
+Create and activate a virtual Python environment and simply run
 ```
 pip install nkululeko
 ```
 
 Some examples for *ini*-files (which you use to control nkululeko) are in the [tests folder](https://github.com/felixbur/nkululeko/tree/main/tests).
 
 
@@ -79,20 +79,21 @@
 type = ['praat']
 [MODEL]
 type = svm
 [EXPL]
 model = tree
 plot_tree = True
 [PLOT]
-combine_per_speaker = True
+combine_per_speaker = mode
 ```
+Read the [Hello World example](#hello-world-example) for initial usage with Emo-DB dataset.
 
 Here is an overview of the interfaces:
 * **nkululeko.nkululeko**: doing experiments
-* **nkululeko.demo**: demo the current best model on commandline
+* **nkululeko.demo**: demo the current best model on command line
 * **nkululeko.test**: predict a series of files with the current best model
 * **nkululeko.explore**: perform data exploration
 * **nkululeko.augment**: augment the current training data
 
 Alternatively, there is a central "experiment" class that can be used by own experiments
 
 There's my [blog](http://blog.syntheticspeech.de/?s=nkululeko) with tutorials:
@@ -120,58 +121,59 @@
 * [Run multiple experiments in one go](http://blog.syntheticspeech.de/2022/03/28/how-to-run-multiple-experiments-in-one-go-with-nkululeko/)
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
+ * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework.
 ![sketch](images/class_diagram.png)
 
-Currently the following linear classifiers are implemented (integrated from sklearn):
+Currently, the following linear classifiers are implemented (integrated from sklearn):
 * SVM, SVR, XGB, XGR, Tree, Tree_regressor, KNN, KNN_regressor, NaiveBayes, GMM
   and the following ANNs
 * MLP, CNN (tbd)
 
 Here's [an animation that shows the progress of classification done with nkululeko](https://youtu.be/6Y0M382GjvM)
 
 ### Initialization file
 You could 
 * use a generic main python file (like my_experiment.py), 
 * adapt the path to your nkululeko src 
 * and then adapt an .ini file (again fitting at least the paths to src and data)
   
-Here's [an overview on the ini-file options](./ini_file.md)
+Here's [an overview of the ini-file options](./ini_file.md)
 
 ### <a name="helloworld">Hello World example</a>
-* NEW [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
+* NEW: [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * Set up Python on your computer, version >= 3.6
 * Open a terminal/commandline/console window
 * Test python by typing ```python```, python should start with version >3 (NOT 2!). You can leave the Python Interpreter by typing *exit()*
-* Create a folder on your computer for this example, let's call it *nkulu_work*
-* Get a copy of the [Berlin emodb in audformat](https://tubcloud.tu-berlin.de/s/LfkysdXJfiobiEG) and unpack the same folder (*nkulu_work*)
+* Create a folder on your computer for this example, let's call it `nkulu_work`
+* Get a copy of the [Berlin emodb in audformat](https://tubcloud.tu-berlin.de/s/LfkysdXJfiobiEG) and unpack the same folder (`nkulu_work`)
 * Make sure the folder is called "emodb" and does contain the database files directly (not box-in-a-box)
-* Also, in the *nkulu_work* folder: 
-  * Create a python environment
+* Also, in the `nkulu_work` folder: 
+  * Create a Python environment
     * ```python -m venv venv```
   * Then, activate it:
-    * under linux / mac
+    * under Linux / mac
       * ```source venv/bin/activate```
     * under Windows
       * ```venv\Scripts\activate.bat```
     * if that worked, you should see a ```(venv)``` in front of your prompt
   * Install the required packages in your environment
     * ```pip install nkululeko```
     * Repeat until all error messages vanished (or fix them, or try to ignore them)...
 * Now you should have two folders in your *nkulu_work* folder:
   * *emodb* and *venv*
-* Download a copy of the file [exp_emodb.ini](demos/exp_emodb.ini)
+* Download a copy of the file [exp_emodb.ini](demos/exp_emodb.ini) to the current working directory (```nkulu_work```)
 * Run the demo
   * ```python -m nkululeko.nkululeko --config exp_emodb.ini```
 * Find the results in the newly created folder exp_emodb 
   * Inspect ```exp_emodb/images/run_0/emodb_xgb_os_0_000_cnf.png```
   * This is the main result of you experiment: a confusion matrix for the emodb emotional categories
 * Inspect and play around with the [demo configuration file](demos/exp_emodb.ini) that defined your experiment, then re-run.
 * There are many ways to experiment with different classifiers and acoustic features sets, [all described here](https://github.com/felixbur/nkululeko/blob/main/ini_file.md)
@@ -182,11 +184,11 @@
 * Feature scaling
 * Label encoding
 * Binning (continuous to categorical)
 * Online demo interface for trained models 
 
 ### Outlook
 * Classifiers: CNN
-* Feature extractors: mid level descriptors, Mel-spectra
+* Feature extractors: mid-level descriptors, Mel-spectra
 
-## Licence
+## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
```

### Comparing `nkululeko-0.44.0/nkululeko/augment.py` & `nkululeko-0.44.1/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/augmenter.py` & `nkululeko-0.44.1/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/cacheddataset.py` & `nkululeko-0.44.1/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/dataset.py` & `nkululeko-0.44.1/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/dataset_csv.py` & `nkululeko-0.44.1/nkululeko/dataset_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,18 @@
         root = self.util.config_val_data(self.name, '', '')
         absolut_path = eval(self.util.config_val_data(self.name, 'absolute_path', True))
         self.util.debug(f'loading {self.name}')
 #        df = pd.read_csv(root, index_col='file')       
         df = audformat.utils.read_csv(root)       
         if not absolut_path:
             # add the root folder to the relative paths of the files 
-            #df = df.set_index(df.index.to_series().apply(lambda x: os.path.dirname(root)+'/'+x))
-            df = df.set_index(df.index.set_levels(df.index.levels[0].map(lambda x: os.path.dirname(root)+'/'+x), 0))
+            if audformat.index_type(df.index) == 'segmented':
+                df = df.set_index(df.index.set_levels(df.index.levels[0].map(lambda x: os.path.dirname(root)+'/'+x), 0))
+            else:
+                df = df.set_index(df.index.to_series().apply(lambda x: os.path.dirname(root)+'/'+x)) 
         self.df = df
         self.db = None
         self.got_target = True
         self.is_labeled = self.got_target
         self.start_fresh = eval(self.util.config_val('DATA', 'no_reuse', 'False'))
         if self.is_labeled and not 'class_label' in self.df.columns:
             self.df['class_label'] = self.df[self.target]
```

### Comparing `nkululeko-0.44.0/nkululeko/dataset_ravdess.py` & `nkululeko-0.44.1/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/demo.py` & `nkululeko-0.44.1/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/demo_predictor.py` & `nkululeko-0.44.1/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/experiment.py` & `nkululeko-0.44.1/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/explore.py` & `nkululeko-0.44.1/nkululeko/explore.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,16 +36,18 @@
     # split into train and test
     expr.fill_train_and_tests()
     util.debug(f'train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}')
 
     plot_feats = eval(util.config_val('EXPL', 'feature_distributions', 'False'))
     tsne = eval(util.config_val('EXPL', 'tsne', 'False'))
     scatter = eval(util.config_val('EXPL', 'scatter', 'False'))
-    if plot_feats or tsne or scatter: 
-        # extract features
+    model_type = util.config_val('EXPL', 'model', False)
+    plot_tree = eval(util.config_val('EXPL', 'plot_tree', 'False'))
+    if plot_feats or tsne or scatter or model_type or plot_tree: 
+        # these investigations need features to explore
         expr.extract_feats()
 
     # explore
     expr.analyse_features()
 
     print('DONE')
```

### Comparing `nkululeko-0.44.0/nkululeko/feats_analyser.py` & `nkululeko-0.44.1/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feats_audmodel.py` & `nkululeko-0.44.1/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feats_clap.py` & `nkululeko-0.44.1/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feats_import.py` & `nkululeko-0.44.1/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feats_mld.py` & `nkululeko-0.44.1/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feats_opensmile.py` & `nkululeko-0.44.1/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feats_oxbow.py` & `nkululeko-0.44.1/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feats_praat.py` & `nkululeko-0.44.1/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feats_trill.py` & `nkululeko-0.44.1/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feats_wav2vec2.py` & `nkululeko-0.44.1/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feature_extractor.py` & `nkululeko-0.44.1/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/featureset.py` & `nkululeko-0.44.1/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/feinberg_praat.py` & `nkululeko-0.44.1/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/filter_data.py` & `nkululeko-0.44.1/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/loss_ccc.py` & `nkululeko-0.44.1/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/loss_softf1loss.py` & `nkululeko-0.44.1/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/model.py` & `nkululeko-0.44.1/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/model_cnn.py` & `nkululeko-0.44.1/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/model_gmm.py` & `nkululeko-0.44.1/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/model_knn.py` & `nkululeko-0.44.1/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/model_knn_reg.py` & `nkululeko-0.44.1/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/model_mlp.py` & `nkululeko-0.44.1/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/model_mlp_regression.py` & `nkululeko-0.44.1/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/model_svm.py` & `nkululeko-0.44.1/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/modelrunner.py` & `nkululeko-0.44.1/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/nkululeko.py` & `nkululeko-0.44.1/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/plots.py` & `nkululeko-0.44.1/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/reporter.py` & `nkululeko-0.44.1/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/runmanager.py` & `nkululeko-0.44.1/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/scaler.py` & `nkululeko-0.44.1/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/test.py` & `nkululeko-0.44.1/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/test_predictor.py` & `nkululeko-0.44.1/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko/util.py` & `nkululeko-0.44.1/nkululeko/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.44.0/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.44.1/nkululeko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.44.0
+Version: 0.44.1
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,29 +18,29 @@
 * [Overview](#overview)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Hello World](#hello-world-example)
 * [Licence](#licence)
 
 ## Overview
-A project to detect speaker characteristics by machine learning experiments with a high level interface.
+A project to detect speaker characteristics by machine learning experiments with a high-level interface.
 
 The idea is to have a framework (based on e.g. sklearn and torch) that can be used by people not being experienced programmers as they mainly have to adapt an initialization parameter file per experiment.
 
-* The latest features can be seen at [the ini-file options](./ini_file.md) that are used to control Nkululeko
+* The latest features can be seen in [the ini-file](./ini_file.md) options](./ini_file.md) that are used to control Nkululeko
 * Below is a [Hello World example](#helloworld) that should set you up fastly.
 * [Here's a blog post on how to set up nkululeko on your computer.](http://blog.syntheticspeech.de/2021/08/30/how-to-set-up-your-first-nkululeko-project/)
 * [Here's a slide presentation about nkululeko](docs/nkululeko.pdf)
 * [Here's a video presentation about nkululeko](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * [Here's the 2022 LREC article on nkululeko](http://felix.syntheticspeech.de/publications/Nkululeko_LREC.pdf)
 
 Here are some examples of typical output:
 
 ### Confusion matrix
-Per default, Nkululeko displays results as a  confusion matrix, using binning with regression.
+Per default, Nkululeko displays results as a confusion matrix using binning with regression.
 
 <img src="images/conf_mat.png" width="500px"/>
 
 ### Epoch progression
 The point when overfitting starts can sometimes be seen by looking at the results per epoch:
 
 <img src="images/epoch_progression.png" width="500px"/>
@@ -63,15 +63,15 @@
 ### Data distribution
 Sometimes you only want to take a look at your data:
 
 <img src="images/data_plot.png" width="500px"/>
 
 ## Installation
 
-Create and activate a virtual python environment and simply run
+Create and activate a virtual Python environment and simply run
 ```
 pip install nkululeko
 ```
 
 Some examples for *ini*-files (which you use to control nkululeko) are in the [tests folder](https://github.com/felixbur/nkululeko/tree/main/tests).
 
 
@@ -95,20 +95,21 @@
 type = ['praat']
 [MODEL]
 type = svm
 [EXPL]
 model = tree
 plot_tree = True
 [PLOT]
-combine_per_speaker = True
+combine_per_speaker = mode
 ```
+Read the [Hello World example](#hello-world-example) for initial usage with Emo-DB dataset.
 
 Here is an overview of the interfaces:
 * **nkululeko.nkululeko**: doing experiments
-* **nkululeko.demo**: demo the current best model on commandline
+* **nkululeko.demo**: demo the current best model on command line
 * **nkululeko.test**: predict a series of files with the current best model
 * **nkululeko.explore**: perform data exploration
 * **nkululeko.augment**: augment the current training data
 
 Alternatively, there is a central "experiment" class that can be used by own experiments
 
 There's my [blog](http://blog.syntheticspeech.de/?s=nkululeko) with tutorials:
@@ -136,58 +137,59 @@
 * [Run multiple experiments in one go](http://blog.syntheticspeech.de/2022/03/28/how-to-run-multiple-experiments-in-one-go-with-nkululeko/)
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
+ * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework.
 ![sketch](images/class_diagram.png)
 
-Currently the following linear classifiers are implemented (integrated from sklearn):
+Currently, the following linear classifiers are implemented (integrated from sklearn):
 * SVM, SVR, XGB, XGR, Tree, Tree_regressor, KNN, KNN_regressor, NaiveBayes, GMM
   and the following ANNs
 * MLP, CNN (tbd)
 
 Here's [an animation that shows the progress of classification done with nkululeko](https://youtu.be/6Y0M382GjvM)
 
 ### Initialization file
 You could 
 * use a generic main python file (like my_experiment.py), 
 * adapt the path to your nkululeko src 
 * and then adapt an .ini file (again fitting at least the paths to src and data)
   
-Here's [an overview on the ini-file options](./ini_file.md)
+Here's [an overview of the ini-file options](./ini_file.md)
 
 ### <a name="helloworld">Hello World example</a>
-* NEW [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
+* NEW: [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * Set up Python on your computer, version >= 3.6
 * Open a terminal/commandline/console window
 * Test python by typing ```python```, python should start with version >3 (NOT 2!). You can leave the Python Interpreter by typing *exit()*
-* Create a folder on your computer for this example, let's call it *nkulu_work*
-* Get a copy of the [Berlin emodb in audformat](https://tubcloud.tu-berlin.de/s/LfkysdXJfiobiEG) and unpack the same folder (*nkulu_work*)
+* Create a folder on your computer for this example, let's call it `nkulu_work`
+* Get a copy of the [Berlin emodb in audformat](https://tubcloud.tu-berlin.de/s/LfkysdXJfiobiEG) and unpack the same folder (`nkulu_work`)
 * Make sure the folder is called "emodb" and does contain the database files directly (not box-in-a-box)
-* Also, in the *nkulu_work* folder: 
-  * Create a python environment
+* Also, in the `nkulu_work` folder: 
+  * Create a Python environment
     * ```python -m venv venv```
   * Then, activate it:
-    * under linux / mac
+    * under Linux / mac
       * ```source venv/bin/activate```
     * under Windows
       * ```venv\Scripts\activate.bat```
     * if that worked, you should see a ```(venv)``` in front of your prompt
   * Install the required packages in your environment
     * ```pip install nkululeko```
     * Repeat until all error messages vanished (or fix them, or try to ignore them)...
 * Now you should have two folders in your *nkulu_work* folder:
   * *emodb* and *venv*
-* Download a copy of the file [exp_emodb.ini](demos/exp_emodb.ini)
+* Download a copy of the file [exp_emodb.ini](demos/exp_emodb.ini) to the current working directory (```nkulu_work```)
 * Run the demo
   * ```python -m nkululeko.nkululeko --config exp_emodb.ini```
 * Find the results in the newly created folder exp_emodb 
   * Inspect ```exp_emodb/images/run_0/emodb_xgb_os_0_000_cnf.png```
   * This is the main result of you experiment: a confusion matrix for the emodb emotional categories
 * Inspect and play around with the [demo configuration file](demos/exp_emodb.ini) that defined your experiment, then re-run.
 * There are many ways to experiment with different classifiers and acoustic features sets, [all described here](https://github.com/felixbur/nkululeko/blob/main/ini_file.md)
@@ -198,22 +200,27 @@
 * Feature scaling
 * Label encoding
 * Binning (continuous to categorical)
 * Online demo interface for trained models 
 
 ### Outlook
 * Classifiers: CNN
-* Feature extractors: mid level descriptors, Mel-spectra
+* Feature extractors: mid-level descriptors, Mel-spectra
 
-## Licence
+## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.44.1
+--------------
+* bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
+* bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
+
 Version 0.44.0
 --------------
 * added scatter functions: tsne, pca, umap
 
 Version 0.43.7
 --------------
 * added clap features
```

### Comparing `nkululeko-0.44.0/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.44.1/nkululeko.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 nkululeko/model_xgb.py
 nkululeko/model_xgr.py
 nkululeko/modelrunner.py
 nkululeko/nkululeko.py
 nkululeko/plots.py
 nkululeko/reporter.py
 nkululeko/result.py
-nkululeko/runmanager copy.py
 nkululeko/runmanager.py
 nkululeko/scaler.py
 nkululeko/test.py
 nkululeko/test_predictor.py
 nkululeko/util.py
 nkululeko.egg-info/PKG-INFO
 nkululeko.egg-info/SOURCES.txt
```

### Comparing `nkululeko-0.44.0/setup.cfg` & `nkululeko-0.44.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nkululeko
-version = 0.44.0
+version = 0.44.1
 author = Felix Burkhardt
 author_email = fxburk@gmail.com
 description = Machine learning audio prediction experiments based on templates
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/felixbur/nkululeko
 classifiers =
```


# Comparing `tmp/dvclive-2.7.0.tar.gz` & `tmp/dvclive-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvclive-2.7.0.tar", last modified: Mon Apr 24 08:54:15 2023, max compression
+gzip compressed data, was "dvclive-2.8.0.tar", last modified: Thu Apr 27 16:09:24 2023, max compression
```

## Comparing `dvclive-2.7.0.tar` & `dvclive-2.8.0.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.291425 dvclive-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-24 08:54:03.000000 dvclive-2.7.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 08:54:03.000000 dvclive-2.7.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.279425 dvclive-2.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-24 08:54:03.000000 dvclive-2.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-24 08:54:03.000000 dvclive-2.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.283425 dvclive-2.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-24 08:54:03.000000 dvclive-2.7.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-24 08:54:03.000000 dvclive-2.7.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-24 08:54:03.000000 dvclive-2.7.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-24 08:54:03.000000 dvclive-2.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-24 08:54:03.000000 dvclive-2.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-24 08:54:03.000000 dvclive-2.7.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 08:54:03.000000 dvclive-2.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-24 08:54:03.000000 dvclive-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-24 08:54:15.291425 dvclive-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-24 08:54:03.000000 dvclive-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.283425 dvclive-2.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   321138 2023-04-24 08:54:03.000000 dvclive-2.7.0/docs/dvc_plots_diff.png
--rw-r--r--   0 runner    (1001) docker     (123)   676021 2023-04-24 08:54:03.000000 dvclive-2.7.0/docs/studio_compare.png
--rw-r--r--   0 runner    (1001) docker     (123)   501824 2023-04-24 08:54:03.000000 dvclive-2.7.0/docs/vscode_experiments.png
--rw-r--r--   0 runner    (1001) docker     (123)   627561 2023-04-24 08:54:03.000000 dvclive-2.7.0/docs/vscode_plots.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.283425 dvclive-2.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-04-24 08:54:03.000000 dvclive-2.7.0/examples/DVCLive-Quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-24 08:54:03.000000 dvclive-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-24 08:54:15.291425 dvclive-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 08:54:03.000000 dvclive-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.279425 dvclive-2.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.287425 dvclive-2.7.0/src/dvclive/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)    19834 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/optuna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.287425 dvclive-2.7.0/src/dvclive/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.287425 dvclive-2.7.0/src/dvclive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.287425 dvclive-2.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.291425 dvclive-2.7.0/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/plots/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/plots/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/plots/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_dvc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.291425 dvclive-2.7.0/tests/test_frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_log_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.841721 dvclive-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-27 16:09:05.000000 dvclive-2.8.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 16:09:05.000000 dvclive-2.8.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.821719 dvclive-2.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 16:09:05.000000 dvclive-2.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 16:09:05.000000 dvclive-2.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.825719 dvclive-2.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-27 16:09:05.000000 dvclive-2.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-27 16:09:05.000000 dvclive-2.8.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 16:09:05.000000 dvclive-2.8.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-27 16:09:05.000000 dvclive-2.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-27 16:09:05.000000 dvclive-2.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-27 16:09:05.000000 dvclive-2.8.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-27 16:09:05.000000 dvclive-2.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-27 16:09:05.000000 dvclive-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-27 16:09:24.841721 dvclive-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-27 16:09:05.000000 dvclive-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.825719 dvclive-2.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   321138 2023-04-27 16:09:05.000000 dvclive-2.8.0/docs/dvc_plots_diff.png
+-rw-r--r--   0 runner    (1001) docker     (123)   676021 2023-04-27 16:09:05.000000 dvclive-2.8.0/docs/studio_compare.png
+-rw-r--r--   0 runner    (1001) docker     (123)   501824 2023-04-27 16:09:06.000000 dvclive-2.8.0/docs/vscode_experiments.png
+-rw-r--r--   0 runner    (1001) docker     (123)   627561 2023-04-27 16:09:06.000000 dvclive-2.8.0/docs/vscode_plots.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.825719 dvclive-2.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-04-27 16:09:06.000000 dvclive-2.8.0/examples/DVCLive-Quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-27 16:09:06.000000 dvclive-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-27 16:09:24.841721 dvclive-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 16:09:06.000000 dvclive-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.821719 dvclive-2.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.829720 dvclive-2.8.0/src/dvclive/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/optuna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.833720 dvclive-2.8.0/src/dvclive/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.833720 dvclive-2.8.0/src/dvclive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.837720 dvclive-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.837720 dvclive-2.8.0/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/plots/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/plots/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/plots/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/plots/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_dvc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.841721 dvclive-2.8.0/tests/test_frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_log_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_utils.py
```

### Comparing `dvclive-2.7.0/.cruft.json` & `dvclive-2.8.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/.github/dependabot.yml` & `dvclive-2.8.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/.github/workflows/release.yml` & `dvclive-2.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/.github/workflows/tests.yml` & `dvclive-2.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/.gitignore` & `dvclive-2.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/.pre-commit-config.yaml` & `dvclive-2.8.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
       - id: codespell
         additional_dependencies: ["tomli"]
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.261'
+    rev: 'v0.0.262'
     hooks:
       - id: ruff
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
     - id: mdformat
       args: ["--wrap=80"]
```

### Comparing `dvclive-2.7.0/CODE_OF_CONDUCT.rst` & `dvclive-2.8.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/CONTRIBUTING.rst` & `dvclive-2.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/LICENSE` & `dvclive-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/PKG-INFO` & `dvclive-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvclive
-Version: 2.7.0
+Version: 2.8.0
 Summary: Metric logger for ML projects.
 Home-page: https://github.com/iterative/dvclive
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Project-URL: Documentation, https://dvc.org/doc/dvclive
 Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dvclive Version: 2.7.0 Summary: Metric logger for
+Metadata-Version: 2.1 Name: dvclive Version: 2.8.0 Summary: Metric logger for
 ML projects. Home-page: https://github.com/iterative/dvclive Maintainer-email:
 support@dvc.org License: Apache-2.0 Project-URL: Documentation, https://
 dvc.org/doc/dvclive Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai Platform:
 any Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `dvclive-2.7.0/README.md` & `dvclive-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/docs/dvc_plots_diff.png` & `dvclive-2.8.0/docs/dvc_plots_diff.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/docs/studio_compare.png` & `dvclive-2.8.0/docs/studio_compare.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/docs/vscode_experiments.png` & `dvclive-2.8.0/docs/vscode_experiments.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/docs/vscode_plots.png` & `dvclive-2.8.0/docs/vscode_plots.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/examples/DVCLive-Quickstart.ipynb` & `dvclive-2.8.0/examples/DVCLive-Quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/pyproject.toml` & `dvclive-2.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/setup.cfg` & `dvclive-2.8.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,18 @@
 sklearn = 
 	scikit-learn
 plots = 
 	%(sklearn)s
 markdown = 
 	matplotlib
 tests = 
-	pytest==7.2.0
-	pytest-sugar==0.9.5
-	pytest-cov==3.0.0
-	pytest-mock==3.8.2
+	pytest>=7.2.0,<8.0
+	pytest-sugar>=0.9.6,<1.0
+	pytest-cov>=3.0.0,<4.0
+	pytest-mock>=3.8.2,<4.0
 	%(image)s
 	%(plots)s
 	%(markdown)s
 	ipython
 dev = 
 	%(tests)s
 	%(all)s
```

### Comparing `dvclive-2.7.0/src/dvclive/catalyst.py` & `dvclive-2.8.0/src/dvclive/catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/dvc.py` & `dvclive-2.8.0/src/dvclive/dvc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 # ruff: noqa: SLF001
-import logging
 import os
 import random
 from pathlib import Path
 
 from dvclive import env
 from dvclive.plots import Image, Metric
 from dvclive.serialize import dump_yaml
 
-logging.basicConfig()
-logger = logging.getLogger("dvclive")
-logger.setLevel(os.getenv(env.DVCLIVE_LOGLEVEL, "INFO").upper())
-
 _CHECKPOINT_SLEEP = 0.1
 
 
 def _dvc_dir(dirname):
     return os.path.join(dirname, ".dvc")
 
 
@@ -102,15 +97,15 @@
         plots.append(metrics_config)
     if live._images:
         images_path = (plots_path / Image.subfolder).relative_to(live.dir)
         plots.append(images_path.as_posix())
     if live._plots:
         for plot in live._plots.values():
             plot_path = plot.output_path.relative_to(live.dir)
-            plots.append({plot_path.as_posix(): plot.get_properties()})
+            plots.append({plot_path.as_posix(): plot.plot_config})
     if plots:
         dvcyaml["plots"] = plots
 
     if live._artifacts:
         dvcyaml["artifacts"] = live._artifacts
         for artifact in dvcyaml["artifacts"].values():
             abs_path = os.path.realpath(artifact["path"])
```

### Comparing `dvclive-2.7.0/src/dvclive/error.py` & `dvclive-2.8.0/src/dvclive/error.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/fastai.py` & `dvclive-2.8.0/src/dvclive/fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/huggingface.py` & `dvclive-2.8.0/src/dvclive/huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/keras.py` & `dvclive-2.8.0/src/dvclive/keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/lgbm.py` & `dvclive-2.8.0/src/dvclive/lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/lightning.py` & `dvclive-2.8.0/src/dvclive/lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/live.py` & `dvclive-2.8.0/src/dvclive/live.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,25 @@
 )
 from .error import (
     InvalidDataTypeError,
     InvalidParameterTypeError,
     InvalidPlotTypeError,
     InvalidReportModeError,
 )
-from .plots import PLOT_TYPES, SKLEARN_PLOTS, Image, Metric, NumpyEncoder
+from .plots import PLOT_TYPES, SKLEARN_PLOTS, CustomPlot, Image, Metric, NumpyEncoder
 from .report import BLANK_NOTEBOOK_REPORT, make_report
 from .serialize import dump_json, dump_yaml, load_yaml
 from .studio import get_studio_updates
 from .utils import env2bool, inside_notebook, matplotlib_installed, open_file_in_browser
 
-logging.basicConfig()
 logger = logging.getLogger("dvclive")
+handler = logging.StreamHandler()
+formatter = logging.Formatter("%(levelname)s:%(name)s:%(message)s")
+handler.setFormatter(formatter)
+logger.addHandler(handler)
 logger.setLevel(os.getenv(env.DVCLIVE_LOGLEVEL, "INFO").upper())
 
 ParamLike = Union[int, float, str, bool, List["ParamLike"], Dict[str, "ParamLike"]]
 StrPath = Union[str, Path]
 
 
 class Live:
@@ -257,58 +260,99 @@
         self.step += 1
 
     def log_metric(self, name: str, val: Union[int, float], timestamp: bool = False):
         if not Metric.could_log(val):
             raise InvalidDataTypeError(name, type(val))
 
         if name in self._metrics:
-            data = self._metrics[name]
+            metric = self._metrics[name]
         else:
-            data = Metric(name, self.plots_dir)
-            self._metrics[name] = data
+            metric = Metric(name, self.plots_dir)
+            self._metrics[name] = metric
 
-        data.step = self.step
-        data.dump(val, timestamp=timestamp)
+        metric.step = self.step
+        metric.dump(val, timestamp=timestamp)
 
-        self.summary = set_in(self.summary, data.summary_keys, val)
+        self.summary = set_in(self.summary, metric.summary_keys, val)
         logger.debug(f"Logged {name}: {val}")
 
     def log_image(self, name: str, val):
         if not Image.could_log(val):
             raise InvalidDataTypeError(name, type(val))
 
         if isinstance(val, (str, Path)):
             from PIL import Image as ImagePIL
 
             val = ImagePIL.open(val)
 
         if name in self._images:
-            data = self._images[name]
+            image = self._images[name]
         else:
-            data = Image(name, self.plots_dir)
-            self._images[name] = data
+            image = Image(name, self.plots_dir)
+            self._images[name] = image
 
-        data.step = self.step
-        data.dump(val)
+        image.step = self.step
+        image.dump(val)
         logger.debug(f"Logged {name}: {val}")
 
+    def log_plot(
+        self,
+        name: str,
+        datapoints: List[Dict],
+        x: str,
+        y: str,
+        template: Optional[str] = None,
+        title: Optional[str] = None,
+        x_label: Optional[str] = None,
+        y_label: Optional[str] = None,
+    ):
+        if not CustomPlot.could_log(datapoints):
+            raise InvalidDataTypeError(name, type(datapoints))
+
+        if name in self._plots:
+            plot = self._plots[name]
+        else:
+            plot = CustomPlot(
+                name,
+                self.plots_dir,
+                x=x,
+                y=y,
+                template=template,
+                title=title,
+                x_label=x_label,
+                y_label=y_label,
+            )
+            self._plots[name] = plot
+
+        plot.step = self.step
+        plot.dump(datapoints)
+        logger.debug(f"Logged {name}")
+
     def log_sklearn_plot(self, kind, labels, predictions, name=None, **kwargs):
         val = (labels, predictions)
 
+        plot_config = {
+            k: v
+            for k, v in kwargs.items()
+            if k in ("title", "x_label", "y_label", "normalized")
+        }
         name = name or kind
         if name in self._plots:
-            data = self._plots[name]
+            plot = self._plots[name]
         elif kind in SKLEARN_PLOTS and SKLEARN_PLOTS[kind].could_log(val):
-            data = SKLEARN_PLOTS[kind](name, self.plots_dir, **kwargs)
-            self._plots[data.name] = data
+            plot = SKLEARN_PLOTS[kind](name, self.plots_dir, **plot_config)
+            self._plots[plot.name] = plot
         else:
             raise InvalidPlotTypeError(name)
 
-        data.step = self.step
-        data.dump(val, **kwargs)
+        sklearn_kwargs = {
+            k: v for k, v in kwargs.items() if k not in plot_config or k != "normalized"
+        }
+        plot.step = self.step
+        plot.dump(val, **sklearn_kwargs)
         logger.debug(f"Logged {name}")
 
     def _read_params(self):
         if os.path.isfile(self.params_file):
             params = load_yaml(self.params_file)
             self._params.update(params)
```

### Comparing `dvclive-2.7.0/src/dvclive/optuna.py` & `dvclive-2.8.0/src/dvclive/optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/plots/base.py` & `dvclive-2.8.0/src/dvclive/plots/base.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/plots/image.py` & `dvclive-2.8.0/src/dvclive/plots/image.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/plots/metric.py` & `dvclive-2.8.0/src/dvclive/plots/metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/plots/utils.py` & `dvclive-2.8.0/src/dvclive/plots/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/report.py` & `dvclive-2.8.0/src/dvclive/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dvc_render.html import render_html
 from dvc_render.image import ImageRenderer
 from dvc_render.markdown import render_markdown
 from dvc_render.table import TableRenderer
 from dvc_render.vega import VegaRenderer
 
 from dvclive.error import InvalidReportModeError
-from dvclive.plots import SKLEARN_PLOTS, Image, Metric
+from dvclive.plots import SKLEARN_PLOTS, CustomPlot, Image, Metric
 from dvclive.plots.sklearn import SKLearnPlot
 from dvclive.serialize import load_yaml
 from dvclive.utils import inside_colab, parse_tsv
 
 if TYPE_CHECKING:
     from dvclive import Live
 
@@ -82,25 +82,43 @@
                     ImageRenderer.TITLE_FIELD: name,
                 }
             ]
             renderers.append(ImageRenderer(data, name))
     return renderers
 
 
-def get_plot_renderers(plots_folder, live):
+def get_custom_plot_renderers(plots_folder, live):
+    renderers = []
+    for suffix in CustomPlot.suffixes:
+        for file in Path(plots_folder).rglob(f"*{suffix}"):
+            name = file.relative_to(plots_folder).with_suffix("").as_posix()
+
+            logged_plot = live._plots[name]
+            properties = logged_plot.plot_config
+
+            data = json.loads(file.read_text())
+
+            for row in data:
+                row["rev"] = "workspace"
+
+            renderers.append(VegaRenderer(data, name, **properties))
+    return renderers
+
+
+def get_sklearn_plot_renderers(plots_folder, live):
     renderers = []
     for suffix in SKLearnPlot.suffixes:
         for file in Path(plots_folder).rglob(f"*{suffix}"):
             name = file.relative_to(plots_folder).with_suffix("").as_posix()
             properties = {}
 
             logged_plot = live._plots[name]
             for default_name, plot_class in SKLEARN_PLOTS.items():
                 if isinstance(logged_plot, plot_class):
-                    properties = logged_plot.get_properties()
+                    properties = logged_plot.plot_config
                     data_field = default_name
                     break
 
             data = json.loads(file.read_text())
 
             if data_field in data:
                 data = data[data_field]
@@ -142,15 +160,18 @@
     renderers = []
     renderers.extend(get_params_renderers(live.params_file))
     renderers.extend(get_metrics_renderers(live.metrics_file))
     renderers.extend(get_scalar_renderers(plots_path / Metric.subfolder))
     renderers.extend(
         get_image_renderers(plots_path / Image.subfolder, report_mode=live._report_mode)
     )
-    renderers.extend(get_plot_renderers(plots_path / SKLearnPlot.subfolder, live))
+    renderers.extend(
+        get_sklearn_plot_renderers(plots_path / SKLearnPlot.subfolder, live)
+    )
+    renderers.extend(get_custom_plot_renderers(plots_path / CustomPlot.subfolder, live))
 
     if live._report_mode == "html":
         render_html(renderers, live.report_file, refresh_seconds=5)
     elif live._report_mode == "notebook":
         from IPython.display import HTML, IFrame
 
         render_html(
```

### Comparing `dvclive-2.7.0/src/dvclive/serialize.py` & `dvclive-2.8.0/src/dvclive/serialize.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/studio.py` & `dvclive-2.8.0/src/dvclive/studio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # ruff: noqa: SLF001
-import logging
 import os
 from pathlib import Path
 
 from dvclive.serialize import load_yaml
 from dvclive.utils import parse_metrics
 
-logger = logging.getLogger(__name__)
-
 
 def _get_unsent_datapoints(plot, latest_step):
     return [x for x in plot if int(x["step"]) > latest_step]
 
 
 def _cast_to_numbers(datapoints):
     for datapoint in datapoints:
```

### Comparing `dvclive-2.7.0/src/dvclive/utils.py` & `dvclive-2.8.0/src/dvclive/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive/xgb.py` & `dvclive-2.8.0/src/dvclive/xgb.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/src/dvclive.egg-info/PKG-INFO` & `dvclive-2.8.0/src/dvclive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvclive
-Version: 2.7.0
+Version: 2.8.0
 Summary: Metric logger for ML projects.
 Home-page: https://github.com/iterative/dvclive
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Project-URL: Documentation, https://dvc.org/doc/dvclive
 Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dvclive Version: 2.7.0 Summary: Metric logger for
+Metadata-Version: 2.1 Name: dvclive Version: 2.8.0 Summary: Metric logger for
 ML projects. Home-page: https://github.com/iterative/dvclive Maintainer-email:
 support@dvc.org License: Apache-2.0 Project-URL: Documentation, https://
 dvc.org/doc/dvclive Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai Platform:
 any Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `dvclive-2.7.0/src/dvclive.egg-info/SOURCES.txt` & `dvclive-2.8.0/src/dvclive.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -40,26 +40,28 @@
 src/dvclive.egg-info/SOURCES.txt
 src/dvclive.egg-info/dependency_links.txt
 src/dvclive.egg-info/not-zip-safe
 src/dvclive.egg-info/requires.txt
 src/dvclive.egg-info/top_level.txt
 src/dvclive/plots/__init__.py
 src/dvclive/plots/base.py
+src/dvclive/plots/custom.py
 src/dvclive/plots/image.py
 src/dvclive/plots/metric.py
 src/dvclive/plots/sklearn.py
 src/dvclive/plots/utils.py
 tests/__init__.py
 tests/conftest.py
 tests/test_dvc.py
 tests/test_log_artifact.py
 tests/test_main.py
 tests/test_report.py
 tests/test_studio.py
 tests/test_utils.py
+tests/plots/test_custom.py
 tests/plots/test_image.py
 tests/plots/test_metric.py
 tests/plots/test_sklearn.py
 tests/test_frameworks/test_catalyst.py
 tests/test_frameworks/test_fastai.py
 tests/test_frameworks/test_huggingface.py
 tests/test_frameworks/test_keras.py
```

### Comparing `dvclive-2.7.0/src/dvclive.egg-info/requires.txt` & `dvclive-2.8.0/src/dvclive.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 scikit-learn
 matplotlib
 
 [catalyst]
 catalyst>22
 
 [dev]
-pytest==7.2.0
-pytest-sugar==0.9.5
-pytest-cov==3.0.0
-pytest-mock==3.8.2
+pytest<8.0,>=7.2.0
+pytest-sugar<1.0,>=0.9.6
+pytest-cov<4.0,>=3.0.0
+pytest-mock<4.0,>=3.8.2
 numpy
 pillow
 scikit-learn
 matplotlib
 ipython
 mmcv
 tensorflow
@@ -77,18 +77,18 @@
 pytorch_lightning>=1.9
 torch<2.1
 
 [sklearn]
 scikit-learn
 
 [tests]
-pytest==7.2.0
-pytest-sugar==0.9.5
-pytest-cov==3.0.0
-pytest-mock==3.8.2
+pytest<8.0,>=7.2.0
+pytest-sugar<1.0,>=0.9.6
+pytest-cov<4.0,>=3.0.0
+pytest-mock<4.0,>=3.8.2
 numpy
 pillow
 scikit-learn
 matplotlib
 ipython
 
 [tf]
```

### Comparing `dvclive-2.7.0/tests/conftest.py` & `dvclive-2.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/plots/test_image.py` & `dvclive-2.8.0/tests/plots/test_image.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/plots/test_metric.py` & `dvclive-2.8.0/tests/plots/test_metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/plots/test_sklearn.py` & `dvclive-2.8.0/tests/plots/test_sklearn.py`

 * *Files 16% similar despite different names*

```diff
@@ -151,7 +151,31 @@
     live.log_sklearn_plot("confusion_matrix", y_true, y_pred, name="val/cm")
     # ".json" should be stripped from the name
     live.log_sklearn_plot("confusion_matrix", y_true, y_pred, name="cm.json")
 
     assert (out / "train" / "cm.json").exists()
     assert (out / "val" / "cm.json").exists()
     assert (out / "cm.json").exists()
+
+
+def test_custom_title(tmp_dir, y_true_y_pred_y_score):
+    """https://github.com/iterative/dvclive/issues/453"""
+    live = Live()
+    out = tmp_dir / live.plots_dir / SKLearnPlot.subfolder
+
+    y_true, y_pred, _ = y_true_y_pred_y_score
+
+    live.log_sklearn_plot(
+        "confusion_matrix",
+        y_true,
+        y_pred,
+        name="train/cm",
+        title="Train Confusion Matrix",
+    )
+    live.log_sklearn_plot(
+        "confusion_matrix", y_true, y_pred, name="val/cm", title="Val Confusion Matrix"
+    )
+    assert (out / "train" / "cm.json").exists()
+    assert (out / "val" / "cm.json").exists()
+
+    assert live._plots["train/cm"].plot_config["title"] == "Train Confusion Matrix"
+    assert live._plots["val/cm"].plot_config["title"] == "Val Confusion Matrix"
```

### Comparing `dvclive-2.7.0/tests/test_dvc.py` & `dvclive-2.8.0/tests/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_frameworks/test_catalyst.py` & `dvclive-2.8.0/tests/test_frameworks/test_catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_frameworks/test_fastai.py` & `dvclive-2.8.0/tests/test_frameworks/test_fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_frameworks/test_huggingface.py` & `dvclive-2.8.0/tests/test_frameworks/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_frameworks/test_keras.py` & `dvclive-2.8.0/tests/test_frameworks/test_keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_frameworks/test_lgbm.py` & `dvclive-2.8.0/tests/test_frameworks/test_lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_frameworks/test_lightning.py` & `dvclive-2.8.0/tests/test_frameworks/test_lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_frameworks/test_optuna.py` & `dvclive-2.8.0/tests/test_frameworks/test_optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_frameworks/test_xgboost.py` & `dvclive-2.8.0/tests/test_frameworks/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_log_artifact.py` & `dvclive-2.8.0/tests/test_log_artifact.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_main.py` & `dvclive-2.8.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_report.py` & `dvclive-2.8.0/tests/test_report.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 import pytest
 from IPython import display
 from PIL import Image
 
 from dvclive import Live
 from dvclive.env import DVCLIVE_OPEN
 from dvclive.error import InvalidReportModeError
+from dvclive.plots import CustomPlot
 from dvclive.plots import Image as LiveImage
 from dvclive.plots import Metric
-from dvclive.plots.sklearn import ConfusionMatrix, Roc, SKLearnPlot
+from dvclive.plots.sklearn import SKLearnPlot
 from dvclive.report import (
+    get_custom_plot_renderers,
     get_image_renderers,
     get_metrics_renderers,
     get_params_renderers,
-    get_plot_renderers,
     get_scalar_renderers,
+    get_sklearn_plot_renderers,
 )
 
 
 @pytest.mark.parametrize("mode", ["html", "md", "notebook"])
 def test_get_image_renderers(tmp_dir, mode):
     with Live() as live:
         img = Image.new("RGB", (10, 10), (255, 0, 0))
@@ -129,54 +131,85 @@
     live = Live()
     live.log_sklearn_plot("confusion_matrix", [0, 0, 1, 1], [1, 0, 0, 1])
     live.make_report()
 
     mocked_open.assert_called_once()
 
 
-def test_get_plot_renderers(tmp_dir, mocker):
+def test_get_plot_renderers_sklearn(tmp_dir):
     live = Live()
 
     for _ in range(2):
         live.log_sklearn_plot("confusion_matrix", [0, 0, 1, 1], [1, 0, 0, 1])
         live.log_sklearn_plot(
             "confusion_matrix", [0, 0, 1, 1], [1, 0, 0, 1], name="train/cm"
         )
         live.log_sklearn_plot("roc", [0, 0, 1, 1], [1, 0.1, 0, 1], name="roc_curve")
         live.log_sklearn_plot(
             "roc", [0, 0, 1, 1], [1, 0.1, 0, 1], name="other_roc.json"
         )
         live.next_step()
 
-    plot_renderers = get_plot_renderers(
+    plot_renderers = get_sklearn_plot_renderers(
         tmp_dir / live.plots_dir / SKLearnPlot.subfolder, live
     )
     assert len(plot_renderers) == 4
     plot_renderers_dict = {
         plot_renderer.name: plot_renderer for plot_renderer in plot_renderers
     }
     for name in ("roc_curve", "other_roc"):
         plot_renderer = plot_renderers_dict[name]
         assert plot_renderer.datapoints == [
             {"fpr": 0.0, "rev": "workspace", "threshold": 2.0, "tpr": 0.0},
             {"fpr": 0.5, "rev": "workspace", "threshold": 1.0, "tpr": 0.5},
             {"fpr": 1.0, "rev": "workspace", "threshold": 0.1, "tpr": 0.5},
             {"fpr": 1.0, "rev": "workspace", "threshold": 0.0, "tpr": 1.0},
         ]
-        assert plot_renderer.properties == Roc.DEFAULT_PROPERTIES
+        assert plot_renderer.properties == live._plots[name].plot_config
 
     for name in ("confusion_matrix", "train/cm"):
         plot_renderer = plot_renderers_dict[name]
         assert plot_renderer.datapoints == [
             {"actual": "0", "rev": "workspace", "predicted": "1"},
             {"actual": "0", "rev": "workspace", "predicted": "0"},
             {"actual": "1", "rev": "workspace", "predicted": "0"},
             {"actual": "1", "rev": "workspace", "predicted": "1"},
         ]
-        assert plot_renderer.properties == ConfusionMatrix.DEFAULT_PROPERTIES
+        assert plot_renderer.properties == live._plots[name].plot_config
+
+
+def test_get_plot_renderers_custom(tmp_dir):
+    live = Live()
+
+    datapoints = [{"x": 1, "y": 2}, {"x": 3, "y": 4}]
+    for _ in range(2):
+        live.log_plot("foo_default", datapoints, x="x", y="y")
+        live.log_plot(
+            "foo_scatter",
+            datapoints,
+            x="x",
+            y="y",
+            template="scatter",
+        )
+        live.next_step()
+    plot_renderers = get_custom_plot_renderers(
+        tmp_dir / live.plots_dir / CustomPlot.subfolder, live
+    )
+
+    assert len(plot_renderers) == 2
+    plot_renderers_dict = {
+        plot_renderer.name: plot_renderer for plot_renderer in plot_renderers
+    }
+    for name in ("foo_default", "foo_scatter"):
+        plot_renderer = plot_renderers_dict[name]
+        assert plot_renderer.datapoints == [
+            {"rev": "workspace", "x": 1, "y": 2},
+            {"rev": "workspace", "x": 3, "y": 4},
+        ]
+        assert plot_renderer.properties == live._plots[name].plot_config
 
 
 def test_report_auto_doesnt_set_notebook(tmp_dir, mocker):
     mocker.patch("dvclive.live.inside_notebook", return_value=True)
     live = Live()
     assert live._report_mode != "notebook"
```

### Comparing `dvclive-2.7.0/tests/test_studio.py` & `dvclive-2.8.0/tests/test_studio.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.7.0/tests/test_utils.py` & `dvclive-2.8.0/tests/test_utils.py`

 * *Files identical despite different names*


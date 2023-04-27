# Comparing `tmp/autora-theorist-darts-1.0.0a2.tar.gz` & `tmp/autora-theorist-darts-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-darts-1.0.0a2.tar", last modified: Thu Apr 27 19:32:08 2023, max compression
+gzip compressed data, was "autora-theorist-darts-1.0.0a3.tar", last modified: Thu Apr 27 20:19:13 2023, max compression
```

## Comparing `autora-theorist-darts-1.0.0a2.tar` & `autora-theorist-darts-1.0.0a3.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.725180 autora-theorist-darts-1.0.0a2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.709179 autora-theorist-darts-1.0.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.713179 autora-theorist-darts-1.0.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.717179 autora-theorist-darts-1.0.0a2/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/.idea/autora-darts.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.717179 autora-theorist-darts-1.0.0a2/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-27 19:32:08.725180 autora-theorist-darts-1.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.717179 autora-theorist-darts-1.0.0a2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    21439 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/docs/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/docs/how_it_works.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.721179 autora-theorist-darts-1.0.0a2/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   681971 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/docs/img/darts_computation_graph.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.721179 autora-theorist-darts-1.0.0a2/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/docs/meta_parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/docs/search_space.md
--rw-r--r--   0 runner    (1001) docker     (123)   796099 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/docs/weber.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.721179 autora-theorist-darts-1.0.0a2/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/mkdocs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:32:08.725180 autora-theorist-darts-1.0.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.713179 autora-theorist-darts-1.0.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.713179 autora-theorist-darts-1.0.0a2/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.713179 autora-theorist-darts-1.0.0a2/src/autora/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.725180 autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/architect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/fan_out.py
--rw-r--r--   0 runner    (1001) docker     (123)    30660 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/model_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    19820 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    31170 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.725180 autora-theorist-darts-1.0.0a2/src/autora_theorist_darts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-27 19:32:08.000000 autora-theorist-darts-1.0.0a2/src/autora_theorist_darts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-27 19:32:08.000000 autora-theorist-darts-1.0.0a2/src/autora_theorist_darts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:32:08.000000 autora-theorist-darts-1.0.0a2/src/autora_theorist_darts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 19:32:08.000000 autora-theorist-darts-1.0.0a2/src/autora_theorist_darts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 19:32:08.000000 autora-theorist-darts-1.0.0a2/src/autora_theorist_darts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:08.725180 autora-theorist-darts-1.0.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-04-27 19:31:53.000000 autora-theorist-darts-1.0.0a2/tests/test_sklearn_darts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.881904 autora-theorist-darts-1.0.0a3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.881904 autora-theorist-darts-1.0.0a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/autora-darts.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    21439 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/how_it_works.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   681971 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/img/darts_computation_graph.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/meta_parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/search_space.md
+-rw-r--r--   0 runner    (1001) docker     (123)   796099 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/docs/weber.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.885904 autora-theorist-darts-1.0.0a3/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/mkdocs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.881904 autora-theorist-darts-1.0.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.881904 autora-theorist-darts-1.0.0a3/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.881904 autora-theorist-darts-1.0.0a3/src/autora/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/architect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/fan_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30660 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/model_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19820 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31170 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-27 20:19:13.000000 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-27 20:19:13.000000 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:19:13.000000 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 20:19:13.000000 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 20:19:13.000000 autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:19:13.889904 autora-theorist-darts-1.0.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-04-27 20:18:57.000000 autora-theorist-darts-1.0.0a3/tests/test_sklearn_darts.py
```

### Comparing `autora-theorist-darts-1.0.0a2/.github/workflows/python-publish.yml` & `autora-theorist-darts-1.0.0a3/.github/workflows/python-publish.yml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python#publishing-to-package-registries
 
 # This workflow uses actions that are not certified by GitHub.
 # They are provided by a third-party and are governed by
 # separate terms of service, privacy policy, and support
 # documentation.
 
-name: Upload Python Package
+name: Publish to PyPI
 
 on:
   release:
     types: [published]
 
 permissions:
   contents: read
```

### Comparing `autora-theorist-darts-1.0.0a2/.gitignore` & `autora-theorist-darts-1.0.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/.idea/autora-darts.iml` & `autora-theorist-darts-1.0.0a3/.idea/autora-darts.iml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-darts-1.0.0a3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/.pre-commit-config.yaml` & `autora-theorist-darts-1.0.0a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/PKG-INFO` & `autora-theorist-darts-1.0.0a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: autora-theorist-darts
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Differentiable Architecture Search theorist for AutoRA
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, https://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-darts
 Project-URL: documentation, https://autoresearch.github.io/autora/
-Requires-Python: <4.0,>=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # AutoRA DARTS Theorist
 
 `autora-theorist-darts` is a Python module for fitting data using differentiable architecture 
 search, built on AutoRA.
 
 Website: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
 
 ## User Guide
 
 You will need:
 
-- `python` 3.8.2 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
+- `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 - `graphviz` (optional, required for computation graph visualizations): 
   [https://graphviz.org/download/](https://graphviz.org/download/)
 
 Install DARTS as part of the `autora` package:
 
 ```shell
 pip install -U "autora[theorist-darts]"
```

### Comparing `autora-theorist-darts-1.0.0a2/README.md` & `autora-theorist-darts-1.0.0a3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Website: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
 
 ## User Guide
 
 You will need:
 
-- `python` 3.8.2 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
+- `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 - `graphviz` (optional, required for computation graph visualizations): 
   [https://graphviz.org/download/](https://graphviz.org/download/)
 
 Install DARTS as part of the `autora` package:
 
 ```shell
 pip install -U "autora[theorist-darts]"
```

### Comparing `autora-theorist-darts-1.0.0a2/docs/example.ipynb` & `autora-theorist-darts-1.0.0a3/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/docs/how_it_works.md` & `autora-theorist-darts-1.0.0a3/docs/how_it_works.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/docs/img/darts_computation_graph.jpg` & `autora-theorist-darts-1.0.0a3/docs/img/darts_computation_graph.jpg`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/docs/index.md` & `autora-theorist-darts-1.0.0a3/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/docs/meta_parameters.md` & `autora-theorist-darts-1.0.0a3/docs/meta_parameters.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/docs/quickstart.md` & `autora-theorist-darts-1.0.0a3/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/docs/search_space.md` & `autora-theorist-darts-1.0.0a3/docs/search_space.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/docs/weber.ipynb` & `autora-theorist-darts-1.0.0a3/docs/weber.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/mkdocs/base.yml` & `autora-theorist-darts-1.0.0a3/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/mkdocs/gen_ref_pages.py` & `autora-theorist-darts-1.0.0a3/mkdocs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/mkdocs.yml` & `autora-theorist-darts-1.0.0a3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/pyproject.toml` & `autora-theorist-darts-1.0.0a3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
   { name = "Sebastian Musslick", email = "sebastian_musslick@brown.edu" },
   { name = "John Gerrard Holland", email = "john_holland1@brown.edu" },
 ]
 dynamic = ["version"]
 
 readme = "README.md"
 license = { text = "MIT License" }
-requires-python = ">=3.8.10,<4.0"
 
 dependencies = [
     "autora-core",
     "scikit-learn",
     "torch",
     "matplotlib",
     "graphviz",
```

### Comparing `autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/architect.py` & `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/architect.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/dataset.py` & `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/dataset.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/fan_out.py` & `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/fan_out.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/model_search.py` & `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/model_search.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/operations.py` & `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/operations.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/regressor.py` & `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/regressor.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/utils.py` & `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/src/autora/theorist/darts/visualize.py` & `autora-theorist-darts-1.0.0a3/src/autora/theorist/darts/visualize.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/src/autora_theorist_darts.egg-info/PKG-INFO` & `autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: autora-theorist-darts
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Differentiable Architecture Search theorist for AutoRA
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, https://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-darts
 Project-URL: documentation, https://autoresearch.github.io/autora/
-Requires-Python: <4.0,>=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # AutoRA DARTS Theorist
 
 `autora-theorist-darts` is a Python module for fitting data using differentiable architecture 
 search, built on AutoRA.
 
 Website: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
 
 ## User Guide
 
 You will need:
 
-- `python` 3.8.2 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
+- `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 - `graphviz` (optional, required for computation graph visualizations): 
   [https://graphviz.org/download/](https://graphviz.org/download/)
 
 Install DARTS as part of the `autora` package:
 
 ```shell
 pip install -U "autora[theorist-darts]"
```

### Comparing `autora-theorist-darts-1.0.0a2/src/autora_theorist_darts.egg-info/SOURCES.txt` & `autora-theorist-darts-1.0.0a3/src/autora_theorist_darts.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 README.md
 mkdocs.yml
 pyproject.toml
+.github/workflows/docs-publish.yml
 .github/workflows/python-publish.yml
 .idea/.gitignore
 .idea/autora-darts.iml
 .idea/misc.xml
 .idea/modules.xml
 .idea/vcs.xml
 .idea/inspectionProfiles/Project_Default.xml
```

### Comparing `autora-theorist-darts-1.0.0a2/tests/README.md` & `autora-theorist-darts-1.0.0a3/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a2/tests/test_sklearn_darts.py` & `autora-theorist-darts-1.0.0a3/tests/test_sklearn_darts.py`

 * *Files identical despite different names*


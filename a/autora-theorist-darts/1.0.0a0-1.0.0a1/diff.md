# Comparing `tmp/autora-theorist-darts-1.0.0a0.tar.gz` & `tmp/autora-theorist-darts-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-darts-1.0.0a0.tar", last modified: Thu Apr 27 15:52:59 2023, max compression
+gzip compressed data, was "autora-theorist-darts-1.0.0a1.tar", last modified: Thu Apr 27 15:57:00 2023, max compression
```

## Comparing `autora-theorist-darts-1.0.0a0.tar` & `autora-theorist-darts-1.0.0a1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.115304 autora-theorist-darts-1.0.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.107304 autora-theorist-darts-1.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.107304 autora-theorist-darts-1.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.111304 autora-theorist-darts-1.0.0a0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/.idea/autora-darts.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.111304 autora-theorist-darts-1.0.0a0/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-27 15:52:59.115304 autora-theorist-darts-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.111304 autora-theorist-darts-1.0.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    21439 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/docs/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/docs/how_it_works.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.111304 autora-theorist-darts-1.0.0a0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   681971 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/docs/img/darts_computation_graph.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/docs/introduction.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.111304 autora-theorist-darts-1.0.0a0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/docs/meta_parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/docs/search_space.md
--rw-r--r--   0 runner    (1001) docker     (123)   796099 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/docs/weber.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.115304 autora-theorist-darts-1.0.0a0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/mkdocs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:52:59.115304 autora-theorist-darts-1.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.107304 autora-theorist-darts-1.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.107304 autora-theorist-darts-1.0.0a0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.107304 autora-theorist-darts-1.0.0a0/src/autora/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.115304 autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/architect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/fan_out.py
--rw-r--r--   0 runner    (1001) docker     (123)    30660 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/model_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    19820 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    31170 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.115304 autora-theorist-darts-1.0.0a0/src/autora_theorist_darts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-27 15:52:59.000000 autora-theorist-darts-1.0.0a0/src/autora_theorist_darts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-27 15:52:59.000000 autora-theorist-darts-1.0.0a0/src/autora_theorist_darts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:52:59.000000 autora-theorist-darts-1.0.0a0/src/autora_theorist_darts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 15:52:59.000000 autora-theorist-darts-1.0.0a0/src/autora_theorist_darts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 15:52:59.000000 autora-theorist-darts-1.0.0a0/src/autora_theorist_darts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:52:59.115304 autora-theorist-darts-1.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-04-27 15:52:45.000000 autora-theorist-darts-1.0.0a0/tests/test_sklearn_darts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.027256 autora-theorist-darts-1.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.019256 autora-theorist-darts-1.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.023256 autora-theorist-darts-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.023256 autora-theorist-darts-1.0.0a1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/.idea/autora-darts.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.023256 autora-theorist-darts-1.0.0a1/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-27 15:57:00.027256 autora-theorist-darts-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.023256 autora-theorist-darts-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    21439 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/docs/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/docs/how_it_works.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.023256 autora-theorist-darts-1.0.0a1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   681971 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/docs/img/darts_computation_graph.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/docs/introduction.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.023256 autora-theorist-darts-1.0.0a1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/docs/meta_parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/docs/search_space.md
+-rw-r--r--   0 runner    (1001) docker     (123)   796099 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/docs/weber.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.027256 autora-theorist-darts-1.0.0a1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/mkdocs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:57:00.027256 autora-theorist-darts-1.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.023256 autora-theorist-darts-1.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.019256 autora-theorist-darts-1.0.0a1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.023256 autora-theorist-darts-1.0.0a1/src/autora/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.027256 autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/architect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/fan_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30660 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/model_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19820 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31170 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.027256 autora-theorist-darts-1.0.0a1/src/autora_theorist_darts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-27 15:56:59.000000 autora-theorist-darts-1.0.0a1/src/autora_theorist_darts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-27 15:57:00.000000 autora-theorist-darts-1.0.0a1/src/autora_theorist_darts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:56:59.000000 autora-theorist-darts-1.0.0a1/src/autora_theorist_darts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 15:56:59.000000 autora-theorist-darts-1.0.0a1/src/autora_theorist_darts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 15:56:59.000000 autora-theorist-darts-1.0.0a1/src/autora_theorist_darts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:57:00.027256 autora-theorist-darts-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-04-27 15:56:26.000000 autora-theorist-darts-1.0.0a1/tests/test_sklearn_darts.py
```

### Comparing `autora-theorist-darts-1.0.0a0/.github/workflows/python-publish.yml` & `autora-theorist-darts-1.0.0a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/.gitignore` & `autora-theorist-darts-1.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/.idea/autora-darts.iml` & `autora-theorist-darts-1.0.0a1/.idea/autora-darts.iml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-darts-1.0.0a1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/.pre-commit-config.yaml` & `autora-theorist-darts-1.0.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/PKG-INFO` & `autora-theorist-darts-1.0.0a1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: autora-theorist-darts
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: Differentiable Architecture Search theorist for AutoRA
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, https://www.empiricalresearch.ai
-Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
+Project-URL: repository, https://github.com/AutoResearch/autora-theorist-darts
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4.0,>=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # AutoRA DARTS Theorist
 
 `autora-theorist-darts` is a Python module for fitting data using differentiable architecture 
 search, built on AutoRA.
 
-Website: [empiricalresearch.ai](https://empiricalresearch.ai/autora/theorist/darts/)
+Website: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
 
 ## User Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 - `graphviz` (optional, required for computation graph visualizations): 
@@ -83,15 +83,15 @@
 pip install -e ".[dev]"
 ```
 
 ### Publish the package
 
 Update the metadata under `project` in the pyproject.toml file to include name, description, author-name, author-email and version
 
-- Follow the guide here: https://packaging.python.org/en/latest/tutorials/packaging-projects/
+- Follow the guide here: [https://packaging.python.org/en/latest/tutorials/packaging-projects/](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 
 Build the package using:
 ```shell
 python -m build
 ```
 
 Publish the package to PyPI using `twine`:
```

### Comparing `autora-theorist-darts-1.0.0a0/README.md` & `autora-theorist-darts-1.0.0a1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AutoRA DARTS Theorist
 
 `autora-theorist-darts` is a Python module for fitting data using differentiable architecture 
 search, built on AutoRA.
 
-Website: [empiricalresearch.ai](https://empiricalresearch.ai/autora/theorist/darts/)
+Website: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
 
 ## User Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 - `graphviz` (optional, required for computation graph visualizations): 
@@ -70,15 +70,15 @@
 pip install -e ".[dev]"
 ```
 
 ### Publish the package
 
 Update the metadata under `project` in the pyproject.toml file to include name, description, author-name, author-email and version
 
-- Follow the guide here: https://packaging.python.org/en/latest/tutorials/packaging-projects/
+- Follow the guide here: [https://packaging.python.org/en/latest/tutorials/packaging-projects/](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 
 Build the package using:
 ```shell
 python -m build
 ```
 
 Publish the package to PyPI using `twine`:
```

### Comparing `autora-theorist-darts-1.0.0a0/docs/example.ipynb` & `autora-theorist-darts-1.0.0a1/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/docs/how_it_works.md` & `autora-theorist-darts-1.0.0a1/docs/how_it_works.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/docs/img/darts_computation_graph.jpg` & `autora-theorist-darts-1.0.0a1/docs/img/darts_computation_graph.jpg`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/docs/introduction.md` & `autora-theorist-darts-1.0.0a1/docs/introduction.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/docs/meta_parameters.md` & `autora-theorist-darts-1.0.0a1/docs/meta_parameters.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/docs/quickstart.md` & `autora-theorist-darts-1.0.0a1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/docs/search_space.md` & `autora-theorist-darts-1.0.0a1/docs/search_space.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/docs/weber.ipynb` & `autora-theorist-darts-1.0.0a1/docs/weber.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/mkdocs/base.yml` & `autora-theorist-darts-1.0.0a1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/mkdocs/gen_ref_pages.py` & `autora-theorist-darts-1.0.0a1/mkdocs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/mkdocs.yml` & `autora-theorist-darts-1.0.0a1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/pyproject.toml` & `autora-theorist-darts-1.0.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [project.optional-dependencies]
 dev = [
     "autora-core[dev]"
 ]
 
 [project.urls]
 homepage = "https://www.empiricalresearch.ai"
-repository = "https://github.com/AutoResearch/autora-theorist-template"
+repository = "https://github.com/AutoResearch/autora-theorist-darts"
 documentation = "https://autoresearch.github.io/autora/"
 
 [build-system]
 requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
```

### Comparing `autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/architect.py` & `autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/architect.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/dataset.py` & `autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/dataset.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/fan_out.py` & `autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/fan_out.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/model_search.py` & `autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/model_search.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/operations.py` & `autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/operations.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/regressor.py` & `autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/regressor.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/utils.py` & `autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/src/autora/theorist/darts/visualize.py` & `autora-theorist-darts-1.0.0a1/src/autora/theorist/darts/visualize.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/src/autora_theorist_darts.egg-info/PKG-INFO` & `autora-theorist-darts-1.0.0a1/src/autora_theorist_darts.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: autora-theorist-darts
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: Differentiable Architecture Search theorist for AutoRA
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, https://www.empiricalresearch.ai
-Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
+Project-URL: repository, https://github.com/AutoResearch/autora-theorist-darts
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4.0,>=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # AutoRA DARTS Theorist
 
 `autora-theorist-darts` is a Python module for fitting data using differentiable architecture 
 search, built on AutoRA.
 
-Website: [empiricalresearch.ai](https://empiricalresearch.ai/autora/theorist/darts/)
+Website: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
 
 ## User Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 - `graphviz` (optional, required for computation graph visualizations): 
@@ -83,15 +83,15 @@
 pip install -e ".[dev]"
 ```
 
 ### Publish the package
 
 Update the metadata under `project` in the pyproject.toml file to include name, description, author-name, author-email and version
 
-- Follow the guide here: https://packaging.python.org/en/latest/tutorials/packaging-projects/
+- Follow the guide here: [https://packaging.python.org/en/latest/tutorials/packaging-projects/](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 
 Build the package using:
 ```shell
 python -m build
 ```
 
 Publish the package to PyPI using `twine`:
```

### Comparing `autora-theorist-darts-1.0.0a0/src/autora_theorist_darts.egg-info/SOURCES.txt` & `autora-theorist-darts-1.0.0a1/src/autora_theorist_darts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/tests/README.md` & `autora-theorist-darts-1.0.0a1/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-darts-1.0.0a0/tests/test_sklearn_darts.py` & `autora-theorist-darts-1.0.0a1/tests/test_sklearn_darts.py`

 * *Files identical despite different names*


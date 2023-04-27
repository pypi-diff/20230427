# Comparing `tmp/PyZEAL-0.0.1.tar.gz` & `tmp/PyZEAL-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyZEAL-0.0.1.tar", last modified: Mon Apr  3 16:13:43 2023, max compression
+gzip compressed data, was "PyZEAL-1.0.0rc1.tar", last modified: Thu Apr 27 16:02:44 2023, max compression
```

## Comparing `PyZEAL-0.0.1.tar` & `PyZEAL-1.0.0rc1.tar`

### file list

```diff
@@ -1,53 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:43.587521 PyZEAL-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-03 16:13:43.587521 PyZEAL-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-03 16:13:43.587521 PyZEAL-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:43.579521 PyZEAL-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:43.579521 PyZEAL-0.0.1/src/PyZEAL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-03 16:13:43.000000 PyZEAL-0.0.1/src/PyZEAL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-03 16:13:43.000000 PyZEAL-0.0.1/src/PyZEAL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:13:43.000000 PyZEAL-0.0.1/src/PyZEAL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-03 16:13:43.000000 PyZEAL-0.0.1/src/PyZEAL.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-03 16:13:43.000000 PyZEAL-0.0.1/src/PyZEAL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-03 16:13:43.000000 PyZEAL-0.0.1/src/PyZEAL.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:43.583521 PyZEAL-0.0.1/src/pyzeal/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal/finder_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal/parallel_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal/rootfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:43.583521 PyZEAL-0.0.1/src/pyzeal_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_algorithms/finder_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_algorithms/newton_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_algorithms/simple_holo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_algorithms/simple_holo_newton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:43.583521 PyZEAL-0.0.1/src/pyzeal_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_cli/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:43.583521 PyZEAL-0.0.1/src/pyzeal_logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_logging/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_logging/log_levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_logging/loggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:43.583521 PyZEAL-0.0.1/src/pyzeal_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_types/algorithm_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_types/container_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_types/filter_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_types/parallel_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_types/root_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:43.587521 PyZEAL-0.0.1/src/pyzeal_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_utils/algorithm_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_utils/container_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_utils/filter_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_utils/finder_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_utils/root_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_utils/root_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/src/pyzeal_utils/rounding_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:13:43.587521 PyZEAL-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/test/test_newton_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/test/test_simple_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-03 16:13:28.000000 PyZEAL-0.0.1/test/test_simple_argument_newton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    48722 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.621641 PyZEAL-1.0.0rc1/PyZEAL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48722 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 16:02:44.000000 PyZEAL-1.0.0rc1/PyZEAL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.621641 PyZEAL-1.0.0rc1/pyzeal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.621641 PyZEAL-1.0.0rc1/pyzeal/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.621641 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/argument_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/estimator_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/quad_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/estimators/sum_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/finder_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/newton_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/polynomial_holo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/simple_holo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/algorithms/simple_holo_newton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/cli_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/controller_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/parse_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/cli/parser_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/plugins/custom_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/plugins/custom_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/plugins/installation_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/plugins/plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/plugins/pyzeal_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/log_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/loggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_logging/logger_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/algorithm_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/container_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/estimator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/filter_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/init_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/parallel_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/root_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/settings_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.625641 PyZEAL-1.0.0rc1/pyzeal/rootfinders/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/rootfinders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/rootfinders/finder_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/rootfinders/parallel_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/rootfinders/rootfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/core_settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/default_settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/invalid_setting_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/json_core_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/json_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/json_settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/ram_settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/settings/settings_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_associated_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_newton_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_simple_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/algorithms/test_simple_argument_newton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/newton_grid_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/simple_argument_newton_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/benchmarks/simple_argument_timings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/cli/test_json_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/containers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/containers/test_plain_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/containers/test_rounding_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/estimators/test_quadrature_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/estimators/test_summation_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/resources/estimator_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/resources/finder_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/resources/finder_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/resources/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.629641 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/rootfinders/test_finder_simple_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/tests/test_locator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/pyzeal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/configuration_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/pyzeal/utils/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/containers/plain_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/containers/root_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/containers/rounding_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/pyzeal/utils/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/factories/algorithm_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/factories/container_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/factories/estimator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/factories/settings_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/filter_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/finder_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/initialization_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/install_test_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/install_test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/lambda_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/root_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-27 16:02:35.000000 PyZEAL-1.0.0rc1/pyzeal/utils/service_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:02:44.633641 PyZEAL-1.0.0rc1/setup.cfg
```

### Comparing `PyZEAL-0.0.1/LICENSE` & `PyZEAL-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyZEAL-0.0.1/src/pyzeal/finder_interface.py` & `PyZEAL-1.0.0rc1/pyzeal/rootfinders/finder_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,94 @@
 """
 Module finder_interface of the package pyzeal.
+
 This module contains the base interface for all rootfinder implementations. Its
 methods provide the main root finding API for end users. Internally its
 implementations should build up an appropriate root finding context and then
 employ a `FinderAlgorithm` to calculate the actual roots. Internal book keeping
 is facilitated by the implementations of `RootContainer`.
 
 Authors:\n
 - Philipp Schuette\n
 """
 
 from abc import ABC, abstractmethod
-from typing import Tuple
+from typing import Optional, Tuple
 
 from numpy import int32
 from numpy.typing import NDArray
-from pyzeal_types.filter_types import FilterTypes
-from pyzeal_types.root_types import tVec
-from pyzeal_utils.container_factory import ContainerFactory
-from pyzeal_utils.root_container import RootContainer
+
+from pyzeal.pyzeal_types.filter_types import FilterTypes
+from pyzeal.pyzeal_types.root_types import tVec
+from pyzeal.utils.containers.root_container import RootContainer
+from pyzeal.utils.factories.container_factory import ContainerFactory
+from pyzeal.utils.initialization_handler import PyZEALInitializationHandler
 
 
 class RootFinderInterface(ABC):
     """
     Interface for the main root finding API. After initializing a root finder
     for a given concrete problem methods for calculating roots as well as
     properties for retrieving roots and their orders are available.
     """
 
+    PyZEALInitializationHandler.initPyZEALServices()
+
     @abstractmethod
     def calculateRoots(
         self,
         reRan: Tuple[float, float],
         imRan: Tuple[float, float],
-        precision: Tuple[int, int],
+        precision: Optional[Tuple[int, int]] = None,
     ) -> None:
         """
-        Entry point for starting a root finding calculation in the rectangle
-        `reRan x imRan` up to a number of `precision` significant digits in
-        real and imaginary part.
+        Abstract entry point for starting a root finding calculation in the
+        rectangle `reRan x imRan` up to a number of `precision` significant
+        digits in real and imaginary part.
 
         :param reRan: horizontal extend of the complex region to search in
-        :type reRan: Tuple[int, int]
         :param imRan: vertical extend of the complex region to search in
-        :type imRan: Tuple[int, int]
         :param precision: accuracy of the search in real and imaginary parts
-        :type precision: Tuple[int, int]
         """
 
     @property
     @abstractmethod
     def roots(self) -> tVec:
         """
         Return the roots calculated with this root finder through previous
         calls to `calculateRoots()`.
 
         :return: the set of roots calculated by this finder
-        :rtype: NDArray[np.complex128]
         """
 
     @property
     @abstractmethod
     def orders(self) -> NDArray[int32]:
         """
         Return the orders of the roots calculated with this finder. The output
         is parallel to the return value of the `roots` property.
 
         :return: the orders of the roots calculated by this finder
-        :rtype: NDArray[np.int32]
         """
 
     @property
     @abstractmethod
     def container(self) -> RootContainer:
         """
-        TODO
-        """
+        Return the container instance managing the roots of this finder.
 
-    @container.setter
-    @abstractmethod
-    def container(self, value: RootContainer) -> None:
-        ...
+        :return: the container of this finder
+        """
 
     def setRootFilter(
         self, filterType: FilterTypes, *, threshold: int = 3
     ) -> None:
         """
-        TODO
+        Add a filter of type `filterType` to the set of filters which
+        found roots are checked against.
+
+        :param filterType: the type of root filter to add
+        :param threshold: the threshold for function on root evaluation filters
         """
         ContainerFactory.registerPreDefinedFilter(
             self.container, filterType, threshold=threshold
         )
```

### Comparing `PyZEAL-0.0.1/src/pyzeal/rootfinder.py` & `PyZEAL-1.0.0rc1/pyzeal/rootfinders/rootfinder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """
 Class RootFinder from the package pyzeal.
+
 This module defines an implementation of the main root finding API as defined
 by the `RootFinderInterface` protocol. The class implemented here provides only
-the most basic context for a root finding strategy, i.e. no multiprocessing.
+the most basic context for a root finding strategy, e.g. no support for
+multiprocessing.
 
 Authors:\n
 - Philipp Schuette\n
 """
 
-from signal import SIG_IGN, SIGINT, signal
 from typing import Optional, Tuple
 
 import numpy as np
 from numpy.typing import NDArray
-from pyzeal_logging.log_levels import LogLevel
-from pyzeal_logging.loggable import Loggable
-from pyzeal_types.algorithm_types import AlgorithmTypes
-from pyzeal_types.container_types import ContainerTypes
-from pyzeal_types.root_types import tHoloFunc, tVec
-from pyzeal_utils.algorithm_factory import AlgorithmFactory
-from pyzeal_utils.container_factory import ContainerFactory
-from pyzeal_utils.finder_progress import FinderProgressBar
-from pyzeal_utils.root_context import RootContext
-from pyzeal_utils.root_container import RootContainer
 from rich.progress import TaskID
 
-from pyzeal.finder_interface import RootFinderInterface
+from pyzeal.algorithms.finder_algorithm import FinderAlgorithm
+from pyzeal.pyzeal_logging.log_levels import LogLevel
+from pyzeal.pyzeal_logging.loggable import Loggable
+from pyzeal.pyzeal_types.algorithm_types import AlgorithmTypes
+from pyzeal.pyzeal_types.container_types import ContainerTypes
+from pyzeal.pyzeal_types.estimator_types import EstimatorTypes
+from pyzeal.pyzeal_types.root_types import tHoloFunc, tVec
+from pyzeal.pyzeal_types.settings_types import SettingsServicesTypes
+from pyzeal.rootfinders.finder_interface import RootFinderInterface
+from pyzeal.settings.settings_service import SettingsService
+from pyzeal.utils.containers.root_container import RootContainer
+from pyzeal.utils.finder_progress import FinderProgressBar
+from pyzeal.utils.root_context import RootContext
+from pyzeal.utils.service_locator import ServiceLocator
 
 
 class RootFinder(RootFinderInterface, Loggable):
     """
     Simple (i.e. non-parallel) implementation of the main root finding API.
     """
 
@@ -37,168 +41,201 @@
         "f",
         "df",
         "algorithm",
         "_container",
         "precision",
         "numSamplePoints",
         "verbose",
-        "precision",
-        "_filterFunctionIsZero",
-        "_filterZeroIsInBounds",
     )
 
     def __init__(
         self,
         f: tHoloFunc,
-        df: Optional[tHoloFunc],
+        df: Optional[tHoloFunc] = None,
         *,
-        containerType: ContainerTypes = ContainerTypes.ROUNDING_CONTAINER,
-        algorithmType: AlgorithmTypes = AlgorithmTypes.NEWTON_GRID,
-        precision: Tuple[int, int] = (3, 3),
+        containerType: ContainerTypes = ContainerTypes.DEFAULT,
+        algorithmType: AlgorithmTypes = AlgorithmTypes.DEFAULT,
+        estimatorType: EstimatorTypes = EstimatorTypes.DEFAULT,
+        precision: Optional[Tuple[int, int]] = None,
         numSamplePoints: Optional[int] = None,
-        verbose: bool = True,
+        verbose: Optional[bool] = None,
     ) -> None:
         """
-        Initialize a simple root finder.
+        Initialize a simple, non-parallel root finder.
 
         :param f: the function whose roots should be calculated
-        :type f: Callable[[comlex], complex]
         :param df: the derivative of `f`
-        :type df: Optional[Callable[[complex], complex]]
         :param containerType: the type of container found roots are stored in
-        :type containerType: ContainerTypes
         :param algorithmType: the type of algorithm used for root finding
-        :type algorithmType: AlgorithmTypes
+        :param estimatorType: the type of argument estimator used
         :param precision: the accuracy at which roots are considered exact
-        :type precision: Tuple[int, int]
         :param numSamplePoints: determines grid size for `NewtonGridAlgorithm`
-        :type numSamplePoints: Optional[int]
         :param verbose: flag that toggles the command line progress bar
-        :type verbose: bool
         """
         self.f = f
         self.df = df
-        self.algorithm = AlgorithmFactory.getConcreteAlgorithm(
-            algorithmType, numSamplePoints=numSamplePoints
+        self.algorithm: FinderAlgorithm = ServiceLocator.tryResolve(
+            FinderAlgorithm,
+            algoType=algorithmType,
+            estimatorType=estimatorType,
+            numSamplePoints=numSamplePoints,
         )
-        self._container = ContainerFactory.getConcreteContainer(
-            containerType, precision=precision
+        self._container = ServiceLocator.tryResolve(
+            RootContainer, containerType=containerType, precision=precision
         )
-        self.precision = precision
-        self.verbose = verbose
-        self._filterFunctionIsZero = False
-        self._filterZeroIsInBounds = False
-        self.logger.debug(
-            "initialized a (nonparallel) root finder %s!", str(self)
+        self.precision = (
+            precision or ServiceLocator.tryResolve(SettingsService).precision
+        )
+
+        self.verbose = (
+            verbose
+            if verbose is not None
+            else ServiceLocator.tryResolve(
+                SettingsService, settingsType=SettingsServicesTypes.DEFAULT
+            ).verbose
         )
+        self.logger.debug("initialized the new root finder %s!", str(self))
 
     def __str__(self) -> str:
-        if hasattr(self.f, "__name__") and self.df is None:
-            return f"RootFinder({self.f.__name__}, df=None)"
-        if (
-            hasattr(self.f, "__name__")
-            and self.df is not None
-            and hasattr(self.df, "__name__")
-        ):
-            return f"RootFinder({self.f.__name__}, {self.df.__name__})"
-        return "RootFinder(<unnamed function>)"
+        """
+        Return a simple string representation of a `RootFinder` instance.
+        """
+        if self.df is not None:
+            return (
+                f"RootFinder(f={getattr(self.f, '__name__', '<unnamed>')}, "
+                + f"df={getattr(self.df, '__name__', '<unnamed>')})"
+            )
+        return (
+            f"RootFinder(f={getattr(self.f, '__name__', '<unnamed>')}, "
+            + "df=None)"
+        )
 
     def calculateRoots(
         self,
         reRan: Tuple[float, float],
         imRan: Tuple[float, float],
         precision: Optional[Tuple[int, int]] = None,
     ) -> None:
         """
         Start a (non-parallel) root finding calculation in the rectangle
         `reRan x imRan` up to a number of `precision` significant digits in
         real and imaginary part.
 
         :param reRan: horizontal extend of the complex region to search in
-        :type reRan: Tuple[int, int]
         :param imRan: vertical extend of the complex region to search in
-        :type imRan: Tuple[int, int]
         :param precision: accuracy of the search in real and imaginary parts
-        :type precision: Optional[Tuple[int, int]]
         """
         # if no precision was given, use default precision from constructor
-        precision = self.precision if precision is None else precision
+        precision = precision or self.precision
+        # if a rounding container is used we must calculate with an additional
+        # digit of internal precision to obtain correct results after rounding
+        precision = (precision[0] + 1, precision[1] + 1)
         # desymmetrize the input rectangle
-        (x1, x2), (y1, y2) = sorted(reRan), sorted(imRan)
-        x1 = x1 - 1 * 10 ** (-1 * precision[0])
-        x2 = x2 + 2 * 10 ** (-1 * precision[0])
-        y1 = y1 - 3 * 10 ** (-1 * precision[1])
-        y2 = y2 + 4 * 10 ** (-1 * precision[1])
-        self.logger.debug(
-            "desymmetrized root finding domain to [%f, %f] x [%f, %f]",
-            x1,
-            x2,
-            y1,
-            y2,
-        )
+        (x1, x2), (y1, y2) = self.desymmetrizeDomain(reRan, imRan, precision)
+
         # initialize the progress bar
         progress = FinderProgressBar() if self.verbose else None
         task: Optional[TaskID] = None
-        if progress:
+        if progress is not None:
             task = progress.addTask((x2 - x1) * (y2 - y1))
+            progress.start()
+            self.logger.debug("starting progress bar...")
+
         # construct the root finding context
         context = RootContext(
-            self.f,
-            self.df,
-            self.container,
-            (x1, x2),
-            (y1, y2),
-            precision,
-            progress,
-            task,
+            f=self.f,
+            df=self.df,
+            container=self.container,
+            precision=precision,
+            reRan=(x1, x2),
+            imRan=(y1, y2),
+            progress=progress,
+            task=task,
         )
-        # suppress command line `kill` signals during algorithm runtime
-        signal(SIGINT, SIG_IGN)
+        # shut down root finding in orderly fashion upon command line signals
         try:
             self.logger.info("attempting to calculate roots...")
             self.algorithm.calcRoots(context)
+            if progress is not None and task is not None:
+                progress.update(task, description="[green] search finished!")
         except KeyboardInterrupt:
             self.logger.warning(
                 "root calculation interrupted - some roots may be missing!"
             )
             if progress and task:
                 progress.stop_task(task)
                 progress.update(task, visible=False)
                 progress.refresh()
+        if progress is not None and task is not None:
+            progress.stop()
+        self.logger.info("non-parallel root search finished!")
 
     @property
     def roots(self) -> tVec:
         """
         Return the roots calculated with this root finder through previous
         calls to `calculateRoots()`.
 
         :return: the set of roots calculated by this finder
-        :rtype: NDArray[np.complex128]
         """
         return self.container.getRoots()
 
     @property
     def orders(self) -> NDArray[np.int32]:
         """
         Return the orders of the roots calculated with this finder. The output
         is parallel to the return value of the `roots` property.
 
         :return: the orders of the roots calculated by this finder
-        :rtype: NDArray[np.int32]
         """
         return self.container.getRootOrders()
 
     def setLevel(self, level: LogLevel) -> None:
+        """
+        Set the logging level of this `RootFinder` and all dependent objects
+        like containers and algorithms.
+
+        :param level: the new logging level
+        """
         super().setLevel(level)
         self.container.setLevel(level)
         self.algorithm.setLevel(level)
 
     @property
     def container(self) -> RootContainer:
         """
-        TODO
+        Return the container attached to this rootfinder
         """
         return self._container
 
-    @container.setter
-    def container(self, value: RootContainer) -> None:
-        self._container = value
+    def desymmetrizeDomain(
+        self,
+        reRan: Tuple[float, float],
+        imRan: Tuple[float, float],
+        precision: Tuple[int, int],
+    ) -> Tuple[Tuple[float, float], Tuple[float, float]]:
+        """
+        Desymmetrize the domain to improve numerical stability.
+
+        In practice one notices that target domains as given by `reRan x imRan`
+        often contain roots on/near their boundaries if given e.g. in terms of
+        integers. This method is automatically called by `calculateRoots` so a
+        user does not need to worry about (slightly) perturbing their domains.
+
+        :param reRan: Search range for the real part
+        :param imRan: Search range for the imaginary part
+        :param precision: Accuracy in real and imaginary part
+        :return: New bounds for real and imaginary parts
+        """
+        (x1, x2), (y1, y2) = sorted(reRan), sorted(imRan)
+        x1 = x1 - 1 * 10 ** (-1 * precision[0])
+        x2 = x2 + 2 * 10 ** (-1 * precision[0])
+        y1 = y1 - 3 * 10 ** (-1 * precision[1])
+        y2 = y2 + 4 * 10 ** (-1 * precision[1])
+        self.logger.debug(
+            "desymmetrized root finding domain to [%f, %f] x [%f, %f]",
+            x1,
+            x2,
+            y1,
+            y2,
+        )
+        return (x1, x2), (y1, y2)
```

### Comparing `PyZEAL-0.0.1/src/pyzeal_algorithms/newton_grid.py` & `PyZEAL-1.0.0rc1/pyzeal/algorithms/newton_grid.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 - Luca Wasmuth\n
 """
 
 from itertools import product
 from warnings import filterwarnings
 
 import numpy as np
-import scipy as sp
-from numpy.typing import NDArray
-from pyzeal_utils.root_context import RootContext
+import scipy as sp  # type: ignore
 
-from pyzeal_algorithms.finder_algorithm import FinderAlgorithm
+from pyzeal.algorithms.finder_algorithm import FinderAlgorithm
+from pyzeal.pyzeal_types.root_types import tVec
+from pyzeal.utils.root_context import RootContext
 
 
 class NewtonGridAlgorithm(FinderAlgorithm):
     """
     Class representation of a root finding algorithm for holomorphic functions
     based on starting an ordinary Newton algorithm on a grid of support points
     in the complex plane.
@@ -32,41 +32,29 @@
     __slots__ = ("numSamplePoints",)
 
     def __init__(self, numSamplePoints: int = 50) -> None:
         r"""
         Initialize a root finding algorithm which searches for roots using the
         Newton algorithm with starting points on an evenly spaced grid.
 
-        :param numSamplePoints: number of support points in grid rows/columns
-        :type numSamplePoints: int
+        :param numSamplePoints: Number of support points in grid rows/columns.
         """
         self.numSamplePoints = numSamplePoints
         self.logger.debug("initialized a new NewtonGridAlgorithm!")
 
     def calcRoots(self, context: RootContext) -> None:
         """
         Calculate roots in a given context based on the Newton algorithm on a
         grid of support points in the complex plane.
 
-        :param context: context in which the algorithm operates
-        :type context: RootContext
-        :return: the roots calculated by the algorithm
-        :rtype: NDArray[complex128]
+        :param context: Context in which the algorithm operates.
         """
         self.logger.info(
-            "starting newton grid search for %s on [%f, %f] x [%f, %f]",
-            (
-                context.f.__name__
-                if hasattr(context.f, "__name__")
-                else "<unknown>"
-            ),
-            context.reRan[0],
-            context.reRan[1],
-            context.imRan[0],
-            context.imRan[1],
+            "starting newton grid search for %s",
+            context.functionDataToString(),
         )
         rePoints = np.linspace(
             context.reRan[0],
             context.reRan[1],
             self.numSamplePoints,
             dtype=np.complex128,
         )
@@ -75,17 +63,15 @@
             context.imRan[1],
             self.numSamplePoints,
             dtype=np.complex128,
         )
         points = [x + y * 1j for (x, y) in product(rePoints, imPoints)]
         filterwarnings("ignore", ".*some failed to converge")
         try:
-            roots: NDArray[np.complex128] = sp.optimize.newton(
-                context.f, points, context.df
-            )
+            roots: tVec = sp.optimize.newton(context.f, points, context.df)
         except RuntimeError:
             return
         for root in roots:
             # the newton algorithm does not determine root orders - placeholder
             # value can be anything non-positive
             context.container.addRoot((root, 0), context.toFilterContext())
         if context.progress and context.task:
```

### Comparing `PyZEAL-0.0.1/src/pyzeal_types/filter_types.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/filter_types.py`

 * *Files identical despite different names*

### Comparing `PyZEAL-0.0.1/src/pyzeal_types/parallel_types.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/parallel_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 """
 This module provides type aliases used in conjunction with multiprocessing.
 
 Authors:\n
 - Philipp Schuette\n
 """
 
-from abc import ABC, abstractmethod
 from multiprocessing.managers import BaseManager
-from typing import Callable, Tuple
+from typing import Callable, Protocol, Tuple
 
-from rich.progress import Progress
+from pyzeal.utils.finder_progress import FinderProgressBar
 
 
 # typed queues to be used for message passing with multiprocessing.Queue
-class tQueue(ABC):
+class tQueue(Protocol):
     r"""
     Queue that stores tuples of the form (root: complex, order: int).
     """
 
-    @abstractmethod
     def get(self) -> Tuple[complex, int]:
         "Get first element of the queue."
+        ...
 
-    @abstractmethod
     def put(self, item: Tuple[complex, int]) -> None:
         "Put element into the queue."
+        ...
 
-    @abstractmethod
     def empty(self) -> bool:
         "Check if queue is empty."
+        ...
 
 
 # multiprocessing managers used to share access to progress bars
-class MyManager(BaseManager):
+class FinderProgressManager(BaseManager):
     r"""
     Multiprocessing.BaseManager containing a rich.progress.Progress instance.
     """
-    progress: Callable[..., Progress]
+    finderProgress: Callable[..., FinderProgressBar]
```

### Comparing `PyZEAL-0.0.1/src/pyzeal_types/root_types.py` & `PyZEAL-1.0.0rc1/pyzeal/pyzeal_types/root_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 """
-This module provides type aliases used throughout the PyZEAL project.
+Module `root_types` from the package `pyzeal.pyzeal_types`.
+
+This module provides common type aliases used throughout the PyZEAL project.
 
 Authors:\n
 - Philipp Schuette\n
 """
 
-from typing import Callable, List, Tuple, Union
+from typing import Callable, Tuple
 
 import numpy as np
 from numpy.typing import NDArray
+from typing_extensions import TypeAlias
 
-
-# general purpose types used throughout
-tScal = Union[float, complex]
-tVec = NDArray[np.complex128]
+# general purpose type for numpy arrays with complex entries
+tVec: TypeAlias = NDArray[np.complex128]
 
 # type of functions our root finding algorithms can handle
-tHoloFunc = Callable[[tVec], tVec]
+tHoloFunc: TypeAlias = Callable[[tVec], tVec]
 
 # type used to identify roots of holomorphic functions (point in the plane with
 # its multiplicity)
-tRoot = Tuple[complex, int]
-
-# types used for rootfinder results and internally
-tRecGrid = Tuple[
-    NDArray[np.complex128],
-    NDArray[np.complex128],
-    NDArray[np.complex128],
-    NDArray[np.complex128],
-]
+tRoot: TypeAlias = Tuple[complex, int]
 
-tResVec = Union[List[Tuple[tScal, int]], tVec]
-tErrVec = Union[List[tScal], tVec]
+# type of rectangular grid used internally in simple argument rootfinders
+tRecGrid: TypeAlias = Tuple[tVec, tVec, tVec, tVec]
```

### Comparing `PyZEAL-0.0.1/src/pyzeal_utils/algorithm_factory.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/factories/algorithm_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,69 +5,92 @@
 
 Authors:\n
 - Philipp Schuette\n
 """
 
 from typing import Optional
 
-from pyzeal_types.algorithm_types import AlgorithmTypes
-from pyzeal_algorithms.finder_algorithm import FinderAlgorithm
-from pyzeal_algorithms.newton_grid import NewtonGridAlgorithm
-from pyzeal_algorithms.simple_holo import SimpleArgumentAlgorithm
-from pyzeal_algorithms.simple_holo_newton import SimpleArgumentNewtonAlgorithm
-from pyzeal_logging.config import initLogger
-from pyzeal_logging.log_levels import LogLevel
+from pyzeal.algorithms.finder_algorithm import FinderAlgorithm
+from pyzeal.algorithms.newton_grid import NewtonGridAlgorithm
+from pyzeal.algorithms.polynomial_holo import AssociatedPolynomialAlgorithm
+from pyzeal.algorithms.simple_holo import SimpleArgumentAlgorithm
+from pyzeal.algorithms.simple_holo_newton import SimpleArgumentNewtonAlgorithm
+from pyzeal.pyzeal_logging.log_levels import LogLevel
+from pyzeal.pyzeal_logging.log_manager import LogManager
+from pyzeal.pyzeal_logging.logger_facade import PyZEALLogger
+from pyzeal.pyzeal_types.algorithm_types import AlgorithmTypes
+from pyzeal.pyzeal_types.estimator_types import EstimatorTypes
+from pyzeal.settings.settings_service import SettingsService
+from pyzeal.utils.service_locator import ServiceLocator
 
 
 class AlgorithmFactory:
     "Static factory class used to create instances of root finding algorithms."
 
-    # initialize the module level logger
-    logger = initLogger(__name__.rsplit(".", maxsplit=1)[-1])
+    # the module level logger
+    _logger: Optional[PyZEALLogger] = None
 
     @staticmethod
     def getConcreteAlgorithm(
-        algoType: AlgorithmTypes, *, numSamplePoints: Optional[int] = None
+        algoType: AlgorithmTypes = AlgorithmTypes.DEFAULT,
+        *,
+        estimatorType: EstimatorTypes = EstimatorTypes.DEFAULT,
+        numSamplePoints: Optional[int] = None,
     ) -> FinderAlgorithm:
         """
         Construct and return an algorithm instance based on the given type of
         algorithm `algoType`. Additional, algorithm specific configuration
         arguments are optional.
 
         :param algoType: type of algorithm to construct
-        :type algoType: AlgorithmType
+        :param estimatorType: type of argument estimator to use
         :param numSamplePoints: sample point configuration for NewtonGridAlgo
-        :type numSamplePoints: int
+        :return: a concrete `FinderAlgorithm` instance
         """
+        if AlgorithmFactory._logger is None:
+            AlgorithmFactory._logger = LogManager.initLogger(
+                __name__.rsplit(".", maxsplit=1)[-1],
+                ServiceLocator.tryResolve(SettingsService).logLevel,
+            )
         if algoType == AlgorithmTypes.NEWTON_GRID:
-            AlgorithmFactory.logger.debug(
+            AlgorithmFactory._logger.debug(
                 "requested usage of a NewtonGridAlgorithm..."
             )
             if numSamplePoints:
                 return NewtonGridAlgorithm(numSamplePoints=numSamplePoints)
             return NewtonGridAlgorithm()
         if algoType == AlgorithmTypes.SIMPLE_ARGUMENT:
-            AlgorithmFactory.logger.debug(
+            AlgorithmFactory._logger.debug(
                 "requested usage of a SimpleArgumentAlgorithm..."
             )
-            return SimpleArgumentAlgorithm()
+            return SimpleArgumentAlgorithm(estimatorType=estimatorType)
         if algoType == AlgorithmTypes.SIMPLE_ARGUMENT_NEWTON:
-            AlgorithmFactory.logger.debug(
+            AlgorithmFactory._logger.debug(
                 "requested usage of a SimpleArgumentNewtonAlgorithm..."
             )
-            return SimpleArgumentNewtonAlgorithm()
+            return SimpleArgumentNewtonAlgorithm(estimatorType=estimatorType)
+        if algoType == AlgorithmTypes.ASSOCIATED_POLYNOMIAL:
+            AlgorithmFactory._logger.debug(
+                "requested usage of an AssociatedPolynomialAlgorithm..."
+            )
+            return AssociatedPolynomialAlgorithm(estimatorType=estimatorType)
 
-        # TODO: implement configuration mechanism for default algorithms
-        AlgorithmFactory.logger.debug(
+        # return the current default algorithm
+        AlgorithmFactory._logger.debug(
             "requested usage of the default algorithm..."
         )
-        return NewtonGridAlgorithm()
+        settings = ServiceLocator.tryResolve(SettingsService)
+        return AlgorithmFactory.getConcreteAlgorithm(
+            settings.defaultAlgorithm,
+            numSamplePoints=numSamplePoints,
+            estimatorType=estimatorType,
+        )
 
     @staticmethod
     def setLevel(level: LogLevel) -> None:
         """
         Set the log level.
 
         :param level: the new log level
-        :type level: pyzeal_logging.log_levels.LogLevel
         """
-        AlgorithmFactory.logger.setLevel(level=level.value)
+        if AlgorithmFactory._logger is not None:
+            AlgorithmFactory._logger.setLevel(level=level.value)
```

### Comparing `PyZEAL-0.0.1/src/pyzeal_utils/filter_context.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/filter_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Authors:\n
 - Philipp Schuette\n
 """
 
 from dataclasses import dataclass
 from typing import Callable, Tuple
 
-from pyzeal_types.root_types import tHoloFunc, tRoot
+from pyzeal.pyzeal_types.root_types import tHoloFunc, tRoot
 
 
 @dataclass(frozen=True)
 class FilterContext:
     """
     Container for the data context of a root filter predicate. The container is
     read-only.
```

### Comparing `PyZEAL-0.0.1/src/pyzeal_utils/finder_progress.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/finder_progress.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,13 +34,12 @@
     def addTask(self, total: float) -> TaskID:
         """
         Override the `add_task()` method of generic progress bars by allowing
         only the total amount of work to be adjusted and prescribing a default
         task description.
 
         :param total: the total amount of work contained in the added task
-        :type total: float
         """
         return super().add_task(
             description=(f"[magenta]{getpid()}: " + "[g]getting roots..."),
             total=total,
         )
```

### Comparing `PyZEAL-0.0.1/src/pyzeal_utils/root_container.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/containers/root_container.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,66 +7,61 @@
 Additional checks could also be implemented in subclasses, e.g. checking if a
 root is contained in a certain region.
 
 Authors:\n
 - Philipp Schuette\n
 """
 
-from typing import Protocol
+from typing import Protocol, runtime_checkable
 
 import numpy as np
 from numpy.typing import NDArray
-from pyzeal_logging.loggable import Loggable
-from pyzeal_types.root_types import tRoot, tVec
 
-from pyzeal_utils.filter_context import FilterContext, tRootFilter
+from pyzeal.pyzeal_logging.loggable import Loggable
+from pyzeal.pyzeal_types.root_types import tRoot, tVec
+from pyzeal.utils.filter_context import FilterContext, tRootFilter
 
 
+@runtime_checkable
 class RootContainer(Loggable, Protocol):
     "Structural interface for container classes meant to hold root data."
 
     def addRoot(self, root: tRoot, context: FilterContext) -> None:
         """
         Add a root to the container.
 
         :param root: the root to be added to the container
-        :type root: tRoot
         :param context: the number of valid decimal places of `root`
-        :type context: FilterContext
         """
         ...
 
     def getRoots(self) -> tVec:
         """
         Returns all roots currently held in this container as a vector.
 
         :return: a vector of complex roots
-        :rtype: NDArray[complex128]
         """
         ...
 
     def getRootOrders(self) -> NDArray[np.int32]:
         """
         Returns the orders of all roots currently held in this container as a
         vector which is parallel to the vector returned by `getRoots`.
 
         :return: a vector of integer root orders (multiplicities)
-        :rtype: NDArray[int32]
         """
         ...
 
     def removeRoot(self, root: tRoot) -> bool:
         """
         Remove a root from the container and indicate whether or not a removal
         actually happened via the return value.
 
         :param root: the root to be removed from the container
-        :type root: tRoot
         :return: a boolean flag indicating if a removal happened
-        :rtype: bool
         """
         ...
 
     def clear(self) -> None:
         "Clear all data from the container."
         ...
 
@@ -74,21 +69,18 @@
         """
         Add a new filter predicate to this container instance. The filtering
         applies to all roots added after the filter is registered. To guarantee
         a consistent set of roots any implementation should clear its internal
         root buffer before/after registering a filter.
 
         :param filterPredicate: the predicate used to filter roots
-        :type filterPredicate: Callable[[tRoot, RootContext], bool]
         :param key: a (unique) key under which the filter is registered
-        :type key: str
         """
         ...
 
     def unregisterFilter(self, key: str) -> None:
         """
         Remove a previously registered filter by key.
 
         :param key: key value for the filter to remove
-        :type key: str
         """
         ...
```

### Comparing `PyZEAL-0.0.1/src/pyzeal_utils/root_context.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/root_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,36 +6,52 @@
 Authors:\n
 - Philipp Schuette\n
 """
 
 from dataclasses import dataclass
 from typing import Optional, Tuple
 
-from pyzeal_types.root_types import tHoloFunc
 from rich.progress import TaskID
 
-from pyzeal_utils.filter_context import FilterContext
-from pyzeal_utils.finder_progress import FinderProgressBar
-from pyzeal_utils.root_container import RootContainer
+from pyzeal.pyzeal_types.root_types import tHoloFunc
+from pyzeal.utils.containers.root_container import RootContainer
+from pyzeal.utils.filter_context import FilterContext
+from pyzeal.utils.finder_progress import FinderProgressBar
 
 
 @dataclass(frozen=True)
 class RootContext:
     """
     Container for the data context of a root finding algorithm. The container
     is read-only.
     """
 
     f: tHoloFunc
     df: Optional[tHoloFunc]
     container: RootContainer
+    precision: Tuple[int, int]
     reRan: Tuple[float, float] = (-1.0, 1.0)
     imRan: Tuple[float, float] = (-1.0, 1.0)
-    precision: Tuple[int, int] = 3, 3
     progress: Optional[FinderProgressBar] = None
     task: Optional[TaskID] = None
 
     def toFilterContext(self) -> FilterContext:
         """
-        TODO
+        Get a `FilterContext` object with the same parameters as this
+        `RootContext`
+
+        :return: `FilterContext` object with the same parameters as this
+            `RootContext`
         """
         return FilterContext(self.f, self.reRan, self.imRan, self.precision)
+
+    def functionDataToString(self) -> str:
+        """
+        Return a string describing the data stored by this object
+
+        :return: Object data
+        """
+        return (
+            f"{getattr(self.f, '__name__', '<unnamed>')} on rectangle "
+            + f"[{self.reRan[0]}, {self.reRan[1]}] "
+            + f"x [{self.imRan[0]}, {self.imRan[1]}]"
+        )
```

### Comparing `PyZEAL-0.0.1/src/pyzeal_utils/rounding_container.py` & `PyZEAL-1.0.0rc1/pyzeal/utils/containers/rounding_container.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,58 +4,61 @@
 The concrete container class implemented here automatically rounds added roots
 to a fixed number of decimal places.
 
 Authors:\n
 - Philipp Schuette\n
 """
 
-from typing import Dict, Set, Tuple
+from logging import INFO
+from typing import Dict, Optional, Set, Tuple
 
 import numpy as np
 from numpy.typing import NDArray
-from pyzeal_types.root_types import tRoot, tVec
 
-from pyzeal_utils.filter_context import FilterContext
-from pyzeal_utils.root_container import RootContainer, tRootFilter
+from pyzeal.pyzeal_types.root_types import tRoot, tVec
+from pyzeal.settings.settings_service import SettingsService
+from pyzeal.utils.containers.root_container import RootContainer
+from pyzeal.utils.filter_context import FilterContext, tRootFilter
+from pyzeal.utils.service_locator import ServiceLocator
 
 
 class RoundingContainer(RootContainer):
     """
     This simple container implementation rounds every added root to a given
     number of decimal places and simple ignores any attempts to add additional
     roots which coincide with a previously added root after rounding. The
     multiplicity is not taken into account when comparing old and new roots.
     Changing the desired accuracy automatically removes all calculated roots
     to preserve consistency.
     """
 
     __slots__ = ("precision", "rootSet", "filters")
 
-    def __init__(self, precision: Tuple[int, int]) -> None:
+    def __init__(self, precision: Optional[Tuple[int, int]]) -> None:
         """
-        Initialize a rounding RootContainer with a given accuracy.
+        Initialize a rounding RootContainer. If no precision is given,
+        default precision is used.
 
         :param precision: expected accuracy of roots to be added
-        :type precision: Tuple[int, int]
         """
-        self.precision = precision
+        self.precision = (
+            precision or ServiceLocator.tryResolve(SettingsService).precision
+        )
         self.rootSet: Set[tRoot] = set()
         self.filters: Dict[str, tRootFilter] = {}
-        self.logger.info("initialized a rounding root container")
+        self.logger.info("initialized a new rounding root container")
 
     def addRoot(self, root: tRoot, context: FilterContext) -> None:
         """
         Add a new root with given accuracy to the container. If the accuracy
         differs from the accuracy of roots already added then all previous
         roots are removed.
 
         :param root: the root to be added to the container
-        :type root: tRoot
         :param context: the context of the new root, required for filtering
-        :type context: FilterContext
         """
         for filterPredicate in self.filters.values():
             if not filterPredicate(root, context):
                 self.logger.debug(
                     "root %f+%fi was rejected by container filter!",
                     root[0].real,
                     root[0].imag,
@@ -64,28 +67,35 @@
         if context.precision != self.precision:
             self.clear()
             self.logger.debug(
                 "new accuracy detected - rounding container cleared!"
             )
             self.precision = context.precision
         self.logger.debug(
-            "attempting to add new root %f+%fi to rounding container!",
+            "attempting to add new root %f + %fi to rounding container!",
             root[0].real,
             root[0].imag,
         )
-        self.rootSet.add(RoundingContainer.roundRoot(root, self.precision))
+        roundedRoot = RoundingContainer.roundRoot(root, self.precision)
+        if self.logger.isEnabledFor(INFO) and roundedRoot in self.rootSet:
+            self.logger.info("duplicate root discarded by rounding container!")
+            return
+        self.logger.info(
+            "new root %f + %fi added to rounding container",
+            roundedRoot[0].real,
+            roundedRoot[0].imag,
+        )
+        self.rootSet.add(roundedRoot)
 
     def removeRoot(self, root: tRoot) -> bool:
         """
         Remove a given root from the container. Return value indicates success.
 
         :param root: the root to be removed from the container
-        :type root: tRoot
         :return: a boolean flag indicating if a removal happened
-        :rtype: bool
         """
         try:
             self.rootSet.remove(
                 RoundingContainer.roundRoot(root, self.precision)
             )
             self.logger.debug(
                 "removed root %f+%fi from rounding container!",
@@ -102,28 +112,26 @@
             return False
 
     def getRoots(self) -> tVec:
         """
         Returns all roots currently held in this container as a vector.
 
         :return: a vector of complex roots
-        :rtype: NDArray[complex128]
         """
         result = np.empty((len(self.rootSet)), dtype=np.complex128)
         for i, root in enumerate(self.rootSet):
             result[i] = root[0]
         return result
 
     def getRootOrders(self) -> NDArray[np.int32]:
         """
         Returns the orders of all roots currently held in this container as a
         vector which is parallel to the vector returned by `getRoots`.
 
         :return: a vector of integer root orders (multiplicities)
-        :rtype: NDArray[int32]
         """
         result = np.empty((len(self.rootSet)), dtype=np.int32)
         for i, root in enumerate(self.rootSet):
             result[i] = root[1]
         return result
 
     def clear(self) -> None:
@@ -132,31 +140,33 @@
 
     @staticmethod
     def roundRoot(root: tRoot, precision: Tuple[int, int]) -> tRoot:
         """
         Round a given root to a given number of decimal places.
 
         :param root: a root to be rounded
-        :type root: tRoot
         :param precision: the number of decimal places to round to
-        :type precision: int
         :return: the rounded root (multiplicity stays constant)
-        :rtype: tRoot
         """
         x, y = root[0].real, root[0].imag
         return complex(round(x, precision[0]), round(y, precision[1])), root[1]
 
     def registerFilter(self, filterPredicate: tRootFilter, key: str) -> None:
         """
-        TODO
+        Register a new filter to check possible roots against
+
+        :param filterPredicate: New filter to register
+        :param key: A key to identify this filter
         """
         self.filters[key] = filterPredicate
 
     def unregisterFilter(self, key: str) -> None:
         """
-        TODO
+        Remove the filter identified by `key`.
+
+        :param key: Filter key
         """
         try:
             self.filters.pop(key)
             self.logger.debug("removed filter %s", key)
         except KeyError:
             self.logger.info("tried to remove non-existent filter %s!", key)
```


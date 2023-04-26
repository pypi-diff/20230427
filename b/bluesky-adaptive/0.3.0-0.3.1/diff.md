# Comparing `tmp/bluesky-adaptive-0.3.0.tar.gz` & `tmp/bluesky-adaptive-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluesky-adaptive-0.3.0.tar", last modified: Wed Apr 26 18:31:54 2023, max compression
+gzip compressed data, was "bluesky-adaptive-0.3.1.tar", last modified: Wed Apr 26 22:57:10 2023, max compression
```

## Comparing `bluesky-adaptive-0.3.0.tar` & `bluesky-adaptive-0.3.1.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/bluesky_adaptive/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/bluesky_adaptive/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.056794 bluesky-adaptive-0.3.0/bluesky_adaptive/adjudicators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/adjudicators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/adjudicators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/adjudicators/msg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.056794 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43242 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/agents/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/on_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/per_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/per_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/scipy_reccomendations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.056794 bluesky-adaptive-0.3.0/bluesky_adaptive/server/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/comms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/ioc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/logging_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/server_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/server/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_adjudicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_botorch_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_per_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_per_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_scipy_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_sklearn_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/bluesky_adaptive/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.056794 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 18:31:54.000000 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 18:31:54.000000 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:31:54.000000 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 18:31:54.000000 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 18:31:54.000000 bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/distributed.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/min_versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-26 18:31:54.060794 bluesky-adaptive-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68576 2023-04-26 18:31:37.000000 bluesky-adaptive-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:57:10.834418 bluesky-adaptive-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-26 22:57:10.834418 bluesky-adaptive-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:57:10.834418 bluesky-adaptive-0.3.1/bluesky_adaptive/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 22:57:10.834418 bluesky-adaptive-0.3.1/bluesky_adaptive/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:57:10.830417 bluesky-adaptive-0.3.1/bluesky_adaptive/adjudicators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/adjudicators/README-ADJUDICATORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/adjudicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/adjudicators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/adjudicators/msg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:57:10.830417 bluesky-adaptive-0.3.1/bluesky_adaptive/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43242 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/agents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/agents/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/agents/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/agents/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/on_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/per_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/per_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/scipy_reccomendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:57:10.830417 bluesky-adaptive-0.3.1/bluesky_adaptive/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/server/comms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/server/ioc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/server/logging_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/server/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/server/server_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/server/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:57:10.834418 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_adjudicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_botorch_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_per_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_per_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_scipy_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_sklearn_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/bluesky_adaptive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:57:10.830417 bluesky-adaptive-0.3.1/bluesky_adaptive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-26 22:57:10.000000 bluesky-adaptive-0.3.1/bluesky_adaptive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-26 22:57:10.000000 bluesky-adaptive-0.3.1/bluesky_adaptive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:57:10.000000 bluesky-adaptive-0.3.1/bluesky_adaptive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 22:57:10.000000 bluesky-adaptive-0.3.1/bluesky_adaptive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 22:57:10.000000 bluesky-adaptive-0.3.1/bluesky_adaptive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:57:10.834418 bluesky-adaptive-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:57:10.834418 bluesky-adaptive-0.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/docs/source/distributed.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/docs/source/min_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/requirements-agents.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-26 22:57:10.834418 bluesky-adaptive-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68576 2023-04-26 22:56:52.000000 bluesky-adaptive-0.3.1/versioneer.py
```

### Comparing `bluesky-adaptive-0.3.0/CONTRIBUTING.rst` & `bluesky-adaptive-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/LICENSE` & `bluesky-adaptive-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/adjudicators/base.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/adjudicators/base.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/adjudicators/msg.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/adjudicators/msg.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/agents/base.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/agents/base.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/agents/botorch.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/agents/botorch.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/agents/simple.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/agents/simple.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/agents/sklearn.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/agents/sklearn.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/on_stop.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/on_stop.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/per_event.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/per_event.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/per_start.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/per_start.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/recommendations.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/recommendations.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/scipy_reccomendations.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/scipy_reccomendations.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/server/comms.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/server/comms.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/server/ioc_server.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/server/ioc_server.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/server/logging_setup.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/server/logging_setup.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/server/server.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/server/server.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/server/server_api.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/server/server_api.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/server/server_resources.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/server/server_resources.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/server/utils.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/server/utils.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/server/worker.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/server/worker.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/conftest.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_adjudicators.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_adjudicators.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_agents.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_botorch_agents.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_botorch_agents.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_kafka.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_per_event.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_per_event.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_per_start.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_per_start.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_scipy_rec.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_scipy_rec.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/tests/test_sklearn_agents.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/tests/test_sklearn_agents.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive/utils.py` & `bluesky-adaptive-0.3.1/bluesky_adaptive/utils.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/bluesky_adaptive.egg-info/SOURCES.txt` & `bluesky-adaptive-0.3.1/bluesky_adaptive.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
+requirements-agents.txt
+requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 bluesky_adaptive/__init__.py
 bluesky_adaptive/_version.py
 bluesky_adaptive/on_stop.py
@@ -17,14 +19,15 @@
 bluesky_adaptive/scipy_reccomendations.py
 bluesky_adaptive/utils.py
 bluesky_adaptive.egg-info/PKG-INFO
 bluesky_adaptive.egg-info/SOURCES.txt
 bluesky_adaptive.egg-info/dependency_links.txt
 bluesky_adaptive.egg-info/requires.txt
 bluesky_adaptive.egg-info/top_level.txt
+bluesky_adaptive/adjudicators/README-ADJUDICATORS.md
 bluesky_adaptive/adjudicators/__init__.py
 bluesky_adaptive/adjudicators/base.py
 bluesky_adaptive/adjudicators/msg.py
 bluesky_adaptive/agents/__init__.py
 bluesky_adaptive/agents/base.py
 bluesky_adaptive/agents/botorch.py
 bluesky_adaptive/agents/simple.py
```

### Comparing `bluesky-adaptive-0.3.0/docs/Makefile` & `bluesky-adaptive-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/docs/make.bat` & `bluesky-adaptive-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/docs/source/conf.py` & `bluesky-adaptive-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/docs/source/distributed.rst` & `bluesky-adaptive-0.3.1/docs/source/distributed.rst`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/docs/source/examples.rst` & `bluesky-adaptive-0.3.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/docs/source/index.rst` & `bluesky-adaptive-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/docs/source/min_versions.rst` & `bluesky-adaptive-0.3.1/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/docs/source/release-history.rst` & `bluesky-adaptive-0.3.1/docs/source/release-history.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ===============
 Release History
 ===============
 
+v0.3.1 (2023-04-26)
+-------------------
++ MANIFEST updates for packaging and documentation
+
 v0.3.0 (2023-04-26)
 -------------------
 + Add distributed agents: base classes, simple, sklearn, and gpytorch agents
 + First implementation of a server and FAST API
 + Add adjudicators (meta-agents)
 + Updates to development workflow in-line with scientific cookiecutter
```

### Comparing `bluesky-adaptive-0.3.0/setup.py` & `bluesky-adaptive-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `bluesky-adaptive-0.3.0/versioneer.py` & `bluesky-adaptive-0.3.1/versioneer.py`

 * *Files identical despite different names*


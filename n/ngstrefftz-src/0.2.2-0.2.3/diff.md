# Comparing `tmp/ngstrefftz-src-0.2.2.tar.gz` & `tmp/ngstrefftz-src-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngstrefftz-src-0.2.2.tar", last modified: Wed Feb 15 11:38:26 2023, max compression
+gzip compressed data, was "ngstrefftz-src-0.2.3.tar", last modified: Thu Apr 27 13:47:46 2023, max compression
```

## Comparing `ngstrefftz-src-0.2.2.tar` & `ngstrefftz-src-0.2.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:38:26.118500 ngstrefftz-src-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-15 11:38:26.118500 ngstrefftz-src-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:38:26.110499 ngstrefftz-src-0.2.2/external_dependencies/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:38:26.114500 ngstrefftz-src-0.2.2/external_dependencies/ngstents/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:38:26.114500 ngstrefftz-src-0.2.2/external_dependencies/ngstents/py/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/py/_drawtents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/py/ctau_experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/py/tentinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:38:26.118500 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/advection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/burgers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   133375 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/concurrentqueue.h
--rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/conservationlaw.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/euler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/maxwell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/paralleldepend.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/python_conslaw.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/python_tents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/symbolic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31227 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    47723 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/tents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/tents.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/tentsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/tentsolver_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/vis3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/vis3d.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-02-15 11:37:43.000000 ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/wave.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:38:26.110499 ngstrefftz-src-0.2.2/ngstrefftz_src.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-15 11:38:26.000000 ngstrefftz-src-0.2.2/ngstrefftz_src.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-02-15 11:38:26.000000 ngstrefftz-src-0.2.2/ngstrefftz_src.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 11:38:26.000000 ngstrefftz-src-0.2.2/ngstrefftz_src.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-15 11:38:26.000000 ngstrefftz-src-0.2.2/ngstrefftz_src.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 11:38:26.000000 ngstrefftz-src-0.2.2/ngstrefftz_src.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 11:38:26.118500 ngstrefftz-src-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:38:26.114500 ngstrefftz-src-0.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/airy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/diffopmapped.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/embtrefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/embtrefftz.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/intrule4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/mesh1dtents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/mesh1dtents.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/monomialfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/monomialfespace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/planewavefe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/planewavefe.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/python_trefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    48909 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/scalarmappedfe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/scalarmappedfe.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/specialcoefficientfunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/specialcoefficientfunction.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    38072 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/trefftzfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/trefftzfespace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    43502 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/twavetents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/src/twavetents.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:38:26.118500 ngstrefftz-src-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/test/embt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/test/tents.py
--rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/test/trefftz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-02-15 11:37:42.000000 ngstrefftz-src-0.2.2/test/twave.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.364179 ngstrefftz-src-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 13:47:46.364179 ngstrefftz-src-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.356179 ngstrefftz-src-0.2.3/external_dependencies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.360179 ngstrefftz-src-0.2.3/external_dependencies/ngstents/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.360179 ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/_drawtents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/ctau_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/tentinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.360179 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/advection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/burgers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   133375 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/concurrentqueue.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/conservationlaw.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/maxwell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/paralleldepend.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/python_conslaw.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/python_tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/symbolic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31227 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    47723 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tents.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tentsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tentsolver_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/vis3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/vis3d.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/wave.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.356179 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 13:47:46.000000 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-27 13:47:46.000000 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:47:46.000000 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 13:47:46.000000 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 13:47:46.000000 ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:47:46.364179 ngstrefftz-src-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.360179 ngstrefftz-src-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/airy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/diffopmapped.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25648 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/embtrefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/embtrefftz.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/intrule4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/mesh1dtents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/mesh1dtents.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/monomialfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/monomialfespace.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/planewavefe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/planewavefe.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/python_trefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    48909 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/scalarmappedfe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/scalarmappedfe.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/specialcoefficientfunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/specialcoefficientfunction.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    38072 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/trefftzfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/trefftzfespace.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    43502 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/twavetents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/src/twavetents.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:47:46.360179 ngstrefftz-src-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/test/embt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/test/tents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/test/trefftz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-27 13:47:02.000000 ngstrefftz-src-0.2.3/test/twave.py
```

### Comparing `ngstrefftz-src-0.2.2/LICENSE` & `ngstrefftz-src-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/PKG-INFO` & `ngstrefftz-src-0.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz-src
-Version: 0.2.2
+Version: 0.2.3
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `ngstrefftz-src-0.2.2/README.md` & `ngstrefftz-src-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,20 +35,23 @@
 ```bash
 git clone --recursive https://github.com/PaulSt/NGSTrefftz
 mkdir ./NGSTrefftz/make && cd ./NGSTrefftz/make
 cmake ../src && make install
 ```
 
 ### Dependencies
-To build the package the following software needs to be installed
- * [cmake](https://cmake.org/) >= 3.1
- * [gcc](https://gcc.gnu.org/) >= 9 or [clang](https://clang.llvm.org/) >= 10
- * [ngsolve](https://www.ngsolve.org) >= 6.2
-
-To access the newest features the nightly version of NGSolve works best and [lapack](http://www.netlib.org/lapack/) >= 3.9 is required.
+ * if you are using pip to install the package you can install the newest ngsolve and other dependencies using
+```bash
+pip install ngsolve --pre
+```
+ * if you build the package from source the following software needs to be installed
+   * [cmake](https://cmake.org/) >= 3.1
+   * [gcc](https://gcc.gnu.org/) >= 9 or [clang](https://clang.llvm.org/) >= 10
+   * [lapack](http://www.netlib.org/lapack/) >= 3.9 (required to access the newest features)
+   * [ngsolve](https://www.ngsolve.org) >= 6.2  (to access the newest features the nightly version of NGSolve works best)
 
 ## News
 ⚠️ Oct, 2022: With v0.2.0 the git history has undergone a major cleanup, please make sure to clone the repo anew.
 
 🚀 Oct, 2022: New and improved implementation of the embedded Trefftz method via `EmbeddedTrefftzFES`!
 
 🚀 Aug, 2022: Three different [pip](https://pypi.org/search/?q=ngstrefftz)-installer available, now using wheels! 
@@ -71,7 +74,12 @@
 * *A space-time quasi-Trefftz DG method for the wave equation with piecewise-smooth coefficients*   
 Lise-Marie Imbert-Gérard, Andrea Moiola, Paul Stocker  
 [![arXiv](https://img.shields.io/badge/arXiv-2011.04617-b31b1b.svg)](https://arxiv.org/abs/2011.04617)
 * *Tent pitching and Trefftz-DG method for the acoustic wave equation*  
 Ilaria Perugia, Joachim Schöberl, Paul Stocker, Christoph Wintersteiger   
 [![arXiv](https://img.shields.io/badge/arXiv-1907.02367-b31b1b.svg)](https://arxiv.org/abs/1907.02367)
 
+If you are using `ngstrefftz` in your academic work, please consider citing 
+```
+Stocker, P., (2022). NGSTrefftz: Add-on to NGSolve for Trefftz methods. 
+Journal of Open Source Software, 7(71), 4135, https://doi.org/10.21105/joss.04135
+```
```

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/README.md` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/py/_drawtents.py` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/_drawtents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/py/ctau_experiments.py` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/ctau_experiments.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/py/tentinfo.py` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/py/tentinfo.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/CMakeLists.txt` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/advection.cpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/advection.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/burgers.cpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/burgers.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/concurrentqueue.h` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/concurrentqueue.h`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/conservationlaw.hpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/conservationlaw.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/euler.cpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/euler.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/maxwell.cpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/maxwell.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/paralleldepend.hpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/paralleldepend.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/python_conslaw.cpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/python_conslaw.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/python_tents.cpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/python_tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/symbolic.cpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/symbolic.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/tents.cpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/tents.hpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/tentsolver.hpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tentsolver.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/tentsolver_impl.hpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/tentsolver_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/vis3d.cpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/vis3d.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/vis3d.hpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/vis3d.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/external_dependencies/ngstents/src/wave.cpp` & `ngstrefftz-src-0.2.3/external_dependencies/ngstents/src/wave.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/ngstrefftz_src.egg-info/PKG-INFO` & `ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz-src
-Version: 0.2.2
+Version: 0.2.3
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `ngstrefftz-src-0.2.2/ngstrefftz_src.egg-info/SOURCES.txt` & `ngstrefftz-src-0.2.3/ngstrefftz_src.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/setup.py` & `ngstrefftz-src-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,17 +116,19 @@
         # subprocess.check_call(['mkdir', 'ngstents'], cwd=self.build_lib)
         # subprocess.check_call(['mv', '_pytents.so', 'ngstents'], cwd=self.build_lib)
 
 import netgen.version
 import ngsolve
 import pkg_resources
 netgen_name = netgen.config.NETGEN_PYTHON_PACKAGE_NAME
-avx2 = netgen_name.replace('netgen-mesher', '') # keep -avx2 suffix
+# avx2 = netgen_name.replace('netgen-mesher', '') # keep -avx2 suffix
+avx2 = ''
 name = 'ngstrefftz' + avx2
-ngsolve_version = pkg_resources.get_distribution("ngsolve").version
+# ngsolve_version = pkg_resources.get_distribution("ngsolve").version
+ngsolve_version = '6.2.2301'
 install_requires = [ 'ngsolve'+avx2+'>='+ngsolve_version ]
 
 if sys.argv[1] == "sdist":
     package_data = {"ngstrefftz": ["*"
                                 ,"../test/*"
                                 ,"../external_dependencies/ngstents/*"\
                                 ,"../external_dependencies/ngstents/src/*"\
```

### Comparing `ngstrefftz-src-0.2.2/src/CMakeLists.txt` & `ngstrefftz-src-0.2.3/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/__init__.py` & `ngstrefftz-src-0.2.3/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/airy.cpp` & `ngstrefftz-src-0.2.3/src/airy.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/diffopmapped.hpp` & `ngstrefftz-src-0.2.3/src/diffopmapped.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/embtrefftz.cpp` & `ngstrefftz-src-0.2.3/src/embtrefftz.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                    SliceMatrix<Complex, ColMajor> V);
 }
 
 namespace ngcomp
 {
 
   template <class SCAL>
-  std::tuple<shared_ptr<Array<Matrix<SCAL>>>, shared_ptr<BaseVector>>
+  std::tuple<vector<shared_ptr<Matrix<SCAL>>>, shared_ptr<BaseVector>>
   EmbTrefftz (shared_ptr<SumOfIntegrals> bf, shared_ptr<FESpace> fes,
               shared_ptr<SumOfIntegrals> lf, double eps,
               shared_ptr<FESpace> test_fes, int tndof, bool getrange,
               std::map<std::string, Vector<SCAL>> *stats)
   {
     static Timer svdtt ("svdtrefftz");
     RegionTimer reg (svdtt);
@@ -127,46 +127,49 @@
     if (lf)
       for (auto icf : lf->icfs)
         {
           auto &dx = icf->dx;
           lfis[dx.vb] += icf->MakeLinearFormIntegrator ();
         }
 
-    Array<Matrix<SCAL>> ETmats (ne);
+    vector<shared_ptr<Matrix<SCAL>>> ETmats (ne);
     VVector<SCAL> lfvec (ndof);
+    lfvec = 0.0;
 
     size_t active_elements = 0;
     size_t test_local_ndof = test_fes->GetNDof () / ne;
     Vector<SCAL> sing_val_avg (test_local_ndof);
     sing_val_avg = 0;
     Vector<double> sing_val_max (test_local_ndof);
     sing_val_max = 0;
     Vector<double> sing_val_min (test_local_ndof);
     sing_val_min = DBL_MAX;
 
+    bool has_hidden_dofs = false;
+    for (DofId d = 0; d < ndof || !has_hidden_dofs; d++)
+      if (HIDDEN_DOF == fes->GetDofCouplingType (d))
+        has_hidden_dofs = true;
+
     ma->IterateElements (VOL, lh, [&] (auto ei, LocalHeap &mlh) {
       bool definedhere = false;
       for (auto icf : bf->icfs)
         {
           if (icf->dx.vb == VOL)
             if ((!icf->dx.definedonelements)
                 || (icf->dx.definedonelements->Test (ei.Nr ())))
               definedhere = true;
         }
       if (!definedhere)
         return; // escape lambda
 
-      Array<DofId> test_dofs;
+      Array<DofId> dofs, test_dofs;
       test_fes->GetDofNrs (ei, test_dofs);
-      Array<DofId> dofs;
       fes->GetDofNrs (ei, dofs);
 
       FlatMatrix<SCAL> elmat (test_dofs.Size (), dofs.Size (), mlh);
-      FlatMatrix<SCAL, ColMajor> U (test_dofs.Size (), mlh),
-          Vt (dofs.Size (), mlh);
 
       auto &trafo = ma->GetTrafo (ei, mlh);
 
       auto &test_fel = test_fes->GetFE (ei, mlh);
       auto &trial_fel = fes->GetFE (ei, mlh);
 
       elmat = 0.0;
@@ -201,35 +204,60 @@
                   cout << IM (6) << "ExceptionNOSIMD " << e.What () << endl
                        << "switching to scalar evaluation" << endl;
                   bfi->SetSimdEvaluate (false);
                   bfi_ind = 0;
                 }
             }
         }
+
+      if (has_hidden_dofs) // extract visible dofs, if needed
+        {
+          Array<DofId> vdofs, vtest_dofs;
+          fes->GetDofNrs (ei, vdofs, VISIBLE_DOF);
+          test_fes->GetDofNrs (ei, vtest_dofs, VISIBLE_DOF);
+          FlatMatrix<SCAL> velmat (vtest_dofs.Size (), vdofs.Size (), mlh);
+          for (int jj = 0; jj < dofs.Size (); jj++)
+            for (int ii = 0; ii < test_dofs.Size (); ii++)
+              {
+                auto j = vdofs.Pos (dofs[jj]);
+                auto i = vtest_dofs.Pos (test_dofs[ii]);
+                if (i != size_t (-1) && j != size_t (-1))
+                  velmat (i, j) = elmat (ii, jj);
+              }
+          dofs = std::move (vdofs);
+          test_dofs = std::move (vtest_dofs);
+          elmat.Assign (velmat);
+        }
+
+      FlatMatrix<SCAL, ColMajor> U (test_dofs.Size (), mlh),
+          Vt (dofs.Size (), mlh);
       ngbla::GetSVD<SCAL> (elmat, U, Vt);
 
       // either tndof is given, or try to determine local size of trefftz
       // space, must be at least dim(trefftz)>=dim(trial)-dim(test)
       int nz = 0;
       if (tndof)
         nz = tndof;
       else
         {
-          nz = max (trial_fel.GetNDof () - test_fel.GetNDof (), 0);
+          nz = dofs.Size () - test_dofs.Size ();
+          nz = max (nz, 0);
           for (int i = 0; i < min (elmat.Width (), elmat.Height ()); i++)
             if (abs (elmat (i, i)) < eps)
               nz++;
         }
-      if (trial_fel.GetNDof () - test_fel.GetNDof () > nz)
+      if (dofs.Size () - test_dofs.Size () > nz)
         throw Exception ("test fes not large enough for given tndof");
 
       if (getrange)
-        ETmats[ei.Nr ()] = U.Cols (0, dofs.Size () - nz);
+        ETmats[ei.Nr ()]
+            = make_shared<Matrix<SCAL>> (U.Cols (0, dofs.Size () - nz));
       else
-        ETmats[ei.Nr ()] = Trans (Vt.Rows (dofs.Size () - nz, dofs.Size ()));
+        ETmats[ei.Nr ()] = make_shared<Matrix<SCAL>> (
+            Trans (Vt.Rows (dofs.Size () - nz, dofs.Size ())));
 
       if (stats)
         {
           active_elements += 1;
           for (size_t i = 0; i < elmat.Height (); i++)
             {
               sing_val_avg[i] += elmat (i, i);
@@ -275,77 +303,95 @@
       {
         sing_val_avg /= active_elements;
         (*stats)["singavg"] = Vector<SCAL> (sing_val_avg);
         (*stats)["singmax"] = Vector<double> (sing_val_max);
         (*stats)["singmin"] = Vector<double> (sing_val_min);
       }
 
-    return std::make_tuple (make_shared<Array<Matrix<SCAL>>> (ETmats),
-                            make_shared<VVector<SCAL>> (lfvec));
+    return std::make_tuple (ETmats, make_shared<VVector<SCAL>> (lfvec));
   }
 
-  template std::tuple<shared_ptr<Array<Matrix<double>>>,
+  template std::tuple<vector<shared_ptr<Matrix<double>>>,
                       shared_ptr<BaseVector>>
   EmbTrefftz<double> (shared_ptr<SumOfIntegrals> bf, shared_ptr<FESpace> fes,
                       shared_ptr<SumOfIntegrals> lf, double eps,
                       shared_ptr<FESpace> test_fes, int tndof, bool getrange,
                       std::map<std::string, Vector<double>> *stats);
-  template std::tuple<shared_ptr<Array<Matrix<Complex>>>,
+  template std::tuple<vector<shared_ptr<Matrix<Complex>>>,
                       shared_ptr<BaseVector>>
   EmbTrefftz<Complex> (shared_ptr<SumOfIntegrals> bf, shared_ptr<FESpace> fes,
                        shared_ptr<SumOfIntegrals> lf, double eps,
                        shared_ptr<FESpace> test_fes, int tndof, bool getrange,
                        std::map<std::string, Vector<Complex>> *stats);
 
   template <class SCAL>
-  shared_ptr<BaseMatrix> Elmats2Sparse (shared_ptr<Array<Matrix<SCAL>>> ETmats,
-                                        shared_ptr<FESpace> fes)
+  shared_ptr<BaseMatrix>
+  Elmats2Sparse (vector<shared_ptr<Matrix<SCAL>>> ETmats,
+                 shared_ptr<FESpace> fes)
   {
     auto ma = fes->GetMeshAccess ();
     size_t ne = ma->GetNE (VOL);
     size_t ndof = fes->GetNDof ();
     size_t dim = fes->GetDimension ();
 
+    int hidden_dofs = 0;
+    for (DofId d : Range (ndof))
+      if (HIDDEN_DOF == fes->GetDofCouplingType (d))
+        hidden_dofs++;
+
     Table<int> table, table2;
-    TableCreator<int> creator (ne);
-    TableCreator<int> creator2 (ne);
+    TableCreator<int> creator (ne + hidden_dofs);
+    TableCreator<int> creator2 (ne + hidden_dofs);
     int prevdofs = 0;
+
     for (; !creator.Done (); creator++, creator2++)
       {
         prevdofs = 0;
         for (auto ei : ma->Elements (VOL))
           {
-            int nz = (*ETmats)[ei.Nr ()].Width ();
+            int nz = (ETmats[ei.Nr ()])->Width ();
             Array<DofId> dnums;
-            fes->GetDofNrs (ei, dnums);
+            fes->GetDofNrs (ei, dnums, VISIBLE_DOF);
             bool hasregdof = false;
             for (DofId d : dnums)
               if (IsRegularDof (d))
                 {
                   creator.Add (ei.Nr (), d);
                   hasregdof = true;
                 }
             // assumption here: Either all or no dof is regular
             if (hasregdof)
               {
                 for (int d = 0; d < nz; d++)
-                  creator2.Add (ei.Nr (), d + prevdofs);
-                prevdofs += nz;
+                  creator2.Add (ei.Nr (), prevdofs++);
               }
           }
+
+        for (int d = 0, hcnt = 0; d < ndof; d++)
+          if (HIDDEN_DOF == fes->GetDofCouplingType (d))
+            {
+              creator.Add (ne + hcnt, d);
+              creator2.Add (ne + hcnt++, prevdofs++);
+            }
       }
     table = creator.MoveTable ();
     table2 = creator2.MoveTable ();
 
     SparseMatrix<SCAL> PP (fes->GetNDof (), prevdofs, table, table2, false);
     auto P = make_shared<SparseMatrix<SCAL>> (PP);
     P->SetZero ();
     for (auto ei : ma->Elements (VOL))
       P->AddElementMatrix (table[ei.Nr ()], table2[ei.Nr ()],
-                           (*ETmats)[ei.Nr ()]);
+                           *(ETmats[ei.Nr ()]));
+
+    SCAL one = 1;
+    FlatMatrix<SCAL> I (1, 1, &one);
+    for (int hd = 0; hd < hidden_dofs; hd++)
+      P->AddElementMatrix (table[ne + hd], table2[ne + hd], I);
+
     return P;
   }
 
   ////////////////////////// EmbTrefftzFESpace ///////////////////////////
 
   template <typename T, typename shrdT>
   shared_ptr<BaseVector>
@@ -366,15 +412,15 @@
     T::Update ();
     int ndof = fes->GetNDof ();
     all2comp.SetSize (ndof);
     all2comp = 0;
 
     for (auto ei : this->ma->Elements (VOL))
       {
-        int nz = (*ETmats)[ei.Nr ()].Width ();
+        int nz = (ETmats[ei.Nr ()])->Width ();
         Array<DofId> dofs;
         T::GetDofNrs (ei, dofs);
         for (int i = nz; i < dofs.Size (); i++)
           all2comp[dofs[i]] = NO_DOF_NR_CONDENSE;
         ////for(int i=0;i<dofs.Size()-nz;i++)
         // for(int i=nz;i<dofs.Size();i++)
         ////this->free_dofs->Clear(dofs[i]);
@@ -397,14 +443,79 @@
       if (all2comp[i] >= 0)
         this->ctofdof[all2comp[i]] = T::GetDofCouplingType (i);
 
     T::FinalizeUpdate ();
     return std::get<1> (embtr);
   }
 
+  template <typename T, typename shrdT>
+  void EmbTrefftzFESpace<T, shrdT>::GetDofNrs (ElementId ei,
+                                               Array<int> &dnums) const
+  {
+    T::GetDofNrs (ei, dnums);
+    if (all2comp.Size () == fes->GetNDof ())
+      for (DofId &d : dnums)
+        if (IsRegularDof (d))
+          d = all2comp[d];
+  }
+
+  template <typename T, typename shrdT>
+  void
+  EmbTrefftzFESpace<T, shrdT>::VTransformMR (ElementId ei,
+                                             const SliceMatrix<double> mat,
+                                             TRANSFORM_TYPE type) const
+  {
+    static Timer timer ("EmbTrefftz: MTransform");
+    RegionTimer reg (timer);
+
+    size_t nz = (ETmats[ei.Nr ()])->Width ();
+    Matrix<double> temp_mat (mat.Height (), mat.Width ());
+
+    if (type == TRANSFORM_MAT_LEFT)
+      {
+        temp_mat.Rows (0, nz) = Trans (*(ETmats[ei.Nr ()])) * mat;
+        mat = temp_mat;
+      }
+    if (type == TRANSFORM_MAT_RIGHT)
+      {
+        temp_mat.Cols (0, nz) = mat * (*(ETmats[ei.Nr ()]));
+        mat = temp_mat;
+      }
+    if (type == TRANSFORM_MAT_LEFT_RIGHT)
+      {
+        temp_mat.Cols (0, nz) = mat * (*(ETmats[ei.Nr ()]));
+        mat.Rows (0, nz) = Trans (*(ETmats[ei.Nr ()])) * temp_mat;
+      }
+  }
+
+  template <typename T, typename shrdT>
+  void
+  EmbTrefftzFESpace<T, shrdT>::VTransformVR (ElementId ei,
+                                             const SliceVector<double> vec,
+                                             TRANSFORM_TYPE type) const
+  {
+    static Timer timer ("EmbTrefftz: VTransform");
+    RegionTimer reg (timer);
+
+    size_t nz = (ETmats[ei.Nr ()])->Width ();
+
+    if (type == TRANSFORM_RHS)
+      {
+        Vector<double> new_vec (vec.Size ());
+        new_vec = Trans (*(ETmats[ei.Nr ()])) * vec;
+        vec = new_vec;
+      }
+    else if (type == TRANSFORM_SOL)
+      {
+        Vector<double> new_vec (vec.Size ());
+        new_vec = (*(ETmats[ei.Nr ()])) * vec;
+        vec = new_vec;
+      }
+  }
+
   template class EmbTrefftzFESpace<L2HighOrderFESpace,
                                    shared_ptr<L2HighOrderFESpace>>;
   static RegisterFESpace<
       EmbTrefftzFESpace<L2HighOrderFESpace, shared_ptr<L2HighOrderFESpace>>>
       initembt ("L2EmbTrefftzFESpace");
 
   template class EmbTrefftzFESpace<VectorL2FESpace,
@@ -416,16 +527,17 @@
   template class EmbTrefftzFESpace<MonomialFESpace,
                                    shared_ptr<MonomialFESpace>>;
   static RegisterFESpace<
       EmbTrefftzFESpace<MonomialFESpace, shared_ptr<MonomialFESpace>>>
       initembt3 ("MonomialEmbTrefftzFESpace");
 }
 
-#ifdef NGS_PYTHON
+////////////////////////// python interface ///////////////////////////
 
+#ifdef NGS_PYTHON
 template <typename T, typename shrdT>
 void ExportETSpace (py::module m, string label)
 {
   auto pyspace
       = ngcomp::ExportFESpace<ngcomp::EmbTrefftzFESpace<T, shrdT>> (m, label);
 
   pyspace.def (py::init ([pyspace] (shrdT fes) {
@@ -497,31 +609,35 @@
                         shared_ptr<ngcomp::BaseVector>> {
         shared_ptr<py::dict> pystats = nullptr;
         if (stats_dict)
           pystats = make_shared<py::dict> (*stats_dict);
 
         if (fes->IsComplex ())
           {
-            std::map<std::string, ngcomp::Vector<Complex>> stats;
+            std::map<std::string, ngcomp::Vector<Complex>> *stats = nullptr;
+            if (pystats)
+              stats = new std::map<std::string, ngcomp::Vector<Complex>>;
             auto P = ngcomp::EmbTrefftz<Complex> (bf, fes, lf, eps, test_fes,
-                                                  tndof, getrange, &stats);
+                                                  tndof, getrange, stats);
             if (pystats)
-              for (auto const &x : stats)
+              for (auto const &x : *stats)
                 (*pystats)[py::cast (x.first)] = py::cast (x.second);
             return std::make_tuple (
                 ngcomp::Elmats2Sparse<Complex> (std::get<0> (P), fes),
                 std::get<1> (P));
           }
         else
           {
-            std::map<std::string, ngcomp::Vector<double>> stats;
+            std::map<std::string, ngcomp::Vector<double>> *stats = nullptr;
+            if (pystats)
+              stats = new std::map<std::string, ngcomp::Vector<double>>;
             auto P = ngcomp::EmbTrefftz<double> (bf, fes, lf, eps, test_fes,
-                                                 tndof, getrange, &stats);
+                                                 tndof, getrange, stats);
             if (pystats)
-              for (auto const &x : stats)
+              for (auto const &x : *stats)
                 (*pystats)[py::cast (x.first)] = py::cast (x.second);
             return std::make_tuple (
                 ngcomp::Elmats2Sparse<double> (std::get<0> (P), fes),
                 std::get<1> (P));
           }
       },
       R"mydelimiter(
@@ -550,29 +666,33 @@
           optional<py::dict> stats_dict) -> shared_ptr<ngcomp::BaseMatrix> {
         shared_ptr<py::dict> pystats = nullptr;
         if (stats_dict)
           pystats = make_shared<py::dict> (*stats_dict);
 
         if (fes->IsComplex ())
           {
-            std::map<std::string, ngcomp::Vector<Complex>> stats;
+            std::map<std::string, ngcomp::Vector<Complex>> *stats = nullptr;
+            if (pystats)
+              stats = new std::map<std::string, ngcomp::Vector<Complex>>;
             auto P = std::get<0> (ngcomp::EmbTrefftz<Complex> (
-                bf, fes, nullptr, eps, test_fes, tndof, getrange, &stats));
+                bf, fes, nullptr, eps, test_fes, tndof, getrange, stats));
             if (pystats)
-              for (auto const &x : stats)
+              for (auto const &x : *stats)
                 (*pystats)[py::cast (x.first)] = py::cast (x.second);
             return ngcomp::Elmats2Sparse<Complex> (P, fes);
           }
         else
           {
-            std::map<std::string, ngcomp::Vector<double>> stats;
+            std::map<std::string, ngcomp::Vector<double>> *stats = nullptr;
+            if (pystats)
+              stats = new std::map<std::string, ngcomp::Vector<double>>;
             auto P = std::get<0> (ngcomp::EmbTrefftz<double> (
-                bf, fes, nullptr, eps, test_fes, tndof, getrange, &stats));
+                bf, fes, nullptr, eps, test_fes, tndof, getrange, stats));
             if (pystats)
-              for (auto const &x : stats)
+              for (auto const &x : *stats)
                 (*pystats)[py::cast (x.first)] = py::cast (x.second);
             return ngcomp::Elmats2Sparse<double> (P, fes);
           }
       },
       R"mydelimiter(
                 Used without the parameter lf as input the function only returns the Trefftz embedding.
```

### Comparing `ngstrefftz-src-0.2.2/src/embtrefftz.hpp` & `ngstrefftz-src-0.2.3/src/embtrefftz.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 #include <fem.hpp>
 #include <integratorcf.hpp>
 #include <variant>
 #include <bla.hpp>
 
 namespace ngcomp
 {
+
   template <class SCAL>
-  std::tuple<shared_ptr<BaseMatrix>, shared_ptr<BaseVector>>
+  std::tuple<vector<shared_ptr<Matrix<SCAL>>>, shared_ptr<BaseVector>>
   EmbTrefftz (shared_ptr<SumOfIntegrals> bf, shared_ptr<FESpace> fes,
               shared_ptr<SumOfIntegrals> lf, double eps,
-              shared_ptr<FESpace> fes_test, int tndof,
+              shared_ptr<FESpace> test_fes, int tndof, bool getrange,
               std::map<std::string, Vector<SCAL>> *stats = nullptr);
 
   template <typename T, typename shrdT>
   class EmbTrefftzFESpace
       : public T //, public std::enable_shared_from_this<EmbTrefftzFESpace>
   {
-    shared_ptr<Array<Matrix<double>>> ETmats;
+    vector<shared_ptr<Matrix<double>>> ETmats;
     shrdT fes;
     Array<DofId> all2comp;
 
   public:
     EmbTrefftzFESpace (shared_ptr<MeshAccess> ama, const Flags &flags,
                        bool parseflags = false)
         : T (ama, flags, parseflags)
@@ -44,74 +45,22 @@
       // this->FinalizeUpdate();
     }
 
     shared_ptr<BaseVector>
     SetOp (shared_ptr<SumOfIntegrals> bf, shared_ptr<SumOfIntegrals> lf,
            double eps, shared_ptr<FESpace> test_fes, int tndof);
 
-    void GetDofNrs (ElementId ei, Array<int> &dnums) const override
-    {
-      T::GetDofNrs (ei, dnums);
-      if (all2comp.Size () == fes->GetNDof ())
-        for (DofId &d : dnums)
-          if (IsRegularDof (d))
-            d = all2comp[d];
-    }
-
-    void VTransformMR (ElementId ei, const SliceMatrix<double> mat,
-                       TRANSFORM_TYPE type) const
-    {
-      static Timer timer ("EmbTrefftz: MTransform");
-      RegionTimer reg (timer);
-
-      size_t nz = ((*ETmats)[ei.Nr ()]).Width ();
-      Matrix<double> bla (mat.Height (), mat.Width ());
+    void GetDofNrs (ElementId ei, Array<int> &dnums) const override;
 
-      if (type == TRANSFORM_MAT_LEFT)
-        {
-          bla.Rows (0, nz) = Trans ((*ETmats)[ei.Nr ()]) * mat;
-          mat = bla;
-        }
-      if (type == TRANSFORM_MAT_RIGHT)
-        {
-          bla.Cols (0, nz) = mat * ((*ETmats)[ei.Nr ()]);
-          mat = bla;
-        }
-      if (type == TRANSFORM_MAT_LEFT_RIGHT)
-        {
-          // mat = mat * Trans(*ETmats[ei.Nr()]);
-          // mat = (*ETmats[ei.Nr()]) * mat;
-          bla.Cols (0, nz) = mat * ((*ETmats)[ei.Nr ()]);
-          mat.Rows (0, nz) = Trans ((*ETmats)[ei.Nr ()]) * bla;
-        }
-    }
+    virtual void VTransformMR (ElementId ei, const SliceMatrix<double> mat,
+                               TRANSFORM_TYPE type) const override;
 
     virtual void VTransformVR (ElementId ei, const SliceVector<double> vec,
-                               TRANSFORM_TYPE type) const
-    {
-      static Timer timer ("EmbTrefftz: VTransform");
-      RegionTimer reg (timer);
-      size_t nz = ((*ETmats)[ei.Nr ()]).Width ();
-      if (type == TRANSFORM_RHS)
-        {
-          Vector<double> new_vec (vec.Size ());
-          new_vec = Trans ((*ETmats)[ei.Nr ()]) * vec;
-          vec = new_vec;
-        }
-      else if (type == TRANSFORM_SOL)
-        {
-          Vector<double> new_vec (vec.Size ());
-          new_vec = ((*ETmats)[ei.Nr ()]) * vec;
-          vec = new_vec;
-        }
-      else
-        cout << "transform " << type << " nothing here" << endl;
-    }
+                               TRANSFORM_TYPE type) const override;
   };
-
 }
 
 #ifdef NGS_PYTHON
 #include <python_ngstd.hpp>
 void ExportEmbTrefftz (py::module m);
 #endif // NGS_PYTHON
```

### Comparing `ngstrefftz-src-0.2.2/src/intrule4.cpp` & `ngstrefftz-src-0.2.3/src/intrule4.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/mesh1dtents.cpp` & `ngstrefftz-src-0.2.3/src/mesh1dtents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/monomialfespace.cpp` & `ngstrefftz-src-0.2.3/src/monomialfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/monomialfespace.hpp` & `ngstrefftz-src-0.2.3/src/monomialfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/planewavefe.cpp` & `ngstrefftz-src-0.2.3/src/planewavefe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/planewavefe.hpp` & `ngstrefftz-src-0.2.3/src/planewavefe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/python_trefftz.cpp` & `ngstrefftz-src-0.2.3/src/python_trefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/scalarmappedfe.cpp` & `ngstrefftz-src-0.2.3/src/scalarmappedfe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/scalarmappedfe.hpp` & `ngstrefftz-src-0.2.3/src/scalarmappedfe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/specialcoefficientfunction.cpp` & `ngstrefftz-src-0.2.3/src/specialcoefficientfunction.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/specialcoefficientfunction.hpp` & `ngstrefftz-src-0.2.3/src/specialcoefficientfunction.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/trefftzfespace.cpp` & `ngstrefftz-src-0.2.3/src/trefftzfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/trefftzfespace.hpp` & `ngstrefftz-src-0.2.3/src/trefftzfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/twavetents.cpp` & `ngstrefftz-src-0.2.3/src/twavetents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/src/twavetents.hpp` & `ngstrefftz-src-0.2.3/src/twavetents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/test/embt.py` & `ngstrefftz-src-0.2.3/test/embt.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/test/tents.py` & `ngstrefftz-src-0.2.3/test/tents.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     >>> SetNumThreads(4)
     >>> c = 1
     >>> t_step = 2/sqrt(3)
     >>> initmesh = Mesh(unit_square.GenerateMesh(maxh = 0.4))
     >>> for maxh in range(3):
     ...     SolveWaveTentsFO(initmesh, order, c, t_step) # doctest:+ELLIPSIS
     ...     initmesh.Refine()
-    0.01...
+    0.0...
     0.00...
     0.0001...
     """
 
     D = initmesh.dim
     t = CoordCF(D)
     t_start = 0
```

### Comparing `ngstrefftz-src-0.2.2/test/trefftz.py` & `ngstrefftz-src-0.2.3/test/trefftz.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-src-0.2.2/test/twave.py` & `ngstrefftz-src-0.2.3/test/twave.py`

 * *Files identical despite different names*


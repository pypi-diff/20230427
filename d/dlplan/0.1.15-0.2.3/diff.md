# Comparing `tmp/dlplan-0.1.15.tar.gz` & `tmp/dlplan-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlplan-0.1.15.tar", last modified: Fri Apr 21 20:48:41 2023, max compression
+gzip compressed data, was "dlplan-0.2.3.tar", last modified: Thu Apr 27 15:38:56 2023, max compression
```

## Comparing `dlplan-0.1.15.tar` & `dlplan-0.2.3.tar`

### file list

```diff
@@ -1,423 +1,414 @@
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.981469 dlplan-0.1.15/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2239 2023-03-31 08:44:12.000000 dlplan-0.1.15/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    34916 2022-09-07 06:24:55.000000 dlplan-0.1.15/LICENSE.md
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      338 2023-03-20 10:57:38.000000 dlplan-0.1.15/MANIFEST.in
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      345 2023-04-21 20:48:41.981469 dlplan-0.1.15/PKG-INFO
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4772 2023-03-31 09:18:26.000000 dlplan-0.1.15/README.md
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.933468 dlplan-0.1.15/api/
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.937468 dlplan-0.1.15/api/python/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1068 2023-04-06 08:55:26.000000 dlplan-0.1.15/api/python/CMakeLists.txt
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.941468 dlplan-0.1.15/api/python/src/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    17252 2023-04-05 11:38:47.000000 dlplan-0.1.15/api/python/src/core.cpp
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.941468 dlplan-0.1.15/api/python/src/dlplan/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      204 2022-09-07 06:24:55.000000 dlplan-0.1.15/api/python/src/dlplan/__init__.py
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.941468 dlplan-0.1.15/api/python/src/dlplan.egg-info/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      345 2023-04-21 20:48:41.000000 dlplan-0.1.15/api/python/src/dlplan.egg-info/PKG-INFO
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    12146 2023-04-21 20:48:41.000000 dlplan-0.1.15/api/python/src/dlplan.egg-info/SOURCES.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)        1 2023-04-21 20:48:41.000000 dlplan-0.1.15/api/python/src/dlplan.egg-info/dependency_links.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)        1 2023-03-20 12:47:52.000000 dlplan-0.1.15/api/python/src/dlplan.egg-info/not-zip-safe
--rw-rw-r--   0 dominik   (1000) dominik   (1000)       62 2023-04-21 20:48:41.000000 dlplan-0.1.15/api/python/src/dlplan.egg-info/requires.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)       15 2023-04-21 20:48:41.000000 dlplan-0.1.15/api/python/src/dlplan.egg-info/top_level.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     5792 2023-04-05 09:47:43.000000 dlplan-0.1.15/api/python/src/generator.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      830 2023-04-06 09:00:15.000000 dlplan-0.1.15/api/python/src/main.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4070 2023-03-31 09:18:08.000000 dlplan-0.1.15/api/python/src/novelty.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     5615 2023-03-27 14:29:17.000000 dlplan-0.1.15/api/python/src/policy.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2738 2023-04-17 12:39:54.000000 dlplan-0.1.15/api/python/src/state_space.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      784 2022-09-26 12:30:34.000000 dlplan-0.1.15/api/python/src/weisfeiler_lehman.cpp
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.941468 dlplan-0.1.15/api/python/test/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)        0 2022-09-07 06:24:55.000000 dlplan-0.1.15/api/python/test/__init__.py
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.941468 dlplan-0.1.15/api/python/test/__pycache__/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      153 2022-09-29 07:55:44.000000 dlplan-0.1.15/api/python/test/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4387 2023-03-30 13:10:35.000000 dlplan-0.1.15/api/python/test/__pycache__/test_barman.cpython-38-pytest-6.2.5.pyc
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    12899 2023-04-04 15:43:46.000000 dlplan-0.1.15/api/python/test/__pycache__/test_core.cpython-38-pytest-6.2.5.pyc
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2147 2023-04-04 15:43:46.000000 dlplan-0.1.15/api/python/test/__pycache__/test_generate.cpython-38-pytest-6.2.5.pyc
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3319 2023-03-30 13:10:34.000000 dlplan-0.1.15/api/python/test/test_barman.py
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4098 2023-03-31 09:30:57.000000 dlplan-0.1.15/api/python/test/test_core.py
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4467 2023-04-04 15:42:11.000000 dlplan-0.1.15/api/python/test/test_generate.py
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.941468 dlplan-0.1.15/examples/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      106 2022-10-04 09:53:17.000000 dlplan-0.1.15/examples/CMakeLists.txt
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.941468 dlplan-0.1.15/examples/core/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)       85 2022-09-07 06:24:55.000000 dlplan-0.1.15/examples/core/CMakeLists.txt
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.941468 dlplan-0.1.15/examples/core/__pycache__/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4645 2022-09-07 06:24:55.000000 dlplan-0.1.15/examples/core/__pycache__/tarski.cpython-36.pyc
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4663 2022-09-07 06:24:55.000000 dlplan-0.1.15/examples/core/__pycache__/tarski.cpython-37.pyc
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2310 2023-03-30 08:44:23.000000 dlplan-0.1.15/examples/core/core.cpp
--rwxrwxr-x   0 dominik   (1000) dominik   (1000)     2438 2023-02-08 14:06:08.000000 dlplan-0.1.15/examples/core/core.py
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.945468 dlplan-0.1.15/examples/generator/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      121 2022-09-07 06:24:55.000000 dlplan-0.1.15/examples/generator/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3036 2023-04-04 15:37:09.000000 dlplan-0.1.15/examples/generator/generator.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2562 2023-04-04 15:37:16.000000 dlplan-0.1.15/examples/generator/generator.py
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.945468 dlplan-0.1.15/examples/policy/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      103 2022-09-07 06:24:55.000000 dlplan-0.1.15/examples/policy/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3247 2023-03-27 14:29:17.000000 dlplan-0.1.15/examples/policy/policy.cpp
--rwxrwxr-x   0 dominik   (1000) dominik   (1000)     1925 2022-09-26 12:30:34.000000 dlplan-0.1.15/examples/policy/policy.py
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.945468 dlplan-0.1.15/examples/state_space/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)       27 2022-10-04 09:53:17.000000 dlplan-0.1.15/examples/state_space/CMakeLists.txt
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.945468 dlplan-0.1.15/examples/state_space/delivery/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      913 2023-03-20 08:30:53.000000 dlplan-0.1.15/examples/state_space/delivery/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2261 2023-04-06 07:52:07.000000 dlplan-0.1.15/examples/state_space/delivery/delivery.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1992 2023-03-30 06:56:50.000000 dlplan-0.1.15/examples/state_space/delivery/delivery.py
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1271 2022-10-04 09:53:17.000000 dlplan-0.1.15/examples/state_space/delivery/domain.pddl
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      704 2022-10-04 09:53:17.000000 dlplan-0.1.15/examples/state_space/delivery/instance_2_1_0.pddl
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      749 2022-10-04 09:53:17.000000 dlplan-0.1.15/examples/state_space/delivery/instance_2_2_0.pddl
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.949468 dlplan-0.1.15/experiments/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      353 2023-03-20 08:31:30.000000 dlplan-0.1.15/experiments/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1271 2022-09-07 06:24:55.000000 dlplan-0.1.15/experiments/domain.pddl
--rwxrwxr-x   0 dominik   (1000) dominik   (1000)  2510856 2023-04-21 20:28:19.000000 dlplan-0.1.15/experiments/experiment_generator
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     6140 2023-04-06 07:58:39.000000 dlplan-0.1.15/experiments/experiment_generator.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1543 2022-09-26 12:30:34.000000 dlplan-0.1.15/experiments/experiment_parser.py
--rwxrwxr-x   0 dominik   (1000) dominik   (1000)     5147 2023-03-20 08:31:41.000000 dlplan-0.1.15/experiments/experiment_runner.py
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2100 2022-09-07 06:24:55.000000 dlplan-0.1.15/experiments/instance_large.pddl
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      749 2022-09-07 06:24:55.000000 dlplan-0.1.15/experiments/instance_small.pddl
--rwxrwxr-x   0 dominik   (1000) dominik   (1000)     2891 2022-09-07 06:24:55.000000 dlplan-0.1.15/experiments/main.py
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.933468 dlplan-0.1.15/include/
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.949468 dlplan-0.1.15/include/dlplan/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    25657 2023-04-05 11:34:02.000000 dlplan-0.1.15/include/dlplan/core.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4502 2023-04-05 09:40:57.000000 dlplan-0.1.15/include/dlplan/generator.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     7208 2023-03-31 09:00:57.000000 dlplan-0.1.15/include/dlplan/novelty.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.953468 dlplan-0.1.15/include/dlplan/phmap/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)   166554 2022-09-07 06:24:55.000000 dlplan-0.1.15/include/dlplan/phmap/btree.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     5404 2022-09-07 06:24:55.000000 dlplan-0.1.15/include/dlplan/phmap/meminfo.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)   186642 2022-09-07 06:24:55.000000 dlplan-0.1.15/include/dlplan/phmap/phmap.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)   180847 2022-09-07 06:24:55.000000 dlplan-0.1.15/include/dlplan/phmap/phmap_base.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    22491 2022-09-07 06:24:55.000000 dlplan-0.1.15/include/dlplan/phmap/phmap_bits.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    28525 2022-09-07 06:24:55.000000 dlplan-0.1.15/include/dlplan/phmap/phmap_config.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     9632 2022-09-07 06:24:55.000000 dlplan-0.1.15/include/dlplan/phmap/phmap_dump.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     6257 2022-09-07 06:24:55.000000 dlplan-0.1.15/include/dlplan/phmap/phmap_fwd_decl.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    10739 2022-09-07 06:24:55.000000 dlplan-0.1.15/include/dlplan/phmap/phmap_utils.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    10680 2023-03-31 09:03:15.000000 dlplan-0.1.15/include/dlplan/policy.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3747 2023-04-17 12:39:40.000000 dlplan-0.1.15/include/dlplan/state_space.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.953468 dlplan-0.1.15/include/dlplan/utils/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4412 2023-02-01 07:29:13.000000 dlplan-0.1.15/include/dlplan/utils/cache.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     6652 2022-11-13 08:50:15.000000 dlplan-0.1.15/include/dlplan/utils/dynamic_bitset.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      475 2022-09-26 12:30:34.000000 dlplan-0.1.15/include/dlplan/utils/hashing.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1591 2022-09-07 06:24:55.000000 dlplan-0.1.15/include/dlplan/utils/pimpl.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1289 2022-10-17 06:43:50.000000 dlplan-0.1.15/include/dlplan/weisfeiler_lehman.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      179 2023-03-21 07:01:08.000000 dlplan-0.1.15/pyproject.toml
--rw-rw-r--   0 dominik   (1000) dominik   (1000)       47 2023-03-20 09:59:47.000000 dlplan-0.1.15/requirements.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)       38 2023-04-21 20:48:41.981469 dlplan-0.1.15/setup.cfg
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2426 2023-04-21 20:48:28.000000 dlplan-0.1.15/setup.py
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.953468 dlplan-0.1.15/src/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      170 2023-04-06 07:53:18.000000 dlplan-0.1.15/src/CMakeLists.txt
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.957468 dlplan-0.1.15/src/core/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      805 2022-09-12 07:41:00.000000 dlplan-0.1.15/src/core/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1259 2023-03-31 09:27:58.000000 dlplan-0.1.15/src/core/atom.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1129 2023-03-30 09:37:40.000000 dlplan-0.1.15/src/core/cache.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      785 2023-03-30 13:07:09.000000 dlplan-0.1.15/src/core/constant.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    25107 2023-04-05 11:38:10.000000 dlplan-0.1.15/src/core/core.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    12883 2023-03-30 12:44:02.000000 dlplan-0.1.15/src/core/element_factory.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3319 2023-03-30 12:44:06.000000 dlplan-0.1.15/src/core/element_factory.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.957468 dlplan-0.1.15/src/core/elements/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2748 2023-03-30 06:56:50.000000 dlplan-0.1.15/src/core/elements/boolean.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.957468 dlplan-0.1.15/src/core/elements/booleans/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1940 2023-03-30 06:36:28.000000 dlplan-0.1.15/src/core/elements/booleans/empty.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2673 2023-03-30 06:36:28.000000 dlplan-0.1.15/src/core/elements/booleans/inclusion.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2154 2023-03-31 09:30:43.000000 dlplan-0.1.15/src/core/elements/booleans/nullary.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3085 2023-03-30 06:56:50.000000 dlplan-0.1.15/src/core/elements/concept.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.957468 dlplan-0.1.15/src/core/elements/concepts/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3134 2023-03-30 08:47:44.000000 dlplan-0.1.15/src/core/elements/concepts/all.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3347 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/concepts/and.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1582 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/concepts/bot.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3039 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/concepts/diff.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3402 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/concepts/equal.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2483 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/concepts/not.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2509 2023-03-30 08:51:09.000000 dlplan-0.1.15/src/core/elements/concepts/one_of.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3340 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/concepts/or.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3236 2023-03-31 09:30:57.000000 dlplan-0.1.15/src/core/elements/concepts/primitive.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2896 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/concepts/projection.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3093 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/concepts/some.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3260 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/concepts/subset.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1708 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/concepts/top.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1539 2023-03-30 07:42:06.000000 dlplan-0.1.15/src/core/elements/element.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2757 2023-03-30 06:56:50.000000 dlplan-0.1.15/src/core/elements/numerical.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.957468 dlplan-0.1.15/src/core/elements/numericals/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4402 2023-03-30 06:36:28.000000 dlplan-0.1.15/src/core/elements/numericals/concept_distance.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1936 2023-03-30 08:10:27.000000 dlplan-0.1.15/src/core/elements/numericals/count.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4408 2023-03-30 06:36:28.000000 dlplan-0.1.15/src/core/elements/numericals/role_distance.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4353 2023-03-30 06:36:28.000000 dlplan-0.1.15/src/core/elements/numericals/sum_concept_distance.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4552 2023-03-30 06:36:28.000000 dlplan-0.1.15/src/core/elements/numericals/sum_role_distance.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3049 2023-03-30 06:56:50.000000 dlplan-0.1.15/src/core/elements/role.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.961468 dlplan-0.1.15/src/core/elements/roles/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3102 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/and.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3229 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/compose.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2927 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/diff.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2518 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/identity.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2446 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/inverse.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2340 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/not.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3095 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/or.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3695 2023-03-31 09:28:21.000000 dlplan-0.1.15/src/core/elements/roles/primitive.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3124 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/restrict.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1661 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/top.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3033 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/transitive_closure.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3339 2023-03-30 08:47:41.000000 dlplan-0.1.15/src/core/elements/roles/transitive_reflexive_closure.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      479 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/elements/types.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4095 2023-03-30 07:40:16.000000 dlplan-0.1.15/src/core/elements/utils.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      789 2022-10-17 06:43:50.000000 dlplan-0.1.15/src/core/elements/utils.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     6375 2023-03-31 09:27:22.000000 dlplan-0.1.15/src/core/instance_info.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      741 2023-03-30 13:05:23.000000 dlplan-0.1.15/src/core/object.cpp
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.961468 dlplan-0.1.15/src/core/parser/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     8134 2023-03-30 12:37:27.000000 dlplan-0.1.15/src/core/parser/expression_factory.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      384 2023-03-30 12:37:31.000000 dlplan-0.1.15/src/core/parser/expression_factory.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.961468 dlplan-0.1.15/src/core/parser/expressions/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      849 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/boolean.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.961468 dlplan-0.1.15/src/core/parser/expressions/booleans/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1403 2022-10-26 07:38:37.000000 dlplan-0.1.15/src/core/parser/expressions/booleans/empty.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1694 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/booleans/inclusion.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1040 2023-03-30 12:15:34.000000 dlplan-0.1.15/src/core/parser/expressions/booleans/nullary.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      848 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concept.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.961468 dlplan-0.1.15/src/core/parser/expressions/concepts/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1210 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/all.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1249 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/and.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      844 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/bot.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1199 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/diff.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1247 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/equal.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1099 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/not.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      957 2023-03-30 12:16:19.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/one_of.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1242 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/or.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1122 2023-03-30 12:15:44.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/primitive.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1383 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/projection.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1221 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/some.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1255 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/subset.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      844 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/concepts/top.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2338 2022-10-17 06:43:50.000000 dlplan-0.1.15/src/core/parser/expressions/expression.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      875 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/numerical.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.961468 dlplan-0.1.15/src/core/parser/expressions/numericals/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1450 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/numericals/concept_distance.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1395 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/numericals/count.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1390 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/numericals/role_distance.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1478 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/numericals/sum_concept_distance.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1417 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/numericals/sum_role_distance.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      810 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/role.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.965468 dlplan-0.1.15/src/core/parser/expressions/roles/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1240 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/and.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1239 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/compose.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1215 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/diff.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1132 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/identity.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1106 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/inverse.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1050 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/not.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1236 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/or.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1158 2023-03-30 12:15:54.000000 dlplan-0.1.15/src/core/parser/expressions/roles/primitive.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1253 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/restrict.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      811 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/top.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1165 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/transitive_closure.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1240 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/core/parser/expressions/roles/transitive_reflexive_closure.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2192 2023-03-30 12:38:17.000000 dlplan-0.1.15/src/core/parser/parser.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      911 2023-03-30 12:38:09.000000 dlplan-0.1.15/src/core/parser/parser.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      216 2022-10-17 06:43:50.000000 dlplan-0.1.15/src/core/parser/types.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1123 2022-10-17 06:43:50.000000 dlplan-0.1.15/src/core/parser/utils.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1070 2023-03-30 13:07:32.000000 dlplan-0.1.15/src/core/predicate.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3351 2023-03-31 09:28:21.000000 dlplan-0.1.15/src/core/state.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2231 2023-03-31 09:27:43.000000 dlplan-0.1.15/src/core/vocabulary_info.cpp
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.965468 dlplan-0.1.15/src/generator/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1610 2022-10-26 12:37:49.000000 dlplan-0.1.15/src/generator/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    11859 2023-04-04 15:36:27.000000 dlplan-0.1.15/src/generator/feature_generator.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     5618 2023-04-05 08:07:38.000000 dlplan-0.1.15/src/generator/feature_generator.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     8630 2023-04-05 09:40:24.000000 dlplan-0.1.15/src/generator/generator.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2705 2022-10-17 06:43:50.000000 dlplan-0.1.15/src/generator/generator_data.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.965468 dlplan-0.1.15/src/generator/rules/
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.965468 dlplan-0.1.15/src/generator/rules/booleans/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1455 2023-03-30 07:57:50.000000 dlplan-0.1.15/src/generator/rules/booleans/empty.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      406 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/booleans/empty.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1938 2023-03-30 07:57:37.000000 dlplan-0.1.15/src/generator/rules/booleans/inclusion.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      418 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/booleans/inclusion.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1085 2023-03-30 12:42:52.000000 dlplan-0.1.15/src/generator/rules/booleans/nullary.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      412 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/booleans/nullary.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.969468 dlplan-0.1.15/src/generator/rules/concepts/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1148 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/all.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      400 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/all.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1155 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/and.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      400 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/and.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      840 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/bot.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      400 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/bot.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1161 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/diff.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      403 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/diff.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2289 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/equal.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      407 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/equal.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      917 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/not.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      400 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/not.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      979 2023-03-30 12:43:30.000000 dlplan-0.1.15/src/generator/rules/concepts/one_of.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      408 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/one_of.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1149 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/or.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      397 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/or.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1086 2023-03-30 12:43:07.000000 dlplan-0.1.15/src/generator/rules/concepts/primitive.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      418 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/primitive.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1043 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/projection.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      421 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/projection.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1154 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/some.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      403 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/some.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1266 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/subset.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      409 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/subset.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      840 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/concepts/top.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      400 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/concepts/top.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.969468 dlplan-0.1.15/src/generator/rules/numericals/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3468 2023-03-30 08:11:37.000000 dlplan-0.1.15/src/generator/rules/numericals/concept_distance.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      444 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/numericals/concept_distance.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1471 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/numericals/count.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      412 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/numericals/count.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.969468 dlplan-0.1.15/src/generator/rules/roles/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1128 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/and.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      391 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/and.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1153 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/compose.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      403 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/compose.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1134 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/diff.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      470 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/diff.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      926 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/identity.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      406 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/identity.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      916 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/inverse.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      435 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/inverse.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      894 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/not.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      391 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/not.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1122 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/or.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      388 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/or.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1068 2023-03-30 12:43:18.000000 dlplan-0.1.15/src/generator/rules/roles/primitive.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      409 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/primitive.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1258 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/restrict.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      406 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/restrict.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      820 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/top.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      391 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/top.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1055 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/transitive_closure.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      435 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/transitive_closure.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1112 2023-03-30 07:58:15.000000 dlplan-0.1.15/src/generator/rules/roles/transitive_reflexive_closure.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      464 2022-10-26 07:27:05.000000 dlplan-0.1.15/src/generator/rules/roles/transitive_reflexive_closure.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1368 2022-10-26 07:25:21.000000 dlplan-0.1.15/src/generator/rules/rule.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.969468 dlplan-0.1.15/src/novelty/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      651 2022-10-20 12:35:57.000000 dlplan-0.1.15/src/novelty/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)       75 2022-10-17 06:43:50.000000 dlplan-0.1.15/src/novelty/novelty.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1972 2023-03-31 09:01:53.000000 dlplan-0.1.15/src/novelty/novelty_base.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1887 2023-02-01 07:29:13.000000 dlplan-0.1.15/src/novelty/novelty_table.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    12678 2023-04-06 07:56:07.000000 dlplan-0.1.15/src/novelty/tuple_graph.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     5106 2023-03-31 09:01:46.000000 dlplan-0.1.15/src/novelty/tuple_index_generator.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1453 2023-03-30 12:44:48.000000 dlplan-0.1.15/src/novelty/tuple_node.cpp
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.973468 dlplan-0.1.15/src/policy/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      717 2022-11-13 08:50:15.000000 dlplan-0.1.15/src/policy/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1308 2023-03-27 11:58:50.000000 dlplan-0.1.15/src/policy/cache.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4074 2023-03-27 14:29:17.000000 dlplan-0.1.15/src/policy/condition.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2680 2023-03-27 14:29:17.000000 dlplan-0.1.15/src/policy/condition.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     6459 2023-03-27 14:29:17.000000 dlplan-0.1.15/src/policy/effect.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4101 2023-03-27 14:29:17.000000 dlplan-0.1.15/src/policy/effect.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.973468 dlplan-0.1.15/src/policy/parser/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4644 2023-03-27 14:29:17.000000 dlplan-0.1.15/src/policy/parser/expression_factory.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      930 2022-09-26 12:30:34.000000 dlplan-0.1.15/src/policy/parser/expression_factory.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    16349 2023-03-30 06:35:31.000000 dlplan-0.1.15/src/policy/parser/expressions.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2319 2023-03-30 06:35:31.000000 dlplan-0.1.15/src/policy/parser/parser.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      900 2022-09-26 12:30:34.000000 dlplan-0.1.15/src/policy/parser/parser.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      239 2022-09-26 12:30:34.000000 dlplan-0.1.15/src/policy/parser/types.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      474 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/policy/parser/utils.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      263 2022-09-26 12:30:34.000000 dlplan-0.1.15/src/policy/parser/utils.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     5361 2023-03-27 14:29:17.000000 dlplan-0.1.15/src/policy/policy.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     5621 2023-03-31 13:10:41.000000 dlplan-0.1.15/src/policy/policy_builder.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1913 2023-03-27 14:29:17.000000 dlplan-0.1.15/src/policy/policy_builder.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     5387 2023-04-21 20:46:03.000000 dlplan-0.1.15/src/policy/policy_impl.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    18803 2023-03-31 09:05:10.000000 dlplan-0.1.15/src/policy/policy_minimizer.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      324 2023-03-27 14:29:17.000000 dlplan-0.1.15/src/policy/reader.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      489 2023-03-27 14:29:17.000000 dlplan-0.1.15/src/policy/reader.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     4961 2023-03-31 09:03:45.000000 dlplan-0.1.15/src/policy/rule.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      188 2022-10-17 06:43:50.000000 dlplan-0.1.15/src/policy/writer.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      233 2022-10-17 06:43:50.000000 dlplan-0.1.15/src/policy/writer.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.973468 dlplan-0.1.15/src/state_space/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      591 2023-04-21 13:13:31.000000 dlplan-0.1.15/src/state_space/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      674 2023-04-04 14:37:29.000000 dlplan-0.1.15/src/state_space/generator.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      229 2023-04-04 14:37:24.000000 dlplan-0.1.15/src/state_space/generator.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     7246 2023-04-06 07:48:33.000000 dlplan-0.1.15/src/state_space/reader.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      261 2023-04-04 12:44:39.000000 dlplan-0.1.15/src/state_space/reader.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)    13425 2023-04-17 12:40:44.000000 dlplan-0.1.15/src/state_space/state_space.cpp
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.977469 dlplan-0.1.15/src/utils/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     8458 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/utils/MurmurHash3.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1108 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/utils/MurmurHash3.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      571 2022-11-11 15:13:54.000000 dlplan-0.1.15/src/utils/collections.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2049 2022-09-12 07:41:00.000000 dlplan-0.1.15/src/utils/command.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      735 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/utils/countdown_timer.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      449 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/utils/countdown_timer.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      143 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/utils/logging.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1765 2022-10-17 06:43:50.000000 dlplan-0.1.15/src/utils/logging.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      234 2022-10-20 12:35:57.000000 dlplan-0.1.15/src/utils/math.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      227 2022-10-20 12:35:57.000000 dlplan-0.1.15/src/utils/math.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      284 2022-09-12 07:41:00.000000 dlplan-0.1.15/src/utils/memory.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3238 2023-03-27 14:29:17.000000 dlplan-0.1.15/src/utils/set_operators.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     7310 2022-09-22 10:35:08.000000 dlplan-0.1.15/src/utils/sha-256.c
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      249 2022-09-22 10:35:08.000000 dlplan-0.1.15/src/utils/sha-256.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      789 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/utils/system.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      178 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/utils/system.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     9816 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/utils/threadpool.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1931 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/utils/timer.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      803 2022-09-07 06:24:55.000000 dlplan-0.1.15/src/utils/timer.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1529 2022-09-26 12:30:34.000000 dlplan-0.1.15/src/utils/tokenizer.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.977469 dlplan-0.1.15/src/weisfeiler_lehman/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      568 2022-09-12 07:41:00.000000 dlplan-0.1.15/src/weisfeiler_lehman/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      122 2023-03-30 06:34:28.000000 dlplan-0.1.15/src/weisfeiler_lehman/color.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      946 2023-03-30 06:34:28.000000 dlplan-0.1.15/src/weisfeiler_lehman/color.h
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2220 2022-09-12 07:41:00.000000 dlplan-0.1.15/src/weisfeiler_lehman/weisfeiler_lehman.cpp
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.977469 dlplan-0.1.15/tests/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      535 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/CMakeLists.txt
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.981469 dlplan-0.1.15/tests/core/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      958 2022-09-07 06:24:55.000000 dlplan-0.1.15/tests/core/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1799 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/core/b_empty.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1329 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/core/b_inclusion.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      891 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/core/b_nullary.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2585 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_all.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1170 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_and.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      931 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_bot.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1171 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_diff.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1700 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_equal.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1144 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_not.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      990 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_one_of.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1185 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_or.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1661 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_primitive.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2056 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_projection.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1338 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_some.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1673 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_subset.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      942 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/c_top.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2655 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/core/core.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2498 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/core/multi_instance.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2518 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/core/n_concept_distance.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1807 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/core/n_count.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2716 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/core/n_role_distance.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2865 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/core/n_sum_concept_distance.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3018 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/core/n_sum_role_distance.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1172 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_and.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1379 2023-03-30 13:34:01.000000 dlplan-0.1.15/tests/core/r_compose.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1177 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_diff.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      988 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_identity.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      986 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_inverse.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      938 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_not.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1222 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_or.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1736 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_primitive.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1113 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_restrict.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1002 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_top.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2035 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_transitive_closure.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2090 2023-03-30 13:33:40.000000 dlplan-0.1.15/tests/core/r_transitive_reflexive_closure.cpp
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.981469 dlplan-0.1.15/tests/generator/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)       27 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/generator/CMakeLists.txt
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.981469 dlplan-0.1.15/tests/generator/delivery/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      913 2023-03-20 09:44:19.000000 dlplan-0.1.15/tests/generator/delivery/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     8227 2023-04-06 08:01:18.000000 dlplan-0.1.15/tests/generator/delivery/delivery.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1271 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/generator/delivery/domain.pddl
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      749 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/generator/delivery/instance_2_2_0.pddl
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2061 2022-11-10 09:43:26.000000 dlplan-0.1.15/tests/generator/delivery/instance_4_2_29.pddl
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.981469 dlplan-0.1.15/tests/novelty/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      243 2022-10-17 06:43:50.000000 dlplan-0.1.15/tests/novelty/CMakeLists.txt
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.981469 dlplan-0.1.15/tests/novelty/gripper/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      645 2023-03-20 08:31:50.000000 dlplan-0.1.15/tests/novelty/gripper/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      926 2022-10-17 06:43:50.000000 dlplan-0.1.15/tests/novelty/gripper/domain.pddl
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      878 2023-04-06 08:00:24.000000 dlplan-0.1.15/tests/novelty/gripper/gripper.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      261 2022-10-17 06:43:50.000000 dlplan-0.1.15/tests/novelty/gripper/p-1-0.pddl
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     3306 2022-10-17 06:43:50.000000 dlplan-0.1.15/tests/novelty/tuple_index_generator.cpp
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.981469 dlplan-0.1.15/tests/policy/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      250 2022-09-07 06:24:55.000000 dlplan-0.1.15/tests/policy/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2430 2023-04-21 20:42:59.000000 dlplan-0.1.15/tests/policy/policy_builder.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     9811 2023-04-21 20:14:13.000000 dlplan-0.1.15/tests/policy/policy_minimizer.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     2075 2023-03-27 14:29:17.000000 dlplan-0.1.15/tests/policy/utils.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      507 2022-11-13 08:50:21.000000 dlplan-0.1.15/tests/policy/utils.h
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.981469 dlplan-0.1.15/tests/state_space/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)       52 2023-03-20 09:01:05.000000 dlplan-0.1.15/tests/state_space/CMakeLists.txt
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.981469 dlplan-0.1.15/tests/state_space/gripper/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      663 2023-03-20 09:50:25.000000 dlplan-0.1.15/tests/state_space/gripper/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      926 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/state_space/gripper/domain.pddl
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      476 2023-04-06 07:59:34.000000 dlplan-0.1.15/tests/state_space/gripper/gripper.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      261 2022-09-26 12:30:34.000000 dlplan-0.1.15/tests/state_space/gripper/p-1-0.pddl
-drwxrwxr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-21 20:48:41.981469 dlplan-0.1.15/tests/state_space/spanner/
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      668 2023-03-20 11:50:50.000000 dlplan-0.1.15/tests/state_space/spanner/CMakeLists.txt
--rw-rw-r--   0 dominik   (1000) dominik   (1000)     1374 2023-03-20 07:25:13.000000 dlplan-0.1.15/tests/state_space/spanner/domain.pddl
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      374 2023-03-20 07:25:13.000000 dlplan-0.1.15/tests/state_space/spanner/problem.pddl
--rw-rw-r--   0 dominik   (1000) dominik   (1000)      478 2023-04-06 08:50:59.000000 dlplan-0.1.15/tests/state_space/spanner/spanner.cpp
--rw-rw-r--   0 dominik   (1000) dominik   (1000)       72 2022-09-07 06:24:55.000000 dlplan-0.1.15/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.253500 dlplan-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-27 15:38:36.000000 dlplan-0.2.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-04-27 15:38:36.000000 dlplan-0.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-27 15:38:36.000000 dlplan-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 15:38:56.253500 dlplan-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-27 15:38:36.000000 dlplan-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.193500 dlplan-0.2.3/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.209500 dlplan-0.2.3/api/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.209500 dlplan-0.2.3/api/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/src/core.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.209500 dlplan-0.2.3/api/python/src/dlplan/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/src/dlplan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.209500 dlplan-0.2.3/api/python/src/dlplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 15:38:56.000000 dlplan-0.2.3/api/python/src/dlplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-04-27 15:38:56.000000 dlplan-0.2.3/api/python/src/dlplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:38:56.000000 dlplan-0.2.3/api/python/src/dlplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:38:56.000000 dlplan-0.2.3/api/python/src/dlplan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 15:38:56.000000 dlplan-0.2.3/api/python/src/dlplan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 15:38:56.000000 dlplan-0.2.3/api/python/src/dlplan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/src/generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/src/novelty.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/src/policy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/src/state_space.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/src/weisfeiler_lehman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.209500 dlplan-0.2.3/api/python/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/test/test_barman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-27 15:38:36.000000 dlplan-0.2.3/api/python/test/test_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.209500 dlplan-0.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.209500 dlplan-0.2.3/examples/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/core/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.209500 dlplan-0.2.3/examples/core/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/core/__pycache__/tarski.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/core/__pycache__/tarski.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/core/core.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2438 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.209500 dlplan-0.2.3/examples/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/generator/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/generator/generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/generator/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.213500 dlplan-0.2.3/examples/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/policy/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/policy/policy.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/policy/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.213500 dlplan-0.2.3/examples/state_space/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/state_space/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.213500 dlplan-0.2.3/examples/state_space/delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/state_space/delivery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/state_space/delivery/delivery.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/state_space/delivery/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/state_space/delivery/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/state_space/delivery/instance_2_1_0.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-27 15:38:36.000000 dlplan-0.2.3/examples/state_space/delivery/instance_2_2_0.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.213500 dlplan-0.2.3/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-27 15:38:36.000000 dlplan-0.2.3/experiments/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-27 15:38:36.000000 dlplan-0.2.3/experiments/experiment_generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-27 15:38:36.000000 dlplan-0.2.3/experiments/experiment_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5147 2023-04-27 15:38:36.000000 dlplan-0.2.3/experiments/experiment_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-04-27 15:38:36.000000 dlplan-0.2.3/experiments/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.197500 dlplan-0.2.3/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.217500 dlplan-0.2.3/include/dlplan/
+-rw-r--r--   0 runner    (1001) docker     (123)    25657 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/novelty.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.217500 dlplan-0.2.3/include/dlplan/phmap/
+-rw-r--r--   0 runner    (1001) docker     (123)   166554 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/phmap/btree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/phmap/meminfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)   186642 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/phmap/phmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)   180847 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/phmap/phmap_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22491 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/phmap/phmap_bits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28525 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/phmap/phmap_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/phmap/phmap_dump.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/phmap/phmap_fwd_decl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/phmap/phmap_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/policy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/state_space.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.221500 dlplan-0.2.3/include/dlplan/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/utils/cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/utils/dynamic_bitset.h
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/utils/hashing.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/utils/pimpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-27 15:38:36.000000 dlplan-0.2.3/include/dlplan/weisfeiler_lehman.h
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-27 15:38:36.000000 dlplan-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 15:38:36.000000 dlplan-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:38:56.253500 dlplan-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-27 15:38:36.000000 dlplan-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.221500 dlplan-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.221500 dlplan-0.2.3/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/atom.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/constant.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25107 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/core.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/element_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/element_factory.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.225500 dlplan-0.2.3/src/core/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/boolean.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.225500 dlplan-0.2.3/src/core/elements/booleans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/booleans/empty.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/booleans/inclusion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/booleans/nullary.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concept.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.229500 dlplan-0.2.3/src/core/elements/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/all.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/bot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/equal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/one_of.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/projection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/some.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/subset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/concepts/top.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/element.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/numerical.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.229500 dlplan-0.2.3/src/core/elements/numericals/
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/numericals/concept_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/numericals/count.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/numericals/role_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/numericals/sum_concept_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/numericals/sum_role_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/role.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.229500 dlplan-0.2.3/src/core/elements/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/compose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/identity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/restrict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/top.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/transitive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/roles/transitive_reflexive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/elements/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/instance_info.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/object.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.229500 dlplan-0.2.3/src/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expression_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expression_factory.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.229500 dlplan-0.2.3/src/core/parser/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/boolean.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.229500 dlplan-0.2.3/src/core/parser/expressions/booleans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/booleans/empty.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/booleans/inclusion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/booleans/nullary.h
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concept.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.233500 dlplan-0.2.3/src/core/parser/expressions/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/all.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/bot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/equal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/one_of.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/projection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/some.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/subset.h
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/concepts/top.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/expression.h
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/numerical.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.233500 dlplan-0.2.3/src/core/parser/expressions/numericals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/numericals/concept_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/numericals/count.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/numericals/role_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/numericals/sum_concept_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/numericals/sum_role_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/role.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.233500 dlplan-0.2.3/src/core/parser/expressions/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/compose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/identity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/restrict.h
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/top.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/transitive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/expressions/roles/transitive_reflexive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/parser/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/predicate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/core/vocabulary_info.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.233500 dlplan-0.2.3/src/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/feature_generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/feature_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/generator_data.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.233500 dlplan-0.2.3/src/generator/rules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.233500 dlplan-0.2.3/src/generator/rules/booleans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/booleans/empty.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/booleans/empty.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/booleans/inclusion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/booleans/inclusion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/booleans/nullary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/booleans/nullary.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.237500 dlplan-0.2.3/src/generator/rules/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/all.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/all.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/and.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/bot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/bot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/diff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/equal.h
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/not.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/one_of.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/one_of.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/or.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/primitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/projection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/projection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/some.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/some.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/subset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/subset.h
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/top.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/concepts/top.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.237500 dlplan-0.2.3/src/generator/rules/numericals/
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/numericals/concept_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/numericals/concept_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/numericals/count.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/numericals/count.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.241500 dlplan-0.2.3/src/generator/rules/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/and.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/compose.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/compose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/diff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/identity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/identity.h
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/inverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/not.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/or.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/primitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/restrict.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/restrict.h
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/top.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/top.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/transitive_closure.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/transitive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/transitive_reflexive_closure.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/roles/transitive_reflexive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/generator/rules/rule.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.241500 dlplan-0.2.3/src/novelty/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/novelty/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/novelty/novelty.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/novelty/novelty_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/novelty/novelty_table.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/novelty/tuple_graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/novelty/tuple_index_generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/novelty/tuple_node.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.241500 dlplan-0.2.3/src/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/condition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/condition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/effect.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/effect.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.241500 dlplan-0.2.3/src/policy/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/parser/expression_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/parser/expression_factory.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16349 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/parser/expressions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/parser/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/parser/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/parser/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/parser/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/parser/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/policy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/policy_builder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/policy_builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/policy_impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/policy_minimizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/policy/writer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.245500 dlplan-0.2.3/src/state_space/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/state_space/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/state_space/generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/state_space/generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/state_space/reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/state_space/reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/state_space/state_space.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.245500 dlplan-0.2.3/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/MurmurHash3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/MurmurHash3.h
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/collections.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/command.h
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/countdown_timer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/countdown_timer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/math.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/math.h
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/set_operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/sha-256.c
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/sha-256.h
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/system.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/system.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/threadpool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/timer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/timer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/utils/tokenizer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.245500 dlplan-0.2.3/src/weisfeiler_lehman/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/weisfeiler_lehman/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/weisfeiler_lehman/color.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/weisfeiler_lehman/color.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-27 15:38:36.000000 dlplan-0.2.3/src/weisfeiler_lehman/weisfeiler_lehman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.245500 dlplan-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.249500 dlplan-0.2.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/b_empty.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/b_inclusion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/b_nullary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_all.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_and.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_bot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_diff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_not.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_one_of.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_or.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_primitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_projection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_some.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_subset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/c_top.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/core.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/multi_instance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/n_concept_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/n_count.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/n_role_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/n_sum_concept_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/n_sum_role_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_and.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_compose.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_diff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_identity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_inverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_not.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_or.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_primitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_restrict.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_top.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_transitive_closure.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/core/r_transitive_reflexive_closure.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.249500 dlplan-0.2.3/tests/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/generator/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.249500 dlplan-0.2.3/tests/generator/delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/generator/delivery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/generator/delivery/delivery.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/generator/delivery/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/generator/delivery/instance_2_2_0.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/generator/delivery/instance_4_2_29.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.249500 dlplan-0.2.3/tests/novelty/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/novelty/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.249500 dlplan-0.2.3/tests/novelty/gripper/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/novelty/gripper/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/novelty/gripper/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/novelty/gripper/gripper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/novelty/gripper/p-1-0.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/novelty/tuple_index_generator.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.249500 dlplan-0.2.3/tests/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/policy/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/policy/policy_builder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/policy/policy_minimizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/policy/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/policy/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.249500 dlplan-0.2.3/tests/state_space/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/state_space/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.253500 dlplan-0.2.3/tests/state_space/gripper/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/state_space/gripper/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/state_space/gripper/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/state_space/gripper/gripper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/state_space/gripper/p-1-0.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:56.253500 dlplan-0.2.3/tests/state_space/spanner/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/state_space/spanner/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/state_space/spanner/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/state_space/spanner/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-27 15:38:36.000000 dlplan-0.2.3/tests/state_space/spanner/spanner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 15:38:36.000000 dlplan-0.2.3/tox.ini
```

### Comparing `dlplan-0.1.15/CMakeLists.txt` & `dlplan-0.2.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/LICENSE.md` & `dlplan-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/README.md` & `dlplan-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/api/python/CMakeLists.txt` & `dlplan-0.2.3/api/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/api/python/src/core.cpp` & `dlplan-0.2.3/api/python/src/core.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/api/python/src/dlplan.egg-info/SOURCES.txt` & `dlplan-0.2.3/api/python/src/dlplan.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,14 @@
 api/python/src/dlplan.egg-info/not-zip-safe
 api/python/src/dlplan.egg-info/requires.txt
 api/python/src/dlplan.egg-info/top_level.txt
 api/python/test/__init__.py
 api/python/test/test_barman.py
 api/python/test/test_core.py
 api/python/test/test_generate.py
-api/python/test/__pycache__/__init__.cpython-38.pyc
-api/python/test/__pycache__/test_barman.cpython-38-pytest-6.2.5.pyc
-api/python/test/__pycache__/test_core.cpython-38-pytest-6.2.5.pyc
-api/python/test/__pycache__/test_generate.cpython-38-pytest-6.2.5.pyc
 examples/CMakeLists.txt
 examples/core/CMakeLists.txt
 examples/core/core.cpp
 examples/core/core.py
 examples/core/__pycache__/tarski.cpython-36.pyc
 examples/core/__pycache__/tarski.cpython-37.pyc
 examples/generator/CMakeLists.txt
@@ -45,21 +41,17 @@
 examples/state_space/delivery/CMakeLists.txt
 examples/state_space/delivery/delivery.cpp
 examples/state_space/delivery/delivery.py
 examples/state_space/delivery/domain.pddl
 examples/state_space/delivery/instance_2_1_0.pddl
 examples/state_space/delivery/instance_2_2_0.pddl
 experiments/CMakeLists.txt
-experiments/domain.pddl
-experiments/experiment_generator
 experiments/experiment_generator.cpp
 experiments/experiment_parser.py
 experiments/experiment_runner.py
-experiments/instance_large.pddl
-experiments/instance_small.pddl
 experiments/main.py
 include/dlplan/core.h
 include/dlplan/generator.h
 include/dlplan/novelty.h
 include/dlplan/policy.h
 include/dlplan/state_space.h
 include/dlplan/weisfeiler_lehman.h
```

### Comparing `dlplan-0.1.15/api/python/src/generator.cpp` & `dlplan-0.2.3/api/python/src/generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/api/python/src/main.cpp` & `dlplan-0.2.3/api/python/src/main.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/api/python/src/novelty.cpp` & `dlplan-0.2.3/api/python/src/novelty.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/api/python/src/policy.cpp` & `dlplan-0.2.3/api/python/src/policy.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/api/python/src/weisfeiler_lehman.cpp` & `dlplan-0.2.3/api/python/src/weisfeiler_lehman.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/api/python/test/test_barman.py` & `dlplan-0.2.3/api/python/test/test_barman.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/api/python/test/test_core.py` & `dlplan-0.2.3/api/python/test/test_core.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/api/python/test/test_generate.py` & `dlplan-0.2.3/api/python/test/test_generate.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/core/__pycache__/tarski.cpython-36.pyc` & `dlplan-0.2.3/examples/core/__pycache__/tarski.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/core/__pycache__/tarski.cpython-37.pyc` & `dlplan-0.2.3/examples/core/__pycache__/tarski.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/core/core.cpp` & `dlplan-0.2.3/examples/core/core.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/core/core.py` & `dlplan-0.2.3/examples/core/core.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/generator/generator.cpp` & `dlplan-0.2.3/examples/generator/generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/generator/generator.py` & `dlplan-0.2.3/examples/generator/generator.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/policy/policy.cpp` & `dlplan-0.2.3/examples/policy/policy.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/policy/policy.py` & `dlplan-0.2.3/examples/policy/policy.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/state_space/delivery/CMakeLists.txt` & `dlplan-0.2.3/examples/state_space/delivery/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/state_space/delivery/delivery.cpp` & `dlplan-0.2.3/examples/state_space/delivery/delivery.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/state_space/delivery/delivery.py` & `dlplan-0.2.3/examples/state_space/delivery/delivery.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/state_space/delivery/domain.pddl` & `dlplan-0.2.3/examples/state_space/delivery/domain.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/state_space/delivery/instance_2_1_0.pddl` & `dlplan-0.2.3/examples/state_space/delivery/instance_2_1_0.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/examples/state_space/delivery/instance_2_2_0.pddl` & `dlplan-0.2.3/examples/state_space/delivery/instance_2_2_0.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/experiments/domain.pddl` & `dlplan-0.2.3/tests/generator/delivery/domain.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/experiments/experiment_generator.cpp` & `dlplan-0.2.3/experiments/experiment_generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/experiments/experiment_parser.py` & `dlplan-0.2.3/experiments/experiment_parser.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/experiments/experiment_runner.py` & `dlplan-0.2.3/experiments/experiment_runner.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/experiments/instance_large.pddl` & `dlplan-0.2.3/tests/generator/delivery/instance_4_2_29.pddl`

 * *Files 1% similar despite different names*

```diff
@@ -1,80 +1,79 @@
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;;; Instance file automatically generated by the Tarski FSTRIPS writer
 ;;; 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 
-(define (problem delivery-4x4-3)
+(define (problem delivery-4x4-2)
     (:domain delivery)
 
     (:objects
         c_0_0 c_0_1 c_0_2 c_0_3 c_1_0 c_1_1 c_1_2 c_1_3 c_2_0 c_2_1 c_2_2 c_2_3 c_3_0 c_3_1 c_3_2 c_3_3 - cell
-        p1 p2 p3 - package
+        p1 p2 - package
         t1 - truck
     )
 
     (:init
+        (adjacent c_0_0 c_0_1)
+        (adjacent c_2_1 c_3_1)
+        (adjacent c_0_2 c_0_1)
+        (adjacent c_3_3 c_3_2)
+        (adjacent c_0_1 c_0_0)
         (adjacent c_0_2 c_1_2)
-        (adjacent c_1_0 c_0_0)
-        (adjacent c_2_3 c_1_3)
-        (adjacent c_2_3 c_3_3)
-        (adjacent c_3_2 c_3_3)
-        (adjacent c_3_1 c_3_2)
-        (adjacent c_3_0 c_3_1)
-        (adjacent c_1_3 c_0_3)
-        (adjacent c_3_2 c_3_1)
+        (adjacent c_3_1 c_3_0)
         (adjacent c_2_2 c_1_2)
+        (adjacent c_3_0 c_3_1)
         (adjacent c_0_1 c_1_1)
-        (adjacent c_2_0 c_3_0)
-        (adjacent c_2_1 c_2_0)
         (adjacent c_1_3 c_1_2)
-        (adjacent c_1_2 c_1_1)
-        (adjacent c_1_2 c_1_3)
-        (adjacent c_2_0 c_1_0)
-        (adjacent c_2_2 c_2_3)
-        (adjacent c_1_1 c_0_1)
-        (adjacent c_2_0 c_2_1)
-        (adjacent c_0_0 c_1_0)
-        (adjacent c_2_1 c_1_1)
-        (adjacent c_1_3 c_2_3)
-        (adjacent c_3_3 c_2_3)
+        (adjacent c_2_3 c_1_3)
+        (adjacent c_3_1 c_2_1)
         (adjacent c_2_2 c_2_1)
-        (adjacent c_2_1 c_3_1)
-        (adjacent c_1_0 c_2_0)
-        (adjacent c_3_1 c_3_0)
-        (adjacent c_1_1 c_1_2)
-        (adjacent c_0_3 c_0_2)
-        (adjacent c_2_3 c_2_2)
-        (adjacent c_1_0 c_1_1)
+        (adjacent c_1_1 c_2_1)
+        (adjacent c_0_3 c_1_3)
         (adjacent c_3_2 c_2_2)
-        (adjacent c_3_1 c_2_1)
-        (adjacent c_0_1 c_0_0)
         (adjacent c_1_1 c_1_0)
-        (adjacent c_1_1 c_2_1)
+        (adjacent c_1_1 c_0_1)
+        (adjacent c_0_2 c_0_3)
+        (adjacent c_2_1 c_1_1)
+        (adjacent c_3_2 c_3_3)
         (adjacent c_1_2 c_2_2)
+        (adjacent c_0_3 c_0_2)
+        (adjacent c_2_3 c_2_2)
+        (adjacent c_1_2 c_1_1)
+        (adjacent c_3_3 c_2_3)
         (adjacent c_2_1 c_2_2)
-        (adjacent c_0_2 c_0_1)
         (adjacent c_2_2 c_3_2)
+        (adjacent c_3_1 c_3_2)
         (adjacent c_0_1 c_0_2)
+        (adjacent c_1_3 c_0_3)
+        (adjacent c_3_2 c_3_1)
+        (adjacent c_1_0 c_1_1)
+        (adjacent c_1_0 c_2_0)
+        (adjacent c_2_3 c_3_3)
+        (adjacent c_1_3 c_2_3)
+        (adjacent c_1_2 c_1_3)
+        (adjacent c_1_1 c_1_2)
+        (adjacent c_0_0 c_1_0)
+        (adjacent c_1_0 c_0_0)
         (adjacent c_3_0 c_2_0)
-        (adjacent c_0_3 c_1_3)
+        (adjacent c_2_0 c_1_0)
+        (adjacent c_2_0 c_2_1)
+        (adjacent c_2_1 c_2_0)
         (adjacent c_1_2 c_0_2)
-        (adjacent c_3_3 c_3_2)
-        (adjacent c_0_2 c_0_3)
-        (adjacent c_0_0 c_0_1)
-        (at p1 c_1_2)
-        (at p2 c_3_2)
-        (at p3 c_1_1)
-        (at t1 c_2_0)
+        (adjacent c_2_2 c_2_3)
+        (adjacent c_2_0 c_3_0)
+        (at t1 c_3_1)
+        (at p1 c_1_3)
+        (at p2 c_1_2)
         (empty t1)
     )
 
     (:goal
-        (and (at p1 c_0_0) (at p2 c_0_0) (at p3 c_0_0))
+        (and (at p1 c_1_1) (at p2 c_1_1))
     )
 
     
     
     
 )
```

### Comparing `dlplan-0.1.15/experiments/instance_small.pddl` & `dlplan-0.2.3/tests/generator/delivery/instance_2_2_0.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/experiments/main.py` & `dlplan-0.2.3/experiments/main.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/core.h` & `dlplan-0.2.3/include/dlplan/core.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/generator.h` & `dlplan-0.2.3/include/dlplan/generator.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/novelty.h` & `dlplan-0.2.3/include/dlplan/novelty.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/phmap/btree.h` & `dlplan-0.2.3/include/dlplan/phmap/btree.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/phmap/meminfo.h` & `dlplan-0.2.3/include/dlplan/phmap/meminfo.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/phmap/phmap.h` & `dlplan-0.2.3/include/dlplan/phmap/phmap.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/phmap/phmap_base.h` & `dlplan-0.2.3/include/dlplan/phmap/phmap_base.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/phmap/phmap_bits.h` & `dlplan-0.2.3/include/dlplan/phmap/phmap_bits.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/phmap/phmap_config.h` & `dlplan-0.2.3/include/dlplan/phmap/phmap_config.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/phmap/phmap_dump.h` & `dlplan-0.2.3/include/dlplan/phmap/phmap_dump.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/phmap/phmap_fwd_decl.h` & `dlplan-0.2.3/include/dlplan/phmap/phmap_fwd_decl.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/phmap/phmap_utils.h` & `dlplan-0.2.3/include/dlplan/phmap/phmap_utils.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/policy.h` & `dlplan-0.2.3/include/dlplan/policy.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/state_space.h` & `dlplan-0.2.3/include/dlplan/state_space.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/utils/cache.h` & `dlplan-0.2.3/include/dlplan/utils/cache.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/utils/dynamic_bitset.h` & `dlplan-0.2.3/include/dlplan/utils/dynamic_bitset.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/utils/pimpl.h` & `dlplan-0.2.3/include/dlplan/utils/pimpl.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/include/dlplan/weisfeiler_lehman.h` & `dlplan-0.2.3/include/dlplan/weisfeiler_lehman.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/setup.py` & `dlplan-0.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import subprocess
 from pathlib import Path
 
 from setuptools import setup, Extension, find_packages
 from setuptools.command.build_ext import build_ext
 
-__version__ = "0.1.15"
+__version__ = "0.2.3"
 HERE = Path(__file__).resolve().parent
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
@@ -56,15 +56,15 @@
     name="dlplan",
     version=__version__,
     author="Dominik Drexler, Jendrik Seipp and Guillem Francès",
     author_email="dominik.drexler@liu.se",
     url="https://github.com/rleap-project/dlplan",
     description="A library for using description logics features in planning",
     long_description="",
-    install_requires=["pybind11", "pybind11-global", "state_space_generator"],
+    install_requires=["pybind11", "pybind11-global"],
     packages=['dlplan'],
     package_dir={"": "api/python/src"},
     ext_modules=[CMakeExtension("_dlplan")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     extras_require={
         'test': [
```

### Comparing `dlplan-0.1.15/src/core/CMakeLists.txt` & `dlplan-0.2.3/src/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/atom.cpp` & `dlplan-0.2.3/src/core/atom.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/cache.h` & `dlplan-0.2.3/src/core/cache.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/constant.cpp` & `dlplan-0.2.3/src/core/constant.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/core.cpp` & `dlplan-0.2.3/src/core/core.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/element_factory.cpp` & `dlplan-0.2.3/src/core/element_factory.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/element_factory.h` & `dlplan-0.2.3/src/core/element_factory.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/boolean.h` & `dlplan-0.2.3/src/core/elements/boolean.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/booleans/empty.h` & `dlplan-0.2.3/src/core/elements/booleans/empty.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/booleans/inclusion.h` & `dlplan-0.2.3/src/core/elements/booleans/inclusion.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/booleans/nullary.h` & `dlplan-0.2.3/src/core/elements/booleans/nullary.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concept.h` & `dlplan-0.2.3/src/core/elements/concept.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/all.h` & `dlplan-0.2.3/src/core/elements/concepts/all.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/and.h` & `dlplan-0.2.3/src/core/elements/concepts/and.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/bot.h` & `dlplan-0.2.3/src/core/elements/concepts/bot.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/diff.h` & `dlplan-0.2.3/src/core/elements/concepts/diff.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/equal.h` & `dlplan-0.2.3/src/core/elements/concepts/equal.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/not.h` & `dlplan-0.2.3/src/core/elements/concepts/not.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/one_of.h` & `dlplan-0.2.3/src/core/elements/concepts/one_of.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/or.h` & `dlplan-0.2.3/src/core/elements/concepts/or.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/primitive.h` & `dlplan-0.2.3/src/core/elements/concepts/primitive.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/projection.h` & `dlplan-0.2.3/src/core/elements/concepts/projection.h`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 namespace dlplan::core::element {
 
 class ProjectionConcept : public Concept {
 private:
     void compute_result(const RoleDenotation& denot, ConceptDenotation& result) const {
-        for (const auto pair : denot) {
+        for (const auto& pair : denot) {
             if (m_pos == 0) result.insert(pair.first);
             else if (m_pos == 1) result.insert(pair.second);
         }
     }
 
     std::unique_ptr<ConceptDenotation> evaluate_impl(const State& state, DenotationsCaches& caches) const override {
         auto denotation = std::make_unique<ConceptDenotation>(
```

### Comparing `dlplan-0.1.15/src/core/elements/concepts/some.h` & `dlplan-0.2.3/src/core/elements/concepts/some.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/subset.h` & `dlplan-0.2.3/src/core/elements/concepts/subset.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/concepts/top.h` & `dlplan-0.2.3/src/core/elements/concepts/top.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/element.h` & `dlplan-0.2.3/src/core/elements/element.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/numerical.h` & `dlplan-0.2.3/src/core/elements/numerical.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/numericals/concept_distance.h` & `dlplan-0.2.3/src/core/elements/numericals/concept_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/numericals/count.h` & `dlplan-0.2.3/src/core/elements/numericals/count.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/numericals/role_distance.h` & `dlplan-0.2.3/src/core/elements/numericals/role_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/numericals/sum_concept_distance.h` & `dlplan-0.2.3/src/core/elements/numericals/sum_concept_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/numericals/sum_role_distance.h` & `dlplan-0.2.3/src/core/elements/numericals/sum_role_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/role.h` & `dlplan-0.2.3/src/core/elements/role.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/and.h` & `dlplan-0.2.3/src/core/elements/roles/and.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/compose.h` & `dlplan-0.2.3/src/core/elements/roles/compose.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/diff.h` & `dlplan-0.2.3/src/core/elements/roles/diff.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/identity.h` & `dlplan-0.2.3/src/core/elements/roles/identity.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/inverse.h` & `dlplan-0.2.3/src/core/elements/roles/inverse.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/not.h` & `dlplan-0.2.3/src/core/elements/roles/not.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/or.h` & `dlplan-0.2.3/src/core/elements/roles/or.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/primitive.h` & `dlplan-0.2.3/src/core/elements/roles/primitive.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/restrict.h` & `dlplan-0.2.3/src/core/elements/roles/restrict.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/top.h` & `dlplan-0.2.3/src/core/elements/roles/top.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/roles/transitive_closure.h` & `dlplan-0.2.3/src/core/elements/roles/transitive_closure.h`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 class TransitiveClosureRole : public Role {
 private:
     void compute_result(const RoleDenotation& denot, RoleDenotation& result) const {
         result = denot;
         bool changed = false;
         do {
             RoleDenotation tmp_result = result;
-            for (const auto pair_1 : tmp_result) {
-                for (const auto pair_2 : tmp_result) {
+            for (const auto& pair_1 : tmp_result) {
+                for (const auto& pair_2 : tmp_result) {
                     if (pair_1.second == pair_2.first) {
                         result.insert(std::make_pair(pair_1.first, pair_2.second));
                     }
                 }
             }
             changed = (result.size() != tmp_result.size());
         } while (changed);
```

### Comparing `dlplan-0.1.15/src/core/elements/roles/transitive_reflexive_closure.h` & `dlplan-0.2.3/src/core/elements/roles/transitive_reflexive_closure.h`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 class TransitiveReflexiveClosureRole : public Role {
 private:
     void compute_result(const RoleDenotation& denot, int num_objects, RoleDenotation& result) const {
         result = denot;
         bool changed = false;
         do {
             RoleDenotation tmp_result = result;
-            for (const auto pair_1 : tmp_result) {
-                for (const auto pair_2 : tmp_result) {
+            for (const auto& pair_1 : tmp_result) {
+                for (const auto& pair_2 : tmp_result) {
                     if (pair_1.second == pair_2.first) {
                         result.insert(std::make_pair(pair_1.first, pair_2.second));
                     }
                 }
             }
             changed = (result.size() != tmp_result.size());
         } while (changed);
```

### Comparing `dlplan-0.1.15/src/core/elements/utils.cpp` & `dlplan-0.2.3/src/core/elements/utils.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/elements/utils.h` & `dlplan-0.2.3/src/core/elements/utils.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/instance_info.cpp` & `dlplan-0.2.3/src/core/instance_info.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/object.cpp` & `dlplan-0.2.3/src/core/object.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expression_factory.cpp` & `dlplan-0.2.3/src/core/parser/expression_factory.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/boolean.h` & `dlplan-0.2.3/src/core/parser/expressions/boolean.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/booleans/empty.h` & `dlplan-0.2.3/src/core/parser/expressions/booleans/empty.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/booleans/inclusion.h` & `dlplan-0.2.3/src/core/parser/expressions/booleans/inclusion.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/booleans/nullary.h` & `dlplan-0.2.3/src/core/parser/expressions/booleans/nullary.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concept.h` & `dlplan-0.2.3/src/core/parser/expressions/concept.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/all.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/all.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/and.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/and.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/bot.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/bot.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/diff.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/diff.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/equal.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/equal.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/not.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/not.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/one_of.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/one_of.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/or.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/or.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/primitive.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/primitive.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/projection.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/projection.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/some.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/some.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/subset.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/subset.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/concepts/top.h` & `dlplan-0.2.3/src/core/parser/expressions/concepts/top.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/expression.h` & `dlplan-0.2.3/src/core/parser/expressions/expression.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/numerical.h` & `dlplan-0.2.3/src/core/parser/expressions/numerical.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/numericals/concept_distance.h` & `dlplan-0.2.3/src/core/parser/expressions/numericals/concept_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/numericals/count.h` & `dlplan-0.2.3/src/core/parser/expressions/numericals/count.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/numericals/role_distance.h` & `dlplan-0.2.3/src/core/parser/expressions/numericals/role_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/numericals/sum_concept_distance.h` & `dlplan-0.2.3/src/core/parser/expressions/numericals/sum_concept_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/numericals/sum_role_distance.h` & `dlplan-0.2.3/src/core/parser/expressions/numericals/sum_role_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/role.h` & `dlplan-0.2.3/src/core/parser/expressions/role.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/and.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/and.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/compose.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/compose.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/diff.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/diff.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/identity.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/identity.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/inverse.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/inverse.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/not.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/not.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/or.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/or.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/primitive.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/primitive.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/restrict.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/restrict.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/top.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/top.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/transitive_closure.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/transitive_closure.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/expressions/roles/transitive_reflexive_closure.h` & `dlplan-0.2.3/src/core/parser/expressions/roles/transitive_reflexive_closure.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/parser.cpp` & `dlplan-0.2.3/src/core/parser/parser.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/parser.h` & `dlplan-0.2.3/src/core/parser/parser.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/parser/utils.h` & `dlplan-0.2.3/src/core/parser/utils.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/predicate.cpp` & `dlplan-0.2.3/src/core/predicate.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/state.cpp` & `dlplan-0.2.3/src/core/state.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/core/vocabulary_info.cpp` & `dlplan-0.2.3/src/core/vocabulary_info.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/CMakeLists.txt` & `dlplan-0.2.3/src/generator/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/feature_generator.cpp` & `dlplan-0.2.3/src/generator/feature_generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/feature_generator.h` & `dlplan-0.2.3/src/generator/feature_generator.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/generator.cpp` & `dlplan-0.2.3/src/generator/generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/generator_data.h` & `dlplan-0.2.3/src/generator/generator_data.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/booleans/empty.cpp` & `dlplan-0.2.3/src/generator/rules/booleans/empty.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/booleans/inclusion.cpp` & `dlplan-0.2.3/src/generator/rules/booleans/inclusion.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/booleans/nullary.cpp` & `dlplan-0.2.3/src/generator/rules/booleans/nullary.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/all.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/all.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/and.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/and.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/bot.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/bot.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/diff.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/diff.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/equal.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/equal.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/not.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/not.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/one_of.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/one_of.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/or.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/or.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/primitive.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/primitive.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/projection.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/projection.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/some.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/some.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/subset.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/subset.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/concepts/top.cpp` & `dlplan-0.2.3/src/generator/rules/concepts/top.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/numericals/concept_distance.cpp` & `dlplan-0.2.3/src/generator/rules/numericals/concept_distance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/numericals/count.cpp` & `dlplan-0.2.3/src/generator/rules/numericals/count.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/and.cpp` & `dlplan-0.2.3/src/generator/rules/roles/and.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/compose.cpp` & `dlplan-0.2.3/src/generator/rules/roles/compose.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/diff.cpp` & `dlplan-0.2.3/src/generator/rules/roles/diff.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/identity.cpp` & `dlplan-0.2.3/src/generator/rules/roles/identity.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/inverse.cpp` & `dlplan-0.2.3/src/generator/rules/roles/inverse.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/not.cpp` & `dlplan-0.2.3/src/generator/rules/roles/not.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/or.cpp` & `dlplan-0.2.3/src/generator/rules/roles/or.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/primitive.cpp` & `dlplan-0.2.3/src/generator/rules/roles/primitive.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/restrict.cpp` & `dlplan-0.2.3/src/generator/rules/roles/restrict.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/top.cpp` & `dlplan-0.2.3/src/generator/rules/roles/top.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/transitive_closure.cpp` & `dlplan-0.2.3/src/generator/rules/roles/transitive_closure.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/roles/transitive_reflexive_closure.cpp` & `dlplan-0.2.3/src/generator/rules/roles/transitive_reflexive_closure.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/generator/rules/rule.h` & `dlplan-0.2.3/src/generator/rules/rule.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/novelty/CMakeLists.txt` & `dlplan-0.2.3/src/novelty/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/novelty/novelty_base.cpp` & `dlplan-0.2.3/src/novelty/novelty_base.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/novelty/novelty_table.cpp` & `dlplan-0.2.3/src/novelty/novelty_table.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/novelty/tuple_graph.cpp` & `dlplan-0.2.3/src/novelty/tuple_graph.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/novelty/tuple_index_generator.cpp` & `dlplan-0.2.3/src/novelty/tuple_index_generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/novelty/tuple_node.cpp` & `dlplan-0.2.3/src/novelty/tuple_node.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/CMakeLists.txt` & `dlplan-0.2.3/src/policy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/cache.h` & `dlplan-0.2.3/src/policy/cache.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/condition.cpp` & `dlplan-0.2.3/src/policy/condition.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/condition.h` & `dlplan-0.2.3/src/policy/condition.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/effect.cpp` & `dlplan-0.2.3/src/policy/effect.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/effect.h` & `dlplan-0.2.3/src/policy/effect.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/parser/expression_factory.cpp` & `dlplan-0.2.3/src/policy/parser/expression_factory.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/parser/expression_factory.h` & `dlplan-0.2.3/src/policy/parser/expression_factory.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/parser/expressions.h` & `dlplan-0.2.3/src/policy/parser/expressions.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/parser/parser.cpp` & `dlplan-0.2.3/src/policy/parser/parser.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/parser/parser.h` & `dlplan-0.2.3/src/policy/parser/parser.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/policy.cpp` & `dlplan-0.2.3/src/policy/policy.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/policy_builder.cpp` & `dlplan-0.2.3/src/policy/policy_builder.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/policy_builder.h` & `dlplan-0.2.3/src/policy/policy_builder.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/policy_impl.cpp` & `dlplan-0.2.3/src/policy/policy_impl.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -106,24 +106,24 @@
     copy_to_builder(builder);
     const auto booleans = builder.get_booleans();
     std::vector<std::shared_ptr<const core::Boolean>> sorted_booleans(booleans.begin(), booleans.end());
     std::sort(sorted_booleans.begin(), sorted_booleans.end(), [](const auto& b1, const auto& b2){ return b1->get_index() < b2->get_index(); });
     ss << "(:boolean_features ";
     for (const auto& boolean : sorted_booleans) {
         ss << "\"" << boolean->compute_repr() << "\"";
-        if (boolean != *booleans.rbegin()) ss << " ";
+        if (boolean != *sorted_booleans.rbegin()) ss << " ";
     }
     ss << ")\n";
     const auto numericals = builder.get_numericals();
     std::vector<std::shared_ptr<const core::Numerical>> sorted_numericals(numericals.begin(), numericals.end());
     std::sort(sorted_numericals.begin(), sorted_numericals.end(), [](const auto& n1, const auto& n2){ return n1->get_index() < n2->get_index(); });
     ss << "(:numerical_features ";
     for (const auto& numerical : sorted_numericals) {
         ss << "\"" << numerical->compute_repr() << "\"";
-        if (numerical != *numericals.rbegin()) ss << " ";
+        if (numerical != *sorted_numericals.rbegin()) ss << " ";
     }
     ss << ")\n";
     const auto rules = builder.get_result().get_rules();
     std::vector<std::shared_ptr<const Rule>> sorted_rules(rules.begin(), rules.end());
     std::sort(sorted_rules.begin(), sorted_rules.end(), [](const auto& r1, const auto& r2){ return r1->compute_repr() < r2->compute_repr(); });
     for (const auto& r : sorted_rules) {
         ss << r->str() << "\n";
```

### Comparing `dlplan-0.1.15/src/policy/policy_minimizer.cpp` & `dlplan-0.2.3/src/policy/policy_minimizer.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/policy/rule.cpp` & `dlplan-0.2.3/src/policy/rule.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/state_space/CMakeLists.txt` & `dlplan-0.2.3/src/state_space/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-find_package(pybind11 REQUIRED)
-
 add_library(dlplanstatespace SHARED)
 target_sources(dlplanstatespace
     PRIVATE
         generator.cpp
         reader.cpp
         state_space.cpp)
 
-target_link_libraries(dlplanstatespace dlplancore pybind11::embed)
+target_link_libraries(dlplanstatespace dlplancore)
 target_include_directories(dlplanstatespace
     PUBLIC
         ${PROJECT_SOURCE_DIR}/include
 )
 
 install(
     TARGETS
```

### Comparing `dlplan-0.1.15/src/state_space/generator.cpp` & `dlplan-0.2.3/src/state_space/generator.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,19 @@
 #include <iostream>
 #include <fstream>
 #include <sstream>
 #include <iostream>
 
 #include "../utils/command.h"
 
-#include <pybind11/embed.h> // everything needed for embedding
-namespace py = pybind11;
-
-
 using namespace dlplan::core;
 using namespace std::string_literals;
 
 namespace dlplan::state_space::generator {
 
 void generate_state_space_files(const std::string& domain_file,
     const std::string& instance_file) {
-    py::scoped_interpreter guard{};
-    py::module_ state_space_generator = py::module_::import("state_space_generator.state_space_generator");
-    state_space_generator.attr("generate_state_space")(domain_file, instance_file);
+    utils::Command::exec(
+        "python3 -c \"import state_space_generator.state_space_generator; state_space_generator.state_space_generator.generate_state_space(\\\"" + domain_file + "\\\", \\\"" + instance_file + "\\\")\"");
 }
 
 }
```

### Comparing `dlplan-0.1.15/src/state_space/reader.cpp` & `dlplan-0.2.3/src/state_space/reader.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/state_space/state_space.cpp` & `dlplan-0.2.3/src/state_space/state_space.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/MurmurHash3.cpp` & `dlplan-0.2.3/src/utils/MurmurHash3.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/MurmurHash3.h` & `dlplan-0.2.3/src/utils/MurmurHash3.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/collections.h` & `dlplan-0.2.3/src/utils/collections.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/command.h` & `dlplan-0.2.3/src/utils/command.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/countdown_timer.cpp` & `dlplan-0.2.3/src/utils/countdown_timer.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/logging.h` & `dlplan-0.2.3/src/utils/logging.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/set_operators.h` & `dlplan-0.2.3/src/utils/set_operators.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/sha-256.c` & `dlplan-0.2.3/src/utils/sha-256.c`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/system.cpp` & `dlplan-0.2.3/src/utils/system.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/threadpool.h` & `dlplan-0.2.3/src/utils/threadpool.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/timer.cpp` & `dlplan-0.2.3/src/utils/timer.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/timer.h` & `dlplan-0.2.3/src/utils/timer.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/utils/tokenizer.h` & `dlplan-0.2.3/src/utils/tokenizer.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/weisfeiler_lehman/CMakeLists.txt` & `dlplan-0.2.3/src/weisfeiler_lehman/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/weisfeiler_lehman/color.h` & `dlplan-0.2.3/src/weisfeiler_lehman/color.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/src/weisfeiler_lehman/weisfeiler_lehman.cpp` & `dlplan-0.2.3/src/weisfeiler_lehman/weisfeiler_lehman.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/CMakeLists.txt` & `dlplan-0.2.3/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/CMakeLists.txt` & `dlplan-0.2.3/tests/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/b_empty.cpp` & `dlplan-0.2.3/tests/core/b_empty.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/b_inclusion.cpp` & `dlplan-0.2.3/tests/core/b_inclusion.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/b_nullary.cpp` & `dlplan-0.2.3/tests/core/b_nullary.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_all.cpp` & `dlplan-0.2.3/tests/core/c_all.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_and.cpp` & `dlplan-0.2.3/tests/core/c_and.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_bot.cpp` & `dlplan-0.2.3/tests/core/c_bot.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_diff.cpp` & `dlplan-0.2.3/tests/core/c_diff.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_equal.cpp` & `dlplan-0.2.3/tests/core/c_equal.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_not.cpp` & `dlplan-0.2.3/tests/core/c_not.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_one_of.cpp` & `dlplan-0.2.3/tests/core/c_one_of.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_or.cpp` & `dlplan-0.2.3/tests/core/c_or.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_primitive.cpp` & `dlplan-0.2.3/tests/core/c_primitive.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_projection.cpp` & `dlplan-0.2.3/tests/core/c_projection.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_some.cpp` & `dlplan-0.2.3/tests/core/c_some.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_subset.cpp` & `dlplan-0.2.3/tests/core/c_subset.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/c_top.cpp` & `dlplan-0.2.3/tests/core/c_top.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/core.cpp` & `dlplan-0.2.3/tests/core/core.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/multi_instance.cpp` & `dlplan-0.2.3/tests/core/multi_instance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/n_concept_distance.cpp` & `dlplan-0.2.3/tests/core/n_concept_distance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/n_count.cpp` & `dlplan-0.2.3/tests/core/n_count.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/n_role_distance.cpp` & `dlplan-0.2.3/tests/core/n_role_distance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/n_sum_concept_distance.cpp` & `dlplan-0.2.3/tests/core/n_sum_concept_distance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/n_sum_role_distance.cpp` & `dlplan-0.2.3/tests/core/n_sum_role_distance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_and.cpp` & `dlplan-0.2.3/tests/core/r_and.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_compose.cpp` & `dlplan-0.2.3/tests/core/r_compose.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_diff.cpp` & `dlplan-0.2.3/tests/core/r_diff.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_identity.cpp` & `dlplan-0.2.3/tests/core/r_identity.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_inverse.cpp` & `dlplan-0.2.3/tests/core/r_inverse.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_not.cpp` & `dlplan-0.2.3/tests/core/r_not.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_or.cpp` & `dlplan-0.2.3/tests/core/r_or.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_primitive.cpp` & `dlplan-0.2.3/tests/core/r_primitive.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_restrict.cpp` & `dlplan-0.2.3/tests/core/r_restrict.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_top.cpp` & `dlplan-0.2.3/tests/core/r_top.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_transitive_closure.cpp` & `dlplan-0.2.3/tests/core/r_transitive_closure.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/core/r_transitive_reflexive_closure.cpp` & `dlplan-0.2.3/tests/core/r_transitive_reflexive_closure.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/generator/delivery/CMakeLists.txt` & `dlplan-0.2.3/tests/generator/delivery/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/generator/delivery/delivery.cpp` & `dlplan-0.2.3/tests/generator/delivery/delivery.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/novelty/gripper/CMakeLists.txt` & `dlplan-0.2.3/tests/novelty/gripper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/novelty/gripper/domain.pddl` & `dlplan-0.2.3/tests/novelty/gripper/domain.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/novelty/gripper/gripper.cpp` & `dlplan-0.2.3/tests/novelty/gripper/gripper.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/novelty/tuple_index_generator.cpp` & `dlplan-0.2.3/tests/novelty/tuple_index_generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/policy/policy_builder.cpp` & `dlplan-0.2.3/tests/policy/policy_builder.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/policy/policy_minimizer.cpp` & `dlplan-0.2.3/tests/policy/policy_minimizer.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/policy/utils.cpp` & `dlplan-0.2.3/tests/policy/utils.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/state_space/gripper/CMakeLists.txt` & `dlplan-0.2.3/tests/state_space/gripper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/state_space/gripper/domain.pddl` & `dlplan-0.2.3/tests/state_space/gripper/domain.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/state_space/spanner/CMakeLists.txt` & `dlplan-0.2.3/tests/state_space/spanner/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.1.15/tests/state_space/spanner/domain.pddl` & `dlplan-0.2.3/tests/state_space/spanner/domain.pddl`

 * *Files identical despite different names*


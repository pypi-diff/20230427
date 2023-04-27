# Comparing `tmp/spatialpy-1.2.1.tar.gz` & `tmp/spatialpy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SpatialPy/SpatialPy/dist/.tmp-p4t2uwbg/spatialpy-1.2.1.tar", last modified: Wed Mar  1 20:57:11 2023, max compression
+gzip compressed data, was "/home/runner/work/SpatialPy/SpatialPy/dist/.tmp-u95lv5db/spatialpy-1.2.2.tar", last modified: Thu Apr 27 20:31:58 2023, max compression
```

## Comparing `spatialpy-1.2.1.tar` & `spatialpy-1.2.2.tar`

### file list

```diff
@@ -1,151 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-01 20:56:58.000000 spatialpy-1.2.1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-01 20:56:58.000000 spatialpy-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-01 20:56:58.000000 spatialpy-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-03-01 20:57:11.000000 spatialpy-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-03-01 20:56:58.000000 spatialpy-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-01 20:56:59.000000 spatialpy-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-01 20:57:11.000000 spatialpy-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-03-01 20:56:59.000000 spatialpy-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/boundarycondition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/datafunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    51067 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/initialcondition.py
--rw-r--r--   0 runner    (1001) docker     (123)    37573 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    42753 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    38913 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/spatialpyerror.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/species.py
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/timespan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/core/vtkreader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26703 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/build_expression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/build/SConstruct
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1630 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Copyright.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    25014 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/License.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2700 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/Ann.sln
--rwxr-xr-x   0 runner    (1001) docker     (123)     2278 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/ann2fig/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4356 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/ann2fig/ann2fig.vcproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/dll/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14366 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/dll/dll.vcproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/sample/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6200 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/sample/sample.vcproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6851 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/test/test.vcproj
--rwxr-xr-x   0 runner    (1001) docker     (123)     5199 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Make-config
--rwxr-xr-x   0 runner    (1001) docker     (123)     4617 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     2614 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ReadMe.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ann2fig/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2919 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ann2fig/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)    22094 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ann2fig/ann2fig.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/doc/
--rwxr-xr-x   0 runner    (1001) docker     (123)   357854 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/doc/ANNmanual.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35654 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANN.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     8426 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANNperf.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     6497 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANNx.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3232 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     6939 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/ann_sample.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/data.pts
--rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/query.pts
--rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/sample.save
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6747 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/ANN.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     3894 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/SConscript
--rwxr-xr-x   0 runner    (1001) docker     (123)     2766 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_fix_rad_search.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     2793 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_pr_search.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_search.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    16641 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_tree.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4065 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_tree.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4202 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/brute.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    17117 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_dump.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7512 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_fix_rad_search.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1842 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_fix_rad_search.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     9128 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_pr_search.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     2076 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_pr_search.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_search.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     2097 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_search.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    17306 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_split.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     3798 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_split.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    15691 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_tree.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     8183 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_tree.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    15514 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_util.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4875 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_util.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5499 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/perf.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4620 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/pr_queue.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4524 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/pr_queue_k.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3379 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)    64523 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/ann_test.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    23218 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/rand.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/rand.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test1-data.pts
--rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test1-query.pts
--rwxr-xr-x   0 runner    (1001) docker     (123)      270 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test1.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     2916 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test1.save
--rwxr-xr-x   0 runner    (1001) docker     (123)   380197 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2-data.pts
--rwxr-xr-x   0 runner    (1001) docker     (123)     7607 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2-query.pts
--rwxr-xr-x   0 runner    (1001) docker     (123)      387 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     6739 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2.save
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/NRMConstant_v5.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/count_cores.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/particle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/particle_system.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/propensities.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/pthread_barrier.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/read_lammps_input_file.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/simulate.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/simulate_rdme.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/propensity_file_template.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/NRMConstant_v5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/SConscript
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/count_cores.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/output.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/particle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/pthread_barrier.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/read_lammps_input_file.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate_rdme.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate_threads.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27206 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/solvers/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy/stochss/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/stochss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-03-01 20:56:59.000000 spatialpy-1.2.1/spatialpy/stochss/stochss_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-01 20:57:11.000000 spatialpy-1.2.1/spatialpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:57:11.000000 spatialpy-1.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-01 20:56:59.000000 spatialpy-1.2.1/test/test_mincde.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-03-01 20:56:59.000000 spatialpy-1.2.1/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-03-01 20:56:59.000000 spatialpy-1.2.1/test/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-03-01 20:56:59.000000 spatialpy-1.2.1/test/test_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-27 20:31:35.000000 spatialpy-1.2.2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 20:31:35.000000 spatialpy-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-27 20:31:35.000000 spatialpy-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-27 20:31:58.000000 spatialpy-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-04-27 20:31:35.000000 spatialpy-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 20:31:36.000000 spatialpy-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 20:31:58.000000 spatialpy-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-27 20:31:36.000000 spatialpy-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/boundarycondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/datafunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51067 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/initialcondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37573 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42753 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38913 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/spatialpyerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/species.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/timespan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/core/vtkreader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26703 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/build_expression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/build/SConstruct
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1630 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Copyright.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25014 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/License.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2700 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/Ann.sln
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2278 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/ann2fig/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4356 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/ann2fig/ann2fig.vcproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/dll/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14366 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/dll/dll.vcproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/sample/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6200 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/sample/sample.vcproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6851 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/test/test.vcproj
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5199 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Make-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4617 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2614 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ReadMe.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ann2fig/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2919 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ann2fig/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22094 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ann2fig/ann2fig.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/doc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   357854 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/doc/ANNmanual.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35654 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANN.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8426 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANNperf.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6497 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANNx.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3232 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6939 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/ann_sample.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/data.pts
+-rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/query.pts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/sample.save
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6747 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/ANN.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3894 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/SConscript
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2766 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_fix_rad_search.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2793 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_pr_search.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_search.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16641 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_tree.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4065 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_tree.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4202 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/brute.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17117 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_dump.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7512 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_fix_rad_search.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1842 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_fix_rad_search.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9128 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_pr_search.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2076 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_pr_search.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_search.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2097 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_search.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17306 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_split.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3798 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_split.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15691 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_tree.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8183 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_tree.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15514 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_util.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4875 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_util.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5499 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/perf.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4620 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/pr_queue.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4524 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/pr_queue_k.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3379 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64523 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/ann_test.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23218 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/rand.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/rand.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test1-data.pts
+-rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test1-query.pts
+-rwxr-xr-x   0 runner    (1001) docker     (123)      270 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test1.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2916 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test1.save
+-rwxr-xr-x   0 runner    (1001) docker     (123)   380197 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2-data.pts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7607 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2-query.pts
+-rwxr-xr-x   0 runner    (1001) docker     (123)      387 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6739 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2.save
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/NRMConstant_v5.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/count_cores.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/particle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/particle_system.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/propensities.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/pthread_barrier.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/read_lammps_input_file.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/simulate.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/simulate_rdme.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/propensity_file_template.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/NRMConstant_v5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/SConscript
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/count_cores.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/output.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/particle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/pthread_barrier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/read_lammps_input_file.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate_rdme.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate_threads.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27206 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/solvers/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy/stochss/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/stochss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-04-27 20:31:36.000000 spatialpy-1.2.2/spatialpy/stochss/stochss_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 20:31:58.000000 spatialpy-1.2.2/spatialpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/test/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/integration_tests/test_mincde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/integration_tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/integration_tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/integration_tests/test_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/ioperformance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/models/birth_death.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/models/cylinder_demo3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/models/mincde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/models/mincde_5r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/run_integration_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/run_system_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1924 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/run_unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/test/system_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/system_tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/system_tests/test_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:58.000000 spatialpy-1.2.2/test/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/unit_tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51977 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/unit_tests/test_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/unit_tests/test_species.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17303 2023-04-27 20:31:36.000000 spatialpy-1.2.2/test/unit_tests/test_timespan.py
```

### Comparing `spatialpy-1.2.1/COPYRIGHT` & `spatialpy-1.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/LICENSE` & `spatialpy-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/PKG-INFO` & `spatialpy-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialpy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python Interface for Spatial Stochastic Biochemical Simulations
 Home-page: https://spatialpy.github.io/SpatialPy/
 Download-URL: https://github.com/StochSS/SpatialPy/tarball/main/
 Author: See AUTHORS
 Author-email: bdrawert@unca.edu
 Maintainer: See AUTHORS
 Maintainer-email: bdrawert@unca.edu
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spatialpy Version: 1.2.1 Summary: Python Interface
+Metadata-Version: 2.1 Name: spatialpy Version: 1.2.2 Summary: Python Interface
 for Spatial Stochastic Biochemical Simulations Home-page: https://
 spatialpy.github.io/SpatialPy/ Download-URL: https://github.com/StochSS/
 SpatialPy/tarball/main/ Author: See AUTHORS Author-email: bdrawert@unca.edu
 Maintainer: See AUTHORS Maintainer-email: bdrawert@unca.edu License: GPL-3.0-
 only Project-URL: Tracker, https://github.com/StochSS/SpatialPy/issues Project-
 URL: Source, https://github.com/StochSS/SpatialPy Keywords: biochemical
 simulation,Gillespie algorithm,stochastic simulation,biology,spatial
```

### Comparing `spatialpy-1.2.1/README.md` & `spatialpy-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/setup.py` & `spatialpy-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/__init__.py` & `spatialpy-1.2.2/spatialpy/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/__version__.py` & `spatialpy-1.2.2/spatialpy/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # =============================================================================
 # @file    __version__.py
 # @brief   SpatialPy version info
 # @license Please see the file named LICENSE in the project directory
 # @website https://github.com/StochSS/SpatialPy
 # =============================================================================
 
-__version__      = '1.2.1'
+__version__      = '1.2.2'
 __title__        = 'SpatialPy'
 __description__  = 'Python Interface for Spatial Stochastic Biochemical Simulations'
 __url__          = 'https://spatialpy.github.io/SpatialPy/'
 __download_url__ = 'https://github.com/StochSS/SpatialPy/tarball/main/'
 __author__       = 'See AUTHORS'
 __email__        = 'bdrawert@unca.edu'
 __license__      = 'GPL-3.0-only'
```

### Comparing `spatialpy-1.2.1/spatialpy/core/__init__.py` & `spatialpy-1.2.2/spatialpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/boundarycondition.py` & `spatialpy-1.2.2/spatialpy/core/boundarycondition.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/cleanup.py` & `spatialpy-1.2.2/spatialpy/core/cleanup.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/datafunction.py` & `spatialpy-1.2.2/spatialpy/core/datafunction.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/domain.py` & `spatialpy-1.2.2/spatialpy/core/domain.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/geometry.py` & `spatialpy-1.2.2/spatialpy/core/geometry.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/initialcondition.py` & `spatialpy-1.2.2/spatialpy/core/initialcondition.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/lattice.py` & `spatialpy-1.2.2/spatialpy/core/lattice.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/model.py` & `spatialpy-1.2.2/spatialpy/core/model.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/parameter.py` & `spatialpy-1.2.2/spatialpy/core/parameter.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/reaction.py` & `spatialpy-1.2.2/spatialpy/core/reaction.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/result.py` & `spatialpy-1.2.2/spatialpy/core/result.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/spatialpyerror.py` & `spatialpy-1.2.2/spatialpy/core/spatialpyerror.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/species.py` & `spatialpy-1.2.2/spatialpy/core/species.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/timespan.py` & `spatialpy-1.2.2/spatialpy/core/timespan.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/transformation.py` & `spatialpy-1.2.2/spatialpy/core/transformation.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/visualization.py` & `spatialpy-1.2.2/spatialpy/core/visualization.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/core/vtkreader.py` & `spatialpy-1.2.2/spatialpy/core/vtkreader.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/__init__.py` & `spatialpy-1.2.2/spatialpy/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/build_expression.py` & `spatialpy-1.2.2/spatialpy/solvers/build_expression.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/build/SConstruct` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/build/SConstruct`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Copyright.txt` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Copyright.txt`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/License.txt` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/License.txt`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/Ann.sln` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/Ann.sln`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/Makefile` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/Makefile`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/ann2fig/ann2fig.vcproj` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/ann2fig/ann2fig.vcproj`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/dll/dll.vcproj` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/dll/dll.vcproj`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/sample/sample.vcproj` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/sample/sample.vcproj`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/test/test.vcproj` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/MS_Win32/test/test.vcproj`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Make-config` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Make-config`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Makefile` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/Makefile`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ReadMe.txt` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ann2fig/Makefile` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ann2fig/Makefile`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ann2fig/ann2fig.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/ann2fig/ann2fig.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/doc/ANNmanual.pdf` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/doc/ANNmanual.pdf`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANN.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANN.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANNperf.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANNperf.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANNx.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/include/ANN/ANNx.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/Makefile` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/Makefile`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/ann_sample.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/ann_sample.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/sample.save` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/sample/sample.save`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/ANN.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/ANN.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/Makefile` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/Makefile`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_fix_rad_search.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_fix_rad_search.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_pr_search.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_pr_search.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_search.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_search.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_tree.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_tree.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_tree.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/bd_tree.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/brute.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/brute.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_dump.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_dump.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_fix_rad_search.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_fix_rad_search.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_fix_rad_search.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_fix_rad_search.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_pr_search.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_pr_search.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_pr_search.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_pr_search.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_search.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_search.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_search.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_search.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_split.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_split.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_split.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_split.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_tree.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_tree.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_tree.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_tree.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_util.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_util.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_util.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/kd_util.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/perf.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/perf.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/pr_queue.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/pr_queue.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/pr_queue_k.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/src/pr_queue_k.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/Makefile` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/Makefile`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/ann_test.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/ann_test.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/rand.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/rand.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/rand.h` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/rand.h`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test1.save` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test1.save`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2-data.pts` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2-data.pts`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2-query.pts` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2-query.pts`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2.save` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/external/ANN/test/test2.save`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/NRMConstant_v5.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/NRMConstant_v5.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/count_cores.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/count_cores.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/model.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/model.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/output.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/output.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/particle.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/particle.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/particle_system.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/particle_system.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/propensities.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/propensities.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/pthread_barrier.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/pthread_barrier.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/read_lammps_input_file.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/read_lammps_input_file.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/simulate.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/simulate.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/simulate_rdme.hpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/include/simulate_rdme.hpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/propensity_file_template.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/propensity_file_template.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/NRMConstant_v5.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/NRMConstant_v5.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/count_cores.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/count_cores.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/model.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/model.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/output.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/output.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/particle.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/particle.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/pthread_barrier.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/pthread_barrier.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/read_lammps_input_file.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/read_lammps_input_file.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate_rdme.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate_rdme.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate_threads.cpp` & `spatialpy-1.2.2/spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate_threads.cpp`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/solvers/solver.py` & `spatialpy-1.2.2/spatialpy/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/stochss/__init__.py` & `spatialpy-1.2.2/spatialpy/stochss/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy/stochss/stochss_export.py` & `spatialpy-1.2.2/spatialpy/stochss/stochss_export.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/spatialpy.egg-info/PKG-INFO` & `spatialpy-1.2.2/spatialpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialpy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python Interface for Spatial Stochastic Biochemical Simulations
 Home-page: https://spatialpy.github.io/SpatialPy/
 Download-URL: https://github.com/StochSS/SpatialPy/tarball/main/
 Author: See AUTHORS
 Author-email: bdrawert@unca.edu
 Maintainer: See AUTHORS
 Maintainer-email: bdrawert@unca.edu
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spatialpy Version: 1.2.1 Summary: Python Interface
+Metadata-Version: 2.1 Name: spatialpy Version: 1.2.2 Summary: Python Interface
 for Spatial Stochastic Biochemical Simulations Home-page: https://
 spatialpy.github.io/SpatialPy/ Download-URL: https://github.com/StochSS/
 SpatialPy/tarball/main/ Author: See AUTHORS Author-email: bdrawert@unca.edu
 Maintainer: See AUTHORS Maintainer-email: bdrawert@unca.edu License: GPL-3.0-
 only Project-URL: Tracker, https://github.com/StochSS/SpatialPy/issues Project-
 URL: Source, https://github.com/StochSS/SpatialPy Keywords: biochemical
 simulation,Gillespie algorithm,stochastic simulation,biology,spatial
```

### Comparing `spatialpy-1.2.1/spatialpy.egg-info/SOURCES.txt` & `spatialpy-1.2.2/spatialpy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -114,11 +114,29 @@
 spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/pthread_barrier.cpp
 spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/read_lammps_input_file.cpp
 spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate.cpp
 spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate_rdme.cpp
 spatialpy/solvers/c_base/ssa_sdpd-c-simulation-engine/src/simulate_threads.cpp
 spatialpy/stochss/__init__.py
 spatialpy/stochss/stochss_export.py
-test/test_mincde.py
-test/test_model.py
-test/test_solver.py
-test/test_threads.py
+test/__init__.py
+test/ioperformance.py
+test/run_integration_tests.py
+test/run_system_tests.py
+test/run_unit_tests.py
+test/integration_tests/__init__.py
+test/integration_tests/test_mincde.py
+test/integration_tests/test_model.py
+test/integration_tests/test_solver.py
+test/integration_tests/test_threads.py
+test/models/__init__.py
+test/models/birth_death.py
+test/models/cylinder_demo3D.py
+test/models/mincde.py
+test/models/mincde_5r.py
+test/system_tests/__init__.py
+test/system_tests/test_compiler.py
+test/unit_tests/__init__.py
+test/unit_tests/test_parameter.py
+test/unit_tests/test_reaction.py
+test/unit_tests/test_species.py
+test/unit_tests/test_timespan.py
```

### Comparing `spatialpy-1.2.1/test/test_mincde.py` & `spatialpy-1.2.2/test/integration_tests/test_mincde.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/test/test_model.py` & `spatialpy-1.2.2/test/integration_tests/test_model.py`

 * *Files identical despite different names*

### Comparing `spatialpy-1.2.1/test/test_solver.py` & `spatialpy-1.2.2/test/integration_tests/test_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         self.assertEqual(len(result_list), 3)
 
     def test_solver_expressions(self):
         """
         Ensure that expression conversions to C++ result in (roughly) equivalent values as Python.
         """
         tmpdir = tempfile.mkdtemp()
-        src_path = os.path.join(os.path.dirname(__file__), "assets", "evaluate.c")
+        src_path = os.path.join(os.path.dirname(os.path.dirname(__file__)), "assets", "evaluate.c")
         exe_path = os.path.join(tmpdir, "test")
 
         def build(expr_args: "list[str]", expr_str: "str", use_bool=False):
             args = ["gcc", "-o", exe_path, src_path, "-lm"]
             expr_num = str(len(expr_args))
             expr_args = ",".join(expr_args)
             args.append(f"-DEXP{expr_num}({expr_args})=({expr_str})")
```

### Comparing `spatialpy-1.2.1/test/test_threads.py` & `spatialpy-1.2.2/test/integration_tests/test_threads.py`

 * *Files identical despite different names*


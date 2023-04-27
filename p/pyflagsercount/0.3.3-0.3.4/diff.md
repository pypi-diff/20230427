# Comparing `tmp/pyflagsercount-0.3.3.tar.gz` & `tmp/pyflagsercount-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflagsercount-0.3.3.tar", last modified: Tue Mar 28 13:29:16 2023, max compression
+gzip compressed data, was "pyflagsercount-0.3.4.tar", last modified: Thu Apr 27 13:11:24 2023, max compression
```

## Comparing `pyflagsercount-0.3.3.tar` & `pyflagsercount-0.3.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-03-28 13:29:16.508576 pyflagsercount-0.3.3/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)        0 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/.gitmodules
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      848 2023-03-23 12:35:44.000000 pyflagsercount-0.3.3/CMakeLists.txt
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      426 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/Makefile
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      564 2023-03-28 13:29:16.508576 pyflagsercount-0.3.3/PKG-INFO
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      712 2022-12-09 00:23:03.000000 pyflagsercount-0.3.3/README.md
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-03-28 13:29:16.500576 pyflagsercount-0.3.3/docs/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)   185566 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/docs/documentation_flagser.pdf
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)    13697 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/docs/documentation_flagser.tex
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-03-28 13:29:16.500576 pyflagsercount-0.3.3/include/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)    15216 2023-03-28 13:26:53.000000 pyflagsercount-0.3.3/include/argparser.h
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     5293 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/include/cnpy.h
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     1480 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/include/definitions.h
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)    12699 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/include/directed_flag_complex.h
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     4619 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/include/directed_graph.h
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     5066 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/include/input.h
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-03-28 13:29:16.504576 pyflagsercount-0.3.3/pyflagsercount/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      120 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/pyflagsercount/__init__.py
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-03-28 13:29:16.504576 pyflagsercount-0.3.3/pyflagsercount/__pycache__/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      308 2023-03-23 12:40:00.000000 pyflagsercount-0.3.3/pyflagsercount/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     2623 2023-03-23 12:40:00.000000 pyflagsercount-0.3.3/pyflagsercount/__pycache__/flagser_functions.cpython-38.pyc
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     3903 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/pyflagsercount/flagser_functions.py
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-03-28 13:29:16.504576 pyflagsercount-0.3.3/pyflagsercount.egg-info/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      564 2023-03-28 13:29:16.000000 pyflagsercount-0.3.3/pyflagsercount.egg-info/PKG-INFO
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     1058 2023-03-28 13:29:16.000000 pyflagsercount-0.3.3/pyflagsercount.egg-info/SOURCES.txt
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)        1 2023-03-28 13:29:16.000000 pyflagsercount-0.3.3/pyflagsercount.egg-info/dependency_links.txt
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)        1 2023-03-23 12:44:14.000000 pyflagsercount-0.3.3/pyflagsercount.egg-info/not-zip-safe
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       14 2023-03-28 13:29:16.000000 pyflagsercount-0.3.3/pyflagsercount.egg-info/requires.txt
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       15 2023-03-28 13:29:16.000000 pyflagsercount-0.3.3/pyflagsercount.egg-info/top_level.txt
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-03-28 13:29:16.504576 pyflagsercount-0.3.3/scripts/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     1169 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/scripts/binary2simplex.py
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     1604 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/scripts/binary2simplex_analysis.py
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      658 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/scripts/parse_progress.py
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       38 2023-03-28 13:29:16.508576 pyflagsercount-0.3.3/setup.cfg
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     3637 2023-03-28 13:27:48.000000 pyflagsercount-0.3.3/setup.py
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-03-28 13:29:16.504576 pyflagsercount-0.3.3/src/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     5178 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/src/flagser-count-individ.cpp
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     4687 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/src/flagser-count.cpp
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     5556 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/src/flagser_count_bindings.cpp
-drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-03-28 13:29:16.508576 pyflagsercount-0.3.3/test/
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       52 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/test/A.flag
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       36 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/test/B.edges
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       71 2023-03-28 13:28:05.000000 pyflagsercount-0.3.3/test/B.out
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       21 2023-03-28 13:28:05.000000 pyflagsercount-0.3.3/test/B0.simplices
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       21 2023-03-28 13:28:05.000000 pyflagsercount-0.3.3/test/B1.simplices
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       45 2023-03-28 13:28:05.000000 pyflagsercount-0.3.3/test/C.cliques
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       48 2023-03-28 13:28:05.000000 pyflagsercount-0.3.3/test/C0.binary
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       40 2023-03-28 13:28:05.000000 pyflagsercount-0.3.3/test/C1.binary
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      164 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/test/C_col.npy
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      164 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/test/C_row.npy
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      296 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/test/D_indices.npy
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      464 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/test/D_indices64.npy
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      160 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/test/D_indptr.npy
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      192 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/test/D_indptr64.npy
--rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     3217 2022-12-08 20:06:18.000000 pyflagsercount-0.3.3/test/run_test.py
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-04-27 13:11:24.747718 pyflagsercount-0.3.4/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)        0 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/.gitmodules
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      848 2023-03-23 12:35:44.000000 pyflagsercount-0.3.4/CMakeLists.txt
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      426 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/Makefile
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      564 2023-04-27 13:11:24.747718 pyflagsercount-0.3.4/PKG-INFO
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      712 2022-12-09 00:23:03.000000 pyflagsercount-0.3.4/README.md
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-04-27 13:11:24.743718 pyflagsercount-0.3.4/docs/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)   185566 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/docs/documentation_flagser.pdf
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)    13697 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/docs/documentation_flagser.tex
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-04-27 13:11:24.747718 pyflagsercount-0.3.4/include/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)    15216 2023-03-28 13:26:53.000000 pyflagsercount-0.3.4/include/argparser.h
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     5293 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/include/cnpy.h
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     1480 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/include/definitions.h
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)    12699 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/include/directed_flag_complex.h
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     4619 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/include/directed_graph.h
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     5066 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/include/input.h
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-04-27 13:11:24.747718 pyflagsercount-0.3.4/pyflagsercount/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      120 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/pyflagsercount/__init__.py
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-04-27 13:11:24.747718 pyflagsercount-0.3.4/pyflagsercount/__pycache__/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      308 2023-03-23 12:40:00.000000 pyflagsercount-0.3.4/pyflagsercount/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     2623 2023-03-23 12:40:00.000000 pyflagsercount-0.3.4/pyflagsercount/__pycache__/flagser_functions.cpython-38.pyc
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     3903 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/pyflagsercount/flagser_functions.py
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-04-27 13:11:24.747718 pyflagsercount-0.3.4/pyflagsercount.egg-info/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      564 2023-04-27 13:11:24.000000 pyflagsercount-0.3.4/pyflagsercount.egg-info/PKG-INFO
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     1058 2023-04-27 13:11:24.000000 pyflagsercount-0.3.4/pyflagsercount.egg-info/SOURCES.txt
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)        1 2023-04-27 13:11:24.000000 pyflagsercount-0.3.4/pyflagsercount.egg-info/dependency_links.txt
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)        1 2023-03-23 12:44:14.000000 pyflagsercount-0.3.4/pyflagsercount.egg-info/not-zip-safe
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       27 2023-04-27 13:11:24.000000 pyflagsercount-0.3.4/pyflagsercount.egg-info/requires.txt
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       15 2023-04-27 13:11:24.000000 pyflagsercount-0.3.4/pyflagsercount.egg-info/top_level.txt
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-04-27 13:11:24.747718 pyflagsercount-0.3.4/scripts/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     1169 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/scripts/binary2simplex.py
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     1604 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/scripts/binary2simplex_analysis.py
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      658 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/scripts/parse_progress.py
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       38 2023-04-27 13:11:24.747718 pyflagsercount-0.3.4/setup.cfg
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     3652 2023-04-27 13:10:04.000000 pyflagsercount-0.3.4/setup.py
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-04-27 13:11:24.747718 pyflagsercount-0.3.4/src/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     5178 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/src/flagser-count-individ.cpp
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     4687 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/src/flagser-count.cpp
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     5556 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/src/flagser_count_bindings.cpp
+drwxrwxr-x   0 phys3smithj  (1001) phys3smithj  (1001)        0 2023-04-27 13:11:24.747718 pyflagsercount-0.3.4/test/
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       52 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/test/A.flag
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       36 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/test/B.edges
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       71 2023-03-28 13:28:05.000000 pyflagsercount-0.3.4/test/B.out
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       21 2023-03-28 13:28:05.000000 pyflagsercount-0.3.4/test/B0.simplices
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       21 2023-03-28 13:28:05.000000 pyflagsercount-0.3.4/test/B1.simplices
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       45 2023-03-28 13:28:05.000000 pyflagsercount-0.3.4/test/C.cliques
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       48 2023-03-28 13:28:05.000000 pyflagsercount-0.3.4/test/C0.binary
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)       40 2023-03-28 13:28:05.000000 pyflagsercount-0.3.4/test/C1.binary
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      164 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/test/C_col.npy
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      164 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/test/C_row.npy
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      296 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/test/D_indices.npy
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      464 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/test/D_indices64.npy
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      160 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/test/D_indptr.npy
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)      192 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/test/D_indptr64.npy
+-rw-rw-r--   0 phys3smithj  (1001) phys3smithj  (1001)     3217 2022-12-08 20:06:18.000000 pyflagsercount-0.3.4/test/run_test.py
```

### Comparing `pyflagsercount-0.3.3/CMakeLists.txt` & `pyflagsercount-0.3.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/PKG-INFO` & `pyflagsercount-0.3.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: pyflagsercount
-Version: 0.3.3
+Version: 0.3.4
 Summary: A package for counting directed cliques in directed graphs
 Home-page: https://github.com/JasonPSmith/flagser-count
 Author: Jason P. Smith
 Author-email: jasonsmith.bath@gmail.com
 License: UNKNOWN
 Description: A program for counting directed cliques in directed graphs, adapted from https://github.com/luetge/flagser
```

### Comparing `pyflagsercount-0.3.3/README.md` & `pyflagsercount-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/docs/documentation_flagser.pdf` & `pyflagsercount-0.3.4/docs/documentation_flagser.pdf`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/docs/documentation_flagser.tex` & `pyflagsercount-0.3.4/docs/documentation_flagser.tex`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/include/argparser.h` & `pyflagsercount-0.3.4/include/argparser.h`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/include/cnpy.h` & `pyflagsercount-0.3.4/include/cnpy.h`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/include/definitions.h` & `pyflagsercount-0.3.4/include/definitions.h`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/include/directed_flag_complex.h` & `pyflagsercount-0.3.4/include/directed_flag_complex.h`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/include/directed_graph.h` & `pyflagsercount-0.3.4/include/directed_graph.h`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/include/input.h` & `pyflagsercount-0.3.4/include/input.h`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/pyflagsercount/__pycache__/flagser_functions.cpython-38.pyc` & `pyflagsercount-0.3.4/pyflagsercount/__pycache__/flagser_functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/pyflagsercount/flagser_functions.py` & `pyflagsercount-0.3.4/pyflagsercount/flagser_functions.py`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/pyflagsercount.egg-info/PKG-INFO` & `pyflagsercount-0.3.4/pyflagsercount.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: pyflagsercount
-Version: 0.3.3
+Version: 0.3.4
 Summary: A package for counting directed cliques in directed graphs
 Home-page: https://github.com/JasonPSmith/flagser-count
 Author: Jason P. Smith
 Author-email: jasonsmith.bath@gmail.com
 License: UNKNOWN
 Description: A program for counting directed cliques in directed graphs, adapted from https://github.com/luetge/flagser
```

### Comparing `pyflagsercount-0.3.3/pyflagsercount.egg-info/SOURCES.txt` & `pyflagsercount-0.3.4/pyflagsercount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/scripts/binary2simplex.py` & `pyflagsercount-0.3.4/scripts/binary2simplex.py`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/scripts/binary2simplex_analysis.py` & `pyflagsercount-0.3.4/scripts/binary2simplex_analysis.py`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/scripts/parse_progress.py` & `pyflagsercount-0.3.4/scripts/parse_progress.py`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/setup.py` & `pyflagsercount-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,19 +71,19 @@
         if not os.path.exists(self.build_temp):
             os.makedirs(self.build_temp)
         subprocess.check_call(['cmake', ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call(['cmake', '--build', '.'] + build_args, cwd=self.build_temp)
 
 setup(
     name='pyflagsercount',
-    version='0.3.3',
+    version='0.3.4',
     author='Jason P. Smith',
     author_email='jasonsmith.bath@gmail.com',
     description='A package for counting directed cliques in directed graphs',
     long_description= 'A program for counting directed cliques in directed graphs, adapted from https://github.com/luetge/flagser\n\nOfficial source code repo: https://github.com/JasonPSmith/flagser-count\n\nRequirements: numpy ≥ 1.17.0 and cmake version ≥ 3.9.',
     url='https://github.com/JasonPSmith/flagser-count',
     ext_modules=[CMakeExtension('pyflagsercount')],
     cmdclass=dict(build_ext=CMakeBuild),
     packages=["pyflagsercount"],
-    install_requires=['numpy>=1.17.0'],
+    install_requires=['numpy>=1.17.0','cmake>=3.9.0'],
     zip_safe=False,
 )
```

### Comparing `pyflagsercount-0.3.3/src/flagser-count-individ.cpp` & `pyflagsercount-0.3.4/src/flagser-count-individ.cpp`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/src/flagser-count.cpp` & `pyflagsercount-0.3.4/src/flagser-count.cpp`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/src/flagser_count_bindings.cpp` & `pyflagsercount-0.3.4/src/flagser_count_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyflagsercount-0.3.3/test/run_test.py` & `pyflagsercount-0.3.4/test/run_test.py`

 * *Files identical despite different names*

